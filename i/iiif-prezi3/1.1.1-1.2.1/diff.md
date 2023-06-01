# Comparing `tmp/iiif-prezi3-1.1.1.tar.gz` & `tmp/iiif-prezi3-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iiif-prezi3-1.1.1.tar", last modified: Fri Jan 27 14:44:15 2023, max compression
+gzip compressed data, was "iiif-prezi3-1.2.1.tar", last modified: Thu Jun  1 15:39:22 2023, max compression
```

## Comparing `iiif-prezi3-1.1.1.tar` & `iiif-prezi3-1.2.1.tar`

### file list

```diff
@@ -1,45 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 14:44:15.952582 iiif-prezi3-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-01-27 14:44:04.000000 iiif-prezi3-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6820 2023-01-27 14:44:15.952582 iiif-prezi3-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-01-27 14:44:04.000000 iiif-prezi3-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 14:44:15.944581 iiif-prezi3-1.1.1/iiif_prezi3/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-01-27 14:44:04.000000 iiif-prezi3-1.1.1/iiif_prezi3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-01-27 14:44:04.000000 iiif-prezi3-1.1.1/iiif_prezi3/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 14:44:15.948582 iiif-prezi3-1.1.1/iiif_prezi3/config/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-01-27 14:44:04.000000 iiif-prezi3-1.1.1/iiif_prezi3/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-01-27 14:44:04.000000 iiif-prezi3-1.1.1/iiif_prezi3/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-27 14:44:04.000000 iiif-prezi3-1.1.1/iiif_prezi3/config/extensions.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 14:44:15.948582 iiif-prezi3-1.1.1/iiif_prezi3/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 14:44:04.000000 iiif-prezi3-1.1.1/iiif_prezi3/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-01-27 14:44:04.000000 iiif-prezi3-1.1.1/iiif_prezi3/extensions/example_extension.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 14:44:15.948582 iiif-prezi3-1.1.1/iiif_prezi3/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-01-27 14:44:04.000000 iiif-prezi3-1.1.1/iiif_prezi3/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-01-27 14:44:04.000000 iiif-prezi3-1.1.1/iiif_prezi3/helpers/add_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-01-27 14:44:04.000000 iiif-prezi3-1.1.1/iiif_prezi3/helpers/add_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-01-27 14:44:04.000000 iiif-prezi3-1.1.1/iiif_prezi3/helpers/add_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-01-27 14:44:04.000000 iiif-prezi3-1.1.1/iiif_prezi3/helpers/add_range.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-01-27 14:44:04.000000 iiif-prezi3-1.1.1/iiif_prezi3/helpers/add_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-01-27 14:44:04.000000 iiif-prezi3-1.1.1/iiif_prezi3/helpers/annotation_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-01-27 14:44:04.000000 iiif-prezi3-1.1.1/iiif_prezi3/helpers/auto_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-01-27 14:44:04.000000 iiif-prezi3-1.1.1/iiif_prezi3/helpers/canvas_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-01-27 14:44:04.000000 iiif-prezi3-1.1.1/iiif_prezi3/helpers/canvas_sizes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-01-27 14:44:04.000000 iiif-prezi3-1.1.1/iiif_prezi3/helpers/create_canvas_from_iiif.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-01-27 14:44:04.000000 iiif-prezi3-1.1.1/iiif_prezi3/helpers/make_canvas.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-01-27 14:44:04.000000 iiif-prezi3-1.1.1/iiif_prezi3/helpers/make_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-01-27 14:44:04.000000 iiif-prezi3-1.1.1/iiif_prezi3/helpers/make_manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-01-27 14:44:04.000000 iiif-prezi3-1.1.1/iiif_prezi3/helpers/make_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-01-27 14:44:04.000000 iiif-prezi3-1.1.1/iiif_prezi3/helpers/make_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-01-27 14:44:04.000000 iiif-prezi3-1.1.1/iiif_prezi3/helpers/set_hwd.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-01-27 14:44:04.000000 iiif-prezi3-1.1.1/iiif_prezi3/helpers/set_hwd_from_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-01-27 14:44:04.000000 iiif-prezi3-1.1.1/iiif_prezi3/helpers/set_hwd_from_iiif.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-01-27 14:44:04.000000 iiif-prezi3-1.1.1/iiif_prezi3/helpers/to_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-01-27 14:44:04.000000 iiif-prezi3-1.1.1/iiif_prezi3/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    12902 2023-01-27 14:44:04.000000 iiif-prezi3-1.1.1/iiif_prezi3/skeleton.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 14:44:15.944581 iiif-prezi3-1.1.1/iiif_prezi3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6820 2023-01-27 14:44:15.000000 iiif-prezi3-1.1.1/iiif_prezi3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-01-27 14:44:15.000000 iiif-prezi3-1.1.1/iiif_prezi3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 14:44:15.000000 iiif-prezi3-1.1.1/iiif_prezi3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-01-27 14:44:15.000000 iiif-prezi3-1.1.1/iiif_prezi3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-01-27 14:44:15.000000 iiif-prezi3-1.1.1/iiif_prezi3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-27 14:44:15.952582 iiif-prezi3-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-01-27 14:44:04.000000 iiif-prezi3-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:39:22.696999 iiif-prezi3-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-01 15:39:13.000000 iiif-prezi3-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6820 2023-06-01 15:39:22.696999 iiif-prezi3-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-06-01 15:39:13.000000 iiif-prezi3-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:39:22.688999 iiif-prezi3-1.2.1/iiif_prezi3/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-01 15:39:13.000000 iiif-prezi3-1.2.1/iiif_prezi3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-06-01 15:39:13.000000 iiif-prezi3-1.2.1/iiif_prezi3/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:39:22.688999 iiif-prezi3-1.2.1/iiif_prezi3/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-01 15:39:13.000000 iiif-prezi3-1.2.1/iiif_prezi3/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-01 15:39:13.000000 iiif-prezi3-1.2.1/iiif_prezi3/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-01 15:39:13.000000 iiif-prezi3-1.2.1/iiif_prezi3/config/extensions.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:39:22.688999 iiif-prezi3-1.2.1/iiif_prezi3/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 15:39:13.000000 iiif-prezi3-1.2.1/iiif_prezi3/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-01 15:39:13.000000 iiif-prezi3-1.2.1/iiif_prezi3/extensions/example_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:39:22.692999 iiif-prezi3-1.2.1/iiif_prezi3/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-01 15:39:13.000000 iiif-prezi3-1.2.1/iiif_prezi3/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-06-01 15:39:13.000000 iiif-prezi3-1.2.1/iiif_prezi3/helpers/add_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-01 15:39:13.000000 iiif-prezi3-1.2.1/iiif_prezi3/helpers/add_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-06-01 15:39:13.000000 iiif-prezi3-1.2.1/iiif_prezi3/helpers/add_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-01 15:39:13.000000 iiif-prezi3-1.2.1/iiif_prezi3/helpers/add_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-01 15:39:13.000000 iiif-prezi3-1.2.1/iiif_prezi3/helpers/add_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-01 15:39:13.000000 iiif-prezi3-1.2.1/iiif_prezi3/helpers/add_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-01 15:39:13.000000 iiif-prezi3-1.2.1/iiif_prezi3/helpers/add_thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-06-01 15:39:13.000000 iiif-prezi3-1.2.1/iiif_prezi3/helpers/annotation_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-06-01 15:39:13.000000 iiif-prezi3-1.2.1/iiif_prezi3/helpers/auto_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-01 15:39:13.000000 iiif-prezi3-1.2.1/iiif_prezi3/helpers/canvas_sizes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-06-01 15:39:13.000000 iiif-prezi3-1.2.1/iiif_prezi3/helpers/create_canvas_from_iiif.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-01 15:39:13.000000 iiif-prezi3-1.2.1/iiif_prezi3/helpers/make_canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-01 15:39:13.000000 iiif-prezi3-1.2.1/iiif_prezi3/helpers/make_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-01 15:39:13.000000 iiif-prezi3-1.2.1/iiif_prezi3/helpers/make_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-01 15:39:13.000000 iiif-prezi3-1.2.1/iiif_prezi3/helpers/make_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-01 15:39:13.000000 iiif-prezi3-1.2.1/iiif_prezi3/helpers/make_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-01 15:39:13.000000 iiif-prezi3-1.2.1/iiif_prezi3/helpers/set_hwd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-01 15:39:13.000000 iiif-prezi3-1.2.1/iiif_prezi3/helpers/set_hwd_from_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-01 15:39:13.000000 iiif-prezi3-1.2.1/iiif_prezi3/helpers/set_hwd_from_iiif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-01 15:39:13.000000 iiif-prezi3-1.2.1/iiif_prezi3/helpers/to_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-06-01 15:39:13.000000 iiif-prezi3-1.2.1/iiif_prezi3/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13996 2023-06-01 15:39:13.000000 iiif-prezi3-1.2.1/iiif_prezi3/skeleton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:39:22.688999 iiif-prezi3-1.2.1/iiif_prezi3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6820 2023-06-01 15:39:22.000000 iiif-prezi3-1.2.1/iiif_prezi3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-01 15:39:22.000000 iiif-prezi3-1.2.1/iiif_prezi3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 15:39:22.000000 iiif-prezi3-1.2.1/iiif_prezi3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-01 15:39:22.000000 iiif-prezi3-1.2.1/iiif_prezi3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-01 15:39:22.000000 iiif-prezi3-1.2.1/iiif_prezi3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 15:39:22.696999 iiif-prezi3-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-06-01 15:39:13.000000 iiif-prezi3-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:39:22.692999 iiif-prezi3-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-06-01 15:39:13.000000 iiif-prezi3-1.2.1/tests/test_add_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-01 15:39:13.000000 iiif-prezi3-1.2.1/tests/test_add_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-01 15:39:13.000000 iiif-prezi3-1.2.1/tests/test_add_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-06-01 15:39:13.000000 iiif-prezi3-1.2.1/tests/test_add_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-01 15:39:13.000000 iiif-prezi3-1.2.1/tests/test_annotation_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-06-01 15:39:13.000000 iiif-prezi3-1.2.1/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-01 15:39:13.000000 iiif-prezi3-1.2.1/tests/test_canvas_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-06-01 15:39:13.000000 iiif-prezi3-1.2.1/tests/test_create_canvas_from_iiif.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-01 15:39:13.000000 iiif-prezi3-1.2.1/tests/test_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-01 15:39:13.000000 iiif-prezi3-1.2.1/tests/test_helpers_addlabel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-06-01 15:39:13.000000 iiif-prezi3-1.2.1/tests/test_helpers_autofields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-01 15:39:13.000000 iiif-prezi3-1.2.1/tests/test_make_canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-01 15:39:13.000000 iiif-prezi3-1.2.1/tests/test_make_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-01 15:39:13.000000 iiif-prezi3-1.2.1/tests/test_make_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-01 15:39:13.000000 iiif-prezi3-1.2.1/tests/test_make_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-06-01 15:39:13.000000 iiif-prezi3-1.2.1/tests/test_make_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-06-01 15:39:13.000000 iiif-prezi3-1.2.1/tests/test_set_hwd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-01 15:39:13.000000 iiif-prezi3-1.2.1/tests/test_set_hwd_from_file_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-06-01 15:39:13.000000 iiif-prezi3-1.2.1/tests/test_set_hwd_from_iiif.py
```

### Comparing `iiif-prezi3-1.1.1/LICENSE` & `iiif-prezi3-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iiif-prezi3-1.1.1/PKG-INFO` & `iiif-prezi3-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iiif-prezi3
-Version: 1.1.1
+Version: 1.2.1
 Summary: IIIF Presentation v3 API implementation
 Home-page: https://github.com/iiif-prezi/iiif-prezi3
 Author: IIIF Prezi3 Team
 License: Apache License, Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `iiif-prezi3-1.1.1/README.md` & `iiif-prezi3-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `iiif-prezi3-1.1.1/iiif_prezi3/base.py` & `iiif-prezi3-1.2.1/iiif_prezi3/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,15 +11,24 @@
         validate_all = True
         copy_on_model_validation = False
         smart_union = True
         # Allow us to use the field name like service.id rather than service.@id
         allow_population_by_field_name = True
 
     def __getattribute__(self, prop):
