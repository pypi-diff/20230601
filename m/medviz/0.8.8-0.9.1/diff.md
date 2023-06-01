# Comparing `tmp/medviz-0.8.8.tar.gz` & `tmp/medviz-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medviz-0.8.8.tar", last modified: Thu May 18 18:24:40 2023, max compression
+gzip compressed data, was "medviz-0.9.1.tar", last modified: Thu Jun  1 17:25:03 2023, max compression
```

## Comparing `medviz-0.8.8.tar` & `medviz-0.9.1.tar`

### file list

```diff
@@ -1,48 +1,66 @@
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-05-18 18:24:40.696564 medviz-0.8.8/
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)    35149 2023-02-17 19:26:43.000000 medviz-0.8.8/LICENSE
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      149 2023-05-18 14:59:54.000000 medviz-0.8.8/MANIFEST.in
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2274 2023-05-18 18:24:40.696564 medviz-0.8.8/PKG-INFO
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1803 2023-04-27 15:46:29.000000 medviz-0.8.8/README.rst
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)        5 2023-05-18 18:24:32.000000 medviz-0.8.8/VERSION
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-05-18 18:24:40.692564 medviz-0.8.8/medviz/
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1150 2023-05-18 18:24:28.000000 medviz-0.8.8/medviz/__init__.py
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-05-18 18:24:40.692564 medviz-0.8.8/medviz/multimodal/
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)       84 2023-05-18 18:14:13.000000 medviz-0.8.8/medviz/multimodal/__init__.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1056 2023-05-18 18:09:41.000000 medviz-0.8.8/medviz/multimodal/save_dicom_metadata.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      512 2023-05-18 18:13:16.000000 medviz-0.8.8/medviz/multimodal/stats.py
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-05-18 18:24:40.696564 medviz-0.8.8/medviz/plots/
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)       55 2023-05-18 02:10:54.000000 medviz-0.8.8/medviz/plots/__init__.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1552 2023-05-18 02:42:18.000000 medviz-0.8.8/medviz/plots/_plot_image.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)    10511 2023-05-14 06:38:00.000000 medviz-0.8.8/medviz/plots/gif.py
--rw-rw-r--   0 mohsen    (1000) mohsen    (1000)     2273 2023-05-18 02:31:56.000000 medviz-0.8.8/medviz/plots/helper_plot.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     3702 2023-05-17 17:02:52.000000 medviz-0.8.8/medviz/plots/layered_plot2D.py
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-05-18 18:24:40.696564 medviz-0.8.8/medviz/plots/plot2d/
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)       46 2023-05-17 21:56:40.000000 medviz-0.8.8/medviz/plots/plot2d/__init__.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)       86 2023-05-18 18:09:44.000000 medviz-0.8.8/medviz/plots/plot2d/image_masks.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1336 2023-05-18 02:10:51.000000 medviz-0.8.8/medviz/plots/plot2d/images.py
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-05-18 18:24:40.696564 medviz-0.8.8/medviz/plots/plot3d/
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)       46 2023-05-18 02:18:22.000000 medviz-0.8.8/medviz/plots/plot3d/__init__.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2461 2023-05-18 02:47:13.000000 medviz-0.8.8/medviz/plots/plot3d/images.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2364 2023-05-12 19:13:22.000000 medviz-0.8.8/medviz/plots/plot3d/layered_plot.py
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-05-18 18:24:40.696564 medviz-0.8.8/medviz/preprocess/
--rw-rw-r--   0 mohsen    (1000) mohsen    (1000)       86 2023-05-14 03:50:56.000000 medviz-0.8.8/medviz/preprocess/__init__.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1656 2023-05-14 03:51:57.000000 medviz-0.8.8/medviz/preprocess/mask.py
--rw-rw-r--   0 mohsen    (1000) mohsen    (1000)     1658 2023-05-14 04:20:25.000000 medviz-0.8.8/medviz/preprocess/match_image_mask.py
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-05-18 18:24:40.696564 medviz-0.8.8/medviz/utils/
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      476 2023-05-18 03:12:21.000000 medviz-0.8.8/medviz/utils/__init__.py
--rw-rw-r--   0 mohsen    (1000) mohsen    (1000)     2175 2023-05-13 17:59:38.000000 medviz-0.8.8/medviz/utils/array_profile.py
--rw-rw-r--   0 mohsen    (1000) mohsen    (1000)      662 2023-05-13 18:05:32.000000 medviz-0.8.8/medviz/utils/array_threshold.py
--rwxr-xr-x   0 mohsen    (1000) mohsen    (1000)      120 2023-01-02 16:26:25.000000 medviz-0.8.8/medviz/utils/custom_type.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     4587 2023-05-14 03:54:29.000000 medviz-0.8.8/medviz/utils/helper_mask.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      689 2023-01-02 16:26:25.000000 medviz-0.8.8/medviz/utils/log.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      940 2023-04-02 15:43:58.000000 medviz-0.8.8/medviz/utils/reader.py
--rwxr-xr-x   0 mohsen    (1000) mohsen    (1000)       80 2023-05-17 19:24:17.000000 medviz-0.8.8/medviz/utils/utility.py
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-05-18 18:24:40.692564 medviz-0.8.8/medviz.egg-info/
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2274 2023-05-18 18:24:40.000000 medviz-0.8.8/medviz.egg-info/PKG-INFO
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      959 2023-05-18 18:24:40.000000 medviz-0.8.8/medviz.egg-info/SOURCES.txt
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)        1 2023-05-18 18:24:40.000000 medviz-0.8.8/medviz.egg-info/dependency_links.txt
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      174 2023-05-18 18:24:40.000000 medviz-0.8.8/medviz.egg-info/requires.txt
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)        7 2023-05-18 18:24:40.000000 medviz-0.8.8/medviz.egg-info/top_level.txt
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1311 2023-05-18 18:20:06.000000 medviz-0.8.8/pyproject.toml
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)       38 2023-05-18 18:24:40.696564 medviz-0.8.8/setup.cfg
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      170 2023-04-02 14:20:15.000000 medviz-0.8.8/setup.py
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-01 17:25:03.472003 medviz-0.9.1/
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)    36861 2023-05-31 20:04:32.000000 medviz-0.9.1/LICENSE
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)      180 2023-06-01 05:23:25.000000 medviz-0.9.1/MANIFEST.in
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2274 2023-06-01 17:25:03.472003 medviz-0.9.1/PKG-INFO
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1803 2023-04-27 15:46:29.000000 medviz-0.9.1/README.rst
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)        5 2023-06-01 05:24:31.000000 medviz-0.9.1/VERSION
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-01 17:25:03.472003 medviz-0.9.1/medviz/
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2043 2023-06-01 05:52:20.000000 medviz-0.9.1/medviz/__init__.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)      549 2023-05-31 20:21:50.000000 medviz-0.9.1/medviz/bowel.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)      218 2023-05-23 22:19:22.000000 medviz-0.9.1/medviz/bowel2.py
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-01 17:25:03.472003 medviz-0.9.1/medviz/collage/
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)       41 2023-06-01 02:13:13.000000 medviz-0.9.1/medviz/collage/__init__.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1982 2023-06-01 02:40:53.000000 medviz-0.9.1/medviz/collage/compute_collage.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)    24895 2023-05-31 20:21:55.000000 medviz-0.9.1/medviz/collage/main.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2122 2023-06-01 02:47:15.000000 medviz-0.9.1/medviz/collage/stats.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)      134 2023-05-23 22:19:26.000000 medviz-0.9.1/medviz/example.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1620 2023-05-15 18:19:57.000000 medviz-0.9.1/medviz/fat_mul.py
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-01 17:25:03.472003 medviz-0.9.1/medviz/multimodal/
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)       85 2023-05-22 16:27:34.000000 medviz-0.9.1/medviz/multimodal/__init__.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1065 2023-05-24 22:21:17.000000 medviz-0.9.1/medviz/multimodal/save_dicom_metadata.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)      509 2023-05-22 16:27:37.000000 medviz-0.9.1/medviz/multimodal/stats.py
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-01 17:25:03.472003 medviz-0.9.1/medviz/nifti/
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     4331 2023-06-01 05:36:49.000000 medviz-0.9.1/medviz/nifti/helper.py
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-01 17:25:03.472003 medviz-0.9.1/medviz/pkg2/
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)      134 2023-05-23 22:19:26.000000 medviz-0.9.1/medviz/pkg2/example.py
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-01 17:25:03.472003 medviz-0.9.1/medviz/plots/
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)      123 2023-05-23 23:18:05.000000 medviz-0.9.1/medviz/plots/__init__.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1552 2023-05-18 02:42:18.000000 medviz-0.9.1/medviz/plots/_plot_image.py
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-01 17:25:03.472003 medviz-0.9.1/medviz/plots/gif/
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)    10203 2023-05-24 04:19:50.000000 medviz-0.9.1/medviz/plots/gif/gif.py
+-rw-rw-r--   0 mohsen    (1000) mohsen    (1000)     2217 2023-05-25 02:41:16.000000 medviz-0.9.1/medviz/plots/helper_plot.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     3682 2023-05-24 04:19:50.000000 medviz-0.9.1/medviz/plots/layered_plot2D.py
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-01 17:25:03.472003 medviz-0.9.1/medviz/plots/plot2d/
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)      238 2023-05-24 02:22:53.000000 medviz-0.9.1/medviz/plots/plot2d/__init__.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1890 2023-05-24 05:06:19.000000 medviz-0.9.1/medviz/plots/plot2d/image_mask_annotated.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1831 2023-05-24 05:06:19.000000 medviz-0.9.1/medviz/plots/plot2d/image_masks.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1633 2023-05-24 02:54:03.000000 medviz-0.9.1/medviz/plots/plot2d/images.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1891 2023-05-24 02:59:58.000000 medviz-0.9.1/medviz/plots/plot2d/masks.py
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-01 17:25:03.472003 medviz-0.9.1/medviz/plots/plot3d/
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)      114 2023-05-25 02:26:37.000000 medviz-0.9.1/medviz/plots/plot3d/__init__.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1890 2023-05-24 05:06:19.000000 medviz-0.9.1/medviz/plots/plot3d/image_mask_annotated.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2390 2023-05-24 05:06:19.000000 medviz-0.9.1/medviz/plots/plot3d/images.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2060 2023-05-31 20:21:55.000000 medviz-0.9.1/medviz/plots/plot3d/layered_plot.py
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-01 17:25:03.472003 medviz-0.9.1/medviz/preprocess/
+-rw-rw-r--   0 mohsen    (1000) mohsen    (1000)       86 2023-05-14 03:50:56.000000 medviz-0.9.1/medviz/preprocess/__init__.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2015 2023-06-01 05:55:48.000000 medviz-0.9.1/medviz/preprocess/mask.py
+-rw-rw-r--   0 mohsen    (1000) mohsen    (1000)     1753 2023-06-01 05:56:55.000000 medviz-0.9.1/medviz/preprocess/match_image_mask.py
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-01 17:25:03.472003 medviz-0.9.1/medviz/utils/
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)      570 2023-06-01 05:14:13.000000 medviz-0.9.1/medviz/utils/__init__.py
+-rw-rw-r--   0 mohsen    (1000) mohsen    (1000)     2175 2023-05-13 17:59:38.000000 medviz-0.9.1/medviz/utils/array_profile.py
+-rw-rw-r--   0 mohsen    (1000) mohsen    (1000)      662 2023-05-13 18:05:32.000000 medviz-0.9.1/medviz/utils/array_threshold.py
+-rwxr-xr-x   0 mohsen    (1000) mohsen    (1000)      152 2023-05-23 22:19:26.000000 medviz-0.9.1/medviz/utils/custom_type.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     4587 2023-05-23 23:25:32.000000 medviz-0.9.1/medviz/utils/helper_mask.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2448 2023-05-24 04:53:08.000000 medviz-0.9.1/medviz/utils/helper_path.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)      689 2023-01-02 16:26:25.000000 medviz-0.9.1/medviz/utils/log.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)      859 2023-05-24 05:07:22.000000 medviz-0.9.1/medviz/utils/reader.py
+-rwxr-xr-x   0 mohsen    (1000) mohsen    (1000)       80 2023-05-17 19:24:17.000000 medviz-0.9.1/medviz/utils/utility.py
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-01 17:25:03.472003 medviz-0.9.1/medviz.egg-info/
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2274 2023-06-01 17:25:03.000000 medviz-0.9.1/medviz.egg-info/PKG-INFO
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1331 2023-06-01 17:25:03.000000 medviz-0.9.1/medviz.egg-info/SOURCES.txt
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)        1 2023-06-01 17:25:03.000000 medviz-0.9.1/medviz.egg-info/dependency_links.txt
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)      190 2023-06-01 17:25:03.000000 medviz-0.9.1/medviz.egg-info/requires.txt
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)        7 2023-06-01 17:25:03.000000 medviz-0.9.1/medviz.egg-info/top_level.txt
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1359 2023-06-01 05:50:19.000000 medviz-0.9.1/pyproject.toml
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)       38 2023-06-01 17:25:03.472003 medviz-0.9.1/setup.cfg
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)      170 2023-04-02 14:20:15.000000 medviz-0.9.1/setup.py
```

### Comparing `medviz-0.8.8/LICENSE` & `medviz-0.9.1/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,35 @@
+The CoLlAGe script (medviz/collage/main.py) is developed by BrIC Laboratory, under the **BSD 3-Clause License**. 
+
+**CoLlAGe Lisece**
+Copyright (C) 2020 BrIC Laboratory
+
+Redistribution and use in source and binary forms, with or without modification, are permitted provided that the
+following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following
+disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following
+disclaimer in the documentation and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products
+derived from this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES,
+INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
+SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
+WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF
+THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+
+
+Anything else (except `medviz/collage/main.py`) are distributed under the **GNU General Public License v3.0**.
+
                     GNU GENERAL PUBLIC LICENSE
                        Version 3, 29 June 2007
 
  Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
  Everyone is permitted to copy and distribute verbatim copies
  of this license document, but changing it is not allowed.
