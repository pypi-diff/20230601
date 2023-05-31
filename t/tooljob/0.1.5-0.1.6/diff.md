# Comparing `tmp/tooljob-0.1.5.tar.gz` & `tmp/tooljob-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tooljob-0.1.5.tar", last modified: Mon May  8 07:02:16 2023, max compression
+gzip compressed data, was "tooljob-0.1.6.tar", last modified: Wed May 31 22:18:10 2023, max compression
```

## Comparing `tooljob-0.1.5.tar` & `tooljob-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      217 2023-02-26 19:33:55.835763 tooljob-0.1.5/.gitignore
--rw-r--r--   0        0        0      742 2023-02-26 02:20:54.175448 tooljob-0.1.5/README.md
--rw-r--r--   0        0        0      415 2023-05-08 06:56:59.204627 tooljob-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      147 2023-05-08 07:01:48.588575 tooljob-0.1.5/tooljob/__init__.py
--rw-r--r--   0        0        0    14215 2023-05-08 06:45:08.492429 tooljob-0.1.5/tooljob/batch_class.py
--rw-r--r--   0        0        0        0 2023-04-10 03:48:04.176428 tooljob-0.1.5/tooljob/py.typed
--rw-r--r--   0        0        0       68 2023-02-26 07:21:03.717968 tooljob-0.1.5/tooljob/spec/__init__.py
--rw-r--r--   0        0        0      521 2023-05-02 23:13:32.556227 tooljob-0.1.5/tooljob/spec/typedefs.py
--rw-r--r--   0        0        0       29 2023-02-26 07:48:30.506903 tooljob-0.1.5/tooljob/trackers/__init__.py
--rw-r--r--   0        0        0      197 2023-02-26 06:53:20.062932 tooljob-0.1.5/tooljob/trackers/bucket_tracker.py
--rw-r--r--   0        0        0     2618 2023-05-08 05:19:34.316554 tooljob-0.1.5/tooljob/trackers/file_tracker.py
--rw-r--r--   0        0        0     5824 2023-05-08 05:41:56.460788 tooljob-0.1.5/tooljob/trackers/multifile_tracker.py
--rw-r--r--   0        0        0     5358 2023-02-26 19:46:45.227524 tooljob-0.1.5/tooljob/trackers/sql_tracker.py
--rw-r--r--   0        0        0      736 2023-05-08 06:39:33.315696 tooljob-0.1.5/tooljob/trackers/tracker.py
--rw-r--r--   0        0        0     2321 2023-05-02 23:14:50.134997 tooljob-0.1.5/tooljob/trackers/tracker_utils.py
--rw-r--r--   0        0        0      281 1970-01-01 00:00:00.000000 tooljob-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      217 2023-02-26 19:33:55.835763 tooljob-0.1.6/.gitignore
+-rw-r--r--   0        0        0      742 2023-02-26 02:20:54.175448 tooljob-0.1.6/README.md
+-rw-r--r--   0        0        0      415 2023-05-08 06:56:59.204627 tooljob-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      147 2023-05-31 22:18:05.135091 tooljob-0.1.6/tooljob/__init__.py
+-rw-r--r--   0        0        0    14245 2023-05-30 06:26:48.269493 tooljob-0.1.6/tooljob/batch_class.py
+-rw-r--r--   0        0        0        0 2023-04-10 03:48:04.176428 tooljob-0.1.6/tooljob/py.typed
+-rw-r--r--   0        0        0       68 2023-02-26 07:21:03.717968 tooljob-0.1.6/tooljob/spec/__init__.py
+-rw-r--r--   0        0        0      521 2023-05-02 23:13:32.556227 tooljob-0.1.6/tooljob/spec/typedefs.py
+-rw-r--r--   0        0        0       29 2023-02-26 07:48:30.506903 tooljob-0.1.6/tooljob/trackers/__init__.py
+-rw-r--r--   0        0        0      197 2023-02-26 06:53:20.062932 tooljob-0.1.6/tooljob/trackers/bucket_tracker.py
+-rw-r--r--   0        0        0     2618 2023-05-08 05:19:34.316554 tooljob-0.1.6/tooljob/trackers/file_tracker.py
+-rw-r--r--   0        0        0     5839 2023-05-30 06:21:25.602685 tooljob-0.1.6/tooljob/trackers/multifile_tracker.py
+-rw-r--r--   0        0        0     5358 2023-02-26 19:46:45.227524 tooljob-0.1.6/tooljob/trackers/sql_tracker.py
+-rw-r--r--   0        0        0      736 2023-05-08 06:39:33.315696 tooljob-0.1.6/tooljob/trackers/tracker.py
+-rw-r--r--   0        0        0     2387 2023-05-31 22:18:05.136330 tooljob-0.1.6/tooljob/trackers/tracker_utils.py
+-rw-r--r--   0        0        0      281 1970-01-01 00:00:00.000000 tooljob-0.1.6/PKG-INFO
```

### Comparing `tooljob-0.1.5/README.md` & `tooljob-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `tooljob-0.1.5/tooljob/batch_class.py` & `tooljob-0.1.6/tooljob/batch_class.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     def __init__(
         self,
         *,
         jobs: typing.Sequence[spec.JobData] | None = None,
         tracker: str | None = None,
         output_dir: str | None = None,
         output_filetype: str | None = None,
-        outputs: typing.Mapping[str, str] | None = None,
+        outputs: spec.ShorthandOutputsSpec | None = None,
         db_config: toolsql.DBConfig | None = None,
         bucket_path: str | None = None,
         name: str | None = None,
         styles: toolcli.StyleTheme | None = None,
         verbose: bool = False,
     ) -> None:
         self.name = name
@@ -49,14 +49,15 @@
             styles = {}
         self.styles = styles
         self.verbose = verbose
         self.tracker = trackers.create_tracker(
             tracker=tracker,
             output_dir=output_dir,
             output_filetype=output_filetype,
+            outputs=outputs,
             db_config=db_config,
             bucket_path=bucket_path,
             batch=self,
         )
 
     #
     # # names
```

