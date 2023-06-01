# Comparing `tmp/adaptive_scheduler-2.0.1.tar.gz` & `tmp/adaptive_scheduler-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adaptive_scheduler-2.0.1.tar", last modified: Wed May 17 22:57:18 2023, max compression
+gzip compressed data, was "adaptive_scheduler-2.1.0.tar", last modified: Thu Jun  1 18:29:37 2023, max compression
```

## Comparing `adaptive_scheduler-2.0.1.tar` & `adaptive_scheduler-2.1.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:57:18.053563 adaptive_scheduler-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-17 22:57:18.053563 adaptive_scheduler-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8242 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:57:18.053563 adaptive_scheduler-2.0.1/adaptive_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/adaptive_scheduler/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7755 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/adaptive_scheduler/_mock_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:57:18.045563 adaptive_scheduler-2.0.1/adaptive_scheduler/_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/adaptive_scheduler/_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12733 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/adaptive_scheduler/_scheduler/base_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/adaptive_scheduler/_scheduler/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/adaptive_scheduler/_scheduler/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     8670 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/adaptive_scheduler/_scheduler/pbs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/adaptive_scheduler/_scheduler/slurm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:57:18.049563 adaptive_scheduler-2.0.1/adaptive_scheduler/_server_support/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/adaptive_scheduler/_server_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/adaptive_scheduler/_server_support/base_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/adaptive_scheduler/_server_support/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    13282 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/adaptive_scheduler/_server_support/database_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/adaptive_scheduler/_server_support/job_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/adaptive_scheduler/_server_support/kill_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/adaptive_scheduler/_server_support/launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/adaptive_scheduler/_server_support/parse_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21460 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/adaptive_scheduler/_server_support/run_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/adaptive_scheduler/_server_support/slurm_run.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-17 22:57:18.053563 adaptive_scheduler-2.0.1/adaptive_scheduler/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/adaptive_scheduler/client_support.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/adaptive_scheduler/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/adaptive_scheduler/server_support.py
--rw-r--r--   0 runner    (1001) docker     (123)    35819 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/adaptive_scheduler/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    32694 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/adaptive_scheduler/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:57:18.045563 adaptive_scheduler-2.0.1/adaptive_scheduler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-17 22:57:18.000000 adaptive_scheduler-2.0.1/adaptive_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-17 22:57:18.000000 adaptive_scheduler-2.0.1/adaptive_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 22:57:18.000000 adaptive_scheduler-2.0.1/adaptive_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-17 22:57:18.000000 adaptive_scheduler-2.0.1/adaptive_scheduler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-17 22:57:18.000000 adaptive_scheduler-2.0.1/adaptive_scheduler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-17 22:57:18.000000 adaptive_scheduler-2.0.1/adaptive_scheduler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-17 22:57:18.053563 adaptive_scheduler-2.0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      523 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:57:18.053563 adaptive_scheduler-2.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/tests/test_base_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/tests/test_client_support.py
--rw-r--r--   0 runner    (1001) docker     (123)    13256 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/tests/test_database_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/tests/test_job_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6801 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/tests/test_kill_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/tests/test_launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/tests/test_log_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/tests/test_log_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    10239 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/tests/test_run_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/tests/test_server_support_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     8312 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/tests/test_slurm_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     8731 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/tests/test_slurm_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    16970 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10801 2023-05-17 22:56:55.000000 adaptive_scheduler-2.0.1/tests/test_widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:29:37.103995 adaptive_scheduler-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-01 18:29:22.000000 adaptive_scheduler-2.1.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-01 18:29:22.000000 adaptive_scheduler-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-01 18:29:22.000000 adaptive_scheduler-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-01 18:29:37.103995 adaptive_scheduler-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8242 2023-06-01 18:29:22.000000 adaptive_scheduler-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:29:37.103995 adaptive_scheduler-2.1.0/adaptive_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-01 18:29:22.000000 adaptive_scheduler-2.1.0/adaptive_scheduler/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8025 2023-06-01 18:29:22.000000 adaptive_scheduler-2.1.0/adaptive_scheduler/_mock_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:29:37.099995 adaptive_scheduler-2.1.0/adaptive_scheduler/_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:29:22.000000 adaptive_scheduler-2.1.0/adaptive_scheduler/_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12740 2023-06-01 18:29:22.000000 adaptive_scheduler-2.1.0/adaptive_scheduler/_scheduler/base_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-01 18:29:22.000000 adaptive_scheduler-2.1.0/adaptive_scheduler/_scheduler/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-06-01 18:29:22.000000 adaptive_scheduler-2.1.0/adaptive_scheduler/_scheduler/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8670 2023-06-01 18:29:22.000000 adaptive_scheduler-2.1.0/adaptive_scheduler/_scheduler/pbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-06-01 18:29:22.000000 adaptive_scheduler-2.1.0/adaptive_scheduler/_scheduler/slurm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:29:37.099995 adaptive_scheduler-2.1.0/adaptive_scheduler/_server_support/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-01 18:29:22.000000 adaptive_scheduler-2.1.0/adaptive_scheduler/_server_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-01 18:29:22.000000 adaptive_scheduler-2.1.0/adaptive_scheduler/_server_support/base_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-06-01 18:29:22.000000 adaptive_scheduler-2.1.0/adaptive_scheduler/_server_support/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13265 2023-06-01 18:29:22.000000 adaptive_scheduler-2.1.0/adaptive_scheduler/_server_support/database_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11146 2023-06-01 18:29:22.000000 adaptive_scheduler-2.1.0/adaptive_scheduler/_server_support/job_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-06-01 18:29:22.000000 adaptive_scheduler-2.1.0/adaptive_scheduler/_server_support/kill_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-06-01 18:29:22.000000 adaptive_scheduler-2.1.0/adaptive_scheduler/_server_support/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-06-01 18:29:22.000000 adaptive_scheduler-2.1.0/adaptive_scheduler/_server_support/parse_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21459 2023-06-01 18:29:22.000000 adaptive_scheduler-2.1.0/adaptive_scheduler/_server_support/run_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-06-01 18:29:22.000000 adaptive_scheduler-2.1.0/adaptive_scheduler/_server_support/slurm_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-01 18:29:37.103995 adaptive_scheduler-2.1.0/adaptive_scheduler/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-06-01 18:29:22.000000 adaptive_scheduler-2.1.0/adaptive_scheduler/client_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-01 18:29:22.000000 adaptive_scheduler-2.1.0/adaptive_scheduler/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-01 18:29:22.000000 adaptive_scheduler-2.1.0/adaptive_scheduler/server_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35816 2023-06-01 18:29:22.000000 adaptive_scheduler-2.1.0/adaptive_scheduler/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32660 2023-06-01 18:29:22.000000 adaptive_scheduler-2.1.0/adaptive_scheduler/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:29:37.099995 adaptive_scheduler-2.1.0/adaptive_scheduler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-01 18:29:37.000000 adaptive_scheduler-2.1.0/adaptive_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-06-01 18:29:37.000000 adaptive_scheduler-2.1.0/adaptive_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 18:29:37.000000 adaptive_scheduler-2.1.0/adaptive_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-01 18:29:37.000000 adaptive_scheduler-2.1.0/adaptive_scheduler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-01 18:29:37.000000 adaptive_scheduler-2.1.0/adaptive_scheduler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-01 18:29:37.000000 adaptive_scheduler-2.1.0/adaptive_scheduler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-06-01 18:29:22.000000 adaptive_scheduler-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-01 18:29:37.103995 adaptive_scheduler-2.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      523 2023-06-01 18:29:22.000000 adaptive_scheduler-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:29:37.103995 adaptive_scheduler-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-06-01 18:29:22.000000 adaptive_scheduler-2.1.0/tests/test_base_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-06-01 18:29:22.000000 adaptive_scheduler-2.1.0/tests/test_client_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13256 2023-06-01 18:29:22.000000 adaptive_scheduler-2.1.0/tests/test_database_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-06-01 18:29:22.000000 adaptive_scheduler-2.1.0/tests/test_job_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6801 2023-06-01 18:29:22.000000 adaptive_scheduler-2.1.0/tests/test_kill_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-01 18:29:22.000000 adaptive_scheduler-2.1.0/tests/test_launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-06-01 18:29:22.000000 adaptive_scheduler-2.1.0/tests/test_log_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-06-01 18:29:22.000000 adaptive_scheduler-2.1.0/tests/test_log_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10239 2023-06-01 18:29:22.000000 adaptive_scheduler-2.1.0/tests/test_run_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-06-01 18:29:22.000000 adaptive_scheduler-2.1.0/tests/test_server_support_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8312 2023-06-01 18:29:22.000000 adaptive_scheduler-2.1.0/tests/test_slurm_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8731 2023-06-01 18:29:22.000000 adaptive_scheduler-2.1.0/tests/test_slurm_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16981 2023-06-01 18:29:22.000000 adaptive_scheduler-2.1.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10801 2023-06-01 18:29:22.000000 adaptive_scheduler-2.1.0/tests/test_widgets.py
```

### Comparing `adaptive_scheduler-2.0.1/LICENSE` & `adaptive_scheduler-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.1/PKG-INFO` & `adaptive_scheduler-2.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adaptive_scheduler
-Version: 2.0.1
+Version: 2.1.0
 Summary: Run many `adaptive.Learner`s on many cores (>10k) using `mpi4py.futures`, `ipyparallel`, `dask-mpi`, or `process-pool`.
 Maintainer-email: Bas Nijholt <bas@nijho.lt>
 License: BSD-3
 Project-URL: homepage, https://adaptive-scheduler.readthedocs.io/
 Project-URL: documentation, https://adaptive-scheduler.readthedocs.io/
 Project-URL: repository, https://github.com/basnijholt/adaptive-scheduler
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `adaptive_scheduler-2.0.1/README.md` & `adaptive_scheduler-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.1/adaptive_scheduler/_mock_scheduler.py` & `adaptive_scheduler-2.1.0/adaptive_scheduler/_mock_scheduler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python
 from __future__ import annotations
 
 import asyncio
 import datetime
 import logging
 import os
+import signal
 import subprocess
 from typing import TYPE_CHECKING, List, Tuple, Union
 
 import structlog
 import zmq
 import zmq.asyncio
 from toolz.dicttoolz import dissoc
@@ -93,49 +94,53 @@
         return n_running >= self.max_running_jobs
 
     def _get_new_job_id(self) -> str:
         job_id = self._job_id
         self._job_id += 1
         return str(job_id)
 
-    async def _submit_coro(self, job_id: str, fname: str) -> None:
+    async def _submit_coro(self, job_name: str, job_id: str, fname: str) -> None:
         await asyncio.sleep(self.startup_delay)
         while self._queue_is_full():
             await asyncio.sleep(self.refresh_interval)
-        self._submit(job_id, fname)
+        self._submit(job_name, job_id, fname)
 
-    def _submit(self, job_id: str, fname: str) -> None:
+    def _submit(self, job_name: str, job_id: str, fname: str) -> None:
         if job_id in self._current_queue:
             # job_id could be cancelled before it started
             cmd = f"{self.bash} {fname}"
             proc = subprocess.Popen(
                 cmd.split(),
                 stdout=subprocess.PIPE,
-                env=dict(os.environ, JOB_ID=job_id),
+                env=dict(os.environ, JOB_ID=job_id, NAME=job_name),
+                preexec_fn=os.setpgrp,  # Set a new process group for the process
             )
             info = self._current_queue[job_id]
             info["proc"] = proc
             info["state"] = "R"
 
     def submit(self, job_name: str, fname: str) -> str:
         job_id = self._get_new_job_id()
         self._current_queue[job_id] = {
             "job_name": job_name,
             "proc": None,
             "state": "P",
             "timestamp": str(datetime.datetime.now()),  # noqa: DTZ005
         }
-        self.ioloop.create_task(self._submit_coro(job_id, fname))
+        self.ioloop.create_task(self._submit_coro(job_name, job_id, fname))
         return job_id
 
     def cancel(self, job_id: str) -> None:
         job_id = str(job_id)
         info = self._current_queue.pop(job_id)
         if info["proc"] is not None:
-            info["proc"].kill()
+            os.killpg(
+                os.getpgid(info["proc"].pid),
+                signal.SIGTERM,
+            )  # Kill the process group
 
     async def _refresh_coro(self) -> Coroutine[None, None, None]:
         while True:
             try:
                 await asyncio.sleep(self.refresh_interval)
                 self._refresh()
             except Exception as e:  # noqa: BLE001
```

