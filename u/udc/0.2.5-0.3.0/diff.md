# Comparing `tmp/udc-0.2.5.tar.gz` & `tmp/udc-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "udc-0.2.5.tar", max compression
+gzip compressed data, was "udc-0.3.0.tar", max compression
```

## Comparing `udc-0.2.5.tar` & `udc-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,16 @@
--rw-r--r--   0        0        0    11357 2023-05-12 01:09:39.984612 udc-0.2.5/LICENSE
--rw-r--r--   0        0        0     2527 2023-05-25 04:58:47.601734 udc-0.2.5/README.md
--rw-r--r--   0        0        0      750 2023-05-29 23:33:02.194201 udc-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      260 2023-05-29 18:47:36.753206 udc-0.2.5/udc/__init__.py
--rw-r--r--   0        0        0      340 2023-05-29 18:47:36.753717 udc-0.2.5/udc/benchling/__init__.py
--rw-r--r--   0        0        0     1248 2023-05-29 18:47:36.754096 udc-0.2.5/udc/benchling/entry.py
--rw-r--r--   0        0        0     1483 2023-05-29 18:47:36.754504 udc-0.2.5/udc/benchling/resource.py
--rw-r--r--   0        0        0     2257 2023-05-29 18:47:36.754873 udc-0.2.5/udc/benchling/root.py
--rw-r--r--   0        0        0      357 2023-05-29 18:47:36.755234 udc-0.2.5/udc/benchling/schema.py
--rw-r--r--   0        0        0      353 2023-05-29 18:47:36.755595 udc-0.2.5/udc/benchling/sequence.py
--rw-r--r--   0        0        0      331 2023-05-25 04:20:16.308186 udc-0.2.5/udc/main.py
--rw-r--r--   0        0        0       49 2023-05-25 04:58:47.606168 udc-0.2.5/udc/quilt/__init__.py
--rw-r--r--   0        0        0      275 2023-05-29 18:47:36.755973 udc-0.2.5/udc/quilt/resource.py
--rw-r--r--   0        0        0      467 2023-05-24 21:56:51.804905 udc-0.2.5/udc/types.py
--rw-r--r--   0        0        0     2502 2023-05-25 04:58:47.606836 udc-0.2.5/udc/un/cli.yaml
--rw-r--r--   0        0        0     3539 2023-05-29 23:32:28.314799 udc-0.2.5/udc/un/un_cli.py
--rw-r--r--   0        0        0     1265 2023-05-25 13:21:33.255738 udc-0.2.5/udc/un/un_uri.py
--rw-r--r--   0        0        0     2135 2023-05-29 18:47:36.756742 udc-0.2.5/udc/un/un_yaml.py
--rw-r--r--   0        0        0     3185 1970-01-01 00:00:00.000000 udc-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-12 01:09:39.984612 udc-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2545 2023-06-01 02:59:07.585224 udc-0.3.0/README.md
+-rw-r--r--   0        0        0      799 2023-06-01 02:59:07.588789 udc-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      232 2023-06-01 02:59:07.594491 udc-0.3.0/udc/__init__.py
+-rw-r--r--   0        0        0     1130 2023-06-01 02:59:07.595367 udc-0.3.0/udc/benchling/__init__.py
+-rw-r--r--   0        0        0     1265 2023-06-01 02:59:07.596228 udc-0.3.0/udc/benchling/entry.py
+-rw-r--r--   0        0        0      693 2023-06-01 02:59:07.596749 udc-0.3.0/udc/benchling/resource.py
+-rw-r--r--   0        0        0     2244 2023-06-01 02:59:07.597617 udc-0.3.0/udc/benchling/root.py
+-rw-r--r--   0        0        0      357 2023-05-31 06:12:37.912100 udc-0.3.0/udc/benchling/schema.py
+-rw-r--r--   0        0        0      353 2023-05-31 06:12:37.911714 udc-0.3.0/udc/benchling/sequence.py
+-rw-r--r--   0        0        0      334 2023-06-01 02:59:07.598493 udc-0.3.0/udc/main.py
+-rw-r--r--   0        0        0       49 2023-05-25 04:58:47.606168 udc-0.3.0/udc/quilt/__init__.py
+-rw-r--r--   0        0        0      275 2023-05-31 00:13:14.714433 udc-0.3.0/udc/quilt/resource.py
+-rw-r--r--   0        0        0      496 2023-06-01 02:59:07.599263 udc-0.3.0/udc/types.py
+-rw-r--r--   0        0        0      276 2023-06-01 02:59:07.599906 udc-0.3.0/udc/wrapper.py
+-rw-r--r--   0        0        0     3244 1970-01-01 00:00:00.000000 udc-0.3.0/PKG-INFO
```

### Comparing `udc-0.2.5/LICENSE` & `udc-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `udc-0.2.5/README.md` & `udc-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -53,45 +53,45 @@
 ```bash
 udc list "quilt+s3://quilt-example#package=examples/wellplates@6782cf98a2"
 ```
 
 e.g.,
 <!--pytest-codeblocks:expected-output-->
 ```bash
