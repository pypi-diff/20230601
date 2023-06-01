# Comparing `tmp/spaces-0.1.3.tar.gz` & `tmp/spaces-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spaces-0.1.3.tar", max compression
+gzip compressed data, was "spaces-0.2.0.tar", max compression
```

## Comparing `spaces-0.1.3.tar` & `spaces-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,13 @@
--rw-r--r--   0        0        0       61 2023-04-27 15:34:16.931108 spaces-0.1.3/README.md
--rw-r--r--   0        0        0      532 2023-04-27 16:28:17.320678 spaces-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       80 2023-04-27 15:40:38.868471 spaces-0.1.3/spaces/__init__.py
--rw-r--r--   0        0        0      103 2023-04-27 15:40:23.864577 spaces-0.1.3/spaces/gpu/__init__.py
--rw-r--r--   0        0        0      612 2023-04-27 16:27:32.868982 spaces-0.1.3/spaces/gpu/client.py
--rw-r--r--   0        0        0     5396 2023-04-27 15:36:02.266379 spaces-0.1.3/spaces/gpu/decorator.py
--rw-r--r--   0        0        0     1183 2023-04-27 15:39:25.436982 spaces-0.1.3/spaces/gpu/patching.py
--rw-r--r--   0        0        0      362 2023-04-27 16:25:15.393923 spaces-0.1.3/spaces/utils.py
--rw-r--r--   0        0        0      806 1970-01-01 00:00:00.000000 spaces-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       61 2023-02-23 09:04:36.869652 spaces-0.2.0/README.md
+-rw-r--r--   0        0        0     1302 2023-06-01 09:07:32.352913 spaces-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      168 2023-05-23 16:06:07.578194 spaces-0.2.0/spaces/__init__.py
+-rw-r--r--   0        0        0       61 2023-05-23 12:16:01.390521 spaces-0.2.0/spaces/config.py
+-rw-r--r--   0        0        0      259 2023-05-30 12:29:38.149333 spaces-0.2.0/spaces/gpu/__init__.py
+-rw-r--r--   0        0        0     1577 2023-05-31 17:56:04.987325 spaces-0.2.0/spaces/gpu/client.py
+-rw-r--r--   0        0        0     1107 2023-05-23 15:41:58.726616 spaces-0.2.0/spaces/gpu/decorator.py
+-rw-r--r--   0        0        0     3579 2023-05-30 13:33:47.192592 spaces-0.2.0/spaces/gpu/torch.py
+-rw-r--r--   0        0        0     6528 2023-05-31 15:42:07.658085 spaces-0.2.0/spaces/gpu/wrappers.py
+-rw-r--r--   0        0        0     1147 2023-05-29 13:46:54.364944 spaces-0.2.0/spaces/gradio.py
+-rw-r--r--   0        0        0     1386 2023-05-30 13:53:53.832283 spaces-0.2.0/spaces/utils.py
+-rw-r--r--   0        0        0      815 1970-01-01 00:00:00.000000 spaces-0.2.0/setup.py
+-rw-r--r--   0        0        0      848 1970-01-01 00:00:00.000000 spaces-0.2.0/PKG-INFO
```

### Comparing `spaces-0.1.3/PKG-INFO` & `spaces-0.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: spaces
-Version: 0.1.3
+Version: 0.2.0
 Summary: Utilities for Hugging Face Spaces
 Home-page: https://huggingface.co
 License: Apache-2.0
 Author: Charles Bensimon
 Author-email: charles@huggingface.co
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: psutil (>=5.9.5,<6.0.0)
+Requires-Dist: pydantic (>=1.10.8,<2.0.0)
 Requires-Dist: requests (>=2.29.0,<3.0.0)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
 Project-URL: Repository, https://github.com/huggingface/huggingface_hub
 Description-Content-Type: text/markdown
 
 # Hugging Face Spaces
```