### Comparing `adaptive_scheduler-2.0.1/adaptive_scheduler/_scheduler/base_scheduler.py` & `adaptive_scheduler-2.1.0/adaptive_scheduler/_scheduler/base_scheduler.py`

 * *Files 0% similar despite different names*

```diff
@@ -340,15 +340,15 @@
         """Writes a job script."""
         with self.batch_fname(name).open("w", encoding="utf-8") as f:
             job_script = self.job_script(options)
             f.write(job_script)
 
     def start_job(self, name: str) -> None:
         """Writes a job script and submits it to the scheduler."""
-        submit_cmd = f"{self.submit_cmd} {self.batch_fname(name)}"
+        submit_cmd = f"{self.submit_cmd} {name} {self.batch_fname(name)}"
         run_submit(submit_cmd)
 
     def __getstate__(self) -> dict[str, Any]:
         """Return the state of the scheduler."""
         return {
             "cores": self.cores,
             "python_executable": self.python_executable,
```

### Comparing `adaptive_scheduler-2.0.1/adaptive_scheduler/_scheduler/common.py` & `adaptive_scheduler-2.1.0/adaptive_scheduler/_scheduler/common.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.1/adaptive_scheduler/_scheduler/local.py` & `adaptive_scheduler-2.1.0/adaptive_scheduler/_scheduler/local.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 """LocalMockScheduler for Adaptive Scheduler."""
 from __future__ import annotations
 
 import textwrap
