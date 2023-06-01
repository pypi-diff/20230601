# Comparing `tmp/elias-0.2.0.tar.gz` & `tmp/elias-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/d/Projects/elias/dist/.tmp-46s1rhv8/elias-0.2.0.tar", last modified: Mon Apr 24 08:35:40 2023, max compression
+gzip compressed data, was "/mnt/d/Projects/elias/dist/.tmp-elv4s3hw/elias-0.2.1.tar", last modified: Thu Jun  1 16:31:17 2023, max compression
```

## Comparing `elias-0.2.0.tar` & `elias-0.2.1.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-04-24 08:35:40.000000 elias-0.2.0/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2022-04-27 09:37:39.000000 elias-0.2.0/LICENSE
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2138 2023-04-24 08:35:40.000000 elias-0.2.0/PKG-INFO
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1736 2022-04-27 09:37:39.000000 elias-0.2.0/README.md
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      110 2022-04-27 09:37:39.000000 elias-0.2.0/pyproject.toml
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      707 2023-04-24 08:35:40.000000 elias-0.2.0/setup.cfg
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)       98 2022-04-27 09:37:39.000000 elias-0.2.0/setup.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-04-24 08:35:38.000000 elias-0.2.0/src/
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-04-24 08:35:38.000000 elias-0.2.0/src/elias/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2022-04-27 09:37:39.000000 elias-0.2.0/src/elias/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)    22222 2023-04-24 08:29:27.000000 elias-0.2.0/src/elias/config.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-04-24 08:35:39.000000 elias-0.2.0/src/elias/data/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2022-04-27 09:37:39.000000 elias-0.2.0/src/elias/data/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     8439 2022-04-27 09:37:39.000000 elias-0.2.0/src/elias/data/combined.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4507 2022-04-27 09:37:39.000000 elias-0.2.0/src/elias/data/loader.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4987 2022-04-27 09:37:39.000000 elias-0.2.0/src/elias/data/sampling.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1047 2022-04-27 09:37:39.000000 elias-0.2.0/src/elias/data/stop_criterion.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-04-24 08:35:39.000000 elias-0.2.0/src/elias/folder/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      156 2022-04-27 09:37:39.000000 elias-0.2.0/src/elias/folder/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1355 2022-04-27 09:37:39.000000 elias-0.2.0/src/elias/folder/analysis.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     8126 2022-05-13 11:41:20.000000 elias-0.2.0/src/elias/folder/data.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)    13271 2022-12-23 10:38:59.000000 elias-0.2.0/src/elias/folder/folder.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1491 2022-12-23 10:15:28.000000 elias-0.2.0/src/elias/folder/model.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4564 2023-01-14 17:00:38.000000 elias-0.2.0/src/elias/folder/run.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-04-24 08:35:39.000000 elias-0.2.0/src/elias/manager/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      294 2022-04-27 09:37:39.000000 elias-0.2.0/src/elias/manager/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2705 2022-04-27 09:37:39.000000 elias-0.2.0/src/elias/manager/analysis.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1594 2022-04-27 09:37:39.000000 elias-0.2.0/src/elias/manager/artifact.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)    12045 2022-04-27 09:37:39.000000 elias-0.2.0/src/elias/manager/buffered.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)    13104 2022-10-23 15:43:10.000000 elias-0.2.0/src/elias/manager/data.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)    22291 2022-12-23 10:55:00.000000 elias-0.2.0/src/elias/manager/model.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2914 2022-05-10 13:31:36.000000 elias-0.2.0/src/elias/manager/run.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-04-24 08:35:40.000000 elias-0.2.0/src/elias/util/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      361 2022-06-24 14:37:22.000000 elias-0.2.0/src/elias/util/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     6824 2023-03-21 10:22:24.000000 elias-0.2.0/src/elias/util/fs.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     7919 2022-06-24 13:43:08.000000 elias-0.2.0/src/elias/util/io.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4690 2023-03-21 10:20:42.000000 elias-0.2.0/src/elias/util/range.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1248 2022-10-24 10:11:39.000000 elias-0.2.0/src/elias/util/timing.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5512 2022-05-11 08:27:09.000000 elias-0.2.0/src/elias/util/version.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-04-24 08:35:39.000000 elias-0.2.0/src/elias.egg-info/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2138 2023-04-24 08:35:38.000000 elias-0.2.0/src/elias.egg-info/PKG-INFO
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      898 2023-04-24 08:35:38.000000 elias-0.2.0/src/elias.egg-info/SOURCES.txt
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        1 2023-04-24 08:35:38.000000 elias-0.2.0/src/elias.egg-info/dependency_links.txt
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      100 2023-04-24 08:35:38.000000 elias-0.2.0/src/elias.egg-info/requires.txt
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        6 2023-04-24 08:35:38.000000 elias-0.2.0/src/elias.egg-info/top_level.txt
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-01 16:31:17.686972 elias-0.2.1/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2022-04-27 09:37:39.000000 elias-0.2.1/LICENSE
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2138 2023-06-01 16:31:17.686972 elias-0.2.1/PKG-INFO
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1736 2022-04-27 09:37:39.000000 elias-0.2.1/README.md
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      110 2022-04-27 09:37:39.000000 elias-0.2.1/pyproject.toml
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      707 2023-06-01 16:31:17.697341 elias-0.2.1/setup.cfg
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)       98 2022-04-27 09:37:39.000000 elias-0.2.1/setup.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-01 16:31:15.931860 elias-0.2.1/src/
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-01 16:31:16.137287 elias-0.2.1/src/elias/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2022-04-27 09:37:39.000000 elias-0.2.1/src/elias/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)    22222 2023-04-24 08:29:27.000000 elias-0.2.1/src/elias/config.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-01 16:31:16.581947 elias-0.2.1/src/elias/data/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2022-04-27 09:37:39.000000 elias-0.2.1/src/elias/data/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     8439 2022-04-27 09:37:39.000000 elias-0.2.1/src/elias/data/combined.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4507 2022-04-27 09:37:39.000000 elias-0.2.1/src/elias/data/loader.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4987 2022-04-27 09:37:39.000000 elias-0.2.1/src/elias/data/sampling.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1047 2022-04-27 09:37:39.000000 elias-0.2.1/src/elias/data/stop_criterion.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-01 16:31:16.896908 elias-0.2.1/src/elias/folder/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      156 2022-04-27 09:37:39.000000 elias-0.2.1/src/elias/folder/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1355 2022-04-27 09:37:39.000000 elias-0.2.1/src/elias/folder/analysis.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     8126 2022-05-13 11:41:20.000000 elias-0.2.1/src/elias/folder/data.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)    13271 2022-12-23 10:38:59.000000 elias-0.2.1/src/elias/folder/folder.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1491 2022-12-23 10:15:28.000000 elias-0.2.1/src/elias/folder/model.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4983 2023-05-29 14:26:02.000000 elias-0.2.1/src/elias/folder/run.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-01 16:31:17.267704 elias-0.2.1/src/elias/manager/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      294 2022-04-27 09:37:39.000000 elias-0.2.1/src/elias/manager/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2705 2022-04-27 09:37:39.000000 elias-0.2.1/src/elias/manager/analysis.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1594 2022-04-27 09:37:39.000000 elias-0.2.1/src/elias/manager/artifact.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)    12045 2022-04-27 09:37:39.000000 elias-0.2.1/src/elias/manager/buffered.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)    13104 2022-10-23 15:43:10.000000 elias-0.2.1/src/elias/manager/data.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)    22291 2022-12-23 10:55:00.000000 elias-0.2.1/src/elias/manager/model.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2918 2023-05-29 14:22:02.000000 elias-0.2.1/src/elias/manager/run.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-01 16:31:17.645622 elias-0.2.1/src/elias/util/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      361 2022-06-24 14:37:22.000000 elias-0.2.1/src/elias/util/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     6870 2023-04-28 12:57:24.000000 elias-0.2.1/src/elias/util/fs.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     7919 2022-06-24 13:43:08.000000 elias-0.2.1/src/elias/util/io.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4690 2023-03-21 10:20:42.000000 elias-0.2.1/src/elias/util/range.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1248 2022-10-24 10:11:39.000000 elias-0.2.1/src/elias/util/timing.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      390 2023-05-26 09:28:39.000000 elias-0.2.1/src/elias/util/typing.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5512 2022-05-11 08:27:09.000000 elias-0.2.1/src/elias/util/version.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-01 16:31:16.321601 elias-0.2.1/src/elias.egg-info/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2138 2023-06-01 16:31:15.000000 elias-0.2.1/src/elias.egg-info/PKG-INFO
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      923 2023-06-01 16:31:15.000000 elias-0.2.1/src/elias.egg-info/SOURCES.txt
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        1 2023-06-01 16:31:15.000000 elias-0.2.1/src/elias.egg-info/dependency_links.txt
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      100 2023-06-01 16:31:15.000000 elias-0.2.1/src/elias.egg-info/requires.txt
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        6 2023-06-01 16:31:15.000000 elias-0.2.1/src/elias.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `elias-0.2.0/PKG-INFO` & `elias-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elias
-Version: 0.2.0
+Version: 0.2.1
 Summary: ELIAS experiment library for facilitating machine learning projects
 Home-page: https://github.com/tobias-kirschstein/elias
 Author: Tobias Kirschstein
 Author-email: tobias.kirschstein@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `elias-0.2.0/README.md` & `elias-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `elias-0.2.0/setup.cfg` & `elias-0.2.1/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = elias
-version = 0.2.0
+version = 0.2.1
 author = Tobias Kirschstein
 author_email = tobias.kirschstein@gmail.com
 description = ELIAS experiment library for facilitating machine learning projects
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tobias-kirschstein/elias
 project_urls =
```

