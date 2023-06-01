# Comparing `tmp/gefyra-1.1.1.tar.gz` & `tmp/gefyra-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gefyra-1.1.1.tar", max compression
+gzip compressed data, was "gefyra-1.1.2.tar", max compression
```

## Comparing `gefyra-1.1.1.tar` & `gefyra-1.1.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     2151 2023-05-31 07:45:19.989690 gefyra-1.1.1/README.md
--rw-r--r--   0        0        0        0 2023-05-31 07:45:19.989690 gefyra-1.1.1/gefyra/__init__.py
--rw-r--r--   0        0        0    15368 2023-05-31 07:45:19.989690 gefyra-1.1.1/gefyra/__main__.py
--rw-r--r--   0        0        0      200 2023-05-31 07:45:19.989690 gefyra-1.1.1/gefyra/api/__init__.py
--rw-r--r--   0        0        0     9037 2023-05-31 07:45:19.989690 gefyra-1.1.1/gefyra/api/bridge.py
--rw-r--r--   0        0        0     1306 2023-05-31 07:45:19.989690 gefyra-1.1.1/gefyra/api/down.py
--rw-r--r--   0        0        0     1605 2023-05-31 07:45:19.989690 gefyra-1.1.1/gefyra/api/list.py
--rw-r--r--   0        0        0     2523 2023-05-31 07:45:19.989690 gefyra-1.1.1/gefyra/api/reflect.py
--rw-r--r--   0        0        0     6142 2023-05-31 07:45:19.989690 gefyra-1.1.1/gefyra/api/run.py
--rw-r--r--   0        0        0     6277 2023-05-31 07:45:19.989690 gefyra-1.1.1/gefyra/api/status.py
--rw-r--r--   0        0        0     2917 2023-05-31 07:45:19.989690 gefyra-1.1.1/gefyra/api/up.py
--rw-r--r--   0        0        0     1562 2023-05-31 07:45:19.989690 gefyra-1.1.1/gefyra/api/utils.py
--rw-r--r--   0        0        0        0 2023-05-31 07:45:19.989690 gefyra-1.1.1/gefyra/cluster/__init__.py
--rw-r--r--   0        0        0     7090 2023-05-31 07:45:19.989690 gefyra-1.1.1/gefyra/cluster/manager.py
--rw-r--r--   0        0        0     8850 2023-05-31 07:45:19.989690 gefyra-1.1.1/gefyra/cluster/resources.py
--rw-r--r--   0        0        0     3016 2023-05-31 07:45:19.989690 gefyra-1.1.1/gefyra/cluster/utils.py
--rw-r--r--   0        0        0     8650 2023-05-31 07:45:19.989690 gefyra-1.1.1/gefyra/configuration.py
--rw-r--r--   0        0        0      260 2023-05-31 07:45:19.989690 gefyra-1.1.1/gefyra/local/__init__.py
--rw-r--r--   0        0        0     6677 2023-05-31 07:45:19.989690 gefyra-1.1.1/gefyra/local/bridge.py
--rw-r--r--   0        0        0     4609 2023-05-31 07:45:19.989690 gefyra-1.1.1/gefyra/local/cargo.py
--rw-r--r--   0        0        0        0 2023-05-31 07:45:19.989690 gefyra-1.1.1/gefyra/local/cargoimage/__init__.py
--rw-r--r--   0        0        0     1098 2023-05-31 07:45:19.989690 gefyra-1.1.1/gefyra/local/cargoimage/cargo_dockerfile.py
--rw-r--r--   0        0        0     1121 2023-05-31 07:45:19.989690 gefyra-1.1.1/gefyra/local/check.py
--rw-r--r--   0        0        0     2150 2023-05-31 07:45:19.989690 gefyra-1.1.1/gefyra/local/minikube.py
--rw-r--r--   0        0        0     4300 2023-05-31 07:45:19.989690 gefyra-1.1.1/gefyra/local/networking.py
--rw-r--r--   0        0        0     3948 2023-05-31 07:45:19.989690 gefyra-1.1.1/gefyra/local/telemetry.py
--rw-r--r--   0        0        0     8109 2023-05-31 07:45:19.989690 gefyra-1.1.1/gefyra/local/utils.py
--rw-r--r--   0        0        0     1326 2023-05-31 07:45:19.989690 gefyra-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     3338 1970-01-01 00:00:00.000000 gefyra-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2151 2023-06-01 13:36:25.494723 gefyra-1.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-01 13:36:25.494723 gefyra-1.1.2/gefyra/__init__.py
+-rw-r--r--   0        0        0    15432 2023-06-01 13:36:25.494723 gefyra-1.1.2/gefyra/__main__.py
+-rw-r--r--   0        0        0      200 2023-06-01 13:36:25.494723 gefyra-1.1.2/gefyra/api/__init__.py
+-rw-r--r--   0        0        0     9037 2023-06-01 13:36:25.494723 gefyra-1.1.2/gefyra/api/bridge.py
+-rw-r--r--   0        0        0     1306 2023-06-01 13:36:25.494723 gefyra-1.1.2/gefyra/api/down.py
+-rw-r--r--   0        0        0     1605 2023-06-01 13:36:25.494723 gefyra-1.1.2/gefyra/api/list.py
+-rw-r--r--   0        0        0     2523 2023-06-01 13:36:25.494723 gefyra-1.1.2/gefyra/api/reflect.py
+-rw-r--r--   0        0        0     6142 2023-06-01 13:36:25.494723 gefyra-1.1.2/gefyra/api/run.py
+-rw-r--r--   0        0        0     6277 2023-06-01 13:36:25.494723 gefyra-1.1.2/gefyra/api/status.py
+-rw-r--r--   0        0        0     2917 2023-06-01 13:36:25.494723 gefyra-1.1.2/gefyra/api/up.py
+-rw-r--r--   0        0        0     1562 2023-06-01 13:36:25.494723 gefyra-1.1.2/gefyra/api/utils.py
+-rw-r--r--   0        0        0        0 2023-06-01 13:36:25.494723 gefyra-1.1.2/gefyra/cluster/__init__.py
+-rw-r--r--   0        0        0     7090 2023-06-01 13:36:25.494723 gefyra-1.1.2/gefyra/cluster/manager.py
+-rw-r--r--   0        0        0     8850 2023-06-01 13:36:25.494723 gefyra-1.1.2/gefyra/cluster/resources.py
+-rw-r--r--   0        0        0     3016 2023-06-01 13:36:25.494723 gefyra-1.1.2/gefyra/cluster/utils.py
+-rw-r--r--   0        0        0     8650 2023-06-01 13:36:25.494723 gefyra-1.1.2/gefyra/configuration.py
+-rw-r--r--   0        0        0      260 2023-06-01 13:36:25.494723 gefyra-1.1.2/gefyra/local/__init__.py
+-rw-r--r--   0        0        0     6677 2023-06-01 13:36:25.494723 gefyra-1.1.2/gefyra/local/bridge.py
+-rw-r--r--   0        0        0     4609 2023-06-01 13:36:25.494723 gefyra-1.1.2/gefyra/local/cargo.py
+-rw-r--r--   0        0        0        0 2023-06-01 13:36:25.494723 gefyra-1.1.2/gefyra/local/cargoimage/__init__.py
+-rw-r--r--   0        0        0     1098 2023-06-01 13:36:25.494723 gefyra-1.1.2/gefyra/local/cargoimage/cargo_dockerfile.py
+-rw-r--r--   0        0        0     1121 2023-06-01 13:36:25.494723 gefyra-1.1.2/gefyra/local/check.py
+-rw-r--r--   0        0        0     2150 2023-06-01 13:36:25.494723 gefyra-1.1.2/gefyra/local/minikube.py
+-rw-r--r--   0        0        0     4300 2023-06-01 13:36:25.494723 gefyra-1.1.2/gefyra/local/networking.py
+-rw-r--r--   0        0        0     3948 2023-06-01 13:36:25.494723 gefyra-1.1.2/gefyra/local/telemetry.py
+-rw-r--r--   0        0        0     8109 2023-06-01 13:36:25.494723 gefyra-1.1.2/gefyra/local/utils.py
+-rw-r--r--   0        0        0     1326 2023-06-01 13:36:25.494723 gefyra-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3338 1970-01-01 00:00:00.000000 gefyra-1.1.2/PKG-INFO
```

### Comparing `gefyra-1.1.1/README.md` & `gefyra-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `gefyra-1.1.1/gefyra/__main__.py` & `gefyra-1.1.2/gefyra/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
     "--expose",
     help="Exposes ports from k8s container spec to host",
     required=False,
     default=True,
     action="store_false",
 )
 reflect_parser.add_argument(
-    "-i", "--image", help="The docker image to run in Gefyra", required=True
+    "-i", "--image", help="The docker image to run in Gefyra", required=False
 )
 reflect_parser.add_argument(
     "-v",
     "--volume",
     action="append",
     help="Bind mount a volume into the container in notation src:dest, allowed multiple times",
     required=False,
@@ -491,14 +491,15 @@
             down(config=configuration)
         elif args.action == "status":
             _status = status(config=configuration)
             print_status(_status)
         elif args.action == "check":
             probe_docker()
             probe_kubernetes(config=configuration)
+            version(config=configuration_package, check=False)
         elif args.action == "telemetry":
             telemetry_command(on=args.on, off=args.off)
         else:
             parser.print_help()
     except KeyboardInterrupt:
         logger.warning("Program interrupted by user. Exiting...")
         exit(1)
```

