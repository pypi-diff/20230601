# Comparing `tmp/liteobj-0.0.5.tar.gz` & `tmp/liteobj-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liteobj-0.0.5.tar", last modified: Thu Jun  1 19:00:33 2023, max compression
+gzip compressed data, was "liteobj-0.0.6.tar", last modified: Thu Jun  1 21:12:54 2023, max compression
```

## Comparing `liteobj-0.0.5.tar` & `liteobj-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-01 19:00:33.342050 liteobj-0.0.5/
--rwxr-xr-x   0 user      (1000) user      (1000)    11538 2023-05-25 22:18:19.000000 liteobj-0.0.5/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)      255 2023-06-01 19:00:33.342050 liteobj-0.0.5/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     1221 2023-06-01 19:00:09.000000 liteobj-0.0.5/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-01 19:00:33.342050 liteobj-0.0.5/liteobj/
--rw-r--r--   0 user      (1000) user      (1000)       20 2023-05-25 22:02:13.000000 liteobj-0.0.5/liteobj/__init__.py
--rwxr-xr-x   0 user      (1000) user      (1000)     3212 2023-06-01 18:46:53.000000 liteobj-0.0.5/liteobj/lite.py
--rw-r--r--   0 user      (1000) user      (1000)       28 2023-05-25 21:59:58.000000 liteobj-0.0.5/liteobj/requirements.txt
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-01 19:00:33.342050 liteobj-0.0.5/liteobj.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)      255 2023-06-01 19:00:33.000000 liteobj-0.0.5/liteobj.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      275 2023-06-01 19:00:33.000000 liteobj-0.0.5/liteobj.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-06-01 19:00:33.000000 liteobj-0.0.5/liteobj.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       38 2023-06-01 19:00:33.000000 liteobj-0.0.5/liteobj.egg-info/entry_points.txt
--rw-r--r--   0 user      (1000) user      (1000)       29 2023-06-01 19:00:33.000000 liteobj-0.0.5/liteobj.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)        8 2023-06-01 19:00:33.000000 liteobj-0.0.5/liteobj.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)       38 2023-06-01 19:00:33.342050 liteobj-0.0.5/setup.cfg
--rwxr-xr-x   0 user      (1000) user      (1000)      706 2023-06-01 18:38:23.000000 liteobj-0.0.5/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-01 21:12:54.372393 liteobj-0.0.6/
+-rwxr-xr-x   0 user      (1000) user      (1000)    11538 2023-05-25 22:18:19.000000 liteobj-0.0.6/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)      255 2023-06-01 21:12:54.372393 liteobj-0.0.6/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     1221 2023-06-01 19:00:09.000000 liteobj-0.0.6/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-01 21:12:54.372393 liteobj-0.0.6/liteobj/
+-rw-r--r--   0 user      (1000) user      (1000)       97 2023-06-01 21:10:19.000000 liteobj-0.0.6/liteobj/__init__.py
+-rwxr-xr-x   0 user      (1000) user      (1000)     3897 2023-06-01 21:04:12.000000 liteobj-0.0.6/liteobj/lite.py
+-rw-r--r--   0 user      (1000) user      (1000)       28 2023-05-25 21:59:58.000000 liteobj-0.0.6/liteobj/requirements.txt
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-06-01 21:12:54.372393 liteobj-0.0.6/liteobj.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)      255 2023-06-01 21:12:54.000000 liteobj-0.0.6/liteobj.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      286 2023-06-01 21:12:54.000000 liteobj-0.0.6/liteobj.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-06-01 21:12:54.000000 liteobj-0.0.6/liteobj.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       38 2023-06-01 21:12:54.000000 liteobj-0.0.6/liteobj.egg-info/entry_points.txt
+-rw-r--r--   0 user      (1000) user      (1000)       29 2023-06-01 21:12:54.000000 liteobj-0.0.6/liteobj.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)        8 2023-06-01 21:12:54.000000 liteobj-0.0.6/liteobj.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)       38 2023-06-01 21:12:54.372393 liteobj-0.0.6/setup.cfg
+-rwxr-xr-x   0 user      (1000) user      (1000)      767 2023-06-01 21:12:51.000000 liteobj-0.0.6/setup.py
+-rw-r--r--   0 user      (1000) user      (1000)       21 2023-06-01 21:09:46.000000 liteobj-0.0.6/version.py
```

### Comparing `liteobj-0.0.5/LICENSE` & `liteobj-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `liteobj-0.0.5/README.md` & `liteobj-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `liteobj-0.0.5/setup.py` & `liteobj-0.0.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 00000000: 0d0a 6672 6f6d 2073 6574 7570 746f 6f6c  ..from setuptool
 00000010: 7320 696d 706f 7274 2073 6574 7570 0d0a  s import setup..