-import warnings
 from typing import TYPE_CHECKING
 
 from adaptive_scheduler._scheduler.base_scheduler import BaseScheduler
 from adaptive_scheduler._scheduler.common import run_submit
 
 if TYPE_CHECKING:
     from pathlib import Path
     from typing import Any
 
     from adaptive_scheduler.utils import EXECUTOR_TYPES
 
 
 class LocalMockScheduler(BaseScheduler):
-    """A scheduler that can be used for testing and runs locally.
-
-    CANCELLING DOESN'T WORK ATM, ALSO LEAVES ZOMBIE PROCESSES!
-    """
+    """A scheduler that can be used for testing and runs locally."""
 
     # Attributes that all schedulers need to have
     _ext = ".batch"
     _JOB_ID_VARIABLE = "${JOB_ID}"
 
     def __init__(
         self,
@@ -40,15 +36,14 @@
         batch_folder: str | Path = "",
         # LocalMockScheduler specific
         mock_scheduler_kwargs: dict[str, Any] | None = None,
     ) -> None:
         """Initialize the LocalMockScheduler."""
         import adaptive_scheduler._mock_scheduler
 
-        warnings.warn("The LocalMockScheduler currently doesn't work!", stacklevel=2)
         super().__init__(
             cores,
             python_executable=python_executable,
             log_folder=log_folder,
             mpiexec_executable=mpiexec_executable,
             executor_type=executor_type,
             num_threads=num_threads,
@@ -114,15 +109,16 @@
 
     def queue(self, *, me_only: bool = True) -> dict[str, dict]:  # noqa: ARG002
         """Get the queue of the scheduler."""
         return self.mock_scheduler.queue()
 
     def start_job(self, name: str) -> None:
         """Start a job."""
-        submit_cmd = f"{self.submit_cmd} {name} {self.batch_fname(name)}"
+        name_prefix = name.rsplit("-", 1)[0]
+        submit_cmd = f"{self.submit_cmd} {name} {self.batch_fname(name_prefix)}"
         run_submit(submit_cmd, name)
 
     @property
     def extra_scheduler(self) -> str:
         """Get the extra scheduler options."""
         msg = "extra_scheduler is not implemented."
         raise NotImplementedError(msg)
```

### Comparing `adaptive_scheduler-2.0.1/adaptive_scheduler/_scheduler/pbs.py` & `adaptive_scheduler-2.1.0/adaptive_scheduler/_scheduler/pbs.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.1/adaptive_scheduler/_scheduler/slurm.py` & `adaptive_scheduler-2.1.0/adaptive_scheduler/_scheduler/slurm.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.1/adaptive_scheduler/_server_support/base_manager.py` & `adaptive_scheduler-2.1.0/adaptive_scheduler/_server_support/base_manager.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.1/adaptive_scheduler/_server_support/common.py` & `adaptive_scheduler-2.1.0/adaptive_scheduler/_server_support/common.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.1/adaptive_scheduler/_server_support/database_manager.py` & `adaptive_scheduler-2.1.0/adaptive_scheduler/_server_support/database_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,15 @@
 
     Attributes
     ----------
     failed : list
         A list of entries that have failed and have been removed from the database.
     """
 
-    def __init__(  # noqa: PLR0913
+    def __init__(
         self,
         url: str,
         scheduler: BaseScheduler,
         db_fname: str | Path,
         learners: list[adaptive.BaseLearner],
         fnames: FnamesTypes,
         *,
```

### Comparing `adaptive_scheduler-2.0.1/adaptive_scheduler/_server_support/job_manager.py` & `adaptive_scheduler-2.1.0/adaptive_scheduler/_server_support/job_manager.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,18 +25,50 @@
     scheduler: BaseScheduler,
     database_manager: DatabaseManager,
     runner_kwargs: dict[str, Any] | None = None,
     goal: GoalTypes,
     log_interval: int | float = 60,
     save_interval: int | float = 300,
     save_dataframe: bool = True,
-    dataframe_format: _DATAFRAME_FORMATS = "parquet",
+    dataframe_format: _DATAFRAME_FORMATS = "pickle",
     loky_start_method: LOKY_START_METHODS = "loky",
 ) -> dict[str, Any]:
-    """Return the command line options for the job_script."""
+    """Return the command line options for the job_script.
+
+    Parameters
+    ----------
+    scheduler : `~adaptive_scheduler.scheduler.BaseScheduler`
+        A scheduler instance from `adaptive_scheduler.scheduler`.
+    database_manager
+        A database manager instance.
+    runner_kwargs : dict, default: None
+        Extra keyword argument to pass to the `adaptive.Runner`. Note that this dict
+        will be serialized and pasted in the ``job_script``.
+    goal : callable, default: None
+        The goal passed to the `adaptive.Runner`. Note that this function will
+        be serialized and pasted in the ``job_script``. Can be a smart-goal
+        that accepts
+        ``Callable[[adaptive.BaseLearner], bool] | int | float | datetime | timedelta | None``.
+        See `adaptive_scheduler.utils.smart_goal` for more information.
+    log_interval : int, default: 300
+        Time in seconds between log entries.
+    save_interval : int, default: 300
+        Time in seconds between saving of the learners.
+    save_dataframe : bool
+        Whether to periodically save the learner's data as a `pandas.DataFame`.
+    dataframe_format : str
+        The format in which to save the `pandas.DataFame`. See the type hint for the options.
+    loky_start_method : str
+        Loky start method, by default "loky".
+
+    Returns
+    -------
+    dict
+        The command line options for the job_script.
+    """
     if runner_kwargs is None:
         runner_kwargs = {}
     runner_kwargs["goal"] = goal
     base64_runner_kwargs = _serialize_to_b64(runner_kwargs)
     n = scheduler.cores
     if scheduler.executor_type == "ipyparallel":
         n -= 1
@@ -78,14 +110,33 @@
         jobs will run forever, resulting in the jobs that were not initially started
         (because of this `max_simultaneous_jobs` condition) to not ever start.
     max_fails_per_job : int, default: 40
         Maximum number of times that a job can fail. This is here as a fail switch
         because a job might fail instantly because of a bug inside your code.
         The job manager will stop when
         ``n_jobs * total_number_of_jobs_failed > max_fails_per_job`` is true.
+    save_dataframe : bool
+        Whether to periodically save the learner's data as a `pandas.DataFame`.
+    dataframe_format : str
+        The format in which to save the `pandas.DataFame`. See the type hint for the options.
+    loky_start_method : str
+        Loky start method, by default "loky".
+    log_interval : int, default: 300
+        Time in seconds between log entries.
+    save_interval : int, default: 300
+        Time in seconds between saving of the learners.
+    runner_kwargs : dict, default: None
+        Extra keyword argument to pass to the `adaptive.Runner`. Note that this dict
+        will be serialized and pasted in the ``job_script``.
+    goal : callable, default: None
+        The goal passed to the `adaptive.Runner`. Note that this function will
+        be serialized and pasted in the ``job_script``. Can be a smart-goal
+        that accepts
+        ``Callable[[adaptive.BaseLearner], bool] | int | float | datetime | timedelta | None``.
+        See `adaptive_scheduler.utils.smart_goal` for more information.
 
     Attributes
     ----------
     n_started : int
         Total number of jobs started by the `JobManager`.
     """
 
@@ -96,15 +147,15 @@
         scheduler: BaseScheduler,
         interval: int | float = 30,
         *,
         max_simultaneous_jobs: int = 100,
         max_fails_per_job: int = 50,
         # Command line launcher options
         save_dataframe: bool = True,
-        dataframe_format: _DATAFRAME_FORMATS = "parquet",
+        dataframe_format: _DATAFRAME_FORMATS = "pickle",
         loky_start_method: LOKY_START_METHODS = "loky",
         log_interval: int | float = 60,
         save_interval: int | float = 300,
         runner_kwargs: dict[str, Any] | None = None,
         goal: GoalTypes = None,
     ) -> None:
         super().__init__()