-        val = super(Base, self).__getattribute__(prop)
+        try:
+            val = super(Base, self).__getattribute__(prop)
+        except AttributeError:
+            super_fields = super(Base, self).__getattribute__("__fields__")
+            if "__root__" in super_fields:
+                obj = super(Base, self).__getattribute__("__root__")
+                val = super(Base, obj).__getattribute__(prop)
+            else:
+                raise
+
         # __root__ is a custom pydantic thing
         if hasattr(val, '__root__'):
             if type(val.__root__) in [AnyUrl]:
                 # cast it to a string
                 return str(val.__root__)
             else:
                 return val.__root__
@@ -51,21 +60,28 @@
         super().__setattr__(key, value)
 
     def json(self, **kwargs):
         return self.jsonld(**kwargs)
 
     def jsonld(self, **kwargs):
         # approach 6- use the pydantic .dict() function to get the dict with pydantic options, add the context at the top and dump to json with modified kwargs
-        excluded_args = ["exclude_unset", "exclude_defaults", "exclude_none", "by_alias"]
+        excluded_args = ["exclude_unset", "exclude_defaults", "exclude_none", "by_alias", "ensure_ascii", "default"]
         pydantic_args = ["include", "exclude", "encoder"]
         dict_kwargs = dict([(arg, kwargs[arg]) for arg in kwargs.keys() if arg in pydantic_args])
 
         json_kwargs = dict([(arg, kwargs[arg]) for arg in kwargs.keys() if arg not in pydantic_args + excluded_args])
         return json.dumps({"@context": "http://iiif.io/api/presentation/3/context.json",
-                           **self.dict(exclude_unset=False, exclude_defaults=False, exclude_none=True, by_alias=True, **dict_kwargs)}, default=pydantic_encoder, **json_kwargs)
+                           **self.dict(exclude_unset=False,
+                                       exclude_defaults=False,
+                                       exclude_none=True,
+                                       by_alias=True,
+                                       **dict_kwargs)},
+                          ensure_ascii=False,
+                          default=pydantic_encoder,
+                          **json_kwargs)
 
     def jsonld_dict(self, **kwargs):
         pydantic_args = ["include", "exclude", "encoder"]
         dict_kwargs = dict([(arg, kwargs[arg]) for arg in kwargs.keys() if arg in pydantic_args])
 
         return {"@context": "http://iiif.io/api/presentation/3/context.json",
                 **self.dict(exclude_unset=False, exclude_defaults=False, exclude_none=True, by_alias=True, **dict_kwargs)}