### Comparing `elias-0.2.0/src/elias/config.py` & `elias-0.2.1/src/elias/config.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.0/src/elias/data/combined.py` & `elias-0.2.1/src/elias/data/combined.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.0/src/elias/data/loader.py` & `elias-0.2.1/src/elias/data/loader.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.0/src/elias/data/sampling.py` & `elias-0.2.1/src/elias/data/sampling.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.0/src/elias/data/stop_criterion.py` & `elias-0.2.1/src/elias/data/stop_criterion.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.0/src/elias/folder/analysis.py` & `elias-0.2.1/src/elias/folder/analysis.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.0/src/elias/folder/data.py` & `elias-0.2.1/src/elias/folder/data.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.0/src/elias/folder/folder.py` & `elias-0.2.1/src/elias/folder/folder.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.0/src/elias/folder/model.py` & `elias-0.2.1/src/elias/folder/model.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.0/src/elias/folder/run.py` & `elias-0.2.1/src/elias/folder/run.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,27 +15,32 @@
     """
     Manages several runs stored in a folder. A run can be the result of any arbitrary script.
     Typically the artifacts of several runs of the same script would be stored in the same run folder.
     Each run is identified by an incrementing run id.
     Runs in the same run folder share a name format that can contain the following wildcards:
         - $: for the run id
         - *: for extra name information for a run (optional)
+
+    A typical name format might look like this: RUN-$[-*]
     """
 
     _name_format: str
     _folder: Folder
 
     def __init__(self, location: str, name_format: str, localize_via_run_name: bool = False):
         ensure_directory_exists(location)
         self._folder = Folder(location)
         self._name_format = name_format
         self._localize_via_run_name = localize_via_run_name
 
         self._cls_run_manager: Type[_RunManagerType] = reveal_type_var(self, _RunManagerType)
 
