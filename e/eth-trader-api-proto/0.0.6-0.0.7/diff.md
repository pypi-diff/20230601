# Comparing `tmp/eth-trader-api-proto-0.0.6.tar.gz` & `tmp/eth-trader-api-proto-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eth-trader-api-proto-0.0.6.tar", last modified: Thu Jun  1 13:49:44 2023, max compression
+gzip compressed data, was "eth-trader-api-proto-0.0.7.tar", last modified: Thu Jun  1 13:57:36 2023, max compression
```

## Comparing `eth-trader-api-proto-0.0.6.tar` & `eth-trader-api-proto-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 atulsrivastava   (501) staff       (20)        0 2023-06-01 13:49:44.029759 eth-trader-api-proto-0.0.6/
--rw-r--r--   0 atulsrivastava   (501) staff       (20)      114 2023-06-01 13:49:44.029592 eth-trader-api-proto-0.0.6/PKG-INFO
--rw-r--r--   0 atulsrivastava   (501) staff       (20)     1111 2023-06-01 13:49:30.000000 eth-trader-api-proto-0.0.6/README.md
--rw-r--r--   0 atulsrivastava   (501) staff       (20)      357 2023-06-01 13:36:22.000000 eth-trader-api-proto-0.0.6/pyproject.toml
--rw-r--r--   0 atulsrivastava   (501) staff       (20)       38 2023-06-01 13:49:44.029806 eth-trader-api-proto-0.0.6/setup.cfg
-drwxr-xr-x   0 atulsrivastava   (501) staff       (20)        0 2023-06-01 13:49:44.027658 eth-trader-api-proto-0.0.6/src/
-drwxr-xr-x   0 atulsrivastava   (501) staff       (20)        0 2023-06-01 13:49:44.028403 eth-trader-api-proto-0.0.6/src/eth_trader_api/
--rw-r--r--   0 atulsrivastava   (501) staff       (20)        0 2023-06-01 13:35:50.000000 eth-trader-api-proto-0.0.6/src/eth_trader_api/__init__.py
--rw-r--r--   0 atulsrivastava   (501) staff       (20)     5089 2023-06-01 13:35:50.000000 eth-trader-api-proto-0.0.6/src/eth_trader_api/proto.py
-drwxr-xr-x   0 atulsrivastava   (501) staff       (20)        0 2023-06-01 13:49:44.029409 eth-trader-api-proto-0.0.6/src/eth_trader_api_proto.egg-info/
--rw-r--r--   0 atulsrivastava   (501) staff       (20)      114 2023-06-01 13:49:44.000000 eth-trader-api-proto-0.0.6/src/eth_trader_api_proto.egg-info/PKG-INFO
--rw-r--r--   0 atulsrivastava   (501) staff       (20)      322 2023-06-01 13:49:44.000000 eth-trader-api-proto-0.0.6/src/eth_trader_api_proto.egg-info/SOURCES.txt
--rw-r--r--   0 atulsrivastava   (501) staff       (20)        1 2023-06-01 13:49:44.000000 eth-trader-api-proto-0.0.6/src/eth_trader_api_proto.egg-info/dependency_links.txt
--rw-r--r--   0 atulsrivastava   (501) staff       (20)       22 2023-06-01 13:49:44.000000 eth-trader-api-proto-0.0.6/src/eth_trader_api_proto.egg-info/requires.txt
--rw-r--r--   0 atulsrivastava   (501) staff       (20)       15 2023-06-01 13:49:44.000000 eth-trader-api-proto-0.0.6/src/eth_trader_api_proto.egg-info/top_level.txt
+drwxr-xr-x   0 atulsrivastava   (501) staff       (20)        0 2023-06-01 13:57:36.855386 eth-trader-api-proto-0.0.7/
+-rw-r--r--   0 atulsrivastava   (501) staff       (20)      114 2023-06-01 13:57:36.855220 eth-trader-api-proto-0.0.7/PKG-INFO
+-rw-r--r--   0 atulsrivastava   (501) staff       (20)     1111 2023-06-01 13:57:23.000000 eth-trader-api-proto-0.0.7/README.md
+-rw-r--r--   0 atulsrivastava   (501) staff       (20)      357 2023-06-01 13:57:11.000000 eth-trader-api-proto-0.0.7/pyproject.toml
+-rw-r--r--   0 atulsrivastava   (501) staff       (20)       38 2023-06-01 13:57:36.855441 eth-trader-api-proto-0.0.7/setup.cfg
+drwxr-xr-x   0 atulsrivastava   (501) staff       (20)        0 2023-06-01 13:57:36.853211 eth-trader-api-proto-0.0.7/src/
+drwxr-xr-x   0 atulsrivastava   (501) staff       (20)        0 2023-06-01 13:57:36.854176 eth-trader-api-proto-0.0.7/src/eth_trader_api/
+-rw-r--r--   0 atulsrivastava   (501) staff       (20)       20 2023-06-01 13:56:19.000000 eth-trader-api-proto-0.0.7/src/eth_trader_api/__init__.py
+-rw-r--r--   0 atulsrivastava   (501) staff       (20)     5089 2023-06-01 13:56:12.000000 eth-trader-api-proto-0.0.7/src/eth_trader_api/proto.py
+drwxr-xr-x   0 atulsrivastava   (501) staff       (20)        0 2023-06-01 13:57:36.855031 eth-trader-api-proto-0.0.7/src/eth_trader_api_proto.egg-info/
+-rw-r--r--   0 atulsrivastava   (501) staff       (20)      114 2023-06-01 13:57:36.000000 eth-trader-api-proto-0.0.7/src/eth_trader_api_proto.egg-info/PKG-INFO
+-rw-r--r--   0 atulsrivastava   (501) staff       (20)      322 2023-06-01 13:57:36.000000 eth-trader-api-proto-0.0.7/src/eth_trader_api_proto.egg-info/SOURCES.txt
+-rw-r--r--   0 atulsrivastava   (501) staff       (20)        1 2023-06-01 13:57:36.000000 eth-trader-api-proto-0.0.7/src/eth_trader_api_proto.egg-info/dependency_links.txt
+-rw-r--r--   0 atulsrivastava   (501) staff       (20)       22 2023-06-01 13:57:36.000000 eth-trader-api-proto-0.0.7/src/eth_trader_api_proto.egg-info/requires.txt
+-rw-r--r--   0 atulsrivastava   (501) staff       (20)       15 2023-06-01 13:57:36.000000 eth-trader-api-proto-0.0.7/src/eth_trader_api_proto.egg-info/top_level.txt
```

### Comparing `eth-trader-api-proto-0.0.6/README.md` & `eth-trader-api-proto-0.0.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     cd python
     rm -rf dist/ && python3 -m build 
 ```
 
 you can install package locally before uploading it to the pypi
 
 ```shell
-    pip install dist/eth-trader-api-proto-0.0.6.tar.gz
+    pip install dist/eth-trader-api-proto-0.0.7.tar.gz
 ```
 
     (Don't forget to fix the proto compilation issues before releasing)
     To upload this library officially to pypi, use this command
 
 ```shell
     python3 -m twine upload --repository pypi dist/*
```

### Comparing `eth-trader-api-proto-0.0.6/src/eth_trader_api/proto.py` & `eth-trader-api-proto-0.0.7/src/eth_trader_api/proto.py`

 * *Files identical despite different names*

