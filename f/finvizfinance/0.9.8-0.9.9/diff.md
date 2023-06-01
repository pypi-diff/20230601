# Comparing `tmp/finvizfinance-0.9.8.tar.gz` & `tmp/finvizfinance-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/finvizfinance-0.9.8.tar", last modified: Sat May  8 07:52:33 2021, max compression
+gzip compressed data, was "dist/finvizfinance-0.9.9.tar", last modified: Sat Jul  3 22:53:18 2021, max compression
```

## Comparing `finvizfinance-0.9.8.tar` & `finvizfinance-0.9.9.tar`

### file list

```diff
@@ -1,37 +1,76 @@
-drwxr-xr-x   0 tianningli   (501) staff       (20)        0 2021-05-08 07:52:33.000000 finvizfinance-0.9.8/
--rw-r--r--   0 tianningli   (501) staff       (20)     4768 2021-05-08 07:52:33.000000 finvizfinance-0.9.8/PKG-INFO
--rw-r--r--   0 tianningli   (501) staff       (20)     3936 2021-02-05 23:11:24.000000 finvizfinance-0.9.8/README.md
-drwxr-xr-x   0 tianningli   (501) staff       (20)        0 2021-05-08 07:52:33.000000 finvizfinance-0.9.8/finvizfinance/
--rw-r--r--   0 tianningli   (501) staff       (20)        0 2020-07-24 00:12:59.000000 finvizfinance-0.9.8/finvizfinance/__init__.py
--rw-r--r--   0 tianningli   (501) staff       (20)     1145 2021-02-05 22:59:03.000000 finvizfinance-0.9.8/finvizfinance/crypto.py
--rw-r--r--   0 tianningli   (501) staff       (20)     4574 2021-04-27 21:41:01.000000 finvizfinance-0.9.8/finvizfinance/earnings.py
--rw-r--r--   0 tianningli   (501) staff       (20)     1533 2021-04-27 21:41:29.000000 finvizfinance-0.9.8/finvizfinance/forex.py
--rw-r--r--   0 tianningli   (501) staff       (20)     1348 2021-04-27 21:42:14.000000 finvizfinance-0.9.8/finvizfinance/future.py
-drwxr-xr-x   0 tianningli   (501) staff       (20)        0 2021-05-08 07:52:33.000000 finvizfinance-0.9.8/finvizfinance/group/
--rw-r--r--   0 tianningli   (501) staff       (20)        0 2020-07-24 00:12:59.000000 finvizfinance-0.9.8/finvizfinance/group/__init__.py
--rw-r--r--   0 tianningli   (501) staff       (20)     2948 2021-02-05 23:01:50.000000 finvizfinance-0.9.8/finvizfinance/group/overview.py
--rw-r--r--   0 tianningli   (501) staff       (20)      561 2021-04-16 22:08:27.000000 finvizfinance-0.9.8/finvizfinance/group/performance.py
--rw-r--r--   0 tianningli   (501) staff       (20)     1218 2021-02-05 23:02:01.000000 finvizfinance-0.9.8/finvizfinance/group/spectrum.py
--rw-r--r--   0 tianningli   (501) staff       (20)      551 2021-02-05 23:02:01.000000 finvizfinance-0.9.8/finvizfinance/group/valuation.py
--rw-r--r--   0 tianningli   (501) staff       (20)     2800 2021-04-22 01:46:50.000000 finvizfinance-0.9.8/finvizfinance/insider.py
--rw-r--r--   0 tianningli   (501) staff       (20)     1725 2021-02-05 23:00:42.000000 finvizfinance-0.9.8/finvizfinance/news.py
--rw-r--r--   0 tianningli   (501) staff       (20)    12252 2021-05-08 07:48:37.000000 finvizfinance-0.9.8/finvizfinance/quote.py
-drwxr-xr-x   0 tianningli   (501) staff       (20)        0 2021-05-08 07:52:33.000000 finvizfinance-0.9.8/finvizfinance/screener/
--rw-r--r--   0 tianningli   (501) staff       (20)        0 2020-07-24 00:12:59.000000 finvizfinance-0.9.8/finvizfinance/screener/__init__.py
--rw-r--r--   0 tianningli   (501) staff       (20)     5701 2021-04-27 21:38:53.000000 finvizfinance-0.9.8/finvizfinance/screener/custom.py
--rw-r--r--   0 tianningli   (501) staff       (20)      597 2021-02-24 01:54:00.000000 finvizfinance-0.9.8/finvizfinance/screener/financial.py
--rw-r--r--   0 tianningli   (501) staff       (20)     9279 2021-04-27 21:35:28.000000 finvizfinance-0.9.8/finvizfinance/screener/overview.py
--rw-r--r--   0 tianningli   (501) staff       (20)      597 2021-02-24 01:54:18.000000 finvizfinance-0.9.8/finvizfinance/screener/ownership.py
--rw-r--r--   0 tianningli   (501) staff       (20)      607 2021-02-24 01:54:24.000000 finvizfinance-0.9.8/finvizfinance/screener/performance.py
--rw-r--r--   0 tianningli   (501) staff       (20)      597 2021-02-24 01:54:30.000000 finvizfinance-0.9.8/finvizfinance/screener/technical.py
--rw-r--r--   0 tianningli   (501) staff       (20)     1960 2021-02-05 23:01:39.000000 finvizfinance-0.9.8/finvizfinance/screener/ticker.py
--rw-r--r--   0 tianningli   (501) staff       (20)      601 2021-02-24 01:54:38.000000 finvizfinance-0.9.8/finvizfinance/screener/valuation.py
--rw-r--r--   0 tianningli   (501) staff       (20)    52919 2021-04-19 05:49:59.000000 finvizfinance-0.9.8/finvizfinance/util.py
-drwxr-xr-x   0 tianningli   (501) staff       (20)        0 2021-05-08 07:52:33.000000 finvizfinance-0.9.8/finvizfinance.egg-info/
--rw-r--r--   0 tianningli   (501) staff       (20)     4768 2021-05-08 07:52:33.000000 finvizfinance-0.9.8/finvizfinance.egg-info/PKG-INFO
--rw-r--r--   0 tianningli   (501) staff       (20)      899 2021-05-08 07:52:33.000000 finvizfinance-0.9.8/finvizfinance.egg-info/SOURCES.txt
--rw-r--r--   0 tianningli   (501) staff       (20)        1 2021-05-08 07:52:33.000000 finvizfinance-0.9.8/finvizfinance.egg-info/dependency_links.txt
--rw-r--r--   0 tianningli   (501) staff       (20)       34 2021-05-08 07:52:33.000000 finvizfinance-0.9.8/finvizfinance.egg-info/requires.txt
--rw-r--r--   0 tianningli   (501) staff       (20)       14 2021-05-08 07:52:33.000000 finvizfinance-0.9.8/finvizfinance.egg-info/top_level.txt
--rw-r--r--   0 tianningli   (501) staff       (20)       38 2021-05-08 07:52:33.000000 finvizfinance-0.9.8/setup.cfg
--rw-r--r--   0 tianningli   (501) staff       (20)     1183 2021-05-08 07:51:19.000000 finvizfinance-0.9.8/setup.py
+drwxr-xr-x   0 tianningli   (501) staff       (20)        0 2021-07-03 22:53:18.000000 finvizfinance-0.9.9/
+drwxr-xr-x   0 tianningli   (501) staff       (20)        0 2021-07-03 22:53:18.000000 finvizfinance-0.9.9/.github/
+-rw-r--r--   0 tianningli   (501) staff       (20)       71 2021-01-04 23:57:57.000000 finvizfinance-0.9.9/.github/FUNDING.yml
+-rw-r--r--   0 tianningli   (501) staff       (20)      266 2021-02-05 22:56:54.000000 finvizfinance-0.9.9/.travis.yml
+-rw-r--r--   0 tianningli   (501) staff       (20)     5223 2021-04-19 05:56:04.000000 finvizfinance-0.9.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 tianningli   (501) staff       (20)     2279 2021-04-14 21:40:38.000000 finvizfinance-0.9.9/CONTRIBUTING.md
+-rw-r--r--   0 tianningli   (501) staff       (20)   270116 2021-02-24 04:38:44.000000 finvizfinance-0.9.9/Industry.jpg
+-rw-r--r--   0 tianningli   (501) staff       (20)     1068 2020-07-23 23:58:47.000000 finvizfinance-0.9.9/LICENSE
+-rw-r--r--   0 tianningli   (501) staff       (20)     4768 2021-07-03 22:53:18.000000 finvizfinance-0.9.9/PKG-INFO
+-rw-r--r--   0 tianningli   (501) staff       (20)     3936 2021-02-05 23:11:24.000000 finvizfinance-0.9.9/README.md
+drwxr-xr-x   0 tianningli   (501) staff       (20)        0 2021-07-03 22:53:18.000000 finvizfinance-0.9.9/asset/
+-rw-r--r--   0 tianningli   (501) staff       (20)    85012 2020-07-26 02:29:02.000000 finvizfinance-0.9.9/asset/insider.png
+-rw-r--r--   0 tianningli   (501) staff       (20)    41390 2020-07-23 23:58:47.000000 finvizfinance-0.9.9/asset/insider_trader.png
+-rw-r--r--   0 tianningli   (501) staff       (20)    34485 2020-07-25 21:56:16.000000 finvizfinance-0.9.9/asset/news_blogs.png
+-rw-r--r--   0 tianningli   (501) staff       (20)    33182 2020-07-25 21:50:19.000000 finvizfinance-0.9.9/asset/news_news.png
+-rw-r--r--   0 tianningli   (501) staff       (20)    19105 2020-07-23 23:58:47.000000 finvizfinance-0.9.9/asset/outer_rating.png
+-rw-r--r--   0 tianningli   (501) staff       (20)    34451 2020-07-27 02:20:44.000000 finvizfinance-0.9.9/asset/screen_overview.png
+-rw-r--r--   0 tianningli   (501) staff       (20)    22286 2020-07-23 23:58:47.000000 finvizfinance-0.9.9/asset/stock_news.png
+-rw-r--r--   0 tianningli   (501) staff       (20)    29445 2021-01-04 23:57:57.000000 finvizfinance-0.9.9/asset/tsla.jpg
+drwxr-xr-x   0 tianningli   (501) staff       (20)        0 2021-07-03 22:53:18.000000 finvizfinance-0.9.9/docs/
+-rw-r--r--   0 tianningli   (501) staff       (20)      634 2020-07-30 03:27:01.000000 finvizfinance-0.9.9/docs/Makefile
+-rw-r--r--   0 tianningli   (501) staff       (20)     2221 2021-07-03 22:52:01.000000 finvizfinance-0.9.9/docs/conf.py
+-rw-r--r--   0 tianningli   (501) staff       (20)      126 2020-08-13 11:15:39.000000 finvizfinance-0.9.9/docs/crypto.rst
+-rw-r--r--   0 tianningli   (501) staff       (20)      128 2020-08-21 07:17:05.000000 finvizfinance-0.9.9/docs/earnings.rst
+-rw-r--r--   0 tianningli   (501) staff       (20)      125 2020-08-13 11:37:27.000000 finvizfinance-0.9.9/docs/forex.rst
+-rw-r--r--   0 tianningli   (501) staff       (20)      117 2021-01-04 23:57:57.000000 finvizfinance-0.9.9/docs/future.rst
+-rw-r--r--   0 tianningli   (501) staff       (20)      401 2020-08-15 03:24:56.000000 finvizfinance-0.9.9/docs/group.rst
+-rw-r--r--   0 tianningli   (501) staff       (20)     2176 2021-07-03 22:51:54.000000 finvizfinance-0.9.9/docs/index.rst
+-rw-r--r--   0 tianningli   (501) staff       (20)      116 2020-07-30 00:19:58.000000 finvizfinance-0.9.9/docs/insider.rst
+-rw-r--r--   0 tianningli   (501) staff       (20)      795 2020-07-30 03:27:01.000000 finvizfinance-0.9.9/docs/make.bat
+-rw-r--r--   0 tianningli   (501) staff       (20)      107 2020-07-30 00:19:58.000000 finvizfinance-0.9.9/docs/news.rst
+-rw-r--r--   0 tianningli   (501) staff       (20)      125 2021-04-04 02:59:06.000000 finvizfinance-0.9.9/docs/quote.rst
+-rw-r--r--   0 tianningli   (501) staff       (20)      670 2021-02-24 02:03:15.000000 finvizfinance-0.9.9/docs/screener.rst
+drwxr-xr-x   0 tianningli   (501) staff       (20)        0 2021-07-03 22:53:18.000000 finvizfinance-0.9.9/example/
+-rw-r--r--   0 tianningli   (501) staff       (20)     7657 2021-01-04 23:57:57.000000 finvizfinance-0.9.9/example/audusd_d1_s.jpg
+-rw-r--r--   0 tianningli   (501) staff       (20)     8844 2021-01-04 23:57:57.000000 finvizfinance-0.9.9/example/btcusd_m5_s.jpg
+-rw-r--r--   0 tianningli   (501) staff       (20)   115031 2021-01-04 23:57:57.000000 finvizfinance-0.9.9/example/example.ipynb
+-rw-r--r--   0 tianningli   (501) staff       (20)    30451 2021-01-04 23:57:57.000000 finvizfinance-0.9.9/example/tsla.jpg
+drwxr-xr-x   0 tianningli   (501) staff       (20)        0 2021-07-03 22:53:18.000000 finvizfinance-0.9.9/finvizfinance/
+-rw-r--r--   0 tianningli   (501) staff       (20)      191 2021-07-03 22:52:08.000000 finvizfinance-0.9.9/finvizfinance/__init__.py
+-rw-r--r--   0 tianningli   (501) staff       (20)     1686 2021-07-03 22:44:16.000000 finvizfinance-0.9.9/finvizfinance/calendar.py
+-rw-r--r--   0 tianningli   (501) staff       (20)     1145 2021-02-05 22:59:03.000000 finvizfinance-0.9.9/finvizfinance/crypto.py
+-rw-r--r--   0 tianningli   (501) staff       (20)     4574 2021-04-27 21:41:01.000000 finvizfinance-0.9.9/finvizfinance/earnings.py
+-rw-r--r--   0 tianningli   (501) staff       (20)     1533 2021-04-27 21:41:29.000000 finvizfinance-0.9.9/finvizfinance/forex.py
+-rw-r--r--   0 tianningli   (501) staff       (20)     1348 2021-07-03 22:44:49.000000 finvizfinance-0.9.9/finvizfinance/future.py
+drwxr-xr-x   0 tianningli   (501) staff       (20)        0 2021-07-03 22:53:18.000000 finvizfinance-0.9.9/finvizfinance/group/
+-rw-r--r--   0 tianningli   (501) staff       (20)        0 2020-07-24 00:12:59.000000 finvizfinance-0.9.9/finvizfinance/group/__init__.py
+-rw-r--r--   0 tianningli   (501) staff       (20)     2948 2021-02-05 23:01:50.000000 finvizfinance-0.9.9/finvizfinance/group/overview.py
+-rw-r--r--   0 tianningli   (501) staff       (20)      561 2021-04-16 22:08:27.000000 finvizfinance-0.9.9/finvizfinance/group/performance.py
+-rw-r--r--   0 tianningli   (501) staff       (20)     1218 2021-02-05 23:02:01.000000 finvizfinance-0.9.9/finvizfinance/group/spectrum.py
+-rw-r--r--   0 tianningli   (501) staff       (20)      551 2021-02-05 23:02:01.000000 finvizfinance-0.9.9/finvizfinance/group/valuation.py
+-rw-r--r--   0 tianningli   (501) staff       (20)     2800 2021-07-03 22:45:00.000000 finvizfinance-0.9.9/finvizfinance/insider.py
+-rw-r--r--   0 tianningli   (501) staff       (20)     1725 2021-07-03 22:45:09.000000 finvizfinance-0.9.9/finvizfinance/news.py
+-rw-r--r--   0 tianningli   (501) staff       (20)    12253 2021-07-03 22:50:15.000000 finvizfinance-0.9.9/finvizfinance/quote.py
+drwxr-xr-x   0 tianningli   (501) staff       (20)        0 2021-07-03 22:53:18.000000 finvizfinance-0.9.9/finvizfinance/screener/
+-rw-r--r--   0 tianningli   (501) staff       (20)        0 2020-07-24 00:12:59.000000 finvizfinance-0.9.9/finvizfinance/screener/__init__.py
+-rw-r--r--   0 tianningli   (501) staff       (20)     5701 2021-07-03 22:46:28.000000 finvizfinance-0.9.9/finvizfinance/screener/custom.py
+-rw-r--r--   0 tianningli   (501) staff       (20)      597 2021-02-24 01:54:00.000000 finvizfinance-0.9.9/finvizfinance/screener/financial.py
+-rw-r--r--   0 tianningli   (501) staff       (20)     9279 2021-07-03 22:46:49.000000 finvizfinance-0.9.9/finvizfinance/screener/overview.py
+-rw-r--r--   0 tianningli   (501) staff       (20)      597 2021-02-24 01:54:18.000000 finvizfinance-0.9.9/finvizfinance/screener/ownership.py
+-rw-r--r--   0 tianningli   (501) staff       (20)      607 2021-02-24 01:54:24.000000 finvizfinance-0.9.9/finvizfinance/screener/performance.py
+-rw-r--r--   0 tianningli   (501) staff       (20)      597 2021-02-24 01:54:30.000000 finvizfinance-0.9.9/finvizfinance/screener/technical.py
+-rw-r--r--   0 tianningli   (501) staff       (20)     1960 2021-02-05 23:01:39.000000 finvizfinance-0.9.9/finvizfinance/screener/ticker.py
+-rw-r--r--   0 tianningli   (501) staff       (20)      601 2021-02-24 01:54:38.000000 finvizfinance-0.9.9/finvizfinance/screener/valuation.py
+-rw-r--r--   0 tianningli   (501) staff       (20)    52919 2021-07-03 22:46:00.000000 finvizfinance-0.9.9/finvizfinance/util.py
+drwxr-xr-x   0 tianningli   (501) staff       (20)        0 2021-07-03 22:53:18.000000 finvizfinance-0.9.9/finvizfinance.egg-info/
+-rw-r--r--   0 tianningli   (501) staff       (20)     4768 2021-07-03 22:53:18.000000 finvizfinance-0.9.9/finvizfinance.egg-info/PKG-INFO
+-rw-r--r--   0 tianningli   (501) staff       (20)     1508 2021-07-03 22:53:18.000000 finvizfinance-0.9.9/finvizfinance.egg-info/SOURCES.txt
+-rw-r--r--   0 tianningli   (501) staff       (20)        1 2021-07-03 22:53:18.000000 finvizfinance-0.9.9/finvizfinance.egg-info/dependency_links.txt
+-rw-r--r--   0 tianningli   (501) staff       (20)       34 2021-07-03 22:53:18.000000 finvizfinance-0.9.9/finvizfinance.egg-info/requires.txt
+-rw-r--r--   0 tianningli   (501) staff       (20)       14 2021-07-03 22:53:18.000000 finvizfinance-0.9.9/finvizfinance.egg-info/top_level.txt
+-rw-r--r--   0 tianningli   (501) staff       (20)     2040 2021-05-08 07:56:15.000000 finvizfinance-0.9.9/release.md
+-rw-r--r--   0 tianningli   (501) staff       (20)       34 2020-07-29 05:08:47.000000 finvizfinance-0.9.9/requirements.txt
+-rw-r--r--   0 tianningli   (501) staff       (20)     2572 2021-07-03 22:50:42.000000 finvizfinance-0.9.9/runtest.py
+-rw-r--r--   0 tianningli   (501) staff       (20)       38 2021-07-03 22:53:18.000000 finvizfinance-0.9.9/setup.cfg
+-rw-r--r--   0 tianningli   (501) staff       (20)     1183 2021-07-03 22:52:15.000000 finvizfinance-0.9.9/setup.py
```

### Comparing `finvizfinance-0.9.8/PKG-INFO` & `finvizfinance-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finvizfinance
-Version: 0.9.8
+Version: 0.9.9
 Summary: Finviz Finance. Information downloader.
 Home-page: https://github.com/lit26/finvizfinance
 Author: Tianning Li
 Author-email: ltianningli@gmail.com
 License: The MIT License (MIT)
 Description: # finvizfinance
