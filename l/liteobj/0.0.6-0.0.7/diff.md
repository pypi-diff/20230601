# Comparing `tmp/liteobj-0.0.6.tar.gz` & `tmp/liteobj-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liteobj-0.0.6.tar", last modified: Thu Jun  1 21:12:54 2023, max compression
+gzip compressed data, was "liteobj-0.0.7.tar", last modified: Thu Jun  1 21:37:47 2023, max compression
```

## Comparing `liteobj-0.0.6.tar` & `liteobj-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-01 21:12:54.372393 liteobj-0.0.6/
--rwxr-xr-x   0 user      (1000) user      (1000)    11538 2023-05-25 22:18:19.000000 liteobj-0.0.6/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)      255 2023-06-01 21:12:54.372393 liteobj-0.0.6/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     1221 2023-06-01 19:00:09.000000 liteobj-0.0.6/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-01 21:12:54.372393 liteobj-0.0.6/liteobj/
--rw-r--r--   0 user      (1000) user      (1000)       97 2023-06-01 21:10:19.000000 liteobj-0.0.6/liteobj/__init__.py
--rwxr-xr-x   0 user      (1000) user      (1000)     3897 2023-06-01 21:04:12.000000 liteobj-0.0.6/liteobj/lite.py
--rw-r--r--   0 user      (1000) user      (1000)       28 2023-05-25 21:59:58.000000 liteobj-0.0.6/liteobj/requirements.txt
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-01 21:12:54.372393 liteobj-0.0.6/liteobj.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)      255 2023-06-01 21:12:54.000000 liteobj-0.0.6/liteobj.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      286 2023-06-01 21:12:54.000000 liteobj-0.0.6/liteobj.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-06-01 21:12:54.000000 liteobj-0.0.6/liteobj.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       38 2023-06-01 21:12:54.000000 liteobj-0.0.6/liteobj.egg-info/entry_points.txt
--rw-r--r--   0 user      (1000) user      (1000)       29 2023-06-01 21:12:54.000000 liteobj-0.0.6/liteobj.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)        8 2023-06-01 21:12:54.000000 liteobj-0.0.6/liteobj.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)       38 2023-06-01 21:12:54.372393 liteobj-0.0.6/setup.cfg
--rwxr-xr-x   0 user      (1000) user      (1000)      767 2023-06-01 21:12:51.000000 liteobj-0.0.6/setup.py
--rw-r--r--   0 user      (1000) user      (1000)       21 2023-06-01 21:09:46.000000 liteobj-0.0.6/version.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-01 21:37:47.772456 liteobj-0.0.7/
+-rwxr-xr-x   0 user      (1000) user      (1000)    11538 2023-05-25 22:18:19.000000 liteobj-0.0.7/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)      255 2023-06-01 21:37:47.772456 liteobj-0.0.7/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     1221 2023-06-01 19:00:09.000000 liteobj-0.0.7/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-01 21:37:47.772456 liteobj-0.0.7/liteobj/
+-rw-r--r--   0 user      (1000) user      (1000)       93 2023-06-01 21:37:36.000000 liteobj-0.0.7/liteobj/__init__.py
+-rwxr-xr-x   0 user      (1000) user      (1000)     3897 2023-06-01 21:04:12.000000 liteobj-0.0.7/liteobj/lite.py
+-rw-r--r--   0 user      (1000) user      (1000)       28 2023-05-25 21:59:58.000000 liteobj-0.0.7/liteobj/requirements.txt
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-01 21:37:47.772456 liteobj-0.0.7/liteobj.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)      255 2023-06-01 21:37:47.000000 liteobj-0.0.7/liteobj.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      275 2023-06-01 21:37:47.000000 liteobj-0.0.7/liteobj.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-06-01 21:37:47.000000 liteobj-0.0.7/liteobj.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       38 2023-06-01 21:37:47.000000 liteobj-0.0.7/liteobj.egg-info/entry_points.txt
+-rw-r--r--   0 user      (1000) user      (1000)       29 2023-06-01 21:37:47.000000 liteobj-0.0.7/liteobj.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)        8 2023-06-01 21:37:47.000000 liteobj-0.0.7/liteobj.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)       38 2023-06-01 21:37:47.772456 liteobj-0.0.7/setup.cfg
+-rwxr-xr-x   0 user      (1000) user      (1000)      849 2023-06-01 21:35:12.000000 liteobj-0.0.7/setup.py
```

### Comparing `liteobj-0.0.6/LICENSE` & `liteobj-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `liteobj-0.0.6/README.md` & `liteobj-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `liteobj-0.0.6/liteobj/lite.py` & `liteobj-0.0.7/liteobj/lite.py`

 * *Files identical despite different names*

### Comparing `liteobj-0.0.6/setup.py` & `liteobj-0.0.7/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,48 +1,54 @@
 00000000: 0d0a 6672 6f6d 2073 6574 7570 746f 6f6c  ..from setuptool
 00000010: 7320 696d 706f 7274 2073 6574 7570 0d0a  s import setup..
