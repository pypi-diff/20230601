# Comparing `tmp/peachdb-imagebind-0.0.1.tar.gz` & `tmp/peachdb-imagebind-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peachdb-imagebind-0.0.1.tar", last modified: Thu Jun  1 14:30:05 2023, max compression
+gzip compressed data, was "peachdb-imagebind-0.0.2.tar", last modified: Thu Jun  1 14:33:27 2023, max compression
```

## Comparing `peachdb-imagebind-0.0.1.tar` & `peachdb-imagebind-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-01 14:30:05.357674 peachdb-imagebind-0.0.1/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    20848 2023-05-27 00:15:35.000000 peachdb-imagebind-0.0.1/LICENSE
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       83 2023-06-01 14:30:05.357674 peachdb-imagebind-0.0.1/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     4716 2023-05-27 00:15:35.000000 peachdb-imagebind-0.0.1/README.md
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-01 14:30:05.353674 peachdb-imagebind-0.0.1/imagebind/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-01 14:14:54.000000 peachdb-imagebind-0.0.1/imagebind/__init__.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-01 14:30:05.357674 peachdb-imagebind-0.0.1/imagebind/bpe/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)  1356917 2023-06-01 14:14:54.000000 peachdb-imagebind-0.0.1/imagebind/bpe/bpe_simple_vocab_16e6.txt.gz
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    11341 2023-06-01 14:20:53.000000 peachdb-imagebind-0.0.1/imagebind/data.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-01 14:30:05.357674 peachdb-imagebind-0.0.1/imagebind/models/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-01 14:14:54.000000 peachdb-imagebind-0.0.1/imagebind/models/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3989 2023-06-01 14:14:54.000000 peachdb-imagebind-0.0.1/imagebind/models/helpers.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    16162 2023-06-01 14:14:54.000000 peachdb-imagebind-0.0.1/imagebind/models/imagebind_model.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    22618 2023-06-01 14:14:54.000000 peachdb-imagebind-0.0.1/imagebind/models/multimodal_preprocessors.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     9765 2023-06-01 14:14:54.000000 peachdb-imagebind-0.0.1/imagebind/models/transformer.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-01 14:30:05.357674 peachdb-imagebind-0.0.1/peachdb_imagebind.egg-info/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       83 2023-06-01 14:30:05.000000 peachdb-imagebind-0.0.1/peachdb_imagebind.egg-info/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      483 2023-06-01 14:30:05.000000 peachdb-imagebind-0.0.1/peachdb_imagebind.egg-info/SOURCES.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       39 2023-06-01 14:30:05.000000 peachdb-imagebind-0.0.1/peachdb_imagebind.egg-info/dependency_links.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      115 2023-06-01 14:30:05.000000 peachdb-imagebind-0.0.1/peachdb_imagebind.egg-info/requires.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       10 2023-06-01 14:30:05.000000 peachdb-imagebind-0.0.1/peachdb_imagebind.egg-info/top_level.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-06-01 14:30:05.357674 peachdb-imagebind-0.0.1/setup.cfg
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      444 2023-06-01 14:30:01.000000 peachdb-imagebind-0.0.1/setup.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-01 14:33:27.693112 peachdb-imagebind-0.0.2/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    20848 2023-05-27 00:15:35.000000 peachdb-imagebind-0.0.2/LICENSE
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       24 2023-06-01 14:33:15.000000 peachdb-imagebind-0.0.2/MANIFEST.in
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       83 2023-06-01 14:33:27.693112 peachdb-imagebind-0.0.2/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     4716 2023-05-27 00:15:35.000000 peachdb-imagebind-0.0.2/README.md
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-01 14:33:27.689112 peachdb-imagebind-0.0.2/imagebind/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-01 14:14:54.000000 peachdb-imagebind-0.0.2/imagebind/__init__.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-01 14:33:27.689112 peachdb-imagebind-0.0.2/imagebind/bpe/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)  1356917 2023-06-01 14:14:54.000000 peachdb-imagebind-0.0.2/imagebind/bpe/bpe_simple_vocab_16e6.txt.gz
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    11341 2023-06-01 14:20:53.000000 peachdb-imagebind-0.0.2/imagebind/data.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-01 14:33:27.689112 peachdb-imagebind-0.0.2/imagebind/models/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-01 14:14:54.000000 peachdb-imagebind-0.0.2/imagebind/models/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3989 2023-06-01 14:14:54.000000 peachdb-imagebind-0.0.2/imagebind/models/helpers.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    16162 2023-06-01 14:14:54.000000 peachdb-imagebind-0.0.2/imagebind/models/imagebind_model.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    22618 2023-06-01 14:14:54.000000 peachdb-imagebind-0.0.2/imagebind/models/multimodal_preprocessors.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     9765 2023-06-01 14:14:54.000000 peachdb-imagebind-0.0.2/imagebind/models/transformer.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-01 14:33:27.693112 peachdb-imagebind-0.0.2/peachdb_imagebind.egg-info/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       83 2023-06-01 14:33:27.000000 peachdb-imagebind-0.0.2/peachdb_imagebind.egg-info/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      512 2023-06-01 14:33:27.000000 peachdb-imagebind-0.0.2/peachdb_imagebind.egg-info/SOURCES.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       39 2023-06-01 14:33:27.000000 peachdb-imagebind-0.0.2/peachdb_imagebind.egg-info/dependency_links.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      115 2023-06-01 14:33:27.000000 peachdb-imagebind-0.0.2/peachdb_imagebind.egg-info/requires.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       10 2023-06-01 14:33:27.000000 peachdb-imagebind-0.0.2/peachdb_imagebind.egg-info/top_level.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      115 2023-06-01 14:21:40.000000 peachdb-imagebind-0.0.2/requirements.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-06-01 14:33:27.693112 peachdb-imagebind-0.0.2/setup.cfg
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      444 2023-06-01 14:33:23.000000 peachdb-imagebind-0.0.2/setup.py
```

### Comparing `peachdb-imagebind-0.0.1/LICENSE` & `peachdb-imagebind-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `peachdb-imagebind-0.0.1/README.md` & `peachdb-imagebind-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `peachdb-imagebind-0.0.1/imagebind/bpe/bpe_simple_vocab_16e6.txt.gz` & `peachdb-imagebind-0.0.2/imagebind/bpe/bpe_simple_vocab_16e6.txt.gz`

 * *Files identical despite different names*

### Comparing `peachdb-imagebind-0.0.1/imagebind/data.py` & `peachdb-imagebind-0.0.2/imagebind/data.py`

 * *Files identical despite different names*

### Comparing `peachdb-imagebind-0.0.1/imagebind/models/helpers.py` & `peachdb-imagebind-0.0.2/imagebind/models/helpers.py`

 * *Files identical despite different names*

### Comparing `peachdb-imagebind-0.0.1/imagebind/models/imagebind_model.py` & `peachdb-imagebind-0.0.2/imagebind/models/imagebind_model.py`

 * *Files identical despite different names*

### Comparing `peachdb-imagebind-0.0.1/imagebind/models/multimodal_preprocessors.py` & `peachdb-imagebind-0.0.2/imagebind/models/multimodal_preprocessors.py`

 * *Files identical despite different names*

### Comparing `peachdb-imagebind-0.0.1/imagebind/models/transformer.py` & `peachdb-imagebind-0.0.2/imagebind/models/transformer.py`

 * *Files identical despite different names*