```

### Comparing `finvizfinance-0.9.8/README.md` & `finvizfinance-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `finvizfinance-0.9.8/finvizfinance/crypto.py` & `finvizfinance-0.9.9/finvizfinance/crypto.py`

 * *Files identical despite different names*

### Comparing `finvizfinance-0.9.8/finvizfinance/earnings.py` & `finvizfinance-0.9.9/finvizfinance/earnings.py`

 * *Files identical despite different names*

### Comparing `finvizfinance-0.9.8/finvizfinance/forex.py` & `finvizfinance-0.9.9/finvizfinance/forex.py`

 * *Files identical despite different names*

### Comparing `finvizfinance-0.9.8/finvizfinance/future.py` & `finvizfinance-0.9.9/finvizfinance/future.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from finvizfinance.util import webScrap
-import pandas as pd
 import json
+import pandas as pd
+from finvizfinance.util import webScrap
 
 """
 .. module:: future
    :synopsis: future.
 
 .. moduleauthor:: Tianning Li <ltianningli@gmail.com>
 """
```

### Comparing `finvizfinance-0.9.8/finvizfinance/group/overview.py` & `finvizfinance-0.9.9/finvizfinance/group/overview.py`

 * *Files identical despite different names*

### Comparing `finvizfinance-0.9.8/finvizfinance/group/performance.py` & `finvizfinance-0.9.9/finvizfinance/group/performance.py`

 * *Files identical despite different names*

### Comparing `finvizfinance-0.9.8/finvizfinance/group/spectrum.py` & `finvizfinance-0.9.9/finvizfinance/group/spectrum.py`

 * *Files identical despite different names*

### Comparing `finvizfinance-0.9.8/finvizfinance/group/valuation.py` & `finvizfinance-0.9.9/finvizfinance/group/valuation.py`

 * *Files identical despite different names*

### Comparing `finvizfinance-0.9.8/finvizfinance/insider.py` & `finvizfinance-0.9.9/finvizfinance/insider.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from finvizfinance.util import webScrap, numberCovert
 import pandas as pd
