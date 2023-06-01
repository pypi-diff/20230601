# Comparing `tmp/st_pop_up_component-0.0.1.tar.gz` & `tmp/st_pop_up_component-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_pop_up_component-0.0.1.tar", last modified: Thu Jun  1 11:38:52 2023, max compression
+gzip compressed data, was "st_pop_up_component-0.0.2.tar", last modified: Thu Jun  1 12:16:41 2023, max compression
```

## Comparing `st_pop_up_component-0.0.1.tar` & `st_pop_up_component-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 11:38:52.573469 st_pop_up_component-0.0.1/
--rw-rw-rw-   0        0        0     1082 2023-05-31 22:38:10.000000 st_pop_up_component-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       56 2023-05-31 22:54:48.000000 st_pop_up_component-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      196 2023-06-01 11:38:52.573082 st_pop_up_component-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-01 11:38:52.574468 st_pop_up_component-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      592 2023-06-01 11:36:45.000000 st_pop_up_component-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-01 11:38:52.515234 st_pop_up_component-0.0.1/st_pop_up_component/
--rw-rw-rw-   0        0        0     4417 2023-06-01 11:31:13.000000 st_pop_up_component-0.0.1/st_pop_up_component/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 11:38:52.499521 st_pop_up_component-0.0.1/st_pop_up_component/frontend/
-drwxrwxrwx   0        0        0        0 2023-06-01 11:38:52.554611 st_pop_up_component-0.0.1/st_pop_up_component/frontend/build/
--rw-rw-rw-   0        0        0      691 2023-06-01 11:32:03.000000 st_pop_up_component-0.0.1/st_pop_up_component/frontend/build/asset-manifest.json
--rw-rw-rw-   0        0        0   206960 2023-05-31 22:38:10.000000 st_pop_up_component-0.0.1/st_pop_up_component/frontend/build/bootstrap.min.css
--rw-rw-rw-   0        0        0     2101 2023-06-01 11:32:03.000000 st_pop_up_component-0.0.1/st_pop_up_component/frontend/build/index.html
-drwxrwxrwx   0        0        0        0 2023-06-01 11:38:52.500521 st_pop_up_component-0.0.1/st_pop_up_component/frontend/build/static/
-drwxrwxrwx   0        0        0        0 2023-06-01 11:38:52.570944 st_pop_up_component-0.0.1/st_pop_up_component/frontend/build/static/js/
--rw-rw-rw-   0        0        0   464244 2023-06-01 11:32:03.000000 st_pop_up_component-0.0.1/st_pop_up_component/frontend/build/static/js/2.a733c068.chunk.js
--rw-rw-rw-   0        0        0     2059 2023-06-01 11:32:03.000000 st_pop_up_component-0.0.1/st_pop_up_component/frontend/build/static/js/2.a733c068.chunk.js.LICENSE.txt
--rw-rw-rw-   0        0        0  1710219 2023-06-01 11:32:03.000000 st_pop_up_component-0.0.1/st_pop_up_component/frontend/build/static/js/2.a733c068.chunk.js.map
--rw-rw-rw-   0        0        0      855 2023-06-01 11:32:03.000000 st_pop_up_component-0.0.1/st_pop_up_component/frontend/build/static/js/main.6500dfab.chunk.js
--rw-rw-rw-   0        0        0     2698 2023-06-01 11:32:03.000000 st_pop_up_component-0.0.1/st_pop_up_component/frontend/build/static/js/main.6500dfab.chunk.js.map
--rw-rw-rw-   0        0        0     1598 2023-06-01 11:32:03.000000 st_pop_up_component-0.0.1/st_pop_up_component/frontend/build/static/js/runtime-main.08bd5a01.js
--rw-rw-rw-   0        0        0     8383 2023-06-01 11:32:03.000000 st_pop_up_component-0.0.1/st_pop_up_component/frontend/build/static/js/runtime-main.08bd5a01.js.map
-drwxrwxrwx   0        0        0        0 2023-06-01 11:38:52.545373 st_pop_up_component-0.0.1/st_pop_up_component.egg-info/
--rw-rw-rw-   0        0        0      196 2023-06-01 11:38:52.000000 st_pop_up_component-0.0.1/st_pop_up_component.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      923 2023-06-01 11:38:52.000000 st_pop_up_component-0.0.1/st_pop_up_component.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 11:38:52.000000 st_pop_up_component-0.0.1/st_pop_up_component.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-01 11:38:52.000000 st_pop_up_component-0.0.1/st_pop_up_component.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-06-01 11:38:52.000000 st_pop_up_component-0.0.1/st_pop_up_component.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-01 12:16:41.567953 st_pop_up_component-0.0.2/
+-rw-rw-rw-   0        0        0     1082 2023-05-31 22:38:10.000000 st_pop_up_component-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       56 2023-05-31 22:54:48.000000 st_pop_up_component-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      196 2023-06-01 12:16:41.566659 st_pop_up_component-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-01 12:16:41.567953 st_pop_up_component-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      592 2023-06-01 12:12:51.000000 st_pop_up_component-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 12:16:41.509524 st_pop_up_component-0.0.2/st_pop_up_component/
+-rw-rw-rw-   0        0        0     4417 2023-06-01 12:13:49.000000 st_pop_up_component-0.0.2/st_pop_up_component/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 12:16:41.489007 st_pop_up_component-0.0.2/st_pop_up_component/frontend/
+drwxrwxrwx   0        0        0        0 2023-06-01 12:16:41.547997 st_pop_up_component-0.0.2/st_pop_up_component/frontend/build/
+-rw-rw-rw-   0        0        0      691 2023-06-01 11:32:03.000000 st_pop_up_component-0.0.2/st_pop_up_component/frontend/build/asset-manifest.json
+-rw-rw-rw-   0        0        0   206960 2023-05-31 22:38:10.000000 st_pop_up_component-0.0.2/st_pop_up_component/frontend/build/bootstrap.min.css
+-rw-rw-rw-   0        0        0     2101 2023-06-01 11:32:03.000000 st_pop_up_component-0.0.2/st_pop_up_component/frontend/build/index.html
+drwxrwxrwx   0        0        0        0 2023-06-01 12:16:41.490330 st_pop_up_component-0.0.2/st_pop_up_component/frontend/build/static/
+drwxrwxrwx   0        0        0        0 2023-06-01 12:16:41.565075 st_pop_up_component-0.0.2/st_pop_up_component/frontend/build/static/js/
+-rw-rw-rw-   0        0        0   464244 2023-06-01 11:32:03.000000 st_pop_up_component-0.0.2/st_pop_up_component/frontend/build/static/js/2.a733c068.chunk.js
+-rw-rw-rw-   0        0        0     2059 2023-06-01 11:32:03.000000 st_pop_up_component-0.0.2/st_pop_up_component/frontend/build/static/js/2.a733c068.chunk.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  1710219 2023-06-01 11:32:03.000000 st_pop_up_component-0.0.2/st_pop_up_component/frontend/build/static/js/2.a733c068.chunk.js.map
+-rw-rw-rw-   0        0        0      855 2023-06-01 11:32:03.000000 st_pop_up_component-0.0.2/st_pop_up_component/frontend/build/static/js/main.6500dfab.chunk.js
+-rw-rw-rw-   0        0        0     2698 2023-06-01 11:32:03.000000 st_pop_up_component-0.0.2/st_pop_up_component/frontend/build/static/js/main.6500dfab.chunk.js.map
+-rw-rw-rw-   0        0        0     1598 2023-06-01 11:32:03.000000 st_pop_up_component-0.0.2/st_pop_up_component/frontend/build/static/js/runtime-main.08bd5a01.js
+-rw-rw-rw-   0        0        0     8383 2023-06-01 11:32:03.000000 st_pop_up_component-0.0.2/st_pop_up_component/frontend/build/static/js/runtime-main.08bd5a01.js.map
+drwxrwxrwx   0        0        0        0 2023-06-01 12:16:41.540300 st_pop_up_component-0.0.2/st_pop_up_component.egg-info/
+-rw-rw-rw-   0        0        0      196 2023-06-01 12:16:41.000000 st_pop_up_component-0.0.2/st_pop_up_component.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      923 2023-06-01 12:16:41.000000 st_pop_up_component-0.0.2/st_pop_up_component.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 12:16:41.000000 st_pop_up_component-0.0.2/st_pop_up_component.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-01 12:16:41.000000 st_pop_up_component-0.0.2/st_pop_up_component.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-06-01 12:16:41.000000 st_pop_up_component-0.0.2/st_pop_up_component.egg-info/top_level.txt
```

### Comparing `st_pop_up_component-0.0.1/LICENSE` & `st_pop_up_component-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `st_pop_up_component-0.0.1/setup.py` & `st_pop_up_component-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="st_pop_up_component",
-    version="0.0.1",
+    version="0.0.2",
     author="Siva S",
     author_email="",
     description="",
     long_description="",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `st_pop_up_component-0.0.1/st_pop_up_component/__init__.py` & `st_pop_up_component-0.0.2/st_pop_up_component/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 
 # Create a wrapper function for the component. This is an optional
 # best practice - we could simply expose the component function returned by
 # `declare_component` and call it done. The wrapper allows us to customize
 # our component's API: we can pre-process its input args, post-process its
 # output value, and add a docstring for users.