```

### Comparing `adaptive_scheduler-2.0.1/adaptive_scheduler/_server_support/kill_manager.py` & `adaptive_scheduler-2.1.0/adaptive_scheduler/_server_support/kill_manager.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.1/adaptive_scheduler/_server_support/launcher.py` & `adaptive_scheduler-2.1.0/adaptive_scheduler/_server_support/launcher.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.1/adaptive_scheduler/_server_support/parse_logs.py` & `adaptive_scheduler-2.1.0/adaptive_scheduler/_server_support/parse_logs.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.1/adaptive_scheduler/_server_support/run_manager.py` & `adaptive_scheduler-2.1.0/adaptive_scheduler/_server_support/run_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,15 @@
         db_fname: str | Path | None = None,
         overwrite_db: bool = True,
         job_manager_kwargs: dict[str, Any] | None = None,
         kill_manager_kwargs: dict[str, Any] | None = None,
         loky_start_method: LOKY_START_METHODS = "loky",
         cleanup_first: bool = False,
         save_dataframe: bool = False,
-        dataframe_format: _DATAFRAME_FORMATS = "parquet",
+        dataframe_format: _DATAFRAME_FORMATS = "pickle",
         max_log_lines: int = 500,
         max_fails_per_job: int = 50,
         max_simultaneous_jobs: int = 100,
     ) -> None:
         super().__init__()
 
         # Set from arguments
