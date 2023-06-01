# Comparing `tmp/pycobertura-3.2.0.tar.gz` & `tmp/pycobertura-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycobertura-3.2.0.tar", last modified: Sat May 13 04:10:13 2023, max compression
+gzip compressed data, was "pycobertura-3.2.1.tar", last modified: Thu Jun  1 09:02:24 2023, max compression
```

## Comparing `pycobertura-3.2.0.tar` & `pycobertura-3.2.1.tar`

### file list

```diff
@@ -1,137 +1,137 @@
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-05-13 04:10:13.571233 pycobertura-3.2.0/
--rw-r--r--   0 alexandre   (501) staff       (20)       32 2022-10-07 08:01:13.000000 pycobertura-3.2.0/.coveragerc
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-05-13 04:10:13.548811 pycobertura-3.2.0/.github/
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-05-13 04:10:13.552763 pycobertura-3.2.0/.github/workflows/
--rw-r--r--   0 alexandre   (501) staff       (20)      642 2022-03-20 16:09:41.000000 pycobertura-3.2.0/.github/workflows/build-and-test-pycobertura.yml
--rw-r--r--   0 alexandre   (501) staff       (20)      604 2022-03-03 22:33:26.000000 pycobertura-3.2.0/.gitignore
--rw-r--r--   0 alexandre   (501) staff       (20)    15532 2023-05-13 04:09:27.000000 pycobertura-3.2.0/CHANGES.md
--rw-r--r--   0 alexandre   (501) staff       (20)     1103 2022-03-03 22:33:26.000000 pycobertura-3.2.0/LICENSE
--rw-r--r--   0 alexandre   (501) staff       (20)    24292 2023-05-13 04:10:13.571343 pycobertura-3.2.0/PKG-INFO
--rw-r--r--   0 alexandre   (501) staff       (20)    23306 2023-05-13 04:07:52.000000 pycobertura-3.2.0/README.md
--rw-r--r--   0 alexandre   (501) staff       (20)        6 2023-05-13 04:08:58.000000 pycobertura-3.2.0/__version__
--rw-r--r--   0 alexandre   (501) staff       (20)     2697 2022-01-04 01:58:44.000000 pycobertura-3.2.0/aysha-logo.svg
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-05-13 04:10:13.556563 pycobertura-3.2.0/images/
--rw-r--r--   0 alexandre   (501) staff       (20)    30894 2022-03-03 22:33:26.000000 pycobertura-3.2.0/images/example_csv_diff_output.png
--rw-r--r--   0 alexandre   (501) staff       (20)   172765 2023-05-13 04:07:52.000000 pycobertura-3.2.0/images/example_github_annotation_diff.png
--rw-r--r--   0 alexandre   (501) staff       (20)   103005 2023-04-29 17:28:15.000000 pycobertura-3.2.0/images/example_github_annotation_show.png
--rw-r--r--   0 alexandre   (501) staff       (20)    61287 2022-03-03 22:33:26.000000 pycobertura-3.2.0/images/example_json_output.png
--rw-r--r--   0 alexandre   (501) staff       (20)    53710 2022-03-03 22:33:26.000000 pycobertura-3.2.0/images/example_markdown_diff_output.png
--rw-r--r--   0 alexandre   (501) staff       (20)    45822 2022-03-03 22:33:26.000000 pycobertura-3.2.0/images/example_yaml_output.png
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-05-13 04:10:13.558408 pycobertura-3.2.0/pycobertura/
--rw-r--r--   0 alexandre   (501) staff       (20)      119 2022-01-04 01:58:44.000000 pycobertura-3.2.0/pycobertura/__init__.py
--rw-r--r--   0 alexandre   (501) staff       (20)     9607 2023-05-13 04:07:52.000000 pycobertura-3.2.0/pycobertura/cli.py
--rw-r--r--   0 alexandre   (501) staff       (20)    15355 2022-10-24 18:43:16.000000 pycobertura-3.2.0/pycobertura/cobertura.py
--rw-r--r--   0 alexandre   (501) staff       (20)     4886 2023-04-29 17:12:17.000000 pycobertura-3.2.0/pycobertura/filesystem.py
--rw-r--r--   0 alexandre   (501) staff       (20)      203 2023-04-05 07:16:26.000000 pycobertura-3.2.0/pycobertura/merge.py
--rw-r--r--   0 alexandre   (501) staff       (20)    17838 2023-05-13 04:07:52.000000 pycobertura-3.2.0/pycobertura/reporters.py
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-05-13 04:10:13.560701 pycobertura-3.2.0/pycobertura/templates/
--rw-r--r--   0 alexandre   (501) staff       (20)        0 2022-01-04 01:58:44.000000 pycobertura-3.2.0/pycobertura/templates/__init__.py
--rw-r--r--   0 alexandre   (501) staff       (20)      624 2022-10-07 08:01:13.000000 pycobertura-3.2.0/pycobertura/templates/filters.py
--rw-r--r--   0 alexandre   (501) staff       (20)     2805 2022-03-04 19:55:00.000000 pycobertura-3.2.0/pycobertura/templates/html-delta.jinja2
--rw-r--r--   0 alexandre   (501) staff       (20)     1764 2022-03-03 22:33:26.000000 pycobertura-3.2.0/pycobertura/templates/html.jinja2
--rw-r--r--   0 alexandre   (501) staff       (20)      473 2022-01-04 01:58:44.000000 pycobertura-3.2.0/pycobertura/templates/macro.source.jinja2
--rw-r--r--   0 alexandre   (501) staff       (20)     7797 2022-01-04 01:58:44.000000 pycobertura-3.2.0/pycobertura/templates/normalize.css
--rw-r--r--   0 alexandre   (501) staff       (20)    11452 2022-01-04 01:58:44.000000 pycobertura-3.2.0/pycobertura/templates/skeleton.css
--rw-r--r--   0 alexandre   (501) staff       (20)     7151 2022-10-07 23:42:24.000000 pycobertura-3.2.0/pycobertura/utils.py
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-05-13 04:10:13.559466 pycobertura-3.2.0/pycobertura.egg-info/
--rw-r--r--   0 alexandre   (501) staff       (20)    24292 2023-05-13 04:10:13.000000 pycobertura-3.2.0/pycobertura.egg-info/PKG-INFO
--rw-r--r--   0 alexandre   (501) staff       (20)     3405 2023-05-13 04:10:13.000000 pycobertura-3.2.0/pycobertura.egg-info/SOURCES.txt
--rw-r--r--   0 alexandre   (501) staff       (20)        1 2023-05-13 04:10:13.000000 pycobertura-3.2.0/pycobertura.egg-info/dependency_links.txt
--rw-r--r--   0 alexandre   (501) staff       (20)       60 2023-05-13 04:10:13.000000 pycobertura-3.2.0/pycobertura.egg-info/entry_points.txt
--rw-r--r--   0 alexandre   (501) staff       (20)        1 2022-03-04 19:49:40.000000 pycobertura-3.2.0/pycobertura.egg-info/not-zip-safe
--rw-r--r--   0 alexandre   (501) staff       (20)       44 2023-05-13 04:10:13.000000 pycobertura-3.2.0/pycobertura.egg-info/requires.txt
--rw-r--r--   0 alexandre   (501) staff       (20)       12 2023-05-13 04:10:13.000000 pycobertura-3.2.0/pycobertura.egg-info/top_level.txt
--rw-r--r--   0 alexandre   (501) staff       (20)      122 2022-03-03 22:33:26.000000 pycobertura-3.2.0/pyproject.toml
--rw-r--r--   0 alexandre   (501) staff       (20)      997 2022-10-07 08:01:13.000000 pycobertura-3.2.0/pytest.ini
--rwxr-xr-x   0 alexandre   (501) staff       (20)      415 2022-10-09 09:37:38.000000 pycobertura-3.2.0/release.sh
--rw-r--r--   0 alexandre   (501) staff       (20)     1300 2023-05-13 04:10:13.571691 pycobertura-3.2.0/setup.cfg
--rw-r--r--   0 alexandre   (501) staff       (20)       38 2022-03-03 22:33:26.000000 pycobertura-3.2.0/setup.py
--rw-r--r--   0 alexandre   (501) staff       (20)       82 2022-10-07 08:01:13.000000 pycobertura-3.2.0/test-requirements.txt
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-05-13 04:10:13.565121 pycobertura-3.2.0/tests/
--rw-r--r--   0 alexandre   (501) staff       (20)       64 2022-10-07 23:42:24.000000 pycobertura-3.2.0/tests/.testgitignore
--rw-r--r--   0 alexandre   (501) staff       (20)      748 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/README.generate-dummy-coverage-for-testing.md
--rw-r--r--   0 alexandre   (501) staff       (20)        0 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/__init__.py
--rw-r--r--   0 alexandre   (501) staff       (20)     1162 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/cobertura-generated-by-istanbul-from-coffeescript.xml
--rw-r--r--   0 alexandre   (501) staff       (20)     7963 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/cobertura.xml
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-05-13 04:10:13.565744 pycobertura-3.2.0/tests/dummy/
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-05-13 04:10:13.571097 pycobertura-3.2.0/tests/dummy/dummy/
--rw-r--r--   0 alexandre   (501) staff       (20)        0 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/dummy/dummy/__init__.py
--rw-r--r--   0 alexandre   (501) staff       (20)       41 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/dummy/dummy/dummy.py
--rw-r--r--   0 alexandre   (501) staff       (20)       20 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/dummy/dummy/dummy2.py
--rw-r--r--   0 alexandre   (501) staff       (20)      995 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/dummy/dummy-with-prefix.zip
--rw-r--r--   0 alexandre   (501) staff       (20)      687 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/dummy/dummy.zip
--rw-r--r--   0 alexandre   (501) staff       (20)     1032 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/dummy/setup.cfg
--rw-r--r--   0 alexandre   (501) staff       (20)      179 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/dummy/test_dummy.py
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-05-13 04:10:13.566044 pycobertura-3.2.0/tests/dummy.linestatus/
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-05-13 04:10:13.566190 pycobertura-3.2.0/tests/dummy.linestatus/dummy/
--rw-r--r--   0 alexandre   (501) staff       (20)       14 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/dummy.linestatus/dummy/__init__.py
--rw-r--r--   0 alexandre   (501) staff       (20)      623 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/dummy.linestatus/test1.xml
--rw-r--r--   0 alexandre   (501) staff       (20)      578 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/dummy.linestatus/test2.xml
--rw-r--r--   0 alexandre   (501) staff       (20)      861 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/dummy.original-better-cov.xml
--rw-r--r--   0 alexandre   (501) staff       (20)      852 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/dummy.original-full-cov.xml
--rw-r--r--   0 alexandre   (501) staff       (20)      858 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/dummy.original.xml
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-05-13 04:10:13.566771 pycobertura-3.2.0/tests/dummy.source1/
--rw-r--r--   0 alexandre   (501) staff       (20)     1456 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/dummy.source1/coverage.xml
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-05-13 04:10:13.567307 pycobertura-3.2.0/tests/dummy.source1/dummy/
--rw-r--r--   0 alexandre   (501) staff       (20)        0 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/dummy.source1/dummy/__init__.py
--rw-r--r--   0 alexandre   (501) staff       (20)       56 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/dummy.source1/dummy/dummy.py
--rw-r--r--   0 alexandre   (501) staff       (20)       20 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/dummy.source1/dummy/dummy2.py
--rw-r--r--   0 alexandre   (501) staff       (20)       64 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/dummy.source1/dummy/dummy4.py
--rw-r--r--   0 alexandre   (501) staff       (20)     1032 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/dummy.source1/setup.cfg
--rw-r--r--   0 alexandre   (501) staff       (20)      119 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/dummy.source1/test_dummy.py
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-05-13 04:10:13.567704 pycobertura-3.2.0/tests/dummy.source2/
--rw-r--r--   0 alexandre   (501) staff       (20)     1423 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/dummy.source2/coverage.xml
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-05-13 04:10:13.568200 pycobertura-3.2.0/tests/dummy.source2/dummy/
--rw-r--r--   0 alexandre   (501) staff       (20)        0 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/dummy.source2/dummy/__init__.py
--rw-r--r--   0 alexandre   (501) staff       (20)       56 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/dummy.source2/dummy/dummy.py
--rw-r--r--   0 alexandre   (501) staff       (20)       44 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/dummy.source2/dummy/dummy2.py
--rw-r--r--   0 alexandre   (501) staff       (20)      209 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/dummy.source2/dummy/dummy3.py
--rw-r--r--   0 alexandre   (501) staff       (20)     1032 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/dummy.source2/setup.cfg
--rw-r--r--   0 alexandre   (501) staff       (20)      179 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/dummy.source2/test_dummy.py
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-05-13 04:10:13.568606 pycobertura-3.2.0/tests/dummy.uncovered/
--rw-r--r--   0 alexandre   (501) staff       (20)     1178 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/dummy.uncovered/coverage.xml
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-05-13 04:10:13.569455 pycobertura-3.2.0/tests/dummy.uncovered/dummy/
--rw-r--r--   0 alexandre   (501) staff       (20)        0 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/dummy.uncovered/dummy/__init__.py
--rw-r--r--   0 alexandre   (501) staff       (20)      114 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/dummy.uncovered/dummy/dummy.py
--rw-r--r--   0 alexandre   (501) staff       (20)     1032 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/dummy.uncovered/setup.cfg
--rw-r--r--   0 alexandre   (501) staff       (20)      178 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/dummy.uncovered/test_dummy.py
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-05-13 04:10:13.569009 pycobertura-3.2.0/tests/dummy.uncovered.addcode/
--rw-r--r--   0 alexandre   (501) staff       (20)     1250 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/dummy.uncovered.addcode/coverage.xml
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-05-13 04:10:13.569234 pycobertura-3.2.0/tests/dummy.uncovered.addcode/dummy/
--rw-r--r--   0 alexandre   (501) staff       (20)        0 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/dummy.uncovered.addcode/dummy/__init__.py
--rw-r--r--   0 alexandre   (501) staff       (20)      185 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/dummy.uncovered.addcode/dummy/dummy.py
--rw-r--r--   0 alexandre   (501) staff       (20)     1032 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/dummy.uncovered.addcode/setup.cfg
--rw-r--r--   0 alexandre   (501) staff       (20)      178 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/dummy.uncovered.addcode/test_dummy.py
--rw-r--r--   0 alexandre   (501) staff       (20)     1093 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/dummy.with-dummy2-better-and-worse.xml
--rw-r--r--   0 alexandre   (501) staff       (20)     1092 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/dummy.with-dummy2-better-cov.xml
--rw-r--r--   0 alexandre   (501) staff       (20)     1080 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/dummy.with-dummy2-full-cov.xml
--rw-r--r--   0 alexandre   (501) staff       (20)     1090 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/dummy.with-dummy2-no-cov.xml
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-05-13 04:10:13.569884 pycobertura-3.2.0/tests/dummy.zeroexit1/
--rw-r--r--   0 alexandre   (501) staff       (20)      969 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/dummy.zeroexit1/coverage.xml
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-05-13 04:10:13.570123 pycobertura-3.2.0/tests/dummy.zeroexit1/dummy/
--rw-r--r--   0 alexandre   (501) staff       (20)        0 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/dummy.zeroexit1/dummy/__init__.py
--rw-r--r--   0 alexandre   (501) staff       (20)      108 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/dummy.zeroexit1/dummy/dummy.py
--rw-r--r--   0 alexandre   (501) staff       (20)     1032 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/dummy.zeroexit1/setup.cfg
--rw-r--r--   0 alexandre   (501) staff       (20)       58 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/dummy.zeroexit1/test_dummy.py
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-05-13 04:10:13.570521 pycobertura-3.2.0/tests/dummy.zeroexit2/
--rw-r--r--   0 alexandre   (501) staff       (20)     1000 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/dummy.zeroexit2/coverage.xml
-drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-05-13 04:10:13.570748 pycobertura-3.2.0/tests/dummy.zeroexit2/dummy/
--rw-r--r--   0 alexandre   (501) staff       (20)        0 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/dummy.zeroexit2/dummy/__init__.py
--rw-r--r--   0 alexandre   (501) staff       (20)      134 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/dummy.zeroexit2/dummy/dummy.py
--rw-r--r--   0 alexandre   (501) staff       (20)     1032 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/dummy.zeroexit2/setup.cfg
--rw-r--r--   0 alexandre   (501) staff       (20)       68 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/dummy.zeroexit2/test_dummy.py
--rw-r--r--   0 alexandre   (501) staff       (20)    30824 2023-05-13 04:07:52.000000 pycobertura-3.2.0/tests/test_cli.py
--rw-r--r--   0 alexandre   (501) staff       (20)     9064 2022-03-03 22:33:26.000000 pycobertura-3.2.0/tests/test_cobertura.py
--rw-r--r--   0 alexandre   (501) staff       (20)     5737 2022-10-07 08:01:13.000000 pycobertura-3.2.0/tests/test_cobertura_diff.py
--rw-r--r--   0 alexandre   (501) staff       (20)      127 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/test_colorize.py
--rw-r--r--   0 alexandre   (501) staff       (20)      429 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/test_extrapolate_coverage.py
--rw-r--r--   0 alexandre   (501) staff       (20)     6494 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/test_filesystem.py
--rw-r--r--   0 alexandre   (501) staff       (20)     6429 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/test_hunkify_coverage.py
--rw-r--r--   0 alexandre   (501) staff       (20)      187 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/test_imports.py
--rw-r--r--   0 alexandre   (501) staff       (20)     1166 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/test_rangify.py
--rw-r--r--   0 alexandre   (501) staff       (20)     1076 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/test_reconcile_lines.py
--rw-r--r--   0 alexandre   (501) staff       (20)      926 2022-10-07 23:42:24.000000 pycobertura-3.2.0/tests/test_regex_utils.py
--rw-r--r--   0 alexandre   (501) staff       (20)    21608 2023-05-13 04:07:52.000000 pycobertura-3.2.0/tests/test_reporters.py
--rw-r--r--   0 alexandre   (501) staff       (20)     1175 2022-03-03 22:33:26.000000 pycobertura-3.2.0/tests/test_stringify.py
--rw-r--r--   0 alexandre   (501) staff       (20)      420 2022-01-04 01:58:44.000000 pycobertura-3.2.0/tests/utils.py
--rw-r--r--   0 alexandre   (501) staff       (20)      528 2022-10-07 08:01:13.000000 pycobertura-3.2.0/tox.ini
+drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-06-01 09:02:24.819012 pycobertura-3.2.1/
+-rw-r--r--   0 alexandre   (501) staff       (20)       32 2023-06-01 08:45:26.000000 pycobertura-3.2.1/.coveragerc
+drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-06-01 09:02:24.798379 pycobertura-3.2.1/.github/
+drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-06-01 09:02:24.802555 pycobertura-3.2.1/.github/workflows/
+-rw-r--r--   0 alexandre   (501) staff       (20)      650 2023-06-01 08:59:53.000000 pycobertura-3.2.1/.github/workflows/build-and-test-pycobertura.yml
+-rw-r--r--   0 alexandre   (501) staff       (20)      604 2022-03-03 22:33:26.000000 pycobertura-3.2.1/.gitignore
+-rw-r--r--   0 alexandre   (501) staff       (20)    15716 2023-06-01 09:01:19.000000 pycobertura-3.2.1/CHANGES.md
+-rw-r--r--   0 alexandre   (501) staff       (20)     1103 2022-03-03 22:33:26.000000 pycobertura-3.2.1/LICENSE
+-rw-r--r--   0 alexandre   (501) staff       (20)    24292 2023-06-01 09:02:24.819142 pycobertura-3.2.1/PKG-INFO
+-rw-r--r--   0 alexandre   (501) staff       (20)    23306 2023-05-13 04:07:52.000000 pycobertura-3.2.1/README.md
+-rw-r--r--   0 alexandre   (501) staff       (20)        6 2023-06-01 09:00:34.000000 pycobertura-3.2.1/__version__
+-rw-r--r--   0 alexandre   (501) staff       (20)     2697 2022-01-04 01:58:44.000000 pycobertura-3.2.1/aysha-logo.svg
+drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-06-01 09:02:24.805472 pycobertura-3.2.1/images/
+-rw-r--r--   0 alexandre   (501) staff       (20)    30894 2022-03-03 22:33:26.000000 pycobertura-3.2.1/images/example_csv_diff_output.png
+-rw-r--r--   0 alexandre   (501) staff       (20)   172765 2023-05-13 04:07:52.000000 pycobertura-3.2.1/images/example_github_annotation_diff.png
+-rw-r--r--   0 alexandre   (501) staff       (20)   103005 2023-04-29 17:28:15.000000 pycobertura-3.2.1/images/example_github_annotation_show.png
+-rw-r--r--   0 alexandre   (501) staff       (20)    61287 2022-03-03 22:33:26.000000 pycobertura-3.2.1/images/example_json_output.png
+-rw-r--r--   0 alexandre   (501) staff       (20)    53710 2022-03-03 22:33:26.000000 pycobertura-3.2.1/images/example_markdown_diff_output.png
+-rw-r--r--   0 alexandre   (501) staff       (20)    45822 2022-03-03 22:33:26.000000 pycobertura-3.2.1/images/example_yaml_output.png
+drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-06-01 09:02:24.807160 pycobertura-3.2.1/pycobertura/
+-rw-r--r--   0 alexandre   (501) staff       (20)      119 2022-01-04 01:58:44.000000 pycobertura-3.2.1/pycobertura/__init__.py
+-rw-r--r--   0 alexandre   (501) staff       (20)     9607 2023-06-01 08:45:26.000000 pycobertura-3.2.1/pycobertura/cli.py
+-rw-r--r--   0 alexandre   (501) staff       (20)    15355 2023-06-01 08:45:26.000000 pycobertura-3.2.1/pycobertura/cobertura.py
+-rw-r--r--   0 alexandre   (501) staff       (20)     4944 2023-06-01 08:59:53.000000 pycobertura-3.2.1/pycobertura/filesystem.py
+-rw-r--r--   0 alexandre   (501) staff       (20)      203 2023-04-05 07:16:26.000000 pycobertura-3.2.1/pycobertura/merge.py
+-rw-r--r--   0 alexandre   (501) staff       (20)    17838 2023-06-01 08:45:26.000000 pycobertura-3.2.1/pycobertura/reporters.py
+drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-06-01 09:02:24.809107 pycobertura-3.2.1/pycobertura/templates/
+-rw-r--r--   0 alexandre   (501) staff       (20)        0 2022-01-04 01:58:44.000000 pycobertura-3.2.1/pycobertura/templates/__init__.py
+-rw-r--r--   0 alexandre   (501) staff       (20)      624 2023-06-01 08:45:26.000000 pycobertura-3.2.1/pycobertura/templates/filters.py
+-rw-r--r--   0 alexandre   (501) staff       (20)     2805 2023-06-01 08:45:26.000000 pycobertura-3.2.1/pycobertura/templates/html-delta.jinja2
+-rw-r--r--   0 alexandre   (501) staff       (20)     1764 2023-06-01 08:45:26.000000 pycobertura-3.2.1/pycobertura/templates/html.jinja2
+-rw-r--r--   0 alexandre   (501) staff       (20)      473 2022-01-04 01:58:44.000000 pycobertura-3.2.1/pycobertura/templates/macro.source.jinja2
+-rw-r--r--   0 alexandre   (501) staff       (20)     7797 2022-01-04 01:58:44.000000 pycobertura-3.2.1/pycobertura/templates/normalize.css
+-rw-r--r--   0 alexandre   (501) staff       (20)    11452 2022-01-04 01:58:44.000000 pycobertura-3.2.1/pycobertura/templates/skeleton.css
+-rw-r--r--   0 alexandre   (501) staff       (20)     7151 2023-06-01 08:45:26.000000 pycobertura-3.2.1/pycobertura/utils.py
+drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-06-01 09:02:24.808093 pycobertura-3.2.1/pycobertura.egg-info/
+-rw-r--r--   0 alexandre   (501) staff       (20)    24292 2023-06-01 09:02:24.000000 pycobertura-3.2.1/pycobertura.egg-info/PKG-INFO
+-rw-r--r--   0 alexandre   (501) staff       (20)     3405 2023-06-01 09:02:24.000000 pycobertura-3.2.1/pycobertura.egg-info/SOURCES.txt
+-rw-r--r--   0 alexandre   (501) staff       (20)        1 2023-06-01 09:02:24.000000 pycobertura-3.2.1/pycobertura.egg-info/dependency_links.txt
+-rw-r--r--   0 alexandre   (501) staff       (20)       60 2023-06-01 09:02:24.000000 pycobertura-3.2.1/pycobertura.egg-info/entry_points.txt
+-rw-r--r--   0 alexandre   (501) staff       (20)        1 2022-03-04 19:49:40.000000 pycobertura-3.2.1/pycobertura.egg-info/not-zip-safe
+-rw-r--r--   0 alexandre   (501) staff       (20)       44 2023-06-01 09:02:24.000000 pycobertura-3.2.1/pycobertura.egg-info/requires.txt
+-rw-r--r--   0 alexandre   (501) staff       (20)       12 2023-06-01 09:02:24.000000 pycobertura-3.2.1/pycobertura.egg-info/top_level.txt
+-rw-r--r--   0 alexandre   (501) staff       (20)      122 2022-03-03 22:33:26.000000 pycobertura-3.2.1/pyproject.toml
+-rw-r--r--   0 alexandre   (501) staff       (20)      997 2023-06-01 08:45:26.000000 pycobertura-3.2.1/pytest.ini
+-rwxr-xr-x   0 alexandre   (501) staff       (20)      415 2022-10-09 09:37:38.000000 pycobertura-3.2.1/release.sh
+-rw-r--r--   0 alexandre   (501) staff       (20)     1300 2023-06-01 09:02:24.819503 pycobertura-3.2.1/setup.cfg
+-rw-r--r--   0 alexandre   (501) staff       (20)       38 2022-03-03 22:33:26.000000 pycobertura-3.2.1/setup.py
+-rw-r--r--   0 alexandre   (501) staff       (20)       82 2022-10-07 08:01:13.000000 pycobertura-3.2.1/test-requirements.txt
+drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-06-01 09:02:24.813248 pycobertura-3.2.1/tests/
+-rw-r--r--   0 alexandre   (501) staff       (20)       64 2022-10-07 23:42:24.000000 pycobertura-3.2.1/tests/.testgitignore
+-rw-r--r--   0 alexandre   (501) staff       (20)      748 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/README.generate-dummy-coverage-for-testing.md
+-rw-r--r--   0 alexandre   (501) staff       (20)        0 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/__init__.py
+-rw-r--r--   0 alexandre   (501) staff       (20)     1162 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/cobertura-generated-by-istanbul-from-coffeescript.xml
+-rw-r--r--   0 alexandre   (501) staff       (20)     7963 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/cobertura.xml
+drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-06-01 09:02:24.813895 pycobertura-3.2.1/tests/dummy/
+drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-06-01 09:02:24.818896 pycobertura-3.2.1/tests/dummy/dummy/
+-rw-r--r--   0 alexandre   (501) staff       (20)        0 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/dummy/dummy/__init__.py
+-rw-r--r--   0 alexandre   (501) staff       (20)       41 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/dummy/dummy/dummy.py
+-rw-r--r--   0 alexandre   (501) staff       (20)       20 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/dummy/dummy/dummy2.py
+-rw-r--r--   0 alexandre   (501) staff       (20)      995 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/dummy/dummy-with-prefix.zip
+-rw-r--r--   0 alexandre   (501) staff       (20)      687 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/dummy/dummy.zip
+-rw-r--r--   0 alexandre   (501) staff       (20)     1032 2023-05-21 07:37:14.000000 pycobertura-3.2.1/tests/dummy/setup.cfg
+-rw-r--r--   0 alexandre   (501) staff       (20)      179 2023-05-21 07:35:57.000000 pycobertura-3.2.1/tests/dummy/test_dummy.py
+drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-06-01 09:02:24.814200 pycobertura-3.2.1/tests/dummy.linestatus/
+drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-06-01 09:02:24.814325 pycobertura-3.2.1/tests/dummy.linestatus/dummy/
+-rw-r--r--   0 alexandre   (501) staff       (20)       14 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/dummy.linestatus/dummy/__init__.py
+-rw-r--r--   0 alexandre   (501) staff       (20)      623 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/dummy.linestatus/test1.xml
+-rw-r--r--   0 alexandre   (501) staff       (20)      578 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/dummy.linestatus/test2.xml
+-rw-r--r--   0 alexandre   (501) staff       (20)      861 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/dummy.original-better-cov.xml
+-rw-r--r--   0 alexandre   (501) staff       (20)      852 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/dummy.original-full-cov.xml
+-rw-r--r--   0 alexandre   (501) staff       (20)      858 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/dummy.original.xml
+drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-06-01 09:02:24.814718 pycobertura-3.2.1/tests/dummy.source1/
+-rw-r--r--   0 alexandre   (501) staff       (20)     1456 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/dummy.source1/coverage.xml
+drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-06-01 09:02:24.815189 pycobertura-3.2.1/tests/dummy.source1/dummy/
+-rw-r--r--   0 alexandre   (501) staff       (20)        0 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/dummy.source1/dummy/__init__.py
+-rw-r--r--   0 alexandre   (501) staff       (20)       56 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/dummy.source1/dummy/dummy.py
+-rw-r--r--   0 alexandre   (501) staff       (20)       20 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/dummy.source1/dummy/dummy2.py
+-rw-r--r--   0 alexandre   (501) staff       (20)       64 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/dummy.source1/dummy/dummy4.py
+-rw-r--r--   0 alexandre   (501) staff       (20)     1032 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/dummy.source1/setup.cfg
+-rw-r--r--   0 alexandre   (501) staff       (20)      119 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/dummy.source1/test_dummy.py
+drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-06-01 09:02:24.815566 pycobertura-3.2.1/tests/dummy.source2/
+-rw-r--r--   0 alexandre   (501) staff       (20)     1423 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/dummy.source2/coverage.xml
+drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-06-01 09:02:24.816040 pycobertura-3.2.1/tests/dummy.source2/dummy/
+-rw-r--r--   0 alexandre   (501) staff       (20)        0 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/dummy.source2/dummy/__init__.py
+-rw-r--r--   0 alexandre   (501) staff       (20)       56 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/dummy.source2/dummy/dummy.py
+-rw-r--r--   0 alexandre   (501) staff       (20)       44 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/dummy.source2/dummy/dummy2.py
+-rw-r--r--   0 alexandre   (501) staff       (20)      209 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/dummy.source2/dummy/dummy3.py
+-rw-r--r--   0 alexandre   (501) staff       (20)     1032 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/dummy.source2/setup.cfg
+-rw-r--r--   0 alexandre   (501) staff       (20)      179 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/dummy.source2/test_dummy.py
+drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-06-01 09:02:24.816433 pycobertura-3.2.1/tests/dummy.uncovered/
+-rw-r--r--   0 alexandre   (501) staff       (20)     1178 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/dummy.uncovered/coverage.xml
+drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-06-01 09:02:24.817299 pycobertura-3.2.1/tests/dummy.uncovered/dummy/
+-rw-r--r--   0 alexandre   (501) staff       (20)        0 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/dummy.uncovered/dummy/__init__.py
+-rw-r--r--   0 alexandre   (501) staff       (20)      114 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/dummy.uncovered/dummy/dummy.py
+-rw-r--r--   0 alexandre   (501) staff       (20)     1032 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/dummy.uncovered/setup.cfg
+-rw-r--r--   0 alexandre   (501) staff       (20)      178 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/dummy.uncovered/test_dummy.py
+drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-06-01 09:02:24.816841 pycobertura-3.2.1/tests/dummy.uncovered.addcode/
+-rw-r--r--   0 alexandre   (501) staff       (20)     1250 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/dummy.uncovered.addcode/coverage.xml
+drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-06-01 09:02:24.817073 pycobertura-3.2.1/tests/dummy.uncovered.addcode/dummy/
+-rw-r--r--   0 alexandre   (501) staff       (20)        0 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/dummy.uncovered.addcode/dummy/__init__.py
+-rw-r--r--   0 alexandre   (501) staff       (20)      185 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/dummy.uncovered.addcode/dummy/dummy.py
+-rw-r--r--   0 alexandre   (501) staff       (20)     1032 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/dummy.uncovered.addcode/setup.cfg
+-rw-r--r--   0 alexandre   (501) staff       (20)      178 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/dummy.uncovered.addcode/test_dummy.py
+-rw-r--r--   0 alexandre   (501) staff       (20)     1093 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/dummy.with-dummy2-better-and-worse.xml
+-rw-r--r--   0 alexandre   (501) staff       (20)     1092 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/dummy.with-dummy2-better-cov.xml
+-rw-r--r--   0 alexandre   (501) staff       (20)     1080 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/dummy.with-dummy2-full-cov.xml
+-rw-r--r--   0 alexandre   (501) staff       (20)     1090 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/dummy.with-dummy2-no-cov.xml
+drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-06-01 09:02:24.817705 pycobertura-3.2.1/tests/dummy.zeroexit1/
+-rw-r--r--   0 alexandre   (501) staff       (20)      969 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/dummy.zeroexit1/coverage.xml
+drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-06-01 09:02:24.817932 pycobertura-3.2.1/tests/dummy.zeroexit1/dummy/
+-rw-r--r--   0 alexandre   (501) staff       (20)        0 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/dummy.zeroexit1/dummy/__init__.py
+-rw-r--r--   0 alexandre   (501) staff       (20)      108 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/dummy.zeroexit1/dummy/dummy.py
+-rw-r--r--   0 alexandre   (501) staff       (20)     1032 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/dummy.zeroexit1/setup.cfg
+-rw-r--r--   0 alexandre   (501) staff       (20)       58 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/dummy.zeroexit1/test_dummy.py
+drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-06-01 09:02:24.818329 pycobertura-3.2.1/tests/dummy.zeroexit2/
+-rw-r--r--   0 alexandre   (501) staff       (20)     1000 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/dummy.zeroexit2/coverage.xml
+drwxr-xr-x   0 alexandre   (501) staff       (20)        0 2023-06-01 09:02:24.818548 pycobertura-3.2.1/tests/dummy.zeroexit2/dummy/
+-rw-r--r--   0 alexandre   (501) staff       (20)        0 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/dummy.zeroexit2/dummy/__init__.py
+-rw-r--r--   0 alexandre   (501) staff       (20)      134 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/dummy.zeroexit2/dummy/dummy.py
+-rw-r--r--   0 alexandre   (501) staff       (20)     1032 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/dummy.zeroexit2/setup.cfg
+-rw-r--r--   0 alexandre   (501) staff       (20)       68 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/dummy.zeroexit2/test_dummy.py
+-rw-r--r--   0 alexandre   (501) staff       (20)    30824 2023-06-01 08:45:26.000000 pycobertura-3.2.1/tests/test_cli.py
+-rw-r--r--   0 alexandre   (501) staff       (20)     9064 2023-06-01 08:45:26.000000 pycobertura-3.2.1/tests/test_cobertura.py
+-rw-r--r--   0 alexandre   (501) staff       (20)     6117 2023-06-01 08:59:53.000000 pycobertura-3.2.1/tests/test_cobertura_diff.py
+-rw-r--r--   0 alexandre   (501) staff       (20)      127 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/test_colorize.py
+-rw-r--r--   0 alexandre   (501) staff       (20)      429 2023-06-01 08:45:26.000000 pycobertura-3.2.1/tests/test_extrapolate_coverage.py
+-rw-r--r--   0 alexandre   (501) staff       (20)     6853 2023-06-01 08:59:53.000000 pycobertura-3.2.1/tests/test_filesystem.py
+-rw-r--r--   0 alexandre   (501) staff       (20)     6429 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/test_hunkify_coverage.py
+-rw-r--r--   0 alexandre   (501) staff       (20)      187 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/test_imports.py
+-rw-r--r--   0 alexandre   (501) staff       (20)     1166 2023-06-01 08:45:26.000000 pycobertura-3.2.1/tests/test_rangify.py
+-rw-r--r--   0 alexandre   (501) staff       (20)     1076 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/test_reconcile_lines.py
+-rw-r--r--   0 alexandre   (501) staff       (20)      926 2022-10-07 23:42:24.000000 pycobertura-3.2.1/tests/test_regex_utils.py
+-rw-r--r--   0 alexandre   (501) staff       (20)    21608 2023-06-01 08:45:26.000000 pycobertura-3.2.1/tests/test_reporters.py
+-rw-r--r--   0 alexandre   (501) staff       (20)     1175 2023-06-01 08:45:26.000000 pycobertura-3.2.1/tests/test_stringify.py
+-rw-r--r--   0 alexandre   (501) staff       (20)      420 2022-01-04 01:58:44.000000 pycobertura-3.2.1/tests/utils.py
+-rw-r--r--   0 alexandre   (501) staff       (20)      551 2023-06-01 08:59:53.000000 pycobertura-3.2.1/tox.ini
```

### Comparing `pycobertura-3.2.0/.github/workflows/build-and-test-pycobertura.yml` & `pycobertura-3.2.1/.github/workflows/build-and-test-pycobertura.yml`

 * *Files 21% similar despite different names*

```diff
@@ -7,15 +7,15 @@
   pull_request:
 
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.7", "3.8", "3.9", "3.10"]
+        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
 
     steps:
       - uses: actions/checkout@v2
         with:
           fetch-depth: 0
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
```

### Comparing `pycobertura-3.2.0/.gitignore` & `pycobertura-3.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/CHANGES.md` & `pycobertura-3.2.1/CHANGES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 # Release Notes
 
 ## Unreleased
 