### Comparing `gefyra-1.1.1/gefyra/api/bridge.py` & `gefyra-1.1.2/gefyra/api/bridge.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.1.1/gefyra/api/down.py` & `gefyra-1.1.2/gefyra/api/down.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.1.1/gefyra/api/list.py` & `gefyra-1.1.2/gefyra/api/list.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.1.1/gefyra/api/reflect.py` & `gefyra-1.1.2/gefyra/api/reflect.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.1.1/gefyra/api/run.py` & `gefyra-1.1.2/gefyra/api/run.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.1.1/gefyra/api/status.py` & `gefyra-1.1.2/gefyra/api/status.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.1.1/gefyra/api/up.py` & `gefyra-1.1.2/gefyra/api/up.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.1.1/gefyra/api/utils.py` & `gefyra-1.1.2/gefyra/api/utils.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.1.1/gefyra/cluster/manager.py` & `gefyra-1.1.2/gefyra/cluster/manager.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.1.1/gefyra/cluster/resources.py` & `gefyra-1.1.2/gefyra/cluster/resources.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.1.1/gefyra/cluster/utils.py` & `gefyra-1.1.2/gefyra/cluster/utils.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.1.1/gefyra/configuration.py` & `gefyra-1.1.2/gefyra/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 console = logging.StreamHandler(sys.stdout)
 formatter = logging.Formatter("[%(levelname)s] %(message)s")
 console.setFormatter(formatter)
 
 logger = logging.getLogger("gefyra")
 logger.addHandler(console)
 