```

### Comparing `medviz-0.8.8/PKG-INFO` & `medviz-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medviz
-Version: 0.8.8
+Version: 0.9.1
 Summary: Medical Image Visualization Tool 🐍🚀🎉🦕
 Author-email: Mohsen Hariri <mohsen.hariri@case.eud>
 License: GPL-3.0 License
 Keywords: MRI,CT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `medviz-0.8.8/README.rst` & `medviz-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `medviz-0.8.8/medviz/multimodal/save_dicom_metadata.py` & `medviz-0.9.1/medviz/multimodal/save_dicom_metadata.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,17 +17,15 @@
             and element.VR != "UN"
         ):
             metadata[element.keyword] = element.value
 
     return metadata
 
 
-def save_dicom_metadata(
-    base_path, id_func=lambda x: x, pattern="**/*.dcm", save_path="./"
-):
+def save_dicom_metadata(base_path, id_func=lambda x: x, pattern="**/*.dcm", save_path: str or Path = "./"):
     paths = Path(base_path).glob(pattern)
     metadata_list = []
 
     for path in paths:
         id = id_func(path.stem)
 
         metadata = read_dicom_metadata(path)
```

### Comparing `medviz-0.8.8/medviz/plots/_plot_image.py` & `medviz-0.9.1/medviz/plots/_plot_image.py`

 * *Files identical despite different names*

### Comparing `medviz-0.8.8/medviz/plots/gif.py` & `medviz-0.9.1/medviz/plots/gif/gif.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,17 +77,15 @@
     num_masks = len(masks_data)
 
     if segments:
         try:
             assert len(segments) == num_masks
         except AssertionError:
             # raise ValueError("Number of segments must be equal to the number of masks")
