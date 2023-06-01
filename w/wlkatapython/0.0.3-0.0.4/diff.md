# Comparing `tmp/wlkatapython-0.0.3.tar.gz` & `tmp/wlkatapython-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wlkatapython-0.0.3.tar", last modified: Thu Jun  1 12:43:23 2023, max compression
+gzip compressed data, was "wlkatapython-0.0.4.tar", last modified: Thu Jun  1 13:06:21 2023, max compression
```

## Comparing `wlkatapython-0.0.3.tar` & `wlkatapython-0.0.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 12:43:23.695996 wlkatapython-0.0.3/
--rw-rw-rw-   0        0        0      302 2023-06-01 12:43:23.694997 wlkatapython-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-01 12:43:23.695996 wlkatapython-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      419 2023-06-01 12:42:54.000000 wlkatapython-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-01 12:43:23.693990 wlkatapython-0.0.3/wlkatapython.egg-info/
--rw-rw-rw-   0        0        0      302 2023-06-01 12:43:23.000000 wlkatapython-0.0.3/wlkatapython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      168 2023-06-01 12:43:23.000000 wlkatapython-0.0.3/wlkatapython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 12:43:23.000000 wlkatapython-0.0.3/wlkatapython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-01 12:43:23.000000 wlkatapython-0.0.3/wlkatapython.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    10136 2023-06-01 11:48:59.000000 wlkatapython-0.0.3/wlkatapython.py
+drwxrwxrwx   0        0        0        0 2023-06-01 13:06:21.236503 wlkatapython-0.0.4/
+-rw-rw-rw-   0        0        0      367 2023-06-01 13:06:21.236503 wlkatapython-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-01 13:06:21.236503 wlkatapython-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      477 2023-06-01 13:06:02.000000 wlkatapython-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 13:06:21.235501 wlkatapython-0.0.4/wlkatapython.egg-info/
+-rw-rw-rw-   0        0        0      367 2023-06-01 13:06:21.000000 wlkatapython-0.0.4/wlkatapython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      168 2023-06-01 13:06:21.000000 wlkatapython-0.0.4/wlkatapython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 13:06:21.000000 wlkatapython-0.0.4/wlkatapython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-01 13:06:21.000000 wlkatapython-0.0.4/wlkatapython.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    10136 2023-06-01 11:48:59.000000 wlkatapython-0.0.4/wlkatapython.py
```

### Comparing `wlkatapython-0.0.3/wlkatapython.py` & `wlkatapython-0.0.4/wlkatapython.py`

 * *Files identical despite different names*