-quilt+s3://quilt-example#package=examples/wellplates@6782cf98a2&path=README.md
-quilt+s3://quilt-example#package=examples/wellplates@6782cf98a2&path=autoplate_H1N1.csv
-quilt+s3://quilt-example#package=examples/wellplates@6782cf98a2&path=data_products.ipynb
-quilt+s3://quilt-example#package=examples/wellplates@6782cf98a2&path=neutralisation-altair.json
-quilt+s3://quilt-example#package=examples/wellplates@6782cf98a2&path=neutralisation.json
-quilt+s3://quilt-example#package=examples/wellplates@6782cf98a2&path=quilt_summarize.json
-quilt+s3://quilt-example#package=examples/wellplates@6782cf98a2&path=render.html
+"quilt+s3://quilt-example#package=examples/wellplates@6782cf98a2&path=README.md"
+"quilt+s3://quilt-example#package=examples/wellplates@6782cf98a2&path=autoplate_H1N1.csv"
+"quilt+s3://quilt-example#package=examples/wellplates@6782cf98a2&path=data_products.ipynb"
+"quilt+s3://quilt-example#package=examples/wellplates@6782cf98a2&path=neutralisation-altair.json"
+"quilt+s3://quilt-example#package=examples/wellplates@6782cf98a2&path=neutralisation.json"
+"quilt+s3://quilt-example#package=examples/wellplates@6782cf98a2&path=quilt_summarize.json"
+"quilt+s3://quilt-example#package=examples/wellplates@6782cf98a2&path=render.html"
 ```
 
 ### List all versions of a package
 
 ```bash
 udc list "quilt+s3://quilt-example#package=examples/wellplates" | head -n 1
 ```
 
 e.g.,
 <!--pytest-codeblocks:expected-output-->
 ```bash
-quilt+s3://quilt-example#package=examples/wellplates@6782cf98a2c600f4c519efd5de868d5ef1e05ac92fcb0fa56044bb8c925c5f02
+"quilt+s3://quilt-example#package=examples/wellplates@6782cf98a2c600f4c519efd5de868d5ef1e05ac92fcb0fa56044bb8c925c5f02"
 ```
 
 ### List all packages in a registry
 
 ```bash
 udc list quilt+s3://quilt-example | head -n 1
 ```
 
 e.g.,
 <!--pytest-codeblocks:expected-output-->
 ```bash
-quilt+s3://quilt-example#package=akarve/amazon-reviews:latest
+"quilt+s3://quilt-example#package=akarve/amazon-reviews:latest"
 ```
 
 ## Development
 
 ### Testing
 
 <!--pytest.mark.skip-->
```

### Comparing `udc-0.2.5/pyproject.toml` & `udc-0.3.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [tool.poetry]
 name = "udc"
-version = "0.2.5"
+version = "0.3.0"
 description = ""
 authors = ["Ernest Prabhakar <ernest@quiltdata.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 anyio = "^3.7.0"
 trio = "^0.22.0"
 asyncclick = "^8.1.3.4"
 quilt3 = "^5.3.1"
 urllib3 = "<2"
 typing-extensions = "^4.5.0"
-quiltplus = ">0.8.0"
-#  quiltplus = {git = "https://github.com/quiltdata/quiltplus.git", rev = "main"}
+quiltplus = ">=0.9.0"
+# quiltplus = {git = "https://github.com/quiltdata/quiltplus.git", rev = "42-resourceattrs-to-align-with-udc"}
 benchling-sdk = "^1.6.1"
+un-yaml = "^0.1.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest-coverage = "^0.0"
 pytest-watcher = "^0.2.6"
 pytest-asyncio = "^0.21.0"
 pytest-trio = "^0.8.0"
 pytest-codeblocks = "^0.16.1"
```

### Comparing `udc-0.2.5/udc/benchling/entry.py` & `udc-0.3.0/udc/benchling/entry.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,11 +26,11 @@
         }
 
     def wrap(self, id, sub_type):
         item_dict = {"id": id, sub_type: id}
         item = type(f"wrap_{sub_type}", (object,), item_dict)
         return self.item_uri(item, sub_type)
 
