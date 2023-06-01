# Comparing `tmp/sdss-tree-3.1.7.tar.gz` & `tmp/sdss-tree-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sdss-tree-3.1.7.tar", last modified: Wed May 31 12:55:26 2023, max compression
+gzip compressed data, was "dist/sdss-tree-4.0.0.tar", last modified: Thu Jun  1 19:38:32 2023, max compression
```

## Comparing `sdss-tree-3.1.7.tar` & `sdss-tree-4.0.0.tar`

### file list

```diff
@@ -1,54 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:55:26.000000 sdss-tree-3.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-31 12:55:26.000000 sdss-tree-3.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:55:26.000000 sdss-tree-3.1.7/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)    20812 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/bin/setup_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:55:26.000000 sdss-tree-3.1.7/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:55:26.000000 sdss-tree-3.1.7/python/sdss_tree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-31 12:55:26.000000 sdss-tree-3.1.7/python/sdss_tree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-31 12:55:26.000000 sdss-tree-3.1.7/python/sdss_tree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 12:55:26.000000 sdss-tree-3.1.7/python/sdss_tree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 12:55:26.000000 sdss-tree-3.1.7/python/sdss_tree.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-31 12:55:26.000000 sdss-tree-3.1.7/python/sdss_tree.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-31 12:55:26.000000 sdss-tree-3.1.7/python/sdss_tree.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:55:26.000000 sdss-tree-3.1.7/python/tree/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11445 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/changelog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:55:26.000000 sdss-tree-3.1.7/python/tree/data/
--rw-r--r--   0 runner    (1001) docker     (123)    22519 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/basework.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/bosswork.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/dr10.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/dr11.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/dr12.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/dr13.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/dr14.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/dr15.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/dr16.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/dr17.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/dr18.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/dr7.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    14091 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/dr8.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/dr9.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    11435 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/ipl1.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/ipl2.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/mpl10.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/mpl11.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/mpl3.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/mpl4.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/mpl5.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/mpl6.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/mpl7.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/mpl8.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/mpl9.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    25151 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/sdss5.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    13212 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/data/sdsswork.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:55:26.000000 sdss-tree-3.1.7/python/tree/etc/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/etc/tree.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:55:26.000000 sdss-tree-3.1.7/python/tree/misc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8550 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/misc/docutree.py
--rw-r--r--   0 runner    (1001) docker     (123)    31512 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/python/tree/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-05-31 12:55:26.000000 sdss-tree-3.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-31 12:55:12.000000 sdss-tree-3.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:32.000000 sdss-tree-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-01 19:38:20.000000 sdss-tree-4.0.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-01 19:38:20.000000 sdss-tree-4.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-06-01 19:38:32.000000 sdss-tree-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-06-01 19:38:20.000000 sdss-tree-4.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:32.000000 sdss-tree-4.0.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20992 2023-06-01 19:38:20.000000 sdss-tree-4.0.0/bin/setup_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:32.000000 sdss-tree-4.0.0/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:32.000000 sdss-tree-4.0.0/python/sdss_tree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-06-01 19:38:32.000000 sdss-tree-4.0.0/python/sdss_tree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-01 19:38:32.000000 sdss-tree-4.0.0/python/sdss_tree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 19:38:32.000000 sdss-tree-4.0.0/python/sdss_tree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 19:38:32.000000 sdss-tree-4.0.0/python/sdss_tree.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-01 19:38:32.000000 sdss-tree-4.0.0/python/sdss_tree.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-01 19:38:32.000000 sdss-tree-4.0.0/python/sdss_tree.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:32.000000 sdss-tree-4.0.0/python/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-01 19:38:20.000000 sdss-tree-4.0.0/python/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11445 2023-06-01 19:38:20.000000 sdss-tree-4.0.0/python/tree/changelog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:32.000000 sdss-tree-4.0.0/python/tree/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-06-01 19:38:20.000000 sdss-tree-4.0.0/python/tree/data/dr10.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-06-01 19:38:20.000000 sdss-tree-4.0.0/python/tree/data/dr11.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-01 19:38:20.000000 sdss-tree-4.0.0/python/tree/data/dr12.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-06-01 19:38:20.000000 sdss-tree-4.0.0/python/tree/data/dr13.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-01 19:38:20.000000 sdss-tree-4.0.0/python/tree/data/dr14.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-01 19:38:20.000000 sdss-tree-4.0.0/python/tree/data/dr15.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-06-01 19:38:20.000000 sdss-tree-4.0.0/python/tree/data/dr16.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-06-01 19:38:20.000000 sdss-tree-4.0.0/python/tree/data/dr17.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-06-01 19:38:20.000000 sdss-tree-4.0.0/python/tree/data/dr18.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-06-01 19:38:20.000000 sdss-tree-4.0.0/python/tree/data/dr7.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    14091 2023-06-01 19:38:20.000000 sdss-tree-4.0.0/python/tree/data/dr8.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-06-01 19:38:20.000000 sdss-tree-4.0.0/python/tree/data/dr9.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    11435 2023-06-01 19:38:20.000000 sdss-tree-4.0.0/python/tree/data/ipl1.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-01 19:38:20.000000 sdss-tree-4.0.0/python/tree/data/ipl2.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    25862 2023-06-01 19:38:20.000000 sdss-tree-4.0.0/python/tree/data/sdsswork.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:32.000000 sdss-tree-4.0.0/python/tree/etc/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-01 19:38:20.000000 sdss-tree-4.0.0/python/tree/etc/tree.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:32.000000 sdss-tree-4.0.0/python/tree/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:20.000000 sdss-tree-4.0.0/python/tree/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8550 2023-06-01 19:38:20.000000 sdss-tree-4.0.0/python/tree/misc/docutree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31512 2023-06-01 19:38:20.000000 sdss-tree-4.0.0/python/tree/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-06-01 19:38:32.000000 sdss-tree-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-01 19:38:20.000000 sdss-tree-4.0.0/setup.py
```

### Comparing `sdss-tree-3.1.7/LICENSE.md` & `sdss-tree-4.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss-tree-3.1.7/bin/setup_tree.py` & `sdss-tree-4.0.0/bin/setup_tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -459,14 +459,20 @@
     if default:
         defpath = os.path.join(tree_mod, 'default')
         realpath = default
         if os.path.islink(defpath):
             os.unlink(defpath)
         os.symlink(realpath, defpath)
 
