# Comparing `tmp/bullmq-0.4.1.tar.gz` & `tmp/bullmq-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bullmq-0.4.1.tar", last modified: Mon May 29 08:06:36 2023, max compression
+gzip compressed data, was "bullmq-0.4.2.tar", last modified: Thu Jun  1 17:08:40 2023, max compression
```

## Comparing `bullmq-0.4.1.tar` & `bullmq-0.4.2.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 manuelastudillo   (501) staff       (20)        0 2023-05-29 08:06:36.483868 bullmq-0.4.1/
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1651 2023-05-29 08:06:36.483544 bullmq-0.4.1/PKG-INFO
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      999 2023-05-04 10:32:52.000000 bullmq-0.4.1/README.md
-drwxr-xr-x   0 manuelastudillo   (501) staff       (20)        0 2023-05-29 08:06:36.449809 bullmq-0.4.1/bullmq/
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      269 2023-05-04 10:32:52.000000 bullmq-0.4.1/bullmq/__init__.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1291 2023-05-04 10:32:52.000000 bullmq-0.4.1/bullmq/backoffs.py
-drwxr-xr-x   0 manuelastudillo   (501) staff       (20)        0 2023-05-29 08:06:36.477110 bullmq-0.4.1/bullmq/commands/
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     8245 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/addJob-8.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      810 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/changeDelay-3.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     9375 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/cleanJobsInSet-2.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     5979 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/drain-4.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      501 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/extendLock-2.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      809 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/getCounts-1.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1748 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/getRanges-1.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1313 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/getState-7.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      934 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/getStateV2-7.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      897 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/isFinished-3.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      424 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/isJobInList-1.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      543 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/moveJobFromActiveToWait-4.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)    11863 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/moveStalledJobsToWait-8.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     7013 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/moveToActive-9.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     4123 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/moveToDelayed-8.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)    21423 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/moveToFinished-12.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1315 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/moveToWaitingChildren-4.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     7844 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/obliterate-2.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      522 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/pause-4.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1967 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/promote-6.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      292 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/releaseLock-1.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     7980 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/removeJob-1.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      666 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/removeRepeatable-2.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      846 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/reprocessJob-4.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     3150 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/retryJob-8.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1830 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/retryJobs-6.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      282 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/takeLock-1.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      246 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/updateData-1.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      420 2023-02-13 17:54:41.000000 bullmq-0.4.1/bullmq/commands/updateProgress-2.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      200 2023-04-18 08:29:50.000000 bullmq-0.4.1/bullmq/error_code.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      632 2023-04-18 08:29:50.000000 bullmq-0.4.1/bullmq/event_emitter.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     7343 2023-05-29 08:02:35.000000 bullmq-0.4.1/bullmq/job.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     4847 2023-05-29 08:02:35.000000 bullmq-0.4.1/bullmq/queue.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1356 2023-05-29 08:02:35.000000 bullmq-0.4.1/bullmq/redis_connection.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)    15741 2023-05-29 08:02:35.000000 bullmq-0.4.1/bullmq/scripts.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      699 2023-04-18 08:29:50.000000 bullmq-0.4.1/bullmq/timer.py
-drwxr-xr-x   0 manuelastudillo   (501) staff       (20)        0 2023-05-29 08:06:36.482827 bullmq-0.4.1/bullmq/types/
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      314 2023-05-04 10:32:52.000000 bullmq-0.4.1/bullmq/types/__init__.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      207 2023-05-04 10:32:52.000000 bullmq-0.4.1/bullmq/types/backoff_options.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1920 2023-05-04 10:32:52.000000 bullmq-0.4.1/bullmq/types/job_options.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      395 2023-05-04 10:32:52.000000 bullmq-0.4.1/bullmq/types/keep_jobs.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      189 2023-05-04 10:32:52.000000 bullmq-0.4.1/bullmq/types/queue_options.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      129 2023-05-04 10:32:52.000000 bullmq-0.4.1/bullmq/types/retry_job_options.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1190 2023-05-04 10:32:52.000000 bullmq-0.4.1/bullmq/types/worker_options.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      144 2023-05-29 08:02:35.000000 bullmq-0.4.1/bullmq/utils.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     7490 2023-05-29 08:02:35.000000 bullmq-0.4.1/bullmq/worker.py
-drwxr-xr-x   0 manuelastudillo   (501) staff       (20)        0 2023-05-29 08:06:36.452051 bullmq-0.4.1/bullmq.egg-info/
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1651 2023-05-29 08:06:36.000000 bullmq-0.4.1/bullmq.egg-info/PKG-INFO
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1574 2023-05-29 08:06:36.000000 bullmq-0.4.1/bullmq.egg-info/SOURCES.txt
--rw-r--r--   0 manuelastudillo   (501) staff       (20)        1 2023-05-29 08:06:36.000000 bullmq-0.4.1/bullmq.egg-info/dependency_links.txt
--rw-r--r--   0 manuelastudillo   (501) staff       (20)       14 2023-05-29 08:06:36.000000 bullmq-0.4.1/bullmq.egg-info/requires.txt
--rw-r--r--   0 manuelastudillo   (501) staff       (20)        7 2023-05-29 08:06:36.000000 bullmq-0.4.1/bullmq.egg-info/top_level.txt
--rw-r--r--   0 manuelastudillo   (501) staff       (20)       38 2023-05-29 08:06:36.483971 bullmq-0.4.1/setup.cfg
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1194 2023-05-29 08:03:42.000000 bullmq-0.4.1/setup.py
+drwxr-xr-x   0 manuelastudillo   (501) staff       (20)        0 2023-06-01 17:08:40.790743 bullmq-0.4.2/
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1651 2023-06-01 17:08:40.790384 bullmq-0.4.2/PKG-INFO
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      999 2023-05-04 10:32:52.000000 bullmq-0.4.2/README.md
+drwxr-xr-x   0 manuelastudillo   (501) staff       (20)        0 2023-06-01 17:08:40.746573 bullmq-0.4.2/bullmq/
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      269 2023-05-04 10:32:52.000000 bullmq-0.4.2/bullmq/__init__.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1291 2023-05-04 10:32:52.000000 bullmq-0.4.2/bullmq/backoffs.py
+drwxr-xr-x   0 manuelastudillo   (501) staff       (20)        0 2023-06-01 17:08:40.784465 bullmq-0.4.2/bullmq/commands/
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     8245 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/addJob-8.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      810 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/changeDelay-3.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     9375 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/cleanJobsInSet-2.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     5979 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/drain-4.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      501 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/extendLock-2.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      809 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/getCounts-1.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1748 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/getRanges-1.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1313 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/getState-7.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      934 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/getStateV2-7.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      897 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/isFinished-3.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      424 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/isJobInList-1.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      543 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/moveJobFromActiveToWait-4.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)    11863 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/moveStalledJobsToWait-8.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     7013 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/moveToActive-9.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     4123 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/moveToDelayed-8.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)    21423 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/moveToFinished-12.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1315 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/moveToWaitingChildren-4.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     7844 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/obliterate-2.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      522 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/pause-4.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1967 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/promote-6.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      292 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/releaseLock-1.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     7980 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/removeJob-1.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      666 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/removeRepeatable-2.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      846 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/reprocessJob-4.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     3150 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/retryJob-8.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1830 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/retryJobs-6.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      282 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/takeLock-1.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      246 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/updateData-1.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      420 2023-02-13 17:54:41.000000 bullmq-0.4.2/bullmq/commands/updateProgress-2.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      200 2023-04-18 08:29:50.000000 bullmq-0.4.2/bullmq/error_code.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      632 2023-04-18 08:29:50.000000 bullmq-0.4.2/bullmq/event_emitter.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     7343 2023-05-29 08:02:35.000000 bullmq-0.4.2/bullmq/job.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     4847 2023-05-29 08:02:35.000000 bullmq-0.4.2/bullmq/queue.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1356 2023-05-29 08:02:35.000000 bullmq-0.4.2/bullmq/redis_connection.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)    15741 2023-05-29 08:02:35.000000 bullmq-0.4.2/bullmq/scripts.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      699 2023-04-18 08:29:50.000000 bullmq-0.4.2/bullmq/timer.py
+drwxr-xr-x   0 manuelastudillo   (501) staff       (20)        0 2023-06-01 17:08:40.789564 bullmq-0.4.2/bullmq/types/
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      314 2023-05-04 10:32:52.000000 bullmq-0.4.2/bullmq/types/__init__.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      207 2023-05-04 10:32:52.000000 bullmq-0.4.2/bullmq/types/backoff_options.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1920 2023-05-04 10:32:52.000000 bullmq-0.4.2/bullmq/types/job_options.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      395 2023-05-04 10:32:52.000000 bullmq-0.4.2/bullmq/types/keep_jobs.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      189 2023-05-04 10:32:52.000000 bullmq-0.4.2/bullmq/types/queue_options.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      129 2023-05-04 10:32:52.000000 bullmq-0.4.2/bullmq/types/retry_job_options.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1190 2023-05-04 10:32:52.000000 bullmq-0.4.2/bullmq/types/worker_options.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      144 2023-05-29 08:02:35.000000 bullmq-0.4.2/bullmq/utils.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     7490 2023-05-29 08:02:35.000000 bullmq-0.4.2/bullmq/worker.py
+drwxr-xr-x   0 manuelastudillo   (501) staff       (20)        0 2023-06-01 17:08:40.748326 bullmq-0.4.2/bullmq.egg-info/
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1651 2023-06-01 17:08:40.000000 bullmq-0.4.2/bullmq.egg-info/PKG-INFO
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1574 2023-06-01 17:08:40.000000 bullmq-0.4.2/bullmq.egg-info/SOURCES.txt
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)        1 2023-06-01 17:08:40.000000 bullmq-0.4.2/bullmq.egg-info/dependency_links.txt
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)       21 2023-06-01 17:08:40.000000 bullmq-0.4.2/bullmq.egg-info/requires.txt
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)        7 2023-06-01 17:08:40.000000 bullmq-0.4.2/bullmq.egg-info/top_level.txt
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)       38 2023-06-01 17:08:40.790854 bullmq-0.4.2/setup.cfg
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1177 2023-06-01 17:06:57.000000 bullmq-0.4.2/setup.py
```

### Comparing `bullmq-0.4.1/PKG-INFO` & `bullmq-0.4.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bullmq
-Version: 0.4.1
+Version: 0.4.2
 Summary: BullMQ for Python
 Home-page: https://bullmq.io
 Author: Taskforce.sh Inc.
 Author-email: manast@taskforce.sh
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bullmq-0.4.1/README.md` & `bullmq-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.1/bullmq/backoffs.py` & `bullmq-0.4.2/bullmq/backoffs.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.1/bullmq/commands/addJob-8.lua` & `bullmq-0.4.2/bullmq/commands/addJob-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.1/bullmq/commands/changeDelay-3.lua` & `bullmq-0.4.2/bullmq/commands/changeDelay-3.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.1/bullmq/commands/cleanJobsInSet-2.lua` & `bullmq-0.4.2/bullmq/commands/cleanJobsInSet-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.1/bullmq/commands/drain-4.lua` & `bullmq-0.4.2/bullmq/commands/drain-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.1/bullmq/commands/getCounts-1.lua` & `bullmq-0.4.2/bullmq/commands/getCounts-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.1/bullmq/commands/getRanges-1.lua` & `bullmq-0.4.2/bullmq/commands/getRanges-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.1/bullmq/commands/getState-7.lua` & `bullmq-0.4.2/bullmq/commands/getState-7.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.1/bullmq/commands/getStateV2-7.lua` & `bullmq-0.4.2/bullmq/commands/getStateV2-7.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.1/bullmq/commands/isFinished-3.lua` & `bullmq-0.4.2/bullmq/commands/isFinished-3.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.1/bullmq/commands/moveJobFromActiveToWait-4.lua` & `bullmq-0.4.2/bullmq/commands/moveJobFromActiveToWait-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.1/bullmq/commands/moveStalledJobsToWait-8.lua` & `bullmq-0.4.2/bullmq/commands/moveStalledJobsToWait-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.1/bullmq/commands/moveToActive-9.lua` & `bullmq-0.4.2/bullmq/commands/moveToActive-9.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.1/bullmq/commands/moveToDelayed-8.lua` & `bullmq-0.4.2/bullmq/commands/moveToDelayed-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.1/bullmq/commands/moveToFinished-12.lua` & `bullmq-0.4.2/bullmq/commands/moveToFinished-12.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.1/bullmq/commands/moveToWaitingChildren-4.lua` & `bullmq-0.4.2/bullmq/commands/moveToWaitingChildren-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.1/bullmq/commands/obliterate-2.lua` & `bullmq-0.4.2/bullmq/commands/obliterate-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.1/bullmq/commands/pause-4.lua` & `bullmq-0.4.2/bullmq/commands/pause-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.1/bullmq/commands/promote-6.lua` & `bullmq-0.4.2/bullmq/commands/promote-6.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.1/bullmq/commands/removeJob-1.lua` & `bullmq-0.4.2/bullmq/commands/removeJob-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.1/bullmq/commands/removeRepeatable-2.lua` & `bullmq-0.4.2/bullmq/commands/removeRepeatable-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.1/bullmq/commands/reprocessJob-4.lua` & `bullmq-0.4.2/bullmq/commands/reprocessJob-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.1/bullmq/commands/retryJob-8.lua` & `bullmq-0.4.2/bullmq/commands/retryJob-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.1/bullmq/commands/retryJobs-6.lua` & `bullmq-0.4.2/bullmq/commands/retryJobs-6.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.1/bullmq/event_emitter.py` & `bullmq-0.4.2/bullmq/event_emitter.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.1/bullmq/job.py` & `bullmq-0.4.2/bullmq/job.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.1/bullmq/queue.py` & `bullmq-0.4.2/bullmq/queue.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.1/bullmq/redis_connection.py` & `bullmq-0.4.2/bullmq/redis_connection.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.1/bullmq/scripts.py` & `bullmq-0.4.2/bullmq/scripts.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.1/bullmq/timer.py` & `bullmq-0.4.2/bullmq/timer.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.1/bullmq/types/job_options.py` & `bullmq-0.4.2/bullmq/types/job_options.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.1/bullmq/types/worker_options.py` & `bullmq-0.4.2/bullmq/types/worker_options.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.1/bullmq/worker.py` & `bullmq-0.4.2/bullmq/worker.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.1/bullmq.egg-info/PKG-INFO` & `bullmq-0.4.2/bullmq.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bullmq
-Version: 0.4.1
+Version: 0.4.2
 Summary: BullMQ for Python
 Home-page: https://bullmq.io
 Author: Taskforce.sh Inc.
 Author-email: manast@taskforce.sh
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bullmq-0.4.1/bullmq.egg-info/SOURCES.txt` & `bullmq-0.4.2/bullmq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bullmq-0.4.1/setup.py` & `bullmq-0.4.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,27 +6,29 @@
 
 # Get the long description from the README file
 with open(path.join(".", 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='bullmq',
-    version='0.4.1',    
+    version='0.4.2',    
     description='BullMQ for Python',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://bullmq.io',
     author='Taskforce.sh Inc.',
     author_email='manast@taskforce.sh',
     license='MIT',
     packages=['bullmq'],
     package_data={'bullmq': ['commands/*.lua', 'types/*']},
-    install_requires=['redis',
-                      'msgpack',            
-                      ],
+    install_requires=[
+        'redis',
+        'msgpack',
+        'semver',
+    ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',  
         'Operating System :: POSIX :: Linux',        
         'Programming Language :: Python :: 2',
         'Programming Language :: Python :: 2.7',
```