-    async def list(self) -> list[str]:
+    async def list(self, argv: dict = {}) -> list[str]:
         self.fetch()
         kids = self.children
         return [self.wrap(id, sub_type) for sub_type in kids for id in kids[sub_type]]
```

### Comparing `udc-0.2.5/udc/benchling/resource.py` & `udc-0.3.0/udc/benchling/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,12 @@
-from .entry import BenchlingEntry, BenchlingEntryList
-from .root import BenchlingRoot
-from .schema import BenchlingSchema, BenchlingSchemaList
-from .sequence import BenchlingSequence, BenchlingSequenceList
-
-RESOURCE_MAP = {
-    "entries": [BenchlingEntryList, BenchlingEntry],
-    "dna_sequences": [BenchlingSequenceList, BenchlingSequence],
-    "schemas": [BenchlingSchemaList, BenchlingSchema],
-}
+from .entry import BenchlingEntry, BenchlingEntryList  # NOQA F401
+from .resource import RESOURCE_MAP, BenchlingResource  # NOQA F401
+from .root import BenchlingById, BenchlingRoot  # NOQA F401
+from .schema import BenchlingSchema, BenchlingSchemaList  # NOQA F401
+from .sequence import BenchlingSequence, BenchlingSequenceList  # NOQA F401
 
 RESOURCES = [
     "aa_sequences",
     "api",
     "apps",
     "assay_results",
     "assay_runs",
@@ -51,17 +46,7 @@
     "users",
     "v2",
     "warehouse",
     "workflow_outputs",
     "workflow_task_groups",
     "workflow_tasks",
 ]
-
-
-def BenchlingResource(attrs: dict):
-    root = BenchlingRoot(attrs)
-    type = root.type
-    klasses = RESOURCE_MAP.get(type)
-    if not klasses:
-        raise ValueError(f"Unknown resource type[{type}]: {attrs}")
-    klass = klasses[0] if not root.id else klasses[1]
-    return klass(attrs)
```

### Comparing `udc-0.2.5/udc/benchling/root.py` & `udc-0.3.0/udc/benchling/root.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 BENCH_TYPE_DEFAULT = "entries"
 
 
 class BenchlingRoot:
     BENCH_TENANT = os.environ.get("BENCHLING_TENANT_DNS")
     BENCH_ENTRY = os.environ.get("BENCHLING_ENTRY_ID")
     BENCH_AUTHOR = os.environ.get("BENCHLING_AUTHOR_ID")
-    BENCH_KEY = os.environ.get("BENCHLING_API_KEY")
+    BENCH_KEY = os.environ.get("BENCHLING_API_KEY") or ""
     CLIENT = Benchling(url=f"https://{BENCH_TENANT}", auth_method=ApiKeyAuth(BENCH_KEY))
     DEFAULT_URI = f"benchling+https://{BENCH_TENANT}#type=entries"
 
     def __init__(self, attrs: dict):
         self.attrs = attrs
         self.uri = attrs.get("_uri")
-        self.id = attrs.get(BENCH_ID)
-        self.set_type(attrs.get(BENCH_TYPE))
+        self.id = attrs.get(BENCH_ID) or ""
+        self.set_type(attrs[BENCH_TYPE])
 
     def __repr__(self) -> str:
         return f"<{self.__class__}({self.uri})>"
 
     def set_type(self, btype: str):
         type = btype or BENCH_TYPE_DEFAULT
         types = type.split(".")
@@ -55,15 +55,14 @@
             if "&id=" not in base:
                 base += f"&id={item.id}"
         if sub_type and hasattr(item, sub_type):
             base += f"&{sub_type}={getattr(item, sub_type)}"
         logging.debug(f"item_uri.uri: {base}")
         return base
 
