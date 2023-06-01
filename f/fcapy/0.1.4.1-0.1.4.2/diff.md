# Comparing `tmp/fcapy-0.1.4.1.tar.gz` & `tmp/fcapy-0.1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fcapy-0.1.4.1.tar", last modified: Sat Dec  3 15:37:52 2022, max compression
+gzip compressed data, was "fcapy-0.1.4.2.tar", last modified: Thu Jun  1 17:20:43 2023, max compression
```

## Comparing `fcapy-0.1.4.1.tar` & `fcapy-0.1.4.2.tar`

### file list

```diff
@@ -1,132 +1,93 @@
-drwxrwxr-x   0 egor      (1000) egor      (1000)        0 2022-12-03 15:37:52.070840 fcapy-0.1.4.1/
--rw-rw-r--   0 egor      (1000) egor      (1000)      101 2022-09-08 13:32:19.000000 fcapy-0.1.4.1/.coveragerc
--rw-rw-r--   0 egor      (1000) egor      (1000)      102 2021-04-14 13:31:23.000000 fcapy-0.1.4.1/.gitignore
--rw-rw-r--   0 egor      (1000) egor      (1000)      625 2022-12-03 15:35:09.000000 fcapy-0.1.4.1/.readthedocs.yml
--rw-rw-r--   0 egor      (1000) egor      (1000)      262 2020-12-04 10:31:42.000000 fcapy-0.1.4.1/.travis.yml
--rw-rw-r--   0 egor      (1000) egor      (1000)     2913 2022-12-03 15:35:09.000000 fcapy-0.1.4.1/CHANGELOG.md
--rw-rw-r--   0 egor      (1000) egor      (1000)      110 2021-08-12 16:45:25.000000 fcapy-0.1.4.1/CONTRIBUTING.md
--rw-rw-r--   0 egor      (1000) egor      (1000)    35148 2020-11-19 20:34:33.000000 fcapy-0.1.4.1/LICENSE
--rw-rw-r--   0 egor      (1000) egor      (1000)      111 2021-04-27 12:04:20.000000 fcapy-0.1.4.1/Makefile
--rw-rw-r--   0 egor      (1000) egor      (1000)     9128 2022-12-03 15:37:52.070840 fcapy-0.1.4.1/PKG-INFO
--rw-rw-r--   0 egor      (1000) egor      (1000)     8349 2022-09-18 22:19:19.000000 fcapy-0.1.4.1/README.md
--rw-rw-r--   0 egor      (1000) egor      (1000)      590 2020-12-04 10:31:42.000000 fcapy-0.1.4.1/codecov.yml
-drwxrwxr-x   0 egor      (1000) egor      (1000)        0 2022-12-03 15:37:52.066840 fcapy-0.1.4.1/data/
--rw-rw-r--   0 egor      (1000) egor      (1000)      458 2020-12-04 10:31:42.000000 fcapy-0.1.4.1/data/animal_movement.csv
--rw-rw-r--   0 egor      (1000) egor      (1000)      186 2020-12-04 10:31:42.000000 fcapy-0.1.4.1/data/animal_movement.cxt
--rw-rw-r--   0 egor      (1000) egor      (1000)      708 2020-12-04 10:31:42.000000 fcapy-0.1.4.1/data/animal_movement.json
--rw-rw-r--   0 egor      (1000) egor      (1000)     1481 2020-12-10 14:35:38.000000 fcapy-0.1.4.1/data/animal_movement_concepts.json
--rw-rw-r--   0 egor      (1000) egor      (1000)     1709 2020-12-18 21:50:13.000000 fcapy-0.1.4.1/data/animal_movement_lattice.json
--rw-rw-r--   0 egor      (1000) egor      (1000)   133974 2022-12-02 21:59:41.000000 fcapy-0.1.4.1/data/animal_movement_lattice.png
--rw-rw-r--   0 egor      (1000) egor      (1000)   143462 2022-12-02 21:59:41.000000 fcapy-0.1.4.1/data/animal_movement_lattice_overloaded.png
--rw-rw-r--   0 egor      (1000) egor      (1000)      123 2020-12-04 10:31:42.000000 fcapy-0.1.4.1/data/digits.cxt
--rw-rw-r--   0 egor      (1000) egor      (1000)     3867 2022-10-16 11:58:43.000000 fcapy-0.1.4.1/data/digits_sofia_lattice_22.json
--rw-rw-r--   0 egor      (1000) egor      (1000)      165 2020-12-04 10:31:42.000000 fcapy-0.1.4.1/data/gewaesser.cxt
--rw-rw-r--   0 egor      (1000) egor      (1000)      439 2020-12-04 10:31:42.000000 fcapy-0.1.4.1/data/iris_binarized.csv
--rw-rw-r--   0 egor      (1000) egor      (1000)      514 2020-12-04 10:31:42.000000 fcapy-0.1.4.1/data/lattice.cxt
--rw-rw-r--   0 egor      (1000) egor      (1000)      266 2020-12-04 10:31:42.000000 fcapy-0.1.4.1/data/liveinwater.cxt
--rw-rw-r--   0 egor      (1000) egor      (1000)      317 2020-12-17 18:28:11.000000 fcapy-0.1.4.1/data/mango.csv
--rw-rw-r--   0 egor      (1000) egor      (1000)      635 2021-02-07 11:24:14.000000 fcapy-0.1.4.1/data/mango_bin.csv
--rw-rw-r--   0 egor      (1000) egor      (1000)      438 2020-12-04 10:31:42.000000 fcapy-0.1.4.1/data/tealady.cxt
-drwxrwxr-x   0 egor      (1000) egor      (1000)        0 2022-12-03 15:37:52.066840 fcapy-0.1.4.1/docs/
--rw-rw-r--   0 egor      (1000) egor      (1000)      638 2020-12-04 10:31:42.000000 fcapy-0.1.4.1/docs/Makefile
-drwxrwxr-x   0 egor      (1000) egor      (1000)        0 2022-12-03 15:37:52.066840 fcapy-0.1.4.1/docs/images/
--rw-rw-r--   0 egor      (1000) egor      (1000)    28054 2022-05-17 14:56:19.000000 fcapy-0.1.4.1/docs/images/animal_context_lattice.png
--rw-rw-r--   0 egor      (1000) egor      (1000)   444841 2022-07-04 14:07:15.000000 fcapy-0.1.4.1/docs/images/live_in_water_representation_comparison.png
--rw-rw-r--   0 egor      (1000) egor      (1000)      799 2020-12-04 10:31:42.000000 fcapy-0.1.4.1/docs/make.bat
-drwxrwxr-x   0 egor      (1000) egor      (1000)        0 2022-12-03 15:37:52.070840 fcapy-0.1.4.1/docs/source/
--rw-rw-r--   0 egor      (1000) egor      (1000)     1159 2022-12-03 15:35:09.000000 fcapy-0.1.4.1/docs/source/api.rst
--rw-rw-r--   0 egor      (1000) egor      (1000)     3321 2022-12-03 15:35:09.000000 fcapy-0.1.4.1/docs/source/conf.py
--rw-rw-r--   0 egor      (1000) egor      (1000)      115 2021-09-24 14:50:11.000000 fcapy-0.1.4.1/docs/source/examples.rst
--rw-rw-r--   0 egor      (1000) egor      (1000)      643 2022-07-04 15:22:02.000000 fcapy-0.1.4.1/docs/source/index.rst
-drwxrwxr-x   0 egor      (1000) egor      (1000)        0 2022-12-03 15:37:52.070840 fcapy-0.1.4.1/fcapy/
--rw-rw-r--   0 egor      (1000) egor      (1000)     1045 2022-09-18 22:19:19.000000 fcapy-0.1.4.1/fcapy/__init__.py
-drwxrwxr-x   0 egor      (1000) egor      (1000)        0 2022-12-03 15:37:52.070840 fcapy-0.1.4.1/fcapy/algorithms/
--rw-rw-r--   0 egor      (1000) egor      (1000)      735 2022-09-08 13:32:19.000000 fcapy-0.1.4.1/fcapy/algorithms/__init__.py
--rw-rw-r--   0 egor      (1000) egor      (1000)    21850 2022-10-16 11:58:43.000000 fcapy-0.1.4.1/fcapy/algorithms/concept_construction.py
--rw-rw-r--   0 egor      (1000) egor      (1000)    29660 2022-09-08 13:32:19.000000 fcapy-0.1.4.1/fcapy/algorithms/lattice_construction.py
-drwxrwxr-x   0 egor      (1000) egor      (1000)        0 2022-12-03 15:37:52.070840 fcapy-0.1.4.1/fcapy/context/
--rw-rw-r--   0 egor      (1000) egor      (1000)      617 2022-09-18 22:19:19.000000 fcapy-0.1.4.1/fcapy/context/__init__.py
--rw-rw-r--   0 egor      (1000) egor      (1000)    36161 2022-12-03 14:33:04.000000 fcapy-0.1.4.1/fcapy/context/bintable.py
--rw-rw-r--   0 egor      (1000) egor      (1000)     1679 2022-12-02 21:59:41.000000 fcapy-0.1.4.1/fcapy/context/bintable_errors.py
--rw-rw-r--   0 egor      (1000) egor      (1000)     7810 2021-03-28 21:05:36.000000 fcapy-0.1.4.1/fcapy/context/converters.py
--rw-rw-r--   0 egor      (1000) egor      (1000)    27872 2022-12-02 21:59:41.000000 fcapy-0.1.4.1/fcapy/context/formal_context.py
-drwxrwxr-x   0 egor      (1000) egor      (1000)        0 2022-12-03 15:37:52.070840 fcapy-0.1.4.1/fcapy/lattice/
--rw-rw-r--   0 egor      (1000) egor      (1000)      785 2022-09-07 14:07:45.000000 fcapy-0.1.4.1/fcapy/lattice/__init__.py
--rw-rw-r--   0 egor      (1000) egor      (1000)    37202 2022-10-16 11:58:43.000000 fcapy-0.1.4.1/fcapy/lattice/concept_lattice.py
--rw-rw-r--   0 egor      (1000) egor      (1000)     2295 2022-10-16 11:58:43.000000 fcapy-0.1.4.1/fcapy/lattice/concept_measures.py
--rw-rw-r--   0 egor      (1000) egor      (1000)     6723 2022-10-16 11:58:43.000000 fcapy-0.1.4.1/fcapy/lattice/formal_concept.py
--rw-rw-r--   0 egor      (1000) egor      (1000)    10888 2022-09-10 12:12:23.000000 fcapy-0.1.4.1/fcapy/lattice/pattern_concept.py
-drwxrwxr-x   0 egor      (1000) egor      (1000)        0 2022-12-03 15:37:52.070840 fcapy-0.1.4.1/fcapy/ml/
--rw-rw-r--   0 egor      (1000) egor      (1000)      530 2022-09-07 14:19:42.000000 fcapy-0.1.4.1/fcapy/ml/__init__.py
--rw-rw-r--   0 egor      (1000) egor      (1000)     3851 2021-09-09 16:16:29.000000 fcapy-0.1.4.1/fcapy/ml/decision_based_model.py
--rw-rw-r--   0 egor      (1000) egor      (1000)    27818 2022-09-15 12:41:24.000000 fcapy-0.1.4.1/fcapy/ml/decision_lattice.py
--rw-rw-r--   0 egor      (1000) egor      (1000)     6249 2022-09-08 13:32:19.000000 fcapy-0.1.4.1/fcapy/ml/decision_poset_structure.py
-drwxrwxr-x   0 egor      (1000) egor      (1000)        0 2022-12-03 15:37:52.070840 fcapy-0.1.4.1/fcapy/mvcontext/
--rw-rw-r--   0 egor      (1000) egor      (1000)      662 2021-03-25 10:29:49.000000 fcapy-0.1.4.1/fcapy/mvcontext/__init__.py
--rw-rw-r--   0 egor      (1000) egor      (1000)    24158 2022-09-18 15:46:41.000000 fcapy-0.1.4.1/fcapy/mvcontext/mvcontext.py
--rw-rw-r--   0 egor      (1000) egor      (1000)    12658 2021-08-06 16:31:28.000000 fcapy-0.1.4.1/fcapy/mvcontext/pattern_structure.py
-drwxrwxr-x   0 egor      (1000) egor      (1000)        0 2022-12-03 15:37:52.070840 fcapy-0.1.4.1/fcapy/poset/
--rw-rw-r--   0 egor      (1000) egor      (1000)     1100 2022-09-07 14:11:59.000000 fcapy-0.1.4.1/fcapy/poset/__init__.py
--rw-rw-r--   0 egor      (1000) egor      (1000)     7656 2022-10-16 11:58:43.000000 fcapy-0.1.4.1/fcapy/poset/lattice.py
--rw-rw-r--   0 egor      (1000) egor      (1000)    35094 2022-10-16 11:58:43.000000 fcapy-0.1.4.1/fcapy/poset/poset.py
--rw-rw-r--   0 egor      (1000) egor      (1000)     1943 2022-10-16 11:58:43.000000 fcapy-0.1.4.1/fcapy/poset/tree.py
-drwxrwxr-x   0 egor      (1000) egor      (1000)        0 2022-12-03 15:37:52.070840 fcapy-0.1.4.1/fcapy/utils/
--rw-rw-r--   0 egor      (1000) egor      (1000)      156 2021-03-25 10:29:49.000000 fcapy-0.1.4.1/fcapy/utils/__init__.py
--rw-rw-r--   0 egor      (1000) egor      (1000)     2961 2022-09-12 15:15:25.000000 fcapy-0.1.4.1/fcapy/utils/utils.py
-drwxrwxr-x   0 egor      (1000) egor      (1000)        0 2022-12-03 15:37:52.070840 fcapy-0.1.4.1/fcapy/visualizer/
--rw-rw-r--   0 egor      (1000) egor      (1000)     1195 2022-09-15 12:41:40.000000 fcapy-0.1.4.1/fcapy/visualizer/__init__.py
--rw-rw-r--   0 egor      (1000) egor      (1000)     4228 2022-09-08 13:32:19.000000 fcapy-0.1.4.1/fcapy/visualizer/line_layouts.py
--rw-rw-r--   0 egor      (1000) egor      (1000)    20018 2022-10-16 11:58:43.000000 fcapy-0.1.4.1/fcapy/visualizer/line_visualizers.py
--rw-rw-r--   0 egor      (1000) egor      (1000)     3023 2022-09-08 13:32:19.000000 fcapy-0.1.4.1/fcapy/visualizer/measures.py
--rw-rw-r--   0 egor      (1000) egor      (1000)    10761 2022-07-04 17:33:05.000000 fcapy-0.1.4.1/fcapy/visualizer/mover.py
--rw-rw-r--   0 egor      (1000) egor      (1000)    17702 2022-09-08 13:32:19.000000 fcapy-0.1.4.1/fcapy/visualizer/visualizer.py
-drwxrwxr-x   0 egor      (1000) egor      (1000)        0 2022-12-03 15:37:52.070840 fcapy-0.1.4.1/fcapy.egg-info/
--rw-rw-r--   0 egor      (1000) egor      (1000)     9128 2022-12-03 15:37:52.000000 fcapy-0.1.4.1/fcapy.egg-info/PKG-INFO
--rw-rw-r--   0 egor      (1000) egor      (1000)     2875 2022-12-03 15:37:52.000000 fcapy-0.1.4.1/fcapy.egg-info/SOURCES.txt
--rw-rw-r--   0 egor      (1000) egor      (1000)        1 2022-12-03 15:37:52.000000 fcapy-0.1.4.1/fcapy.egg-info/dependency_links.txt
--rw-rw-r--   0 egor      (1000) egor      (1000)      653 2022-12-03 15:37:52.000000 fcapy-0.1.4.1/fcapy.egg-info/requires.txt
--rw-rw-r--   0 egor      (1000) egor      (1000)       12 2022-12-03 15:37:52.000000 fcapy-0.1.4.1/fcapy.egg-info/top_level.txt
--rw-rw-r--   0 egor      (1000) egor      (1000)       94 2021-01-12 17:03:44.000000 fcapy-0.1.4.1/pytest.ini
--rw-rw-r--   0 egor      (1000) egor      (1000)       38 2022-12-03 15:37:52.070840 fcapy-0.1.4.1/setup.cfg
--rw-rw-r--   0 egor      (1000) egor      (1000)     2024 2022-12-03 15:35:09.000000 fcapy-0.1.4.1/setup.py
-drwxrwxr-x   0 egor      (1000) egor      (1000)        0 2022-12-03 15:37:52.070840 fcapy-0.1.4.1/tests/
--rw-rw-r--   0 egor      (1000) egor      (1000)        0 2020-12-08 19:04:08.000000 fcapy-0.1.4.1/tests/__init__.py
-drwxrwxr-x   0 egor      (1000) egor      (1000)        0 2022-12-03 15:37:52.070840 fcapy-0.1.4.1/tests/algorithms/
--rw-rw-r--   0 egor      (1000) egor      (1000)        0 2020-12-14 17:46:29.000000 fcapy-0.1.4.1/tests/algorithms/__init__.py
--rw-rw-r--   0 egor      (1000) egor      (1000)     9116 2022-10-16 11:58:43.000000 fcapy-0.1.4.1/tests/algorithms/test_concept_construction.py
--rw-rw-r--   0 egor      (1000) egor      (1000)    14174 2022-09-08 13:32:19.000000 fcapy-0.1.4.1/tests/algorithms/test_lattice_construction.py
-drwxrwxr-x   0 egor      (1000) egor      (1000)        0 2022-12-03 15:37:52.070840 fcapy-0.1.4.1/tests/context/
--rw-rw-r--   0 egor      (1000) egor      (1000)    53248 2020-12-04 10:31:42.000000 fcapy-0.1.4.1/tests/context/.coverage
--rw-rw-r--   0 egor      (1000) egor      (1000)        0 2020-12-08 18:52:44.000000 fcapy-0.1.4.1/tests/context/__init__.py
--rw-rw-r--   0 egor      (1000) egor      (1000)     1861 2021-03-28 21:05:36.000000 fcapy-0.1.4.1/tests/context/data_to_test.py
--rw-rw-r--   0 egor      (1000) egor      (1000)     7029 2022-09-18 22:19:19.000000 fcapy-0.1.4.1/tests/context/test_bintable.py
--rw-rw-r--   0 egor      (1000) egor      (1000)     3379 2021-03-28 21:05:36.000000 fcapy-0.1.4.1/tests/context/test_converters.py
--rw-rw-r--   0 egor      (1000) egor      (1000)    12495 2022-10-16 11:58:43.000000 fcapy-0.1.4.1/tests/context/test_formal_context.py
-drwxrwxr-x   0 egor      (1000) egor      (1000)        0 2022-12-03 15:37:52.070840 fcapy-0.1.4.1/tests/lattice/
--rw-rw-r--   0 egor      (1000) egor      (1000)        0 2020-12-08 19:19:47.000000 fcapy-0.1.4.1/tests/lattice/__init__.py
--rw-rw-r--   0 egor      (1000) egor      (1000)    14850 2022-12-02 21:59:41.000000 fcapy-0.1.4.1/tests/lattice/test_concept_lattice.py
--rw-rw-r--   0 egor      (1000) egor      (1000)     1366 2022-09-08 13:32:19.000000 fcapy-0.1.4.1/tests/lattice/test_concept_measures.py
--rw-rw-r--   0 egor      (1000) egor      (1000)     5209 2022-10-16 11:58:43.000000 fcapy-0.1.4.1/tests/lattice/test_formal_concept.py
--rw-rw-r--   0 egor      (1000) egor      (1000)     2855 2021-08-06 16:31:28.000000 fcapy-0.1.4.1/tests/lattice/test_pattern_concept.py
-drwxrwxr-x   0 egor      (1000) egor      (1000)        0 2022-12-03 15:37:52.070840 fcapy-0.1.4.1/tests/ml/
--rw-rw-r--   0 egor      (1000) egor      (1000)        0 2021-01-10 15:43:40.000000 fcapy-0.1.4.1/tests/ml/__init__.py
--rw-rw-r--   0 egor      (1000) egor      (1000)     5904 2021-08-18 12:25:32.000000 fcapy-0.1.4.1/tests/ml/test_decision_lattice.py
-drwxrwxr-x   0 egor      (1000) egor      (1000)        0 2022-12-03 15:37:52.070840 fcapy-0.1.4.1/tests/mvcontext/
--rw-rw-r--   0 egor      (1000) egor      (1000)        0 2021-01-09 16:32:50.000000 fcapy-0.1.4.1/tests/mvcontext/__init__.py
--rw-rw-r--   0 egor      (1000) egor      (1000)    10139 2022-09-18 15:46:41.000000 fcapy-0.1.4.1/tests/mvcontext/test_mvcontext.py
--rw-rw-r--   0 egor      (1000) egor      (1000)     4724 2021-08-06 16:31:28.000000 fcapy-0.1.4.1/tests/mvcontext/test_pattern_structure.py
-drwxrwxr-x   0 egor      (1000) egor      (1000)        0 2022-12-03 15:37:52.070840 fcapy-0.1.4.1/tests/poset/
--rw-rw-r--   0 egor      (1000) egor      (1000)        0 2021-04-27 12:04:20.000000 fcapy-0.1.4.1/tests/poset/__init__.py
--rw-rw-r--   0 egor      (1000) egor      (1000)     7045 2022-09-08 13:32:19.000000 fcapy-0.1.4.1/tests/poset/test_lattice.py
--rw-rw-r--   0 egor      (1000) egor      (1000)    22063 2022-09-18 15:46:41.000000 fcapy-0.1.4.1/tests/poset/test_poset.py
--rw-rw-r--   0 egor      (1000) egor      (1000)      709 2020-12-04 10:31:42.000000 fcapy-0.1.4.1/tests/test_init.py
-drwxrwxr-x   0 egor      (1000) egor      (1000)        0 2022-12-03 15:37:52.070840 fcapy-0.1.4.1/tests/utils/
--rw-rw-r--   0 egor      (1000) egor      (1000)        0 2020-12-18 21:50:13.000000 fcapy-0.1.4.1/tests/utils/__init__.py
--rw-rw-r--   0 egor      (1000) egor      (1000)     1236 2021-01-13 15:21:27.000000 fcapy-0.1.4.1/tests/utils/test_utils.py
-drwxrwxr-x   0 egor      (1000) egor      (1000)        0 2022-12-03 15:37:52.070840 fcapy-0.1.4.1/tests/visualizer/
--rw-rw-r--   0 egor      (1000) egor      (1000)        0 2020-12-14 19:40:13.000000 fcapy-0.1.4.1/tests/visualizer/__init__.py
--rw-rw-r--   0 egor      (1000) egor      (1000)     4242 2022-09-08 13:32:19.000000 fcapy-0.1.4.1/tests/visualizer/test_line_layouts.py
--rw-rw-r--   0 egor      (1000) egor      (1000)     5523 2022-09-08 13:32:19.000000 fcapy-0.1.4.1/tests/visualizer/test_line_visualizers.py
--rw-rw-r--   0 egor      (1000) egor      (1000)      919 2022-05-17 14:47:40.000000 fcapy-0.1.4.1/tests/visualizer/test_measures.py
--rw-rw-r--   0 egor      (1000) egor      (1000)     2877 2022-07-01 15:36:03.000000 fcapy-0.1.4.1/tests/visualizer/test_mover.py
--rw-rw-r--   0 egor      (1000) egor      (1000)     1376 2021-07-09 17:45:59.000000 fcapy-0.1.4.1/tests/visualizer/test_visualizer.py
+drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:20:43.947313 fcapy-0.1.4.2/
+-rw-r--r--   0 egordudyrev   (501) staff       (20)    35148 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/LICENSE
+-rw-r--r--   0 egordudyrev   (501) staff       (20)    49690 2023-06-01 17:20:43.947103 fcapy-0.1.4.2/PKG-INFO
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     8514 2023-05-31 22:55:03.000000 fcapy-0.1.4.2/README.md
+drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:20:43.931414 fcapy-0.1.4.2/fcapy/
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     1071 2023-05-31 22:55:03.000000 fcapy-0.1.4.2/fcapy/__init__.py
+drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:20:43.933817 fcapy-0.1.4.2/fcapy/algorithms/
+-rw-r--r--   0 egordudyrev   (501) staff       (20)      735 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/fcapy/algorithms/__init__.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)    22047 2023-05-31 22:55:03.000000 fcapy-0.1.4.2/fcapy/algorithms/concept_construction.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)    30947 2023-05-31 22:55:03.000000 fcapy-0.1.4.2/fcapy/algorithms/lattice_construction.py
+drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:20:43.935415 fcapy-0.1.4.2/fcapy/context/
+-rw-r--r--   0 egordudyrev   (501) staff       (20)      617 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/fcapy/context/__init__.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)    36139 2023-05-31 22:55:03.000000 fcapy-0.1.4.2/fcapy/context/bintable.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     1679 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/fcapy/context/bintable_errors.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     7810 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/fcapy/context/converters.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)    28200 2023-05-31 22:55:03.000000 fcapy-0.1.4.2/fcapy/context/formal_context.py
+drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:20:43.936292 fcapy-0.1.4.2/fcapy/lattice/
+-rw-r--r--   0 egordudyrev   (501) staff       (20)      785 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/fcapy/lattice/__init__.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)    37577 2023-06-01 17:20:06.000000 fcapy-0.1.4.2/fcapy/lattice/concept_lattice.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     2692 2023-06-01 17:20:06.000000 fcapy-0.1.4.2/fcapy/lattice/concept_measures.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     6723 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/fcapy/lattice/formal_concept.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)    10888 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/fcapy/lattice/pattern_concept.py
+drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:20:43.937224 fcapy-0.1.4.2/fcapy/ml/
+-rw-r--r--   0 egordudyrev   (501) staff       (20)      530 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/fcapy/ml/__init__.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     3851 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/fcapy/ml/decision_based_model.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)    27818 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/fcapy/ml/decision_lattice.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     6249 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/fcapy/ml/decision_poset_structure.py
+drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:20:43.938022 fcapy-0.1.4.2/fcapy/mvcontext/
+-rw-r--r--   0 egordudyrev   (501) staff       (20)      662 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/fcapy/mvcontext/__init__.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)    25294 2023-05-31 22:55:03.000000 fcapy-0.1.4.2/fcapy/mvcontext/mvcontext.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)    21249 2023-05-31 22:55:03.000000 fcapy-0.1.4.2/fcapy/mvcontext/pattern_structure.py
+drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:20:43.938885 fcapy-0.1.4.2/fcapy/poset/
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     1100 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/fcapy/poset/__init__.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     7656 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/fcapy/poset/lattice.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)    35094 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/fcapy/poset/poset.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     1943 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/fcapy/poset/tree.py
+drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:20:43.939276 fcapy-0.1.4.2/fcapy/utils/
+-rw-r--r--   0 egordudyrev   (501) staff       (20)      156 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/fcapy/utils/__init__.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     2961 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/fcapy/utils/utils.py
+drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:20:43.940426 fcapy-0.1.4.2/fcapy/visualizer/
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     1195 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/fcapy/visualizer/__init__.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     4228 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/fcapy/visualizer/line_layouts.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)    20018 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/fcapy/visualizer/line_visualizers.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     3023 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/fcapy/visualizer/measures.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)    10768 2023-05-31 22:55:03.000000 fcapy-0.1.4.2/fcapy/visualizer/mover.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)    17702 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/fcapy/visualizer/visualizer.py
+drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:20:43.932742 fcapy-0.1.4.2/fcapy.egg-info/
+-rw-r--r--   0 egordudyrev   (501) staff       (20)    49690 2023-06-01 17:20:43.000000 fcapy-0.1.4.2/fcapy.egg-info/PKG-INFO
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     2112 2023-06-01 17:20:43.000000 fcapy-0.1.4.2/fcapy.egg-info/SOURCES.txt
+-rw-r--r--   0 egordudyrev   (501) staff       (20)        1 2023-06-01 17:20:43.000000 fcapy-0.1.4.2/fcapy.egg-info/dependency_links.txt
+-rw-r--r--   0 egordudyrev   (501) staff       (20)      236 2023-06-01 17:20:43.000000 fcapy-0.1.4.2/fcapy.egg-info/requires.txt
+-rw-r--r--   0 egordudyrev   (501) staff       (20)        6 2023-06-01 17:20:43.000000 fcapy-0.1.4.2/fcapy.egg-info/top_level.txt
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     1115 2023-05-31 22:55:03.000000 fcapy-0.1.4.2/pyproject.toml
+-rw-r--r--   0 egordudyrev   (501) staff       (20)       38 2023-06-01 17:20:43.947364 fcapy-0.1.4.2/setup.cfg
+drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:20:43.940690 fcapy-0.1.4.2/tests/
+drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:20:43.941439 fcapy-0.1.4.2/tests/algorithms/
+-rw-r--r--   0 egordudyrev   (501) staff       (20)        0 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/tests/algorithms/__init__.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     6006 2023-05-31 20:34:02.000000 fcapy-0.1.4.2/tests/algorithms/test_concept_construction.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)    14418 2023-05-31 20:34:02.000000 fcapy-0.1.4.2/tests/algorithms/test_lattice_construction.py
+drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:20:43.942596 fcapy-0.1.4.2/tests/context/
+-rw-r--r--   0 egordudyrev   (501) staff       (20)        0 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/tests/context/__init__.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     1861 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/tests/context/data_to_test.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     7029 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/tests/context/test_bintable.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     3379 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/tests/context/test_converters.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)    12847 2023-05-31 20:34:02.000000 fcapy-0.1.4.2/tests/context/test_formal_context.py
+drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:20:43.943621 fcapy-0.1.4.2/tests/lattice/
+-rw-r--r--   0 egordudyrev   (501) staff       (20)        0 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/tests/lattice/__init__.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)    15404 2023-05-31 20:34:02.000000 fcapy-0.1.4.2/tests/lattice/test_concept_lattice.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     2028 2023-06-01 17:20:06.000000 fcapy-0.1.4.2/tests/lattice/test_concept_measures.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     5209 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/tests/lattice/test_formal_concept.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     2855 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/tests/lattice/test_pattern_concept.py
+drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:20:43.943967 fcapy-0.1.4.2/tests/ml/
+-rw-r--r--   0 egordudyrev   (501) staff       (20)        0 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/tests/ml/__init__.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     6146 2023-05-31 20:34:02.000000 fcapy-0.1.4.2/tests/ml/test_decision_lattice.py
+drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:20:43.944549 fcapy-0.1.4.2/tests/mvcontext/
+-rw-r--r--   0 egordudyrev   (501) staff       (20)        0 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/tests/mvcontext/__init__.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)    11993 2023-05-31 20:34:02.000000 fcapy-0.1.4.2/tests/mvcontext/test_mvcontext.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     7883 2023-05-31 20:34:02.000000 fcapy-0.1.4.2/tests/mvcontext/test_pattern_structure.py
+drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:20:43.945088 fcapy-0.1.4.2/tests/poset/
+-rw-r--r--   0 egordudyrev   (501) staff       (20)        0 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/tests/poset/__init__.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     7045 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/tests/poset/test_lattice.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)    22063 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/tests/poset/test_poset.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)      709 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/tests/test_init.py
+drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:20:43.945507 fcapy-0.1.4.2/tests/utils/
+-rw-r--r--   0 egordudyrev   (501) staff       (20)        0 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/tests/utils/__init__.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     1236 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/tests/utils/test_utils.py
+drwxr-xr-x   0 egordudyrev   (501) staff       (20)        0 2023-06-01 17:20:43.946632 fcapy-0.1.4.2/tests/visualizer/
+-rw-r--r--   0 egordudyrev   (501) staff       (20)        0 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/tests/visualizer/__init__.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     4242 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/tests/visualizer/test_line_layouts.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     5523 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/tests/visualizer/test_line_visualizers.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)      919 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/tests/visualizer/test_measures.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     2877 2023-04-11 14:16:21.000000 fcapy-0.1.4.2/tests/visualizer/test_mover.py
+-rw-r--r--   0 egordudyrev   (501) staff       (20)     1463 2023-05-31 22:55:03.000000 fcapy-0.1.4.2/tests/visualizer/test_visualizer.py
```

### Comparing `fcapy-0.1.4.1/LICENSE` & `fcapy-0.1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.1/PKG-INFO` & `fcapy-0.1.4.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,11 @@
-Metadata-Version: 2.1
-Name: fcapy
-Version: 0.1.4.1
-Summary: A library to work with formal (and pattern) contexts, concepts, lattices
-Home-page: https://github.com/EgorDudyrev/FCApy
-Author: Egor Dudyrev
-Author-email: egor.dudyrev@yandex.ru
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: context
-Provides-Extra: mvcontext
-Provides-Extra: lattice
-Provides-Extra: algorithms
-Provides-Extra: visualizer
-Provides-Extra: poset
-Provides-Extra: ml
-Provides-Extra: tests
-Provides-Extra: docs
-Provides-Extra: all
-License-File: LICENSE
-
 # FCApy
 
