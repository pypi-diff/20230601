# Comparing `tmp/cxbuild-0.1.1.tar.gz` & `tmp/cxbuild-0.1.2.tar.gz`

## Comparing `cxbuild-0.1.1.tar` & `cxbuild-0.1.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 cxbuild-0.1.1/.gitmodules
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 cxbuild-0.1.1/CHANGELOG.md
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 cxbuild-0.1.1/CMakeLists.txt
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 cxbuild-0.1.1/requirements.txt
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 cxbuild-0.1.1/.github/workflows/build_wheels.yml
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 cxbuild-0.1.1/.procure/__init__.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cxbuild-0.1.1/cxbuild/__about__.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 cxbuild-0.1.1/cxbuild/__init__.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 cxbuild-0.1.1/cxbuild/activity.py
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 cxbuild-0.1.1/cxbuild/backend.py
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 cxbuild-0.1.1/cxbuild/build_tool.py
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 cxbuild-0.1.1/cxbuild/cmake_extension.py
--rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 cxbuild-0.1.1/cxbuild/cmake_tool.py
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 cxbuild-0.1.1/cxbuild/copyutils.py
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 cxbuild-0.1.1/cxbuild/cxbuild.py
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 cxbuild-0.1.1/cxbuild/extension_builder.py
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 cxbuild-0.1.1/cxbuild/pip_tool.py
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 cxbuild-0.1.1/cxbuild/project.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 cxbuild-0.1.1/cxbuild/project_base.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 cxbuild-0.1.1/cxbuild/pyproject.py
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 cxbuild-0.1.1/cxbuild/setup_tool.py
--rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 cxbuild-0.1.1/cxbuild/solution.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 cxbuild-0.1.1/cxbuild/tool.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 cxbuild-0.1.1/cxbuild/cli/__init__.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 cxbuild-0.1.1/pkg/cxb_simple/CMakeLists.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cxbuild-0.1.1/pkg/cxb_simple/README.md
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 cxbuild-0.1.1/pkg/cxb_simple/pyproject.toml
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 cxbuild-0.1.1/pkg/cxb_simple/setup.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 cxbuild-0.1.1/pkg/cxb_simple/cxb_simple/__init__.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 cxbuild-0.1.1/pkg/cxb_simple/cxb_simple/__main__.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 cxbuild-0.1.1/pkg/cxb_simple/src/main.cpp
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cxbuild-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 cxbuild-0.1.1/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 cxbuild-0.1.1/LICENSE
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 cxbuild-0.1.1/README.md
--rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 cxbuild-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 cxbuild-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 cxbuild-0.1.2/.gitmodules
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 cxbuild-0.1.2/CHANGELOG.md
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 cxbuild-0.1.2/CMakeLists.txt
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 cxbuild-0.1.2/requirements.txt
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 cxbuild-0.1.2/.github/workflows/build_wheels.yml
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 cxbuild-0.1.2/.procure/__init__.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cxbuild-0.1.2/cxbuild/__about__.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 cxbuild-0.1.2/cxbuild/__init__.py
+-rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 cxbuild-0.1.2/cxbuild/activity.py
+-rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 cxbuild-0.1.2/cxbuild/backend.py
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 cxbuild-0.1.2/cxbuild/build_tool.py
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 cxbuild-0.1.2/cxbuild/cmake_extension.py
+-rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 cxbuild-0.1.2/cxbuild/cmake_tool.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 cxbuild-0.1.2/cxbuild/copyutils.py
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 cxbuild-0.1.2/cxbuild/cxbuild.py
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 cxbuild-0.1.2/cxbuild/extension_builder.py
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 cxbuild-0.1.2/cxbuild/pip_tool.py
+-rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 cxbuild-0.1.2/cxbuild/project.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 cxbuild-0.1.2/cxbuild/project_base.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 cxbuild-0.1.2/cxbuild/pyproject.py
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 cxbuild-0.1.2/cxbuild/setup_tool.py
+-rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 cxbuild-0.1.2/cxbuild/solution.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 cxbuild-0.1.2/cxbuild/tool.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 cxbuild-0.1.2/cxbuild/cli/__init__.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 cxbuild-0.1.2/pkg/cxb_simple/CMakeLists.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cxbuild-0.1.2/pkg/cxb_simple/README.md
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 cxbuild-0.1.2/pkg/cxb_simple/pyproject.toml
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 cxbuild-0.1.2/pkg/cxb_simple/setup.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 cxbuild-0.1.2/pkg/cxb_simple/cxb_simple/__init__.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 cxbuild-0.1.2/pkg/cxb_simple/cxb_simple/__main__.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 cxbuild-0.1.2/pkg/cxb_simple/src/main.cpp
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cxbuild-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 cxbuild-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 cxbuild-0.1.2/LICENSE
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 cxbuild-0.1.2/README.md
+-rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 cxbuild-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 cxbuild-0.1.2/PKG-INFO
```

### Comparing `cxbuild-0.1.1/CMakeLists.txt` & `cxbuild-0.1.2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cxbuild-0.1.1/.github/workflows/build_wheels.yml` & `cxbuild-0.1.2/.github/workflows/build_wheels.yml`

 * *Files identical despite different names*

### Comparing `cxbuild-0.1.1/cxbuild/activity.py` & `cxbuild-0.1.2/cxbuild/activity.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,27 +20,32 @@
 
 class Activity(pydantic.BaseModel):
     type: ActivityType = None
     root: Path = Path.cwd()
     path: Path = Path.cwd() / "_cxbuild/activity.json"
     mode: BuildMode = BuildMode.RELEASE
 
