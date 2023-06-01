# Comparing `tmp/comex-0.1.0.tar.gz` & `tmp/comex-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comex-0.1.0.tar", last modified: Sat May 27 08:52:35 2023, max compression
+gzip compressed data, was "comex-0.1.1.tar", last modified: Thu Jun  1 12:42:45 2023, max compression
```

## Comparing `comex-0.1.0.tar` & `comex-0.1.1.tar`

### file list

```diff
@@ -1,58 +1,60 @@
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:52:35.060000 comex-0.1.0/
--rwxrwxrwx   0 noble      (501) staff       (20)    11357 2023-05-09 06:59:54.000000 comex-0.1.0/LICENSE
--rwxrwxrwx   0 noble      (501) staff       (20)     8106 2023-05-27 08:52:35.100000 comex-0.1.0/PKG-INFO
--rwxrwxrwx   0 noble      (501) staff       (20)     7489 2023-05-27 06:29:25.000000 comex-0.1.0/README.md
--rwxrwxrwx   0 noble      (501) staff       (20)     1036 2023-05-27 08:52:35.100000 comex-0.1.0/setup.cfg
--rwxrwxrwx   0 noble      (501) staff       (20)       38 2023-05-09 06:59:54.000000 comex-0.1.0/setup.py
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:52:35.060000 comex-0.1.0/src/
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:52:35.060000 comex-0.1.0/src/comex/
--rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:28:52.000000 comex-0.1.0/src/comex/__init__.py
--rwxrwxrwx   0 noble      (501) staff       (20)      109 2023-05-27 08:28:48.000000 comex-0.1.0/src/comex/__main__.py
--rwxrwxrwx   0 noble      (501) staff       (20)     3664 2023-05-27 08:52:22.000000 comex-0.1.0/src/comex/cli.py
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:52:35.060000 comex-0.1.0/src/comex/codeviews/
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:52:35.060000 comex-0.1.0/src/comex/codeviews/AST/
--rwxrwxrwx   0 noble      (501) staff       (20)     4196 2023-05-09 06:59:54.000000 comex-0.1.0/src/comex/codeviews/AST/AST.py
--rwxrwxrwx   0 noble      (501) staff       (20)      968 2023-05-27 08:37:58.000000 comex-0.1.0/src/comex/codeviews/AST/AST_driver.py
--rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-09 06:59:54.000000 comex-0.1.0/src/comex/codeviews/AST/__init__.py
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:52:35.060000 comex-0.1.0/src/comex/codeviews/CFG/
--rwxrwxrwx   0 noble      (501) staff       (20)     1426 2023-05-09 06:59:54.000000 comex-0.1.0/src/comex/codeviews/CFG/CFG.py
--rwxrwxrwx   0 noble      (501) staff       (20)    51528 2023-05-27 08:37:07.000000 comex-0.1.0/src/comex/codeviews/CFG/CFG_csharp.py
--rwxrwxrwx   0 noble      (501) staff       (20)     1300 2023-05-27 08:37:31.000000 comex-0.1.0/src/comex/codeviews/CFG/CFG_driver.py
--rwxrwxrwx   0 noble      (501) staff       (20)    78323 2023-05-27 08:37:41.000000 comex-0.1.0/src/comex/codeviews/CFG/CFG_java.py
--rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-09 06:59:54.000000 comex-0.1.0/src/comex/codeviews/CFG/__init__.py
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:52:35.060000 comex-0.1.0/src/comex/codeviews/CST/
--rwxrwxrwx   0 noble      (501) staff       (20)     2540 2023-05-27 08:36:43.000000 comex-0.1.0/src/comex/codeviews/CST/CST_driver.py
--rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-09 06:59:54.000000 comex-0.1.0/src/comex/codeviews/CST/__init__.py
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:52:35.060000 comex-0.1.0/src/comex/codeviews/DFG/
--rwxrwxrwx   0 noble      (501) staff       (20)     1246 2023-05-27 08:38:26.000000 comex-0.1.0/src/comex/codeviews/DFG/DFG_driver.py
--rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-09 06:59:54.000000 comex-0.1.0/src/comex/codeviews/DFG/__init__.py
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:52:35.060000 comex-0.1.0/src/comex/codeviews/SDFG/
--rwxrwxrwx   0 noble      (501) staff       (20)     4535 2023-05-27 08:38:37.000000 comex-0.1.0/src/comex/codeviews/SDFG/SDFG.py
--rwxrwxrwx   0 noble      (501) staff       (20)    32117 2023-05-27 08:38:51.000000 comex-0.1.0/src/comex/codeviews/SDFG/SDFG_csharp.py
--rwxrwxrwx   0 noble      (501) staff       (20)    61608 2023-05-27 08:38:58.000000 comex-0.1.0/src/comex/codeviews/SDFG/SDFG_java.py
--rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-09 06:59:54.000000 comex-0.1.0/src/comex/codeviews/SDFG/__init__.py
--rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-09 06:59:54.000000 comex-0.1.0/src/comex/codeviews/__init__.py
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:52:35.060000 comex-0.1.0/src/comex/codeviews/combined_graph/
--rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-09 06:59:54.000000 comex-0.1.0/src/comex/codeviews/combined_graph/__init__.py
--rwxrwxrwx   0 noble      (501) staff       (20)     9551 2023-05-27 08:36:32.000000 comex-0.1.0/src/comex/codeviews/combined_graph/combined_driver.py
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:52:35.060000 comex-0.1.0/src/comex/tree_parser/
--rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:49:05.000000 comex-0.1.0/src/comex/tree_parser/__init__.py
--rwxrwxrwx   0 noble      (501) staff       (20)     8617 2023-05-27 08:35:50.000000 comex-0.1.0/src/comex/tree_parser/cs_parser.py
--rwxrwxrwx   0 noble      (501) staff       (20)     6152 2023-05-27 08:04:01.000000 comex-0.1.0/src/comex/tree_parser/custom_parser.py
--rwxrwxrwx   0 noble      (501) staff       (20)    10057 2023-05-27 08:35:58.000000 comex-0.1.0/src/comex/tree_parser/java_parser.py
--rwxrwxrwx   0 noble      (501) staff       (20)     1819 2023-05-27 08:36:07.000000 comex-0.1.0/src/comex/tree_parser/parser_driver.py
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:52:35.060000 comex-0.1.0/src/comex/utils/
--rwxrwxrwx   0 noble      (501) staff       (20)     1763 2023-05-09 07:00:15.000000 comex-0.1.0/src/comex/utils/DFG_utils.py
--rwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:48:37.000000 comex-0.1.0/src/comex/utils/__init__.py
--rwxrwxrwx   0 noble      (501) staff       (20)    19424 2023-05-24 03:11:00.000000 comex-0.1.0/src/comex/utils/cs_nodes.py
--rwxrwxrwx   0 noble      (501) staff       (20)    25191 2023-05-09 06:59:54.000000 comex-0.1.0/src/comex/utils/java_nodes.py
--rwxrwxrwx   0 noble      (501) staff       (20)     1083 2023-05-09 06:59:54.000000 comex-0.1.0/src/comex/utils/postprocessor.py
--rwxrwxrwx   0 noble      (501) staff       (20)     2418 2023-05-09 06:59:54.000000 comex-0.1.0/src/comex/utils/preprocessor.py
--rwxrwxrwx   0 noble      (501) staff       (20)     2055 2023-05-09 06:59:54.000000 comex-0.1.0/src/comex/utils/src_parser.py
-drwxrwxrwx   0 noble      (501) staff       (20)        0 2023-05-27 08:52:35.060000 comex-0.1.0/src/comex.egg-info/
--rwxrwxrwx   0 noble      (501) staff       (20)     8106 2023-05-27 08:52:35.000000 comex-0.1.0/src/comex.egg-info/PKG-INFO
--rwxrwxrwx   0 noble      (501) staff       (20)     1404 2023-05-27 08:52:35.000000 comex-0.1.0/src/comex.egg-info/SOURCES.txt
--rwxrwxrwx   0 noble      (501) staff       (20)        1 2023-05-27 08:52:35.000000 comex-0.1.0/src/comex.egg-info/dependency_links.txt
--rwxrwxrwx   0 noble      (501) staff       (20)       40 2023-05-27 08:52:35.000000 comex-0.1.0/src/comex.egg-info/entry_points.txt
--rwxrwxrwx   0 noble      (501) staff       (20)      151 2023-05-27 08:52:35.000000 comex-0.1.0/src/comex.egg-info/requires.txt
--rwxrwxrwx   0 noble      (501) staff       (20)        6 2023-05-27 08:52:35.000000 comex-0.1.0/src/comex.egg-info/top_level.txt
+drwxr-xr-x   0 noble      (501) staff       (20)        0 2023-06-01 12:42:45.915888 comex-0.1.1/
+-rw-r--r--   0 noble      (501) staff       (20)    11357 2023-06-01 12:38:00.000000 comex-0.1.1/LICENSE
+-rw-r--r--   0 noble      (501) staff       (20)     8209 2023-06-01 12:42:45.915991 comex-0.1.1/PKG-INFO
+-rw-r--r--   0 noble      (501) staff       (20)     7592 2023-06-01 12:38:00.000000 comex-0.1.1/README.md
+-rw-r--r--   0 noble      (501) staff       (20)     1036 2023-06-01 12:42:45.916386 comex-0.1.1/setup.cfg
+-rw-r--r--   0 noble      (501) staff       (20)       38 2023-06-01 12:38:00.000000 comex-0.1.1/setup.py
+drwxr-xr-x   0 noble      (501) staff       (20)        0 2023-06-01 12:42:45.908534 comex-0.1.1/src/
+drwxr-xr-x   0 noble      (501) staff       (20)        0 2023-06-01 12:42:45.910353 comex-0.1.1/src/comex/
+-rw-r--r--   0 noble      (501) staff       (20)        0 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/__init__.py
+-rw-r--r--   0 noble      (501) staff       (20)      104 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/__main__.py
+-rw-r--r--   0 noble      (501) staff       (20)     3664 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/cli.py
+drwxr-xr-x   0 noble      (501) staff       (20)        0 2023-06-01 12:42:45.911340 comex-0.1.1/src/comex/codeviews/
+drwxr-xr-x   0 noble      (501) staff       (20)        0 2023-06-01 12:42:45.911731 comex-0.1.1/src/comex/codeviews/AST/
+-rw-r--r--   0 noble      (501) staff       (20)     4196 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/codeviews/AST/AST.py
+-rw-r--r--   0 noble      (501) staff       (20)      968 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/codeviews/AST/AST_driver.py
+-rw-r--r--   0 noble      (501) staff       (20)        0 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/codeviews/AST/__init__.py
+drwxr-xr-x   0 noble      (501) staff       (20)        0 2023-06-01 12:42:45.912689 comex-0.1.1/src/comex/codeviews/CFG/
+-rw-r--r--   0 noble      (501) staff       (20)     1426 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/codeviews/CFG/CFG.py
+-rw-r--r--   0 noble      (501) staff       (20)    51528 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/codeviews/CFG/CFG_csharp.py
+-rw-r--r--   0 noble      (501) staff       (20)     1300 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/codeviews/CFG/CFG_driver.py
+-rw-r--r--   0 noble      (501) staff       (20)    78323 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/codeviews/CFG/CFG_java.py
+-rw-r--r--   0 noble      (501) staff       (20)        0 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/codeviews/CFG/__init__.py
+drwxr-xr-x   0 noble      (501) staff       (20)        0 2023-06-01 12:42:45.913002 comex-0.1.1/src/comex/codeviews/CST/
+-rw-r--r--   0 noble      (501) staff       (20)     2540 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/codeviews/CST/CST_driver.py
+-rw-r--r--   0 noble      (501) staff       (20)        0 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/codeviews/CST/__init__.py
+drwxr-xr-x   0 noble      (501) staff       (20)        0 2023-06-01 12:42:45.913297 comex-0.1.1/src/comex/codeviews/DFG/
+-rw-r--r--   0 noble      (501) staff       (20)     1246 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/codeviews/DFG/DFG_driver.py
+-rw-r--r--   0 noble      (501) staff       (20)        0 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/codeviews/DFG/__init__.py
+drwxr-xr-x   0 noble      (501) staff       (20)        0 2023-06-01 12:42:45.913865 comex-0.1.1/src/comex/codeviews/SDFG/
+-rw-r--r--   0 noble      (501) staff       (20)     4535 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/codeviews/SDFG/SDFG.py
+-rw-r--r--   0 noble      (501) staff       (20)    32117 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/codeviews/SDFG/SDFG_csharp.py
+-rw-r--r--   0 noble      (501) staff       (20)    61608 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/codeviews/SDFG/SDFG_java.py
+-rw-r--r--   0 noble      (501) staff       (20)        0 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/codeviews/SDFG/__init__.py
+-rw-r--r--   0 noble      (501) staff       (20)        0 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/codeviews/__init__.py
+drwxr-xr-x   0 noble      (501) staff       (20)        0 2023-06-01 12:42:45.914083 comex-0.1.1/src/comex/codeviews/combined_graph/
+-rw-r--r--   0 noble      (501) staff       (20)        0 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/codeviews/combined_graph/__init__.py
+-rw-r--r--   0 noble      (501) staff       (20)     9551 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/codeviews/combined_graph/combined_driver.py
+drwxr-xr-x   0 noble      (501) staff       (20)        0 2023-06-01 12:42:45.914705 comex-0.1.1/src/comex/tree_parser/
+-rw-r--r--   0 noble      (501) staff       (20)        0 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/tree_parser/__init__.py
+-rw-r--r--   0 noble      (501) staff       (20)     8617 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/tree_parser/cs_parser.py
+-rw-r--r--   0 noble      (501) staff       (20)     6152 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/tree_parser/custom_parser.py
+-rw-r--r--   0 noble      (501) staff       (20)    10057 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/tree_parser/java_parser.py
+-rw-r--r--   0 noble      (501) staff       (20)     1818 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/tree_parser/parser_driver.py
+drwxr-xr-x   0 noble      (501) staff       (20)        0 2023-06-01 12:42:45.915630 comex-0.1.1/src/comex/utils/
+-rw-r--r--   0 noble      (501) staff       (20)     1763 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/utils/DFG_utils.py
+-rw-r--r--   0 noble      (501) staff       (20)        0 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/utils/__init__.py
+-rw-r--r--   0 noble      (501) staff       (20)    19424 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/utils/cs_nodes.py
+-rw-r--r--   0 noble      (501) staff       (20)    25191 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/utils/java_nodes.py
+-rw-r--r--   0 noble      (501) staff       (20)     1083 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/utils/postprocessor.py
+-rw-r--r--   0 noble      (501) staff       (20)     2418 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/utils/preprocessor.py
+-rw-r--r--   0 noble      (501) staff       (20)     2055 2023-06-01 12:38:00.000000 comex-0.1.1/src/comex/utils/src_parser.py
+drwxr-xr-x   0 noble      (501) staff       (20)        0 2023-06-01 12:42:45.911200 comex-0.1.1/src/comex.egg-info/
+-rw-r--r--   0 noble      (501) staff       (20)     8209 2023-06-01 12:42:45.000000 comex-0.1.1/src/comex.egg-info/PKG-INFO
+-rw-r--r--   0 noble      (501) staff       (20)     1428 2023-06-01 12:42:45.000000 comex-0.1.1/src/comex.egg-info/SOURCES.txt
+-rw-r--r--   0 noble      (501) staff       (20)        1 2023-06-01 12:42:45.000000 comex-0.1.1/src/comex.egg-info/dependency_links.txt
+-rw-r--r--   0 noble      (501) staff       (20)       40 2023-06-01 12:42:45.000000 comex-0.1.1/src/comex.egg-info/entry_points.txt
+-rw-r--r--   0 noble      (501) staff       (20)      151 2023-06-01 12:42:45.000000 comex-0.1.1/src/comex.egg-info/requires.txt
+-rw-r--r--   0 noble      (501) staff       (20)        6 2023-06-01 12:42:45.000000 comex-0.1.1/src/comex.egg-info/top_level.txt
+drwxr-xr-x   0 noble      (501) staff       (20)        0 2023-06-01 12:42:45.915770 comex-0.1.1/tests/
+-rw-r--r--   0 noble      (501) staff       (20)     4508 2023-06-01 12:38:00.000000 comex-0.1.1/tests/test_codeviews.py
```

### Comparing `comex-0.1.0/LICENSE` & `comex-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `comex-0.1.0/PKG-INFO` & `comex-0.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,53 +1,33 @@
-Metadata-Version: 2.1
-Name: comex
-Version: 0.1.0
-Summary: Generate combined multi-code view graphs
-Home-page: https://github.com/IBM/tree-sitter-codeviews
-License: Apache-2.0
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # Tree Sitter Multi Codeview Generator
 
-Tree Sitter Multi Codeview Generator aims to generate combined multi-code view graphs that can be used with various types of machine learning models (sequence model neural networks, graph neural networks, etc). It is also designed to be easily extended to various source code languages. [tree-sitter](https://tree-sitter.github.io/tree-sitter/) is used for parsing which is highly efficient and has support for over 40+ languages. Currently, this repository supports codeviews for Java in over 40 possible combinations of codeviews. It has been structured such that support for other languages can be easily added. If you wish to add support for more languages, please refer to the [contributing](https://github.com/IBM/tree-sitter-codeviews/blob/main/CONTRIBUTING.md) guide.
+Tree Sitter Multi Codeview Generator aims to generate combined multi-code view graphs that can be used with various types of machine learning models (sequence models, graph neural networks, etc). 
+
+# Comex
+`comex` is a rebuild of Tree Sitter Multi Codeview Generator for easier invocation as a Python package. This rebuild also includes a cli interface. Currently, ```comex``` generates codeviews for Java and C#, for both method-level and file-level code snippets.  ```comex``` can be used to generate over $15$ possible combinations of codeviews for both languages (complete list [here](https://github.com/IBM/tree-sitter-codeviews/blob/main/List_Of_Views.pdf)). ```comex``` is designed to be easily extendable to various programming languages. This is primarliy because we use [tree-sitter](https://tree-sitter.github.io/tree-sitter/) for parsing, a highly efficient incremental parser that supports over $40$ languages. If you wish to add support for more languages, please refer to the [contributing](https://github.com/IBM/tree-sitter-codeviews/blob/main/CONTRIBUTING.md) guide.
 
-## Comex
-`comex` is a rebuild of Tree Sitter Multi Codeview Generator for easier invocation as a Python package. 
-This rebuild also includes a cli interface for easier usage.
-It isolates the logic pertaining to the generation and combination of codeviews to better differentiate tasks involved in the `IBM OSCP Project`.
+**Note**: While C# _method-level_ support is available on the ```main``` branch, _file-level_ support is available on the ```dev``` branch but is currently under active development and testing.
 
-### Installation
+## Installation from PyPi
 
 `comex` is published on the Python Registry and can be easily installed via pip:
 
 ```console
 pip install comex
 ```
 
 **Note**: You would need to install GraphViz([dot](https://graphviz.org/download/)) so that the graph visualizations are generated
 
----
+## Installation from source
+
 To setup `comex` for development using the source code in your python environment:
 
 ```console
 pip install -r requirements-dev.txt
 ```
-**Note**: Please clone recursively so sub-modules are setup correctly
-```console
-git clone --recursive {...}
-```
 
 This performs an editable install, meaning that comex would be available throughout your environment (particularly relevant if you use conda or something of the sort). This means now you can interact and import from `comex` just like any other package while remaining standalone but also reflecting any code side updates without any other manual steps
 
 ---
 ### Usage as a CLI
 
 This is the recommended way to get started with `comex` as it is the most user friendly
```

