# Comparing `tmp/fcapy-0.1.4.2.tar.gz` & `tmp/fcapy-0.1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fcapy-0.1.4.2.tar", last modified: Thu Jun  1 17:20:43 2023, max compression
+gzip compressed data, was "fcapy-0.1.4.3.tar", last modified: Thu Jun  1 17:51:55 2023, max compression
```

## Comparing `fcapy-0.1.4.2.tar` & `fcapy-0.1.4.3.tar`

### file list

```diff
@@ -1,93 +1,112 @@
-drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:20:43.947313 fcapy-0.1.4.2/
--rw-r--r--   0 egordudyrev   (501) staff       (20)    35148 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/LICENSE
--rw-r--r--   0 egordudyrev   (501) staff       (20)    49690 2023-06-01 17:20:43.947103 fcapy-0.1.4.2/PKG-INFO
--rw-r--r--   0 egordudyrev   (501) staff       (20)     8514 2023-05-31 22:55:03.000000 fcapy-0.1.4.2/README.md
-drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:20:43.931414 fcapy-0.1.4.2/fcapy/
--rw-r--r--   0 egordudyrev   (501) staff       (20)     1071 2023-05-31 22:55:03.000000 fcapy-0.1.4.2/fcapy/__init__.py
-drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:20:43.933817 fcapy-0.1.4.2/fcapy/algorithms/
--rw-r--r--   0 egordudyrev   (501) staff       (20)      735 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/fcapy/algorithms/__init__.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)    22047 2023-05-31 22:55:03.000000 fcapy-0.1.4.2/fcapy/algorithms/concept_construction.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)    30947 2023-05-31 22:55:03.000000 fcapy-0.1.4.2/fcapy/algorithms/lattice_construction.py
-drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:20:43.935415 fcapy-0.1.4.2/fcapy/context/
--rw-r--r--   0 egordudyrev   (501) staff       (20)      617 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/fcapy/context/__init__.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)    36139 2023-05-31 22:55:03.000000 fcapy-0.1.4.2/fcapy/context/bintable.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)     1679 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/fcapy/context/bintable_errors.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)     7810 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/fcapy/context/converters.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)    28200 2023-05-31 22:55:03.000000 fcapy-0.1.4.2/fcapy/context/formal_context.py
-drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:20:43.936292 fcapy-0.1.4.2/fcapy/lattice/
--rw-r--r--   0 egordudyrev   (501) staff       (20)      785 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/fcapy/lattice/__init__.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)    37577 2023-06-01 17:20:06.000000 fcapy-0.1.4.2/fcapy/lattice/concept_lattice.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)     2692 2023-06-01 17:20:06.000000 fcapy-0.1.4.2/fcapy/lattice/concept_measures.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)     6723 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/fcapy/lattice/formal_concept.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)    10888 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/fcapy/lattice/pattern_concept.py
-drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:20:43.937224 fcapy-0.1.4.2/fcapy/ml/
--rw-r--r--   0 egordudyrev   (501) staff       (20)      530 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/fcapy/ml/__init__.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)     3851 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/fcapy/ml/decision_based_model.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)    27818 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/fcapy/ml/decision_lattice.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)     6249 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/fcapy/ml/decision_poset_structure.py
-drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:20:43.938022 fcapy-0.1.4.2/fcapy/mvcontext/
--rw-r--r--   0 egordudyrev   (501) staff       (20)      662 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/fcapy/mvcontext/__init__.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)    25294 2023-05-31 22:55:03.000000 fcapy-0.1.4.2/fcapy/mvcontext/mvcontext.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)    21249 2023-05-31 22:55:03.000000 fcapy-0.1.4.2/fcapy/mvcontext/pattern_structure.py
-drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:20:43.938885 fcapy-0.1.4.2/fcapy/poset/
--rw-r--r--   0 egordudyrev   (501) staff       (20)     1100 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/fcapy/poset/__init__.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)     7656 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/fcapy/poset/lattice.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)    35094 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/fcapy/poset/poset.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)     1943 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/fcapy/poset/tree.py
-drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:20:43.939276 fcapy-0.1.4.2/fcapy/utils/
--rw-r--r--   0 egordudyrev   (501) staff       (20)      156 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/fcapy/utils/__init__.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)     2961 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/fcapy/utils/utils.py
-drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:20:43.940426 fcapy-0.1.4.2/fcapy/visualizer/
--rw-r--r--   0 egordudyrev   (501) staff       (20)     1195 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/fcapy/visualizer/__init__.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)     4228 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/fcapy/visualizer/line_layouts.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)    20018 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/fcapy/visualizer/line_visualizers.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)     3023 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/fcapy/visualizer/measures.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)    10768 2023-05-31 22:55:03.000000 fcapy-0.1.4.2/fcapy/visualizer/mover.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)    17702 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/fcapy/visualizer/visualizer.py
-drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:20:43.932742 fcapy-0.1.4.2/fcapy.egg-info/
--rw-r--r--   0 egordudyrev   (501) staff       (20)    49690 2023-06-01 17:20:43.000000 fcapy-0.1.4.2/fcapy.egg-info/PKG-INFO
--rw-r--r--   0 egordudyrev   (501) staff       (20)     2112 2023-06-01 17:20:43.000000 fcapy-0.1.4.2/fcapy.egg-info/SOURCES.txt
--rw-r--r--   0 egordudyrev   (501) staff       (20)        1 2023-06-01 17:20:43.000000 fcapy-0.1.4.2/fcapy.egg-info/dependency_links.txt
--rw-r--r--   0 egordudyrev   (501) staff       (20)      236 2023-06-01 17:20:43.000000 fcapy-0.1.4.2/fcapy.egg-info/requires.txt
--rw-r--r--   0 egordudyrev   (501) staff       (20)        6 2023-06-01 17:20:43.000000 fcapy-0.1.4.2/fcapy.egg-info/top_level.txt
--rw-r--r--   0 egordudyrev   (501) staff       (20)     1115 2023-05-31 22:55:03.000000 fcapy-0.1.4.2/pyproject.toml
--rw-r--r--   0 egordudyrev   (501) staff       (20)       38 2023-06-01 17:20:43.947364 fcapy-0.1.4.2/setup.cfg
-drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:20:43.940690 fcapy-0.1.4.2/tests/
-drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:20:43.941439 fcapy-0.1.4.2/tests/algorithms/
--rw-r--r--   0 egordudyrev   (501) staff       (20)        0 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/tests/algorithms/__init__.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)     6006 2023-05-31 20:34:02.000000 fcapy-0.1.4.2/tests/algorithms/test_concept_construction.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)    14418 2023-05-31 20:34:02.000000 fcapy-0.1.4.2/tests/algorithms/test_lattice_construction.py
-drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:20:43.942596 fcapy-0.1.4.2/tests/context/
--rw-r--r--   0 egordudyrev   (501) staff       (20)        0 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/tests/context/__init__.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)     1861 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/tests/context/data_to_test.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)     7029 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/tests/context/test_bintable.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)     3379 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/tests/context/test_converters.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)    12847 2023-05-31 20:34:02.000000 fcapy-0.1.4.2/tests/context/test_formal_context.py
-drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:20:43.943621 fcapy-0.1.4.2/tests/lattice/
--rw-r--r--   0 egordudyrev   (501) staff       (20)        0 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/tests/lattice/__init__.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)    15404 2023-05-31 20:34:02.000000 fcapy-0.1.4.2/tests/lattice/test_concept_lattice.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)     2028 2023-06-01 17:20:06.000000 fcapy-0.1.4.2/tests/lattice/test_concept_measures.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)     5209 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/tests/lattice/test_formal_concept.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)     2855 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/tests/lattice/test_pattern_concept.py
-drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:20:43.943967 fcapy-0.1.4.2/tests/ml/
--rw-r--r--   0 egordudyrev   (501) staff       (20)        0 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/tests/ml/__init__.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)     6146 2023-05-31 20:34:02.000000 fcapy-0.1.4.2/tests/ml/test_decision_lattice.py
-drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:20:43.944549 fcapy-0.1.4.2/tests/mvcontext/
--rw-r--r--   0 egordudyrev   (501) staff       (20)        0 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/tests/mvcontext/__init__.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)    11993 2023-05-31 20:34:02.000000 fcapy-0.1.4.2/tests/mvcontext/test_mvcontext.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)     7883 2023-05-31 20:34:02.000000 fcapy-0.1.4.2/tests/mvcontext/test_pattern_structure.py
-drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:20:43.945088 fcapy-0.1.4.2/tests/poset/
--rw-r--r--   0 egordudyrev   (501) staff       (20)        0 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/tests/poset/__init__.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)     7045 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/tests/poset/test_lattice.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)    22063 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/tests/poset/test_poset.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)      709 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/tests/test_init.py
-drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:20:43.945507 fcapy-0.1.4.2/tests/utils/
--rw-r--r--   0 egordudyrev   (501) staff       (20)        0 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/tests/utils/__init__.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)     1236 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/tests/utils/test_utils.py
-drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:20:43.946632 fcapy-0.1.4.2/tests/visualizer/
--rw-r--r--   0 egordudyrev   (501) staff       (20)        0 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/tests/visualizer/__init__.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)     4242 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/tests/visualizer/test_line_layouts.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)     5523 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/tests/visualizer/test_line_visualizers.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)      919 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/tests/visualizer/test_measures.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)     2877 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/tests/visualizer/test_mover.py
--rw-r--r--   0 egordudyrev   (501) staff       (20)     1463 2023-05-31 22:55:03.000000 fcapy-0.1.4.2/tests/visualizer/test_visualizer.py
+drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:51:55.909657 fcapy-0.1.4.3/
+-rw-r--r--   0 egordudyrev   (501) staff       (20)    35148 2023-04-11 14:16:21.000000 fcapy-0.1.4.3/LICENSE
+-rw-r--r--   0 egordudyrev   (501) staff       (20)    49690 2023-06-01 17:51:55.909451 fcapy-0.1.4.3/PKG-INFO
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     8514 2023-05-31 22:55:03.000000 fcapy-0.1.4.3/README.md
+drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:51:55.887199 fcapy-0.1.4.3/docs/
+drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:51:55.889859 fcapy-0.1.4.3/docs/source/
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     3321 2023-05-31 22:55:03.000000 fcapy-0.1.4.3/docs/source/conf.py
+drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:51:55.890242 fcapy-0.1.4.3/fcapy/
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     1071 2023-06-01 17:51:00.000000 fcapy-0.1.4.3/fcapy/__init__.py
+drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:51:55.892425 fcapy-0.1.4.3/fcapy/algorithms/
+-rw-r--r--   0 egordudyrev   (501) staff       (20)      735 2023-04-11 14:16:21.000000 fcapy-0.1.4.3/fcapy/algorithms/__init__.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)    22047 2023-05-31 22:55:03.000000 fcapy-0.1.4.3/fcapy/algorithms/concept_construction.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)    30947 2023-05-31 22:55:03.000000 fcapy-0.1.4.3/fcapy/algorithms/lattice_construction.py
+drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:51:55.894095 fcapy-0.1.4.3/fcapy/context/
+-rw-r--r--   0 egordudyrev   (501) staff       (20)      617 2023-04-11 14:16:21.000000 fcapy-0.1.4.3/fcapy/context/__init__.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)    36139 2023-05-31 22:55:03.000000 fcapy-0.1.4.3/fcapy/context/bintable.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     1679 2023-04-11 14:16:21.000000 fcapy-0.1.4.3/fcapy/context/bintable_errors.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     7810 2023-04-11 14:16:21.000000 fcapy-0.1.4.3/fcapy/context/converters.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)    28200 2023-05-31 22:55:03.000000 fcapy-0.1.4.3/fcapy/context/formal_context.py
+drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:51:55.895477 fcapy-0.1.4.3/fcapy/lattice/
+-rw-r--r--   0 egordudyrev   (501) staff       (20)      785 2023-04-11 14:16:21.000000 fcapy-0.1.4.3/fcapy/lattice/__init__.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)    37577 2023-06-01 17:20:06.000000 fcapy-0.1.4.3/fcapy/lattice/concept_lattice.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     2692 2023-06-01 17:20:06.000000 fcapy-0.1.4.3/fcapy/lattice/concept_measures.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     6723 2023-04-11 14:16:21.000000 fcapy-0.1.4.3/fcapy/lattice/formal_concept.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)    10888 2023-04-11 14:16:21.000000 fcapy-0.1.4.3/fcapy/lattice/pattern_concept.py
+drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:51:55.896537 fcapy-0.1.4.3/fcapy/ml/
+-rw-r--r--   0 egordudyrev   (501) staff       (20)      530 2023-04-11 14:16:21.000000 fcapy-0.1.4.3/fcapy/ml/__init__.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     3851 2023-04-11 14:16:21.000000 fcapy-0.1.4.3/fcapy/ml/decision_based_model.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)    27818 2023-04-11 14:16:21.000000 fcapy-0.1.4.3/fcapy/ml/decision_lattice.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     6249 2023-04-11 14:16:21.000000 fcapy-0.1.4.3/fcapy/ml/decision_poset_structure.py
+drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:51:55.897192 fcapy-0.1.4.3/fcapy/mvcontext/
+-rw-r--r--   0 egordudyrev   (501) staff       (20)      662 2023-04-11 14:16:21.000000 fcapy-0.1.4.3/fcapy/mvcontext/__init__.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)    25294 2023-05-31 22:55:03.000000 fcapy-0.1.4.3/fcapy/mvcontext/mvcontext.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)    21249 2023-05-31 22:55:03.000000 fcapy-0.1.4.3/fcapy/mvcontext/pattern_structure.py
+drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:51:55.898030 fcapy-0.1.4.3/fcapy/poset/
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     1100 2023-04-11 14:16:21.000000 fcapy-0.1.4.3/fcapy/poset/__init__.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     7656 2023-04-11 14:16:21.000000 fcapy-0.1.4.3/fcapy/poset/lattice.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)    35094 2023-04-11 14:16:21.000000 fcapy-0.1.4.3/fcapy/poset/poset.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     1943 2023-04-11 14:16:21.000000 fcapy-0.1.4.3/fcapy/poset/tree.py
+drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:51:55.898451 fcapy-0.1.4.3/fcapy/utils/
+-rw-r--r--   0 egordudyrev   (501) staff       (20)      156 2023-04-11 14:16:21.000000 fcapy-0.1.4.3/fcapy/utils/__init__.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     2961 2023-04-11 14:16:21.000000 fcapy-0.1.4.3/fcapy/utils/utils.py
+drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:51:55.899663 fcapy-0.1.4.3/fcapy/visualizer/
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     1195 2023-04-11 14:16:21.000000 fcapy-0.1.4.3/fcapy/visualizer/__init__.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     4228 2023-04-11 14:16:21.000000 fcapy-0.1.4.3/fcapy/visualizer/line_layouts.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)    20018 2023-04-11 14:16:21.000000 fcapy-0.1.4.3/fcapy/visualizer/line_visualizers.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     3023 2023-04-11 14:16:21.000000 fcapy-0.1.4.3/fcapy/visualizer/measures.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)    10768 2023-05-31 22:55:03.000000 fcapy-0.1.4.3/fcapy/visualizer/mover.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)    17702 2023-04-11 14:16:21.000000 fcapy-0.1.4.3/fcapy/visualizer/visualizer.py
+drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:51:55.891397 fcapy-0.1.4.3/fcapy.egg-info/
+-rw-r--r--   0 egordudyrev   (501) staff       (20)    49690 2023-06-01 17:51:55.000000 fcapy-0.1.4.3/fcapy.egg-info/PKG-INFO
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     2445 2023-06-01 17:51:55.000000 fcapy-0.1.4.3/fcapy.egg-info/SOURCES.txt
+-rw-r--r--   0 egordudyrev   (501) staff       (20)        1 2023-06-01 17:51:55.000000 fcapy-0.1.4.3/fcapy.egg-info/dependency_links.txt
+-rw-r--r--   0 egordudyrev   (501) staff       (20)      236 2023-06-01 17:51:55.000000 fcapy-0.1.4.3/fcapy.egg-info/requires.txt
+-rw-r--r--   0 egordudyrev   (501) staff       (20)       38 2023-06-01 17:51:55.000000 fcapy-0.1.4.3/fcapy.egg-info/top_level.txt
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     1206 2023-06-01 17:51:00.000000 fcapy-0.1.4.3/pyproject.toml
+-rw-r--r--   0 egordudyrev   (501) staff       (20)       38 2023-06-01 17:51:55.909712 fcapy-0.1.4.3/setup.cfg
+drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:51:55.900038 fcapy-0.1.4.3/tests/
+-rw-r--r--   0 egordudyrev   (501) staff       (20)        0 2023-04-11 14:16:21.000000 fcapy-0.1.4.3/tests/__init__.py
+drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:51:55.900672 fcapy-0.1.4.3/tests/algorithms/
+-rw-r--r--   0 egordudyrev   (501) staff       (20)        0 2023-04-11 14:16:21.000000 fcapy-0.1.4.3/tests/algorithms/__init__.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     6006 2023-05-31 20:34:02.000000 fcapy-0.1.4.3/tests/algorithms/test_concept_construction.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)    14418 2023-05-31 20:34:02.000000 fcapy-0.1.4.3/tests/algorithms/test_lattice_construction.py
+drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:51:55.902008 fcapy-0.1.4.3/tests/context/
+-rw-r--r--   0 egordudyrev   (501) staff       (20)        0 2023-04-11 14:16:21.000000 fcapy-0.1.4.3/tests/context/__init__.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     1861 2023-04-11 14:16:21.000000 fcapy-0.1.4.3/tests/context/data_to_test.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     7029 2023-04-11 14:16:21.000000 fcapy-0.1.4.3/tests/context/test_bintable.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     3379 2023-04-11 14:16:21.000000 fcapy-0.1.4.3/tests/context/test_converters.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)    12847 2023-05-31 20:34:02.000000 fcapy-0.1.4.3/tests/context/test_formal_context.py
+drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:51:55.902920 fcapy-0.1.4.3/tests/lattice/
+-rw-r--r--   0 egordudyrev   (501) staff       (20)        0 2023-04-11 14:16:21.000000 fcapy-0.1.4.3/tests/lattice/__init__.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)    15404 2023-05-31 20:34:02.000000 fcapy-0.1.4.3/tests/lattice/test_concept_lattice.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     2028 2023-06-01 17:20:06.000000 fcapy-0.1.4.3/tests/lattice/test_concept_measures.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     5209 2023-04-11 14:16:21.000000 fcapy-0.1.4.3/tests/lattice/test_formal_concept.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     2855 2023-04-11 14:16:21.000000 fcapy-0.1.4.3/tests/lattice/test_pattern_concept.py
+drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:51:55.903216 fcapy-0.1.4.3/tests/ml/
+-rw-r--r--   0 egordudyrev   (501) staff       (20)        0 2023-04-11 14:16:21.000000 fcapy-0.1.4.3/tests/ml/__init__.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     6146 2023-05-31 20:34:02.000000 fcapy-0.1.4.3/tests/ml/test_decision_lattice.py
+drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:51:55.903737 fcapy-0.1.4.3/tests/mvcontext/
+-rw-r--r--   0 egordudyrev   (501) staff       (20)        0 2023-04-11 14:16:21.000000 fcapy-0.1.4.3/tests/mvcontext/__init__.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)    11993 2023-05-31 20:34:02.000000 fcapy-0.1.4.3/tests/mvcontext/test_mvcontext.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     7883 2023-05-31 20:34:02.000000 fcapy-0.1.4.3/tests/mvcontext/test_pattern_structure.py
+drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:51:55.904229 fcapy-0.1.4.3/tests/poset/
+-rw-r--r--   0 egordudyrev   (501) staff       (20)        0 2023-04-11 14:16:21.000000 fcapy-0.1.4.3/tests/poset/__init__.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     7045 2023-04-11 14:16:21.000000 fcapy-0.1.4.3/tests/poset/test_lattice.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)    22063 2023-04-11 14:16:21.000000 fcapy-0.1.4.3/tests/poset/test_poset.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)      709 2023-04-11 14:16:21.000000 fcapy-0.1.4.3/tests/test_init.py
+drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:51:55.904637 fcapy-0.1.4.3/tests/utils/
+-rw-r--r--   0 egordudyrev   (501) staff       (20)        0 2023-04-11 14:16:21.000000 fcapy-0.1.4.3/tests/utils/__init__.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     1236 2023-04-11 14:16:21.000000 fcapy-0.1.4.3/tests/utils/test_utils.py
+drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:51:55.905665 fcapy-0.1.4.3/tests/visualizer/
+-rw-r--r--   0 egordudyrev   (501) staff       (20)        0 2023-04-11 14:16:21.000000 fcapy-0.1.4.3/tests/visualizer/__init__.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     4242 2023-04-11 14:16:21.000000 fcapy-0.1.4.3/tests/visualizer/test_line_layouts.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     5523 2023-04-11 14:16:21.000000 fcapy-0.1.4.3/tests/visualizer/test_line_visualizers.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)      919 2023-04-11 14:16:21.000000 fcapy-0.1.4.3/tests/visualizer/test_measures.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     2877 2023-04-11 14:16:21.000000 fcapy-0.1.4.3/tests/visualizer/test_mover.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     1463 2023-05-31 22:55:03.000000 fcapy-0.1.4.3/tests/visualizer/test_visualizer.py
+drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:51:55.889166 fcapy-0.1.4.3/venv/
+drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:51:55.909063 fcapy-0.1.4.3/venv/bin/
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     1176 2023-05-14 11:47:04.000000 fcapy-0.1.4.3/venv/bin/activate_this.py
+-rwxr-xr-x   0 egordudyrev   (501) staff       (20)      628 2023-05-14 12:16:07.000000 fcapy-0.1.4.3/venv/bin/rst2html.py
+-rwxr-xr-x   0 egordudyrev   (501) staff       (20)      748 2023-05-14 12:16:07.000000 fcapy-0.1.4.3/venv/bin/rst2html4.py
+-rwxr-xr-x   0 egordudyrev   (501) staff       (20)     1116 2023-05-14 12:16:07.000000 fcapy-0.1.4.3/venv/bin/rst2html5.py
+-rwxr-xr-x   0 egordudyrev   (501) staff       (20)      825 2023-05-14 12:16:07.000000 fcapy-0.1.4.3/venv/bin/rst2latex.py
+-rwxr-xr-x   0 egordudyrev   (501) staff       (20)      633 2023-05-14 12:16:07.000000 fcapy-0.1.4.3/venv/bin/rst2man.py
+-rwxr-xr-x   0 egordudyrev   (501) staff       (20)      798 2023-05-14 12:16:07.000000 fcapy-0.1.4.3/venv/bin/rst2odt.py
+-rwxr-xr-x   0 egordudyrev   (501) staff       (20)     1760 2023-05-14 12:16:07.000000 fcapy-0.1.4.3/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 egordudyrev   (501) staff       (20)      635 2023-05-14 12:16:07.000000 fcapy-0.1.4.3/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 egordudyrev   (501) staff       (20)      671 2023-05-14 12:16:07.000000 fcapy-0.1.4.3/venv/bin/rst2s5.py
+-rwxr-xr-x   0 egordudyrev   (501) staff       (20)      905 2023-05-14 12:16:07.000000 fcapy-0.1.4.3/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 egordudyrev   (501) staff       (20)      636 2023-05-14 12:16:07.000000 fcapy-0.1.4.3/venv/bin/rst2xml.py
+-rwxr-xr-x   0 egordudyrev   (501) staff       (20)      704 2023-05-14 12:16:07.000000 fcapy-0.1.4.3/venv/bin/rstpep2html.py
```

### Comparing `fcapy-0.1.4.2/LICENSE` & `fcapy-0.1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/PKG-INFO` & `fcapy-0.1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fcapy
-Version: 0.1.4.2
+Version: 0.1.4.3
 Summary: A library to work with formal (and pattern) contexts, concepts, lattices
 Author: Egor Dudyrev
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `fcapy-0.1.4.2/README.md` & `fcapy-0.1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/fcapy/__init__.py` & `fcapy-0.1.4.3/fcapy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,8 +20,8 @@
     'bitsets': "The package greatly optimizes BinTables execution",
     'bitarray': "The package greatly optimizes BinTables execution",
     'networkx': "The package to convert POSets to Graphs and to visualize them as graphs",
 }
 LIB_INSTALLED = check_installed_packages(PACKAGE_DESCRIPTION)
 
 
-__version__ = '0.1.4.2'
+__version__ = '0.1.4.3'
```