-00000020: 6672 6f6d 2076 6572 7369 6f6e 2069 6d70  from version imp
-00000030: 6f72 7420 5f5f 7665 7273 696f 6e5f 5f0d  ort __version__.
-00000040: 0a0d 0a72 6570 6f5f 6e61 6d65 203d 2027  ...repo_name = '
-00000050: 6c69 7465 6f62 6a27 0d0a 0d0a 7265 7175  liteobj'....requ
-00000060: 6972 656d 656e 7473 5f66 6e20 3d20 2272  irements_fn = "r
-00000070: 6571 7569 7265 6d65 6e74 732e 7478 7422  equirements.txt"
-00000080: 0d0a 696e 7374 616c 6c5f 7265 7175 6972  ..install_requir
-00000090: 656d 656e 7473 203d 206f 7065 6e28 6622  ements = open(f"
-000000a0: 7b72 6570 6f5f 6e61 6d65 7d2f 7b72 6571  {repo_name}/{req
-000000b0: 7569 7265 6d65 6e74 735f 666e 7d22 292e  uirements_fn}").
-000000c0: 7265 6164 2829 2e73 706c 6974 2829 0d0a  read().split()..
-000000d0: 0d0a 7365 7475 7028 6e61 6d65 3d72 6570  ..setup(name=rep
-000000e0: 6f5f 6e61 6d65 2c0d 0a20 2020 2020 2076  o_name,..      v
-000000f0: 6572 7369 6f6e 3d5f 5f76 6572 7369 6f6e  ersion=__version
-00000100: 5f5f 2c0d 0a20 2020 2020 2064 6573 6372  __,..      descr
-00000110: 6970 7469 6f6e 3d27 4372 6561 7465 206c  iption='Create l
-00000120: 6967 6874 7765 6967 6874 2063 6f6e 6669  ightweight confi
-00000130: 6773 2066 6f72 2069 6e73 7461 6e74 6961  gs for instantia
-00000140: 7469 6e67 204d 4c20 6578 7065 7269 6d65  ting ML experime
-00000150: 6e74 7327 2c0d 0a20 2020 2020 2061 7574  nts',..      aut
-00000160: 686f 723d 2731 6c69 6e74 272c 0d0a 2020  hor='1lint',..  
-00000170: 2020 2020 6175 7468 6f72 5f65 6d61 696c      author_email
-00000180: 3d27 3130 3536 3137 3136 332b 316c 696e  ='105617163+1lin
-00000190: 7440 7573 6572 732e 6e6f 7265 706c 792e  t@users.noreply.
-000001a0: 6769 7468 7562 2e63 6f6d 272c 0d0a 2020  github.com',..  
-000001b0: 2020 2020 7572 6c3d 6627 6874 7470 733a      url=f'https:
-000001c0: 2f2f 6769 7468 7562 2e63 6f6d 2f31 6c69  //github.com/1li
-000001d0: 6e74 2f7b 7265 706f 5f6e 616d 657d 272c  nt/{repo_name}',
-000001e0: 200d 0a20 2020 2020 2069 6e73 7461 6c6c   ..      install
-000001f0: 5f72 6571 7569 7265 733d 696e 7374 616c  _requires=instal
-00000200: 6c5f 7265 7175 6972 656d 656e 7473 2c0d  l_requirements,.
-00000210: 0a20 2020 2020 2070 6163 6b61 6765 733d  .      packages=
-00000220: 5b72 6570 6f5f 6e61 6d65 5d2c 0d0a 2020  [repo_name],..  
-00000230: 2020 2020 7061 636b 6167 655f 6461 7461      package_data
-00000240: 3d7b 7265 706f 5f6e 616d 653a 205b 7265  ={repo_name: [re
-00000250: 7175 6972 656d 656e 7473 5f66 6e5d 7d2c  quirements_fn]},
-00000260: 0d0a 2020 2020 2020 656e 7472 795f 706f  ..      entry_po
-00000270: 696e 7473 3d7b 0d0a 2020 2020 2020 2020  ints={..        
-00000280: 2020 2020 2763 6f6e 736f 6c65 5f73 6372      'console_scr
-00000290: 6970 7473 273a 205b 0d0a 2020 2020 2020  ipts': [..      
-000002a0: 2020 2020 2020 2020 2020 2020 226c 6974              "lit
-000002b0: 6520 3d20 6c69 7465 6f62 6a3a 6d61 696e  e = liteobj:main
-000002c0: 220d 0a20 2020 2020 2020 2020 2020 205d  "..            ]
-000002d0: 0d0a 2020 2020 2020 7d2c 0d0a 2020 2020  ..      },..    
-000002e0: 2020 7363 7269 7074 733d 5b22 7665 7273    scripts=["vers
-000002f0: 696f 6e2e 7079 225d 0d0a 290d 0a0d 0a    ion.py"]..)....
+00000020: 0d0a 7265 706f 5f6e 616d 6520 3d20 276c  ..repo_name = 'l
+00000030: 6974 656f 626a 270d 0a0d 0a5f 5f76 6572  iteobj'....__ver
+00000040: 7369 6f6e 5f5f 203d 204e 6f6e 650d 0a77  sion__ = None..w
+00000050: 6974 6820 6f70 656e 2866 227b 7265 706f  ith open(f"{repo
+00000060: 5f6e 616d 657d 2f5f 5f69 6e69 745f 5f2e  _name}/__init__.
+00000070: 7079 222c 2022 7222 2920 6173 2066 3a0d  py", "r") as f:.
+00000080: 0a20 2020 2076 6572 7369 6f6e 5f73 7461  .    version_sta
+00000090: 7465 6d65 6e74 203d 2066 2e72 6561 646c  tement = f.readl
+000000a0: 696e 6528 290d 0a0d 0a65 7865 6328 7665  ine()....exec(ve
+000000b0: 7273 696f 6e5f 7374 6174 656d 656e 7429  rsion_statement)
+000000c0: 0d0a 0d0a 7265 7175 6972 656d 656e 7473  ....requirements
+000000d0: 5f66 6e20 3d20 2272 6571 7569 7265 6d65  _fn = "requireme
+000000e0: 6e74 732e 7478 7422 0d0a 696e 7374 616c  nts.txt"..instal
+000000f0: 6c5f 7265 7175 6972 656d 656e 7473 203d  l_requirements =
+00000100: 206f 7065 6e28 6622 7b72 6570 6f5f 6e61   open(f"{repo_na
+00000110: 6d65 7d2f 7b72 6571 7569 7265 6d65 6e74  me}/{requirement
+00000120: 735f 666e 7d22 292e 7265 6164 2829 2e73  s_fn}").read().s
+00000130: 706c 6974 2829 0d0a 0d0a 7365 7475 7028  plit()....setup(
+00000140: 0d0a 2020 2020 2020 6e61 6d65 3d72 6570  ..      name=rep
+00000150: 6f5f 6e61 6d65 2c0d 0a20 2020 2020 2076  o_name,..      v
+00000160: 6572 7369 6f6e 3d5f 5f76 6572 7369 6f6e  ersion=__version
+00000170: 5f5f 2c0d 0a20 2020 2020 2064 6573 6372  __,..      descr
+00000180: 6970 7469 6f6e 3d27 4372 6561 7465 206c  iption='Create l
+00000190: 6967 6874 7765 6967 6874 2063 6f6e 6669  ightweight confi
+000001a0: 6773 2066 6f72 2069 6e73 7461 6e74 6961  gs for instantia
+000001b0: 7469 6e67 204d 4c20 6578 7065 7269 6d65  ting ML experime
+000001c0: 6e74 7327 2c0d 0a20 2020 2020 2061 7574  nts',..      aut
+000001d0: 686f 723d 2731 6c69 6e74 272c 0d0a 2020  hor='1lint',..  
+000001e0: 2020 2020 6175 7468 6f72 5f65 6d61 696c      author_email
+000001f0: 3d27 3130 3536 3137 3136 332b 316c 696e  ='105617163+1lin
+00000200: 7440 7573 6572 732e 6e6f 7265 706c 792e  t@users.noreply.
+00000210: 6769 7468 7562 2e63 6f6d 272c 0d0a 2020  github.com',..  
+00000220: 2020 2020 7572 6c3d 6627 6874 7470 733a      url=f'https:
+00000230: 2f2f 6769 7468 7562 2e63 6f6d 2f31 6c69  //github.com/1li
+00000240: 6e74 2f7b 7265 706f 5f6e 616d 657d 272c  nt/{repo_name}',
+00000250: 200d 0a20 2020 2020 2069 6e73 7461 6c6c   ..      install
+00000260: 5f72 6571 7569 7265 733d 696e 7374 616c  _requires=instal
+00000270: 6c5f 7265 7175 6972 656d 656e 7473 2c0d  l_requirements,.
+00000280: 0a20 2020 2020 2070 6163 6b61 6765 733d  .      packages=
+00000290: 5b72 6570 6f5f 6e61 6d65 5d2c 0d0a 2020  [repo_name],..  
+000002a0: 2020 2020 7061 636b 6167 655f 6461 7461      package_data
+000002b0: 3d7b 7265 706f 5f6e 616d 653a 205b 7265  ={repo_name: [re
+000002c0: 7175 6972 656d 656e 7473 5f66 6e5d 7d2c  quirements_fn]},
+000002d0: 0d0a 2020 2020 2020 656e 7472 795f 706f  ..      entry_po
+000002e0: 696e 7473 3d7b 0d0a 2020 2020 2020 2020  ints={..        
+000002f0: 2020 2020 2763 6f6e 736f 6c65 5f73 6372      'console_scr
+00000300: 6970 7473 273a 205b 0d0a 2020 2020 2020  ipts': [..      
+00000310: 2020 2020 2020 2020 2020 2020 226c 6974              "lit
+00000320: 6520 3d20 6c69 7465 6f62 6a3a 6d61 696e  e = liteobj:main
+00000330: 220d 0a20 2020 2020 2020 2020 2020 205d  "..            ]
+00000340: 0d0a 2020 2020 2020 7d2c 0d0a 290d 0a0d  ..      },..)...
+00000350: 0a                                       .
```

