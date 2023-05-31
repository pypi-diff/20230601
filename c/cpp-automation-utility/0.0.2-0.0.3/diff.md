# Comparing `tmp/cpp-automation-utility-0.0.2.tar.gz` & `tmp/cpp-automation-utility-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpp-automation-utility-0.0.2.tar", last modified: Wed May 31 04:21:10 2023, max compression
+gzip compressed data, was "cpp-automation-utility-0.0.3.tar", last modified: Wed May 31 22:55:48 2023, max compression
```

## Comparing `cpp-automation-utility-0.0.2.tar` & `cpp-automation-utility-0.0.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:21:10.961018 cpp-automation-utility-0.0.2/
--rw-rw-rw-   0 root         (0) root         (0)     1080 2023-05-31 04:21:01.000000 cpp-automation-utility-0.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1161 2023-05-31 04:21:10.961018 cpp-automation-utility-0.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      713 2023-05-31 04:21:01.000000 cpp-automation-utility-0.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:21:10.958018 cpp-automation-utility-0.0.2/cau/
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-31 04:21:01.000000 cpp-automation-utility-0.0.2/cau/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3995 2023-05-31 04:21:01.000000 cpp-automation-utility-0.0.2/cau/cau_cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:21:10.958018 cpp-automation-utility-0.0.2/cau/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 04:21:01.000000 cpp-automation-utility-0.0.2/cau/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2321 2023-05-31 04:21:01.000000 cpp-automation-utility-0.0.2/cau/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     4794 2023-05-31 04:21:01.000000 cpp-automation-utility-0.0.2/cau/tests/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)      706 2023-05-31 04:21:01.000000 cpp-automation-utility-0.0.2/cau/timer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:21:10.959018 cpp-automation-utility-0.0.2/cau/wrappers/
--rw-rw-rw-   0 root         (0) root         (0)     9416 2023-05-31 04:21:01.000000 cpp-automation-utility-0.0.2/cau/wrappers/Clang.py
--rw-rw-rw-   0 root         (0) root         (0)     3311 2023-05-31 04:21:01.000000 cpp-automation-utility-0.0.2/cau/wrappers/Conan.py
--rw-rw-rw-   0 root         (0) root         (0)     1368 2023-05-31 04:21:01.000000 cpp-automation-utility-0.0.2/cau/wrappers/Git.py
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-05-31 04:21:01.000000 cpp-automation-utility-0.0.2/cau/wrappers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:21:10.959018 cpp-automation-utility-0.0.2/cau/wrappers/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 04:21:01.000000 cpp-automation-utility-0.0.2/cau/wrappers/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11248 2023-05-31 04:21:01.000000 cpp-automation-utility-0.0.2/cau/wrappers/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     3647 2023-05-31 04:21:01.000000 cpp-automation-utility-0.0.2/cau/wrappers/tests/test_Conan.py
--rw-rw-rw-   0 root         (0) root         (0)     2215 2023-05-31 04:21:01.000000 cpp-automation-utility-0.0.2/cau/wrappers/tests/test_Coverage.py
--rw-rw-rw-   0 root         (0) root         (0)      823 2023-05-31 04:21:01.000000 cpp-automation-utility-0.0.2/cau/wrappers/tests/test_Git.py
--rw-rw-rw-   0 root         (0) root         (0)     2478 2023-05-31 04:21:01.000000 cpp-automation-utility-0.0.2/cau/wrappers/tests/test_Tidy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 04:21:10.960018 cpp-automation-utility-0.0.2/cpp_automation_utility.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1161 2023-05-31 04:21:10.000000 cpp-automation-utility-0.0.2/cpp_automation_utility.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      742 2023-05-31 04:21:10.000000 cpp-automation-utility-0.0.2/cpp_automation_utility.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 04:21:10.000000 cpp-automation-utility-0.0.2/cpp_automation_utility.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-05-31 04:21:10.000000 cpp-automation-utility-0.0.2/cpp_automation_utility.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 04:21:10.000000 cpp-automation-utility-0.0.2/cpp_automation_utility.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      110 2023-05-31 04:21:10.000000 cpp-automation-utility-0.0.2/cpp_automation_utility.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-05-31 04:21:10.000000 cpp-automation-utility-0.0.2/cpp_automation_utility.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 04:21:10.961018 cpp-automation-utility-0.0.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1162 2023-05-31 04:21:01.000000 cpp-automation-utility-0.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 22:55:48.952589 cpp-automation-utility-0.0.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1080 2023-05-31 22:55:40.000000 cpp-automation-utility-0.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1161 2023-05-31 22:55:48.952589 cpp-automation-utility-0.0.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      713 2023-05-31 22:55:40.000000 cpp-automation-utility-0.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 22:55:48.948589 cpp-automation-utility-0.0.3/cau/
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-05-31 22:55:40.000000 cpp-automation-utility-0.0.3/cau/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4044 2023-05-31 22:55:40.000000 cpp-automation-utility-0.0.3/cau/cau_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 22:55:48.949589 cpp-automation-utility-0.0.3/cau/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 22:55:40.000000 cpp-automation-utility-0.0.3/cau/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2321 2023-05-31 22:55:40.000000 cpp-automation-utility-0.0.3/cau/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     4794 2023-05-31 22:55:40.000000 cpp-automation-utility-0.0.3/cau/tests/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      707 2023-05-31 22:55:40.000000 cpp-automation-utility-0.0.3/cau/timer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 22:55:48.950589 cpp-automation-utility-0.0.3/cau/wrappers/
+-rw-rw-rw-   0 root         (0) root         (0)     9406 2023-05-31 22:55:40.000000 cpp-automation-utility-0.0.3/cau/wrappers/Clang.py
+-rw-rw-rw-   0 root         (0) root         (0)     3311 2023-05-31 22:55:40.000000 cpp-automation-utility-0.0.3/cau/wrappers/Conan.py
+-rw-rw-rw-   0 root         (0) root         (0)     1368 2023-05-31 22:55:40.000000 cpp-automation-utility-0.0.3/cau/wrappers/Git.py
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-05-31 22:55:40.000000 cpp-automation-utility-0.0.3/cau/wrappers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 22:55:48.951589 cpp-automation-utility-0.0.3/cau/wrappers/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 22:55:40.000000 cpp-automation-utility-0.0.3/cau/wrappers/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11248 2023-05-31 22:55:40.000000 cpp-automation-utility-0.0.3/cau/wrappers/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     3647 2023-05-31 22:55:40.000000 cpp-automation-utility-0.0.3/cau/wrappers/tests/test_Conan.py
+-rw-rw-rw-   0 root         (0) root         (0)     2215 2023-05-31 22:55:40.000000 cpp-automation-utility-0.0.3/cau/wrappers/tests/test_Coverage.py
+-rw-rw-rw-   0 root         (0) root         (0)      823 2023-05-31 22:55:40.000000 cpp-automation-utility-0.0.3/cau/wrappers/tests/test_Git.py
+-rw-rw-rw-   0 root         (0) root         (0)     2478 2023-05-31 22:55:40.000000 cpp-automation-utility-0.0.3/cau/wrappers/tests/test_Tidy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 22:55:48.952589 cpp-automation-utility-0.0.3/cpp_automation_utility.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1161 2023-05-31 22:55:48.000000 cpp-automation-utility-0.0.3/cpp_automation_utility.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      742 2023-05-31 22:55:48.000000 cpp-automation-utility-0.0.3/cpp_automation_utility.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 22:55:48.000000 cpp-automation-utility-0.0.3/cpp_automation_utility.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-05-31 22:55:48.000000 cpp-automation-utility-0.0.3/cpp_automation_utility.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 22:55:48.000000 cpp-automation-utility-0.0.3/cpp_automation_utility.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      110 2023-05-31 22:55:48.000000 cpp-automation-utility-0.0.3/cpp_automation_utility.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-05-31 22:55:48.000000 cpp-automation-utility-0.0.3/cpp_automation_utility.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 22:55:48.952589 cpp-automation-utility-0.0.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1162 2023-05-31 22:55:40.000000 cpp-automation-utility-0.0.3/setup.py
```

### Comparing `cpp-automation-utility-0.0.2/LICENSE` & `cpp-automation-utility-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cpp-automation-utility-0.0.2/PKG-INFO` & `cpp-automation-utility-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpp-automation-utility
-Version: 0.0.2
+Version: 0.0.3
 Summary: CLI utility to assist C++ in a devops environment
 Home-page: https://gitlab.com/aldridgesoftwaredesigns/cau
 Author: AldridgeSoftwareDesigns
 Author-email: aldridge.robert.james@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7.0