+    def __new__(cls, *args, **kwargs):
+        global _activity
+        if not _activity:
+            _activity = super(Activity, cls).__new__(cls)
+        return _activity
+
     @property
     def artifacts_dir(self):
         return self.root / "_cxbuild/artifacts"
 
-    def commit(self):
+    # Note:  I'm tempted to serialize to the environment itself instead of a file ...
+    def save(self):
+        os.environ["CBX_ACTIVITY"] = str(self.path)
         """Serialize an activity to a JSON string"""
         with open(self.path, "w") as f:
             json.dump({"type": self.type.value, "object": self.json()}, f)
 
-    def make_environ(self):
-        os.environ["CBX_ACTIVITY"] = str(self.path)
-        environ = os.environ.copy()
-        return environ
+_activity: Activity = None
 
 
 class BuildActivity(Activity):
     type: ActivityType = ActivityType.BuildActivity
 
 
 class DevelopActivity(Activity):
@@ -56,18 +61,13 @@
         return BuildActivity.parse_raw(data["object"])
     elif data["type"] == ActivityType.DevelopActivity.value:
         return DevelopActivity.parse_raw(data["object"])
     else:
         raise ValueError("Invalid type")
 
 
-_activity: Activity = None
-
-
 def get_activity() -> Activity:
     global _activity
     if _activity:
         return _activity
     path = Path(os.environ["CBX_ACTIVITY"])
-    activity = deserialize_activity(path)
-    _activity = activity
-    return activity
+    return deserialize_activity(path)
```

### Comparing `cxbuild-0.1.1/cxbuild/backend.py` & `cxbuild-0.1.2/cxbuild/backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     config_settings: dict[str, list[str] | str] | None = None,
     metadata_directory: str | None = None,
 ) -> str:
     logger.debug("Build hook: build_editable")
     logger.debug(f"wheel_directory: {wheel_directory}")
     # If not invoked indirectly by cxbuild itself do the default action
     if not os.environ.get('CBX_ACTIVITY'):
-        return build_meta.build_wheel(wheel_directory, config_settings, metadata_directory)
+        return build_meta.build_editable(wheel_directory, config_settings, metadata_directory)
     return build_wheel(wheel_directory, config_settings, metadata_directory)
 
 
 def get_requires_for_build_sdist(
     config_settings: dict[str, str | list[str]] | None = None  # noqa: ARG001
 ) -> list[str]:
     logger.debug("Build hook: get_requires_for_build_sdist")
```

### Comparing `cxbuild-0.1.1/cxbuild/build_tool.py` & `cxbuild-0.1.2/cxbuild/build_tool.py`

 * *Files identical despite different names*

### Comparing `cxbuild-0.1.1/cxbuild/cmake_extension.py` & `cxbuild-0.1.2/cxbuild/cmake_extension.py`

 * *Files identical despite different names*

### Comparing `cxbuild-0.1.1/cxbuild/cmake_tool.py` & `cxbuild-0.1.2/cxbuild/cmake_tool.py`

 * *Files identical despite different names*

### Comparing `cxbuild-0.1.1/cxbuild/copyutils.py` & `cxbuild-0.1.2/cxbuild/copyutils.py`

 * *Files identical despite different names*

### Comparing `cxbuild-0.1.1/cxbuild/cxbuild.py` & `cxbuild-0.1.2/cxbuild/cxbuild.py`

 * *Files identical despite different names*

### Comparing `cxbuild-0.1.1/cxbuild/extension_builder.py` & `cxbuild-0.1.2/cxbuild/extension_builder.py`

 * *Files identical despite different names*

### Comparing `cxbuild-0.1.1/cxbuild/pip_tool.py` & `cxbuild-0.1.2/cxbuild/pip_tool.py`

 * *Files identical despite different names*

### Comparing `cxbuild-0.1.1/cxbuild/project.py` & `cxbuild-0.1.2/cxbuild/project.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 from .pip_tool import PipConfig, PipTool
 from .copyutils import copy_directory_contents
 
 class Project(ProjectBase):
     def __init__(self, path: Path) -> None:
         super().__init__(path)
 
