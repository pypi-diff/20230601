# Comparing `tmp/bspy-0.0.2.tar.gz` & `tmp/bspy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bspy-0.0.2.tar", last modified: Mon Mar  7 20:04:57 2022, max compression
+gzip compressed data, was "bspy-1.0.1.tar", last modified: Wed May 31 23:45:55 2023, max compression
```

## Comparing `bspy-0.0.2.tar` & `bspy-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,24 @@
-drwxrwxrwx   0        0        0        0 2022-03-07 20:04:57.216418 bspy-0.0.2/
--rw-rw-rw-   0        0        0     1091 2021-12-05 20:22:58.000000 bspy-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     1460 2022-03-07 20:04:57.216418 bspy-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      324 2022-03-07 19:58:46.000000 bspy-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2022-03-07 20:04:57.182513 bspy-0.0.2/bspy/
-drwxrwxrwx   0        0        0        0 2022-03-07 20:04:57.214424 bspy-0.0.2/bspy/bspy.egg-info/
--rw-rw-rw-   0        0        0     1460 2022-03-07 20:04:56.000000 bspy-0.0.2/bspy/bspy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      174 2022-03-07 20:04:57.000000 bspy-0.0.2/bspy/bspy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-03-07 20:04:56.000000 bspy-0.0.2/bspy/bspy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2022-03-07 20:04:57.000000 bspy-0.0.2/bspy/bspy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2022-02-22 07:11:51.000000 bspy-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0     1178 2022-03-07 20:04:57.222403 bspy-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-31 23:45:54.997211 bspy-1.0.1/
+-rw-rw-rw-   0        0        0     1091 2021-12-05 20:22:58.000000 bspy-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     3624 2023-05-31 23:45:54.998208 bspy-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2509 2023-05-31 22:33:10.000000 bspy-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 23:45:54.947148 bspy-1.0.1/bspy/
+-rw-rw-rw-   0        0        0      851 2022-02-20 16:04:59.000000 bspy-1.0.1/bspy/__init__.py
+-rw-rw-rw-   0        0        0    26824 2023-05-27 22:15:48.000000 bspy-1.0.1/bspy/_spline_domain.py
+-rw-rw-rw-   0        0        0     5094 2023-05-27 22:11:33.000000 bspy-1.0.1/bspy/_spline_evaluation.py
+-rw-rw-rw-   0        0        0     6951 2023-05-30 15:31:32.000000 bspy-1.0.1/bspy/_spline_fitting.py
+-rw-rw-rw-   0        0        0     3394 2023-05-27 22:15:35.000000 bspy-1.0.1/bspy/_spline_intersection.py
+-rw-rw-rw-   0        0        0    30613 2023-05-27 22:16:57.000000 bspy-1.0.1/bspy/_spline_operations.py
+-rw-rw-rw-   0        0        0    14524 2022-03-06 05:40:47.000000 bspy-1.0.1/bspy/bspyApp.py
+-rw-rw-rw-   0        0        0    16737 2022-03-07 01:45:17.000000 bspy-1.0.1/bspy/drawableSpline.py
+-rw-rw-rw-   0        0        0    45950 2023-05-31 22:01:34.000000 bspy-1.0.1/bspy/spline.py
+-rw-rw-rw-   0        0        0    60616 2022-03-07 01:47:01.000000 bspy-1.0.1/bspy/splineOpenGLFrame.py
+drwxrwxrwx   0        0        0        0 2023-05-31 23:45:54.975733 bspy-1.0.1/bspy.egg-info/
+-rw-rw-rw-   0        0        0     3624 2023-05-31 23:45:54.000000 bspy-1.0.1/bspy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      400 2023-05-31 23:45:54.000000 bspy-1.0.1/bspy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 23:45:54.000000 bspy-1.0.1/bspy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-05-31 23:45:54.000000 bspy-1.0.1/bspy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2022-02-22 07:11:51.000000 bspy-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1111 2023-05-31 23:45:55.001214 bspy-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-31 23:45:54.994212 bspy-1.0.1/tests/
+-rw-rw-rw-   0        0        0    66440 2023-05-30 15:34:50.000000 bspy-1.0.1/tests/test_bspy.py
```

### Comparing `bspy-0.0.2/LICENSE` & `bspy-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bspy-0.0.2/setup.cfg` & `bspy-1.0.1/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2062 7370 790d 0a76 6572 7369 6f6e   = bspy..version
-00000020: 203d 2030 2e30 2e32 0d0a 6175 7468 6f72   = 0.0.2..author
+00000020: 203d 2031 2e30 2e31 0d0a 6175 7468 6f72   = 1.0.1..author
 00000030: 203d 2045 7269 6320 4272 6563 686e 6572   = Eric Brechner
 00000040: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000050: 2065 7269 6362 7265 6340 6d73 6e2e 636f   ericbrec@msn.co
 00000060: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
 00000070: 204c 6962 7261 7279 2066 6f72 206d 616e   Library for man
 00000080: 6970 756c 6174 696e 6720 616e 6420 7265  ipulating and re
 00000090: 6e64 6572 696e 6720 6e6f 6e2d 756e 6966  ndering non-unif
@@ -58,17 +58,13 @@
 00000390: 6172 6965 7320 3a3a 2050 7974 686f 6e20  aries :: Python 
 000003a0: 4d6f 6475 6c65 730d 0a09 5072 6f67 7261  Modules...Progra
 000003b0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
 000003c0: 3a20 5079 7468 6f6e 203a 3a20 330d 0a09  : Python :: 3...
 000003d0: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
 000003e0: 203a 3a20 4f53 2049 6e64 6570 656e 6465   :: OS Independe
 000003f0: 6e74 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d  nt....[options].
-00000400: 0a70 6163 6b61 6765 5f64 6972 203d 200d  .package_dir = .
-00000410: 0a09 3d20 6273 7079 0d0a 7061 636b 6167  ..= bspy..packag
-00000420: 6573 203d 2066 696e 643a 0d0a 7079 7468  es = find:..pyth
-00000430: 6f6e 5f72 6571 7569 7265 7320 3d20 3e3d  on_requires = >=
-00000440: 332e 300d 0a0d 0a5b 6f70 7469 6f6e 732e  3.0....[options.
-00000450: 7061 636b 6167 6573 2e66 696e 645d 0d0a  packages.find]..
-00000460: 7768 6572 6520 3d20 6273 7079 0d0a 0d0a  where = bspy....
-00000470: 5b65 6767 5f69 6e66 6f5d 0d0a 7461 675f  [egg_info]..tag_
-00000480: 6275 696c 6420 3d20 0d0a 7461 675f 6461  build = ..tag_da
-00000490: 7465 203d 2030 0d0a 0d0a                 te = 0....
+00000400: 0a70 6163 6b61 6765 7320 3d20 6273 7079  .packages = bspy
+00000410: 0d0a 7079 7468 6f6e 5f72 6571 7569 7265  ..python_require
+00000420: 7320 3d20 3e3d 332e 300d 0a0d 0a5b 6567  s = >=3.0....[eg
+00000430: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
+00000440: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
+00000450: 3d20 300d 0a0d 0a                        = 0....
```