-[![Travis (.com)](https://img.shields.io/travis/com/EgorDudyrev/FCApy)](https://travis-ci.com/github/EgorDudyrev/FCApy)
+[![PyPi](https://img.shields.io/pypi/v/fcapy)](https://pypi.org/project/fcapy)
+[![GitHub Workflow](https://img.shields.io/github/actions/workflow/status/EgorDudyrev/caspailleur/python-package.yml?logo=github)](https://github.com/EgorDudyrev/fcapy/actions/workflows/python-package.yml)
 [![Read the Docs (version)](https://img.shields.io/readthedocs/fcapy/latest)](https://fcapy.readthedocs.io/en/latest/)
 [![Codecov](https://img.shields.io/codecov/c/github/EgorDudyrev/FCApy)](https://codecov.io/gh/EgorDudyrev/FCApy)
 [![GitHub](https://img.shields.io/github/license/EgorDudyrev/FCApy)](https://github.com/EgorDudyrev/FCApy/blob/main/LICENSE)
 
 A python package to work with Formal Concept Analysis (FCA).
 
 ## Install
```

### Comparing `fcapy-0.1.4.1/fcapy/__init__.py` & `fcapy-0.1.4.2/fcapy/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,7 +18,10 @@
     'tqdm': "The package helps to track the progress of looped functions and estimate their time to complete",
     'numpy': "The package Uses C++ and vectorized matrix multiplication to speed up IntervalPS execution",
     'bitsets': "The package greatly optimizes BinTables execution",
     'bitarray': "The package greatly optimizes BinTables execution",
     'networkx': "The package to convert POSets to Graphs and to visualize them as graphs",
 }
 LIB_INSTALLED = check_installed_packages(PACKAGE_DESCRIPTION)
+
+
+__version__ = '0.1.4.2'
```

### Comparing `fcapy-0.1.4.1/fcapy/algorithms/__init__.py` & `fcapy-0.1.4.2/fcapy/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.1/fcapy/algorithms/concept_construction.py` & `fcapy-0.1.4.2/fcapy/algorithms/concept_construction.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,351 +1,294 @@
 """
 This module contains functions that take a `FormalContext` (or `MVContext`)
 and return a set of formal (or pattern) concepts.
 Some of them return a `ConceptLattice` instead of just a set of concepts.
 
 """
-from typing import List, Tuple
+from collections import deque
+from typing import List, Tuple, Iterator, Iterable, Union
+
+import numpy as np
+from bitarray import frozenbitarray as fbarray
+from bitarray.util import zeros as bazeros
+from caspailleur.order import inverse_order, sort_intents_inclusion
 
 from fcapy.context.formal_context import FormalContext
+from fcapy.context.bintable import BinTableBitarray
 from fcapy.mvcontext.mvcontext import MVContext
 from fcapy.lattice.formal_concept import FormalConcept
 from fcapy.lattice.pattern_concept import PatternConcept
 from fcapy.utils import utils
-import random
-from copy import deepcopy, copy
-import math
 
 
-def close_by_one(context: MVContext, output_as_concepts=True, iterate_extents=None,
-                 initial_combinations=None, iter_concepts_to_check=None):
+def close_by_one(context: Union[FormalContext, MVContext], n_projections_to_binarize: int = 1000)\
+        -> Iterator[Union[FormalConcept, PatternConcept]]:
     """Return a list of concepts generated by CloseByOne (CbO) algorithm
 
     Parameters
     ----------
     context: `FormalContext` or `MVContext`
         A context to build a set of concepts on
-    output_as_concepts: `bool`
-        A flag whether to return a list of concepts as a list of `FormalConcept`/`PatternConcept` objects (if set True)
-        or as a dictionary with concepts extents and intents
-    iterate_extents: `bool`
-        A flag whether to run CbO by iterating through subsets of objects (if set True) or of attributes (if set False)
-        By default it sets to True if the set of objects is smaller than the set of attributes
-    initial_combinations: `list` of `int`
-        A list of subsets of objects/attributes indexes (depends on ``iterate_extents``) to start CbO algorithm from
-        Default value is empty list []
-    iter_concepts_to_check: `list` of `int`
-        A list of attributes/objects indexes (depends on ``iterate_extents``) to run CbO algorithm on
+    n_projections_to_binarize: int
+        The maximal number of projections of MVContext, s.t. it can be binarized.
+        Binarizing the context may fasten up the computations. However, it can also result in more memory consumption.
 
     Returns
     -------
-    Either ``data`` or ``concepts`` depends on ``output_as_concepts`` attribute
-    data: `dict`
-        A dictionary which contains a set of concepts extents and concepts intents
-    concepts: `list` of `FormalConcept` or `PatternConcept`
-        A list of concepts of class `FormalConcept` (if given context is of type `FormalContext`)
+    concepts: `Iterator` of `FormalConcept` or `PatternConcept`
+        An iterator of concepts of class `FormalConcept` (if given context is of type `FormalContext`)
         or `PatternConcept` (if given context is of type `MVContext`)
 
     """
-    if iterate_extents is False:
-        assert type(context) == FormalContext, "Can set iterate_extents=False only if FormalContext is given"
-
-    if initial_combinations is not None:
-        assert iterate_extents is not None,\
-            "`iterate_extents parameter should be specified if initial_combinations are given " \
-            "(`True if initial_combinations are extents, `False if inital_combinations are intents)"
-
-    if iter_concepts_to_check is not None:
-        assert iterate_extents is not None, \
-            "`iterate_extents parameter should be specified if iter_concepts_to_check are given " \
-            "(`True if iter_concepts_to_check are objects, `False if iter_concepts_to_check are attributes)"
-
-    if iterate_extents is None:
-        iterate_extents = context.n_objects < context.n_attributes if type(context) == FormalConcept else True
-    n_iters = context.n_objects if iterate_extents else context.n_attributes
-
-    # <iterset> - iterating set - the set of object if one construct construct concepts while iterating over objects,
-    #   the set of attributes otherwise
-    # <sideset> - the other set, "sided" with <iterset>.
-    #   If <iterset> is the set of objects then <sideset> is the set of attributes and vice versa
-    iterset_fnc, sideset_fnc = context.extension_i, context.intention_i
-    if not iterate_extents:
-        iterset_fnc, sideset_fnc = sideset_fnc, iterset_fnc
-
-    iter_concepts_to_check = list(range(n_iters)) if iter_concepts_to_check is None else iter_concepts_to_check
+    if isinstance(context, FormalContext):
+        is_wide = context.n_objects < context.n_bin_attrs
 
-    itersets_i_dict = {}
-    sidesets_i = []
-    combinations_to_check = [[]] if initial_combinations is None else initial_combinations
-
-    while len(combinations_to_check) > 0:
-        comb_i = combinations_to_check.pop(0)
-        sideset_i = sideset_fnc(comb_i)
-        iterset_i = tuple(iterset_fnc(sideset_i))
-        iterset_i_new = sorted(set(iterset_i)-set(comb_i))
-
-        is_not_lexicographic = len(comb_i) > 0 and any([g_i < comb_i[-1] for g_i in iterset_i_new])
-        is_duplicate = iterset_i in itersets_i_dict
-        if any([is_not_lexicographic, is_duplicate]):
-            continue
-
-        itersets_i_dict[iterset_i] = len(sidesets_i)
-        sidesets_i.append(sideset_i)
-
-        iterset_i = list(iterset_i)
+        if is_wide:
+            concepts_iterator = close_by_one_objectwise_fbarray(context)
+        else:  # not wide, i.e. contains more objects than attributes
+            concepts_transpose_iter = close_by_one_objectwise_fbarray(context.T)
+            context_hash = context.hash_fixed()
+            concepts_iterator = (
+                FormalConcept(c.intent_i, c.intent, c.extent_i, c.extent, context_hash=context_hash)
+                for c in concepts_transpose_iter
+            )
+
+    else:  # not formal, i.e. many valued context
+        try:
+            n_projections = context.n_bin_attrs
+        except NotImplementedError:
+            n_projections = None
+
+        if n_projections is None or n_projections > n_projections_to_binarize:
+            concepts_iterator = close_by_one_objectwise(context)
+
+        else:  # n_projections <= n_projections_to_binarize:
+            if context.n_objects <= n_projections:
+                extents_iter = ((c.extent_i, c.extent) for c in close_by_one_objectwise_fbarray(context.binarize()))
+            else:  # context.n_objects > n_projections
+                extents_iter = ((c.intent_i, c.intent) for c in close_by_one_objectwise_fbarray(context.binarize().T))
+
+            context_hash = context.hash_fixed()
+            def pattern_concept_factory(extent_i, extent):
+                intent_i = context.intention_i(extent_i)
+                intent = {context.pattern_structures[ps_i].name: pattern for ps_i, pattern in intent_i.items()}
+                return PatternConcept(extent_i, extent, intent_i, intent,
+                                      context.pattern_types, context.attribute_names, context_hash=context_hash)
+            concepts_iterator = (pattern_concept_factory(extent_i, extent) for extent_i, extent in extents_iter)
+    return concepts_iterator
 
-        new_combs = []
-        for g_i in iter_concepts_to_check:
-            if g_i not in iterset_i \
-                    and (len(comb_i) == 0 or g_i > comb_i[-1]):
-                new_combs.append(iterset_i+[g_i])
-        combinations_to_check = new_combs + combinations_to_check
 
-    itersets_i = list({idx: x_i for x_i, idx in itersets_i_dict.items()}.values())
-
-    extents_i, intents_i = itersets_i, sidesets_i
-    if not iterate_extents:
-        extents_i, intents_i = intents_i, extents_i
-
-    if output_as_concepts:
-        object_names = context.object_names
-        attribute_names = context.attribute_names
-        context_hash = context.hash_fixed()
-
-        concepts = []
-        for concept_data in zip(extents_i, intents_i):
-            extent_i, intent_i = concept_data
-            extent = [object_names[g_i] for g_i in extent_i]
-            if type(context) == FormalContext:
-                intent = [attribute_names[m_i] for m_i in intent_i]
-                concept = FormalConcept(extent_i, extent, intent_i, intent, context_hash=context_hash)
-            else:
-                intent = {context.pattern_structures[ps_i].name: description for ps_i, description in intent_i.items()}
-                concept = PatternConcept(
-                    extent_i, extent, intent_i, intent,
-                    context.pattern_types, context.attribute_names,
-                    context_hash=context_hash)
-            concepts.append(concept)
-        return concepts
-
-    data = {'extents_i': extents_i, 'intents_i': intents_i}
-    return data
-
-
-def sofia_objectwise(
-        K: FormalContext or MVContext,
-        L_max: int = 100, measure_name: str = 'LStab',
-        use_tqdm: bool = False,
-        proj_start: int = None
-) -> 'ConceptLattice':
-    from fcapy.lattice import ConceptLattice
+def close_by_one_objectwise(context: Union[FormalContext, MVContext]) -> Iterator[Union[FormalConcept, PatternConcept]]:
+    """Return a list of concepts generated by CloseByOne (CbO) algorithm
 
-    #############
-    # The Setup #
-    #############
-    is_K_multivalued = isinstance(K, MVContext)
-
-    # Define concept constructors based on the class of context K
-    if is_K_multivalued:
-        def concept_factory(ext_i, ext_, int_i, int_, hash_):
-            return PatternConcept(ext_i, ext_, int_i, int_, K.pattern_types, K.attribute_names, context_hash=hash_)
-    else:
-        def concept_factory(ext_i, ext_, int_i, int_, hash_):
-            return FormalConcept(ext_i, ext_, int_i, int_, context_hash=hash_)
+    Parameters
+    ----------
+    context: `FormalContext` or `MVContext`
+        A context to build a set of concepts on
 
-    def close_by_one_proj(K_, extents, i):
-        f = close_by_one(
-            K_,
-            initial_combinations=extents, iter_concepts_to_check=[i-1],
-            output_as_concepts=True, iterate_extents=True,
-        )
-        return f
+    Returns
+    -------
+    concepts: `iterator` of `FormalConcept` or `PatternConcept`
+        A list of concepts of class `FormalConcept` (if given context is of type `FormalContext`)
+        or `PatternConcept` (if given context is of type `MVContext`)
 
-    # Define where to start and where to end while iterating projections
-    proj_start = int(math.log2(L_max)) if proj_start is None else proj_start
-    max_proj = len(K)
-
-    proj_iterator = range(proj_start + 1, max_proj + 1)
-    if use_tqdm:
-        proj_iterator = utils.safe_tqdm(
-            proj_iterator, desc='SOFIA: Iterate objects', initial=proj_start, total=max_proj
-        )
+    """
+    n_objs = context.n_objects
+    object_names, attribute_names = context.object_names, context.attribute_names
+    context_hash = context.hash_fixed()
 
-    #################
-    # The Algorithm #
-    #################
-
-    # Step 1: Construct a lattice on a small enough subset of the context
-    K_proj = K[:proj_start]
-    L_proj = ConceptLattice.from_context(K_proj, algo='CbO')
-
-    for proj_i in proj_iterator:
-        # Step i.0: Update context projection
-        K_proj = K[:proj_i]
-
-        # Step i.1: Update old concepts to the new context
-        K_proj_hash = K_proj.hash_fixed()
-        for c in L_proj:
-            ext_i_new = K_proj.extension_i(c.intent_i)
-            ext_new = [K_proj.object_names[g_i] for g_i in ext_i_new]
-            c_new = concept_factory(ext_i_new, ext_new, c.intent_i, c.intent, K_proj_hash)
-            L_proj._update_element(c, c_new)
-
-        # Step i.2: Construct concepts on a new part of the context
-        extents_proj = [c.extent_i for c in L_proj]
-        new_concepts = close_by_one_proj(K_proj, extents_proj, proj_i)
-
-        # Step i.3: Add new concepts to the lattice
-
-        # concepts that were changed during projection iteration
-        concepts_to_add = list(set(new_concepts) - set(L_proj))
-        # sort concepts to ensure there will be no moment with multiple top or bottom concepts
-        concepts_to_add = L_proj.sort_concepts(concepts_to_add)
-        if len(concepts_to_add) >= 2 and concepts_to_add[-1] < L_proj[L_proj.bottom]:
-            concepts_to_add = [concepts_to_add[-1]] + concepts_to_add[:-1]
-
-        for c in concepts_to_add:  # As, for now, ConceptLattice does not support addition of many elements at once
-            L_proj.add(c)
-
-        # Step i.4: Drop bad concepts from the lattice (if needed)
-        if len(L_proj) > L_max:
-            L_proj.calc_concepts_measures(measure_name, K_proj)
-            measure_values = L_proj.measures[measure_name]
-            thold = sorted(measure_values)[::-1][L_max]
+    def create_concept(extent_idxs, intent_idxs):
+        extent_idxs = sorted(extent_idxs)
+        extent = [object_names[g_i] for g_i in extent_idxs]
+        if type(context) == FormalContext:
+            intent = [attribute_names[m_i] for m_i in intent_idxs]
+            return FormalConcept(extent_idxs, extent, intent_idxs, intent, context_hash=context_hash)
 
-            top_i, bottom_i = L_proj.top, L_proj.bottom
-            concepts_to_remove = [i for i, v in enumerate(measure_values)
-                                  if v <= thold and i != top_i and i != bottom_i]
+        intent = {context.pattern_structures[ps_i].name: description for ps_i, description in intent_idxs.items()}
+        return PatternConcept(extent_idxs, extent, intent_idxs, intent,
+                              context.pattern_types, context.attribute_names, context_hash=context_hash)
+
+    extents_i_found = set()
+    combinations_to_check = deque([tuple()])
+
+    while combinations_to_check:
+        comb_i = combinations_to_check.pop()
+        intent_i = context.intention_i(comb_i)
+        comb_i_set = set(comb_i)
+        if comb_i:
+            objects_lexicographic = [g_i for g_i in range(comb_i[-1]) if g_i not in comb_i_set]
+            extent_lexicographic = context.extension_i(intent_i, base_objects_i=objects_lexicographic)
+            if extent_lexicographic:
+                continue
+
+        base_objects_i = range(comb_i[-1]+1, n_objs) if comb_i else range(n_objs)
+        base_objects_i = [i for i in base_objects_i if i not in comb_i_set]
+        extent_i = comb_i + tuple(context.extension_i(intent_i, base_objects_i=base_objects_i))
 
-            for c_i in concepts_to_remove[::-1]:
-                del L_proj[c_i]
+        if extent_i in extents_i_found:
+            continue
 
-    return L_proj
+        yield create_concept(extent_i, intent_i)
 
+        possible_new_objects = range(n_objs - 1, (comb_i[-1] if comb_i else 0) - 1, -1)
+        extent_i_set = set(extent_i)
+        new_combs = [extent_i + (g_i,) for g_i in possible_new_objects if g_i not in extent_i_set]
+        combinations_to_check.extend(new_combs)
 
-def sofia_binary(
-        K: FormalContext, L_max: int = 100,
-        iterate_attributes: bool = False, measure: str = 'LStab',
-        proj_sorting: str = None, proj_start: int = None, use_tqdm: bool = False):
-    """Return a lattice of the most interesting concepts generated by SOFIA algorithm. Optimized for `FormalContext`
 
-    WARNING: The author of the algorithm (A. Buzmakov) said this function is not an accurate implementation
-    of the original Sofia algorithm. Thus the function may work not as efficient as expected.
+def close_by_one_objectwise_fbarray(context: Union[FormalContext, MVContext])\
+        -> Iterator[Union[FormalConcept, PatternConcept]]:
+    """Return a list of concepts generated by CloseByOne (CbO) algorithm
 
     Parameters
     ----------
-    K: `FormalContext`
-        A context to build a list of concepts on
-    L_max: `int`
-        Maximum size of returned lattice. That is the maximum number of most interesting concepts
-    iterate_attributes: `bool`
-        A flag whether to iterate a set of attributes as a chain of projections (if set to True) or a set of objects o/w
-    measure: `string`
-        The name of a concept interesting measure_name to maximize
-    proj_sorting: `str` of {'ascending', 'descending', 'random', None}
-        A way to sort a chain of projections by their support.
-        E.g. if ``iterate_attributes`` is set to True, 'Ascending' sorting start running projections
-        from an attribute shared by the least amount of objects to an attributes shared by the most amount of objects
-    proj_start: `int`
-        A number of projection (a set of attributes/objects) to construct a basic `ConceptLattice` on
-    use_tqdm: `bool`
-        A flag whether to visualize the progress of the algorithm with `tqdm` bar or not
+    context: `FormalContext` or `MVContext`
+        A context to build a set of concepts on
 
     Returns
     -------
-    lattice: `ConceptLattice`
-        A ConceptLattice which contains a set of Formal (or Pattern) concepts
-        with high values of given interesting measure
+    concepts: `iterator` of `FormalConcept` or `PatternConcept`
+        A list of concepts of class `FormalConcept` (if given context is of type `FormalContext`)
+        or `PatternConcept` (if given context is of type `MVContext`)
 
     """
-    if iterate_attributes:
-        raise NotImplementedError('Sofia algorithm does not work properly for value ``iterate_attributes`` = False'
-                                  'due to wrong stability index calculations')
-
-    def setup_projection_order(K_):
-        max_proj_ = len(K_)
-        if proj_sorting == 'ascending':
-            def key_func(proj_i):
-                return len(K_.intention_i([proj_i]))
-        elif proj_sorting == 'descending':
-            def key_func(proj_i):
-                return -len(K_.intention_i([proj_i]))
-        elif proj_sorting == 'random':
-            rand_idxs = random.sample(range(max_proj_), k=max_proj_)
-
-            def key_func(proj_i):
-                return rand_idxs[proj_i]
-        elif proj_sorting is None:
-            key_func = None
-        else:
-            raise ValueError(f'Sofia_binary error. Unknown proj_sorting is given: {proj_sorting}. ' +
-                             'Possible ones are "ascending", "descending", "random"')
-
-        order = range(max_proj_)
-        if key_func:
-            order = sorted(order, key=key_func)
-        return order
-
-    def setup_measure(measure_):
-        if not isinstance(measure_, str):
-            raise TypeError('Sofia_binary error. For now, you can only specify the name of already defined measure')
-        return measure_
-
-    if iterate_attributes is None:
-        iterate_attributes = False
-        # iterate_attributes = len(K.attribute_names) < len(K.object_names)  #  TODO: Add iterate_attributes support
-
-    K_hash = K.hash_fixed()
-    if iterate_attributes:
-        K = K.T
-
-    proj_order = setup_projection_order(K)
-    measure_name = setup_measure(measure)
-
-    L = sofia_objectwise(K[proj_order], L_max, measure_name=measure_name, use_tqdm=use_tqdm, proj_start=proj_start)
-
-    if iterate_attributes:
-        L = L.T
-
-    for i, c in enumerate(L):
-        c_data = {k: v for k, v in c.__dict__.items() if not k.startswith('_')}
-        c_data['context_hash'] = K_hash
-        L._update_element(c, c.__class__(**c_data))
-
-    return L
+    n_objs, n_attrs = context.n_objects, context.n_bin_attrs
+    object_names, attribute_names = context.object_names, context.attribute_names
+    context_hash = context.hash_fixed()
 
+    def create_concept(extent_idxs: List[int], intent_ba: fbarray):
+        extent_idxs = sorted(extent_idxs)
+        extent = [object_names[g_i] for g_i in extent_idxs]
+        if type(context) == FormalContext:
+            intent_idxs = list(intent_ba.itersearch(True))
+            intent = [attribute_names[m_i] for m_i in intent_idxs]
+            return FormalConcept(extent_idxs, extent, intent_idxs, intent, context_hash=context_hash)
+
+        intent_idxs = context.intention_i(extent_idxs)
+        intent = {context.pattern_structures[ps_i].name: description for ps_i, description in intent_idxs.items()}
+        return PatternConcept(extent_idxs, extent, intent_idxs, intent,
+                              context.pattern_types, context.attribute_names, context_hash=context_hash)
+
+    all_attrs = ~bazeros(n_attrs)
+
+    context_bin = context.binarize() if isinstance(context, MVContext) else context
+    objs_descriptions = BinTableBitarray(context_bin.data.data).data
+
+    def intention_ba(objs_idxs: Iterable[int]) -> fbarray:
+        intent = all_attrs.copy()
+        for g_i in objs_idxs:
+            intent &= objs_descriptions[g_i]
+        return fbarray(intent)
+
+    def extension_iter(intent_ba: fbarray, base_objects: Iterable[int] = range(n_objs)) -> Iterator[int]:
+        for g_i in base_objects:
+            if intent_ba & objs_descriptions[g_i] == intent_ba:
+                yield g_i
+
+    intents_found: set[fbarray] = set()
+    combinations_to_check = deque([tuple()])
+    n_cncpt = 0
+
+    while combinations_to_check:
+        comb_i = combinations_to_check.pop()
+        intent_ba = intention_ba(comb_i)
+        if intent_ba in intents_found:
+            continue
 
-def sofia_general(K: MVContext, L_max=100, measure='LStab', proj_to_start=None, use_tqdm=False):
-    """Return a lattice of the most interesting concepts generated by SOFIA algorithm. Can work with any `MVContext`
+        comb_i_set = set(comb_i)
+        if comb_i:
+            objects_lexicographic = (g_i for g_i in range(comb_i[-1]) if g_i not in comb_i_set)
+            objects_lexicographic = extension_iter(intent_ba, objects_lexicographic)
+            if any(True for _ in objects_lexicographic):
+                continue
+
+        base_objects_i = range((comb_i[-1]+1) if comb_i else 0, n_objs)
+        base_objects_i = (i for i in base_objects_i if i not in comb_i_set)
+        extent_i = comb_i + tuple(extension_iter(intent_ba, base_objects_i))
+
+        yield create_concept(extent_i, intent_ba)
+        n_cncpt += 1
+
+        intents_found.add(intent_ba)
+        possible_new_objects = range(n_objs - 1, (comb_i[-1] if comb_i else 0) - 1, -1)
+        extent_i_set = set(extent_i)
+        new_combs = [extent_i + (g_i,) for g_i in possible_new_objects if g_i not in extent_i_set]
+        combinations_to_check.extend(new_combs)
+
+
+def sofia(
+        K: Union[FormalContext, MVContext], L_max: int = 100, min_supp: float = 0,
+        use_tqdm: bool = False,use_log_stability_bound=True
+) -> List[Union[FormalConcept, PatternConcept]]:
+    min_supp = min_supp * len(K) if min_supp < 1 else min_supp
+
+    if use_log_stability_bound:
+        def stability_lbounds(extents: List[fbarray]) -> List[float]:
+            #assert all(a.count() <= b.count() for a, b in zip(extents, extents[1:]))
+            bounds = []
+            for i, extent in enumerate(extents):
+                bound = extent.count()
+                for potent_child in extents[i-1::-1]:
+                    if potent_child & extent == potent_child:
+                        bound -= potent_child.count()
+                        break
+                bounds.append(bound)
+            return bounds
+    else:
+        def stability_lbounds(extents: List[fbarray]) -> List[float]:
+            children_ordering = inverse_order(sort_intents_inclusion(extents))
+            children_intersections = (
+                ((extent & (~extents[child])).count() for child in children.itersearch(True))
+                if children.any() else [extent.count()]
+                for children, extent in zip(children_ordering, extents)
+            )
+            bounds = [1-sum(2**(-v) for v in intersections) for intersections in children_intersections]
+            return bounds
+
+    extents_proj: List[fbarray] = [fbarray(~bazeros(K.n_objects))]
+
+    n_projs = K.n_bin_attrs
+    proj_iterator = utils.safe_tqdm(enumerate(K.to_bin_attr_extents()), total=n_projs,
+                                    desc='Iter. Sofia projections', disable=not use_tqdm)
+    for proj_i, (_, attr_extent_ba) in proj_iterator:
+        if attr_extent_ba.all():
+            continue
 
-    WARNING: The author of the algorithm (A. Buzmakov) said this is not an accurate implementation
-    of the original Sofia algorithm. Thus, the function may work not as efficient as expected.
-    Moreover, it represents the simplest way to construct a lattice over MVContext. Therefore, it is very inefficient.
+        if attr_extent_ba.count() < min_supp:
+            continue
 
-    Parameters
-    ----------
-    K: `FormalContext` or `MVContext`
-        A context to build a list of concepts on
-    L_max: `int`
-        Maximum size of returned lattice. That is the maximum number of most interesting concepts
-    measure: `string`
-        The name of a concept interesting measure to maximize
-    proj_to_start: `int`
-        A number of projection (a set of attributes/objects) to construct a basic `ConceptLattice` on
-    use_tqdm: `bool`
-        A flag whether to visualize the progress of the algorithm with `tqdm` bar or not
+        new_extents = {extent & attr_extent_ba for extent in extents_proj}
+        extents_proj = sorted(set(extents_proj) | new_extents, key=lambda extent: extent.count())
+        extents_proj = extents_proj[:1] + [extent for extent in extents_proj[1:] if extent.count() >= min_supp]
 
-    Returns
-    -------
-    lattice: `ConceptLattice`
-        A ConceptLattice which contains a set of Formal (or Pattern) concepts
-        with high values of given interesting measure
+        if len(extents_proj) > L_max:
+            measure_values = stability_lbounds(extents_proj)
+            thold = sorted(measure_values)[::-1][L_max]
+            extents_proj = [extent for extent_i, (extent, measure) in enumerate(zip(extents_proj, measure_values))
+                            if measure > thold or extent_i in {0, len(extents_proj)-1}]
 
-    """
-    return sofia_objectwise(K, L_max, measure, use_tqdm, proj_to_start)
+    context_hash = None  # K.hash_fixed()
+    def concept_factory(extent_ba: fbarray):
+        extent_ids = list(extent_ba.itersearch(True))
+        intent_ids = K.intention_i(extent_ids)
+        if isinstance(K, FormalContext):
+            return FormalConcept(extent_ids, [K.object_names[g_i] for g_i in extent_ids],
+                                 intent_ids, [K.attribute_names[m_i] for m_i in intent_ids],
+                                 context_hash=context_hash)
+
+        return PatternConcept(
+            extent_ids, [K.object_names[g_i] for g_i in extent_ids],
+            intent_ids, {K.pattern_structures[ps_i].name: description
+                         for ps_i, description in intent_ids.items()},
+            pattern_types=K.pattern_types,
+            attribute_names=K.attribute_names,
+            context_hash=context_hash
+        )
+    final_concepts = [concept_factory(extent) for extent in extents_proj]
+    return final_concepts
 
 
 def parse_decision_tree_to_extents(tree, X, n_jobs=1) -> List[Tuple[int, ...]]:
     """Return a set of extents of nodes from sklearn `DecisionTree` (or `RandomForest`)
 
     Parameters
     ----------
@@ -527,7 +470,47 @@
                                   concepts[i].extent_i, concepts[i].extent, 
                                   context_hash=context_hash)
                     for i in range(len(concepts))]
         children_dict, parents_dict = parents_dict, children_dict
 
     lattice = ConceptLattice(concepts, children_dict=children_dict)
     return lattice
+
+
+def lcm_skmine(context: Union[FormalContext, MVContext], min_supp: float = 1, n_jobs: int = 1)\
+        -> List[Union[FormalConcept, PatternConcept]]:
+    from skmine.itemsets import LCM
+
+    context_bin = context if isinstance(context, FormalContext) else context.binarize()
+    itemsets = [list(row.itersearch(True)) for row in BinTableBitarray(context_bin.data.data)]
+
+    lcm = LCM(min_supp=min_supp, n_jobs=n_jobs)
+    lcm_data = lcm.fit_transform(itemsets, return_tids=True)
+    intents_i = list(lcm_data['itemset'])
+    extents_i = [list(row) for row in lcm_data['tids']]
+    del lcm_data
+
+    if all(len(intent_i) < context_bin.n_attributes for intent_i in intents_i):
+        intents_i.append(list(range(context_bin.n_attributes)))
+        extents_i.append(context_bin.extension_i(intents_i[-1]))
+
+    if all(len(extent_i) < context_bin.n_objects for extent_i in extents_i):
+        extents_i.append(list(range(context_bin.n_objects)))
+        intents_i.append(context_bin.intention_i(extents_i[-1]))
+
+    context_hash = context.hash_fixed()
+    if isinstance(context, FormalContext):
+        def concept_factory(extent_i, intent_i):
+            return FormalConcept(
+                extent_i, [context.object_names[g_i] for g_i in extent_i],
+                intent_i, [context.attribute_names[m_i] for m_i in intent_i],
+                context_hash=context_hash
+            )
+    else:
+        def concept_factory(extent_i, _):
+            intent_i = context.intention_i(extent_i)
+            intent = {context.pattern_structures[ps_i].name: pattern for ps_i, pattern in intent_i.items()}
+            return PatternConcept(extent_i, [context.object_names[g_i] for g_i in extent_i],
+                                  intent_i, intent,
+                                  context.pattern_types, context.attribute_names, context_hash=context_hash)
+
+    return [concept_factory(extent_i, intent_i) for extent_i, intent_i in zip(extents_i, intents_i)]
```

### Comparing `fcapy-0.1.4.1/fcapy/algorithms/lattice_construction.py` & `fcapy-0.1.4.2/fcapy/algorithms/lattice_construction.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,24 +4,25 @@
 i.e. the order of given concepts in the form {`parent_concept_index`: `child_concept_index`}.
 
 Parent_concept is a concept which is bigger (or more general) than the child concept
 and there is no other concept between these two.
 
 """
 from copy import deepcopy
-from typing import Collection
+from typing import Collection, Union, Tuple, List, Dict, Set
 
 from fcapy.lattice.formal_concept import FormalConcept
 from fcapy.lattice.pattern_concept import PatternConcept
 from fcapy.utils import utils
 
 
 def complete_comparison(
-        concepts: Collection[FormalConcept or PatternConcept],
-        is_concepts_sorted: bool = False, n_jobs: int = 1, use_tqdm: bool = False):
+        concepts: Collection[Union[FormalConcept, PatternConcept]],
+        is_concepts_sorted: bool = False, n_jobs: int = 1, use_tqdm: bool = False
+) -> Dict[int, Set[int]]:
     """Return a dict with subconcepts relation on given ``concepts``. A slow but accurate bruteforce method
 
     Parameters
     ----------
     concepts: `list` of `FormalConcept` or `PatternConcept`
         A list of concepts to compare
     is_concepts_sorted: `bool`
@@ -71,15 +72,15 @@
         b_is = b_is.copy() if not is_concepts_sorted else sorted(b_is)
         for b_i in b_is:
             subconcepts_dict[a_i] -= all_subconcepts_dict[b_i]
 
     return subconcepts_dict
 
 
-def construct_spanning_tree(concepts, is_concepts_sorted=False, use_tqdm=False):
+def construct_spanning_tree(concepts, is_concepts_sorted=False, use_tqdm=False) -> Dict[int, int]:
     """Return a spanning tree of subconcepts relation on given ``concepts``.
 
     A spanning tree means that for each concept from ``concepts`` we look for one parent concept only
     (even if there are actually many of them)
 
     Parameters
     ----------
@@ -139,15 +140,16 @@
 
         subconcepts_st_dict[superconcept_i].add(c_i)
         superconcepts_st_dict[c_i] = {superconcept_i}
 
     return subconcepts_st_dict, superconcepts_st_dict
 
 
-def construct_lattice_from_spanning_tree(concepts, sptree_chains, is_concepts_sorted=False, use_tqdm=False):
+def construct_lattice_from_spanning_tree(concepts, sptree_chains, is_concepts_sorted=False, use_tqdm=False)\
+        -> Dict[int, Set[int]]:
     """Return a dict with subconcepts relation on given concepts from given spanning tree of the relation.
 
     Parameters
     ----------
     concepts: `list` of `FormalConcept` or `PatternConcept`
         A list of concepts to compare
     sptree_chains: `list` of `list` of `int`
@@ -412,15 +414,16 @@
             superconcepts = [i for i in superconcepts if i not in all_superconcepts[sc_i]]
         superconcepts_dict[c_i] = superconcepts
         for superconcept_i in superconcepts_dict[c_i]:
             subconcepts_dict[superconcept_i].add(c_i)
     return subconcepts_dict
 
 
-def construct_lattice_by_spanning_tree(concepts, is_concepts_sorted=False, n_jobs=1, use_tqdm=False):
+def construct_lattice_by_spanning_tree(concepts, is_concepts_sorted=False, n_jobs=1, use_tqdm=False)\
+        -> Dict[int, Set[int]]:
     """Return a dict with subconcepts relation on given ``concepts``. Uses spanning tree approach to fasten the computation
 
     Parameters
     ----------
     concepts: `list` of `FormalConcept` or `PatternConcept`
         A list of concepts to compare
     is_concepts_sorted: `bool`
@@ -446,17 +449,39 @@
             concepts, chains, is_concepts_sorted=is_concepts_sorted, use_tqdm=use_tqdm)
     else:
         subconcepts_dict = construct_lattice_from_spanning_tree_parallel(
             concepts, chains, is_concepts_sorted=is_concepts_sorted, n_jobs=n_jobs)
     return subconcepts_dict
 
 
-def add_concept(new_concept, concepts, subconcepts_dict, superconcepts_dict,
-                top_concept_i=None, bottom_concept_i=None,
-                inplace=True):
+def order_extents_comparison(concepts: List[Union[FormalConcept, PatternConcept]]) -> Dict[int, Set[int]]:
+    from caspailleur.order import inverse_order, sort_intents_inclusion, topological_sorting, test_topologically_sorted
+    from caspailleur.base_functions import isets2bas
+
+    n_objects = max(len(c.extent_i) for c in concepts)
+    extents_ba = list(isets2bas([c.extent_i for c in concepts], n_objects))
+    extents_ba_topo, id_to_topo_map = topological_sorting(extents_ba)
+    assert test_topologically_sorted(extents_ba_topo)
+    assert len(extents_ba_topo) == len(extents_ba)
+
+    subconcepts_ba_topo = inverse_order(sort_intents_inclusion(extents_ba_topo))
+
+    topo_to_id_map = {v: k for k, v in enumerate(id_to_topo_map)}
+
+    subconcepts_dict = {topo_to_id_map[i_topo]: {topo_to_id_map[s] for s in subs_topo.itersearch(True)}
+                        for i_topo, subs_topo in enumerate(subconcepts_ba_topo)}
+
+    return subconcepts_dict
+
+
+def add_concept(
+        new_concept, concepts, subconcepts_dict, superconcepts_dict,
+        top_concept_i=None, bottom_concept_i=None,
+        inplace=True
+) -> Tuple[List[Union[FormalConcept, PatternConcept]], Dict[int, Set[int]], Dict[int, Set[int]], int, int]:
     """Add ``new_concept`` into a set of ``concepts`` regarding its subconcept relation
 
     Parameters
     ----------
     new_concept: `FormalConcept` or `PatternConcept`
         A concept to add
     concepts: `list` of `FormalConcept` or `PatternConcept`
@@ -557,17 +582,19 @@
     concepts.append(new_concept)
     superconcepts_dict[new_concept_i] = direct_superconcepts
     subconcepts_dict[new_concept_i] = direct_subconcepts
 
     return concepts, subconcepts_dict, superconcepts_dict, top_concept_i, bottom_concept_i
 
 
-def remove_concept(concept_i, concepts, subconcepts_dict, superconcepts_dict,
-                   top_concept_i=None, bottom_concept_i=None,
-                   inplace=True):
+def remove_concept(
+        concept_i, concepts, subconcepts_dict, superconcepts_dict,
+        top_concept_i=None, bottom_concept_i=None,
+        inplace=True
+) -> Tuple[List[Union[FormalConcept, PatternConcept]], Dict[int, Set[int]], Dict[int, Set[int]], int, int]:
     """Remove a ``concept_i`` from a set of ``concepts`` regarding its subconcept relation
 
     Parameters
     ----------
     concept_i: `int`
         An index of concept to be removed
     concepts: `list` of `FormalConcept` or `PatternConcept`
```

### Comparing `fcapy-0.1.4.1/fcapy/context/__init__.py` & `fcapy-0.1.4.2/fcapy/context/__init__.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.1/fcapy/context/bintable.py` & `fcapy-0.1.4.2/fcapy/context/bintable.py`

 * *Files identical despite different names*

```diff
@@ -4,15 +4,15 @@
 """
 from abc import ABCMeta, abstractmethod
 from typing import List, Tuple, Optional, Collection, Union
 
 from fcapy.context import bintable_errors as berrors
 from fcapy import LIB_INSTALLED
 #if LIB_INSTALLED['bitarray']:
-from bitarray import frozenbitarray as fbarray, bitarray as barray, util as butil
+from bitarray import frozenbitarray as fbarray, util as butil
 
 #if LIB_INSTALLED['numpy']:
 import numpy as np
 import numpy.typing as npt
 
 
 class AbstractBinTable(metaclass=ABCMeta):
@@ -228,15 +228,15 @@
         assert len(data) > 0, "Too small data to decide what class does it belong to"
         if isinstance(data, list) and isinstance(data[0], list):
             return 'BinTableLists'
         if isinstance(data, list) and isinstance(data[0], fbarray):
             return 'BinTableBitarray'
         if isinstance(data, np.ndarray):
             return 'BinTableNumpy'
-        if isinstance(data, tuple) and len(data) == 2 and isinstance(data[0], fbitarray) and isinstance(data[1], int):
+        if isinstance(data, tuple) and len(data) == 2 and isinstance(data[0], fbarray) and isinstance(data[1], int):
             return 'BinTableBitarray'
 
         raise berrors.UnknownDataTypeError(type(data))
 
 
 class BinTableLists(AbstractBinTable):
     data: List[List[bool]]  # Updating type hint
```

### Comparing `fcapy-0.1.4.1/fcapy/context/bintable_errors.py` & `fcapy-0.1.4.2/fcapy/context/bintable_errors.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.1/fcapy/context/converters.py` & `fcapy-0.1.4.2/fcapy/context/converters.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.1/fcapy/context/formal_context.py` & `fcapy-0.1.4.2/fcapy/context/formal_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 This is the main module of subpackage `context`.
 It contains a class FormalContext which represents a Formal Context object from FCA theory
 
 """
 from itertools import combinations
 from numbers import Integral
-from typing import Tuple, Iterable, List, Collection, Set, Union
+from typing import Tuple, Iterable, List, Collection, Union, Iterator
+from bitarray import frozenbitarray as fbarray
 
 from frozendict import frozendict
 import zlib
 
 from fcapy.context.bintable import init_bintable, BINTABLE_CLASSES, AbstractBinTable
 from fcapy.utils.utils import slice_list
 
@@ -707,7 +708,16 @@
         data : `list` of `list` of `bool`
             Binary data of connections between objects and attributes
         attribute_names : `list` of `str`
             Name of attributes from the context
 
         """
         return self._data.to_list(), self._attribute_names
+
+    def to_bin_attr_extents(self) -> Iterator[Tuple[str, fbarray]]:
+        for i, m in enumerate(self.attribute_names):
+            extent = fbarray(self.data[:, i])
+            yield m, extent
+
+    @property
+    def n_bin_attrs(self) -> int:
+        return self.data.width
```

### Comparing `fcapy-0.1.4.1/fcapy/lattice/__init__.py` & `fcapy-0.1.4.2/fcapy/lattice/__init__.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.1/fcapy/lattice/concept_lattice.py` & `fcapy-0.1.4.2/fcapy/lattice/concept_lattice.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,29 +204,28 @@
         """
         if is_monotone:
             return cls._from_context_monotone(context, algo, **kwargs)
 
         if algo is None:
             algo = 'CbO' if type(context) == MVContext else 'Lindig'
 
-        if algo in {'CbO', 'RandomForest'}:
-            algo_func = {'CbO': cca.close_by_one, 'RandomForest': cca.random_forest_concepts}[algo]
+        if algo in {'CbO', 'RandomForest', 'Sofia', 'LCM'}:
+            algo_func = {'CbO': cca.close_by_one, 'RandomForest': cca.random_forest_concepts,
+                         'Sofia': cca.sofia, 'LCM': cca.lcm_skmine}[algo]
             kwargs_used = utils.get_kwargs_used(kwargs, algo_func)
             concepts = algo_func(context, **kwargs_used)
             concepts = cls.sort_concepts(concepts)
-            subconcepts_dict = lca.construct_lattice_by_spanning_tree(concepts, is_concepts_sorted=True)
+            subconcepts_dict = lca.order_extents_comparison(concepts)
 
             ltc = ConceptLattice(
                 concepts=concepts, subconcepts_dict=subconcepts_dict
             )
 
-        elif algo in {'Sofia', 'Lindig'}:
-            if algo == 'Sofia':
-                algo_func = cca.sofia_general if type(context) == MVContext else cca.sofia_binary
-            elif algo == 'Lindig':
+        elif algo in {'Lindig'}:
+            if algo == 'Lindig':
                 algo_func = cca.lindig_algorithm
             else:
                 raise NotImplementedError("Error. Some unknown algo seen")
 
             kwargs_used = utils.get_kwargs_used(kwargs, algo_func)
             ltc = algo_func(context, **kwargs_used)
 
@@ -301,34 +300,39 @@
         """Calculate the values of ``measure`` for each concept in a lattice
 
         The calculated measure values are stored in ``measures`` property
         of each ``concept`` from ``ConceptLattice.elements``
 
         Parameters
         ----------
-        measure: `str` in {'stability_bounds', 'LStab', 'UStab', 'stability', 'target_entropy', 'mean_information_gain'}
+        measure: `str` in {'stability_bounds', 'LStab', 'UStab', 'stability', 'log_stability_lbound',
+            'target_entropy', 'mean_information_gain'}
             The name of the measure to compute
         context: `FormalContext` or `MVContext`
             The context is used when calculating 'stability' measure
         Returns
         -------
         None
 
         """
         # TODO: Reflect these measures in the docstring
-        possible_measures = ['stability_bounds', 'LStab', 'UStab', 'stability',
+        possible_measures = ['stability_bounds', 'LStab', 'UStab', 'stability', 'log_stability_lbound',
                              'target_entropy', 'mean_information_gain']
 
         from fcapy.lattice import concept_measures as cms
 
         if measure in ('stability_bounds', 'LStab', 'UStab'):
             for c_i, c in enumerate(self):
                 lb, ub = cms.stability_bounds(c_i, self)
                 c.measures['LStab'] = lb
                 c.measures['UStab'] = ub
+        elif measure == 'log_stability_lbound':
+            n_bin_attrs = context.n_bin_attrs
+            for c_i, c in enumerate(self):
+                c.measures['log_stability_lbound'] = cms.log_stability_lbound(c_i, self, n_bin_attrs)
         elif measure == 'stability':
             warnings.warn("Calculation of concept stability index takes exponential time. "
                           "One better use its approximate measure `stability_bounds`")
             assert context is not None, 'ConceptLattice.calc_concepts_measures failed. ' \
                                         'Please specify `context` parameter to calculate the stability'
             for c_i, c in enumerate(self):
                 s = cms.stability(c_i, self, context)
@@ -796,16 +800,18 @@
 
         lattice_metadata = {
             'Top': [self.top], "Bottom": [self.bottom],
             "NodesCount": len(self), "ArcsCount": len(arcs)
         }
         if isinstance(self[0], PatternConcept):
             to_dict_kwargs = dict(json_ready=True)
-        else:  # if FormalConcept
+        elif isinstance(self[0], FormalConcept):  # if FormalConcept
             to_dict_kwargs = dict(objs_order=objs_order, attrs_order=attrs_order)
+        else:
+            raise TypeError(f'Lattice element format is neither PatternConcept nor FormalConcept but {type(self[0])}')
         nodes_data = {"Nodes": [c.to_dict(**to_dict_kwargs) for c in self]}
         arcs_data = {"Arcs": arcs}
         file_data = [lattice_metadata, nodes_data, arcs_data]
         json_data = json.dumps(file_data)
 
         if path is None:
             return json_data
```

### Comparing `fcapy-0.1.4.1/fcapy/lattice/concept_measures.py` & `fcapy-0.1.4.2/fcapy/lattice/concept_measures.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,18 +9,21 @@
 
 For the definition of stability and its bounds look the paper:
 
 Buzmakov, Aleksey & Kuznetsov, Sergei & Napoli, Amedeo. (2014). Scalable Estimates of Concept Stability.
 8478. 10.1007/978-3-319-07248-7_12.
 
 """
+import math
 
 from fcapy.lattice.concept_lattice import ConceptLattice
 from fcapy.context.formal_context import FormalContext
 from fcapy.utils.utils import powerset
+from math import log2
+
 
 from fcapy import LIB_INSTALLED
 if LIB_INSTALLED['numpy']:
     import numpy as np
 
 
 def stability(c_i, lattice: ConceptLattice, context: FormalContext):
@@ -55,14 +58,25 @@
         inv_diff = [2 ** (-len(set(c.extent_i) - set(lattice[child_i].extent_i))) for child_i in children_i]
 
     lb = 1 - sum(inv_diff)
     ub = 1 - max(inv_diff)
     return lb, ub
 
 
+def log_stability_lbound(c_i, lattice: ConceptLattice, n_bin_attrs: int) -> float:
+    extent_i = set(lattice[c_i].extent_i)
+    children_i = lattice.children(c_i)
+    if children_i:
+        bound = min(len(extent_i - set(lattice[child_i].extent_i)) for child_i in children_i)
+    else:
+        bound = math.inf
+    bound -= log2(n_bin_attrs)
+    return bound
+
+
 def target_entropy(c_i, lattice: ConceptLattice, context: FormalContext):
     """Compute the entropy of target labels of objects from concept extent"""
     target_ext = context.target[list(lattice[c_i].extent_i)]
     return np.var(target_ext)
 
 
 def mean_information_gain(c_i, lattice: ConceptLattice):
```

### Comparing `fcapy-0.1.4.1/fcapy/lattice/formal_concept.py` & `fcapy-0.1.4.2/fcapy/lattice/formal_concept.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.1/fcapy/lattice/pattern_concept.py` & `fcapy-0.1.4.2/fcapy/lattice/pattern_concept.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.1/fcapy/ml/__init__.py` & `fcapy-0.1.4.2/fcapy/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.1/fcapy/ml/decision_based_model.py` & `fcapy-0.1.4.2/fcapy/ml/decision_based_model.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.1/fcapy/ml/decision_lattice.py` & `fcapy-0.1.4.2/fcapy/ml/decision_lattice.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.1/fcapy/ml/decision_poset_structure.py` & `fcapy-0.1.4.2/fcapy/ml/decision_poset_structure.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.1/fcapy/mvcontext/__init__.py` & `fcapy-0.1.4.2/fcapy/mvcontext/__init__.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.1/fcapy/mvcontext/mvcontext.py` & `fcapy-0.1.4.2/fcapy/mvcontext/mvcontext.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 This module implements the class MVContext which is used to represent a Many Valued Context from FCA theory
 
 """
 from collections.abc import Iterable
 from frozendict import frozendict
 from itertools import combinations
 import zlib
-from typing import Tuple
+from typing import Tuple, Iterator, List
 import json
+from bitarray import frozenbitarray as fbarray
 
 from fcapy import LIB_INSTALLED
+from fcapy.context import FormalContext
 from fcapy.mvcontext import pattern_structure as PS
 
 
 if LIB_INSTALLED['numpy']:
     import numpy as np
 
 
@@ -91,15 +93,15 @@
         assert len(value) == self._n_attributes,\
             'MVContext.attribute_names.setter: Length of "value" should match length of data[0]'
         assert all(type(name) == str for name in value),\
             'MVContext.object_names.setter: Object names should be of type str'
         self._attribute_names = value
 
     @property
-    def pattern_structures(self):
+    def pattern_structures(self) -> List[PS.AbstractPS]:
         """A list of pattern structures kept in a context"""
         return self._pattern_structures
 
     @pattern_structures.setter
     def pattern_structures(self, value):
         self._pattern_structures = value
 
@@ -109,15 +111,15 @@
         return self._pattern_types
 
     @property
     def target(self):
         """A list of target values for Supervised ML scenarios"""
         return self._target
 
-    def assemble_pattern_structures(self, data, pattern_types):
+    def assemble_pattern_structures(self, data, pattern_types) -> List[PS.AbstractPS]:
         """Return pattern_structures based on ``data`` and the ``pattern_types``"""
         if data is None:
             return None
 
         if pattern_types is not None:
             defined_patterns = set([attr_name for attr_names in pattern_types.keys()
                                     for attr_name in (attr_names if type(attr_names) != str else [attr_names])])
@@ -296,15 +298,15 @@
 
         Parameters
         ----------
         path: `str`
             A path to .json file
         json_data: `str`
             A json encoded data
-        pattern_types: `tuple[AbstractPS]`
+        pattern_types: `Tuple[AbstractPS]`
             Tuple of additional Pattern Structures not defined in fcapy.mvcontext.pattern_structure
 
         Returns
         -------
         mvK: `MVContext`
 
         """
@@ -594,7 +596,30 @@
         """Check If description `a` is 'smaller' (more general) then description `b`"""
         for ps_i, descr in a.items():
             if ps_i not in b:
                 continue
             if not self._pattern_structures[ps_i].leq_descriptions(descr, b[ps_i]):
                 return False
         return True
+
+    def describe_pattern(self, data: dict) -> str:
+        pattern_names = [ps.name for ps in self.pattern_structures]
+        data_i = {pattern_names.index(k): v for k, v in data.items()}
+        description = [self.pattern_structures[i].describe_pattern(v) for i, v in data_i.items()]
+        description = [descr for descr in description if descr]
+        return '; '.join(description)
+
+    def to_bin_attr_extents(self) -> Iterator[Tuple[str, fbarray]]:
+        for ps_i, ps in enumerate(self.pattern_structures):
+            for m, extent in ps.to_bin_attr_extents():
+                yield m, extent
+
+    def binarize(self) -> FormalContext:
+        attr_names, attr_extents = zip(*list(self.to_bin_attr_extents()))
+        K = FormalContext(list(attr_extents)).T
+        K.object_names = self.object_names
+        K.attribute_names = attr_names
+        return K
+
+    @property
+    def n_bin_attrs(self) -> int:
+        return sum(ps.n_bin_attrs for ps in self.pattern_structures)
```

### Comparing `fcapy-0.1.4.1/fcapy/poset/__init__.py` & `fcapy-0.1.4.2/fcapy/poset/__init__.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.1/fcapy/poset/lattice.py` & `fcapy-0.1.4.2/fcapy/poset/lattice.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.1/fcapy/poset/poset.py` & `fcapy-0.1.4.2/fcapy/poset/poset.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.1/fcapy/poset/tree.py` & `fcapy-0.1.4.2/fcapy/poset/tree.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.1/fcapy/utils/utils.py` & `fcapy-0.1.4.2/fcapy/utils/utils.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.1/fcapy/visualizer/__init__.py` & `fcapy-0.1.4.2/fcapy/visualizer/__init__.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.1/fcapy/visualizer/line_layouts.py` & `fcapy-0.1.4.2/fcapy/visualizer/line_layouts.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.1/fcapy/visualizer/line_visualizers.py` & `fcapy-0.1.4.2/fcapy/visualizer/line_visualizers.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.1/fcapy/visualizer/measures.py` & `fcapy-0.1.4.2/fcapy/visualizer/measures.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.1/fcapy/visualizer/mover.py` & `fcapy-0.1.4.2/fcapy/visualizer/mover.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Dict, Tuple, List, Optional
 
-from attr import dataclass
+from dataclasses import dataclass
 
 from fcapy.poset import POSet
 from fcapy.visualizer.line_layouts import LAYOUTS
 from fcapy.utils.utils import get_kwargs_used
 
 PosDictType = Dict[int, Tuple[float, float]]
```

### Comparing `fcapy-0.1.4.1/fcapy/visualizer/visualizer.py` & `fcapy-0.1.4.2/fcapy/visualizer/visualizer.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.1/tests/algorithms/test_lattice_construction.py` & `fcapy-0.1.4.2/tests/algorithms/test_lattice_construction.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,18 +115,24 @@
         'lattice_construction.construct_lattice_by_spanning_tree failed.' \
         'Parallel computing give wrong result when concepts are sorted'
     assert sub_with_sptree_unsort == sub_parallel_unsort, \
         'lattice_construction.construct_lattice_by_spanning_tree failed.' \
         'Parallel computing give wrong result when concepts are not sorted'
 
 
+def test_order_extent_comparison():
+    ctx = read_cxt('data/animal_movement.cxt')
+    concepts = list(ConceptLattice.from_context(ctx))
+    assert lca.complete_comparison(concepts) == lca.order_extents_comparison(concepts)
+
+
 def test_add_concept():
     ctx = read_csv('data/mango_bin.csv')
     np.random.seed(13)
-    concepts_true = cca.close_by_one(ctx)
+    concepts_true = list(cca.close_by_one(ctx))
     np.random.shuffle(concepts_true)
     top_concept_i, bottom_concept_i = ConceptLattice.get_top_bottom_concepts_i(concepts_true)
     concepts_true = [concepts_true[top_concept_i], concepts_true[bottom_concept_i]] + \
                [c for c_i, c in enumerate(concepts_true) if c_i not in [top_concept_i, bottom_concept_i]]
 
     subconcepts_dict_true = lca.complete_comparison(concepts_true)
     superconcepts_dict_true = ConceptLattice._transpose_hierarchy(subconcepts_dict_true)
@@ -180,16 +186,16 @@
     assert set(concepts) == set(concepts_true), error_msg
     assert subconcepts_dict == subconcepts_dict_true, error_msg
     assert superconcepts_dict == superconcepts_dict_true, error_msg
 
 
 def test_remove_concept():
     ctx = read_csv('data/mango_bin.csv')
-    concepts_true = cca.close_by_one(ctx)
-    concepts_true1 = cca.close_by_one(ctx)
+    concepts_true = list(cca.close_by_one(ctx))
+    concepts_true1 = list(cca.close_by_one(ctx))
     np.random.seed(13)
     np.random.shuffle(concepts_true)
     np.random.seed(13)
     np.random.shuffle(concepts_true1)
     top_concept_i, bottom_concept_i = ConceptLattice.get_top_bottom_concepts_i(concepts_true)
 
     subconcepts_dict_true = lca.complete_comparison(concepts_true)
```

### Comparing `fcapy-0.1.4.1/tests/context/data_to_test.py` & `fcapy-0.1.4.2/tests/context/data_to_test.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.1/tests/context/test_bintable.py` & `fcapy-0.1.4.2/tests/context/test_bintable.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.1/tests/context/test_converters.py` & `fcapy-0.1.4.2/tests/context/test_converters.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.1/tests/context/test_formal_context.py` & `fcapy-0.1.4.2/tests/context/test_formal_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import pytest
 import os
 from operator import itemgetter
 import filecmp
 
+from bitarray import frozenbitarray
+
 from fcapy.context import FormalContext, read_cxt, read_json, read_csv, from_pandas
 from fcapy.lattice.concept_lattice import ConceptLattice
 from .data_to_test import animal_movement_data
 
 
 def test_data_property(animal_movement_data):
     K = FormalContext()
@@ -293,7 +295,12 @@
         ctx.get_minimal_generators(c.intent)
 
 
 def test_invert():
     ctx = read_csv('data/mango_bin.csv')
     assert ~~ctx == ctx, 'FormalContext.__invert__ failed'
 
+
+def test_to_bin_attr_extents():
+    K = FormalContext([[False, False, True], [False, True, True]], attribute_names=['a', 'b', 'c'])
+    bin_attr_extents_true = [('a', frozenbitarray('00')), ('b', frozenbitarray('01')), ('c', frozenbitarray('11'))]
+    assert list(K.to_bin_attr_extents()) == bin_attr_extents_true
```

### Comparing `fcapy-0.1.4.1/tests/lattice/test_concept_lattice.py` & `fcapy-0.1.4.2/tests/lattice/test_concept_lattice.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,35 +50,45 @@
         c4 = FormalConcept((1,), ('b',), (1,), ('b',), context_hash=context_hash)
         concepts = [c1, c2, c3, c4]
 
         assert set(ltc) == set(concepts),\
             'ConceptLattice.from_context failed. Wrong concepts in the constructed lattice'
 
     ctx = converters.read_csv('data/mango_bin.csv')
-    ltc_cbo, ltc_sofia, ltc_lindig = [ConceptLattice.from_context(ctx, algo=alg_name)
-                                      for alg_name in ['CbO', 'Sofia', 'Lindig']]
-    for L in [ltc_cbo, ltc_sofia, ltc_lindig]:
+    ltc_cbo, ltc_sofia, ltc_lindig, ltc_LCM = [ConceptLattice.from_context(ctx, algo=alg_name)
+                                      for alg_name in ['CbO', 'Sofia', 'Lindig', 'LCM']]
+    for c in list(ltc_sofia):
+        ltc_sofia._update_element(
+            c, FormalConcept(c.extent_i, c.extent, c.intent_i, c.intent, context_hash=ctx.hash_fixed()))
+    for L in [ltc_cbo, ltc_sofia, ltc_lindig, ltc_LCM]:
         assert all([idx == L.index(el) for idx, el in enumerate(L)]),\
             "ConceptLattice.from_context failed. Something is wrong with lattice.index function"
-    for L in [ltc_sofia, ltc_lindig]:
+    for L in [ltc_sofia, ltc_lindig, ltc_LCM]:
         assert ltc_cbo == L, "ConceptLattice.from_context failed. Lattices differ when constructed by different methods"
 
     data = [[1, 10],
             [2, 22],
             [3, 100],
             [4, 60]]
     object_names = ['a', 'b', 'c', 'd']
     attribute_names = ['M1', 'M2']
     pattern_types = {'M1': ps.IntervalPS, 'M2': ps.IntervalPS}
     mvctx = mvcontext.MVContext(data, pattern_types, object_names, attribute_names)
-    ltc_cbo, ltc_sofia = [ConceptLattice.from_context(mvctx, algo=alg_name) for alg_name in ['CbO', 'Sofia']]
-    for L in [ltc_cbo, ltc_sofia]:
+    ltc_cbo, ltc_sofia, ltc_LCM = [ConceptLattice.from_context(mvctx, algo=alg_name) for alg_name in ['CbO', 'Sofia', 'LCM']]
+
+    from fcapy.lattice.pattern_concept import PatternConcept
+    for c in list(ltc_sofia):
+        ltc_sofia._update_element(
+            c, PatternConcept(c.extent_i, c.extent, c.intent_i, c.intent,
+                              mvctx.pattern_types, mvctx.attribute_names, context_hash=mvctx.hash_fixed()))
+
+    for L in [ltc_cbo, ltc_sofia, ltc_LCM]:
         assert all([idx == L.index(el) for idx, el in enumerate(L)]),\
             "ConceptLattice.from_context failed. Something is wrong with lattice.index function"
-    for L in [ltc_sofia]:
+    for L in [ltc_sofia, ltc_LCM]:
         assert ltc_cbo == L, "ConceptLattice.from_context failed. Lattices differ when constructed by different methods"
 
     with pytest.raises(NotImplementedError):
         ConceptLattice.from_context(mvctx, algo='Lindig')
 
     with pytest.raises(ValueError):
         ConceptLattice.from_context(mvctx, algo='OtHeR MeThOd')
@@ -232,15 +242,15 @@
         "ConceptLattice.get_chains failed. The result changes with is_concepts_sorted parameter"
 
 
 def test_add_concept():
     ctx = converters.read_csv('data/mango_bin.csv')
     from fcapy.algorithms import concept_construction as cca, lattice_construction as lca
 
-    concepts = cca.close_by_one(ctx)
+    concepts = list(cca.close_by_one(ctx))
     np.random.shuffle(concepts)
     top_concept_i, bottom_concept_i = ConceptLattice.get_top_bottom_concepts_i(concepts)
     concepts = [concepts[top_concept_i], concepts[bottom_concept_i]] + \
                [c for c_i, c in enumerate(concepts) if c_i not in [top_concept_i, bottom_concept_i]]
     ltc = ConceptLattice(concepts[:2],
                          children_dict={0: {1}, 1: set()})
```

### Comparing `fcapy-0.1.4.1/tests/lattice/test_concept_measures.py` & `fcapy-0.1.4.2/tests/lattice/test_concept_measures.py`

 * *Files 18% similar despite different names*

```diff
@@ -28,7 +28,22 @@
 
     # TODO: Check why stability bounds are not fully match the ones from latviz.loria.ft
     mae = sum([abs(lstabs_true[c_i]-lstabs_est[c_i])
                if len(c.extent_i) > 0 else 0 for c_i, c in enumerate(ltc)]
               )/len(lstabs_true)
     assert mae < 0.05, "concept_measure.stability_bounds failed. " \
                        "Lower stability bounds of concepts does not match the ones computed by latviz.loria.ft"
+
+
+def test_log_stability_lbound():
+    ctx = read_json('data/animal_movement.json')
+    ltc = ConceptLattice.read_json('data/animal_movement_lattice.json')
+    lstabs_true = [c.measures.get('LStab') for c in ltc]
+    
+    ltc.calc_concepts_measures('log_stability_lbound', ctx)
+    lstabs_est = [c.measures.get('LStab') for c in ltc]
+
+    mae = sum(abs(lstabs_true[c_i] - lstabs_est[c_i]) if len(c.extent_i) > 0 else 0 for c_i, c in enumerate(ltc))
+    mae /= len(lstabs_true)
+    assert mae < 0.05, "concept_measure.stability_bounds failed. " \
+                       "Lower stability bounds of concepts does not match the ones computed by latviz.loria.ft"
+
```

### Comparing `fcapy-0.1.4.1/tests/lattice/test_formal_concept.py` & `fcapy-0.1.4.2/tests/lattice/test_formal_concept.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.1/tests/lattice/test_pattern_concept.py` & `fcapy-0.1.4.2/tests/lattice/test_pattern_concept.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.1/tests/ml/test_decision_lattice.py` & `fcapy-0.1.4.2/tests/ml/test_decision_lattice.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import pytest
-from fcapy.lattice.concept_lattice import ConceptLattice
 from fcapy.ml import decision_lattice as dl
 from fcapy.mvcontext.mvcontext import MVContext
 from fcapy.mvcontext import pattern_structure as ps
 
 import numpy as np
-from sklearn.datasets import load_iris, load_boston
+from sklearn.datasets import load_iris
 from sklearn.metrics import accuracy_score, mean_squared_error, mean_absolute_error
 from sklearn.tree import DecisionTreeRegressor
 from sklearn.ensemble import RandomForestRegressor, GradientBoostingRegressor
 from xgboost import XGBRegressor
 
 
 def test_dlpredictor():
@@ -47,25 +46,27 @@
     dlc.fit(mvctx_train)
 
     assert dlc.class_names == sorted(set(Y)), "DecisionLatticeClassifier.class_names failed"
 
     preds_train = dlc.predict(mvctx_train)
     preds_test = dlc.predict(mvctx_test)
     acc_train, acc_test = accuracy_score(y_train, preds_train), accuracy_score(y_test, preds_test)
-    assert acc_train > 0.44, f"DecisionLatticeClassifier failed. To low train quality {acc_train}"
-    assert acc_train > 0.44, f"DecisionLatticeClassifier failed. To low test quality {acc_test}"
+    assert acc_train > 0.42, f"DecisionLatticeClassifier failed. To low train quality {acc_train}"
+    assert acc_test > 0.33, f"DecisionLatticeClassifier failed. To low test quality {acc_test}"
 
     probs_train = np.array(dlc.predict_proba(mvctx_train))
     assert np.array(probs_train).sum(1).mean(),\
         "DecisionLatticeClassifier.predict_proba failed. Probabilities does not sum to 1"
     assert np.mean(np.argmax(probs_train, 1) == preds_train) == 1,\
         "DecisionLatticeClassifier.predict_proba failed. Probability predictions does not match class predictions"
 
 
+@pytest.mark.skip(reason="Load boston function has been removed. Should rewrite the test for another dataset")
 def test_dlregressor():
+    from sklearn.datasets import load_boston
     boston_data = load_boston()
     X_boston = boston_data['data'][:10]
     y_boston = boston_data['target'][:10]
     features_boston = [str(f) for f in boston_data['feature_names']]
 
     np.random.seed(42)
     train_idxs = np.random.choice(range(len(X_boston)), size=int(len(X_boston) * 0.8), replace=False)
@@ -84,15 +85,18 @@
     preds_test = dlc.predict(mvctx_test)
     preds_test = [p if p is not None else np.mean(y_train) for p in preds_test]
     mse_train, mse_test = mean_squared_error(y_train, preds_train), mean_squared_error(y_test, preds_test)
     assert mse_train < 1, f"DecisionLatticeRegressor failed. To low train quality {mse_train}"
     assert mse_test < 29, f"DecisionLatticeRegressor failed. To low test quality {mse_test}"
 
 
+@pytest.mark.skip(reason="Load boston function has been removed. Should rewrite the test for another dataset")
 def test_dlr_from_dtrees():
+    from sklearn.datasets import load_boston
+
     boston_data = load_boston()
     X_boston = boston_data['data'][:100]
     y_boston = boston_data['target'][:100]
     features_boston = [str(f) for f in boston_data['feature_names']]
 
     np.random.seed(42)
     train_idxs = np.random.choice(range(len(X_boston)), size=int(len(X_boston) * 0.8), replace=False)
```

### Comparing `fcapy-0.1.4.1/tests/mvcontext/test_mvcontext.py` & `fcapy-0.1.4.2/tests/mvcontext/test_mvcontext.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import pytest
+from bitarray import frozenbitarray
+
 from fcapy.mvcontext import mvcontext, pattern_structure as PS
 from fcapy.lattice.concept_lattice import ConceptLattice
 import math
 from frozendict import frozendict
-from fcapy import LIB_INSTALLED
+from fcapy import LIB_INSTALLED, context
 import numpy as np
 from sklearn.datasets import load_breast_cancer
 
 
 def test_init():
     mvctx = mvcontext.MVContext()
 
@@ -235,7 +237,47 @@
     c_i = 3
     subc_i = sorted(ltc.children_dict[c_i])[0]
     mg1 = mvctx.generators_by_intent_difference(ltc[subc_i].intent_i, ltc[c_i].intent_i)
     mg2 = mvctx.get_minimal_generators(ltc[subc_i].intent_i, base_objects=list(ltc[c_i].extent_i),
                                        use_indexes=True)
 
     assert set(mg1) == set(mg2), "MVContext.generators_by_intent_difference failed"
+
+
+def test_to_bin_attr_extents():
+    ptypes = {'attr': PS.AttributePS, 'sps': PS.SetPS, 'ips': PS.IntervalPS}
+    data = [[True, 'a', 1], [False, 'b', 2]]
+    K = mvcontext.MVContext(data, pattern_types=ptypes, attribute_names=['attr', 'sps', 'ips'])
+
+    bin_attrs_true = [
+        ('attr', frozenbitarray('10')),
+        ('sps: a, b', frozenbitarray('11')),
+        ('sps: a', frozenbitarray('10')),
+        ('sps: b', frozenbitarray('01')),
+        ('sps: ∅', frozenbitarray('00')),
+        ('ips: (1.0, 2.0)', frozenbitarray('11')),
+        ('ips: (2.0, 2.0)', frozenbitarray('01')),
+        ('ips: (1.0, 1.0)', frozenbitarray('10')),
+        ('ips: ∅',      frozenbitarray('00')),
+    ]
+    assert list(K.to_bin_attr_extents()) == bin_attrs_true
+
+
+def test_to_binarize():
+    ptypes = {'attr': PS.AttributePS, 'sps': PS.SetPS, 'ips': PS.IntervalPS}
+    data = [[True, 'a', 1], [False, 'b', 2]]
+    mvK = mvcontext.MVContext(data, pattern_types=ptypes, attribute_names=['attr', 'sps', 'ips'])
+
+    bin_data_true = [[True, True, True, False, False, True, False, True, False],
+                     [False, True, False, True, False, True, True, False, False]]
+    attr_names_true = ['attr', 'sps: a, b', 'sps: a', 'sps: b', 'sps: ∅',
+                  'ips: (1.0, 2.0)', 'ips: (2.0, 2.0)', 'ips: (1.0, 1.0)', 'ips: ∅']
+    K_true = context.FormalContext(bin_data_true, object_names=mvK.object_names, attribute_names=attr_names_true)
+    assert mvK.binarize()
+    assert mvK.binarize() == K_true
+
+
+def test_n_bin_attrs():
+    ptypes = {'attr': PS.AttributePS, 'sps': PS.SetPS, 'ips': PS.IntervalPS}
+    data = [[True, 'a', 1], [False, 'b', 2]]
+    mvK = mvcontext.MVContext(data, pattern_types=ptypes, attribute_names=['attr', 'sps', 'ips'])
+    assert mvK.n_bin_attrs == mvK.binarize().n_bin_attrs
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fcapy-0.1.4.1/tests/poset/test_lattice.py` & `fcapy-0.1.4.2/tests/poset/test_lattice.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.1/tests/poset/test_poset.py` & `fcapy-0.1.4.2/tests/poset/test_poset.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.1/tests/test_init.py` & `fcapy-0.1.4.2/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.1/tests/utils/test_utils.py` & `fcapy-0.1.4.2/tests/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.1/tests/visualizer/test_line_layouts.py` & `fcapy-0.1.4.2/tests/visualizer/test_line_layouts.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.1/tests/visualizer/test_line_visualizers.py` & `fcapy-0.1.4.2/tests/visualizer/test_line_visualizers.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.1/tests/visualizer/test_measures.py` & `fcapy-0.1.4.2/tests/visualizer/test_measures.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.1/tests/visualizer/test_mover.py` & `fcapy-0.1.4.2/tests/visualizer/test_mover.py`

 * *Files identical despite different names*

### Comparing `fcapy-0.1.4.1/tests/visualizer/test_visualizer.py` & `fcapy-0.1.4.2/tests/visualizer/test_visualizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     vsl = visualizer.ConceptLatticeVisualizer(ltc)
     vsl.draw_networkx(draw_node_indices=True)
 
     vsl = visualizer.POSetVisualizer(ltc)
     vsl.draw_networkx(draw_node_indices=True)
 
 
+@pytest.mark.skip(reason="Outdated functionality that causes Github actions problems")
 def test_draw_plotly():
     path = 'data/animal_movement.json'
     ctx = converters.read_json(path)
     ltc = ConceptLattice.from_context(ctx)
 
     vsl = visualizer.ConceptLatticeVisualizer(ltc)
     vsl.draw_plotly()
```