### Comparing `comex-0.1.0/README.md` & `comex-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,50 @@
+Metadata-Version: 2.1
+Name: comex
+Version: 0.1.1
+Summary: Generate combined multi-code view graphs
+Home-page: https://github.com/IBM/tree-sitter-codeviews
+License: Apache-2.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 # Tree Sitter Multi Codeview Generator
 
-Tree Sitter Multi Codeview Generator aims to generate combined multi-code view graphs that can be used with various types of machine learning models (sequence model neural networks, graph neural networks, etc). It is also designed to be easily extended to various source code languages. [tree-sitter](https://tree-sitter.github.io/tree-sitter/) is used for parsing which is highly efficient and has support for over 40+ languages. Currently, this repository supports codeviews for Java in over 40 possible combinations of codeviews. It has been structured such that support for other languages can be easily added. If you wish to add support for more languages, please refer to the [contributing](https://github.com/IBM/tree-sitter-codeviews/blob/main/CONTRIBUTING.md) guide.
+Tree Sitter Multi Codeview Generator aims to generate combined multi-code view graphs that can be used with various types of machine learning models (sequence models, graph neural networks, etc). 
+
+# Comex
+`comex` is a rebuild of Tree Sitter Multi Codeview Generator for easier invocation as a Python package. This rebuild also includes a cli interface. Currently, ```comex``` generates codeviews for Java and C#, for both method-level and file-level code snippets.  ```comex``` can be used to generate over $15$ possible combinations of codeviews for both languages (complete list [here](https://github.com/IBM/tree-sitter-codeviews/blob/main/List_Of_Views.pdf)). ```comex``` is designed to be easily extendable to various programming languages. This is primarliy because we use [tree-sitter](https://tree-sitter.github.io/tree-sitter/) for parsing, a highly efficient incremental parser that supports over $40$ languages. If you wish to add support for more languages, please refer to the [contributing](https://github.com/IBM/tree-sitter-codeviews/blob/main/CONTRIBUTING.md) guide.
 
-## Comex
-`comex` is a rebuild of Tree Sitter Multi Codeview Generator for easier invocation as a Python package. 
-This rebuild also includes a cli interface for easier usage.
-It isolates the logic pertaining to the generation and combination of codeviews to better differentiate tasks involved in the `IBM OSCP Project`.
+**Note**: While C# _method-level_ support is available on the ```main``` branch, _file-level_ support is available on the ```dev``` branch but is currently under active development and testing.
 
-### Installation
+## Installation from PyPi
 
 `comex` is published on the Python Registry and can be easily installed via pip:
 
 ```console
 pip install comex
 ```
 
 **Note**: You would need to install GraphViz([dot](https://graphviz.org/download/)) so that the graph visualizations are generated
 
----
+## Installation from source
+
 To setup `comex` for development using the source code in your python environment:
 
 ```console
 pip install -r requirements-dev.txt
 ```
-**Note**: Please clone recursively so sub-modules are setup correctly
-```console
-git clone --recursive {...}
-```
 
 This performs an editable install, meaning that comex would be available throughout your environment (particularly relevant if you use conda or something of the sort). This means now you can interact and import from `comex` just like any other package while remaining standalone but also reflecting any code side updates without any other manual steps
 
 ---
 ### Usage as a CLI
 
 This is the recommended way to get started with `comex` as it is the most user friendly
```

### Comparing `comex-0.1.0/setup.cfg` & `comex-0.1.1/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = comex
-version = 0.1.0
+version = 0.1.1
 description = Generate combined multi-code view graphs
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/IBM/tree-sitter-codeviews
 license = Apache-2.0
 license_file = LICENSE
 classifiers =
```

### Comparing `comex-0.1.0/src/comex/cli.py` & `comex-0.1.1/src/comex/cli.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.0/src/comex/codeviews/AST/AST.py` & `comex-0.1.1/src/comex/codeviews/AST/AST.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.0/src/comex/codeviews/AST/AST_driver.py` & `comex-0.1.1/src/comex/codeviews/AST/AST_driver.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.0/src/comex/codeviews/CFG/CFG.py` & `comex-0.1.1/src/comex/codeviews/CFG/CFG.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.0/src/comex/codeviews/CFG/CFG_csharp.py` & `comex-0.1.1/src/comex/codeviews/CFG/CFG_csharp.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.0/src/comex/codeviews/CFG/CFG_driver.py` & `comex-0.1.1/src/comex/codeviews/CFG/CFG_driver.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.0/src/comex/codeviews/CFG/CFG_java.py` & `comex-0.1.1/src/comex/codeviews/CFG/CFG_java.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.0/src/comex/codeviews/CST/CST_driver.py` & `comex-0.1.1/src/comex/codeviews/CST/CST_driver.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.0/src/comex/codeviews/DFG/DFG_driver.py` & `comex-0.1.1/src/comex/codeviews/DFG/DFG_driver.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.0/src/comex/codeviews/SDFG/SDFG.py` & `comex-0.1.1/src/comex/codeviews/SDFG/SDFG.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.0/src/comex/codeviews/SDFG/SDFG_csharp.py` & `comex-0.1.1/src/comex/codeviews/SDFG/SDFG_csharp.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.0/src/comex/codeviews/SDFG/SDFG_java.py` & `comex-0.1.1/src/comex/codeviews/SDFG/SDFG_java.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.0/src/comex/codeviews/combined_graph/combined_driver.py` & `comex-0.1.1/src/comex/codeviews/combined_graph/combined_driver.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.0/src/comex/tree_parser/cs_parser.py` & `comex-0.1.1/src/comex/tree_parser/cs_parser.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.0/src/comex/tree_parser/custom_parser.py` & `comex-0.1.1/src/comex/tree_parser/custom_parser.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.0/src/comex/tree_parser/java_parser.py` & `comex-0.1.1/src/comex/tree_parser/java_parser.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.0/src/comex/tree_parser/parser_driver.py` & `comex-0.1.1/src/comex/tree_parser/parser_driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from ..tree_parser.java_parser import JavaParser
 from ..tree_parser.cs_parser import CSParser
 from ..utils import preprocessor
 
-
 class ParserDriver:
     """Driver class for the parser"""
 
     def __init__(self, src_language, src_code):
         """Initialize the driver. Preprocess the code before parsing"""
         self.src_language = src_language
         self.src_code = self.pre_process_src_code(src_language, src_code)
```

### Comparing `comex-0.1.0/src/comex/utils/DFG_utils.py` & `comex-0.1.1/src/comex/utils/DFG_utils.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.0/src/comex/utils/cs_nodes.py` & `comex-0.1.1/src/comex/utils/cs_nodes.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.0/src/comex/utils/java_nodes.py` & `comex-0.1.1/src/comex/utils/java_nodes.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.0/src/comex/utils/postprocessor.py` & `comex-0.1.1/src/comex/utils/postprocessor.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.0/src/comex/utils/preprocessor.py` & `comex-0.1.1/src/comex/utils/preprocessor.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.0/src/comex/utils/src_parser.py` & `comex-0.1.1/src/comex/utils/src_parser.py`

 * *Files identical despite different names*

### Comparing `comex-0.1.0/src/comex.egg-info/PKG-INFO` & `comex-0.1.1/src/comex.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comex
-Version: 0.1.0
+Version: 0.1.1
 Summary: Generate combined multi-code view graphs
 Home-page: https://github.com/IBM/tree-sitter-codeviews
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -13,41 +13,38 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Tree Sitter Multi Codeview Generator
 
-Tree Sitter Multi Codeview Generator aims to generate combined multi-code view graphs that can be used with various types of machine learning models (sequence model neural networks, graph neural networks, etc). It is also designed to be easily extended to various source code languages. [tree-sitter](https://tree-sitter.github.io/tree-sitter/) is used for parsing which is highly efficient and has support for over 40+ languages. Currently, this repository supports codeviews for Java in over 40 possible combinations of codeviews. It has been structured such that support for other languages can be easily added. If you wish to add support for more languages, please refer to the [contributing](https://github.com/IBM/tree-sitter-codeviews/blob/main/CONTRIBUTING.md) guide.
+Tree Sitter Multi Codeview Generator aims to generate combined multi-code view graphs that can be used with various types of machine learning models (sequence models, graph neural networks, etc). 
 
-## Comex
-`comex` is a rebuild of Tree Sitter Multi Codeview Generator for easier invocation as a Python package. 
-This rebuild also includes a cli interface for easier usage.
-It isolates the logic pertaining to the generation and combination of codeviews to better differentiate tasks involved in the `IBM OSCP Project`.
+# Comex
+`comex` is a rebuild of Tree Sitter Multi Codeview Generator for easier invocation as a Python package. This rebuild also includes a cli interface. Currently, ```comex``` generates codeviews for Java and C#, for both method-level and file-level code snippets.  ```comex``` can be used to generate over $15$ possible combinations of codeviews for both languages (complete list [here](https://github.com/IBM/tree-sitter-codeviews/blob/main/List_Of_Views.pdf)). ```comex``` is designed to be easily extendable to various programming languages. This is primarliy because we use [tree-sitter](https://tree-sitter.github.io/tree-sitter/) for parsing, a highly efficient incremental parser that supports over $40$ languages. If you wish to add support for more languages, please refer to the [contributing](https://github.com/IBM/tree-sitter-codeviews/blob/main/CONTRIBUTING.md) guide.
 
-### Installation
+**Note**: While C# _method-level_ support is available on the ```main``` branch, _file-level_ support is available on the ```dev``` branch but is currently under active development and testing.
+
+## Installation from PyPi
 
 `comex` is published on the Python Registry and can be easily installed via pip:
 
 ```console
 pip install comex
 ```
 
 **Note**: You would need to install GraphViz([dot](https://graphviz.org/download/)) so that the graph visualizations are generated
 
----
+## Installation from source
+
 To setup `comex` for development using the source code in your python environment:
 
 ```console
 pip install -r requirements-dev.txt
 ```
-**Note**: Please clone recursively so sub-modules are setup correctly
-```console
-git clone --recursive {...}
-```
 
 This performs an editable install, meaning that comex would be available throughout your environment (particularly relevant if you use conda or something of the sort). This means now you can interact and import from `comex` just like any other package while remaining standalone but also reflecting any code side updates without any other manual steps
 
 ---
 ### Usage as a CLI
 
 This is the recommended way to get started with `comex` as it is the most user friendly
```

### Comparing `comex-0.1.0/src/comex.egg-info/SOURCES.txt` & `comex-0.1.1/src/comex.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -37,8 +37,9 @@
 src/comex/tree_parser/parser_driver.py
 src/comex/utils/DFG_utils.py
 src/comex/utils/__init__.py
 src/comex/utils/cs_nodes.py
 src/comex/utils/java_nodes.py
 src/comex/utils/postprocessor.py
 src/comex/utils/preprocessor.py
-src/comex/utils/src_parser.py
+src/comex/utils/src_parser.py
+tests/test_codeviews.py
```

