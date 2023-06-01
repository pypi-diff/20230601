# Comparing `tmp/init_thumbnail-0.1.1.tar.gz` & `tmp/init_thumbnail-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "init_thumbnail-0.1.1.tar", max compression
+gzip compressed data, was "init_thumbnail-0.1.2.tar", max compression
```

## Comparing `init_thumbnail-0.1.1.tar` & `init_thumbnail-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-06-01 14:58:56.109327 init_thumbnail-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-06-01 14:58:56.109252 init_thumbnail-0.1.1/init_thumbnail/__init__.py
--rw-r--r--   0        0        0       56 2023-06-01 16:35:47.195224 init_thumbnail-0.1.1/init_thumbnail/__main__.py
--rw-r--r--   0        0        0     1242 2023-06-01 16:36:21.409060 init_thumbnail-0.1.1/init_thumbnail/main.py
--rw-r--r--   0        0        0      423 2023-06-01 16:40:31.795904 init_thumbnail-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      336 1970-01-01 00:00:00.000000 init_thumbnail-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-01 14:58:56.109327 init_thumbnail-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-01 14:58:56.109252 init_thumbnail-0.1.2/init_thumbnail/__init__.py
+-rw-r--r--   0        0        0       56 2023-06-01 16:35:47.195224 init_thumbnail-0.1.2/init_thumbnail/__main__.py
+-rw-r--r--   0        0        0     1242 2023-06-01 16:42:50.109391 init_thumbnail-0.1.2/init_thumbnail/main.py
+-rw-r--r--   0        0        0      425 2023-06-01 16:45:10.550224 init_thumbnail-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      336 1970-01-01 00:00:00.000000 init_thumbnail-0.1.2/PKG-INFO
```

### Comparing `init_thumbnail-0.1.1/init_thumbnail/main.py` & `init_thumbnail-0.1.2/init_thumbnail/main.py`

 * *Files identical despite different names*