+    def get_location(self) -> str:
+        return self._folder.get_location()
+
     def cd(self, sub_folder: str):
         # Inplace cd to avoid having to infer the correct subclass of the current object
         self._folder.cd(sub_folder, inplace=True)
 
     def list_runs(self) -> List[str]:
         return self._folder.list_file_numbering(self._name_format, return_only_file_names=True)
 
@@ -81,14 +86,23 @@
         -------
             A run name following the name format of this run folder
         """
 
         return self._folder.substitute(self._name_format, run_id, name=name)
 
     def resolve_run_name(self, run_name_or_id: Union[str, int]) -> Optional[str]:
+        """
+        Find complete run name given a partial run name or run ID.
+
+        :param run_name_or_id:
+            for example, RUN-2 or 2
+        :return:
+            The complete run name that was found in the run folder, e.g., RUN-2-higher_LR
+        """
+
         if isinstance(run_name_or_id, int):
             return self.get_run_name_by_id(run_name_or_id)
         elif self._folder.file_exists(run_name_or_id):
             # Run name was given in its entirety
             return run_name_or_id
         else:
             # Maybe run name was given without optional parts, e.g., NET-123 instead of NET-123-more-dropout
```

### Comparing `elias-0.2.0/src/elias/manager/analysis.py` & `elias-0.2.1/src/elias/manager/analysis.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.0/src/elias/manager/artifact.py` & `elias-0.2.1/src/elias/manager/artifact.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.0/src/elias/manager/buffered.py` & `elias-0.2.1/src/elias/manager/buffered.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.0/src/elias/manager/data.py` & `elias-0.2.1/src/elias/manager/data.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.0/src/elias/manager/model.py` & `elias-0.2.1/src/elias/manager/model.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.0/src/elias/manager/run.py` & `elias-0.2.1/src/elias/manager/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 #   For optional wildcards, we cannot resolve the run_name here because we don't have the name_format (only folder has)
 #   Maybe instantiation only via folders? But how to handle additional parameters in the __init__ for the manager?
 class RunManager(Generic[_ConfigType], ArtifactManager):
 
     def __init__(self, location: str, run_name: str, artifact_type=ArtifactType.JSON):
         run_location = f"{location}/{run_name}"
         assert Path(run_location).is_dir(), \
-            f"Could not find directory '{location}'. Is the path correct?"
+            f"Could not find directory '{run_location}'. Is the path correct?"
         super(RunManager, self).__init__(run_location, artifact_type=artifact_type)
 
         self._location = run_location
         self._run_name = run_name
         self._config_cls: Config = reveal_type_var(self, _ConfigType)
 
     @classmethod
```

### Comparing `elias-0.2.0/src/elias/util/fs.py` & `elias-0.2.1/src/elias/util/fs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import re
 from pathlib import Path
 from shutil import copy2
-from typing import Callable
+from typing import Callable, Union
 
 import PIL
 from PIL import Image
 
 from elias.util.range import IndexRangeBundle
 
 
@@ -23,41 +23,41 @@
     -------
         the file path with the specified extension if it did not already have that ending
     """
 
     return file if file.endswith(ending) else f"{file}.{ending}"
 
 
