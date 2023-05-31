# Comparing `tmp/catencfamily-0.0.2.tar.gz` & `tmp/catencfamily-0.0.3.tar.gz`

## Comparing `catencfamily-0.0.2.tar` & `catencfamily-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 catencfamily-0.0.2/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catencfamily-0.0.2/src/catfamilyenc/__init__.py
--rw-r--r--   0        0        0    87907 2020-02-02 00:00:00.000000 catencfamily-0.0.2/src/catfamilyenc/catencfamily.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 catencfamily-0.0.2/LICENSE
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 catencfamily-0.0.2/README.md
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 catencfamily-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 catencfamily-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 catencfamily-0.0.3/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catencfamily-0.0.3/src/catfamilyenc/__init__.py
+-rw-r--r--   0        0        0    87907 2020-02-02 00:00:00.000000 catencfamily-0.0.3/src/catfamilyenc/catencfamily.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 catencfamily-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 catencfamily-0.0.3/README.md
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 catencfamily-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 catencfamily-0.0.3/PKG-INFO
```

### Comparing `catencfamily-0.0.2/requirements.txt` & `catencfamily-0.0.3/requirements.txt`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #    pip-compile
 #
 angel-cd==1.0.3
     # via cdlib
 bimlpa==0.1.2
     # via cdlib
 cdlib==0.2.6
-    # via catfamilyenc (pyproject.toml)
+    # via catencfamily (pyproject.toml)
 certifi==2023.5.7
     # via requests
 charset-normalizer==3.1.0
     # via requests
 chinese-whispers==0.8.1
     # via cdlib
 colorama==0.4.6
@@ -50,37 +50,37 @@
 levenshtein==0.21.0
     # via python-levenshtein
 markov-clustering==0.0.6.dev0
     # via cdlib
 matplotlib==3.7.1
     # via
     #   bimlpa
-    #   catfamilyenc (pyproject.toml)
+    #   catencfamily (pyproject.toml)
     #   cdlib
     #   nf1
     #   pyclustering
     #   seaborn
 networkx==2.8.8
     # via
     #   angel-cd
     #   bimlpa
-    #   catfamilyenc (pyproject.toml)
+    #   catencfamily (pyproject.toml)
     #   cdlib
     #   chinese-whispers
     #   demon
     #   dynetx
     #   eva-lcd
     #   python-louvain
     #   thresholdclustering
 nf1==0.0.4
     # via cdlib
 numpy==1.24.3
     # via
     #   angel-cd
-    #   catfamilyenc (pyproject.toml)
+    #   catencfamily (pyproject.toml)
     #   cdlib
     #   contourpy
     #   dynetx
     #   eva-lcd
     #   markov-clustering
     #   matplotlib
     #   nf1
@@ -93,20 +93,20 @@
     #   thresholdclustering
 packaging==23.1
     # via
     #   matplotlib
     #   pooch
 pandas==2.0.2
     # via
-    #   catfamilyenc (pyproject.toml)
+    #   catencfamily (pyproject.toml)
     #   cdlib
     #   nf1
     #   seaborn
 pathlib==1.0.1
-    # via catfamilyenc (pyproject.toml)
+    # via catencfamily (pyproject.toml)
 pillow==9.5.0
     # via
     #   matplotlib
     #   pyclustering
 platformdirs==3.5.1
     # via pooch
 pooch==1.7.0
@@ -134,15 +134,15 @@
 rapidfuzz==3.0.0
     # via levenshtein
 requests==2.31.0
     # via pooch
 scikit-learn==1.2.2
     # via
     #   bimlpa
-    #   catfamilyenc (pyproject.toml)
+    #   catencfamily (pyproject.toml)
     #   cdlib
     #   markov-clustering
 scipy==1.10.1
     # via
     #   cdlib
     #   markov-clustering
     #   nf1
```

### Comparing `catencfamily-0.0.2/src/catfamilyenc/catencfamily.py` & `catencfamily-0.0.3/src/catfamilyenc/catencfamily.py`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.2/LICENSE` & `catencfamily-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.2/README.md` & `catencfamily-0.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -11,13 +11,13 @@
 python >= 3.7
 pandas
 numpy
 networkx
 cdlib
 scikit-learn
 matplotlib
-pathlib
+pathlib</code></pre>
 
 
 ## License
 
 _MIT License. Any contribution is welcome!
```

### Comparing `catencfamily-0.0.2/pyproject.toml` & `catencfamily-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "catencfamily"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Ashok Kumar Harnal", email="ashokharnal@gmail.com" },
 ]
 description = "A class to generate a family of categorical encoders using network analysis"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `catencfamily-0.0.2/PKG-INFO` & `catencfamily-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catencfamily
-Version: 0.0.2
+Version: 0.0.3
 Summary: A class to generate a family of categorical encoders using network analysis
 Project-URL: Homepage, https://github.com/harnalashok/CatEncodersFamily
 Author-email: Ashok Kumar Harnal <ashokharnal@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -31,13 +31,13 @@
 python >= 3.7
 pandas
 numpy
 networkx
 cdlib
 scikit-learn
 matplotlib
-pathlib
+pathlib</code></pre>
 
 
 ## License
 
 _MIT License. Any contribution is welcome!
```