+    # create a symlink from sdsswork to sdss5
+    path5 = os.path.join(tree_mod, 'sdss5')
+    if os.path.islink(path5):
+        os.unlink(path5)
+    os.symlink('sdsswork', path5)
+
 
 def check_output_dir(output_dir):
     ''' Check the output directory '''
 
     # check if output directory is within a pip package directory
     if 'site-packages' in output_dir or output_dir.endswith('python/tree/etc'):
         output_dir = os.path.expanduser('~/.tree/environments')
```

### Comparing `sdss-tree-3.1.7/python/sdss_tree.egg-info/requires.txt` & `sdss-tree-4.0.0/python/sdss_tree.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `sdss-tree-3.1.7/python/tree/changelog.py` & `sdss-tree-4.0.0/python/tree/changelog.py`

 * *Files identical despite different names*

### Comparing `sdss-tree-3.1.7/python/tree/data/dr10.cfg` & `sdss-tree-4.0.0/python/tree/data/dr10.cfg`

 * *Files identical despite different names*

### Comparing `sdss-tree-3.1.7/python/tree/data/dr11.cfg` & `sdss-tree-4.0.0/python/tree/data/dr11.cfg`

 * *Files identical despite different names*

### Comparing `sdss-tree-3.1.7/python/tree/data/dr12.cfg` & `sdss-tree-4.0.0/python/tree/data/dr12.cfg`

 * *Files identical despite different names*

### Comparing `sdss-tree-3.1.7/python/tree/data/dr13.cfg` & `sdss-tree-4.0.0/python/tree/data/dr13.cfg`

 * *Files identical despite different names*

### Comparing `sdss-tree-3.1.7/python/tree/data/dr14.cfg` & `sdss-tree-4.0.0/python/tree/data/dr14.cfg`

 * *Files identical despite different names*

### Comparing `sdss-tree-3.1.7/python/tree/data/dr15.cfg` & `sdss-tree-4.0.0/python/tree/data/dr15.cfg`

 * *Files identical despite different names*

### Comparing `sdss-tree-3.1.7/python/tree/data/dr16.cfg` & `sdss-tree-4.0.0/python/tree/data/dr16.cfg`

 * *Files identical despite different names*

### Comparing `sdss-tree-3.1.7/python/tree/data/dr17.cfg` & `sdss-tree-4.0.0/python/tree/data/dr17.cfg`

 * *Files identical despite different names*

### Comparing `sdss-tree-3.1.7/python/tree/data/dr18.cfg` & `sdss-tree-4.0.0/python/tree/data/dr18.cfg`

 * *Files identical despite different names*

### Comparing `sdss-tree-3.1.7/python/tree/data/dr7.cfg` & `sdss-tree-4.0.0/python/tree/data/dr7.cfg`

 * *Files identical despite different names*