+## 3.2.1 (2023-06-01)
+
+* Make `ZipFileSystem` read files in text mode to fix diffing mixed file systems. Thanks @ernestask
+* Add Python 3.11 as a supported version. Thanks @ernestask
+
 ## 3.2.0 (2023-05-12)
 
 * `pycobertura diff` now supports output format: `github-annotation`. Thanks @goatwu1993
 
 ## 3.1.0 (2023-04-29)
 
 * `pycobertura show` now supports output format: `github-annotation`. Thanks @goatwu1993
```

### Comparing `pycobertura-3.2.0/LICENSE` & `pycobertura-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/PKG-INFO` & `pycobertura-3.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycobertura
-Version: 3.2.0
+Version: 3.2.1
 Summary: "A Cobertura coverage parser that can diff reports and show coverage progress."
 Home-page: https://github.com/aconrad/pycobertura
 Author: "Alex Conrad"
 Author-email: "alexandre.conrad@gmail.com"
 Maintainer: "Alex Conrad"
 Maintainer-email: "alexandre.conrad@gmail.com"
 Keywords: "cobertura coverage diff report parser parse xml"
```

### Comparing `pycobertura-3.2.0/README.md` & `pycobertura-3.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/aysha-logo.svg` & `pycobertura-3.2.1/aysha-logo.svg`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/images/example_csv_diff_output.png` & `pycobertura-3.2.1/images/example_csv_diff_output.png`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/images/example_github_annotation_diff.png` & `pycobertura-3.2.1/images/example_github_annotation_diff.png`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/images/example_github_annotation_show.png` & `pycobertura-3.2.1/images/example_github_annotation_show.png`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/images/example_json_output.png` & `pycobertura-3.2.1/images/example_json_output.png`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/images/example_markdown_diff_output.png` & `pycobertura-3.2.1/images/example_markdown_diff_output.png`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/images/example_yaml_output.png` & `pycobertura-3.2.1/images/example_yaml_output.png`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/pycobertura/cli.py` & `pycobertura-3.2.1/pycobertura/cli.py`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/pycobertura/cobertura.py` & `pycobertura-3.2.1/pycobertura/cobertura.py`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/pycobertura/filesystem.py` & `pycobertura-3.2.1/pycobertura/filesystem.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,17 +62,17 @@
         return self.real_filename(filename) in self.zipfile.namelist()
 
     @contextmanager
     def open(self, filename):
         filename = self.real_filename(filename)
 
         try:
-            f = self.zipfile.open(filename)
-            yield f
-            f.close()
+            with self.zipfile.open(filename) as f:
+                with io.TextIOWrapper(f, encoding="utf-8") as t:
+                    yield t
         except KeyError:
             raise self.FileNotFound(filename)
 
 
 class GitFileSystem(FileSystem):
     def __init__(self, repo_folder, ref):
         self.repository = repo_folder
```