```

### Comparing `iiif-prezi3-1.1.1/iiif_prezi3/config/config.py` & `iiif-prezi3-1.2.1/iiif_prezi3/config/config.py`

 * *Files identical despite different names*

### Comparing `iiif-prezi3-1.1.1/iiif_prezi3/helpers/__init__.py` & `iiif-prezi3-1.2.1/iiif_prezi3/helpers/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+from .add_image import AddImage  # noqa: F401
 from .add_item import AddItem, AddItemByReference  # noqa: F401
 from .add_label import AddLabel  # noqa: F401
 from .add_metadata import AddMetadata  # noqa: F401
 from .add_range import AddRange  # noqa: F401
 from .add_service import AddService  # noqa: F401
+from .add_thumbnail import AddThumbnail  # noqa: F401
 from .annotation_helpers import AnnotationHelpers  # noqa: F401
 from .auto_fields import *  # noqa: F401,F403
-from .canvas_helpers import CanvasHelpers  # noqa: F401
 from .canvas_sizes import MaxHelper, MinHelper  # noqa: F401
 from .create_canvas_from_iiif import CreateCanvasFromIIIF  # noqa: F401
 from .make_canvas import MakeCanvas  # noqa: F401
 from .make_collection import MakeCollection  # noqa: F401
 from .make_manifest import MakeManifest  # noqa: F401
 from .make_range import MakeRange  # noqa: F401
 from .make_service import MakeService  # noqa: F401
