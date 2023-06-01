# Comparing `tmp/rasm_arch-1.2.1.tar.gz` & `tmp/rasm_arch-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rasm_arch-1.2.1.tar", last modified: Thu Jun  1 09:50:40 2023, max compression
+gzip compressed data, was "rasm_arch-1.2.5.tar", last modified: Thu Jun  1 11:22:05 2023, max compression
```

## Comparing `rasm_arch-1.2.1.tar` & `rasm_arch-1.2.5.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2023-06-01 09:50:40.822704 rasm_arch-1.2.1/
--rw-r--r--   0 alicia    (1000) alicia    (1000)     1098 2022-10-16 09:52:15.000000 rasm_arch-1.2.1/LICENSE
--rw-r--r--   0 alicia    (1000) alicia    (1000)      171 2023-06-01 08:59:29.000000 rasm_arch-1.2.1/MANIFEST.in
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     7092 2023-06-01 09:50:40.822704 rasm_arch-1.2.1/PKG-INFO
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     6021 2023-06-01 09:47:57.000000 rasm_arch-1.2.1/README.md
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2023-06-01 09:50:40.814704 rasm_arch-1.2.1/bin/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)    10373 2023-06-01 09:48:38.000000 rasm_arch-1.2.1/bin/rasm-arch
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2023-06-01 09:50:40.814704 rasm_arch-1.2.1/rasm_arch/
--rw-r--r--   0 alicia    (1000) alicia    (1000)       66 2023-06-01 09:48:50.000000 rasm_arch-1.2.1/rasm_arch/__init__.py
--rw-rw-r--   0 alicia    (1000) alicia    (1000)    48343 2023-06-01 09:40:44.000000 rasm_arch-1.2.1/rasm_arch/rasm_arch.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2023-06-01 09:50:40.818704 rasm_arch-1.2.1/rasm_arch/resources/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)  1972594 2023-05-31 17:13:54.000000 rasm_arch-1.2.1/rasm_arch/resources/mushaf_simple.json
--rw-rw-r--   0 alicia    (1000) alicia    (1000)  2288703 2023-05-31 17:14:35.000000 rasm_arch-1.2.1/rasm_arch/resources/mushaf_uthmani.json
--rw-r--r--   0 alicia    (1000) alicia    (1000)     3013 2023-06-01 09:00:08.000000 rasm_arch-1.2.1/rasm_arch/util.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2023-06-01 09:50:40.818704 rasm_arch-1.2.1/rasm_arch.egg-info/
--rw-rw-r--   0 alicia    (1000) alicia    (1000)     7092 2023-06-01 09:50:40.000000 rasm_arch-1.2.1/rasm_arch.egg-info/PKG-INFO
--rw-rw-r--   0 alicia    (1000) alicia    (1000)      350 2023-06-01 09:50:40.000000 rasm_arch-1.2.1/rasm_arch.egg-info/SOURCES.txt
--rw-rw-r--   0 alicia    (1000) alicia    (1000)        1 2023-06-01 09:50:40.000000 rasm_arch-1.2.1/rasm_arch.egg-info/dependency_links.txt
--rw-rw-r--   0 alicia    (1000) alicia    (1000)       10 2023-06-01 09:50:40.000000 rasm_arch-1.2.1/rasm_arch.egg-info/top_level.txt
--rw-rw-r--   0 alicia    (1000) alicia    (1000)       38 2023-06-01 09:50:40.822704 rasm_arch-1.2.1/setup.cfg
--rw-r--r--   0 alicia    (1000) alicia    (1000)     2808 2023-06-01 09:48:47.000000 rasm_arch-1.2.1/setup.py
-drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2023-06-01 09:50:40.822704 rasm_arch-1.2.1/tests/
--rw-r--r--   0 alicia    (1000) alicia    (1000)    13532 2023-06-01 07:45:44.000000 rasm_arch-1.2.1/tests/test_rasm_arch.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2023-06-01 11:22:05.618489 rasm_arch-1.2.5/
+-rw-r--r--   0 alicia    (1000) alicia    (1000)     1098 2022-10-16 09:52:15.000000 rasm_arch-1.2.5/LICENSE
+-rw-r--r--   0 alicia    (1000) alicia    (1000)      156 2023-06-01 11:19:04.000000 rasm_arch-1.2.5/MANIFEST.in
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     7092 2023-06-01 11:22:05.614489 rasm_arch-1.2.5/PKG-INFO
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     6021 2023-06-01 11:20:20.000000 rasm_arch-1.2.5/README.md
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2023-06-01 11:22:05.610489 rasm_arch-1.2.5/bin/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)    10373 2023-06-01 11:20:33.000000 rasm_arch-1.2.5/bin/rasm-arch
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2023-06-01 11:22:05.610489 rasm_arch-1.2.5/rasm_arch/
+-rw-r--r--   0 alicia    (1000) alicia    (1000)       66 2023-06-01 11:20:37.000000 rasm_arch-1.2.5/rasm_arch/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)    48348 2023-06-01 11:17:28.000000 rasm_arch-1.2.5/rasm_arch/rasm_arch.py
+-rw-r--r--   0 alicia    (1000) alicia    (1000)     3013 2023-06-01 11:17:20.000000 rasm_arch-1.2.5/rasm_arch/util.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2023-06-01 11:22:05.610489 rasm_arch-1.2.5/rasm_arch.egg-info/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)     7092 2023-06-01 11:22:05.000000 rasm_arch-1.2.5/rasm_arch.egg-info/PKG-INFO
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)      367 2023-06-01 11:22:05.000000 rasm_arch-1.2.5/rasm_arch.egg-info/SOURCES.txt
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        1 2023-06-01 11:22:05.000000 rasm_arch-1.2.5/rasm_arch.egg-info/dependency_links.txt
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)       25 2023-06-01 11:22:05.000000 rasm_arch-1.2.5/rasm_arch.egg-info/top_level.txt
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2023-06-01 11:22:05.614489 rasm_arch-1.2.5/rasm_arch_data/
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)        0 2023-05-22 15:41:58.000000 rasm_arch-1.2.5/rasm_arch_data/__init__.py
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)  1972594 2023-05-31 17:13:54.000000 rasm_arch-1.2.5/rasm_arch_data/mushaf_simple.json
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)  2288703 2023-05-31 17:14:35.000000 rasm_arch-1.2.5/rasm_arch_data/mushaf_uthmani.json
+-rw-rw-r--   0 alicia    (1000) alicia    (1000)       38 2023-06-01 11:22:05.618489 rasm_arch-1.2.5/setup.cfg
+-rw-r--r--   0 alicia    (1000) alicia    (1000)     2687 2023-06-01 11:20:41.000000 rasm_arch-1.2.5/setup.py
+drwxrwxr-x   0 alicia    (1000) alicia    (1000)        0 2023-06-01 11:22:05.614489 rasm_arch-1.2.5/tests/
+-rw-r--r--   0 alicia    (1000) alicia    (1000)    13532 2023-06-01 07:45:44.000000 rasm_arch-1.2.5/tests/test_rasm_arch.py
```

### Comparing `rasm_arch-1.2.1/LICENSE` & `rasm_arch-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rasm_arch-1.2.1/PKG-INFO` & `rasm_arch-1.2.5/rasm_arch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: rasm_arch
-Version: 1.2.1
+Name: rasm-arch
+Version: 1.2.5
 Summary: text utility for converting Arabic-scripted text to a completely dediacritised skeleton
 Home-page: https://github.com/kabikaj/rasm_arch
 Download-URL: https://github.com/kabikaj/rasm_arch
 Author: Alicia González Martínez and Thomas Milo
 Author-email: aliciagm85+kabikaj@gmail.com
 License: MIT
 Keywords: arabic,persian,urdu,quran,manuscript,rasm,unicode,NLP,digital humanities
