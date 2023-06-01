# Comparing `tmp/cli2-2.6.1.tar.gz` & `tmp/cli2-2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cli2-2.6.1.tar", last modified: Sun Apr 23 14:48:33 2023, max compression
+gzip compressed data, was "cli2-2.6.2.tar", last modified: Thu Jun  1 07:08:29 2023, max compression
```

## Comparing `cli2-2.6.1.tar` & `cli2-2.6.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 14:48:33.659612 cli2-2.6.1/
--rw-rw-rw-   0 root         (0) root         (0)      161 2023-04-21 18:09:22.000000 cli2-2.6.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2455 2023-04-23 14:48:33.659612 cli2-2.6.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2134 2023-04-21 18:09:22.000000 cli2-2.6.1/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      303 2023-04-21 18:09:22.000000 cli2-2.6.1/classifiers.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 14:48:33.656279 cli2-2.6.1/cli2/
--rw-rw-rw-   0 root         (0) root         (0)      213 2023-04-21 18:09:22.000000 cli2-2.6.1/cli2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12039 2023-04-22 22:55:18.000000 cli2-2.6.1/cli2/argument.py
--rw-rw-rw-   0 root         (0) root         (0)     1118 2023-04-21 18:09:22.000000 cli2-2.6.1/cli2/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2097 2023-04-21 18:09:22.000000 cli2-2.6.1/cli2/colors.py
--rw-rw-rw-   0 root         (0) root         (0)     5840 2023-04-21 19:16:37.000000 cli2-2.6.1/cli2/command.py
--rw-rw-rw-   0 root         (0) root         (0)      480 2023-04-21 18:09:22.000000 cli2-2.6.1/cli2/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     1554 2023-04-21 21:55:13.000000 cli2-2.6.1/cli2/entry_point.py
--rw-rw-rw-   0 root         (0) root         (0)     5653 2023-04-21 18:09:22.000000 cli2-2.6.1/cli2/group.py
--rw-rw-rw-   0 root         (0) root         (0)     2697 2023-04-21 18:09:22.000000 cli2-2.6.1/cli2/node.py
--rw-rw-rw-   0 root         (0) root         (0)     4843 2023-04-21 21:55:13.000000 cli2-2.6.1/cli2/table.py
--rw-rw-rw-   0 root         (0) root         (0)     2518 2023-04-21 21:55:13.000000 cli2-2.6.1/cli2/test.py
--rw-rw-rw-   0 root         (0) root         (0)     1250 2023-04-21 18:09:22.000000 cli2-2.6.1/cli2/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)    11380 2023-04-22 22:55:18.000000 cli2-2.6.1/cli2/test_command.py
--rw-rw-rw-   0 root         (0) root         (0)     2343 2023-04-21 18:09:22.000000 cli2-2.6.1/cli2/test_decorators.py
--rw-rw-rw-   0 root         (0) root         (0)      424 2023-04-21 21:55:13.000000 cli2-2.6.1/cli2/test_entrypoint.py
--rw-rw-rw-   0 root         (0) root         (0)     2506 2023-04-21 21:55:13.000000 cli2-2.6.1/cli2/test_group.py
--rw-rw-rw-   0 root         (0) root         (0)     3237 2023-04-22 22:55:18.000000 cli2-2.6.1/cli2/test_inject.py
--rw-rw-rw-   0 root         (0) root         (0)     2551 2023-04-21 18:09:22.000000 cli2-2.6.1/cli2/test_node.py
--rw-rw-rw-   0 root         (0) root         (0)     2718 2023-04-21 21:56:13.000000 cli2-2.6.1/cli2/test_table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 14:48:33.659612 cli2-2.6.1/cli2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2455 2023-04-23 14:48:33.000000 cli2-2.6.1/cli2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      549 2023-04-23 14:48:33.000000 cli2-2.6.1/cli2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 14:48:33.000000 cli2-2.6.1/cli2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2023-04-23 14:48:33.000000 cli2-2.6.1/cli2.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       60 2023-04-23 14:48:33.000000 cli2-2.6.1/cli2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-04-23 14:48:33.000000 cli2-2.6.1/cli2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-23 14:48:33.659612 cli2-2.6.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      607 2023-04-23 14:48:33.000000 cli2-2.6.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 07:08:29.930542 cli2-2.6.2/
+-rw-rw-rw-   0 root         (0) root         (0)      161 2023-04-21 18:09:22.000000 cli2-2.6.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2455 2023-06-01 07:08:29.930542 cli2-2.6.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2134 2023-04-21 18:09:22.000000 cli2-2.6.2/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      303 2023-04-21 18:09:22.000000 cli2-2.6.2/classifiers.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 07:08:29.930542 cli2-2.6.2/cli2/
+-rw-rw-rw-   0 root         (0) root         (0)      213 2023-04-21 18:09:22.000000 cli2-2.6.2/cli2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12024 2023-06-01 07:06:56.000000 cli2-2.6.2/cli2/argument.py
+-rw-rw-rw-   0 root         (0) root         (0)     1118 2023-04-21 18:09:22.000000 cli2-2.6.2/cli2/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2097 2023-04-21 18:09:22.000000 cli2-2.6.2/cli2/colors.py
+-rw-rw-rw-   0 root         (0) root         (0)     5839 2023-06-01 07:06:56.000000 cli2-2.6.2/cli2/command.py
+-rw-rw-rw-   0 root         (0) root         (0)      480 2023-04-21 18:09:22.000000 cli2-2.6.2/cli2/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     1554 2023-04-21 21:55:13.000000 cli2-2.6.2/cli2/entry_point.py
+-rw-rw-rw-   0 root         (0) root         (0)     5653 2023-04-21 18:09:22.000000 cli2-2.6.2/cli2/group.py
+-rw-rw-rw-   0 root         (0) root         (0)     2697 2023-04-21 18:09:22.000000 cli2-2.6.2/cli2/node.py
+-rw-rw-rw-   0 root         (0) root         (0)     4843 2023-04-21 21:55:13.000000 cli2-2.6.2/cli2/table.py
+-rw-rw-rw-   0 root         (0) root         (0)     2518 2023-04-21 21:55:13.000000 cli2-2.6.2/cli2/test.py
+-rw-rw-rw-   0 root         (0) root         (0)     1250 2023-04-21 18:09:22.000000 cli2-2.6.2/cli2/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    11490 2023-06-01 07:06:56.000000 cli2-2.6.2/cli2/test_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     2343 2023-04-21 18:09:22.000000 cli2-2.6.2/cli2/test_decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)      424 2023-04-21 21:55:13.000000 cli2-2.6.2/cli2/test_entrypoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     2506 2023-04-21 21:55:13.000000 cli2-2.6.2/cli2/test_group.py
+-rw-rw-rw-   0 root         (0) root         (0)     3237 2023-04-22 22:55:18.000000 cli2-2.6.2/cli2/test_inject.py
+-rw-rw-rw-   0 root         (0) root         (0)     2551 2023-04-21 18:09:22.000000 cli2-2.6.2/cli2/test_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     2718 2023-04-21 21:56:13.000000 cli2-2.6.2/cli2/test_table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 07:08:29.930542 cli2-2.6.2/cli2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2455 2023-06-01 07:08:29.000000 cli2-2.6.2/cli2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      549 2023-06-01 07:08:29.000000 cli2-2.6.2/cli2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 07:08:29.000000 cli2-2.6.2/cli2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2023-06-01 07:08:29.000000 cli2-2.6.2/cli2.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       60 2023-06-01 07:08:29.000000 cli2-2.6.2/cli2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-01 07:08:29.000000 cli2-2.6.2/cli2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-01 07:08:29.930542 cli2-2.6.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      607 2023-06-01 07:08:29.000000 cli2-2.6.2/setup.py
```

### Comparing `cli2-2.6.1/PKG-INFO` & `cli2-2.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli2
-Version: 2.6.1
+Version: 2.6.2
 Summary: image:: https://yourlabs.io/oss/cli2/badges/master/pipeline.svg
 Home-page: https://yourlabs.io/oss/cli2
 Author: James Pic
 Author-email: jamespic@gmail.com
 License: MIT
 Keywords: cli
 Requires-Python: >=3.6