### Comparing `fcapy-0.1.4.2/fcapy/algorithms/__init__.py` & `fcapy-0.1.4.3/fcapy/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/fcapy/algorithms/concept_construction.py` & `fcapy-0.1.4.3/fcapy/algorithms/concept_construction.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/fcapy/algorithms/lattice_construction.py` & `fcapy-0.1.4.3/fcapy/algorithms/lattice_construction.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/fcapy/context/__init__.py` & `fcapy-0.1.4.3/fcapy/context/__init__.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/fcapy/context/bintable.py` & `fcapy-0.1.4.3/fcapy/context/bintable.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/fcapy/context/bintable_errors.py` & `fcapy-0.1.4.3/fcapy/context/bintable_errors.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/fcapy/context/converters.py` & `fcapy-0.1.4.3/fcapy/context/converters.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/fcapy/context/formal_context.py` & `fcapy-0.1.4.3/fcapy/context/formal_context.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/fcapy/lattice/__init__.py` & `fcapy-0.1.4.3/fcapy/lattice/__init__.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/fcapy/lattice/concept_lattice.py` & `fcapy-0.1.4.3/fcapy/lattice/concept_lattice.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/fcapy/lattice/concept_measures.py` & `fcapy-0.1.4.3/fcapy/lattice/concept_measures.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/fcapy/lattice/formal_concept.py` & `fcapy-0.1.4.3/fcapy/lattice/formal_concept.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/fcapy/lattice/pattern_concept.py` & `fcapy-0.1.4.3/fcapy/lattice/pattern_concept.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/fcapy/ml/__init__.py` & `fcapy-0.1.4.3/fcapy/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/fcapy/ml/decision_based_model.py` & `fcapy-0.1.4.3/fcapy/ml/decision_based_model.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/fcapy/ml/decision_lattice.py` & `fcapy-0.1.4.3/fcapy/ml/decision_lattice.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/fcapy/ml/decision_poset_structure.py` & `fcapy-0.1.4.3/fcapy/ml/decision_poset_structure.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/fcapy/mvcontext/__init__.py` & `fcapy-0.1.4.3/fcapy/mvcontext/__init__.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/fcapy/mvcontext/mvcontext.py` & `fcapy-0.1.4.3/fcapy/mvcontext/mvcontext.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/fcapy/mvcontext/pattern_structure.py` & `fcapy-0.1.4.3/fcapy/mvcontext/pattern_structure.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/fcapy/poset/__init__.py` & `fcapy-0.1.4.3/fcapy/poset/__init__.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/fcapy/poset/lattice.py` & `fcapy-0.1.4.3/fcapy/poset/lattice.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/fcapy/poset/poset.py` & `fcapy-0.1.4.3/fcapy/poset/poset.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/fcapy/poset/tree.py` & `fcapy-0.1.4.3/fcapy/poset/tree.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/fcapy/utils/utils.py` & `fcapy-0.1.4.3/fcapy/utils/utils.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/fcapy/visualizer/__init__.py` & `fcapy-0.1.4.3/fcapy/visualizer/__init__.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/fcapy/visualizer/line_layouts.py` & `fcapy-0.1.4.3/fcapy/visualizer/line_layouts.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/fcapy/visualizer/line_visualizers.py` & `fcapy-0.1.4.3/fcapy/visualizer/line_visualizers.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/fcapy/visualizer/measures.py` & `fcapy-0.1.4.3/fcapy/visualizer/measures.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/fcapy/visualizer/mover.py` & `fcapy-0.1.4.3/fcapy/visualizer/mover.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/fcapy/visualizer/visualizer.py` & `fcapy-0.1.4.3/fcapy/visualizer/visualizer.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/fcapy.egg-info/PKG-INFO` & `fcapy-0.1.4.3/fcapy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fcapy
-Version: 0.1.4.2
+Version: 0.1.4.3
 Summary: A library to work with formal (and pattern) contexts, concepts, lattices
 Author: Egor Dudyrev
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `fcapy-0.1.4.2/fcapy.egg-info/SOURCES.txt` & `fcapy-0.1.4.3/fcapy.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 README.md
 pyproject.toml
+docs/source/conf.py
 fcapy/__init__.py
 fcapy.egg-info/PKG-INFO
 fcapy.egg-info/SOURCES.txt
 fcapy.egg-info/dependency_links.txt
 fcapy.egg-info/requires.txt
 fcapy.egg-info/top_level.txt
 fcapy/algorithms/__init__.py
@@ -35,14 +36,15 @@
 fcapy/utils/utils.py
 fcapy/visualizer/__init__.py
 fcapy/visualizer/line_layouts.py
 fcapy/visualizer/line_visualizers.py
 fcapy/visualizer/measures.py
 fcapy/visualizer/mover.py
 fcapy/visualizer/visualizer.py
+tests/__init__.py
 tests/test_init.py
 tests/algorithms/__init__.py
 tests/algorithms/test_concept_construction.py
 tests/algorithms/test_lattice_construction.py
 tests/context/__init__.py
 tests/context/data_to_test.py
 tests/context/test_bintable.py
@@ -64,8 +66,21 @@
 tests/utils/__init__.py
 tests/utils/test_utils.py
 tests/visualizer/__init__.py
 tests/visualizer/test_line_layouts.py
 tests/visualizer/test_line_visualizers.py
 tests/visualizer/test_measures.py
 tests/visualizer/test_mover.py
-tests/visualizer/test_visualizer.py
+tests/visualizer/test_visualizer.py
+venv/bin/activate_this.py
+venv/bin/rst2html.py
+venv/bin/rst2html4.py
+venv/bin/rst2html5.py
+venv/bin/rst2latex.py
+venv/bin/rst2man.py
+venv/bin/rst2odt.py
+venv/bin/rst2odt_prepstyles.py
+venv/bin/rst2pseudoxml.py
+venv/bin/rst2s5.py
+venv/bin/rst2xetex.py
+venv/bin/rst2xml.py
+venv/bin/rstpep2html.py
```

