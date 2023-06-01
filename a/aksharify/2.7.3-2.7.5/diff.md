# Comparing `tmp/aksharify-2.7.3.tar.gz` & `tmp/aksharify-2.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aksharify-2.7.3.tar", max compression
+gzip compressed data, was "aksharify-2.7.5.tar", max compression
```

## Comparing `aksharify-2.7.3.tar` & `aksharify-2.7.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       24 2023-05-29 15:23:03.528860 aksharify-2.7.3/aksharify/__init__.py
--rw-r--r--   0        0        0     7763 2023-06-01 02:42:15.057908 aksharify-2.7.3/aksharify/aksharify.py
--rw-r--r--   0        0        0      923 2023-06-01 02:46:42.208155 aksharify-2.7.3/pyproject.toml
--rw-r--r--   0        0        0     5864 2023-05-30 14:27:02.119233 aksharify-2.7.3/README.md
--rw-r--r--   0        0        0     6661 1970-01-01 00:00:00.000000 aksharify-2.7.3/PKG-INFO
+-rw-r--r--   0        0        0       24 2023-05-29 15:23:03.528860 aksharify-2.7.5/aksharify/__init__.py
+-rw-r--r--   0        0        0     7763 2023-06-01 02:42:15.057908 aksharify-2.7.5/aksharify/aksharify.py
+-rw-r--r--   0        0        0      923 2023-06-01 11:44:58.412316 aksharify-2.7.5/pyproject.toml
+-rw-r--r--   0        0        0     5864 2023-05-30 14:27:02.119233 aksharify-2.7.5/README.md
+-rw-r--r--   0        0        0     6660 1970-01-01 00:00:00.000000 aksharify-2.7.5/PKG-INFO
```

### Comparing `aksharify-2.7.3/aksharify/aksharify.py` & `aksharify-2.7.5/aksharify/aksharify.py`

 * *Files identical despite different names*

### Comparing `aksharify-2.7.3/pyproject.toml` & `aksharify-2.7.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b74 6f6f 6c2e 706f 6574 7279 5d0d 0a6e  [tool.poetry]..n
 00000010: 616d 6520 3d20 2261 6b73 6861 7269 6679  ame = "aksharify
 00000020: 220d 0a76 6572 7369 6f6e 203d 2022 322e  "..version = "2.
-00000030: 372e 3322 0d0a 6465 7363 7269 7074 696f  7.3"..descriptio
+00000030: 372e 3522 0d0a 6465 7363 7269 7074 696f  7.5"..descriptio
 00000040: 6e20 3d20 2250 7974 686f 6e20 4173 6369  n = "Python Asci
 00000050: 6920 2b20 456d 6f6a 6920 4172 7420 4d6f  i + Emoji Art Mo
 00000060: 6475 6c65 220d 0a61 7574 686f 7273 203d  dule"..authors =
 00000070: 205b 2250 7269 6d65 2050 6174 656c 203c   ["Prime Patel <
 00000080: 7072 696d 6573 7061 7465 6c40 676d 6169  primespatel@gmai
 00000090: 6c2e 636f 6d3e 225d 0d0a 6c69 6365 6e73  l.com>"]..licens
 000000a0: 6520 3d20 224d 4954 220d 0a72 6561 646d  e = "MIT"..readm
@@ -44,15 +44,15 @@
 000002b0: 0a20 2020 2020 2020 2022 4f70 6572 6174  .        "Operat
 000002c0: 696e 6720 5379 7374 656d 203a 3a20 4f53  ing System :: OS
 000002d0: 2049 6e64 6570 656e 6465 6e74 222c 0d0a   Independent",..
 000002e0: 2020 2020 5d0d 0a0d 0a5b 746f 6f6c 2e70      ]....[tool.p
 000002f0: 6f65 7472 792e 6465 7065 6e64 656e 6369  oetry.dependenci
 00000300: 6573 5d0d 0a70 7974 686f 6e20 3d20 225e  es]..python = "^
 00000310: 332e 3130 220d 0a70 696c 6c6f 7720 3d20  3.10"..pillow = 
-00000320: 225e 392e 352e 3022 0d0a 7265 7175 6573  "^9.5.0"..reques
-00000330: 7473 203d 2022 5e32 2e33 312e 3022 0d0a  ts = "^2.31.0"..
+00000320: 225e 382e 342e 3022 0d0a 7265 7175 6573  "^8.4.0"..reques
+00000330: 7473 203d 2022 5e32 2e32 372e 3122 0d0a  ts = "^2.27.1"..
 00000340: 0d0a 0d0a 5b62 7569 6c64 2d73 7973 7465  ....[build-syste
 00000350: 6d5d 0d0a 7265 7175 6972 6573 203d 205b  m]..requires = [
 00000360: 2270 6f65 7472 792d 636f 7265 225d 0d0a  "poetry-core"]..
 00000370: 6275 696c 642d 6261 636b 656e 6420 3d20  build-backend = 
 00000380: 2270 6f65 7472 792e 636f 7265 2e6d 6173  "poetry.core.mas
 00000390: 6f6e 7279 2e61 7069 220d 0a              onry.api"..
```

### Comparing `aksharify-2.7.3/README.md` & `aksharify-2.7.5/README.md`

 * *Files identical despite different names*

### Comparing `aksharify-2.7.3/PKG-INFO` & `aksharify-2.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aksharify
-Version: 2.7.3
+Version: 2.7.5
 Summary: Python Ascii + Emoji Art Module
 Home-page: https://primepatel.github.io/aksharify-docs/
 License: MIT
 Keywords: Ascii Art,Emoji Art,Prime Patel,primepatel
 Author: Prime Patel
 Author-email: primespatel@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -13,16 +13,16 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: pillow (>=9.5.0,<10.0.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: pillow (>=8.4.0,<9.0.0)
+Requires-Dist: requests (>=2.27.1,<3.0.0)
 Project-URL: Repository, https://github.com/primepatel/aksharify
 Description-Content-Type: text/markdown
 
 <a name="readme-top"></a>
 
 # __Aksharify__
```