@@ -154,15 +154,15 @@
     ]
   }
 ]
 ```
 
 ## Version
 
-1.2.1
+1.2.5
 
 ## License for the code
  
 Rasm_arch is a text processing utility for converting Arabic-scripted text to a completely dediacritised skeleton.
 
 The code for this project is licensed under the MIT License.
```

### Comparing `rasm_arch-1.2.1/README.md` & `rasm_arch-1.2.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
     ]
   }
 ]
 ```
 
 ## Version
 
-1.2.1
+1.2.5
 
 ## License for the code
  
 Rasm_arch is a text processing utility for converting Arabic-scripted text to a completely dediacritised skeleton.
 
 The code for this project is licensed under the MIT License.
```

### Comparing `rasm_arch-1.2.1/bin/rasm-arch` & `rasm_arch-1.2.5/bin/rasm-arch`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
     parser.add_argument('--paleo', '-p', action='store_true', help='include paleo-orthographic representation of text')
     parser.add_argument('--blocks', '-b', action='store_true', help='return results in letterblocks, instead of words')
     parser.add_argument('--only_rasm', action='store_true', help='do not print start of rub el hizb (۞ U+06de) nor place of sajda (۩ U+06e9) [only for --quran]')
     parser.add_argument('--unstable_alif', '-a', action='store_true', help='remove fatha+alif in non final positions as it is unstable. It works with text option only.')
     parser.add_argument('--uniq', '-u', action='store_true', help='output each unique archigraphemic letterblock, no. of occurrences and list of them')
     parser.add_argument('--sep', default='\t', help='field separator for text output [DEFAULT \\t]')
     parser.add_argument('--json', action='store_true', help='print output in json instead of plain text')