### Comparing `pycobertura-3.2.0/pycobertura/reporters.py` & `pycobertura-3.2.1/pycobertura/reporters.py`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/pycobertura/templates/filters.py` & `pycobertura-3.2.1/pycobertura/templates/filters.py`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/pycobertura/templates/html-delta.jinja2` & `pycobertura-3.2.1/pycobertura/templates/html-delta.jinja2`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/pycobertura/templates/html.jinja2` & `pycobertura-3.2.1/pycobertura/templates/html.jinja2`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/pycobertura/templates/normalize.css` & `pycobertura-3.2.1/pycobertura/templates/normalize.css`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/pycobertura/templates/skeleton.css` & `pycobertura-3.2.1/pycobertura/templates/skeleton.css`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/pycobertura/utils.py` & `pycobertura-3.2.1/pycobertura/utils.py`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/pycobertura.egg-info/PKG-INFO` & `pycobertura-3.2.1/pycobertura.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycobertura
-Version: 3.2.0
+Version: 3.2.1
 Summary: "A Cobertura coverage parser that can diff reports and show coverage progress."
 Home-page: https://github.com/aconrad/pycobertura
 Author: "Alex Conrad"
 Author-email: "alexandre.conrad@gmail.com"
 Maintainer: "Alex Conrad"
 Maintainer-email: "alexandre.conrad@gmail.com"
 Keywords: "cobertura coverage diff report parser parse xml"
