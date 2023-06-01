# Comparing `tmp/cryptopp-1.0.2.tar.gz` & `tmp/cryptopp-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptopp-1.0.2.tar", last modified: Thu May 18 00:50:43 2023, max compression
+gzip compressed data, was "cryptopp-1.0.3.tar", last modified: Thu Jun  1 04:59:52 2023, max compression
```

## Comparing `cryptopp-1.0.2.tar` & `cryptopp-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 bubonic   (1000) bubonic   (1000)        0 2023-05-18 00:50:43.311931 cryptopp-1.0.2/
--rw-rw-r--   0 bubonic   (1000) bubonic   (1000)    35149 2023-05-18 00:13:49.000000 cryptopp-1.0.2/LICENSE
--rw-rw-r--   0 bubonic   (1000) bubonic   (1000)       46 2023-05-18 00:13:57.000000 cryptopp-1.0.2/MANIFEST.in
--rw-rw-r--   0 bubonic   (1000) bubonic   (1000)     3788 2023-05-18 00:50:43.311931 cryptopp-1.0.2/PKG-INFO
--rw-rw-r--   0 bubonic   (1000) bubonic   (1000)     3386 2023-05-18 00:50:34.000000 cryptopp-1.0.2/README.rst
-drwxrwxr-x   0 bubonic   (1000) bubonic   (1000)        0 2023-05-18 00:50:43.311931 cryptopp-1.0.2/cryptopp/
--rw-rw-r--   0 bubonic   (1000) bubonic   (1000)        0 2023-05-18 00:13:57.000000 cryptopp-1.0.2/cryptopp/__init__.py
--rw-rw-r--   0 bubonic   (1000) bubonic   (1000)      247 2023-05-18 00:13:57.000000 cryptopp-1.0.2/cryptopp/config.ini
--rw-rw-r--   0 bubonic   (1000) bubonic   (1000)    18857 2023-05-18 00:39:32.000000 cryptopp-1.0.2/cryptopp/cryptopp.py
-drwxrwxr-x   0 bubonic   (1000) bubonic   (1000)        0 2023-05-18 00:50:43.311931 cryptopp-1.0.2/cryptopp.egg-info/
--rw-rw-r--   0 bubonic   (1000) bubonic   (1000)     3788 2023-05-18 00:50:43.000000 cryptopp-1.0.2/cryptopp.egg-info/PKG-INFO
--rw-rw-r--   0 bubonic   (1000) bubonic   (1000)      295 2023-05-18 00:50:43.000000 cryptopp-1.0.2/cryptopp.egg-info/SOURCES.txt
--rw-rw-r--   0 bubonic   (1000) bubonic   (1000)        1 2023-05-18 00:50:43.000000 cryptopp-1.0.2/cryptopp.egg-info/dependency_links.txt
--rw-rw-r--   0 bubonic   (1000) bubonic   (1000)       52 2023-05-18 00:50:43.000000 cryptopp-1.0.2/cryptopp.egg-info/entry_points.txt
--rw-rw-r--   0 bubonic   (1000) bubonic   (1000)       24 2023-05-18 00:50:43.000000 cryptopp-1.0.2/cryptopp.egg-info/requires.txt
--rw-rw-r--   0 bubonic   (1000) bubonic   (1000)        9 2023-05-18 00:50:43.000000 cryptopp-1.0.2/cryptopp.egg-info/top_level.txt
--rw-rw-r--   0 bubonic   (1000) bubonic   (1000)       38 2023-05-18 00:50:43.311931 cryptopp-1.0.2/setup.cfg
--rw-rw-r--   0 bubonic   (1000) bubonic   (1000)      831 2023-05-18 00:42:28.000000 cryptopp-1.0.2/setup.py
+drwxrwxr-x   0 bubonic   (1000) bubonic   (1000)        0 2023-06-01 04:59:52.101266 cryptopp-1.0.3/
+-rw-rw-r--   0 bubonic   (1000) bubonic   (1000)    35149 2023-05-18 00:13:49.000000 cryptopp-1.0.3/LICENSE
+-rw-rw-r--   0 bubonic   (1000) bubonic   (1000)       46 2023-05-18 00:13:57.000000 cryptopp-1.0.3/MANIFEST.in
+-rw-rw-r--   0 bubonic   (1000) bubonic   (1000)     3788 2023-06-01 04:59:52.101266 cryptopp-1.0.3/PKG-INFO
+-rw-rw-r--   0 bubonic   (1000) bubonic   (1000)     3386 2023-05-18 00:50:34.000000 cryptopp-1.0.3/README.rst
+drwxrwxr-x   0 bubonic   (1000) bubonic   (1000)        0 2023-06-01 04:59:52.101266 cryptopp-1.0.3/cryptopp/
+-rw-rw-r--   0 bubonic   (1000) bubonic   (1000)        0 2023-05-18 00:13:57.000000 cryptopp-1.0.3/cryptopp/__init__.py
+-rw-rw-r--   0 bubonic   (1000) bubonic   (1000)      247 2023-05-18 00:13:57.000000 cryptopp-1.0.3/cryptopp/config.ini
+-rw-rw-r--   0 bubonic   (1000) bubonic   (1000)    18857 2023-06-01 04:49:41.000000 cryptopp-1.0.3/cryptopp/cryptopp.py
+drwxrwxr-x   0 bubonic   (1000) bubonic   (1000)        0 2023-06-01 04:59:52.101266 cryptopp-1.0.3/cryptopp.egg-info/
+-rw-rw-r--   0 bubonic   (1000) bubonic   (1000)     3788 2023-06-01 04:59:52.000000 cryptopp-1.0.3/cryptopp.egg-info/PKG-INFO
+-rw-rw-r--   0 bubonic   (1000) bubonic   (1000)      295 2023-06-01 04:59:52.000000 cryptopp-1.0.3/cryptopp.egg-info/SOURCES.txt
+-rw-rw-r--   0 bubonic   (1000) bubonic   (1000)        1 2023-06-01 04:59:52.000000 cryptopp-1.0.3/cryptopp.egg-info/dependency_links.txt
+-rw-rw-r--   0 bubonic   (1000) bubonic   (1000)       52 2023-06-01 04:59:52.000000 cryptopp-1.0.3/cryptopp.egg-info/entry_points.txt
+-rw-rw-r--   0 bubonic   (1000) bubonic   (1000)       24 2023-06-01 04:59:52.000000 cryptopp-1.0.3/cryptopp.egg-info/requires.txt
+-rw-rw-r--   0 bubonic   (1000) bubonic   (1000)        9 2023-06-01 04:59:52.000000 cryptopp-1.0.3/cryptopp.egg-info/top_level.txt
+-rw-rw-r--   0 bubonic   (1000) bubonic   (1000)       38 2023-06-01 04:59:52.101266 cryptopp-1.0.3/setup.cfg
+-rw-rw-r--   0 bubonic   (1000) bubonic   (1000)      831 2023-06-01 04:58:24.000000 cryptopp-1.0.3/setup.py
```

### Comparing `cryptopp-1.0.2/LICENSE` & `cryptopp-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cryptopp-1.0.2/PKG-INFO` & `cryptopp-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryptopp
-Version: 1.0.2
+Version: 1.0.3
 Summary: Command line Cryptocurrency Portfolio
 Home-page: https://github.com/GordianSimpul/cryptopp
 Author: GordianSimpul/huwwp
 Author-email: gordian@simpul.me
 License: GPLv3
 Keywords: crypto cli portfolio curses cryptocurrency bitcoin
 Classifier: Programming Language :: Python