-00000020: 0d0a 7265 706f 5f6e 616d 6520 3d20 276c  ..repo_name = 'l
-00000030: 6974 656f 626a 270d 0a0d 0a72 6571 7569  iteobj'....requi
-00000040: 7265 6d65 6e74 735f 666e 203d 2022 7265  rements_fn = "re
-00000050: 7175 6972 656d 656e 7473 2e74 7874 220d  quirements.txt".
-00000060: 0a69 6e73 7461 6c6c 5f72 6571 7569 7265  .install_require
-00000070: 6d65 6e74 7320 3d20 6f70 656e 2866 227b  ments = open(f"{
-00000080: 7265 706f 5f6e 616d 657d 2f7b 7265 7175  repo_name}/{requ
-00000090: 6972 656d 656e 7473 5f66 6e7d 2229 2e72  irements_fn}").r
-000000a0: 6561 6428 292e 7370 6c69 7428 290d 0a0d  ead().split()...
-000000b0: 0a73 6574 7570 286e 616d 653d 7265 706f  .setup(name=repo
-000000c0: 5f6e 616d 652c 0d0a 2020 2020 2020 7665  _name,..      ve
-000000d0: 7273 696f 6e3d 2730 2e30 2e35 272c 0d0a  rsion='0.0.5',..
-000000e0: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
-000000f0: 6e3d 2743 7265 6174 6520 6c69 6768 7477  n='Create lightw
-00000100: 6569 6768 7420 636f 6e66 6967 7320 666f  eight configs fo
-00000110: 7220 696e 7374 616e 7469 6174 696e 6720  r instantiating 
-00000120: 4d4c 2065 7870 6572 696d 656e 7473 272c  ML experiments',
-00000130: 0d0a 2020 2020 2020 6175 7468 6f72 3d27  ..      author='
-00000140: 316c 696e 7427 2c0d 0a20 2020 2020 2061  1lint',..      a
-00000150: 7574 686f 725f 656d 6169 6c3d 2731 3035  uthor_email='105
-00000160: 3631 3731 3633 2b31 6c69 6e74 4075 7365  617163+1lint@use
-00000170: 7273 2e6e 6f72 6570 6c79 2e67 6974 6875  rs.noreply.githu
-00000180: 622e 636f 6d27 2c0d 0a20 2020 2020 2075  b.com',..      u
-00000190: 726c 3d66 2768 7474 7073 3a2f 2f67 6974  rl=f'https://git
-000001a0: 6875 622e 636f 6d2f 316c 696e 742f 7b72  hub.com/1lint/{r
-000001b0: 6570 6f5f 6e61 6d65 7d27 2c20 0d0a 2020  epo_name}', ..  
-000001c0: 2020 2020 696e 7374 616c 6c5f 7265 7175      install_requ
-000001d0: 6972 6573 3d69 6e73 7461 6c6c 5f72 6571  ires=install_req
-000001e0: 7569 7265 6d65 6e74 732c 0d0a 2020 2020  uirements,..    
-000001f0: 2020 7061 636b 6167 6573 3d5b 7265 706f    packages=[repo
-00000200: 5f6e 616d 655d 2c0d 0a20 2020 2020 2070  _name],..      p
-00000210: 6163 6b61 6765 5f64 6174 613d 7b72 6570  ackage_data={rep
-00000220: 6f5f 6e61 6d65 3a20 5b72 6571 7569 7265  o_name: [require
-00000230: 6d65 6e74 735f 666e 5d7d 2c0d 0a20 2020  ments_fn]},..   
-00000240: 2020 2065 6e74 7279 5f70 6f69 6e74 733d     entry_points=
-00000250: 7b0d 0a20 2020 2020 2020 2020 2020 2027  {..            '
-00000260: 636f 6e73 6f6c 655f 7363 7269 7074 7327  console_scripts'
-00000270: 3a20 5b0d 0a20 2020 2020 2020 2020 2020  : [..           
-00000280: 2020 2020 2020 2022 6c69 7465 203d 206c         "lite = l
-00000290: 6974 656f 626a 3a6d 6169 6e22 0d0a 2020  iteobj:main"..  
-000002a0: 2020 2020 2020 2020 2020 5d0d 0a20 2020            ]..   
-000002b0: 2020 207d 2c0d 0a20 2020 2020 2029 0d0a     },..      )..
-000002c0: 0d0a                                     ..
+00000020: 6672 6f6d 2076 6572 7369 6f6e 2069 6d70  from version imp
+00000030: 6f72 7420 5f5f 7665 7273 696f 6e5f 5f0d  ort __version__.
+00000040: 0a0d 0a72 6570 6f5f 6e61 6d65 203d 2027  ...repo_name = '
+00000050: 6c69 7465 6f62 6a27 0d0a 0d0a 7265 7175  liteobj'....requ
+00000060: 6972 656d 656e 7473 5f66 6e20 3d20 2272  irements_fn = "r
+00000070: 6571 7569 7265 6d65 6e74 732e 7478 7422  equirements.txt"
+00000080: 0d0a 696e 7374 616c 6c5f 7265 7175 6972  ..install_requir
+00000090: 656d 656e 7473 203d 206f 7065 6e28 6622  ements = open(f"
+000000a0: 7b72 6570 6f5f 6e61 6d65 7d2f 7b72 6571  {repo_name}/{req
+000000b0: 7569 7265 6d65 6e74 735f 666e 7d22 292e  uirements_fn}").
+000000c0: 7265 6164 2829 2e73 706c 6974 2829 0d0a  read().split()..
+000000d0: 0d0a 7365 7475 7028 6e61 6d65 3d72 6570  ..setup(name=rep
+000000e0: 6f5f 6e61 6d65 2c0d 0a20 2020 2020 2076  o_name,..      v
+000000f0: 6572 7369 6f6e 3d5f 5f76 6572 7369 6f6e  ersion=__version
+00000100: 5f5f 2c0d 0a20 2020 2020 2064 6573 6372  __,..      descr
+00000110: 6970 7469 6f6e 3d27 4372 6561 7465 206c  iption='Create l
+00000120: 6967 6874 7765 6967 6874 2063 6f6e 6669  ightweight confi
+00000130: 6773 2066 6f72 2069 6e73 7461 6e74 6961  gs for instantia
+00000140: 7469 6e67 204d 4c20 6578 7065 7269 6d65  ting ML experime
+00000150: 6e74 7327 2c0d 0a20 2020 2020 2061 7574  nts',..      aut
+00000160: 686f 723d 2731 6c69 6e74 272c 0d0a 2020  hor='1lint',..  
+00000170: 2020 2020 6175 7468 6f72 5f65 6d61 696c      author_email
+00000180: 3d27 3130 3536 3137 3136 332b 316c 696e  ='105617163+1lin
+00000190: 7440 7573 6572 732e 6e6f 7265 706c 792e  t@users.noreply.
+000001a0: 6769 7468 7562 2e63 6f6d 272c 0d0a 2020  github.com',..  
+000001b0: 2020 2020 7572 6c3d 6627 6874 7470 733a      url=f'https:
+000001c0: 2f2f 6769 7468 7562 2e63 6f6d 2f31 6c69  //github.com/1li
+000001d0: 6e74 2f7b 7265 706f 5f6e 616d 657d 272c  nt/{repo_name}',
+000001e0: 200d 0a20 2020 2020 2069 6e73 7461 6c6c   ..      install
+000001f0: 5f72 6571 7569 7265 733d 696e 7374 616c  _requires=instal
+00000200: 6c5f 7265 7175 6972 656d 656e 7473 2c0d  l_requirements,.
+00000210: 0a20 2020 2020 2070 6163 6b61 6765 733d  .      packages=
+00000220: 5b72 6570 6f5f 6e61 6d65 5d2c 0d0a 2020  [repo_name],..  
+00000230: 2020 2020 7061 636b 6167 655f 6461 7461      package_data
+00000240: 3d7b 7265 706f 5f6e 616d 653a 205b 7265  ={repo_name: [re
+00000250: 7175 6972 656d 656e 7473 5f66 6e5d 7d2c  quirements_fn]},
+00000260: 0d0a 2020 2020 2020 656e 7472 795f 706f  ..      entry_po
+00000270: 696e 7473 3d7b 0d0a 2020 2020 2020 2020  ints={..        
+00000280: 2020 2020 2763 6f6e 736f 6c65 5f73 6372      'console_scr
+00000290: 6970 7473 273a 205b 0d0a 2020 2020 2020  ipts': [..      
+000002a0: 2020 2020 2020 2020 2020 2020 226c 6974              "lit
+000002b0: 6520 3d20 6c69 7465 6f62 6a3a 6d61 696e  e = liteobj:main
+000002c0: 220d 0a20 2020 2020 2020 2020 2020 205d  "..            ]
+000002d0: 0d0a 2020 2020 2020 7d2c 0d0a 2020 2020  ..      },..    
+000002e0: 2020 7363 7269 7074 733d 5b22 7665 7273    scripts=["vers
+000002f0: 696f 6e2e 7079 225d 0d0a 290d 0a0d 0a    ion.py"]..)....
```

