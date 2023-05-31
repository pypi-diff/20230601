# Comparing `tmp/twofas-cli-0.0.1.tar.gz` & `tmp/twofas-cli-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twofas-cli-0.0.1.tar", last modified: Wed May 31 23:24:52 2023, max compression
+gzip compressed data, was "twofas-cli-0.0.2.tar", last modified: Wed May 31 23:30:41 2023, max compression
```

## Comparing `twofas-cli-0.0.1.tar` & `twofas-cli-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:24:52.049397 twofas-cli-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-31 23:24:41.000000 twofas-cli-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-31 23:24:52.049397 twofas-cli-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-31 23:24:41.000000 twofas-cli-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-31 23:24:41.000000 twofas-cli-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 23:24:52.049397 twofas-cli-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-31 23:24:41.000000 twofas-cli-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:24:52.045397 twofas-cli-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-31 23:24:41.000000 twofas-cli-0.0.1/tests/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:24:52.045397 twofas-cli-0.0.1/twofas_cli/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-31 23:24:41.000000 twofas-cli-0.0.1/twofas_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:24:52.049397 twofas-cli-0.0.1/twofas_cli/api/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-31 23:24:41.000000 twofas-cli-0.0.1/twofas_cli/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-05-31 23:24:41.000000 twofas-cli-0.0.1/twofas_cli/api/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-31 23:24:41.000000 twofas-cli-0.0.1/twofas_cli/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-31 23:24:41.000000 twofas-cli-0.0.1/twofas_cli/crypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-05-31 23:24:41.000000 twofas-cli-0.0.1/twofas_cli/twofas_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:24:52.049397 twofas-cli-0.0.1/twofas_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-31 23:24:52.000000 twofas-cli-0.0.1/twofas_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-31 23:24:52.000000 twofas-cli-0.0.1/twofas_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 23:24:52.000000 twofas-cli-0.0.1/twofas_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-31 23:24:52.000000 twofas-cli-0.0.1/twofas_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-31 23:24:52.000000 twofas-cli-0.0.1/twofas_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-31 23:24:52.000000 twofas-cli-0.0.1/twofas_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:30:41.711619 twofas-cli-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-31 23:30:31.000000 twofas-cli-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-31 23:30:41.711619 twofas-cli-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-31 23:30:31.000000 twofas-cli-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-31 23:30:31.000000 twofas-cli-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 23:30:41.711619 twofas-cli-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-31 23:30:31.000000 twofas-cli-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:30:41.711619 twofas-cli-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-31 23:30:31.000000 twofas-cli-0.0.2/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:30:41.711619 twofas-cli-0.0.2/twofas_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-31 23:30:31.000000 twofas-cli-0.0.2/twofas_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:30:41.711619 twofas-cli-0.0.2/twofas_cli/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-31 23:30:31.000000 twofas-cli-0.0.2/twofas_cli/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-05-31 23:30:31.000000 twofas-cli-0.0.2/twofas_cli/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-31 23:30:31.000000 twofas-cli-0.0.2/twofas_cli/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-31 23:30:31.000000 twofas-cli-0.0.2/twofas_cli/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-05-31 23:30:31.000000 twofas-cli-0.0.2/twofas_cli/twofas_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:30:41.711619 twofas-cli-0.0.2/twofas_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-31 23:30:41.000000 twofas-cli-0.0.2/twofas_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-31 23:30:41.000000 twofas-cli-0.0.2/twofas_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 23:30:41.000000 twofas-cli-0.0.2/twofas_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-31 23:30:41.000000 twofas-cli-0.0.2/twofas_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-31 23:30:41.000000 twofas-cli-0.0.2/twofas_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-31 23:30:41.000000 twofas-cli-0.0.2/twofas_cli.egg-info/top_level.txt
```

### Comparing `twofas-cli-0.0.1/LICENSE` & `twofas-cli-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `twofas-cli-0.0.1/PKG-INFO` & `twofas-cli-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twofas-cli
-Version: 0.0.1
+Version: 0.0.2
 Summary: Unofficial CLI tool for 2FAS using the browser extension api
 Home-page: https://packages.python.org/twofas-cli
 Author: dspd
 Author-email: inmost-chimps-0j@icloud.com
 License: BSD
 Keywords: 2fas twofas
 Classifier: Development Status :: 4 - Beta
```

### Comparing `twofas-cli-0.0.1/README.md` & `twofas-cli-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `twofas-cli-0.0.1/setup.py` & `twofas-cli-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README.md file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="twofas-cli",
-    version="0.0.1",
+    version="0.0.2",
     author="dspd",
     author_email="inmost-chimps-0j@icloud.com",
     description="Unofficial CLI tool for 2FAS using the browser extension api",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="BSD",
     keywords="2fas twofas",
```

### Comparing `twofas-cli-0.0.1/tests/test_cli.py` & `twofas-cli-0.0.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `twofas-cli-0.0.1/twofas_cli/api/api.py` & `twofas-cli-0.0.2/twofas_cli/api/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
             res.raise_for_status()
 
     @staticmethod
     def create_browser_info(name: str) -> dict:
         return {
             'name': name,
             'browser_name': '2FAS CLI',
-            'browser_version': '0.0.1',
+            'browser_version': '0.0.2',
             'public_key': get_public_key_spki()
         }
 
     def create_extension_instance(self, browser_name: str):
         res = requests.post(f'{self.api_base_url}/browser_extensions',
                             headers=self.headers,
                             data=json.dumps(self.create_browser_info(browser_name)))
```

### Comparing `twofas-cli-0.0.1/twofas_cli/common.py` & `twofas-cli-0.0.2/twofas_cli/common.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 def get_settings_dir():
     xdg_config_home = os.getenv('XDG_CONFIG_HOME')
     settings_dir = (Path(xdg_config_home) if xdg_config_home else 
                     Path.home().joinpath('.config'))\
         .joinpath('twofas-cli')
-    settings_dir.mkdir(parents=False, exist_ok=True)
+    settings_dir.mkdir(parents=True, exist_ok=True)
     return settings_dir
 
 
 def get_extension_id():
     settings_dir = get_settings_dir()
     extension_id_file = settings_dir.joinpath('extension_id')
     return extension_id_file.read_text(encoding='utf-8')
```

### Comparing `twofas-cli-0.0.1/twofas_cli/crypt.py` & `twofas-cli-0.0.2/twofas_cli/crypt.py`

 * *Files identical despite different names*

### Comparing `twofas-cli-0.0.1/twofas_cli/twofas_cli.py` & `twofas-cli-0.0.2/twofas_cli/twofas_cli.py`

 * *Files identical despite different names*

### Comparing `twofas-cli-0.0.1/twofas_cli.egg-info/PKG-INFO` & `twofas-cli-0.0.2/twofas_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twofas-cli
-Version: 0.0.1
+Version: 0.0.2
 Summary: Unofficial CLI tool for 2FAS using the browser extension api
 Home-page: https://packages.python.org/twofas-cli
 Author: dspd
 Author-email: inmost-chimps-0j@icloud.com
 License: BSD
 Keywords: 2fas twofas
 Classifier: Development Status :: 4 - Beta
```