```

### Comparing `cryptopp-1.0.2/README.rst` & `cryptopp-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `cryptopp-1.0.2/cryptopp/cryptopp.py` & `cryptopp-1.0.3/cryptopp/cryptopp.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
     CONFIG.read(confpath)
     return CONFIG
 
 
 def get_coin_list():
     global CMC_API_KEY
-    cmc_coin_list_url = "https://pro-api.coinmarketcap.com/v2/cryptocurrency/map?CMC_PRO_API_KEY=%s" % CMC_API_KEY
+    cmc_coin_list_url = "https://pro-api.coinmarketcap.com/v1/cryptocurrency/map?CMC_PRO_API_KEY=%s" % CMC_API_KEY
     
     def inner():
         coinJSON = requests.get(cmc_coin_list_url)
         data = coinJSON.content
         with open(COINLIST, 'wb') as f:
             f.write(data)
```

### Comparing `cryptopp-1.0.2/cryptopp.egg-info/PKG-INFO` & `cryptopp-1.0.3/cryptopp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryptopp
-Version: 1.0.2
+Version: 1.0.3
 Summary: Command line Cryptocurrency Portfolio
 Home-page: https://github.com/GordianSimpul/cryptopp
 Author: GordianSimpul/huwwp
 Author-email: gordian@simpul.me
 License: GPLv3
 Keywords: crypto cli portfolio curses cryptocurrency bitcoin
 Classifier: Programming Language :: Python
```

### Comparing `cryptopp-1.0.2/setup.py` & `cryptopp-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 with open('README.rst', encoding="utf-8") as f:
     readme = f.read()
 
 setup(
     name='cryptopp',
-    version='1.0.2',
+    version='1.0.3',
     description='Command line Cryptocurrency Portfolio',
     long_description=readme,
     author='GordianSimpul/huwwp',
     author_email='gordian@simpul.me',
     url='https://github.com/GordianSimpul/cryptopp',
     license='GPLv3',
     keywords='crypto cli portfolio curses cryptocurrency bitcoin',
```

