# Comparing `tmp/cssbeautifier-1.14.7.tar.gz` & `tmp/cssbeautifier-1.14.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cssbeautifier-1.14.7.tar", last modified: Fri Oct 21 16:34:38 2022, max compression
+gzip compressed data, was "cssbeautifier-1.14.8.tar", last modified: Thu Jun  1 15:31:00 2023, max compression
```

## Comparing `cssbeautifier-1.14.7.tar` & `cssbeautifier-1.14.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 16:34:38.553410 cssbeautifier-1.14.7/
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-10-21 16:32:56.000000 cssbeautifier-1.14.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      291 2022-10-21 16:34:38.553410 cssbeautifier-1.14.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 16:34:38.553410 cssbeautifier-1.14.7/cssbeautifier/
--rw-r--r--   0 runner    (1001) docker     (121)     1883 2022-10-21 16:32:56.000000 cssbeautifier-1.14.7/cssbeautifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-10-21 16:33:59.000000 cssbeautifier-1.14.7/cssbeautifier/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6931 2022-10-21 16:32:56.000000 cssbeautifier-1.14.7/cssbeautifier/_main.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 16:34:38.553410 cssbeautifier-1.14.7/cssbeautifier/css/
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-10-21 16:32:56.000000 cssbeautifier-1.14.7/cssbeautifier/css/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21787 2022-10-21 16:32:56.000000 cssbeautifier-1.14.7/cssbeautifier/css/beautifier.py
--rw-r--r--   0 runner    (1001) docker     (121)     2392 2022-10-21 16:32:56.000000 cssbeautifier-1.14.7/cssbeautifier/css/options.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 16:34:38.549410 cssbeautifier-1.14.7/cssbeautifier/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 16:34:38.553410 cssbeautifier-1.14.7/cssbeautifier/tests/generated/
--rw-r--r--   0 runner    (1001) docker     (121)   327875 2022-10-21 16:34:16.000000 cssbeautifier-1.14.7/cssbeautifier/tests/generated/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 16:34:38.553410 cssbeautifier-1.14.7/cssbeautifier.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      291 2022-10-21 16:34:38.000000 cssbeautifier-1.14.7/cssbeautifier.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      484 2022-10-21 16:34:38.000000 cssbeautifier-1.14.7/cssbeautifier.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-21 16:34:38.000000 cssbeautifier-1.14.7/cssbeautifier.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-10-21 16:34:38.000000 cssbeautifier-1.14.7/cssbeautifier.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-10-21 16:34:38.000000 cssbeautifier-1.14.7/cssbeautifier.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-10-21 16:34:38.000000 cssbeautifier-1.14.7/cssbeautifier.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)      141 2022-10-21 16:32:56.000000 cssbeautifier-1.14.7/js-beautify-test
--rw-r--r--   0 runner    (1001) docker     (121)      218 2022-10-21 16:32:56.000000 cssbeautifier-1.14.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-21 16:34:38.553410 cssbeautifier-1.14.7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     1418 2022-10-21 16:34:38.000000 cssbeautifier-1.14.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:31:00.059179 cssbeautifier-1.14.8/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-01 15:29:28.000000 cssbeautifier-1.14.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-01 15:31:00.059179 cssbeautifier-1.14.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:31:00.055179 cssbeautifier-1.14.8/cssbeautifier/
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-01 15:30:26.000000 cssbeautifier-1.14.8/cssbeautifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 15:30:26.000000 cssbeautifier-1.14.8/cssbeautifier/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-06-01 15:30:26.000000 cssbeautifier-1.14.8/cssbeautifier/_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:31:00.055179 cssbeautifier-1.14.8/cssbeautifier/css/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-01 15:29:28.000000 cssbeautifier-1.14.8/cssbeautifier/css/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21785 2023-06-01 15:30:26.000000 cssbeautifier-1.14.8/cssbeautifier/css/beautifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-01 15:29:28.000000 cssbeautifier-1.14.8/cssbeautifier/css/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:31:00.055179 cssbeautifier-1.14.8/cssbeautifier/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:31:00.055179 cssbeautifier-1.14.8/cssbeautifier/tests/generated/
+-rw-r--r--   0 runner    (1001) docker     (123)   328300 2023-06-01 15:30:40.000000 cssbeautifier-1.14.8/cssbeautifier/tests/generated/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:31:00.055179 cssbeautifier-1.14.8/cssbeautifier.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-01 15:31:00.000000 cssbeautifier-1.14.8/cssbeautifier.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-01 15:31:00.000000 cssbeautifier-1.14.8/cssbeautifier.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 15:31:00.000000 cssbeautifier-1.14.8/cssbeautifier.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-01 15:31:00.000000 cssbeautifier-1.14.8/cssbeautifier.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-01 15:31:00.000000 cssbeautifier-1.14.8/cssbeautifier.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-01 15:31:00.000000 cssbeautifier-1.14.8/cssbeautifier.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      141 2023-06-01 15:29:28.000000 cssbeautifier-1.14.8/js-beautify-test
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-01 15:29:28.000000 cssbeautifier-1.14.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 15:31:00.059179 cssbeautifier-1.14.8/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1418 2023-06-01 15:30:59.000000 cssbeautifier-1.14.8/setup.py
```

### Comparing `cssbeautifier-1.14.7/cssbeautifier/__init__.py` & `cssbeautifier-1.14.8/cssbeautifier/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 def beautify(string, opts=None):
     _main = __import__("cssbeautifier", globals(), locals(), ["_main"])._main
     return _main.beautify(string, opts)
 
 
 def beautify_file(file_name, opts=None):
     _main = __import__("cssbeautifier", globals(), locals(), ["_main"])._main
