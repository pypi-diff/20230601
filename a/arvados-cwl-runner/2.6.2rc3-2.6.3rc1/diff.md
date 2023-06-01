# Comparing `tmp/arvados-cwl-runner-2.6.2rc3.tar.gz` & `tmp/arvados-cwl-runner-2.6.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was ".upload_dist/arvados-cwl-runner-2.6.2rc3.tar", last modified: Mon May  1 21:20:06 2023, max compression
+gzip compressed data, was ".upload_dist/arvados-cwl-runner-2.6.3rc1.tar", last modified: Thu Jun  1 21:38:17 2023, max compression
```

## Comparing `arvados-cwl-runner-2.6.2rc3.tar` & `arvados-cwl-runner-2.6.3rc1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-05-01 21:20:06.000000 arvados-cwl-runner-2.6.2rc3/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    11358 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/LICENSE-2.0.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      168 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/MANIFEST.in
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      561 2023-05-01 21:20:06.000000 arvados-cwl-runner-2.6.2rc3/PKG-INFO
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      149 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/README.rst
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-05-01 21:20:06.000000 arvados-cwl-runner-2.6.2rc3/arvados_cwl/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    20122 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/arvados_cwl/__init__.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       25 2023-05-01 21:20:06.000000 arvados-cwl-runner-2.6.2rc3/arvados_cwl/_version.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    14343 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/arvados_cwl/arv-cwl-schema-v1.0.yml
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    12837 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/arvados_cwl/arv-cwl-schema-v1.1.yml
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    12840 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/arvados_cwl/arv-cwl-schema-v1.2.yml
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    35160 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/arvados_cwl/arvcontainer.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     6934 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/arvados_cwl/arvdocker.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     5438 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/arvados_cwl/arvtool.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    31521 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/arvados_cwl/arvworkflow.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2155 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/arvados_cwl/context.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3986 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/arvados_cwl/done.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    44529 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/arvados_cwl/executor.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    12495 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/arvados_cwl/fsaccess.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    17991 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/arvados_cwl/pathmapper.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      560 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/arvados_cwl/perf.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    39024 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/arvados_cwl/runner.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1810 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/arvados_cwl/util.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-05-01 21:20:06.000000 arvados-cwl-runner-2.6.2rc3/arvados_cwl_runner.egg-info/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      561 2023-05-01 21:20:06.000000 arvados-cwl-runner-2.6.2rc3/arvados_cwl_runner.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1135 2023-05-01 21:20:06.000000 arvados-cwl-runner-2.6.2rc3/arvados_cwl_runner.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2023-05-01 21:20:06.000000 arvados-cwl-runner-2.6.2rc3/arvados_cwl_runner.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       87 2023-05-01 21:20:06.000000 arvados-cwl-runner-2.6.2rc3/arvados_cwl_runner.egg-info/entry_points.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      177 2023-05-01 21:20:06.000000 arvados-cwl-runner-2.6.2rc3/arvados_cwl_runner.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       18 2023-05-01 21:20:06.000000 arvados-cwl-runner-2.6.2rc3/arvados_cwl_runner.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2018-09-21 15:00:40.000000 arvados-cwl-runner-2.6.2rc3/arvados_cwl_runner.egg-info/zip-safe
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2174 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/arvados_version.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-05-01 21:20:06.000000 arvados-cwl-runner-2.6.2rc3/bin/
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      217 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/bin/arvados-cwl-runner
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      217 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/bin/cwl-runner
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       38 2023-05-01 21:20:06.000000 arvados-cwl-runner-2.6.2rc3/setup.cfg
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2073 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/setup.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-05-01 21:20:06.000000 arvados-cwl-runner-2.6.2rc3/tests/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      100 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/tests/__init__.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      158 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/tests/hw.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1049 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/tests/matcher.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      416 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/tests/mock_discovery.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    73382 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/tests/test_container.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     7275 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/tests/test_copy_deps.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     5236 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/tests/test_fsaccess.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     7098 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/tests/test_make_output.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    10597 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/tests/test_pathmapper.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1299 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/tests/test_set_output_prop.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    87484 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/tests/test_submit.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1434 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/tests/test_tq.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2503 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/tests/test_urljoin.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3439 2023-05-01 21:19:49.000000 arvados-cwl-runner-2.6.2rc3/tests/test_util.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-06-01 21:38:17.000000 arvados-cwl-runner-2.6.3rc1/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    11358 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/LICENSE-2.0.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      168 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/MANIFEST.in
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      561 2023-06-01 21:38:17.000000 arvados-cwl-runner-2.6.3rc1/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      149 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/README.rst
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-06-01 21:38:17.000000 arvados-cwl-runner-2.6.3rc1/arvados_cwl/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    20500 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/arvados_cwl/__init__.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       25 2023-06-01 21:38:17.000000 arvados-cwl-runner-2.6.3rc1/arvados_cwl/_version.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    14343 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/arvados_cwl/arv-cwl-schema-v1.0.yml
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    12837 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/arvados_cwl/arv-cwl-schema-v1.1.yml
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    12840 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/arvados_cwl/arv-cwl-schema-v1.2.yml
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    35160 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/arvados_cwl/arvcontainer.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     6934 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/arvados_cwl/arvdocker.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     5438 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/arvados_cwl/arvtool.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    31521 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/arvados_cwl/arvworkflow.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2155 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/arvados_cwl/context.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3986 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/arvados_cwl/done.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    44529 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/arvados_cwl/executor.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    12495 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/arvados_cwl/fsaccess.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    17991 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/arvados_cwl/pathmapper.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      560 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/arvados_cwl/perf.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    39024 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/arvados_cwl/runner.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1810 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/arvados_cwl/util.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-06-01 21:38:17.000000 arvados-cwl-runner-2.6.3rc1/arvados_cwl_runner.egg-info/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      561 2023-06-01 21:38:17.000000 arvados-cwl-runner-2.6.3rc1/arvados_cwl_runner.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1135 2023-06-01 21:38:17.000000 arvados-cwl-runner-2.6.3rc1/arvados_cwl_runner.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2023-06-01 21:38:17.000000 arvados-cwl-runner-2.6.3rc1/arvados_cwl_runner.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       87 2023-06-01 21:38:17.000000 arvados-cwl-runner-2.6.3rc1/arvados_cwl_runner.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      177 2023-06-01 21:38:17.000000 arvados-cwl-runner-2.6.3rc1/arvados_cwl_runner.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       18 2023-06-01 21:38:17.000000 arvados-cwl-runner-2.6.3rc1/arvados_cwl_runner.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2018-09-21 15:00:40.000000 arvados-cwl-runner-2.6.3rc1/arvados_cwl_runner.egg-info/zip-safe
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2174 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/arvados_version.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-06-01 21:38:17.000000 arvados-cwl-runner-2.6.3rc1/bin/
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      217 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/bin/arvados-cwl-runner
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      217 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/bin/cwl-runner
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       38 2023-06-01 21:38:17.000000 arvados-cwl-runner-2.6.3rc1/setup.cfg
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2073 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/setup.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-06-01 21:38:17.000000 arvados-cwl-runner-2.6.3rc1/tests/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      100 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/tests/__init__.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      158 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/tests/hw.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1049 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/tests/matcher.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      416 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/tests/mock_discovery.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    73382 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/tests/test_container.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     7275 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/tests/test_copy_deps.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     5236 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/tests/test_fsaccess.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     7098 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/tests/test_make_output.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    10597 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/tests/test_pathmapper.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1299 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/tests/test_set_output_prop.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    87484 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/tests/test_submit.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1434 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/tests/test_tq.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2503 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/tests/test_urljoin.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3439 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/tests/test_util.py
```

### Comparing `arvados-cwl-runner-2.6.2rc3/LICENSE-2.0.txt` & `arvados-cwl-runner-2.6.3rc1/LICENSE-2.0.txt`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc3/PKG-INFO` & `arvados-cwl-runner-2.6.3rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: arvados-cwl-runner
-Version: 2.6.2rc3
+Version: 2.6.3rc1
 Summary: Arvados Common Workflow Language runner
 Home-page: https://arvados.org
 Author: Arvados
 Author-email: info@arvados.org
 License: Apache 2.0
 Download-URL: https://github.com/arvados/arvados.git
 Description: .. Copyright (C) The Arvados Authors. All rights reserved.
```