-__VERSION__ = "1.1.1"
+__VERSION__ = "1.1.2"
 
 
 def fix_pywin32_in_frozen_build() -> None:  # pragma: no cover
     import os
     import site
 
     if sys.platform != "win32" or not getattr(sys, "frozen", False):
```

### Comparing `gefyra-1.1.1/gefyra/local/bridge.py` & `gefyra-1.1.2/gefyra/local/bridge.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.1.1/gefyra/local/cargo.py` & `gefyra-1.1.2/gefyra/local/cargo.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.1.1/gefyra/local/cargoimage/cargo_dockerfile.py` & `gefyra-1.1.2/gefyra/local/cargoimage/cargo_dockerfile.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.1.1/gefyra/local/check.py` & `gefyra-1.1.2/gefyra/local/check.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.1.1/gefyra/local/minikube.py` & `gefyra-1.1.2/gefyra/local/minikube.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.1.1/gefyra/local/networking.py` & `gefyra-1.1.2/gefyra/local/networking.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.1.1/gefyra/local/telemetry.py` & `gefyra-1.1.2/gefyra/local/telemetry.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.1.1/gefyra/local/utils.py` & `gefyra-1.1.2/gefyra/local/utils.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.1.1/pyproject.toml` & `gefyra-1.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Gefyra"
-version = "1.1.1"
+version = "1.1.2"
 description = "Gefyra runs all developer machine side components of Gefyra's Kubernetes-based development infrastructure"
 authors = ["Michael Schilonka <michael@unikube.io>"]
 readme = "README.md"
 homepage = "https://gefyra.dev"
 repository = "https://github.com/gefyrahq/gefyra"
 documentation = "https://gefyra.dev"
 keywords = [
```

### Comparing `gefyra-1.1.1/PKG-INFO` & `gefyra-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gefyra
-Version: 1.1.1
+Version: 1.1.2
 Summary: Gefyra runs all developer machine side components of Gefyra's Kubernetes-based development infrastructure
 Home-page: https://gefyra.dev
 Keywords: Kubernetes,Development,Cloud-native
 Author: Michael Schilonka
 Author-email: michael@unikube.io
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
```