-def pop_up_component(message:str,key :Any):
+def st_custom_pop_up(message:str,key :Any):
     """Create a new instance of "st_pop_up_component".
 
     Parameters
     ----------
     name: str
         The name of the thing we're saying hello to. The component will display
         the text "Hello, {name}!"
```

### Comparing `st_pop_up_component-0.0.1/st_pop_up_component/frontend/build/asset-manifest.json` & `st_pop_up_component-0.0.2/st_pop_up_component/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `st_pop_up_component-0.0.1/st_pop_up_component/frontend/build/bootstrap.min.css` & `st_pop_up_component-0.0.2/st_pop_up_component/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `st_pop_up_component-0.0.1/st_pop_up_component/frontend/build/index.html` & `st_pop_up_component-0.0.2/st_pop_up_component/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `st_pop_up_component-0.0.1/st_pop_up_component/frontend/build/static/js/2.a733c068.chunk.js` & `st_pop_up_component-0.0.2/st_pop_up_component/frontend/build/static/js/2.a733c068.chunk.js`

 * *Files identical despite different names*

### Comparing `st_pop_up_component-0.0.1/st_pop_up_component/frontend/build/static/js/2.a733c068.chunk.js.LICENSE.txt` & `st_pop_up_component-0.0.2/st_pop_up_component/frontend/build/static/js/2.a733c068.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `st_pop_up_component-0.0.1/st_pop_up_component/frontend/build/static/js/2.a733c068.chunk.js.map` & `st_pop_up_component-0.0.2/st_pop_up_component/frontend/build/static/js/2.a733c068.chunk.js.map`

 * *Files identical despite different names*

### Comparing `st_pop_up_component-0.0.1/st_pop_up_component/frontend/build/static/js/main.6500dfab.chunk.js` & `st_pop_up_component-0.0.2/st_pop_up_component/frontend/build/static/js/main.6500dfab.chunk.js`

 * *Files identical despite different names*

### Comparing `st_pop_up_component-0.0.1/st_pop_up_component/frontend/build/static/js/main.6500dfab.chunk.js.map` & `st_pop_up_component-0.0.2/st_pop_up_component/frontend/build/static/js/main.6500dfab.chunk.js.map`

 * *Files identical despite different names*

### Comparing `st_pop_up_component-0.0.1/st_pop_up_component/frontend/build/static/js/runtime-main.08bd5a01.js` & `st_pop_up_component-0.0.2/st_pop_up_component/frontend/build/static/js/runtime-main.08bd5a01.js`

 * *Files identical despite different names*

### Comparing `st_pop_up_component-0.0.1/st_pop_up_component/frontend/build/static/js/runtime-main.08bd5a01.js.map` & `st_pop_up_component-0.0.2/st_pop_up_component/frontend/build/static/js/runtime-main.08bd5a01.js.map`

 * *Files identical despite different names*

### Comparing `st_pop_up_component-0.0.1/st_pop_up_component.egg-info/SOURCES.txt` & `st_pop_up_component-0.0.2/st_pop_up_component.egg-info/SOURCES.txt`

 * *Files identical despite different names*