```

### Comparing `adaptive_scheduler-2.0.1/adaptive_scheduler/_server_support/slurm_run.py` & `adaptive_scheduler-2.1.0/adaptive_scheduler/_server_support/slurm_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     folder: str | Path = "",
     name: str = "adaptive",
     num_threads: int = 1,
     save_interval: int | float = 300,
     log_interval: int | float = 300,
     cleanup_first: bool = True,
     save_dataframe: bool = True,
-    dataframe_format: _DATAFRAME_FORMATS = "parquet",
+    dataframe_format: _DATAFRAME_FORMATS = "pickle",
     max_fails_per_job: int = 50,
     max_simultaneous_jobs: int = 100,
     exclusive: bool = True,
     executor_type: EXECUTOR_TYPES = "process-pool",
     extra_run_manager_kwargs: dict[str, Any] | None = None,
     extra_scheduler_kwargs: dict[str, Any] | None = None,
 ) -> RunManager:
@@ -69,15 +69,15 @@
         The interval at which to save the learners.
     log_interval : int, default: 300
         The interval at which to log the status of the run.
     cleanup_first : bool, default: True
         Whether to clean up the folder before starting the run.
     save_dataframe : bool, default: True
         Whether to save the `pandas.DataFrame`s with the learners data.
-    dataframe_format : str, default: "parquet"
+    dataframe_format : str, default: "pickle"
         The format to save the `pandas.DataFrame`s in. See
         `adaptive_scheduler.utils.save_dataframes` for more information.
     max_fails_per_job : int, default: 50
         The maximum number of times a job can fail before it is cancelled.
     max_simultaneous_jobs : int, default: 500
         The maximum number of simultaneous jobs.
     executor_type : str
