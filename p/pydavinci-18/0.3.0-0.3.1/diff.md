# Comparing `tmp/pydavinci_18-0.3.0.tar.gz` & `tmp/pydavinci_18-0.3.1.tar.gz`

## Comparing `pydavinci_18-0.3.0.tar` & `pydavinci_18-0.3.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 pydavinci_18-0.3.0/pydavinci/__init__.py
--rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 pydavinci_18-0.3.0/pydavinci/connect.py
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 pydavinci_18-0.3.0/pydavinci/exceptions.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 pydavinci_18-0.3.0/pydavinci/logger.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 pydavinci_18-0.3.0/pydavinci/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydavinci_18-0.3.0/pydavinci/py.typed
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 pydavinci_18-0.3.0/pydavinci/pyremoteobject.py
--rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 pydavinci_18-0.3.0/pydavinci/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydavinci_18-0.3.0/pydavinci/wrappers/__init__.py
--rw-r--r--   0        0        0    10675 2020-02-02 00:00:00.000000 pydavinci_18-0.3.0/pydavinci/wrappers/_basewrappers.py
--rw-r--r--   0        0        0    15924 2020-02-02 00:00:00.000000 pydavinci_18-0.3.0/pydavinci/wrappers/_resolve_stubs.pyi
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 pydavinci_18-0.3.0/pydavinci/wrappers/folder.py
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 pydavinci_18-0.3.0/pydavinci/wrappers/gallery.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 pydavinci_18-0.3.0/pydavinci/wrappers/gallerystill.py
--rw-r--r--   0        0        0     3221 2020-02-02 00:00:00.000000 pydavinci_18-0.3.0/pydavinci/wrappers/gallerystillalbum.py
--rw-r--r--   0        0        0    12517 2020-02-02 00:00:00.000000 pydavinci_18-0.3.0/pydavinci/wrappers/marker.py
--rw-r--r--   0        0        0    10217 2020-02-02 00:00:00.000000 pydavinci_18-0.3.0/pydavinci/wrappers/mediapool.py
--rw-r--r--   0        0        0     5847 2020-02-02 00:00:00.000000 pydavinci_18-0.3.0/pydavinci/wrappers/mediapoolitem.py
--rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 pydavinci_18-0.3.0/pydavinci/wrappers/mediastorage.py
--rw-r--r--   0        0        0    15592 2020-02-02 00:00:00.000000 pydavinci_18-0.3.0/pydavinci/wrappers/project.py
--rw-r--r--   0        0        0     7051 2020-02-02 00:00:00.000000 pydavinci_18-0.3.0/pydavinci/wrappers/projectmanager.py
--rw-r--r--   0        0        0     6040 2020-02-02 00:00:00.000000 pydavinci_18-0.3.0/pydavinci/wrappers/resolve.py
--rw-r--r--   0        0        0    18979 2020-02-02 00:00:00.000000 pydavinci_18-0.3.0/pydavinci/wrappers/timeline.py
--rw-r--r--   0        0        0    11821 2020-02-02 00:00:00.000000 pydavinci_18-0.3.0/pydavinci/wrappers/timelineitem.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pydavinci_18-0.3.0/pydavinci/wrappers/settings/__init__.py
--rw-r--r--   0        0        0    17744 2020-02-02 00:00:00.000000 pydavinci_18-0.3.0/pydavinci/wrappers/settings/components.py
--rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 pydavinci_18-0.3.0/pydavinci/wrappers/settings/constructor.py
--rw-r--r--   0        0        0     8616 2020-02-02 00:00:00.000000 pydavinci_18-0.3.0/pydavinci/wrappers/settings/map.py
--rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 pydavinci_18-0.3.0/pydavinci/wrappers/settings/validator.py
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 pydavinci_18-0.3.0/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pydavinci_18-0.3.0/LICENSE
--rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 pydavinci_18-0.3.0/README.md
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 pydavinci_18-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4866 2020-02-02 00:00:00.000000 pydavinci_18-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 pydavinci_18-0.3.1/pydavinci/__init__.py
+-rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 pydavinci_18-0.3.1/pydavinci/connect.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 pydavinci_18-0.3.1/pydavinci/exceptions.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 pydavinci_18-0.3.1/pydavinci/logger.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 pydavinci_18-0.3.1/pydavinci/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydavinci_18-0.3.1/pydavinci/py.typed
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 pydavinci_18-0.3.1/pydavinci/pyremoteobject.py
+-rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 pydavinci_18-0.3.1/pydavinci/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydavinci_18-0.3.1/pydavinci/wrappers/__init__.py
+-rw-r--r--   0        0        0    10675 2020-02-02 00:00:00.000000 pydavinci_18-0.3.1/pydavinci/wrappers/_basewrappers.py
+-rw-r--r--   0        0        0    15924 2020-02-02 00:00:00.000000 pydavinci_18-0.3.1/pydavinci/wrappers/_resolve_stubs.pyi
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 pydavinci_18-0.3.1/pydavinci/wrappers/folder.py
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 pydavinci_18-0.3.1/pydavinci/wrappers/gallery.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 pydavinci_18-0.3.1/pydavinci/wrappers/gallerystill.py
+-rw-r--r--   0        0        0     3221 2020-02-02 00:00:00.000000 pydavinci_18-0.3.1/pydavinci/wrappers/gallerystillalbum.py
+-rw-r--r--   0        0        0    12517 2020-02-02 00:00:00.000000 pydavinci_18-0.3.1/pydavinci/wrappers/marker.py
+-rw-r--r--   0        0        0    10217 2020-02-02 00:00:00.000000 pydavinci_18-0.3.1/pydavinci/wrappers/mediapool.py
+-rw-r--r--   0        0        0     5847 2020-02-02 00:00:00.000000 pydavinci_18-0.3.1/pydavinci/wrappers/mediapoolitem.py
+-rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 pydavinci_18-0.3.1/pydavinci/wrappers/mediastorage.py
+-rw-r--r--   0        0        0    15592 2020-02-02 00:00:00.000000 pydavinci_18-0.3.1/pydavinci/wrappers/project.py
+-rw-r--r--   0        0        0     7051 2020-02-02 00:00:00.000000 pydavinci_18-0.3.1/pydavinci/wrappers/projectmanager.py
+-rw-r--r--   0        0        0     6040 2020-02-02 00:00:00.000000 pydavinci_18-0.3.1/pydavinci/wrappers/resolve.py
+-rw-r--r--   0        0        0    18979 2020-02-02 00:00:00.000000 pydavinci_18-0.3.1/pydavinci/wrappers/timeline.py
+-rw-r--r--   0        0        0    11821 2020-02-02 00:00:00.000000 pydavinci_18-0.3.1/pydavinci/wrappers/timelineitem.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pydavinci_18-0.3.1/pydavinci/wrappers/settings/__init__.py
+-rw-r--r--   0        0        0    17744 2020-02-02 00:00:00.000000 pydavinci_18-0.3.1/pydavinci/wrappers/settings/components.py
+-rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 pydavinci_18-0.3.1/pydavinci/wrappers/settings/constructor.py
+-rw-r--r--   0        0        0     8616 2020-02-02 00:00:00.000000 pydavinci_18-0.3.1/pydavinci/wrappers/settings/map.py
+-rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 pydavinci_18-0.3.1/pydavinci/wrappers/settings/validator.py
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 pydavinci_18-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pydavinci_18-0.3.1/LICENSE
+-rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 pydavinci_18-0.3.1/README.md
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 pydavinci_18-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4867 2020-02-02 00:00:00.000000 pydavinci_18-0.3.1/PKG-INFO
```

### Comparing `pydavinci_18-0.3.0/pydavinci/connect.py` & `pydavinci_18-0.3.1/pydavinci/connect.py`

 * *Files identical despite different names*

### Comparing `pydavinci_18-0.3.0/pydavinci/logger.py` & `pydavinci_18-0.3.1/pydavinci/logger.py`

 * *Files identical despite different names*

### Comparing `pydavinci_18-0.3.0/pydavinci/utils.py` & `pydavinci_18-0.3.1/pydavinci/utils.py`

 * *Files identical despite different names*

### Comparing `pydavinci_18-0.3.0/pydavinci/wrappers/_basewrappers.py` & `pydavinci_18-0.3.1/pydavinci/wrappers/_basewrappers.py`

 * *Files identical despite different names*

### Comparing `pydavinci_18-0.3.0/pydavinci/wrappers/_resolve_stubs.pyi` & `pydavinci_18-0.3.1/pydavinci/wrappers/_resolve_stubs.pyi`

 * *Files identical despite different names*

### Comparing `pydavinci_18-0.3.0/pydavinci/wrappers/folder.py` & `pydavinci_18-0.3.1/pydavinci/wrappers/folder.py`

 * *Files identical despite different names*

### Comparing `pydavinci_18-0.3.0/pydavinci/wrappers/gallery.py` & `pydavinci_18-0.3.1/pydavinci/wrappers/gallery.py`

 * *Files identical despite different names*

### Comparing `pydavinci_18-0.3.0/pydavinci/wrappers/gallerystill.py` & `pydavinci_18-0.3.1/pydavinci/wrappers/gallerystill.py`

 * *Files identical despite different names*

### Comparing `pydavinci_18-0.3.0/pydavinci/wrappers/gallerystillalbum.py` & `pydavinci_18-0.3.1/pydavinci/wrappers/gallerystillalbum.py`

 * *Files identical despite different names*

### Comparing `pydavinci_18-0.3.0/pydavinci/wrappers/marker.py` & `pydavinci_18-0.3.1/pydavinci/wrappers/marker.py`

 * *Files identical despite different names*

### Comparing `pydavinci_18-0.3.0/pydavinci/wrappers/mediapool.py` & `pydavinci_18-0.3.1/pydavinci/wrappers/mediapool.py`

 * *Files identical despite different names*

### Comparing `pydavinci_18-0.3.0/pydavinci/wrappers/mediapoolitem.py` & `pydavinci_18-0.3.1/pydavinci/wrappers/mediapoolitem.py`

 * *Files identical despite different names*

### Comparing `pydavinci_18-0.3.0/pydavinci/wrappers/mediastorage.py` & `pydavinci_18-0.3.1/pydavinci/wrappers/mediastorage.py`

 * *Files identical despite different names*

### Comparing `pydavinci_18-0.3.0/pydavinci/wrappers/project.py` & `pydavinci_18-0.3.1/pydavinci/wrappers/project.py`

 * *Files identical despite different names*

### Comparing `pydavinci_18-0.3.0/pydavinci/wrappers/projectmanager.py` & `pydavinci_18-0.3.1/pydavinci/wrappers/projectmanager.py`

 * *Files identical despite different names*

### Comparing `pydavinci_18-0.3.0/pydavinci/wrappers/resolve.py` & `pydavinci_18-0.3.1/pydavinci/wrappers/resolve.py`

 * *Files identical despite different names*

### Comparing `pydavinci_18-0.3.0/pydavinci/wrappers/timeline.py` & `pydavinci_18-0.3.1/pydavinci/wrappers/timeline.py`

 * *Files identical despite different names*

### Comparing `pydavinci_18-0.3.0/pydavinci/wrappers/timelineitem.py` & `pydavinci_18-0.3.1/pydavinci/wrappers/timelineitem.py`

 * *Files identical despite different names*

### Comparing `pydavinci_18-0.3.0/pydavinci/wrappers/settings/components.py` & `pydavinci_18-0.3.1/pydavinci/wrappers/settings/components.py`

 * *Files identical despite different names*

### Comparing `pydavinci_18-0.3.0/pydavinci/wrappers/settings/constructor.py` & `pydavinci_18-0.3.1/pydavinci/wrappers/settings/constructor.py`

 * *Files identical despite different names*

### Comparing `pydavinci_18-0.3.0/pydavinci/wrappers/settings/map.py` & `pydavinci_18-0.3.1/pydavinci/wrappers/settings/map.py`

 * *Files identical despite different names*

### Comparing `pydavinci_18-0.3.0/pydavinci/wrappers/settings/validator.py` & `pydavinci_18-0.3.1/pydavinci/wrappers/settings/validator.py`

 * *Files identical despite different names*

### Comparing `pydavinci_18-0.3.0/.gitignore` & `pydavinci_18-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pydavinci_18-0.3.0/LICENSE` & `pydavinci_18-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydavinci_18-0.3.0/README.md` & `pydavinci_18-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <h1 align='center'>PyDavinci18 🍴</h1>
 
 
-> **Note: This project is a fork of Pydavinci!**
+> **Note**: **This project is a fork of Pydavinci!**
 > 
 > PyDavinci is developed by [Pedro Labonia](https://github.com/pedrolabonia) 
 > - [Original project](https://github.com/pedrolabonia/pydavinci)
 > - [Original docs](https://pedrolabonia.github.io/pydavinci)
 > - [Original PyPi](https://pypi.org/project/pydavinci/)
 
 ---
@@ -18,15 +18,15 @@
 ### What can I expect from this fork?
 I plan to service my needs here where the official project is lacking, but I'm more than happy to collaborate with others on changes. For the moment I may have a little more free time than Pedro, but I do not plan to supplant him, given he has already demonstrated superior skill and expertise for this project! If in time PyDavinci truly appears abandoned and demand increases, I may take this project in a more headstrong direction. Otherwise, if development picks up again, I will contribute my changes and archive this repository.
  
 ### Why PyDavinci at all?
 I personally think PyDavinci is the most comprehensive and intuitive API wrapper for DaVinci Resolve. I'd like to see it continue growing! It's very thorough and makes building Python apps for Resolve quick and easy.
 
 ### Anything else to note?
-- Although the package's name is `in03_pydavinci`, do not install this alongside the original, as installations will collide. The project uses the same namespace as `pydavinci`.
+- Although the package's name is `pydavinci18`, do not install this alongside the original, as installations will collide. The project uses the same namespace as `pydavinci`.
 - Documentation is still sparse as I find time to update it! For now go to the original [PyDavinci project](https://github.com/pedrolabonia/pydavinci)
 
 ---
 
 ## Installation
 
 - PyDavinci requires Python 3.10 or higher
```

### Comparing `pydavinci_18-0.3.0/pyproject.toml` & `pydavinci_18-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pydavinci_18-0.3.0/PKG-INFO` & `pydavinci_18-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydavinci-18
-Version: 0.3.0
+Version: 0.3.1
 Summary: Fork of PyDavinci supporting Resolve 18
 Project-URL: Homepage, https://github.com/in03/pydavinci
 Project-URL: Source, https://github.com/in03/pydavinci
 Project-URL: Documentation, https://in03.github.io/pydavinci/resolve
 Project-URL: Changelog, https://github.com/in03/pydavinci/tags
 Author-email: Caleb Trevatt <sk188okj@duck.com>
 License-File: LICENSE
@@ -29,15 +29,15 @@
 Requires-Dist: mkdocstrings-python; extra == 'docs'
 Requires-Dist: pydavinci[dev]; extra == 'docs'
 Description-Content-Type: text/markdown
 
 <h1 align='center'>PyDavinci18 🍴</h1>
 
 
-> **Note: This project is a fork of Pydavinci!**
+> **Note**: **This project is a fork of Pydavinci!**
 > 
 > PyDavinci is developed by [Pedro Labonia](https://github.com/pedrolabonia) 
 > - [Original project](https://github.com/pedrolabonia/pydavinci)
 > - [Original docs](https://pedrolabonia.github.io/pydavinci)
 > - [Original PyPi](https://pypi.org/project/pydavinci/)
 
 ---
@@ -50,15 +50,15 @@
 ### What can I expect from this fork?
 I plan to service my needs here where the official project is lacking, but I'm more than happy to collaborate with others on changes. For the moment I may have a little more free time than Pedro, but I do not plan to supplant him, given he has already demonstrated superior skill and expertise for this project! If in time PyDavinci truly appears abandoned and demand increases, I may take this project in a more headstrong direction. Otherwise, if development picks up again, I will contribute my changes and archive this repository.
  
 ### Why PyDavinci at all?
 I personally think PyDavinci is the most comprehensive and intuitive API wrapper for DaVinci Resolve. I'd like to see it continue growing! It's very thorough and makes building Python apps for Resolve quick and easy.
 
 ### Anything else to note?
-- Although the package's name is `in03_pydavinci`, do not install this alongside the original, as installations will collide. The project uses the same namespace as `pydavinci`.
+- Although the package's name is `pydavinci18`, do not install this alongside the original, as installations will collide. The project uses the same namespace as `pydavinci`.
 - Documentation is still sparse as I find time to update it! For now go to the original [PyDavinci project](https://github.com/pedrolabonia/pydavinci)
 
 ---
 
 ## Installation
 
 - PyDavinci requires Python 3.10 or higher
```