```

### Comparing `pycobertura-3.2.0/pycobertura.egg-info/SOURCES.txt` & `pycobertura-3.2.1/pycobertura.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/pytest.ini` & `pycobertura-3.2.1/pytest.ini`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/setup.cfg` & `pycobertura-3.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/tests/README.generate-dummy-coverage-for-testing.md` & `pycobertura-3.2.1/tests/README.generate-dummy-coverage-for-testing.md`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/tests/cobertura-generated-by-istanbul-from-coffeescript.xml` & `pycobertura-3.2.1/tests/cobertura-generated-by-istanbul-from-coffeescript.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/tests/cobertura.xml` & `pycobertura-3.2.1/tests/cobertura.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/tests/dummy/dummy-with-prefix.zip` & `pycobertura-3.2.1/tests/dummy/dummy-with-prefix.zip`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/tests/dummy/dummy.zip` & `pycobertura-3.2.1/tests/dummy/dummy.zip`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/tests/dummy/setup.cfg` & `pycobertura-3.2.1/tests/dummy/setup.cfg`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/tests/dummy.linestatus/test1.xml` & `pycobertura-3.2.1/tests/dummy.linestatus/test1.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/tests/dummy.linestatus/test2.xml` & `pycobertura-3.2.1/tests/dummy.linestatus/test2.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/tests/dummy.original-better-cov.xml` & `pycobertura-3.2.1/tests/dummy.original-better-cov.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/tests/dummy.original-full-cov.xml` & `pycobertura-3.2.1/tests/dummy.original-full-cov.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/tests/dummy.original.xml` & `pycobertura-3.2.1/tests/dummy.original.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/tests/dummy.source1/coverage.xml` & `pycobertura-3.2.1/tests/dummy.source1/coverage.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/tests/dummy.source1/setup.cfg` & `pycobertura-3.2.1/tests/dummy.source1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/tests/dummy.source2/coverage.xml` & `pycobertura-3.2.1/tests/dummy.source2/coverage.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/tests/dummy.source2/setup.cfg` & `pycobertura-3.2.1/tests/dummy.source2/setup.cfg`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/tests/dummy.uncovered/coverage.xml` & `pycobertura-3.2.1/tests/dummy.uncovered/coverage.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/tests/dummy.uncovered/setup.cfg` & `pycobertura-3.2.1/tests/dummy.uncovered/setup.cfg`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/tests/dummy.uncovered.addcode/coverage.xml` & `pycobertura-3.2.1/tests/dummy.uncovered.addcode/coverage.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/tests/dummy.uncovered.addcode/setup.cfg` & `pycobertura-3.2.1/tests/dummy.uncovered.addcode/setup.cfg`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/tests/dummy.with-dummy2-better-and-worse.xml` & `pycobertura-3.2.1/tests/dummy.with-dummy2-better-and-worse.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/tests/dummy.with-dummy2-better-cov.xml` & `pycobertura-3.2.1/tests/dummy.with-dummy2-better-cov.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/tests/dummy.with-dummy2-full-cov.xml` & `pycobertura-3.2.1/tests/dummy.with-dummy2-full-cov.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/tests/dummy.with-dummy2-no-cov.xml` & `pycobertura-3.2.1/tests/dummy.with-dummy2-no-cov.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/tests/dummy.zeroexit1/coverage.xml` & `pycobertura-3.2.1/tests/dummy.zeroexit1/coverage.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/tests/dummy.zeroexit1/setup.cfg` & `pycobertura-3.2.1/tests/dummy.zeroexit1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/tests/dummy.zeroexit2/coverage.xml` & `pycobertura-3.2.1/tests/dummy.zeroexit2/coverage.xml`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/tests/dummy.zeroexit2/setup.cfg` & `pycobertura-3.2.1/tests/dummy.zeroexit2/setup.cfg`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/tests/test_cli.py` & `pycobertura-3.2.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/tests/test_cobertura.py` & `pycobertura-3.2.1/tests/test_cobertura.py`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/tests/test_cobertura_diff.py` & `pycobertura-3.2.1/tests/test_cobertura_diff.py`

 * *Files 8% similar despite different names*

