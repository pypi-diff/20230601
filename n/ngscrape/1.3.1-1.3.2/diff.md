# Comparing `tmp/ngscrape-1.3.1.tar.gz` & `tmp/ngscrape-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngscrape-1.3.1.tar", last modified: Wed May 31 23:19:00 2023, max compression
+gzip compressed data, was "ngscrape-1.3.2.tar", last modified: Wed May 31 23:47:41 2023, max compression
```

## Comparing `ngscrape-1.3.1.tar` & `ngscrape-1.3.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 23:19:00.884802 ngscrape-1.3.1/
--rw-rw-rw-   0        0        0    35184 2023-05-27 22:41:04.000000 ngscrape-1.3.1/LICENSE
--rw-rw-rw-   0        0        0    44094 2023-05-31 23:19:00.883802 ngscrape-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0      738 2023-05-31 23:18:44.000000 ngscrape-1.3.1/pyproject.toml
--rw-rw-rw-   0        0        0     3057 2023-05-31 22:32:29.000000 ngscrape-1.3.1/readme.md
--rw-rw-rw-   0        0        0       42 2023-05-31 23:19:00.884802 ngscrape-1.3.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-31 23:19:00.852795 ngscrape-1.3.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-31 23:19:00.858794 ngscrape-1.3.1/src/ngscrape/
--rw-rw-rw-   0        0        0    11139 2023-05-31 23:18:40.000000 ngscrape-1.3.1/src/ngscrape/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 23:19:00.881805 ngscrape-1.3.1/src/ngscrape.egg-info/
--rw-rw-rw-   0        0        0    44094 2023-05-31 23:19:00.000000 ngscrape-1.3.1/src/ngscrape.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-05-31 23:19:00.000000 ngscrape-1.3.1/src/ngscrape.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 23:19:00.000000 ngscrape-1.3.1/src/ngscrape.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-05-31 23:19:00.000000 ngscrape-1.3.1/src/ngscrape.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-31 23:19:00.000000 ngscrape-1.3.1/src/ngscrape.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 23:47:41.415890 ngscrape-1.3.2/
+-rw-rw-rw-   0        0        0    35184 2023-05-27 22:41:04.000000 ngscrape-1.3.2/LICENSE
+-rw-rw-rw-   0        0        0    44094 2023-05-31 23:47:41.413370 ngscrape-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0      738 2023-05-31 23:47:21.000000 ngscrape-1.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0     3057 2023-05-31 22:32:29.000000 ngscrape-1.3.2/readme.md
+-rw-rw-rw-   0        0        0       42 2023-05-31 23:47:41.415890 ngscrape-1.3.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-31 23:47:41.352818 ngscrape-1.3.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-31 23:47:41.361806 ngscrape-1.3.2/src/ngscrape/
+-rw-rw-rw-   0        0        0    11147 2023-05-31 23:47:07.000000 ngscrape-1.3.2/src/ngscrape/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 23:47:41.409814 ngscrape-1.3.2/src/ngscrape.egg-info/
+-rw-rw-rw-   0        0        0    44094 2023-05-31 23:47:41.000000 ngscrape-1.3.2/src/ngscrape.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-05-31 23:47:41.000000 ngscrape-1.3.2/src/ngscrape.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 23:47:41.000000 ngscrape-1.3.2/src/ngscrape.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-31 23:47:41.000000 ngscrape-1.3.2/src/ngscrape.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-31 23:47:41.000000 ngscrape-1.3.2/src/ngscrape.egg-info/top_level.txt
```

### Comparing `ngscrape-1.3.1/LICENSE` & `ngscrape-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ngscrape-1.3.1/PKG-INFO` & `ngscrape-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngscrape
-Version: 1.3.1
+Version: 1.3.2
 Summary: Newgrounds flash game scraper powered by bs4 and requests
 Author-email: aeiea <dpthn@proton.me>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ngscrape-1.3.1/pyproject.toml` & `ngscrape-1.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "ngscrape"
-version = "1.3.1"
+version = "1.3.2"
 description = "Newgrounds flash game scraper powered by bs4 and requests"
 readme = "readme.md"
 authors = [{ name = "aeiea", email = "dpthn@proton.me" }]
 license = {file = "LICENSE"}
 classifiers = [
     "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
     "Programming Language :: Python",
```

### Comparing `ngscrape-1.3.1/readme.md` & `ngscrape-1.3.2/readme.md`

 * *Files identical despite different names*

### Comparing `ngscrape-1.3.1/src/ngscrape/__init__.py` & `ngscrape-1.3.2/src/ngscrape/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,17 +77,18 @@
             - `download = 'testdir'`
             - `filename = 'game.swf'`
         - Example output with debug mode:
             - NGScrape: Made request to `https://www.newgrounds.com/portal/view/59593` and got status code `200`
             - NGScrape: Found flash game link `https:\/\/uploads.ungrounded.net\/59000\/59593_alien_booya.swf?f1101313499`
             - NGScrape: Downloaded swf file to testdir/game.swf
         '''
-        if self.cachedsites[url] != None:
+        try:
+            self.cachedsites[url]
             _gameHTML = self.cachedsites[url]
-        else:
+        except:
             if self.cache:
                 self.cachedsites[url] = _gameHTML
             _gameHTML = requests.get(url)
         _soup = bs4.BeautifulSoup(_gameHTML.content, 'html.parser')
         if self.debug:
             print('NGScrape: Made request to ' + url + ' and got status code ' + str(_gameHTML.status_code))
         '''
```

### Comparing `ngscrape-1.3.1/src/ngscrape.egg-info/PKG-INFO` & `ngscrape-1.3.2/src/ngscrape.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngscrape
-Version: 1.3.1
+Version: 1.3.2
 Summary: Newgrounds flash game scraper powered by bs4 and requests
 Author-email: aeiea <dpthn@proton.me>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

