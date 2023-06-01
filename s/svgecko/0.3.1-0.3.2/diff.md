# Comparing `tmp/svgecko-0.3.1.tar.gz` & `tmp/svgecko-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svgecko-0.3.1.tar", last modified: Mon May 29 09:12:58 2023, max compression
+gzip compressed data, was "svgecko-0.3.2.tar", last modified: Thu Jun  1 13:58:44 2023, max compression
```

## Comparing `svgecko-0.3.1.tar` & `svgecko-0.3.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:12:58.432427 svgecko-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-29 09:12:58.432427 svgecko-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-29 09:12:44.000000 svgecko-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 09:12:58.436427 svgecko-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-29 09:12:44.000000 svgecko-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:12:58.432427 svgecko-0.3.1/svgecko/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 09:12:44.000000 svgecko-0.3.1/svgecko/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-29 09:12:44.000000 svgecko-0.3.1/svgecko/example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:12:58.432427 svgecko-0.3.1/svgecko/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-29 09:12:44.000000 svgecko-0.3.1/svgecko/resources/cross.svg
--rw-r--r--   0 runner    (1001) docker     (123)     9237 2023-05-29 09:12:44.000000 svgecko-0.3.1/svgecko/resources/python-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-05-29 09:12:44.000000 svgecko-0.3.1/svgecko/svg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-05-29 09:12:44.000000 svgecko-0.3.1/svgecko/svg_path.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-29 09:12:44.000000 svgecko-0.3.1/svgecko/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:12:58.432427 svgecko-0.3.1/svgecko.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-29 09:12:58.000000 svgecko-0.3.1/svgecko.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-29 09:12:58.000000 svgecko-0.3.1/svgecko.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 09:12:58.000000 svgecko-0.3.1/svgecko.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-29 09:12:58.000000 svgecko-0.3.1/svgecko.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-29 09:12:58.000000 svgecko-0.3.1/svgecko.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:12:58.432427 svgecko-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 09:12:44.000000 svgecko-0.3.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-29 09:12:44.000000 svgecko-0.3.1/tests/test_svg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:58:44.041228 svgecko-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-01 13:58:44.041228 svgecko-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-01 13:58:32.000000 svgecko-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 13:58:44.041228 svgecko-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-01 13:58:32.000000 svgecko-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:58:44.037228 svgecko-0.3.2/svgecko/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:58:32.000000 svgecko-0.3.2/svgecko/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-01 13:58:32.000000 svgecko-0.3.2/svgecko/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:58:44.041228 svgecko-0.3.2/svgecko/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-01 13:58:32.000000 svgecko-0.3.2/svgecko/resources/cross.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9237 2023-06-01 13:58:32.000000 svgecko-0.3.2/svgecko/resources/python-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-06-01 13:58:32.000000 svgecko-0.3.2/svgecko/svg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-06-01 13:58:32.000000 svgecko-0.3.2/svgecko/svg_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-01 13:58:32.000000 svgecko-0.3.2/svgecko/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:58:44.041228 svgecko-0.3.2/svgecko.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-01 13:58:44.000000 svgecko-0.3.2/svgecko.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-01 13:58:44.000000 svgecko-0.3.2/svgecko.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 13:58:44.000000 svgecko-0.3.2/svgecko.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-01 13:58:44.000000 svgecko-0.3.2/svgecko.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-01 13:58:44.000000 svgecko-0.3.2/svgecko.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:58:44.041228 svgecko-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:58:32.000000 svgecko-0.3.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-01 13:58:32.000000 svgecko-0.3.2/tests/test_svg.py
```

### Comparing `svgecko-0.3.1/README.md` & `svgecko-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `svgecko-0.3.1/setup.py` & `svgecko-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='svgecko',
-    version='0.3.1',
+    version='0.3.2',
     author='Josef Ondrej',
     author_email='josef.ondrej@outlook.com',
     description='Lightweight library for arbitrary geometric SVG transformations',
     long_description='Lightweight library for arbitrary geometric SVG transformations',
     long_description_content_type='text/markdown',
     packages=find_packages(),
     package_data={'svgecko': ['resources/*.svg']},
```

### Comparing `svgecko-0.3.1/svgecko/resources/python-logo.svg` & `svgecko-0.3.2/svgecko/resources/python-logo.svg`

 * *Files identical despite different names*

### Comparing `svgecko-0.3.1/svgecko/svg.py` & `svgecko-0.3.2/svgecko/svg.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         self._transform_paths(svg, transformation)
         self._transform_xy_attributes(svg, transformation)
 
         return svg
 
     @staticmethod
     def _transform_xy_attributes(svg: SVG, transformation: Callable[[Tuple[float, float]], Tuple[float, float]]):
-        for attribute_pairs in [('x', 'y'), ('x1', 'y1'), ('x2', 'y2'), ('cx', 'cy')]:
+        for attribute_pairs in [('x', 'y'), ('x1', 'y1'), ('x2', 'y2')]:
             elements_with_both_attributes_selector = f'//*[@{attribute_pairs[0]} and @{attribute_pairs[1]}]'
             elements_with_both_attributes = svg.xml.xpath(elements_with_both_attributes_selector)
             for element in elements_with_both_attributes:
                 x_name, y_name = attribute_pairs
                 x, y = float(element.attrib[x_name]), float(element.attrib[y_name])
                 transformed_x, transformed_y = transformation((x, y))
                 element.attrib[x_name], element.attrib[y_name] = str(transformed_x), str(transformed_y)
```

### Comparing `svgecko-0.3.1/svgecko/svg_path.py` & `svgecko-0.3.2/svgecko/svg_path.py`

 * *Files identical despite different names*

### Comparing `svgecko-0.3.1/tests/test_svg.py` & `svgecko-0.3.2/tests/test_svg.py`

 * *Files identical despite different names*