```

### Comparing `cli2-2.6.1/README.rst` & `cli2-2.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `cli2-2.6.1/cli2/argument.py` & `cli2-2.6.2/cli2/argument.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,15 +198,15 @@
                     + '='
                     + colors.green
                     + 'somearg'
                 )
             else:
                 self.cmd.print('something=somearg')
         elif self.param.kind == self.param.VAR_POSITIONAL:
-            self.cmd.print('Any number of un-named arguments with equal sign')
+            self.cmd.print('Any number of un-named arguments')
 
         if self.doc:
             self.cmd.print(self.doc)
 
     @property
     def iskw(self):
         """Return True if this argument is not positional."""
@@ -335,15 +335,15 @@
             if argument.aliasmatch(arg):
                 return
 
         # edge case varkwargs
         # priority to varkwargs for word= and **{}
         last = self.cmd[[*self.cmd.keys()][-1]]
         if last is not self and last.param.kind == self.param.VAR_KEYWORD:
-            if re.match('^-?-?\\w+=', arg):
+            if re.match('^-?-?[^=]+=', arg):
                 return
             elif arg.startswith('**{') and arg.endswith('}'):
                 return
 
         if (
             self.iskw
             and self.alias[0].startswith('-')
```

### Comparing `cli2-2.6.1/cli2/cli.py` & `cli2-2.6.2/cli2/cli.py`

 * *Files identical despite different names*