### Comparing `fcapy-0.1.4.2/pyproject.toml` & `fcapy-0.1.4.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fcapy"
-version = "0.1.4.2"
+version = "0.1.4.3"
 description = "A library to work with formal (and pattern) contexts, concepts, lattices"
 readme = "README.md"
 authors = [{ name = "Egor Dudyrev" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
@@ -30,8 +30,11 @@
 ml = ["xgboost"]
 visualizer = ["plotly"]
 
 [project.urls]
 Homepage = "https://github.com/EgorDudyrev/FCApy"
 
 [tool.setuptools]
-py-modules = ["fcapy"]
+py-modules = ["fcapy"]
+
+[tool.setuptools.packages]
+find = {}  # Scanning implicit namespaces is active by default
```

### Comparing `fcapy-0.1.4.2/tests/algorithms/test_concept_construction.py` & `fcapy-0.1.4.3/tests/algorithms/test_concept_construction.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/tests/algorithms/test_lattice_construction.py` & `fcapy-0.1.4.3/tests/algorithms/test_lattice_construction.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/tests/context/data_to_test.py` & `fcapy-0.1.4.3/tests/context/data_to_test.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/tests/context/test_bintable.py` & `fcapy-0.1.4.3/tests/context/test_bintable.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/tests/context/test_converters.py` & `fcapy-0.1.4.3/tests/context/test_converters.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/tests/context/test_formal_context.py` & `fcapy-0.1.4.3/tests/context/test_formal_context.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/tests/lattice/test_concept_lattice.py` & `fcapy-0.1.4.3/tests/lattice/test_concept_lattice.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/tests/lattice/test_concept_measures.py` & `fcapy-0.1.4.3/tests/lattice/test_concept_measures.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/tests/lattice/test_formal_concept.py` & `fcapy-0.1.4.3/tests/lattice/test_formal_concept.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/tests/lattice/test_pattern_concept.py` & `fcapy-0.1.4.3/tests/lattice/test_pattern_concept.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/tests/ml/test_decision_lattice.py` & `fcapy-0.1.4.3/tests/ml/test_decision_lattice.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/tests/mvcontext/test_mvcontext.py` & `fcapy-0.1.4.3/tests/mvcontext/test_mvcontext.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/tests/mvcontext/test_pattern_structure.py` & `fcapy-0.1.4.3/tests/mvcontext/test_pattern_structure.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/tests/poset/test_lattice.py` & `fcapy-0.1.4.3/tests/poset/test_lattice.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/tests/poset/test_poset.py` & `fcapy-0.1.4.3/tests/poset/test_poset.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/tests/test_init.py` & `fcapy-0.1.4.3/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/tests/utils/test_utils.py` & `fcapy-0.1.4.3/tests/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/tests/visualizer/test_line_layouts.py` & `fcapy-0.1.4.3/tests/visualizer/test_line_layouts.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/tests/visualizer/test_line_visualizers.py` & `fcapy-0.1.4.3/tests/visualizer/test_line_visualizers.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/tests/visualizer/test_measures.py` & `fcapy-0.1.4.3/tests/visualizer/test_measures.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/tests/visualizer/test_mover.py` & `fcapy-0.1.4.3/tests/visualizer/test_mover.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.2/tests/visualizer/test_visualizer.py` & `fcapy-0.1.4.3/tests/visualizer/test_visualizer.py`

 * *Files identical despite different names*