-    async def list(self) -> list[str]:
+    async def list(self, argv: dict = {}) -> list[str]:
         return [self.item_uri(item) for item in self.items()]
 
 
 class BenchlingById(BenchlingRoot):
     def __init__(self, attrs: dict) -> None:
         super().__init__(attrs)
-        self.id = attrs.get(BENCH_ID)
```

### Comparing `udc-0.2.5/PKG-INFO` & `udc-0.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: udc
-Version: 0.2.5
+Version: 0.3.0
 Summary: 
 Author: Ernest Prabhakar
 Author-email: ernest@quiltdata.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: anyio (>=3.7.0,<4.0.0)
 Requires-Dist: asyncclick (>=8.1.3.4,<9.0.0.0)
 Requires-Dist: benchling-sdk (>=1.6.1,<2.0.0)
 Requires-Dist: quilt3 (>=5.3.1,<6.0.0)
-Requires-Dist: quiltplus (>0.8.0)
+Requires-Dist: quiltplus (>=0.9.0)
 Requires-Dist: trio (>=0.22.0,<0.23.0)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
+Requires-Dist: un-yaml (>=0.1.2,<0.2.0)
 Requires-Dist: urllib3 (<2)
 Description-Content-Type: text/markdown
 
 # UDC
 
 ## The Universal Data Client
 
@@ -73,45 +74,45 @@
 ```bash
 udc list "quilt+s3://quilt-example#package=examples/wellplates@6782cf98a2"
 ```
 
 e.g.,
 <!--pytest-codeblocks:expected-output-->
 ```bash
-quilt+s3://quilt-example#package=examples/wellplates@6782cf98a2&path=README.md
-quilt+s3://quilt-example#package=examples/wellplates@6782cf98a2&path=autoplate_H1N1.csv
-quilt+s3://quilt-example#package=examples/wellplates@6782cf98a2&path=data_products.ipynb
-quilt+s3://quilt-example#package=examples/wellplates@6782cf98a2&path=neutralisation-altair.json
-quilt+s3://quilt-example#package=examples/wellplates@6782cf98a2&path=neutralisation.json
-quilt+s3://quilt-example#package=examples/wellplates@6782cf98a2&path=quilt_summarize.json
-quilt+s3://quilt-example#package=examples/wellplates@6782cf98a2&path=render.html
+"quilt+s3://quilt-example#package=examples/wellplates@6782cf98a2&path=README.md"
+"quilt+s3://quilt-example#package=examples/wellplates@6782cf98a2&path=autoplate_H1N1.csv"
+"quilt+s3://quilt-example#package=examples/wellplates@6782cf98a2&path=data_products.ipynb"
+"quilt+s3://quilt-example#package=examples/wellplates@6782cf98a2&path=neutralisation-altair.json"
+"quilt+s3://quilt-example#package=examples/wellplates@6782cf98a2&path=neutralisation.json"
+"quilt+s3://quilt-example#package=examples/wellplates@6782cf98a2&path=quilt_summarize.json"
+"quilt+s3://quilt-example#package=examples/wellplates@6782cf98a2&path=render.html"
 ```
 
 ### List all versions of a package
 
 ```bash
 udc list "quilt+s3://quilt-example#package=examples/wellplates" | head -n 1
 ```
 
 e.g.,
 <!--pytest-codeblocks:expected-output-->
 ```bash
-quilt+s3://quilt-example#package=examples/wellplates@6782cf98a2c600f4c519efd5de868d5ef1e05ac92fcb0fa56044bb8c925c5f02
+"quilt+s3://quilt-example#package=examples/wellplates@6782cf98a2c600f4c519efd5de868d5ef1e05ac92fcb0fa56044bb8c925c5f02"
 ```
 
 ### List all packages in a registry
 
 ```bash
 udc list quilt+s3://quilt-example | head -n 1
 ```
 
 e.g.,
 <!--pytest-codeblocks:expected-output-->
 ```bash
-quilt+s3://quilt-example#package=akarve/amazon-reviews:latest
+"quilt+s3://quilt-example#package=akarve/amazon-reviews:latest"
 ```
 
 ## Development
 
 ### Testing
 
 <!--pytest.mark.skip-->
```