```

### Comparing `adaptive_scheduler-2.0.1/adaptive_scheduler/client_support.py` & `adaptive_scheduler-2.1.0/adaptive_scheduler/client_support.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.1/adaptive_scheduler/scheduler.py` & `adaptive_scheduler-2.1.0/adaptive_scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.1/adaptive_scheduler/server_support.py` & `adaptive_scheduler-2.1.0/adaptive_scheduler/server_support.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.1/adaptive_scheduler/utils.py` & `adaptive_scheduler-2.1.0/adaptive_scheduler/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -777,30 +777,30 @@
         total_filesize += filesize
     total_time = time.time() - t_start
     return total_filesize, total_time
 
 
 def fname_to_dataframe(
     fname: str | list[str] | Path | list[Path],
-    format: str = "parquet",  # noqa: A002
+    format: str = "pickle",  # noqa: A002
 ) -> Path:
     """Convert a learner filename (data) to a filename is used to save the dataframe."""
     if format == "excel":
         format = "xlsx"  # noqa: A001
     if isinstance(fname, (tuple, list)):
         fname = fname[0]
     p = Path(fname)
     new_name = f"dataframe.{p.stem}.{format}"
     return p.with_name(new_name)
 
 
 def save_dataframe(
     fname: str | list[str],
     *,
-    format: _DATAFRAME_FORMATS = "parquet",  # noqa: A002
+    format: _DATAFRAME_FORMATS = "pickle",  # noqa: A002
     save_kwargs: dict[str, Any] | None = None,
     expand_dicts: bool = True,
     **to_dataframe_kwargs: Any,
 ) -> Callable[[adaptive.BaseLearner], None]:
     """Save the learner's data to disk as pandas.DataFrame."""
     save_kwargs = save_kwargs or {}
 