```

### Comparing `cpp-automation-utility-0.0.2/README.md` & `cpp-automation-utility-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `cpp-automation-utility-0.0.2/cau/cau_cli.py` & `cpp-automation-utility-0.0.3/cau/cau_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 build_type_help = "Build type (Debug|Release)"
 platform_help = "Build platform (linux|win64)"
 
 @cau_cli.command(help="Restores conan dependencies")
 @click.option("-b", "--build-directory", default="build", help=build_directory_help)
 @click.option("-t", "--build-type", default="Debug", help=build_type_help)
 @click.option("-p", "--platform", default="linux", help=platform_help)
+@cau.timer
 def restore(build_directory: str, build_type: str, platform: str):
     """
     Restores conan dependencies
     """
     conan = cau.Conan(build_directory=build_directory, build_type=build_type, platform=platform)
     result = conan.restore()
     sys.exit(result.returncode)
@@ -45,15 +46,15 @@
         _ = conan.restore()
 
     logger.debug("Interrogating git for changed files")
     git = cau.Git()
     changes = git.changed_files()
 
     logger.debug("Performing lint operation")
-    linter = cau.Tidy(touched_files=changes)
+    linter = cau.Tidy(touched_files=changes, compile_database_dir=build_directory)
     result = linter.lint()
     sys.exit(0 if result else 1)
 
 @cau_cli.command(help="Build project via conan")
 @click.option("-s", "--skip-restore", is_flag=True, default=False, help=restore_help)
 @click.option("-b", "--build-directory", default="build", help=build_directory_help)
 @click.option("-t", "--build-type", default="Debug", help=build_type_help)
```

