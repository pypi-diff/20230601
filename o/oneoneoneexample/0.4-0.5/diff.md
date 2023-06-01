# Comparing `tmp/oneoneoneexample-0.4.tar.gz` & `tmp/oneoneoneexample-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oneoneoneexample-0.4.tar", last modified: Wed May 31 22:16:29 2023, max compression
+gzip compressed data, was "oneoneoneexample-0.5.tar", last modified: Thu Jun  1 18:43:19 2023, max compression
```

## Comparing `oneoneoneexample-0.4.tar` & `oneoneoneexample-0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 22:16:29.369442 oneoneoneexample-0.4/
--rw-rw-rw-   0        0        0       61 2023-05-31 22:16:29.369442 oneoneoneexample-0.4/PKG-INFO
--rw-rw-rw-   0        0        0       45 2023-05-31 18:11:11.000000 oneoneoneexample-0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 22:16:29.351924 oneoneoneexample-0.4/oneoneoneexample.egg-info/
--rw-rw-rw-   0        0        0       61 2023-05-31 22:16:29.000000 oneoneoneexample-0.4/oneoneoneexample.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2023-05-31 22:16:29.000000 oneoneoneexample-0.4/oneoneoneexample.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 22:16:29.000000 oneoneoneexample-0.4/oneoneoneexample.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-05-31 22:16:29.000000 oneoneoneexample-0.4/oneoneoneexample.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-31 22:16:29.000000 oneoneoneexample-0.4/oneoneoneexample.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-31 22:16:29.364038 oneoneoneexample-0.4/pdf_generator/
--rw-rw-rw-   0        0        0     4934 2023-05-31 22:14:27.000000 oneoneoneexample-0.4/pdf_generator/convert.py
--rw-rw-rw-   0        0        0      239 2023-05-31 22:14:47.000000 oneoneoneexample-0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-31 22:16:29.369442 oneoneoneexample-0.4/setup.cfg
--rw-rw-rw-   0        0        0      237 2023-05-31 21:36:29.000000 oneoneoneexample-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:43:19.946080 oneoneoneexample-0.5/
+-rw-rw-rw-   0        0        0       61 2023-06-01 18:43:19.944129 oneoneoneexample-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2023-05-31 18:11:11.000000 oneoneoneexample-0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 18:43:19.925086 oneoneoneexample-0.5/oneoneoneexample.egg-info/
+-rw-rw-rw-   0        0        0       61 2023-06-01 18:43:19.000000 oneoneoneexample-0.5/oneoneoneexample.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2023-06-01 18:43:19.000000 oneoneoneexample-0.5/oneoneoneexample.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 18:43:19.000000 oneoneoneexample-0.5/oneoneoneexample.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-06-01 18:43:19.000000 oneoneoneexample-0.5/oneoneoneexample.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-01 18:43:19.000000 oneoneoneexample-0.5/oneoneoneexample.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-01 18:43:19.941975 oneoneoneexample-0.5/pdf_generator/
+-rw-rw-rw-   0        0        0     3327 2023-06-01 18:40:41.000000 oneoneoneexample-0.5/pdf_generator/convert.py
+-rw-rw-rw-   0        0        0      239 2023-06-01 18:41:04.000000 oneoneoneexample-0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-01 18:43:19.946080 oneoneoneexample-0.5/setup.cfg
+-rw-rw-rw-   0        0        0      237 2023-05-31 21:36:29.000000 oneoneoneexample-0.5/setup.py
```