-            print(
-                "Number of segments must be equal to the number of masks, segments will be ignored"
-            )
+            print("Number of segments must be equal to the number of masks, segments will be ignored")
             segments = None
 
     # _, last_slice = assert_shape(ct_data + masks_data)
     last_slice = ct_data.shape[-1] - 1
 
     mask_colors = generate_mask_colors(num_masks, mask_colors)
 
@@ -107,32 +105,28 @@
         plt.imshow(ct_data[:, :, current_slice], cmap="gray")
 
         xbar_title = ""
 
         for i in range(len(masks_data)):
             if not np.all(masks_data[i][:, :, current_slice] == False):
                 xbar_title_update = (
-                    f"{segments[i]}: {mask_colors[i]}"
-                    if segments
-                    else f"Mask {i}: {mask_colors[i]}"
+                    f"{segments[i]}: {mask_colors[i]}" if segments else f"Mask {i}: {mask_colors[i]}"
                 )
                 xbar_title = xbar_title + xbar_title_update
 
             plt.contour(
                 masks_data[i][:, :, current_slice],
                 colors=mask_colors[i],
                 levels=[0.5],
             )
 
         plt.title(f"{title} Slice {current_slice} {xbar_title}")
         plt.axis("off")
 
-    ani = animation.FuncAnimation(
-        fig, update_slice, frames=slice_range, interval=interval
-    )
+    ani = animation.FuncAnimation(fig, update_slice, frames=slice_range, interval=interval)
 
     if save_path:
         if isinstance(save_path, str):
             save_path = Path(save_path)
 
         if save_path.suffix != ".png":
             save_path = save_path.with_suffix(".gif")