```diff
@@ -156,7 +156,17 @@
 def test_diff__has_not_better_coverage():
     from pycobertura.cobertura import Cobertura, CoberturaDiff
 
     cobertura1 = Cobertura('tests/dummy.zeroexit2/coverage.xml')
     cobertura2 = Cobertura('tests/dummy.zeroexit1/coverage.xml')
     differ = CoberturaDiff(cobertura1, cobertura2)
     assert differ.has_better_coverage() is False
+
+
+def test_diff__mixed_filesystems():
+    from pycobertura.cobertura import Cobertura, CoberturaDiff
+
+    cobertura1 = make_cobertura('tests/dummy.original.xml', source='tests/dummy/dummy.zip')
+    cobertura2 = make_cobertura('tests/dummy.original.xml', source='tests/dummy')
+
+    differ = CoberturaDiff(cobertura1, cobertura2)
+    assert differ.has_all_changes_covered() is True
```

### Comparing `pycobertura-3.2.0/tests/test_filesystem.py` & `pycobertura-3.2.1/tests/test_filesystem.py`

 * *Files 5% similar despite different names*

```diff
@@ -98,14 +98,29 @@
     ]
 
     for source_file in source_files_in_zip:
         with fs.open(source_file) as f:
             assert hasattr(f, 'read')
 
 
+def test_filesystem_zip__read_str():
+    from pycobertura.filesystem import ZipFileSystem
+
+    fs = ZipFileSystem("tests/dummy/dummy.zip")
+
+    source_files_in_zip = [
+        'dummy/dummy.py',
+        'dummy/dummy2.py',
+    ]
+
+    for source_file in source_files_in_zip:
+        with fs.open(source_file) as f:
+            assert isinstance(f.read(), str)
+
+
 def test_filesystem_git():
     import pycobertura.filesystem as fsm
 
     branch, folder, filename = "master", "tests/dummy", "test-file"
 
     with patch.object(fsm, "subprocess") as subprocess_mock:
         subprocess_mock.check_output = MagicMock(return_value=b"<file-content>")
```

### Comparing `pycobertura-3.2.0/tests/test_hunkify_coverage.py` & `pycobertura-3.2.1/tests/test_hunkify_coverage.py`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/tests/test_rangify.py` & `pycobertura-3.2.1/tests/test_rangify.py`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/tests/test_reconcile_lines.py` & `pycobertura-3.2.1/tests/test_reconcile_lines.py`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/tests/test_regex_utils.py` & `pycobertura-3.2.1/tests/test_regex_utils.py`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/tests/test_reporters.py` & `pycobertura-3.2.1/tests/test_reporters.py`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/tests/test_stringify.py` & `pycobertura-3.2.1/tests/test_stringify.py`

 * *Files identical despite different names*

### Comparing `pycobertura-3.2.0/tox.ini` & `pycobertura-3.2.1/tox.ini`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [tox]
 skipsdist = True
-envlist = py37, py38, py39, py310, pep8, black
+envlist = py37, py38, py39, py310, py311, pep8, black
 
 [gh-actions]
 python =
     3.7: py37
     3.8: py38
     3.9: py39
     3.10: py310, pep8, black
+    3.11: py311
 
 [flake8]
 max-line-length = 88
 
 [testenv]
 commands =
     pip install -r test-requirements.txt --force-reinstall
```