+from finvizfinance.util import webScrap, numberCovert
 """
 .. module:: insider
    :synopsis: insider table.
 
 .. moduleauthor:: Tianning Li <ltianningli@gmail.com>
 """
```

### Comparing `finvizfinance-0.9.8/finvizfinance/news.py` & `finvizfinance-0.9.9/finvizfinance/news.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from finvizfinance.util import webScrap
 import pandas as pd
+from finvizfinance.util import webScrap
 """
 .. module:: news
    :synopsis: news table.
 
 .. moduleauthor:: Tianning Li <ltianningli@gmail.com>
 """
```

### Comparing `finvizfinance-0.9.8/finvizfinance/quote.py` & `finvizfinance-0.9.9/finvizfinance/quote.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from datetime import datetime
-import requests
 import json
 import pandas as pd
+import requests
 from finvizfinance.util import webScrap, imageScrap, numberCovert, headers
 """
 .. module:: finvizfinance
    :synopsis: individual ticker.
 
 .. moduleauthor:: Tianning Li <ltianningli@gmail.com>
 """
 QUOTE_URL = 'https://finviz.com/quote.ashx?t={ticker}'
 NUM_COL = ['P/E', 'EPS (ttm)', 'Insider Own', 'Shs Outstand', 'Market Cap', 'Forward P/E',
            'EPS nest Y', 'Insider ']
 
