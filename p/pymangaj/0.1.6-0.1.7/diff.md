# Comparing `tmp/pymangaj-0.1.6.tar.gz` & `tmp/pymangaj-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymangaj-0.1.6.tar", last modified: Wed May 31 00:17:40 2023, max compression
+gzip compressed data, was "pymangaj-0.1.7.tar", last modified: Thu Jun  1 00:31:01 2023, max compression
```

## Comparing `pymangaj-0.1.6.tar` & `pymangaj-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 00:17:40.478164 pymangaj-0.1.6/
--rw-rw-rw-   0        0        0     1106 2023-05-02 22:15:56.000000 pymangaj-0.1.6/LICENSE
--rw-rw-rw-   0        0        0     2061 2023-05-31 00:17:40.478164 pymangaj-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     1386 2023-05-30 04:12:15.000000 pymangaj-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 00:17:40.458164 pymangaj-0.1.6/pymangaj/
--rw-rw-rw-   0        0        0       41 2023-05-30 04:12:41.000000 pymangaj-0.1.6/pymangaj/__init__.py
--rw-rw-rw-   0        0        0     3324 2023-05-30 23:43:38.000000 pymangaj-0.1.6/pymangaj/mangalivre.py
--rw-rw-rw-   0        0        0     1665 2023-05-30 01:42:44.000000 pymangaj-0.1.6/pymangaj/muitomanga.py
--rw-rw-rw-   0        0        0     1051 2023-05-31 00:13:55.000000 pymangaj-0.1.6/pymangaj/pymangaj.py
-drwxrwxrwx   0        0        0        0 2023-05-31 00:17:40.476164 pymangaj-0.1.6/pymangaj.egg-info/
--rw-rw-rw-   0        0        0     2061 2023-05-31 00:17:40.000000 pymangaj-0.1.6/pymangaj.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-05-31 00:17:40.000000 pymangaj-0.1.6/pymangaj.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 00:17:40.000000 pymangaj-0.1.6/pymangaj.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-31 00:17:40.000000 pymangaj-0.1.6/pymangaj.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 00:17:40.478164 pymangaj-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      868 2023-05-31 00:17:24.000000 pymangaj-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 00:31:01.117208 pymangaj-0.1.7/
+-rw-rw-rw-   0        0        0     1106 2023-05-02 22:15:56.000000 pymangaj-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0     2208 2023-06-01 00:31:01.117208 pymangaj-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1533 2023-06-01 00:19:06.000000 pymangaj-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 00:31:01.087209 pymangaj-0.1.7/pymangaj/
+-rw-rw-rw-   0        0        0       41 2023-05-30 04:12:41.000000 pymangaj-0.1.7/pymangaj/__init__.py
+-rw-rw-rw-   0        0        0     2927 2023-06-01 00:19:10.000000 pymangaj-0.1.7/pymangaj/chapmanganato.py
+-rw-rw-rw-   0        0        0     3324 2023-06-01 00:17:11.000000 pymangaj-0.1.7/pymangaj/mangalivre.py
+-rw-rw-rw-   0        0        0     1665 2023-05-30 01:42:44.000000 pymangaj-0.1.7/pymangaj/muitomanga.py
+-rw-rw-rw-   0        0        0     1177 2023-06-01 00:17:43.000000 pymangaj-0.1.7/pymangaj/pymangaj.py
+drwxrwxrwx   0        0        0        0 2023-06-01 00:31:01.115207 pymangaj-0.1.7/pymangaj.egg-info/
+-rw-rw-rw-   0        0        0     2208 2023-06-01 00:31:00.000000 pymangaj-0.1.7/pymangaj.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2023-06-01 00:31:00.000000 pymangaj-0.1.7/pymangaj.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 00:31:00.000000 pymangaj-0.1.7/pymangaj.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-01 00:31:00.000000 pymangaj-0.1.7/pymangaj.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 00:31:01.117208 pymangaj-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      868 2023-06-01 00:27:48.000000 pymangaj-0.1.7/setup.py
```

### Comparing `pymangaj-0.1.6/LICENSE` & `pymangaj-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pymangaj-0.1.6/PKG-INFO` & `pymangaj-0.1.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymangaj
-Version: 0.1.6
+Version: 0.1.7
 Summary: Search and download mangas.
 Home-page: https://github.com/jjeanjacques10/pymangaj
 Author: Jean Jacques Barros
 Author-email: jjean.jacques10@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -39,24 +39,26 @@
 pymangaj.search("Naruto", 1, sources=[Sources.MANGA_LIVRE, Sources.MUITO_MANGA])
 ```
 
 ## Sources
 
 pymangaj supports the following manga sources:
 
-|          Source                       | Language | Status | 
-| ------------------------------------- | -------- | ------ | 
-| [MangaLivre](https://mangalivre.net/) |   PT-BR  |   ✅   | 
-| [MuitoManga](https://muitomanga.com/) |   PT-BR  |   ✅   | 
+|          Source                       | Language | Status  |    Source     |
+| ------------------------------------- | -------- | ------  |  ----------   |
+| [MangaLivre](https://mangalivre.net/) |   PT-BR  |   ✅   |  MANGA_LIVRE   |
+| [MuitoManga](https://muitomanga.com/) |   PT-BR  |   ✅   |  MUITO_MANGA   |
+| [Manganato](https://manganato.com/)   |   EN-US  |   ✅   |  CHAPMANGANATO |
 
 ## License
 
 This project is licensed under the [MIT License](./LICENSE). See the LICENSE file for details.
 
 ## Contribution
 
 Contributions to pymangaj are welcome! If you have any bug reports, feature requests, or suggestions, please open an issue on the [GitHub repository](https://github.com/jjeanjacques10/pymangaj).
 
 ## Authors
 
 - [@jjeanjacques10](https://github.com/jjeanjacques10)
 
+
```

