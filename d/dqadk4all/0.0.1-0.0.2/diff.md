# Comparing `tmp/dqadk4all-0.0.1.tar.gz` & `tmp/dqadk4all-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dqadk4all-0.0.1.tar", last modified: Wed May 31 14:03:18 2023, max compression
+gzip compressed data, was "dqadk4all-0.0.2.tar", last modified: Thu Jun  1 08:40:55 2023, max compression
```

## Comparing `dqadk4all-0.0.1.tar` & `dqadk4all-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 14:03:18.611333 dqadk4all-0.0.1/
--rw-rw-rw-   0        0        0      355 2023-05-31 14:03:18.609336 dqadk4all-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       38 2023-05-31 10:46:38.000000 dqadk4all-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 14:03:18.585334 dqadk4all-0.0.1/dqadk4all/
--rw-rw-rw-   0        0        0       64 2023-05-31 14:01:50.000000 dqadk4all-0.0.1/dqadk4all/__init__.py
--rw-rw-rw-   0        0        0     1206 2023-05-31 14:00:08.000000 dqadk4all-0.0.1/dqadk4all/ge_lib.py
-drwxrwxrwx   0        0        0        0 2023-05-31 14:03:18.606339 dqadk4all-0.0.1/dqadk4all.egg-info/
--rw-rw-rw-   0        0        0      355 2023-05-31 14:03:18.000000 dqadk4all-0.0.1/dqadk4all.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-05-31 14:03:18.000000 dqadk4all-0.0.1/dqadk4all.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 14:03:18.000000 dqadk4all-0.0.1/dqadk4all.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-31 14:03:18.000000 dqadk4all-0.0.1/dqadk4all.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 14:03:18.611333 dqadk4all-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      497 2023-05-31 14:00:54.000000 dqadk4all-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:40:55.899712 dqadk4all-0.0.2/
+-rw-rw-rw-   0        0        0      355 2023-06-01 08:40:55.898713 dqadk4all-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       38 2023-05-31 10:46:38.000000 dqadk4all-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 08:40:55.877713 dqadk4all-0.0.2/dqadk4all/
+-rw-rw-rw-   0        0        0      599 2023-05-31 17:23:59.000000 dqadk4all-0.0.2/dqadk4all/__init__.py
+-rw-rw-rw-   0        0        0    25069 2023-05-31 17:28:14.000000 dqadk4all-0.0.2/dqadk4all/ge_lib.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:40:55.897712 dqadk4all-0.0.2/dqadk4all.egg-info/
+-rw-rw-rw-   0        0        0      355 2023-06-01 08:40:55.000000 dqadk4all-0.0.2/dqadk4all.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-06-01 08:40:55.000000 dqadk4all-0.0.2/dqadk4all.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 08:40:55.000000 dqadk4all-0.0.2/dqadk4all.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-01 08:40:55.000000 dqadk4all-0.0.2/dqadk4all.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 08:40:55.899712 dqadk4all-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      497 2023-06-01 08:40:28.000000 dqadk4all-0.0.2/setup.py
```