### Comparing `cli2-2.6.1/cli2/colors.py` & `cli2-2.6.2/cli2/colors.py`

 * *Files identical despite different names*

### Comparing `cli2-2.6.1/cli2/command.py` & `cli2-2.6.2/cli2/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,15 @@
             varkw = arg.param.kind == arg.param.VAR_KEYWORD
             if (arg.iskw or varkw) and not shown_kwargs:
                 self.print('ORANGE', 'NAMED ARGUMENTS')
                 shown_kwargs = True
             arg.help()
 
     def parse(self, *argv):
-        """"Parse arguments into BoundArguments."""
+        """Parse arguments into BoundArguments."""
         self.setargs()
         self.bound = self.sig.bind_partial()
         extra = []
         for current in argv:
             taken = False
             for arg in self.values():
                 taken = arg.take(current)
```

### Comparing `cli2-2.6.1/cli2/entry_point.py` & `cli2-2.6.2/cli2/entry_point.py`

 * *Files identical despite different names*

### Comparing `cli2-2.6.1/cli2/group.py` & `cli2-2.6.2/cli2/group.py`

 * *Files identical despite different names*

### Comparing `cli2-2.6.1/cli2/node.py` & `cli2-2.6.2/cli2/node.py`

 * *Files identical despite different names*

### Comparing `cli2-2.6.1/cli2/table.py` & `cli2-2.6.2/cli2/table.py`

 * *Files identical despite different names*

### Comparing `cli2-2.6.1/cli2/test.py` & `cli2-2.6.2/cli2/test.py`

 * *Files identical despite different names*

### Comparing `cli2-2.6.1/cli2/test_cli.py` & `cli2-2.6.2/cli2/test_cli.py`

 * *Files identical despite different names*

### Comparing `cli2-2.6.1/cli2/test_command.py` & `cli2-2.6.2/cli2/test_command.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,22 +90,24 @@
     cmd.parse('x')
     assert cmd['one'].value == 'x'
     with pytest.raises(ValueError):
         cmd['two'].value
 
 
 def test_positional_only_looksahead():
-    def foo(one=None, /, *two, three=None):  # noqa
+    def foo(one=None, /, *two, three=None, **kwargs):  # noqa
         return (one, two)
     cmd = Command(foo)
 
-    cmd.parse('three=z', 'x', 'y')
+    cmd.parse('y.-7=e', 'three=z', 'x', 'y')
     assert cmd['one'].value == 'x'
     assert cmd['two'].value == ['y']
     assert cmd['three'].value == 'z'
+    # make sure it takes weird keywords too
+    assert cmd['kwargs'].value['y.-7'] == 'e'
 
 
 def test_keyword_only():
     def foo(*one, two=None): return (one, two)
     cmd = Command(foo)
 
     cmd.parse('x')
```

### Comparing `cli2-2.6.1/cli2/test_decorators.py` & `cli2-2.6.2/cli2/test_decorators.py`

 * *Files identical despite different names*

### Comparing `cli2-2.6.1/cli2/test_group.py` & `cli2-2.6.2/cli2/test_group.py`

 * *Files identical despite different names*

### Comparing `cli2-2.6.1/cli2/test_inject.py` & `cli2-2.6.2/cli2/test_inject.py`

 * *Files identical despite different names*

### Comparing `cli2-2.6.1/cli2/test_node.py` & `cli2-2.6.2/cli2/test_node.py`

 * *Files identical despite different names*

### Comparing `cli2-2.6.1/cli2/test_table.py` & `cli2-2.6.2/cli2/test_table.py`

 * *Files identical despite different names*

### Comparing `cli2-2.6.1/cli2.egg-info/PKG-INFO` & `cli2-2.6.2/cli2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli2
-Version: 2.6.1
+Version: 2.6.2
 Summary: image:: https://yourlabs.io/oss/cli2/badges/master/pipeline.svg
 Home-page: https://yourlabs.io/oss/cli2
 Author: James Pic
 Author-email: jamespic@gmail.com
 License: MIT
 Keywords: cli
 Requires-Python: >=3.6
```

### Comparing `cli2-2.6.1/cli2.egg-info/SOURCES.txt` & `cli2-2.6.2/cli2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cli2-2.6.1/setup.py` & `cli2-2.6.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name='cli2',
-    version='2.6.1',
+    version='2.6.2',
     setup_requires='setupmeta',
     install_requires=['docstring_parser==0.7.1'],
     extras_require=dict(
         test=[
             'freezegun',
             'pytest',
             'pytest-cov',
```