### Comparing `tooljob-0.1.5/tooljob/spec/typedefs.py` & `tooljob-0.1.6/tooljob/spec/typedefs.py`

 * *Files identical despite different names*

### Comparing `tooljob-0.1.5/tooljob/trackers/file_tracker.py` & `tooljob-0.1.6/tooljob/trackers/file_tracker.py`

 * *Files identical despite different names*

### Comparing `tooljob-0.1.5/tooljob/trackers/multifile_tracker.py` & `tooljob-0.1.6/tooljob/trackers/multifile_tracker.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,19 +45,19 @@
     """
 
     outputs: spec.OutputsSpec
 
     def __init__(
         self,
         outputs: spec.ShorthandOutputsSpec,
-        output_dir: str | None,
-        output_filetype: str | None,
+        output_dir: str | None = None,
+        output_filetype: str | None = None,
         **kwargs: typing.Any,
     ) -> None:
-        # compile output specifications
+        # compile outputs specifications
         strict_outputs: typing.MutableMapping[str, spec.OutputSpec] = {}
         if isinstance(outputs, list):
             for output in outputs:
                 if isinstance(output, str):
                     strict_outputs[output] = _get_output_dict(
                         default_output_dir=output_dir,
                         default_output_filetype=output_filetype,
```

### Comparing `tooljob-0.1.5/tooljob/trackers/sql_tracker.py` & `tooljob-0.1.6/tooljob/trackers/sql_tracker.py`

 * *Files identical despite different names*

### Comparing `tooljob-0.1.5/tooljob/trackers/tracker.py` & `tooljob-0.1.6/tooljob/trackers/tracker.py`

 * *Files identical despite different names*

### Comparing `tooljob-0.1.5/tooljob/trackers/tracker_utils.py` & `tooljob-0.1.6/tooljob/trackers/tracker_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 
 import typing
 
 if typing.TYPE_CHECKING:
-
     import toolsql
 
     from .. import batch_class
     from .. import spec
     from . import tracker
 
 
@@ -17,18 +16,19 @@
     output_dir: str | None = None,
     output_filetype: str | None = None,
     outputs: spec.ShorthandOutputsSpec | None = None,
     db_config: toolsql.DBConfig | None = None,
     bucket_path: str | None = None,
     batch: batch_class.Batch | None = None,
 ) -> tracker.Tracker:
-
     # determine tracker
     if tracker is None:
-        if output_dir is not None and output_filetype is not None:
+        if outputs is not None:
+            tracker = 'multifile'
+        elif output_dir is not None and output_filetype is not None:
             tracker = 'file'
         elif db_config is not None:
             tracker = 'sql'
         elif bucket_path is not None:
             tracker = 'bucket'
         else:
             raise Exception('invalid tracker: ' + str(tracker))
```