+
 class Quote:
     """quote
     Getting current price of the ticker
 
     """
     def getCurrent(self, ticker):
         """Getting current price of the ticker.
```

### Comparing `finvizfinance-0.9.8/finvizfinance/screener/custom.py` & `finvizfinance-0.9.9/finvizfinance/screener/custom.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+import pandas as pd
 from finvizfinance.screener.overview import Overview
 from finvizfinance.util import webScrap, progressBar, NUMBER_COL
-import pandas as pd
 """
 .. module:: screen.custom
    :synopsis: screen custom table.
 
 .. moduleauthor:: Tianning Li <ltianningli@gmail.com>
 """
```

### Comparing `finvizfinance-0.9.8/finvizfinance/screener/financial.py` & `finvizfinance-0.9.9/finvizfinance/screener/financial.py`

 * *Files identical despite different names*

### Comparing `finvizfinance-0.9.8/finvizfinance/screener/overview.py` & `finvizfinance-0.9.9/finvizfinance/screener/overview.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from finvizfinance.util import webScrap, numberCovert, progressBar, NUMBER_COL, util_dict
-from finvizfinance.quote import finvizfinance
 import pandas as pd
+from finvizfinance.quote import finvizfinance
+from finvizfinance.util import webScrap, numberCovert, progressBar, NUMBER_COL, util_dict
 """
 .. module:: screen.overview
    :synopsis: screen overview table.
 
 .. moduleauthor:: Tianning Li <ltianningli@gmail.com>
 
 """
```

### Comparing `finvizfinance-0.9.8/finvizfinance/screener/ownership.py` & `finvizfinance-0.9.9/finvizfinance/screener/ownership.py`

 * *Files identical despite different names*

### Comparing `finvizfinance-0.9.8/finvizfinance/screener/performance.py` & `finvizfinance-0.9.9/finvizfinance/screener/performance.py`

 * *Files identical despite different names*

### Comparing `finvizfinance-0.9.8/finvizfinance/screener/technical.py` & `finvizfinance-0.9.9/finvizfinance/screener/technical.py`

 * *Files identical despite different names*

### Comparing `finvizfinance-0.9.8/finvizfinance/screener/ticker.py` & `finvizfinance-0.9.9/finvizfinance/screener/ticker.py`

 * *Files identical despite different names*

### Comparing `finvizfinance-0.9.8/finvizfinance/screener/valuation.py` & `finvizfinance-0.9.9/finvizfinance/screener/valuation.py`

 * *Files identical despite different names*

### Comparing `finvizfinance-0.9.8/finvizfinance/util.py` & `finvizfinance-0.9.9/finvizfinance/util.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+import sys
 import requests
 import pandas as pd
 from bs4 import BeautifulSoup
-import sys
 
 """
 .. module:: util
    :synopsis: General function for the package.
 
 .. moduleauthor:: Tianning Li <ltianningli@gmail.com>
 """
```

### Comparing `finvizfinance-0.9.8/finvizfinance.egg-info/PKG-INFO` & `finvizfinance-0.9.9/finvizfinance.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finvizfinance
-Version: 0.9.8
+Version: 0.9.9
 Summary: Finviz Finance. Information downloader.
 Home-page: https://github.com/lit26/finvizfinance
 Author: Tianning Li
 Author-email: ltianningli@gmail.com
 License: The MIT License (MIT)
 Description: # finvizfinance
```

### Comparing `finvizfinance-0.9.8/finvizfinance.egg-info/SOURCES.txt` & `finvizfinance-0.9.9/finvizfinance.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,45 @@
+.travis.yml
+CODE_OF_CONDUCT.md
+CONTRIBUTING.md
+Industry.jpg
+LICENSE
 README.md
+release.md
+requirements.txt
+runtest.py
 setup.py
+.github/FUNDING.yml
+asset/insider.png
+asset/insider_trader.png
+asset/news_blogs.png
+asset/news_news.png
+asset/outer_rating.png
+asset/screen_overview.png
+asset/stock_news.png
+asset/tsla.jpg
+docs/Makefile
+docs/conf.py
+docs/crypto.rst
+docs/earnings.rst
+docs/forex.rst
+docs/future.rst
+docs/group.rst
+docs/index.rst
+docs/insider.rst
+docs/make.bat
+docs/news.rst
+docs/quote.rst
+docs/screener.rst
+example/audusd_d1_s.jpg
+example/btcusd_m5_s.jpg
+example/example.ipynb
+example/tsla.jpg
 finvizfinance/__init__.py
+finvizfinance/calendar.py
 finvizfinance/crypto.py
 finvizfinance/earnings.py
 finvizfinance/forex.py
 finvizfinance/future.py
 finvizfinance/insider.py
 finvizfinance/news.py
 finvizfinance/quote.py
```

### Comparing `finvizfinance-0.9.8/setup.py` & `finvizfinance-0.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import setup, find_packages
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.9.8'
+VERSION = '0.9.9'
 PACKAGE_NAME = 'finvizfinance'
 AUTHOR = 'Tianning Li'
 AUTHOR_EMAIL = 'ltianningli@gmail.com'
 URL = 'https://github.com/lit26/finvizfinance'
 
 LICENSE = 'The MIT License (MIT)'
 DESCRIPTION = 'Finviz Finance. Information downloader.'
```