### Comparing `sdss-tree-3.1.7/python/tree/data/dr8.cfg` & `sdss-tree-4.0.0/python/tree/data/dr8.cfg`

 * *Files identical despite different names*

### Comparing `sdss-tree-3.1.7/python/tree/data/dr9.cfg` & `sdss-tree-4.0.0/python/tree/data/dr9.cfg`

 * *Files identical despite different names*

### Comparing `sdss-tree-3.1.7/python/tree/data/ipl1.cfg` & `sdss-tree-4.0.0/python/tree/data/ipl1.cfg`

 * *Files identical despite different names*

### Comparing `sdss-tree-3.1.7/python/tree/data/ipl2.cfg` & `sdss-tree-4.0.0/python/tree/data/ipl2.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 #
 # Tree configuration for SDSS-V IPL-2 release
 #
+# inherits from IPL-1
+# this file only contains new, or modified, environment variables or paths from IPL-1
 #
 [DEFAULT]
 FILESYSTEM = @FILESYSTEM@
-name = ipl2 current = True
+name = ipl2
+current = True
 phase = 5
 base = ipl1
 release_date = 2023-03-01
 
 [BHM]
 name = ipl-2
```

### Comparing `sdss-tree-3.1.7/python/tree/data/sdss5.cfg` & `sdss-tree-4.0.0/python/tree/data/sdsswork.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #
-# Tree configuration for SDSS-V
+# Tree configuration for SDSS-V, sdsswork, i.e. unreleased data
+#
+# this file should contain those envvars and paths unique to sdsswork
 #
 
 [DEFAULT]
 FILESYSTEM = @FILESYSTEM@
-name = sdss5
+name = sdsswork
 current = True
 phase = 5
 release_date = None
 #
 #
 #
 [general]
@@ -124,14 +126,24 @@
 #
 [MOS]
 name = sdsswork
 MOS_ROOT = %(FILESYSTEM)s/%(name)s/mos
 MOS_TARGET = %(MOS_ROOT)s/target
 #
 #
+# PATHS holds sdss_access path definitions; sdsswork contains path definitions for temporary files,
+# work files, or files not yet releases.  Specific path changes are versioned in
+# drXX.cfg or iplXX.cfg config files.
+#
+# Rules:
+# - paths referencing files released in DRs should be duplicated in their respective drXX.cfg files
+# - paths referencing internally released data should go in their own IPL file, e.g. ipl1.cfg
+# - each new dr or ipl config file inherits from the previous release, and only contains paths
+#   that are new to that release, or have been modified from the previous release.
+#
 [PATHS]
 # robostrategy paths
 rsAllocation = $ROBOSTRATEGY_DATA/allocations/{plan}/rsAllocation-{plan}-{observatory}.fits
 rsAllocationFinal = $ROBOSTRATEGY_DATA/allocations/{plan}/final/rsAllocationFinal-{plan}-{observatory}.fits
 rsAllocationPng = $ROBOSTRATEGY_DATA/allocations/{plan}/rsAllocation-{name}-{plan}-{observatory}.png
 rsAllocationHtml = $ROBOSTRATEGY_DATA/allocations/{plan}/rsAllocation-{plan}-{observatory}.html
 rsAssignments = $ROBOSTRATEGY_DATA/allocations/{plan}/rsAssignments-{plan}-{observatory}.fits
```

### Comparing `sdss-tree-3.1.7/python/tree/misc/docutree.py` & `sdss-tree-4.0.0/python/tree/misc/docutree.py`

 * *Files identical despite different names*

### Comparing `sdss-tree-3.1.7/python/tree/tree.py` & `sdss-tree-4.0.0/python/tree/tree.py`

 * *Files identical despite different names*

### Comparing `sdss-tree-3.1.7/setup.cfg` & `sdss-tree-4.0.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sdss-tree
-version = 3.1.7
+version = 4.0.0
 author = Brian Cherinka
 author_email = bcherinka@stsci.edu
 description = Control and setup of SDSS tree environment and modules
 url = https://github.com/sdss/tree
 project_urls = 
 	Repository = https://github.com/sdss/tree
 	Documentation = https://sdss-tree.readthedocs.org
@@ -99,15 +99,15 @@
 	W504
 	W505
 per-file-ignores = 
 	*/__init__.py:E,W
 max-line-length = 99
 
 [tool:pytest]
-addopts = --cov tree --cov-report html -W ignore
+addopts = --cov tree --cov-report xml --cov-report html --cov-report term -W ignore
 
 [coverage:run]
 branch = true
 include = 
 	python/tree/*
 omit = 
 	*/utils/*.py
```