@@ -861,15 +861,15 @@
 
 
 def load_dataframes(  # noqa: PLR0912
     fnames: list[str] | list[list[str]] | list[Path] | list[list[Path]],
     *,
     concat: bool = True,
     read_kwargs: dict[str, Any] | None = None,
-    format: _DATAFRAME_FORMATS = "parquet",  # noqa: A002
+    format: _DATAFRAME_FORMATS = "pickle",  # noqa: A002
 ) -> pd.DataFrame | list[pd.DataFrame]:
     """Load a list of dataframes from disk."""
     read_kwargs = read_kwargs or {}
     dfs = []
     for fn in fnames:
         fn_df = fname_to_dataframe(fn, format=format)
         if not os.path.exists(fn_df):  # noqa: PTH110
```

### Comparing `adaptive_scheduler-2.0.1/adaptive_scheduler/widgets.py` & `adaptive_scheduler-2.1.0/adaptive_scheduler/widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,15 @@
         return f"Exception with trying to read {fname}:\n{e}."
 
 
 def log_explorer(run_manager: RunManager) -> ipyw.VBox:  # noqa: C901, PLR0915
     """Log explorer widget."""
     import ipywidgets as ipyw
 
-    def _update_fname_dropdown(  # noqa: PLR0913
+    def _update_fname_dropdown(
         run_manager: RunManager,
         fname_dropdown: ipyw.Dropdown,
         only_running_checkbox: ipyw.Checkbox,
         only_failed_checkbox: ipyw.Checkbox,
         sort_by_dropdown: ipyw.Dropdown,
         contains_text: ipyw.Text,
     ) -> Callable[[Any], None]:
@@ -219,15 +219,15 @@
                     textarea.value = _read_file(fname, run_manager.max_log_lines)
                     t = t_new
             except asyncio.CancelledError:
                 return
             except Exception:  # noqa: S110, BLE001
                 pass
 
-    def _tail(  # noqa: PLR0913
+    def _tail(
         dropdown: ipyw.Dropdown,
         tail_button: ipyw.Button,
         textarea: ipyw.Textarea,
         update_button: ipyw.Button,
         only_running_checkbox: ipyw.Checkbox,
         only_failed_checkbox: ipyw.Checkbox,
         sort_by_dropdown: ipyw.Dropdown,
```

### Comparing `adaptive_scheduler-2.0.1/adaptive_scheduler.egg-info/PKG-INFO` & `adaptive_scheduler-2.1.0/adaptive_scheduler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adaptive-scheduler
-Version: 2.0.1
+Version: 2.1.0
 Summary: Run many `adaptive.Learner`s on many cores (>10k) using `mpi4py.futures`, `ipyparallel`, `dask-mpi`, or `process-pool`.
 Maintainer-email: Bas Nijholt <bas@nijho.lt>
 License: BSD-3
 Project-URL: homepage, https://adaptive-scheduler.readthedocs.io/
 Project-URL: documentation, https://adaptive-scheduler.readthedocs.io/
 Project-URL: repository, https://github.com/basnijholt/adaptive-scheduler
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `adaptive_scheduler-2.0.1/adaptive_scheduler.egg-info/SOURCES.txt` & `adaptive_scheduler-2.1.0/adaptive_scheduler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.1/pyproject.toml` & `adaptive_scheduler-2.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 dependencies = [
     "adaptive >= 0.14.1",
     "cloudpickle",
     "dill",
     "ipyparallel",
     "ipywidgets",
     "itables",
-    "jinja2",
     "loky",
     "numpy",
     "pandas",
     "psutil",
     "pyarrow",
     "pyzmq",
     "rich",
@@ -110,14 +109,17 @@
     "ANN401",  # Dynamically typed expressions (typing.Any) are disallowed in {name}
     "D402",    # First line should not be the function's signature
     "PLW0603", # Using the global statement to update `X` is discouraged
     "D401",    # First line of docstring should be in imperative mood
     "SLF001",  # Private member accessed
     "S603",    # `subprocess` call: check for execution of untrusted input
     "S607",    # Starting a process with a partial executable path
+    "PLR0913", # Too many arguments to function call (N > 5)
+    "TD002",   # Missing author in TODO; try: `# TODO(<author_name>): ...`
+    "TD003",   # Missing issue link on the line following this TODO
 ]
 
 [tool.ruff.per-file-ignores]
 "tests/*" = ["SLF001"]
 "tests/test_examples.py" = ["E501"]
 ".github/*" = ["INP001"]
```

### Comparing `adaptive_scheduler-2.0.1/setup.py` & `adaptive_scheduler-2.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.1/tests/test_base_scheduler.py` & `adaptive_scheduler-2.1.0/tests/test_base_scheduler.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.1/tests/test_client_support.py` & `adaptive_scheduler-2.1.0/tests/test_client_support.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.1/tests/test_database_manager.py` & `adaptive_scheduler-2.1.0/tests/test_database_manager.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.1/tests/test_job_manager.py` & `adaptive_scheduler-2.1.0/tests/test_job_manager.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.1/tests/test_kill_manager.py` & `adaptive_scheduler-2.1.0/tests/test_kill_manager.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.1/tests/test_launcher.py` & `adaptive_scheduler-2.1.0/tests/test_launcher.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.1/tests/test_log_generation.py` & `adaptive_scheduler-2.1.0/tests/test_log_generation.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.1/tests/test_log_parsing.py` & `adaptive_scheduler-2.1.0/tests/test_log_parsing.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.1/tests/test_run_manager.py` & `adaptive_scheduler-2.1.0/tests/test_run_manager.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.1/tests/test_server_support_common.py` & `adaptive_scheduler-2.1.0/tests/test_server_support_common.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.1/tests/test_slurm_run.py` & `adaptive_scheduler-2.1.0/tests/test_slurm_run.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.1/tests/test_slurm_scheduler.py` & `adaptive_scheduler-2.1.0/tests/test_slurm_scheduler.py`

 * *Files identical despite different names*

### Comparing `adaptive_scheduler-2.0.1/tests/test_utils.py` & `adaptive_scheduler-2.1.0/tests/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -425,15 +425,15 @@
     assert old_fname == Path(f"{folder}/x_1__y_2__z_3.pickle")
     assert new_fname == Path(f"{folder}/a_42__x_1__y_2__z_3.pickle")
 
 
 def test_fname_to_dataframe_with_folder() -> None:
     """Test `utils.fname_to_dataframe` with `folder`."""
     fname = "test_folder/test.pickle"
-    df_fname = utils.fname_to_dataframe(fname)
+    df_fname = utils.fname_to_dataframe(fname, "parquet")
     assert df_fname == Path("test_folder/dataframe.test.parquet")
 
 
 def test_load_dataframes_with_folder(tmp_path: Path) -> None:
     """Test `utils.load_dataframes` with `folder`."""
     folder = tmp_path / "test_folder"
     folder.mkdir()
```

### Comparing `adaptive_scheduler-2.0.1/tests/test_widgets.py` & `adaptive_scheduler-2.1.0/tests/test_widgets.py`

 * *Files identical despite different names*