### Comparing `arvados-cwl-runner-2.6.2rc3/arvados_cwl/__init__.py` & `arvados-cwl-runner-2.6.3rc1/arvados_cwl/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,18 @@
 
     return "%s %s, %s %s, %s %s" % (sys.argv[0], arvcwlpkg[0].version,
                                     "arvados-python-client", arvpkg[0].version,
                                     "cwltool", cwlpkg[0].version)
 
 
 def arg_parser():  # type: () -> argparse.ArgumentParser
-    parser = argparse.ArgumentParser(description='Arvados executor for Common Workflow Language')
+    parser = argparse.ArgumentParser(
+        description='Arvados executor for Common Workflow Language',
+        parents=[arv_cmd.retry_opt],
+    )
 
     parser.add_argument("--basedir",
                         help="Base directory used to resolve relative references in the input, default to directory of input object file or current directory (if inputs piped/provided on command line).")
     parser.add_argument("--outdir", default=os.path.abspath('.'),
                         help="Output directory, default current directory")
 
     parser.add_argument("--eval-timeout",
@@ -329,25 +332,41 @@
     for key, val in viewitems(cwltool.argparser.get_default_args()):
         if not hasattr(arvargs, key):
             setattr(arvargs, key, val)
 
     try:
         if api_client is None:
             api_client = arvados.safeapi.ThreadSafeApiCache(
-                api_params={"model": OrderedJsonModel(), "timeout": arvargs.http_timeout},
-                keep_params={"num_retries": 4},
+                api_params={
+                    'model': OrderedJsonModel(),
+                    'num_retries': arvargs.retries,
+                    'timeout': arvargs.http_timeout,
+                },
+                keep_params={
+                    'num_retries': arvargs.retries,
+                },
                 version='v1',
             )
             keep_client = api_client.keep
             # Make an API object now so errors are reported early.
             api_client.users().current().execute()
         if keep_client is None:
             block_cache = arvados.keep.KeepBlockCache(disk_cache=True)
-            keep_client = arvados.keep.KeepClient(api_client=api_client, num_retries=4, block_cache=block_cache)
-        executor = ArvCwlExecutor(api_client, arvargs, keep_client=keep_client, num_retries=4, stdout=stdout)
+            keep_client = arvados.keep.KeepClient(
+                api_client=api_client,
+                block_cache=block_cache,
+                num_retries=arvargs.retries,
+            )
+        executor = ArvCwlExecutor(
+            api_client,
+            arvargs,
+            keep_client=keep_client,
+            num_retries=arvargs.retries,
+            stdout=stdout,
+        )
     except WorkflowException as e:
         logger.error(e, exc_info=(sys.exc_info()[1] if arvargs.debug else False))
         return 1
     except Exception:
         logger.exception("Error creating the Arvados CWL Executor")
         return 1
```

### Comparing `arvados-cwl-runner-2.6.2rc3/arvados_cwl/arv-cwl-schema-v1.0.yml` & `arvados-cwl-runner-2.6.3rc1/arvados_cwl/arv-cwl-schema-v1.0.yml`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc3/arvados_cwl/arv-cwl-schema-v1.1.yml` & `arvados-cwl-runner-2.6.3rc1/arvados_cwl/arv-cwl-schema-v1.1.yml`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc3/arvados_cwl/arv-cwl-schema-v1.2.yml` & `arvados-cwl-runner-2.6.3rc1/arvados_cwl/arv-cwl-schema-v1.2.yml`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc3/arvados_cwl/arvcontainer.py` & `arvados-cwl-runner-2.6.3rc1/arvados_cwl/arvcontainer.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc3/arvados_cwl/arvdocker.py` & `arvados-cwl-runner-2.6.3rc1/arvados_cwl/arvdocker.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc3/arvados_cwl/arvtool.py` & `arvados-cwl-runner-2.6.3rc1/arvados_cwl/arvtool.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc3/arvados_cwl/arvworkflow.py` & `arvados-cwl-runner-2.6.3rc1/arvados_cwl/arvworkflow.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc3/arvados_cwl/context.py` & `arvados-cwl-runner-2.6.3rc1/arvados_cwl/context.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc3/arvados_cwl/done.py` & `arvados-cwl-runner-2.6.3rc1/arvados_cwl/done.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc3/arvados_cwl/executor.py` & `arvados-cwl-runner-2.6.3rc1/arvados_cwl/executor.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc3/arvados_cwl/fsaccess.py` & `arvados-cwl-runner-2.6.3rc1/arvados_cwl/fsaccess.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc3/arvados_cwl/pathmapper.py` & `arvados-cwl-runner-2.6.3rc1/arvados_cwl/pathmapper.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc3/arvados_cwl/perf.py` & `arvados-cwl-runner-2.6.3rc1/arvados_cwl/perf.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc3/arvados_cwl/runner.py` & `arvados-cwl-runner-2.6.3rc1/arvados_cwl/runner.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc3/arvados_cwl/util.py` & `arvados-cwl-runner-2.6.3rc1/arvados_cwl/util.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc3/arvados_cwl_runner.egg-info/PKG-INFO` & `arvados-cwl-runner-2.6.3rc1/arvados_cwl_runner.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: arvados-cwl-runner
-Version: 2.6.2rc3
+Version: 2.6.3rc1
 Summary: Arvados Common Workflow Language runner
 Home-page: https://arvados.org
 Author: Arvados
 Author-email: info@arvados.org
 License: Apache 2.0
 Download-URL: https://github.com/arvados/arvados.git
 Description: .. Copyright (C) The Arvados Authors. All rights reserved.
```

### Comparing `arvados-cwl-runner-2.6.2rc3/arvados_cwl_runner.egg-info/SOURCES.txt` & `arvados-cwl-runner-2.6.3rc1/arvados_cwl_runner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc3/arvados_version.py` & `arvados-cwl-runner-2.6.3rc1/arvados_version.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc3/setup.py` & `arvados-cwl-runner-2.6.3rc1/setup.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc3/tests/matcher.py` & `arvados-cwl-runner-2.6.3rc1/tests/matcher.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc3/tests/test_container.py` & `arvados-cwl-runner-2.6.3rc1/tests/test_container.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc3/tests/test_copy_deps.py` & `arvados-cwl-runner-2.6.3rc1/tests/test_copy_deps.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc3/tests/test_fsaccess.py` & `arvados-cwl-runner-2.6.3rc1/tests/test_fsaccess.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc3/tests/test_make_output.py` & `arvados-cwl-runner-2.6.3rc1/tests/test_make_output.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc3/tests/test_pathmapper.py` & `arvados-cwl-runner-2.6.3rc1/tests/test_pathmapper.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc3/tests/test_set_output_prop.py` & `arvados-cwl-runner-2.6.3rc1/tests/test_set_output_prop.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc3/tests/test_submit.py` & `arvados-cwl-runner-2.6.3rc1/tests/test_submit.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc3/tests/test_tq.py` & `arvados-cwl-runner-2.6.3rc1/tests/test_tq.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc3/tests/test_urljoin.py` & `arvados-cwl-runner-2.6.3rc1/tests/test_urljoin.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.2rc3/tests/test_util.py` & `arvados-cwl-runner-2.6.3rc1/tests/test_util.py`

 * *Files identical despite different names*