-    return _main.beautify_file(file, opts)
+    return _main.beautify_file(file_name, opts)
 
 
 def usage(stream=sys.stdout):
     _main = __import__("cssbeautifier", globals(), locals(), ["_main"])._main
     return _main._sage(stream)
```

### Comparing `cssbeautifier-1.14.7/cssbeautifier/_main.py` & `cssbeautifier-1.14.8/cssbeautifier/_main.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,14 @@
 
 
 def beautify_file(file_name, opts=None):
     return process_file(file_name, opts, beautify)
 
 
 def usage(stream=sys.stdout):
-
     print(
         "cssbeautifier.py@"
         + __version__
         + """
 
 CSS beautifier (https://beautifier.io/)
 
@@ -98,15 +97,14 @@
     if stream == sys.stderr:
         return 1
     else:
         return 0
 
 
 def main():
-
     argv = sys.argv[1:]
 
     try:
         opts, args = getopt.getopt(
             argv,
             "hvio:rs:c:e:tnb:",
             [
```

### Comparing `cssbeautifier-1.14.7/cssbeautifier/css/beautifier.py` & `cssbeautifier-1.14.8/cssbeautifier/css/beautifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,14 @@
         stream = open(file_name)
     content = "".join(stream.readlines())
     b = Beautifier(content, opts)
     return b.beautify()
 
 
 def usage(stream=sys.stdout):
-
     print(
         "cssbeautifier.py@"
         + __version__
         + """
 
 CSS beautifier (https://beautifier.io/)
 
@@ -380,15 +379,14 @@
                     if self._input.peek() != "}":
                         self._output.add_new_line(True)
                 if self._input.peek() == ")":
                     self._output.trim(True)
                     if self._options.brace_style == "expand":
                         self._output.add_new_line(True)
             elif self._ch == ":":
-
                 for i in range(0, len(self.NON_SEMICOLON_NEWLINE_PROPERTY)):
                     if self._input.lookBack(self.NON_SEMICOLON_NEWLINE_PROPERTY[i]):
                         insideNonSemiColonValues = True
                         break
 
                 if (
                     (insideRule or enteringConditionalGroup)
```

### Comparing `cssbeautifier-1.14.7/cssbeautifier/css/options.py` & `cssbeautifier-1.14.8/cssbeautifier/css/options.py`

 * *Files identical despite different names*

### Comparing `cssbeautifier-1.14.7/cssbeautifier/tests/generated/tests.py` & `cssbeautifier-1.14.8/cssbeautifier/tests/generated/tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -11114,14 +11114,26 @@
         t(
             'p {\n' +
             '    color: blue;\n' +
             '}')
 
 
         #============================================================
+        # Issue #2012, #2147
+        self.reset_options()
+        t('@extend .btn-blue:hover;')
+        t('@import url("chrome://communicator/skin/");')
+        t('@apply w-4 lg:w-10 space-y-3 lg:space-x-12;')
+        t(
+            'h3 {\n' +
+            '    @apply flex flex-col lg:flex-row space-y-3 lg:space-x-12 items-start;\n' +
+            '}')
+
+
+        #============================================================
         # 
         self.reset_options()
 
 
 
     def testNewline(self):
         self.reset_options()
```

### Comparing `cssbeautifier-1.14.7/setup.py` & `cssbeautifier-1.14.8/setup.py`

 * *Files identical despite different names*