-    parser.add_argument('--version', action='version', version='%(prog)s 1.2.1', help='prints the program version number and exits successfully') #FIXME
+    parser.add_argument('--version', action='version', version='%(prog)s 1.2.5', help='prints the program version number and exits successfully') #FIXME
     args = parser.parse_args()
 
     try:
     
         if args.quran:
             result = rasm(args.quran, paleo=args.paleo,
                                       blocks=args.blocks,
```

### Comparing `rasm_arch-1.2.1/rasm_arch/rasm_arch.py` & `rasm_arch-1.2.5/rasm_arch/rasm_arch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1039,20 +1039,23 @@
         PrivateFileError: decotype file is private.
 
     """ 
     if source == 'tanzil-uthmani':
         source_file = SOURCE.TANZIL_UTHMANI
     elif source == 'decotype':
         source_file = SOURCE.DECOTYPE
-        if not files('rasm_arch.resources').joinpath(source_file).exists():
-            raise PrivateFileError
     else:
         source_file = SOURCE.TANZIL_SIMPLE
 
-    with files('rasm_arch.resources').joinpath(source_file).open() as fp:
+    source_path = files('rasm_arch_data').joinpath(source_file)
+
+    if source == 'decotype' and not source_path.exists():
+        raise PrivateFileError
+
+    with source_path.open() as fp:
         quran = json.load(fp)
     
         i, j, k, m = [(ind-1 if ind else ind) for ind in index[0]]
         n, p, q, r = [(ind-1 if ind else ind) for ind in index[1]]
 
         # we put a maximum upper limit in the end index, copying the start index when the end is absent
         if (n, p, q, r) == (None, None, None, None):
```

### Comparing `rasm_arch-1.2.1/rasm_arch/resources/mushaf_simple.json` & `rasm_arch-1.2.5/rasm_arch_data/mushaf_simple.json`

 * *Files identical despite different names*

### Comparing `rasm_arch-1.2.1/rasm_arch/resources/mushaf_uthmani.json` & `rasm_arch-1.2.5/rasm_arch_data/mushaf_uthmani.json`

 * *Files identical despite different names*

### Comparing `rasm_arch-1.2.1/rasm_arch/util.py` & `rasm_arch-1.2.5/rasm_arch/util.py`

 * *Files identical despite different names*

### Comparing `rasm_arch-1.2.1/rasm_arch.egg-info/PKG-INFO` & `rasm_arch-1.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: rasm-arch
-Version: 1.2.1
+Name: rasm_arch
+Version: 1.2.5
 Summary: text utility for converting Arabic-scripted text to a completely dediacritised skeleton
 Home-page: https://github.com/kabikaj/rasm_arch
 Download-URL: https://github.com/kabikaj/rasm_arch
 Author: Alicia González Martínez and Thomas Milo
 Author-email: aliciagm85+kabikaj@gmail.com
 License: MIT
 Keywords: arabic,persian,urdu,quran,manuscript,rasm,unicode,NLP,digital humanities
@@ -154,15 +154,15 @@
     ]
   }
 ]
 ```
 
 ## Version
 
-1.2.1
+1.2.5
 
 ## License for the code
  
 Rasm_arch is a text processing utility for converting Arabic-scripted text to a completely dediacritised skeleton.
 
 The code for this project is licensed under the MIT License.
```

### Comparing `rasm_arch-1.2.1/setup.py` & `rasm_arch-1.2.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,23 +30,17 @@
 
 def readme():
     with open('README.md') as fp:
         return fp.read()
 
 setup(
     name = "rasm_arch",
-    packages = ["rasm_arch"],
-    package_data = {
-        os.path.join('rasm_arch', 'resources') : [
-            'mushaf_simple.json',
-            'mushaf_uthmani.json',
-            'mushaf_dt.json',
-        ]
-    },
-    version = "1.2.1",
+    packages = ["rasm_arch", "rasm_arch_data"],
+    package_data={"rasm_arch_data": ["*.json"]},
+    version = "1.2.5",
     description = "text utility for converting Arabic-scripted text to a completely dediacritised skeleton",
     long_description = readme(),
     long_description_content_type="text/markdown",
     author = "Alicia González Martínez and Thomas Milo",
     author_email = "aliciagm85+kabikaj@gmail.com",
     url = "https://github.com/kabikaj/rasm_arch",
     download_url = "https://github.com/kabikaj/rasm_arch",
```

### Comparing `rasm_arch-1.2.1/tests/test_rasm_arch.py` & `rasm_arch-1.2.5/tests/test_rasm_arch.py`

 * *Files identical despite different names*

