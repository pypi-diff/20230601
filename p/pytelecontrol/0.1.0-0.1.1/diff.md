# Comparing `tmp/pytelecontrol-0.1.0.tar.gz` & `tmp/pytelecontrol-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytelecontrol-0.1.0.tar", max compression
+gzip compressed data, was "pytelecontrol-0.1.1.tar", max compression
```

## Comparing `pytelecontrol-0.1.0.tar` & `pytelecontrol-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    34454 2023-06-01 13:52:35.411104 pytelecontrol-0.1.0/LICENSE
--rw-r--r--   0        0        0      229 2023-06-01 18:35:15.685483 pytelecontrol-0.1.0/README.md
--rw-r--r--   0        0        0      667 2023-06-01 20:12:47.562277 pytelecontrol-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      161 2023-06-01 16:23:26.341494 pytelecontrol-0.1.0/pytelecontrol/__init__.py
--rw-r--r--   0        0        0     1296 2023-06-01 17:06:45.135778 pytelecontrol-0.1.0/pytelecontrol/__main__.py
--rw-r--r--   0        0        0      940 1970-01-01 00:00:00.000000 pytelecontrol-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    34454 2023-06-01 13:52:35.411104 pytelecontrol-0.1.1/LICENSE
+-rw-r--r--   0        0        0      281 2023-06-01 20:36:57.046239 pytelecontrol-0.1.1/README.md
+-rw-r--r--   0        0        0      666 2023-06-01 21:02:56.819748 pytelecontrol-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      288 2023-06-01 20:43:48.895743 pytelecontrol-0.1.1/pytelecontrol/__init__.py
+-rw-r--r--   0        0        0     1294 2023-06-01 20:18:54.079503 pytelecontrol-0.1.1/pytelecontrol/__main__.py
+-rw-r--r--   0        0        0      992 1970-01-01 00:00:00.000000 pytelecontrol-0.1.1/PKG-INFO
```

### Comparing `pytelecontrol-0.1.0/LICENSE` & `pytelecontrol-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytelecontrol-0.1.0/pyproject.toml` & `pytelecontrol-0.1.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytelecontrol"
-version = "0.1.0"
+version = "0.1.1"
 description = "Remotely access to your PLC, with auto discover feature"
 authors = ["Cesar Freire <cfreire@cfreire.com.pt>", "Ricardo oliveira <ricardo.oliveira.pt@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 repository = "https://gitlab.com/xyzsoft/pytelecontrol"
 keywords = [
 	"Automation",
@@ -19,10 +19,10 @@
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 
 [tool.poetry-dynamic-versioning]
-enable = false
+enable = true
 vcs = "git"
 style = "semver"
```

### Comparing `pytelecontrol-0.1.0/pytelecontrol/__main__.py` & `pytelecontrol-0.1.1/pytelecontrol/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,22 +17,22 @@
         sys.exit(1)
 
 
 def log_setup(loglevel='INFO'):
     """Start logging write version"""
     logging.basicConfig(format=LOG_FORMAT, level=logging.INFO)
     logger = logging.getLogger(__package__)
-    logger.info(f"Starting {__package__} v{__version__}")
+    logger.info(f"Starting {__package__} {__version__}")
     logger.info(f'Changing log level to: {loglevel}')
     logger.setLevel(loglevel)
 
 
 def get_parser():
     parser = argparse.ArgumentParser(description="Remotely access to your PLC, with auto discover feature", prog=__package__)
-    parser.add_argument("--version", action="version", version=f'{__package__} v{__version__}')
+    parser.add_argument("--version", action="version", version=f'{__package__} {__version__}')
     parser.add_argument('--loglevel', default='INFO', choices=['DEBUG', 'INFO', 'WARNING', 'ERROR', 'CRITICAL'],
                         help='Set log level, Defaults to INFO')
     return parser
 
 
 if __name__ == '__main__':
     validate_python()
```

### Comparing `pytelecontrol-0.1.0/PKG-INFO` & `pytelecontrol-0.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytelecontrol
-Version: 0.1.0
+Version: 0.1.1
 Summary: Remotely access to your PLC, with auto discover feature
 Home-page: https://gitlab.com/xyzsoft/pytelecontrol
 License: GPL-3.0-or-later
 Keywords: Automation,PLC,Remote Control
 Author: Cesar Freire
 Author-email: cfreire@cfreire.com.pt
 Requires-Python: >=3.10,<4.0
@@ -25,8 +25,10 @@
 
 
 ## Maintainers
 
   * César Freire <cfreire70@gmail.com>
   * Ricardo oliveira <ricardo.oliveira.pt@gmail.com>
 
+## Running
 
+    $ poetry run python -m pytelecontrol
```