@@ -165,17 +159,15 @@
     num_masks = len(masks_data)
 
     if segments:
         try:
             assert len(segments) == num_masks
         except AssertionError:
             # raise ValueError("Number of segments must be equal to the number of masks")
-            print(
-                "Number of segments must be equal to the number of masks, segments will be ignored"
-            )
+            print("Number of segments must be equal to the number of masks, segments will be ignored")
             segments = None
 
     mask_colors = generate_mask_colors(num_masks, mask_colors)
 
     fig = plt.figure()
 
     def update_slice(frame):
@@ -188,17 +180,15 @@
         plt.imshow(ct_data[:, :, current_slice], cmap="gray")
 
         xbar_title = ""
 
         for i in range(len(masks_data)):
             if not np.all(masks_data[i][:, :, current_slice] == False):
                 xbar_title_update = (
-                    f"{segments[i]}: {mask_colors[i]}"
-                    if segments
-                    else f"Mask {i}: {mask_colors[i]}"
+                    f"{segments[i]}: {mask_colors[i]}" if segments else f"Mask {i}: {mask_colors[i]}"
                 )
                 xbar_title = xbar_title + xbar_title_update
 
             plt.contour(
                 masks_data[i][:, :, current_slice],
                 colors=mask_colors[i],
                 levels=[0.5],
@@ -246,17 +236,15 @@
     num_masks = len(masks_data)
 
     if segments:
         try:
             assert len(segments) == num_masks
         except AssertionError:
             # raise ValueError("Number of segments must be equal to the number of masks")
-            print(
-                "Number of segments must be equal to the number of masks, segments will be ignored"
-            )
+            print("Number of segments must be equal to the number of masks, segments will be ignored")
             segments = None
 
     # assert_shape(ct_data + masks_data)
 
     mask_colors = generate_mask_colors(num_masks, mask_colors)
 
     fig = plt.figure()
@@ -273,32 +261,28 @@
         plt.imshow(ct_data[:, :, current_slice], cmap="gray")
 
         xbar_title = ""
 
         for i in range(len(masks_data)):
             if not np.all(masks_data[i][:, :, current_slice] == False):
                 xbar_title_update = (
-                    f"{segments[i]}: {mask_colors[i]}"
-                    if segments
-                    else f"Mask {i}: {mask_colors[i]}"
+                    f"{segments[i]}: {mask_colors[i]}" if segments else f"Mask {i}: {mask_colors[i]}"
                 )
                 xbar_title = xbar_title + xbar_title_update
 
             plt.contour(
                 masks_data[i][:, :, current_slice],
                 colors=mask_colors[i],
                 levels=[0.5],
             )
 
         plt.title(f"{title} Slice {current_slice} {xbar_title}")
         plt.axis("off")
 
-    ani = animation.FuncAnimation(
-        fig, update_slice, frames=slice_range, interval=interval
-    )
+    ani = animation.FuncAnimation(fig, update_slice, frames=slice_range, interval=interval)
 
     if save_path:
         if isinstance(save_path, str):
             save_path = Path(save_path)
 
         if save_path.suffix != ".png":
             save_path = save_path.with_suffix(".gif")
@@ -335,17 +319,15 @@
     num_masks = len(masks_data)
 
     if segments:
         try:
             assert len(segments) == num_masks
         except AssertionError:
             # raise ValueError("Number of segments must be equal to the number of masks")
-            print(
-                "Number of segments must be equal to the number of masks, segments will be ignored"
-            )
+            print("Number of segments must be equal to the number of masks, segments will be ignored")
             segments = None
 
     assert_shape(ct_data + mask_reference_data + masks_data)
 
     mask_colors = generate_mask_colors(num_masks, mask_colors)
 
     fig = plt.figure()
@@ -366,17 +348,15 @@
         )
 
         xbar_title = ""
 
         for i in range(len(masks_data)):
             if not np.all(masks_data[i][:, :, current_slice] == False):
                 xbar_title_update = (
-                    f"{segments[i]}: {mask_colors[i]}"
-                    if segments
-                    else f"Mask {i}: {mask_colors[i]}"
+                    f"{segments[i]}: {mask_colors[i]}" if segments else f"Mask {i}: {mask_colors[i]}"
                 )
                 xbar_title = xbar_title + xbar_title_update
 
             plt.contour(
                 masks_data[i][:, :, current_slice],
                 colors=mask_colors[i],
                 levels=[0.5],
```

### Comparing `medviz-0.8.8/medviz/plots/helper_plot.py` & `medviz-0.9.1/medviz/plots/helper_plot.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,37 +34,32 @@
             return mask_colors
         except AssertionError:
             raise ValueError(
                 f"Number of masks ({num_masks}) does not match number of colors ({len(mask_colors)})"
             )
 
 
-def plot_image(ax, image_data, cmap="gray"):
-    ax.imshow(image_data, cmap=cmap)
-
-
-def plot_image_imshow(ax, arr, cmap="gray", origin="lower", title="", RGB=False):
-    # ax.imshow(arr, cmap=cmap, origin=origin)
-    ax.imshow(arr, cmap=cmap)
-
+def plot_image(ax, image_data, cmap="gray", origin="upper", title=""):
+    ax.imshow(image_data, cmap=cmap, origin=origin)
     ax.set_title(title)
 
 
 def plot_mask_neighbor(ax, mask_data, cmap="jet", alpha=0.3):
     # ax.imshow(mask_data, cmap=cmap, alpha=alpha, interpolation="bilinear", vmin=0, vmax=1)
     ax.imshow(mask_data, cmap=cmap, alpha=alpha)
 
 
 # def plot_contour(ax, mask_data, color, line_width=0.5,levels=[0.5]):
 #     ax.contour(mask_data, colors=color, linewidths=line_width,levels=levels)
 # ax.contour(mask_data, colors=color, linewidths=line_width, levels=[0.5], alpha=0.5)
 
 
-def plot_contour(ax, mask_data, color, levels=[0.5]):
-    ax.contour(mask_data, colors=color, levels=levels)
+def plot_contour(ax, mask_data, color, origin="lower", title="", levels=[0.5]):
+    ax.contour(mask_data, colors=color, origin=origin, levels=levels)
+    ax.set_title(title)
 
 
 def save_image(plt, save_path):
     if isinstance(save_path, str):
         save_path = Path(save_path)
 
     if save_path.suffix != ".png":
```

### Comparing `medviz-0.8.8/medviz/plots/layered_plot2D.py` & `medviz-0.9.1/medviz/plots/layered_plot2D.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,23 +81,19 @@
         plt.savefig(save_path)
 
 
 import matplotlib.pyplot as plt
 import numpy as np
 
 
-def layered_plot_all2D(
-    id, image_data, mask_data, save_path, mask_color="red", title=""
-):
+def layered_plot_all2D(id, image_data, mask_data, save_path, mask_color="red", title=""):
     image_data_rot = np.flip(np.rot90(image_data, axes=(1, 0)), axis=1)
     mask_data_rot = np.flip(np.rot90(mask_data, axes=(1, 0)), axis=1)
 
-    most_value_nonzero_slices, num_nonzero_slices = significant_slice_idx_data(
-        mask_data_rot
-    )
+    most_value_nonzero_slices, num_nonzero_slices = significant_slice_idx_data(mask_data_rot)
     print(most_value_nonzero_slices, num_nonzero_slices)
     for i in range(num_nonzero_slices):
         slice = most_value_nonzero_slices[i]
         _, ax = plt.subplots()
         plt.subplots_adjust(bottom=0.25)
         plot_image(ax, image_data_rot[:, :, slice], cmap="gray")
         plot_contour(ax, mask_data_rot[:, :, slice], color=mask_color, levels=[0.5])
```

### Comparing `medviz-0.8.8/medviz/plots/plot2d/images.py` & `medviz-0.9.1/medviz/plots/plot2d/images.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,72 @@
 import math
 
 import matplotlib.pyplot as plt
 import numpy as np
 
-from ...plots import plot_image_imshow, save_image
-from ...utils import image_path_to_data_ax
+from ...plots import plot_image, save_image
+from ...utils import image_path_to_data_ax, save_path_file
 
 
-def images_path(paths, rows=None, columns=None, titles=[], cmap="gray", save_path=None):
-    images_data = [
-        image_path_to_data_ax(path) for path in paths
-    ]  # just for nifti files
+def images_path(
+    paths,
+    rows=None,
+    columns=None,
+    titles=[],
+    cmap="gray",
+    origin="upper",
+    save_path=None,
+):
+    images_data = [image_path_to_data_ax(path) for path in paths]
 
     images_array(
         images_data=images_data,
         rows=rows,
         columns=columns,
         titles=titles,
         cmap=cmap,
+        origin=origin,
         save_path=save_path,
     )
 
 
 def images_array(
-    images_data, rows=None, columns=None, titles=[], cmap="gray", save_path=None
+    images_data,
+    rows=None,
+    columns=None,
+    titles=[],
+    cmap="gray",
+    origin="upper",
+    save_path=None,
 ):
     print("Loading images...")
 
+    try:
+        assert len(images_data[0].shape) == 2
+    except AssertionError:
+        raise ValueError("Images must be 2D")
+
     num_images = len(images_data)  # Number of images
     rows = math.ceil(math.sqrt(num_images))  # Number of rows in the grid
     columns = math.ceil(num_images / rows)  # Number of columns in the grid
 
     _, axs = plt.subplots(rows, columns)
     if num_images == 1:
         axs = np.array([axs])
 
     for i, ax in enumerate(axs.flat):
         if i < num_images:
             title = titles[i] if titles else f"Image {i}"
-            plot_image_imshow(ax, images_data[i], cmap=cmap, title=title)
+            plot_image(ax, images_data[i], cmap=cmap, title=title, origin=origin)
             ax.axis("off")
         else:
             ax.axis("off")
 
     plt.tight_layout()
 
     if save_path:
+        save_path = save_path_file(save_path, suffix=".png")
         save_image(plt, save_path)
     else:
         plt.show()
+
+    plt.close()
```

### Comparing `medviz-0.8.8/medviz/plots/plot3d/images.py` & `medviz-0.9.1/medviz/plots/plot3d/images.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import math
 
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib.widgets import Slider
 
+from ...plots import plot_image, save_image
 from ...utils import image_path_to_data_ax
-from .. import plot_image_imshow
 
 
 def images_path(paths, rows=None, columns=None, titles=[], cmap="gray"):
     images_data = [image_path_to_data_ax(path) for path in paths]
 
     images_array(
         images_data=images_data,
@@ -35,17 +35,15 @@
         axs = np.array([axs])
 
     plt.subplots_adjust(bottom=0.25)
 
     for i, ax in enumerate(axs.flat):
         if i < num_images:
             title = titles[i] if titles else f"Image {i}"
-            plot_image_imshow(
-                ax, images_data[i][:, :, init_slice], cmap=cmap, title=title
-            )
+            plot_image(ax, images_data[i][:, :, init_slice], cmap=cmap, title=title)
             ax.axis("off")
             ax.set_xlabel(f"Slice Number: {init_slice}")
 
         else:
             ax.axis("off")
 
     slider_ax = plt.axes([0.2, 0.1, 0.6, 0.03])
@@ -64,17 +62,15 @@
 
         for i, ax in enumerate(axs.flat):
             ax.clear()
 
             if i < num_images:
                 title = titles[i] if titles else f"Image {i}"
 
-                plot_image_imshow(
-                    ax, images_data[i][:, :, slice_num], cmap=cmap, title=title
-                )
+                plot_image(ax, images_data[i][:, :, slice_num], cmap=cmap, title=title)
                 ax.set_xlabel(f"Slice Number: {slice_num}")
                 ax.axis("off")
             else:
                 ax.axis("off")
 
         # ax.set_title(title)
```

### Comparing `medviz-0.8.8/medviz/plots/plot3d/layered_plot.py` & `medviz-0.9.1/medviz/plots/plot3d/layered_plot.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,66 +1,71 @@
-from pathlib import Path
-
 import matplotlib.pyplot as plt
 from matplotlib.widgets import Slider
 
-import medviz as viz
-
-assert_shape = viz.assert_shape
-
-image_path_to_data = viz.image_path_to_data_ax
-mask_path_to_data = viz.mask_path_to_data_ax
-
-generate_mask_colors = viz.generate_mask_colors
-plot_image = viz.plot_image
-plot_contour = viz.plot_contour
+from ...plots import assert_shape, generate_mask_colors, plot_contour, plot_image
+from ...utils import image_path_to_data_ax, mask_path_to_data_ax
 
 
-def layered_plot_path3D(
-    image_path, mask_paths, mask_colors=None, title="Layered Plot", save_path=None
+def layered_slider_path(
+    image_path,
+    masks_path,
+    mask_colors=None,
+    title_image="Image",
+    titles=[],
+    cmap="gray",
+    origin="upper",
 ):
-    image_data = image_path_to_data(image_path)
+    image_data = image_path_to_data_ax(image_path)
 
-    masks_data = []
-    for mask_path in mask_paths:
-        mask_data = mask_path_to_data(mask_path)
-        masks_data.append(mask_data)
+    masks_data = [mask_path_to_data_ax(path) for path in masks_path]
 
-    layered_plot_data3D(
+    layered_slider_array(
         image_data,
         masks_data,
         mask_colors=mask_colors,
-        title=title,
-        save_path=save_path,
+        title_image=title_image,
+        titles=titles,
+        cmap=cmap,
+        origin=origin,
     )
 
 
-def layered_plot_data3D(
-    image_data, masks_data, mask_colors=None, title="Layered Plot", save_path=None
+def layered_slider_array(
+    image_data,
+    masks_data,
+    mask_colors=None,
+    title_image="Image",
+    titles=[],
+    cmap="gray",
+    origin="upper",
 ):
     print("Loading images...")
 
     num_masks = len(masks_data)
 
     init_slice, last_slice = assert_shape(image_data + masks_data)
 
     mask_colors = generate_mask_colors(num_masks, mask_colors)
 
     _, ax = plt.subplots()
     plt.subplots_adjust(bottom=0.25)
 
-    plot_image(ax, image_data[:, :, init_slice], cmap="gray")
+    plot_image(ax, image_data[:, :, init_slice], cmap=cmap)
 
     for i in range(num_masks):
         plot_contour(
-            ax, masks_data[i][:, :, init_slice], color=mask_colors[i], levels=[0.5]
+            ax,
+            masks_data[i][:, :, init_slice],
+            color=mask_colors[i],
+            # origin=origin,
+            levels=[0.5],
         )
 
     ax.set_xlabel(f"Slice Number: {init_slice}")
-    ax.set_title(title)
+    ax.set_title("title")
 
     slider_ax = plt.axes([0.2, 0.1, 0.6, 0.03])
 
     slider = Slider(
         slider_ax,
         "Slice",
         0,
@@ -74,24 +79,12 @@
         ax.clear()
 
         plot_image(ax, image_data[:, :, slice_num], cmap="gray")
         for i in range(num_masks):
             plot_contour(ax, masks_data[i][:, :, slice_num], color=mask_colors[i])
 
         ax.set_xlabel(f"Slice Number: {slice_num}")
-        ax.set_title(title)
+        ax.set_title("title")
 
     slider.on_changed(update)
 
     plt.show()
-
-    if save_path:
-        if isinstance(save_path, str):
-            save_path = Path(save_path)
-
-        if save_path.suffix != ".png":
-            save_path = save_path.with_suffix(".png")
-
-        if not save_path.parent.exists():
-            save_path.parent.mkdir(parents=True)
-
-        plt.savefig(save_path)
```

### Comparing `medviz-0.8.8/medviz/preprocess/match_image_mask.py` & `medviz-0.9.1/medviz/preprocess/match_image_mask.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from pathlib import Path
 
 import pandas as pd
 
+from ..utils import save_path_file, path_in, get_characteristics,significant_slice_idx
 
-def match_image_mask(
-    images_path, masks_path, image_func, mask_func, pattern: str, save_path="./"
-):
+
+
+def match_image_mask(images_path, masks_path, image_func, mask_func, pattern: str, save_path="./"):
     df_dict = {"ID": [], "Image": [], "Mask": []}
 
     image_paths = Path(images_path).glob(pattern)
     mask_paths = Path(masks_path).glob(pattern)
 
     images = {}
     for image_path in image_paths:
@@ -44,16 +45,20 @@
             df_dict["Image"].append(None)
         if id in masks.keys():
             df_dict["Mask"].append(masks[id])
         else:
             df_dict["Mask"].append(None)
 
     df = pd.DataFrame(df_dict, columns=df_dict.keys())
+
+    
+
     save_path = Path(save_path)
     if not save_path.exists():
         save_path.mkdir(parents=True)
 
+    
     save_path = save_path / Path("image_mask.csv")
     df.to_csv(save_path, index=False)
 
     print(f"Number of unique ids: {len(unique_ids)}")
     print(f"Number of all ids: {len(all_ids)}")
```

### Comparing `medviz-0.8.8/medviz/utils/array_profile.py` & `medviz-0.9.1/medviz/utils/array_profile.py`

 * *Files identical despite different names*

### Comparing `medviz-0.8.8/medviz/utils/array_threshold.py` & `medviz-0.9.1/medviz/utils/array_threshold.py`

 * *Files identical despite different names*

### Comparing `medviz-0.8.8/medviz/utils/helper_mask.py` & `medviz-0.9.1/medviz/utils/helper_mask.py`

 * *Files identical despite different names*

### Comparing `medviz-0.8.8/medviz/utils/log.py` & `medviz-0.9.1/medviz/utils/log.py`

 * *Files identical despite different names*

### Comparing `medviz-0.8.8/medviz.egg-info/PKG-INFO` & `medviz-0.9.1/medviz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medviz
-Version: 0.8.8
+Version: 0.9.1
 Summary: Medical Image Visualization Tool 🐍🚀🎉🦕
 Author-email: Mohsen Hariri <mohsen.hariri@case.eud>
 License: GPL-3.0 License
 Keywords: MRI,CT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `medviz-0.8.8/medviz.egg-info/SOURCES.txt` & `medviz-0.9.1/medviz.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,51 @@
 LICENSE
 MANIFEST.in
 README.rst
 VERSION
 pyproject.toml
 setup.py
 medviz/__init__.py
+medviz/bowel.py
+medviz/bowel2.py
+medviz/example.py
+medviz/fat_mul.py
 medviz.egg-info/PKG-INFO
 medviz.egg-info/SOURCES.txt
 medviz.egg-info/dependency_links.txt
 medviz.egg-info/requires.txt
 medviz.egg-info/top_level.txt
+medviz/collage/__init__.py
+medviz/collage/compute_collage.py
+medviz/collage/main.py
+medviz/collage/stats.py
 medviz/multimodal/__init__.py
 medviz/multimodal/save_dicom_metadata.py
 medviz/multimodal/stats.py
+medviz/nifti/helper.py
+medviz/pkg2/example.py
 medviz/plots/__init__.py
 medviz/plots/_plot_image.py
-medviz/plots/gif.py
 medviz/plots/helper_plot.py
 medviz/plots/layered_plot2D.py
+medviz/plots/gif/gif.py
 medviz/plots/plot2d/__init__.py
+medviz/plots/plot2d/image_mask_annotated.py
 medviz/plots/plot2d/image_masks.py
 medviz/plots/plot2d/images.py
+medviz/plots/plot2d/masks.py
 medviz/plots/plot3d/__init__.py
+medviz/plots/plot3d/image_mask_annotated.py
 medviz/plots/plot3d/images.py
 medviz/plots/plot3d/layered_plot.py
 medviz/preprocess/__init__.py
 medviz/preprocess/mask.py
 medviz/preprocess/match_image_mask.py
 medviz/utils/__init__.py
 medviz/utils/array_profile.py
 medviz/utils/array_threshold.py
 medviz/utils/custom_type.py
 medviz/utils/helper_mask.py
+medviz/utils/helper_path.py
 medviz/utils/log.py
 medviz/utils/reader.py
 medviz/utils/utility.py
```

### Comparing `medviz-0.8.8/pyproject.toml` & `medviz-0.9.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -26,26 +26,27 @@
   "pandas >= 1.2.4",
   "matplotlib >= 3.3.4",
   "nibabel >= 3.2.1",
   "imageio >= 2.9.0",
   "scikit-image >= 0.18.3",
   "tabulate >= 0.8.9",
   "pydicom >= 2.1.2",
+  "mahotas >= 1.4.11",
 ]
 
 [tool.setuptools]
-packages = ["medviz","medviz.multimodal"]
+packages = ["medviz", "medviz.multimodal", "medviz.preprocess"]
 
 
 [tool.setuptools.dynamic]
 # version = { attr = "medviz.__version__" }
-version = {file = ["VERSION"]}
+version = { file = ["VERSION"] }
 
 [tool.black]
-line-length = 88
+line-length = 110
 target-version = ["py38"]
 
 [tool.ruff]
 
 [tool.isort]
 profile = "black"
 known_first_party = "medviz"
```

