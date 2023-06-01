# Comparing `tmp/erddaputil-0.1.0.tar.gz` & `tmp/erddaputil-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erddaputil-0.1.0.tar", last modified: Thu Mar 30 20:54:43 2023, max compression
+gzip compressed data, was "erddaputil-0.3.0.tar", last modified: Thu Jun  1 18:00:51 2023, max compression
```

## Comparing `erddaputil-0.1.0.tar` & `erddaputil-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-03-30 20:54:43.708212 erddaputil-0.1.0/
--rw-rw-rw-   0        0        0     1065 2023-03-30 20:48:34.000000 erddaputil-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      545 2023-03-30 20:54:43.708212 erddaputil-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       23 2023-03-30 20:50:10.000000 erddaputil-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-30 20:54:43.707210 erddaputil-0.1.0/erddaputil.egg-info/
--rw-rw-rw-   0        0        0      545 2023-03-30 20:54:43.000000 erddaputil-0.1.0/erddaputil.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      211 2023-03-30 20:54:43.000000 erddaputil-0.1.0/erddaputil.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-30 20:54:43.000000 erddaputil-0.1.0/erddaputil.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       86 2023-03-30 20:54:43.000000 erddaputil-0.1.0/erddaputil.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-03-30 20:54:43.000000 erddaputil-0.1.0/erddaputil.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       88 2022-11-14 15:30:25.000000 erddaputil-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      784 2023-03-30 20:54:43.709181 erddaputil-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-01 18:00:51.368094 erddaputil-0.3.0/
+-rw-rw-rw-   0        0        0     1065 2023-04-19 19:36:54.000000 erddaputil-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     2866 2023-06-01 18:00:51.368094 erddaputil-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2180 2023-06-01 17:55:57.000000 erddaputil-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 18:00:51.364092 erddaputil-0.3.0/erddaputil.egg-info/
+-rw-rw-rw-   0        0        0     2866 2023-06-01 18:00:51.000000 erddaputil-0.3.0/erddaputil.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-06-01 18:00:51.000000 erddaputil-0.3.0/erddaputil.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 18:00:51.000000 erddaputil-0.3.0/erddaputil.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      259 2023-06-01 18:00:51.000000 erddaputil-0.3.0/erddaputil.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 18:00:51.000000 erddaputil-0.3.0/erddaputil.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       88 2023-04-19 19:36:54.000000 erddaputil-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1074 2023-06-01 18:00:51.369092 erddaputil-0.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-01 18:00:51.366092 erddaputil-0.3.0/tests/
+-rw-rw-rw-   0        0        0    50489 2023-05-17 18:30:57.000000 erddaputil-0.3.0/tests/test_erddap_manager.py
```

### Comparing `erddaputil-0.1.0/LICENSE` & `erddaputil-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `erddaputil-0.1.0/setup.cfg` & `erddaputil-0.3.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 7264 6461 7075 7469 6c0d 0a76   = erddaputil..v
-00000020: 6572 7369 6f6e 203d 2030 2e31 2e30 0d0a  ersion = 0.1.0..
+00000020: 6572 7369 6f6e 203d 2030 2e33 2e30 0d0a  ersion = 0.3.0..
 00000030: 6175 7468 6f72 203d 2045 7269 6e20 5475  author = Erin Tu
 00000040: 726e 6275 6c6c 0d0a 6175 7468 6f72 5f65  rnbull..author_e
 00000050: 6d61 696c 203d 2065 7269 6e2e 612e 7475  mail = erin.a.tu
 00000060: 726e 6275 6c6c 4067 6d61 696c 2e63 6f6d  rnbull@gmail.com
 00000070: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 00000080: 546f 6f6c 7320 666f 7220 6d61 6e61 6769  Tools for managi
 00000090: 6e67 2045 5244 4441 500d 0a6c 6f6e 675f  ng ERDDAP..long_
@@ -16,34 +16,53 @@
 000000f0: 6c20 3d20 6874 7470 733a 2f2f 6769 7468  l = https://gith
 00000100: 7562 2e63 6f6d 2f64 666f 2d6d 6564 732f  ub.com/dfo-meds/
 00000110: 6572 6464 6170 7574 696c 0d0a 7072 6f6a  erddaputil..proj
 00000120: 6563 745f 7572 6c73 203d 200d 0a09 4275  ect_urls = ...Bu
 00000130: 6720 5472 6163 6b65 7220 3d20 6874 7470  g Tracker = http
 00000140: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f64  s://github.com/d
 00000150: 666f 2d6d 6564 732f 6572 6464 6170 7574  fo-meds/erddaput
-00000160: 696c 2f69 7373 7565 730d 0a63 6c61 7373  il/issues..class
-00000170: 6966 6965 7273 203d 200d 0a09 5072 6f67  ifiers = ...Prog
-00000180: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000190: 203a 3a20 5079 7468 6f6e 203a 3a20 330d   :: Python :: 3.
-000001a0: 0a09 4c69 6365 6e73 6520 3a3a 204f 5349  ..License :: OSI
-000001b0: 2041 7070 726f 7665 6420 3a3a 204d 4954   Approved :: MIT
-000001c0: 204c 6963 656e 7365 0d0a 094f 7065 7261   License...Opera
-000001d0: 7469 6e67 2053 7973 7465 6d20 3a3a 204f  ting System :: O
-000001e0: 5320 496e 6465 7065 6e64 656e 740d 0a0d  S Independent...
-000001f0: 0a5b 6f70 7469 6f6e 735d 0d0a 7061 636b  .[options]..pack
-00000200: 6167 655f 6469 7220 3d20 0d0a 093d 202e  age_dir = ...= .
-00000210: 0d0a 7061 636b 6167 6573 203d 2066 696e  ..packages = fin
-00000220: 643a 0d0a 7079 7468 6f6e 5f72 6571 7569  d:..python_requi
-00000230: 7265 7320 3d20 3e3d 332e 370d 0a69 6e73  res = >=3.7..ins
-00000240: 7461 6c6c 5f72 6571 7569 7265 7320 3d20  tall_requires = 
-00000250: 0d0a 097a 6972 636f 6e69 756d 0d0a 0961  ...zirconium...a
-00000260: 7574 6f69 6e6a 6563 740d 0a09 7a72 6c6f  utoinject...zrlo
-00000270: 670d 0a09 636c 6963 6b0d 0a09 7265 7175  g...click...requ
-00000280: 6573 7473 0d0a 0961 696f 6874 7470 0d0a  ests...aiohttp..
-00000290: 0970 726f 6d65 7468 6575 735f 636c 6965  .prometheus_clie
-000002a0: 6e74 0d0a 0966 6c61 736b 0d0a 0970 7979  nt...flask...pyy
-000002b0: 616d 6c0d 0a09 746f 6d6c 0d0a 0d0a 5b6f  aml...toml....[o
-000002c0: 7074 696f 6e73 2e70 6163 6b61 6765 732e  ptions.packages.
-000002d0: 6669 6e64 5d0d 0a77 6865 7265 203d 2073  find]..where = s
-000002e0: 7263 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  rc....[egg_info]
-000002f0: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
-00000300: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
+00000160: 696c 2f69 7373 7565 730d 0a09 446f 6375  il/issues...Docu
+00000170: 6d65 6e74 6174 696f 6e20 3d20 6874 7470  mentation = http
+00000180: 733a 2f2f 6572 6464 6170 7574 696c 2e72  s://erddaputil.r
+00000190: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
+000001a0: 2f6c 6174 6573 742f 0d0a 636c 6173 7369  /latest/..classi
+000001b0: 6669 6572 7320 3d20 0d0a 0950 726f 6772  fiers = ...Progr
+000001c0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+000001d0: 3a3a 2050 7974 686f 6e20 3a3a 2033 0d0a  :: Python :: 3..
+000001e0: 094c 6963 656e 7365 203a 3a20 4f53 4920  .License :: OSI 
+000001f0: 4170 7072 6f76 6564 203a 3a20 4d49 5420  Approved :: MIT 
+00000200: 4c69 6365 6e73 650d 0a09 4f70 6572 6174  License...Operat
+00000210: 696e 6720 5379 7374 656d 203a 3a20 4f53  ing System :: OS
+00000220: 2049 6e64 6570 656e 6465 6e74 0d0a 0d0a   Independent....
+00000230: 5b6f 7074 696f 6e73 5d0d 0a70 6163 6b61  [options]..packa
+00000240: 6765 5f64 6972 203d 200d 0a09 3d20 2e0d  ge_dir = ...= ..
+00000250: 0a70 6163 6b61 6765 7320 3d20 6669 6e64  .packages = find
+00000260: 3a0d 0a70 7974 686f 6e5f 7265 7175 6972  :..python_requir
+00000270: 6573 203d 203e 3d33 2e37 0d0a 696e 7374  es = >=3.7..inst
+00000280: 616c 6c5f 7265 7175 6972 6573 203d 200d  all_requires = .
+00000290: 0a09 7a69 7263 6f6e 6975 6d3e 3d31 2e32  ..zirconium>=1.2
+000002a0: 2e34 0d0a 0961 7574 6f69 6e6a 6563 743e  .4...autoinject>
+000002b0: 3d31 2e33 2e32 0d0a 097a 726c 6f67 3e3d  =1.3.2...zrlog>=
+000002c0: 302e 332e 300d 0a09 636c 6963 6b0d 0a09  0.3.0...click...
+000002d0: 6169 6f68 7474 700d 0a09 7265 7175 6573  aiohttp...reques
+000002e0: 7473 0d0a 0970 726f 6d65 7468 6575 735f  ts...prometheus_
+000002f0: 636c 6965 6e74 0d0a 0966 6c61 736b 0d0a  client...flask..
+00000300: 0970 7979 616d 6c0d 0a09 746f 6d6c 0d0a  .pyyaml...toml..
+00000310: 0962 7334 0d0a 0d0a 5b6f 7074 696f 6e73  .bs4....[options
+00000320: 2e65 7874 7261 735f 7265 7175 6972 655d  .extras_require]
+00000330: 0d0a 6173 6220 3d20 0d0a 0961 7a75 7265  ..asb = ...azure
+00000340: 2d69 6465 6e74 6974 790d 0a09 617a 7572  -identity...azur
+00000350: 652d 7374 6f72 6167 652d 626c 6f62 0d0a  e-storage-blob..
+00000360: 0961 7a75 7265 2d73 6572 7669 6365 6275  .azure-servicebu
+00000370: 730d 0a72 6162 6269 746d 7120 3d20 0d0a  s..rabbitmq = ..
+00000380: 0970 696b 610d 0a64 6576 203d 200d 0a09  .pika..dev = ...
+00000390: 7477 696e 650d 0a09 6275 696c 640d 0a09  twine...build...
+000003a0: 7370 6869 6e78 0d0a 0973 7068 696e 782d  sphinx...sphinx-
+000003b0: 746f 6f6c 626f 780d 0a09 7370 6869 6e78  toolbox...sphinx
+000003c0: 2d63 6c69 636b 0d0a 7765 6261 7070 203d  -click..webapp =
+000003d0: 200d 0a09 7761 6974 7265 7373 0d0a 0d0a   ...waitress....
+000003e0: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
+000003f0: 732e 6669 6e64 5d0d 0a77 6865 7265 203d  s.find]..where =
+00000400: 2073 7263 0d0a 0d0a 5b65 6767 5f69 6e66   src....[egg_inf
+00000410: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
+00000420: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
+00000430: 0d0a                                     ..
```

