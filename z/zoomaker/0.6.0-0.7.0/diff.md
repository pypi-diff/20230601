# Comparing `tmp/zoomaker-0.6.0.tar.gz` & `tmp/zoomaker-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zoomaker-0.6.0.tar", max compression
+gzip compressed data, was "zoomaker-0.7.0.tar", max compression
```

## Comparing `zoomaker-0.6.0.tar` & `zoomaker-0.7.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     6710 2023-05-30 08:35:06.044965 zoomaker-0.6.0/README.md
--rw-r--r--   0        0        0      587 2023-05-31 13:30:33.057192 zoomaker-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     7123 2023-05-31 13:30:29.148792 zoomaker-0.6.0/zoomaker.py
--rw-r--r--   0        0        0     7417 1970-01-01 00:00:00.000000 zoomaker-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     7265 2023-06-01 06:47:52.245774 zoomaker-0.7.0/README.md
+-rw-r--r--   0        0        0      587 2023-06-01 08:47:31.698214 zoomaker-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     8056 2023-06-01 08:47:27.180009 zoomaker-0.7.0/zoomaker.py
+-rw-r--r--   0        0        0     7972 1970-01-01 00:00:00.000000 zoomaker-0.7.0/PKG-INFO
```

### Comparing `zoomaker-0.6.0/README.md` & `zoomaker-0.7.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -98,28 +98,43 @@
       rename_to: moebius.bin
 
   extensions:
     - name: sd-webui-tunnels
       src: https://github.com/Bing-su/sd-webui-tunnels.git
       type: git
       install_to: *extensions
+```
+</details>
+
+<details>
+<summary>`zoo.yaml` with script snippets</summary>
+
+Here are a few examples of how to run scripts snippets from the `zoo.yaml` file. For example for starting the Automatic1111's webui, you could setup snippets like these and then run them with `zoomaker run start_webui`. All scripts are run from the root of the project, please adjust the paths accordingly.
 
+```yaml
+scripts:
+  start_webui: |
+    cd .\stable-diffusion-webui && call webui.bat
+```
+
+```yaml
 scripts:
-  start: |
+  start_webui: |
+    conda activate automatic1111
     cd /home/$(whoami)/stable-diffusion-webui/
-    ./webui.sh
+    ./webui.sh --theme dark --xformers --no-half
 ```
 </details>
 
 <details>
 <summary>`zoo.yaml` with web download</summary>
 
 ```yaml
-models:
-  resources:
+resources:
+  models:
     - name: analog-diffusion-v1
       src: https://civitai.com/api/download/models/1344
       type: download
       install_to: ./stable-diffusion-webui/models/Stable-diffusion/
       rename_to: analog-diffusion-v1.safetensors
 ```
 Please note:
```

### Comparing `zoomaker-0.6.0/pyproject.toml` & `zoomaker-0.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zoomaker"
-version = "0.6.0"
+version = "0.7.0"
 description = "Zoomaker - Friendly house keeping for your AI model zoo and related resources."
 authors = ["Benedikt Groß"]
 readme = "README.md"
 homepage = "https://github.com/hfg-gmuend/zoomaker"
 documentation = "https://github.com/hfg-gmuend/zoomaker"
 repository = "https://github.com/hfg-gmuend/zoomaker"
```

### Comparing `zoomaker-0.6.0/zoomaker.py` & `zoomaker-0.7.0/zoomaker.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import subprocess
 import yaml
 import argparse
 from huggingface_hub import hf_hub_download
 import git
 import requests
 from tqdm import tqdm
+import unicodedata
+import re
 
 class Zoomaker:
     def __init__(self, yaml_file: str):
         self.yaml_file = yaml_file
         with open(yaml_file, "r") as f:
             self.data = yaml.safe_load(f)
         self._check_yaml()
@@ -83,15 +85,16 @@
                             repo.git.checkout(revision)
                             print(f"\tgit checkout revision: {repo.head.object.hexsha}")
                         else:
                             repo.remotes.origin.pull()
                             print(f"\tgit pull latest: {repo.head.object.hexsha}")
                 # Download
                 else:
-                    downloaded = self._download_file(src, os.path.join(install_to, os.path.basename(src)))
+                    filename = self._slugify(os.path.basename(src))
+                    downloaded = self._download_file(src, os.path.join(install_to, filename))
                     if rename_to:
                         self._rename_file(downloaded, os.path.join(install_to, rename_to))
                     if revision:
                         print(f"\trevision is not supported for download. Ignoring revision: {revision}")
 
         print(f"\n✅ {counter} resources installed.")
 
@@ -131,20 +134,38 @@
                 file.write(data)
         progress_bar.close()
         if total_size_in_bytes != 0 and progress_bar.n != total_size_in_bytes:
             print("Error: Failed to download the complete file.")
             return None
         return filename
 
+    def _slugify(self, value, allow_unicode=False):
+        """
+        Makes a filename safe for usage on all filesystems.
+
+        Taken from https://github.com/django/django/blob/master/django/utils/text.py
+        Convert to ASCII if 'allow_unicode' is False. Convert spaces or repeated
+        dashes to single dashes. Remove characters that aren't alphanumerics,
+        underscores, or hyphens. Convert to lowercase. Also strip leading and
+        trailing whitespace, dashes, and underscores.
+        """
+        value = str(value)
+        if allow_unicode:
+            value = unicodedata.normalize('NFKC', value)
+        else:
+            value = unicodedata.normalize('NFKD', value).encode('ascii', 'ignore').decode('ascii')
+        value = re.sub(r'[^\w\s-]', '', value.lower())
+        return re.sub(r'[-\s]+', '-', value).strip('-_')
+
 def main():
     parser = argparse.ArgumentParser(description="Install models, git repos and run scripts defined in the zoo.yaml file.")
     parser.add_argument("command", nargs="?", choices=["install", "run"], help="The command to execute.")
     parser.add_argument("script", nargs="?", help="The script name to execute.")
     parser.add_argument("--no-symlinks", action='store_true', help="Do not create symlinks for the installed resources.")
-    parser.add_argument("-v", "--version", action='version', help="The current version of the zoomaker.", version="0.6.0")
+    parser.add_argument("-v", "--version", action='version', help="The current version of the zoomaker.", version="0.7.0")
     args = parser.parse_args()
 
     if args.command == "install":
         Zoomaker("zoo.yaml").install(args.no_symlinks)
     elif args.command == "run":
         Zoomaker("zoo.yaml").run(args.script)
     else:
```

### Comparing `zoomaker-0.6.0/PKG-INFO` & `zoomaker-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zoomaker
-Version: 0.6.0
+Version: 0.7.0
 Summary: Zoomaker - Friendly house keeping for your AI model zoo and related resources.
 Home-page: https://github.com/hfg-gmuend/zoomaker
 Author: Benedikt Groß
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -115,28 +115,43 @@
       rename_to: moebius.bin
 
   extensions:
     - name: sd-webui-tunnels
       src: https://github.com/Bing-su/sd-webui-tunnels.git
       type: git
       install_to: *extensions
+```
+</details>
+
+<details>
+<summary>`zoo.yaml` with script snippets</summary>
+
+Here are a few examples of how to run scripts snippets from the `zoo.yaml` file. For example for starting the Automatic1111's webui, you could setup snippets like these and then run them with `zoomaker run start_webui`. All scripts are run from the root of the project, please adjust the paths accordingly.
+
+```yaml
+scripts:
+  start_webui: |
+    cd .\stable-diffusion-webui && call webui.bat
+```
 
+```yaml
 scripts:
-  start: |
+  start_webui: |
+    conda activate automatic1111
     cd /home/$(whoami)/stable-diffusion-webui/
-    ./webui.sh
+    ./webui.sh --theme dark --xformers --no-half
 ```
 </details>
 
 <details>
 <summary>`zoo.yaml` with web download</summary>
 
 ```yaml
-models:
-  resources:
+resources:
+  models:
     - name: analog-diffusion-v1
       src: https://civitai.com/api/download/models/1344
       type: download
       install_to: ./stable-diffusion-webui/models/Stable-diffusion/
       rename_to: analog-diffusion-v1.safetensors
 ```
 Please note:
```