-    def develop(self, env):
-        tool = PipTool(PipConfig(env=env, source_dir=self.path))
+    def develop(self):
+        tool = PipTool(PipConfig(env=os.environ, source_dir=self.path))
         tool.install()
 
-    def build(self, env):
-        tool = BuildTool(BuildConfig(env=env, source_dir=self.path))
+    def build(self):
+        tool = BuildTool(BuildConfig(env=os.environ, source_dir=self.path))
         tool.build()
 
     def build_wheel(
         self,
         wheel_directory: str,
         config_settings: dict[str, list[str] | str] | None = None,
         metadata_directory: str | None = None
```

### Comparing `cxbuild-0.1.1/cxbuild/pyproject.py` & `cxbuild-0.1.2/cxbuild/pyproject.py`

 * *Files identical despite different names*

### Comparing `cxbuild-0.1.1/cxbuild/setup_tool.py` & `cxbuild-0.1.2/cxbuild/setup_tool.py`

 * *Files identical despite different names*

### Comparing `cxbuild-0.1.1/cxbuild/solution.py` & `cxbuild-0.1.2/cxbuild/solution.py`

 * *Files 12% similar despite different names*

```diff
@@ -67,31 +67,29 @@
     def develop(self):
         print('develop')
         config = self.create_config()
         tool = CMakeTool(config)
         tool.build()
         tool.install()
 
-        activity = DevelopActivity()
-        activity.commit()
+        DevelopActivity().save()
 
         for project in self.projects:
-            project.develop(activity.make_environ())
+            project.develop()
 
     def build(self):
         print('build')
         config = self.create_config()
         tool = CMakeTool(config)
         tool.build()
         tool.install()
 
-        activity = BuildActivity()
-        activity.commit()
+        BuildActivity().save()
 
         for project in self.projects:
-            project.build(activity.make_environ())
+            project.build()
 
     def install(self):
         print('install')
         config = self.create_config()
         tool = CMakeTool(config)
         tool.install()
```

### Comparing `cxbuild-0.1.1/cxbuild/cli/__init__.py` & `cxbuild-0.1.2/cxbuild/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `cxbuild-0.1.1/pkg/cxb_simple/CMakeLists.txt` & `cxbuild-0.1.2/pkg/cxb_simple/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cxbuild-0.1.1/pkg/cxb_simple/pyproject.toml` & `cxbuild-0.1.2/pkg/cxb_simple/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cxbuild-0.1.1/pkg/cxb_simple/src/main.cpp` & `cxbuild-0.1.2/pkg/cxb_simple/src/main.cpp`

 * *Files identical despite different names*

### Comparing `cxbuild-0.1.1/.gitignore` & `cxbuild-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `cxbuild-0.1.1/LICENSE` & `cxbuild-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cxbuild-0.1.1/pyproject.toml` & `cxbuild-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cxbuild"
-version = "0.1.1"
+version = "0.1.2"
 description = 'CMake Extension Builder'
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 keywords = []
 authors = [{ name = "Kurtis Fields", email = "kurtisfields@gmail.com" }]
 classifiers = [
```

### Comparing `cxbuild-0.1.1/PKG-INFO` & `cxbuild-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cxbuild
-Version: 0.1.1
+Version: 0.1.2
 Summary: CMake Extension Builder
 Project-URL: homepage, https://github.com/crungelab/cxbuild
 Project-URL: documentation, https://crungelab.github.io/cxbuild/
 Project-URL: repository, https://github.com/crungelab/cxbuild
 Project-URL: changelog, https://github.com/crungelab/cxbuild/blob/main/CHANGELOG.md
 Author-email: Kurtis Fields <kurtisfields@gmail.com>
 License: MIT License
```