```

### Comparing `iiif-prezi3-1.1.1/iiif_prezi3/helpers/add_item.py` & `iiif-prezi3-1.2.1/iiif_prezi3/helpers/add_item.py`

 * *Files identical despite different names*

### Comparing `iiif-prezi3-1.1.1/iiif_prezi3/helpers/add_label.py` & `iiif-prezi3-1.2.1/iiif_prezi3/helpers/add_label.py`

 * *Files identical despite different names*

### Comparing `iiif-prezi3-1.1.1/iiif_prezi3/helpers/add_metadata.py` & `iiif-prezi3-1.2.1/iiif_prezi3/helpers/add_metadata.py`

 * *Files identical despite different names*

### Comparing `iiif-prezi3-1.1.1/iiif_prezi3/helpers/add_service.py` & `iiif-prezi3-1.2.1/iiif_prezi3/helpers/add_service.py`

 * *Files identical despite different names*

### Comparing `iiif-prezi3-1.1.1/iiif_prezi3/helpers/annotation_helpers.py` & `iiif-prezi3-1.2.1/iiif_prezi3/helpers/annotation_helpers.py`

 * *Files identical despite different names*

### Comparing `iiif-prezi3-1.1.1/iiif_prezi3/helpers/auto_fields.py` & `iiif-prezi3-1.2.1/iiif_prezi3/helpers/auto_fields.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import uuid
 
 from ..config.config import Config, register_config
-from ..skeleton import (AnnotationPage, Canvas, Class, KeyValueString, Range,
-                        Reference)
+from ..skeleton import (AnnotationPage, Canvas, Class, HomepageItem,
+                        KeyValueString, NavPlace, ProviderItem, Range,
+                        Reference, ResourceItem, ServiceItem1)
 
 
 class AutoConfig(Config):
 
     def __init__(self, **kw):
         self.properties = []
         Config.__init__(self, **kw)
@@ -139,18 +140,47 @@
     def manipulate_value(self, what, value=None):
         if not value:
             return []
         else:
             return value
 
 
+class AutoListConfig(Config):
+    def __init__(self):
+        self.properties = ['behavior', 'service', 'services', 'features', 'thumbnail', 'logo', 'rendering', 'homepage', 'metadata',
+                           'partOf', 'provider', 'seeAlso']
+
+
+class AutoList(Auto):
+    def __init__(self, cfg, name=""):
+        super().__init__(cfg, name)
+
+    def manipulate_value(self, what, value=None):
+        if not value:
+            return None
+        if not isinstance(value, list):
+            return [value]
+        else:
+            return value
+
+
+class AutoLanguageListConfig(Config):
+    def __init__(self):
+        self.properties = ['language']
+
+
 aicfg = AutoIdConfig()
 alcfg = AutoLangConfig()
 aitcfg = AutoItemsConfig()
+alstcfg = AutoListConfig()
+allstcfg = AutoLanguageListConfig()
 ai = AutoId(aicfg)
 al = AutoLang(alcfg)
 ait = AutoItems(aitcfg)
