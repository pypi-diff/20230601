# Comparing `tmp/jupyternb-setup-1.3.4rc2.tar.gz` & `tmp/jupyternb-setup-1.3.4rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyternb-setup-1.3.4rc2.tar", last modified: Thu Jun  1 18:20:32 2023, max compression
+gzip compressed data, was "jupyternb-setup-1.3.4rc3.tar", last modified: Thu Jun  1 18:23:49 2023, max compression
```

## Comparing `jupyternb-setup-1.3.4rc2.tar` & `jupyternb-setup-1.3.4rc3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1806 2023-06-01 18:13:01.086115 jupyternb-setup-1.3.4rc2/.gitignore
--rw-r--r--   0        0        0     1071 2023-06-01 17:22:55.849765 jupyternb-setup-1.3.4rc2/LICENSE
--rw-r--r--   0        0        0     4667 2023-06-01 17:22:55.850054 jupyternb-setup-1.3.4rc2/README.md
--rw-r--r--   0        0        0       51 2023-06-01 18:20:21.490180 jupyternb-setup-1.3.4rc2/jupyternb/__init__.py
--rw-r--r--   0        0        0    15308 2023-06-01 18:04:49.632842 jupyternb-setup-1.3.4rc2/jupyternb/jupyter_startup.py
--rw-r--r--   0        0        0      987 2023-06-01 18:20:18.619300 jupyternb-setup-1.3.4rc2/pyproject.toml
--rw-r--r--   0        0        0     5368 1970-01-01 00:00:00.000000 jupyternb-setup-1.3.4rc2/PKG-INFO
+-rw-r--r--   0        0        0     1806 2023-06-01 18:13:01.086115 jupyternb-setup-1.3.4rc3/.gitignore
+-rw-r--r--   0        0        0     1071 2023-06-01 17:22:55.849765 jupyternb-setup-1.3.4rc3/LICENSE
+-rw-r--r--   0        0        0     4667 2023-06-01 17:22:55.850054 jupyternb-setup-1.3.4rc3/README.md
+-rw-r--r--   0        0        0       51 2023-06-01 18:22:07.945162 jupyternb-setup-1.3.4rc3/jupyternb/__init__.py
+-rw-r--r--   0        0        0    15366 2023-06-01 18:23:17.264441 jupyternb-setup-1.3.4rc3/jupyternb/jupyter_startup.py
+-rw-r--r--   0        0        0      977 2023-06-01 18:23:33.328333 jupyternb-setup-1.3.4rc3/pyproject.toml
+-rw-r--r--   0        0        0     5368 1970-01-01 00:00:00.000000 jupyternb-setup-1.3.4rc3/PKG-INFO
```

### Comparing `jupyternb-setup-1.3.4rc2/.gitignore` & `jupyternb-setup-1.3.4rc3/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyternb-setup-1.3.4rc2/LICENSE` & `jupyternb-setup-1.3.4rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyternb-setup-1.3.4rc2/README.md` & `jupyternb-setup-1.3.4rc3/README.md`

 * *Files identical despite different names*

### Comparing `jupyternb-setup-1.3.4rc2/jupyternb/jupyter_startup.py` & `jupyternb-setup-1.3.4rc3/jupyternb/jupyter_startup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 #
 # Author: Komal Thareja (kthare10@renci.org)
 import json
 import os
-import stat
 import traceback
 from datetime import datetime
 
 from fss_utils.sshkey import FABRICSSHKey
 from atomicwrites import atomic_write
 import wget
 import tarfile
@@ -344,11 +343,17 @@
         os.chmod(default_slice_priv_key_config, 0o600)
         os.chmod(default_slice_pub_key_config, 0o644)
 
         self.update_permissions()
         self.custom_install_packages()
 
 
+class Main:
+    @staticmethod
+    def run():
+        js = JupyterStartup()
+        js.initialize()
+
+
 if __name__ == "__main__":
-    js = JupyterStartup()
-    js.initialize()
+    Main.run()
```

### Comparing `jupyternb-setup-1.3.4rc2/pyproject.toml` & `jupyternb-setup-1.3.4rc3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
                "License :: OSI Approved :: MIT License",
                "Operating System :: OS Independent"]
 description = "Fabric Jupyter Notebook Container Setup"
 dynamic = ["version"]
 
 keywords = ["Fabric Jupyter Notebook Container Setup", "Jupyter Hub", "Jupyter Notebook"]
 
-scripts = {"jupyter-startup" = "jupyternb.jupyter_startup:JupyterStartup.initialize"}
+scripts = {"fabric-jupyter-startup" = "jupyternb.jupyter_startup:Main.run"}
 
 requires-python = '>=3.9'
 dependencies = ["nbgitpuller",
                 "fabric_fss_utils",
                 "atomicwrites",
                 "gitpython",
                 "wget"]
```

### Comparing `jupyternb-setup-1.3.4rc2/PKG-INFO` & `jupyternb-setup-1.3.4rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyternb-setup
-Version: 1.3.4rc2
+Version: 1.3.4rc3
 Summary: Fabric Jupyter Notebook Container Setup
 Keywords: Fabric Jupyter Notebook Container Setup,Jupyter Hub,Jupyter Notebook
 Author-email: Komal Thareja <kthare10@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