### Comparing `cpp-automation-utility-0.0.2/cau/tests/conftest.py` & `cpp-automation-utility-0.0.3/cau/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cpp-automation-utility-0.0.2/cau/tests/test_cli.py` & `cpp-automation-utility-0.0.3/cau/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `cpp-automation-utility-0.0.2/cau/timer.py` & `cpp-automation-utility-0.0.3/cau/timer.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     Returns:
         Callable: wrapper function
     """
 
     @functools.wraps(func)
     def timer_wrapper(*args, **kwargs):
         start = time.perf_counter_ns()
-        logger.info("Entering %s", func.__name__)
+        logger.debug("Entering %s", func.__name__)
         try:
             result = func(*args, **kwargs)
         finally:
             logger.info("%s completed in %d ms", func.__name__, (time.perf_counter_ns() - start)/1.0e6)
         return result
 
     return timer_wrapper
```

### Comparing `cpp-automation-utility-0.0.2/cau/wrappers/Clang.py` & `cpp-automation-utility-0.0.3/cau/wrappers/Clang.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
     def __init__(
         self,
         touched_files: DiffCollection = None,
         config: pathlib.Path = None,
         compile_database_dir: pathlib.Path = None
     ) -> None:
-        self._config: pathlib.Path = config or pathlib.Path.cwd()/".gitlab"/".clang-tidy"
+        self._config: pathlib.Path = config or pathlib.Path.cwd()/".clang-tidy"
         self._compile_database_dir: pathlib.Path = compile_database_dir or pathlib.Path.cwd()/"build"
         self._files: DiffCollection = touched_files or []
         self._sources: PathCollection = []
         self._headers: PathCollection = []
         self._results: list(subprocess.CompletedProcess) = []
         logger.debug("Changed files: %s", touched_files)
         if self._files:
```

### Comparing `cpp-automation-utility-0.0.2/cau/wrappers/Conan.py` & `cpp-automation-utility-0.0.3/cau/wrappers/Conan.py`

 * *Files identical despite different names*

### Comparing `cpp-automation-utility-0.0.2/cau/wrappers/Git.py` & `cpp-automation-utility-0.0.3/cau/wrappers/Git.py`

 * *Files identical despite different names*

### Comparing `cpp-automation-utility-0.0.2/cau/wrappers/tests/conftest.py` & `cpp-automation-utility-0.0.3/cau/wrappers/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cpp-automation-utility-0.0.2/cau/wrappers/tests/test_Conan.py` & `cpp-automation-utility-0.0.3/cau/wrappers/tests/test_Conan.py`

 * *Files identical despite different names*

### Comparing `cpp-automation-utility-0.0.2/cau/wrappers/tests/test_Coverage.py` & `cpp-automation-utility-0.0.3/cau/wrappers/tests/test_Coverage.py`

 * *Files identical despite different names*

### Comparing `cpp-automation-utility-0.0.2/cau/wrappers/tests/test_Git.py` & `cpp-automation-utility-0.0.3/cau/wrappers/tests/test_Git.py`

 * *Files identical despite different names*

### Comparing `cpp-automation-utility-0.0.2/cau/wrappers/tests/test_Tidy.py` & `cpp-automation-utility-0.0.3/cau/wrappers/tests/test_Tidy.py`

 * *Files identical despite different names*

### Comparing `cpp-automation-utility-0.0.2/cpp_automation_utility.egg-info/PKG-INFO` & `cpp-automation-utility-0.0.3/cpp_automation_utility.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpp-automation-utility
-Version: 0.0.2
+Version: 0.0.3
 Summary: CLI utility to assist C++ in a devops environment
 Home-page: https://gitlab.com/aldridgesoftwaredesigns/cau
 Author: AldridgeSoftwareDesigns
 Author-email: aldridge.robert.james@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7.0
```

### Comparing `cpp-automation-utility-0.0.2/cpp_automation_utility.egg-info/SOURCES.txt` & `cpp-automation-utility-0.0.3/cpp_automation_utility.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cpp-automation-utility-0.0.2/setup.py` & `cpp-automation-utility-0.0.3/setup.py`

 * *Files identical despite different names*