-def ensure_directory_exists_for_file(path: str):
+def ensure_directory_exists_for_file(path: Union[str, Path]):
     """
     Ensures that the folder to the specified path exists and creates a nested folder structure if necessary.
     Be careful to use trailing '/' if `path` directly constitutes the target folder (and not an arbitrary file
     within that folder).
 
     Parameters
     ----------
         path: path to the file or folder for which an underlying directory structure will be ensured
     """
 
     Path(os.path.dirname(str(path))).mkdir(parents=True, exist_ok=True)
 
 
-def ensure_directory_exists(path: str):
+def ensure_directory_exists(path: Union[str, Path]):
     """
     Ensures that the specified folder exists and creates a nested folder structure if necessary.
 
     Parameters
     ----------
         path: path to the folder which should exist
     """
 
     Path(str(path)).mkdir(parents=True, exist_ok=True)
 
 
-def clear_directory(path: str):
+def clear_directory(path: Union[str, Path]):
     """
     Clears all files from the specified directory, but keeps the directory itself.
     If the directory does not exist, nothing happens.
     """
 
     path = Path(str(path))
     if path.exists():
```

### Comparing `elias-0.2.0/src/elias/util/io.py` & `elias-0.2.1/src/elias/util/io.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.0/src/elias/util/range.py` & `elias-0.2.1/src/elias/util/range.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.0/src/elias/util/timing.py` & `elias-0.2.1/src/elias/util/timing.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.0/src/elias/util/version.py` & `elias-0.2.1/src/elias/util/version.py`

 * *Files identical despite different names*

### Comparing `elias-0.2.0/src/elias.egg-info/PKG-INFO` & `elias-0.2.1/src/elias.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elias
-Version: 0.2.0
+Version: 0.2.1
 Summary: ELIAS experiment library for facilitating machine learning projects
 Home-page: https://github.com/tobias-kirschstein/elias
 Author: Tobias Kirschstein
 Author-email: tobias.kirschstein@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `elias-0.2.0/src/elias.egg-info/SOURCES.txt` & `elias-0.2.1/src/elias.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -29,8 +29,9 @@
 src/elias/manager/model.py
 src/elias/manager/run.py
 src/elias/util/__init__.py
 src/elias/util/fs.py
 src/elias/util/io.py
 src/elias/util/range.py
 src/elias/util/timing.py
+src/elias/util/typing.py
 src/elias/util/version.py
```