-
+alst = AutoList(alstcfg, name="General")
+allst = AutoList(allstcfg, name="Language")
 # Set up some obvious defaults
 ai.register_on_class(AnnotationPage, Class)
 al.register_on_class(KeyValueString, Class, Reference)
-ait.register_on_class(Canvas, Range)
+ait.register_on_class(Canvas, Range, AnnotationPage)
+alst.register_on_class(Class, AnnotationPage, ResourceItem, ServiceItem1, NavPlace, Reference, ProviderItem)
+allst.register_on_class(HomepageItem)
```

### Comparing `iiif-prezi3-1.1.1/iiif_prezi3/helpers/canvas_helpers.py` & `iiif-prezi3-1.2.1/iiif_prezi3/helpers/add_thumbnail.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,14 @@
 from ..loader import monkeypatch_schema
-from ..skeleton import Annotation, AnnotationPage, Canvas, ResourceItem
+from ..skeleton import (AccompanyingCanvas, Annotation, AnnotationCollection,
+                        AnnotationPage, Canvas, Collection, Manifest,
+                        PlaceholderCanvas, Range, Reference, ResourceItem)
 
 
-class CanvasHelpers:
-
-    def add_image(self, image_url, anno_id=None, anno_page_id=None, **kwargs):
-        """Adds an image to an existing canvas.
-
-        Args:
-            image_url (str): An HTTP URL which points to the image.
-            anno_id (str): An HTTP URL for the annotation to which the image will be attached.
-            anno_page_id (str): An HTTP URL for the annotation page to which the annotation will be attached.
-
-        Returns:
-            anno_page (AnnotationPage): the AnnotationPage with an Annotation and ResourceItem attached.
-        """
-        body = ResourceItem(id=image_url, type='Image', **kwargs)
-        annotation = Annotation(id=anno_id, body=body, target=self.id, motivation='painting', type='Annotation')
-        anno_page = AnnotationPage(id=anno_page_id, type='AnnotationPage', items=[annotation])
-        if not self.items:
-            self.items = list()
-        self.items.append(anno_page)
-        return anno_page
-
+class AddThumbnail:
     def add_thumbnail(self, image_url, **kwargs):
         """Adds a thumbnail to an existing canvas.
 
         Args:
             image_url (str): An HTTP URL which points to the thumbnail.
             **kwargs (): see ResourceItem.
 
@@ -36,8 +18,8 @@
         new_thumbnail = ResourceItem(id=image_url, type='Image', **kwargs)
         if not self.thumbnail:
             self.thumbnail = list()
         self.thumbnail.append(new_thumbnail)
         return new_thumbnail
 
 
-monkeypatch_schema(Canvas, CanvasHelpers)
+monkeypatch_schema([Canvas, PlaceholderCanvas, AccompanyingCanvas, AnnotationPage, Collection, Manifest, Annotation, Range, ResourceItem, AnnotationCollection, Reference], AddThumbnail)
```

### Comparing `iiif-prezi3-1.1.1/iiif_prezi3/helpers/canvas_sizes.py` & `iiif-prezi3-1.2.1/iiif_prezi3/helpers/canvas_sizes.py`

 * *Files identical despite different names*

### Comparing `iiif-prezi3-1.1.1/iiif_prezi3/helpers/create_canvas_from_iiif.py` & `iiif-prezi3-1.2.1/iiif_prezi3/helpers/create_canvas_from_iiif.py`

 * *Files identical despite different names*

### Comparing `iiif-prezi3-1.1.1/iiif_prezi3/helpers/make_collection.py` & `iiif-prezi3-1.2.1/iiif_prezi3/helpers/make_collection.py`

 * *Files identical despite different names*

### Comparing `iiif-prezi3-1.1.1/iiif_prezi3/helpers/make_manifest.py` & `iiif-prezi3-1.2.1/iiif_prezi3/helpers/make_manifest.py`

 * *Files identical despite different names*

### Comparing `iiif-prezi3-1.1.1/iiif_prezi3/helpers/make_range.py` & `iiif-prezi3-1.2.1/iiif_prezi3/helpers/make_range.py`

 * *Files identical despite different names*

### Comparing `iiif-prezi3-1.1.1/iiif_prezi3/helpers/make_service.py` & `iiif-prezi3-1.2.1/iiif_prezi3/helpers/make_service.py`

 * *Files identical despite different names*

### Comparing `iiif-prezi3-1.1.1/iiif_prezi3/helpers/set_hwd.py` & `iiif-prezi3-1.2.1/iiif_prezi3/helpers/set_hwd.py`

 * *Files identical despite different names*

### Comparing `iiif-prezi3-1.1.1/iiif_prezi3/helpers/set_hwd_from_file.py` & `iiif-prezi3-1.2.1/iiif_prezi3/helpers/set_hwd_from_file.py`

 * *Files identical despite different names*

### Comparing `iiif-prezi3-1.1.1/iiif_prezi3/helpers/set_hwd_from_iiif.py` & `iiif-prezi3-1.2.1/iiif_prezi3/helpers/set_hwd_from_iiif.py`

 * *Files identical despite different names*

### Comparing `iiif-prezi3-1.1.1/iiif_prezi3/helpers/to_reference.py` & `iiif-prezi3-1.2.1/iiif_prezi3/helpers/to_reference.py`

 * *Files identical despite different names*

### Comparing `iiif-prezi3-1.1.1/iiif_prezi3/loader.py` & `iiif-prezi3-1.2.1/iiif_prezi3/loader.py`

 * *Files identical despite different names*

### Comparing `iiif-prezi3-1.1.1/iiif_prezi3/skeleton.py` & `iiif-prezi3-1.2.1/iiif_prezi3/skeleton.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  iiif_3_0.json
-#   timestamp: 2023-01-27T13:50:20+00:00
+#   timestamp: 2023-06-01T15:24:07+00:00
 
 from __future__ import annotations
 
 from datetime import datetime
 from typing import Any, Dict, List, Optional, Union
 
 from pydantic import AnyUrl, Extra, Field, PositiveFloat, PositiveInt, constr
@@ -52,22 +52,24 @@
         constr(regex=r'^right-to-left$'),
         constr(regex=r'^top-to-bottom$'),
         constr(regex=r'^bottom-to-top$'),
     ]
 
 
 class Id(Base):
-    __root__: AnyUrl = Field(..., title='Id must be presesnt and must be a URI')
+    __root__: AnyUrl = Field(..., title='Id must be present and must be a URI')
 
 
 class LngString(Base):
-    __root__: Dict[str, List[str]]
-
-    class Config:
-        extra = Extra.forbid
+    __root__: Union[
+        Dict[constr(regex=r'^[a-zA-Z-][a-zA-Z-]*$'), List[str]],
+        Dict[constr(regex=r'^none$'), List[str]],
+    ] = Field(
+        ..., title='Language string, must have a language and value must be an array.'
+    )
 
 
 class AnnoTargetItem(Base):
     source: Id
     scope: Id
 
 
@@ -88,21 +90,41 @@
     __root__: PositiveFloat
 
 
 class Format(Base):
     __root__: constr(regex=r'^[a-z][a-z]*/.*$')
 
 
-class AnnoSelectorItem(Base):
+class SelectorItem(Base):
     type: str
-    t: Optional[Duration] = None
+    t: Duration
+
+
+class SelectorItem1(Base):
+    type: constr(regex=r'^FragmentSelector$') = 'FragmentSelector'
+    conformsTo: AnyUrl = 'http://www.w3.org/TR/media-frags/'
+    value: Any
 
 
-class AnnoSelector(Base):
-    __root__: Union[AnyUrl, AnnoSelectorItem]
+class SelectorItem2(Base):
+    type: constr(regex=r'^SvgSelector$') = 'SvgSelector'
+    value: Any
+
+
+class SelectorItem3(Base):
+    type: constr(regex=r'^ImageApiSelector$') = 'ImageApiSelector'
+    region: Optional[Any] = None
+    size: Optional[Any] = None
+    rotation: Optional[Any] = None
+    quality: Optional[Any] = None
+    format: Optional[Any] = None
+
+
+class Selector(Base):
+    __root__: Union[AnyUrl, SelectorItem, SelectorItem1, SelectorItem2, SelectorItem3]
 
 
 class NavPlace(Base):
     id: Optional[Id] = None
     type: str = 'FeatureCollection'
     features: Optional[List[Dict[str, Any]]] = None
 
@@ -136,16 +158,16 @@
 
 
 class SpecificResource(Base):
     id: Optional[Id] = None
     type: constr(regex=r'^SpecificResource$') = 'SpecificResource'
     format: Optional[Format] = None
     accessibility: Optional[str] = None
-    source: Id
-    selector: Union[AnnoSelector, List[AnnoSelector]]
+    source: Union[Id, Class]
+    selector: Union[Selector, List[Selector]]
 
 
 class HomepageItem(Class):
     format: Optional[Format] = None
     language: Optional[List[BCP47]] = None
 
 
@@ -159,40 +181,38 @@
 
 class PartOf(Base):
     __root__: List[Class]
 
 
 class Item(Class):
     type: constr(regex=r'^Canvas$') = 'Canvas'
+    items: List
 
 
 class SeeAlso(Base):
     __root__: External
 
 
 class AnnoTarget(Base):
     __root__: Union[AnyUrl, SpecificResource, AnnoTargetItem]
 
 
 class Model(Base):
     __root__: Union[Manifest, Collection, AnnotationPage]
 
 
-class AnnotationPage(Base):
-    class Config:
-        extra = Extra.forbid
-
-    context: Optional[Any] = Field(None, alias='@context')
+class AnnotationPage(Class):
+    context: Optional[Union[List[AnyUrl], str]] = Field(None, alias='@context')
     id: Id
     type: constr(regex=r'^AnnotationPage$') = 'AnnotationPage'
     rendering: Optional[External] = None
     label: Optional[LngString] = None
     service: Optional[Service] = None
     thumbnail: Optional[List[Resource]] = None
-    items: Optional[List[Annotation]] = None
+    items: List[Annotation]
 
 
 class Collection(Class):
     type: constr(regex=r'^Collection') = Field(
         'Collection',
         description='If you are validating a manifest, you may get this error if there are errors in the manifest. The validator first validates it as a manifest and if that fails it will try and validate it using the other types.',
         title='Are you validating a collection?',
@@ -211,15 +231,15 @@
     placeholderCanvas: Optional[PlaceholderCanvas] = None
     accompanyingCanvas: Optional[AccompanyingCanvas] = None
     thumbnail: Optional[List[Resource]] = None
     homepage: Optional[Homepage] = None
     behavior: Optional[Behavior] = None
     partOf: Optional[PartOf] = None
     items: Optional[List[Union[ManifestRef, CollectionRef, Collection]]] = None
-    annotations: Optional[List[AnnotationPage]] = None
+    annotations: Optional[List[Union[AnnotationPage, AnnotationPageRef]]] = None
 
 
 class Manifest(Class):
     context: Optional[Union[List[AnyUrl], str]] = Field(None, alias='@context')
     id: Id
     label: LngString
     type: constr(regex=r'^Manifest') = 'Manifest'
@@ -240,15 +260,15 @@
     seeAlso: Optional[SeeAlso] = None
     thumbnail: Optional[List[Resource]] = None
     homepage: Optional[Homepage] = None
     behavior: Optional[Behavior] = None
     partOf: Optional[PartOf] = None
     items: Optional[List[Canvas]] = None
     structures: Optional[List[Range]] = None
-    annotations: Optional[List[AnnotationPage]] = None
+    annotations: Optional[List[Union[AnnotationPage, AnnotationPageRef]]] = None
 
 
 class AccompanyingCanvas(Class):
     type: constr(regex=r'^Canvas$') = 'Canvas'
     height: Optional[Dimension] = None
     width: Optional[Dimension] = None
     duration: Optional[Duration] = None
@@ -263,15 +283,15 @@
     seeAlso: Optional[SeeAlso] = None
     service: Optional[Service] = None
     thumbnail: Optional[List[Resource]] = None
     homepage: Optional[Homepage] = None
     behavior: Optional[Behavior] = None
     partOf: Optional[PartOf] = None
     items: List[AnnotationPage]
-    annotations: Optional[List[AnnotationPage]] = None
+    annotations: Optional[List[Union[AnnotationPage, AnnotationPageRef]]] = None
 
 
 class BodyItem(Choice):
     items: List[Resource]
 
 
 class Annotation(Class):
@@ -302,15 +322,15 @@
     placeholderCanvas: Optional[PlaceholderCanvas] = None
     accompanyingCanvas: Optional[AccompanyingCanvas] = None
     thumbnail: Optional[List[Resource]] = None
     homepage: Optional[Homepage] = None
     behavior: Optional[Behavior] = None
     partOf: Optional[PartOf] = None
     items: List[AnnotationPage]
-    annotations: Optional[List[AnnotationPage]] = None
+    annotations: Optional[List[Union[AnnotationPage, AnnotationPageRef]]] = None
 
 
 class PlaceholderCanvas(Class):
     type: constr(regex=r'^Canvas$') = 'Canvas'
     height: Optional[Dimension] = None
     width: Optional[Dimension] = None
     duration: Optional[Duration] = None
@@ -325,15 +345,15 @@
     seeAlso: Optional[SeeAlso] = None
     service: Optional[Service] = None
     thumbnail: Optional[List[Resource]] = None
     homepage: Optional[Homepage] = None
     behavior: Optional[Behavior] = None
     partOf: Optional[PartOf] = None
     items: List[AnnotationPage]
-    annotations: Optional[List[AnnotationPage]] = None
+    annotations: Optional[List[Union[AnnotationPage, AnnotationPageRef]]] = None
 
 
 class ProviderItem(Class):
     type: constr(regex=r'^Agent$') = 'Agent'
     homepage: Optional[Homepage] = None
     logo: Optional[List[Resource]] = None
     seeAlso: Optional[SeeAlso] = None
@@ -346,32 +366,32 @@
 class Range(Class):
     type: constr(regex=r'^Range$') = 'Range'
     rendering: Optional[External] = None
     supplementary: Optional[AnnotationCollection] = None
     service: Optional[Service] = None
     placeholderCanvas: Optional[PlaceholderCanvas] = None
     accompanyingCanvas: Optional[AccompanyingCanvas] = None
-    annotations: Optional[List[AnnotationPage]] = None
+    annotations: Optional[List[Union[AnnotationPage, AnnotationPageRef]]] = None
     thumbnail: Optional[List[Resource]] = None
-    items: List[Union[SpecificResource, Item, Range, CanvasRef, RangeRef]]
+    items: List[Union[SpecificResource, Item, Range, CanvasRef]]
 
 
 class ResourceItem(Base):
     id: Id
     type: str
     height: Optional[Dimension] = None
     width: Optional[Dimension] = None
     duration: Optional[Duration] = None
     language: Optional[str] = None
     rendering: Optional[External] = None
     service: Optional[Service] = None
     format: Optional[Format] = None
     label: Optional[LngString] = None
     thumbnail: Optional[List[Resource]] = None
-    annotations: Optional[List[AnnotationPage]] = None
+    annotations: Optional[List[Union[AnnotationPage, AnnotationPageRef]]] = None
 
 
 class Resource(Base):
     __root__: Union[ResourceItem, ResourceItem1]
 
 
 class ServiceItem(Class):
@@ -390,37 +410,45 @@
     __root__: List[Union[ServiceItem, ServiceItem1]]
 
 
 class AnnotationCollection(Class):
     type: constr(regex=r'^AnnotationCollection$') = 'AnnotationCollection'
     rendering: Optional[External] = None
     partOf: Optional[PartOf] = None
-    next: Optional[AnnotationPage] = None
-    first: Optional[AnnotationPage] = None
-    last: Optional[AnnotationPage] = None
+    next: Optional[AnnotationPageRef] = None
+    first: Optional[AnnotationPageRef] = None
+    last: Optional[AnnotationPageRef] = None
     service: Optional[Service] = None
     thumbnail: Optional[List[Resource]] = None
     items: Optional[List[Annotation]] = None
 
 
 class Reference(Base):
+    class Config:
+        extra = Extra.allow
+
     id: Id
-    label: LngString
+    label: Optional[LngString] = None
     type: constr(
         regex=r'^Manifest$|^AnnotationPage$|^Collection$|^AnnotationCollection$|^Canvas$|^Range$'
     )
     thumbnail: Optional[List[Resource]] = None
 
 
+class AnnotationPageRef(Reference):
+    type: Optional[constr(regex=r'^AnnotationPage$')] = None
+
+
 class CollectionRef(Reference):
     type: Optional[constr(regex=r'^Collection$')] = None
+    label: LngString
 
 
 class ManifestRef(Reference):
-    type: Optional[constr(regex=r'^Manifest$')] = None
+    type: constr(regex=r'^Manifest$') = 'Manifest'
 
     class Config:
         extra = Extra.allow
 
 
 class CanvasRef(Reference):
     type: Optional[constr(regex=r'^Canvas$')] = None
@@ -440,7 +468,8 @@
 Canvas.update_forward_refs()
 PlaceholderCanvas.update_forward_refs()
 ProviderItem.update_forward_refs()
 Range.update_forward_refs()
 ResourceItem.update_forward_refs()
 ServiceItem.update_forward_refs()
 ServiceItem1.update_forward_refs()
+AnnotationCollection.update_forward_refs()
```

### Comparing `iiif-prezi3-1.1.1/iiif_prezi3.egg-info/PKG-INFO` & `iiif-prezi3-1.2.1/iiif_prezi3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iiif-prezi3
-Version: 1.1.1
+Version: 1.2.1
 Summary: IIIF Presentation v3 API implementation
 Home-page: https://github.com/iiif-prezi/iiif-prezi3
 Author: IIIF Prezi3 Team
 License: Apache License, Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `iiif-prezi3-1.1.1/setup.py` & `iiif-prezi3-1.2.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 if os.path.exists("version.txt"):
     VERSION = (this_directory / "version.txt").read_text().strip()
 else:
-    VERSION = "local_test_version"
+    VERSION = "0.0.0.dev0"
 
 REQUIREMENTS = [
     "pydantic >= 1.9.2, <2.0.0",
     "requests >=2.28.0, <3.0.0",
     "Pillow >=9.1.1, <10.0.0"
 ]
 
@@ -31,15 +31,15 @@
     "isort >=5.10.1, <6.0.0",
     "flake8 >=4.0.1, <5.0.0",
     "flake8-docstrings >=1.6.0, <2.0.0",
     "flake8-isort >=4.1.1, <5.0.0",
     "tox >=3.25.0, <4.0.0",
     "Pillow >=9.1.1, <10.0.0",
     "deepdiff >=6.2.2, <7.0.0",
-    "datamodel-code-generator >=0.16.1, <1.0.0"
+    "datamodel-code-generator >=0.17.1, <1.0.0"
 ]
 
 # Setting up
 setup(
     name="iiif-prezi3",
     version=VERSION,
     author="IIIF Prezi3 Team",
```