### Comparing `pymangaj-0.1.6/README.md` & `pymangaj-0.1.7/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -20,23 +20,24 @@
 pymangaj.search("Naruto", 1, sources=[Sources.MANGA_LIVRE, Sources.MUITO_MANGA])
 ```
 
 ## Sources
 
 pymangaj supports the following manga sources:
 
-|          Source                       | Language | Status | 
-| ------------------------------------- | -------- | ------ | 
-| [MangaLivre](https://mangalivre.net/) |   PT-BR  |   ✅   | 
-| [MuitoManga](https://muitomanga.com/) |   PT-BR  |   ✅   | 
+|          Source                       | Language | Status  |    Source     |
+| ------------------------------------- | -------- | ------  |  ----------   |
+| [MangaLivre](https://mangalivre.net/) |   PT-BR  |   ✅   |  MANGA_LIVRE   |
+| [MuitoManga](https://muitomanga.com/) |   PT-BR  |   ✅   |  MUITO_MANGA   |
+| [Manganato](https://manganato.com/)   |   EN-US  |   ✅   |  CHAPMANGANATO |
 
 ## License
 
 This project is licensed under the [MIT License](./LICENSE). See the LICENSE file for details.
 
 ## Contribution
 
 Contributions to pymangaj are welcome! If you have any bug reports, feature requests, or suggestions, please open an issue on the [GitHub repository](https://github.com/jjeanjacques10/pymangaj).
 
 ## Authors
 
-- [@jjeanjacques10](https://github.com/jjeanjacques10)
+- [@jjeanjacques10](https://github.com/jjeanjacques10)
```

### Comparing `pymangaj-0.1.6/pymangaj/mangalivre.py` & `pymangaj-0.1.7/pymangaj/mangalivre.py`

 * *Files identical despite different names*

### Comparing `pymangaj-0.1.6/pymangaj/muitomanga.py` & `pymangaj-0.1.7/pymangaj/muitomanga.py`

 * *Files identical despite different names*

### Comparing `pymangaj-0.1.6/pymangaj/pymangaj.py` & `pymangaj-0.1.7/pymangaj/pymangaj.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from enum import Enum
 from .mangalivre import MangaLivre
 from .muitomanga import MuitoManga
+from .chapmanganato import Chapmanganato
 
 class Sources(Enum):
     MANGA_LIVRE = 'manga_livre'
     MUITO_MANGA = 'muito_manga'
+    CHAPMANGANATO = 'chapmanganato'
 
 class SourceFactory:
     _value_map = {
         Sources.MANGA_LIVRE: MangaLivre,
-        Sources.MUITO_MANGA: MuitoManga
+        Sources.MUITO_MANGA: MuitoManga,
+        Sources.CHAPMANGANATO: Chapmanganato
     }
 
     @staticmethod
     def get_source(value, manga_name, chapter):
         cls = SourceFactory._value_map[value]
         return cls(manga_name, chapter)
```

### Comparing `pymangaj-0.1.6/pymangaj.egg-info/PKG-INFO` & `pymangaj-0.1.7/pymangaj.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymangaj
-Version: 0.1.6
+Version: 0.1.7
 Summary: Search and download mangas.
 Home-page: https://github.com/jjeanjacques10/pymangaj
 Author: Jean Jacques Barros
 Author-email: jjean.jacques10@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -39,24 +39,26 @@
 pymangaj.search("Naruto", 1, sources=[Sources.MANGA_LIVRE, Sources.MUITO_MANGA])
 ```
 
 ## Sources
 
 pymangaj supports the following manga sources:
 
-|          Source                       | Language | Status | 
-| ------------------------------------- | -------- | ------ | 
-| [MangaLivre](https://mangalivre.net/) |   PT-BR  |   ✅   | 
-| [MuitoManga](https://muitomanga.com/) |   PT-BR  |   ✅   | 
+|          Source                       | Language | Status  |    Source     |
+| ------------------------------------- | -------- | ------  |  ----------   |
+| [MangaLivre](https://mangalivre.net/) |   PT-BR  |   ✅   |  MANGA_LIVRE   |
+| [MuitoManga](https://muitomanga.com/) |   PT-BR  |   ✅   |  MUITO_MANGA   |
+| [Manganato](https://manganato.com/)   |   EN-US  |   ✅   |  CHAPMANGANATO |
 
 ## License
 
 This project is licensed under the [MIT License](./LICENSE). See the LICENSE file for details.
 
 ## Contribution
 
 Contributions to pymangaj are welcome! If you have any bug reports, feature requests, or suggestions, please open an issue on the [GitHub repository](https://github.com/jjeanjacques10/pymangaj).
 
 ## Authors
 
 - [@jjeanjacques10](https://github.com/jjeanjacques10)
 
+
```

### Comparing `pymangaj-0.1.6/setup.py` & `pymangaj-0.1.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='pymangaj',
-    version='0.1.6',
+    version='0.1.7',
     description='Search and download mangas.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Jean Jacques Barros',
     author_email='jjean.jacques10@gmail.com',
     url='https://github.com/jjeanjacques10/pymangaj',
     packages=find_packages(),
```

