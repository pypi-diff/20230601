# Comparing `tmp/jsbeautifier-1.9.1.tar.gz` & `tmp/jsbeautifier-v1.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jsbeautifier-1.9.1.tar", last modified: Mon Mar 25 21:36:24 2019, max compression
+gzip compressed data, was "dist/jsbeautifier-v1.5.8.tar", last modified: Thu Jun 25 19:34:13 2015, max compression
```

## Comparing `jsbeautifier-1.9.1.tar` & `jsbeautifier-v1.5.8.tar`

### file list

```diff
@@ -1,54 +1,26 @@
-drwxr-xr-x   0 bitwiseman   (501) staff       (20)        0 2019-03-25 21:36:24.000000 jsbeautifier-1.9.1/
--rw-r--r--   0 bitwiseman   (501) staff       (20)       45 2017-05-04 02:03:00.000000 jsbeautifier-1.9.1/MANIFEST.in
--rw-r--r--   0 bitwiseman   (501) staff       (20)      340 2019-03-25 21:36:24.000000 jsbeautifier-1.9.1/PKG-INFO
--rwxr-xr-x   0 bitwiseman   (501) staff       (20)      141 2017-05-04 02:03:00.000000 jsbeautifier-1.9.1/js-beautify-test
-drwxr-xr-x   0 bitwiseman   (501) staff       (20)        0 2019-03-25 21:36:24.000000 jsbeautifier-1.9.1/jsbeautifier/
--rw-r--r--   0 bitwiseman   (501) staff       (20)    16957 2019-03-25 21:35:34.000000 jsbeautifier-1.9.1/jsbeautifier/__init__.py
--rw-r--r--   0 bitwiseman   (501) staff       (20)       22 2019-03-25 21:35:34.000000 jsbeautifier-1.9.1/jsbeautifier/__version__.py
-drwxr-xr-x   0 bitwiseman   (501) staff       (20)        0 2019-03-25 21:36:24.000000 jsbeautifier-1.9.1/jsbeautifier/core/
--rw-r--r--   0 bitwiseman   (501) staff       (20)       16 2017-10-08 23:48:06.000000 jsbeautifier-1.9.1/jsbeautifier/core/__init__.py
--rw-r--r--   0 bitwiseman   (501) staff       (20)     2139 2019-01-26 07:36:48.000000 jsbeautifier-1.9.1/jsbeautifier/core/directives.py
--rw-r--r--   0 bitwiseman   (501) staff       (20)     4600 2019-01-26 07:36:48.000000 jsbeautifier-1.9.1/jsbeautifier/core/inputscanner.py
--rw-r--r--   0 bitwiseman   (501) staff       (20)     7488 2019-03-25 21:35:34.000000 jsbeautifier-1.9.1/jsbeautifier/core/options.py
--rw-r--r--   0 bitwiseman   (501) staff       (20)    12051 2019-03-25 21:35:34.000000 jsbeautifier-1.9.1/jsbeautifier/core/output.py
--rw-r--r--   0 bitwiseman   (501) staff       (20)     3004 2019-01-26 07:36:48.000000 jsbeautifier-1.9.1/jsbeautifier/core/pattern.py
--rw-r--r--   0 bitwiseman   (501) staff       (20)     6333 2019-01-26 07:36:48.000000 jsbeautifier-1.9.1/jsbeautifier/core/templatablepattern.py
--rw-r--r--   0 bitwiseman   (501) staff       (20)     1643 2018-09-08 04:13:23.000000 jsbeautifier-1.9.1/jsbeautifier/core/token.py
--rw-r--r--   0 bitwiseman   (501) staff       (20)     4382 2019-01-26 07:36:48.000000 jsbeautifier-1.9.1/jsbeautifier/core/tokenizer.py
--rw-r--r--   0 bitwiseman   (501) staff       (20)     2348 2018-09-08 04:13:23.000000 jsbeautifier-1.9.1/jsbeautifier/core/tokenstream.py
--rw-r--r--   0 bitwiseman   (501) staff       (20)     2782 2019-01-26 07:36:48.000000 jsbeautifier-1.9.1/jsbeautifier/core/whitespacepattern.py
-drwxr-xr-x   0 bitwiseman   (501) staff       (20)        0 2019-03-25 21:36:24.000000 jsbeautifier-1.9.1/jsbeautifier/javascript/
--rw-r--r--   0 bitwiseman   (501) staff       (20)       16 2017-10-08 23:48:06.000000 jsbeautifier-1.9.1/jsbeautifier/javascript/__init__.py
--rw-r--r--   0 bitwiseman   (501) staff       (20)     9285 2019-01-30 11:14:00.000000 jsbeautifier-1.9.1/jsbeautifier/javascript/acorn.py
--rw-r--r--   0 bitwiseman   (501) staff       (20)    59067 2019-01-26 07:36:48.000000 jsbeautifier-1.9.1/jsbeautifier/javascript/beautifier.py
--rw-r--r--   0 bitwiseman   (501) staff       (20)     4374 2018-10-12 07:52:46.000000 jsbeautifier-1.9.1/jsbeautifier/javascript/options.py
--rw-r--r--   0 bitwiseman   (501) staff       (20)    21646 2019-01-26 07:36:48.000000 jsbeautifier-1.9.1/jsbeautifier/javascript/tokenizer.py
-drwxr-xr-x   0 bitwiseman   (501) staff       (20)        0 2019-03-25 21:36:24.000000 jsbeautifier-1.9.1/jsbeautifier/tests/
--rw-r--r--   0 bitwiseman   (501) staff       (20)       16 2017-05-04 02:03:00.000000 jsbeautifier-1.9.1/jsbeautifier/tests/__init__.py
-drwxr-xr-x   0 bitwiseman   (501) staff       (20)        0 2019-03-25 21:36:24.000000 jsbeautifier-1.9.1/jsbeautifier/tests/generated/
--rw-r--r--   0 bitwiseman   (501) staff       (20)       16 2017-05-04 02:03:00.000000 jsbeautifier-1.9.1/jsbeautifier/tests/generated/__init__.py
--rw-r--r--   0 bitwiseman   (501) staff       (20)   283803 2019-03-25 21:35:59.000000 jsbeautifier-1.9.1/jsbeautifier/tests/generated/tests.py
--rw-r--r--   0 bitwiseman   (501) staff       (20)     2603 2018-09-08 04:13:23.000000 jsbeautifier-1.9.1/jsbeautifier/tests/test-packer.py
--rw-r--r--   0 bitwiseman   (501) staff       (20)     1412 2018-09-08 04:13:23.000000 jsbeautifier-1.9.1/jsbeautifier/tests/testindentation.py
-drwxr-xr-x   0 bitwiseman   (501) staff       (20)        0 2019-03-25 21:36:24.000000 jsbeautifier-1.9.1/jsbeautifier/unpackers/
--rw-r--r--   0 bitwiseman   (501) staff       (20)     2319 2018-09-08 04:13:23.000000 jsbeautifier-1.9.1/jsbeautifier/unpackers/__init__.py
--rw-r--r--   0 bitwiseman   (501) staff       (20)     1172 2018-09-10 22:45:19.000000 jsbeautifier-1.9.1/jsbeautifier/unpackers/evalbased.py
--rw-r--r--   0 bitwiseman   (501) staff       (20)     1791 2018-09-10 22:45:19.000000 jsbeautifier-1.9.1/jsbeautifier/unpackers/javascriptobfuscator.py
--rw-r--r--   0 bitwiseman   (501) staff       (20)     2783 2018-09-10 22:45:19.000000 jsbeautifier-1.9.1/jsbeautifier/unpackers/myobfuscate.py
--rw-r--r--   0 bitwiseman   (501) staff       (20)     4738 2019-01-17 08:59:59.000000 jsbeautifier-1.9.1/jsbeautifier/unpackers/packer.py
-drwxr-xr-x   0 bitwiseman   (501) staff       (20)        0 2019-03-25 21:36:24.000000 jsbeautifier-1.9.1/jsbeautifier/unpackers/tests/
--rw-r--r--   0 bitwiseman   (501) staff       (20)       40 2017-05-04 02:03:00.000000 jsbeautifier-1.9.1/jsbeautifier/unpackers/tests/__init__.py
--rw-r--r--   0 bitwiseman   (501) staff       (20)     1584 2018-09-08 04:13:23.000000 jsbeautifier-1.9.1/jsbeautifier/unpackers/tests/testjavascriptobfuscator.py
--rw-r--r--   0 bitwiseman   (501) staff       (20)     1172 2018-09-08 04:13:23.000000 jsbeautifier-1.9.1/jsbeautifier/unpackers/tests/testmyobfuscate.py
--rw-r--r--   0 bitwiseman   (501) staff       (20)     1702 2019-01-17 08:59:59.000000 jsbeautifier-1.9.1/jsbeautifier/unpackers/tests/testpacker.py
--rw-r--r--   0 bitwiseman   (501) staff       (20)     1058 2018-09-08 04:13:23.000000 jsbeautifier-1.9.1/jsbeautifier/unpackers/tests/testurlencode.py
--rw-r--r--   0 bitwiseman   (501) staff       (20)      981 2018-09-10 22:45:19.000000 jsbeautifier-1.9.1/jsbeautifier/unpackers/urlencode.py
-drwxr-xr-x   0 bitwiseman   (501) staff       (20)        0 2019-03-25 21:36:24.000000 jsbeautifier-1.9.1/jsbeautifier.egg-info/
--rw-r--r--   0 bitwiseman   (501) staff       (20)      340 2019-03-25 21:36:24.000000 jsbeautifier-1.9.1/jsbeautifier.egg-info/PKG-INFO
--rw-r--r--   0 bitwiseman   (501) staff       (20)     1481 2019-03-25 21:36:24.000000 jsbeautifier-1.9.1/jsbeautifier.egg-info/SOURCES.txt
--rw-r--r--   0 bitwiseman   (501) staff       (20)        1 2019-03-25 21:36:24.000000 jsbeautifier-1.9.1/jsbeautifier.egg-info/dependency_links.txt
--rw-r--r--   0 bitwiseman   (501) staff       (20)       51 2019-03-25 21:36:24.000000 jsbeautifier-1.9.1/jsbeautifier.egg-info/entry_points.txt
--rw-r--r--   0 bitwiseman   (501) staff       (20)       32 2019-03-25 21:36:24.000000 jsbeautifier-1.9.1/jsbeautifier.egg-info/requires.txt
--rw-r--r--   0 bitwiseman   (501) staff       (20)       13 2019-03-25 21:36:24.000000 jsbeautifier-1.9.1/jsbeautifier.egg-info/top_level.txt
--rw-r--r--   0 bitwiseman   (501) staff       (20)       38 2019-03-25 21:36:24.000000 jsbeautifier-1.9.1/setup.cfg
--rwxr-xr-x   0 bitwiseman   (501) staff       (20)     1632 2018-09-10 22:45:19.000000 jsbeautifier-1.9.1/setup.py
+drwxr-xr-x   0 lnewman    (501) staff       (20)        0 2015-06-25 19:34:13.000000 jsbeautifier-v1.5.8/
+-rwxr-xr-x   0 lnewman    (501) staff       (20)      118 2015-06-25 18:59:58.000000 jsbeautifier-v1.5.8/js-beautify
+-rwxr-xr-x   0 lnewman    (501) staff       (20)      153 2015-06-25 18:59:58.000000 jsbeautifier-v1.5.8/js-beautify-test
+drwxr-xr-x   0 lnewman    (501) staff       (20)        0 2015-06-25 19:34:13.000000 jsbeautifier-v1.5.8/jsbeautifier/
+-rw-r--r--   0 lnewman    (501) staff       (20)    83180 2015-06-25 18:59:58.000000 jsbeautifier-v1.5.8/jsbeautifier/__init__.py
+-rw-r--r--   0 lnewman    (501) staff       (20)       23 2015-06-25 19:34:08.000000 jsbeautifier-v1.5.8/jsbeautifier/__version__.py
+drwxr-xr-x   0 lnewman    (501) staff       (20)        0 2015-06-25 19:34:13.000000 jsbeautifier-v1.5.8/jsbeautifier/tests/
+-rw-r--r--   0 lnewman    (501) staff       (20)       16 2015-06-25 18:59:58.000000 jsbeautifier-v1.5.8/jsbeautifier/tests/__init__.py
+-rw-r--r--   0 lnewman    (501) staff       (20)     1126 2015-06-25 18:59:58.000000 jsbeautifier-v1.5.8/jsbeautifier/tests/test-perf-jsbeautifier.py
+-rw-r--r--   0 lnewman    (501) staff       (20)     1369 2015-06-25 18:59:58.000000 jsbeautifier-v1.5.8/jsbeautifier/tests/testindentation.py
+-rw-r--r--   0 lnewman    (501) staff       (20)   119070 2015-06-25 18:59:58.000000 jsbeautifier-v1.5.8/jsbeautifier/tests/testjsbeautifier.py
+drwxr-xr-x   0 lnewman    (501) staff       (20)        0 2015-06-25 19:34:13.000000 jsbeautifier-v1.5.8/jsbeautifier/unpackers/
+-rw-r--r--   0 lnewman    (501) staff       (20)     2316 2015-06-25 18:59:58.000000 jsbeautifier-v1.5.8/jsbeautifier/unpackers/__init__.py
+-rw-r--r--   0 lnewman    (501) staff       (20)     1171 2015-06-25 18:59:58.000000 jsbeautifier-v1.5.8/jsbeautifier/unpackers/evalbased.py
+-rw-r--r--   0 lnewman    (501) staff       (20)     1790 2015-06-25 18:59:58.000000 jsbeautifier-v1.5.8/jsbeautifier/unpackers/javascriptobfuscator.py
+-rw-r--r--   0 lnewman    (501) staff       (20)     2832 2015-06-25 18:59:58.000000 jsbeautifier-v1.5.8/jsbeautifier/unpackers/myobfuscate.py
+-rw-r--r--   0 lnewman    (501) staff       (20)     3594 2015-06-25 18:59:58.000000 jsbeautifier-v1.5.8/jsbeautifier/unpackers/packer.py
+drwxr-xr-x   0 lnewman    (501) staff       (20)        0 2015-06-25 19:34:13.000000 jsbeautifier-v1.5.8/jsbeautifier/unpackers/tests/
+-rw-r--r--   0 lnewman    (501) staff       (20)       40 2015-06-25 18:59:58.000000 jsbeautifier-v1.5.8/jsbeautifier/unpackers/tests/__init__.py
+-rw-r--r--   0 lnewman    (501) staff       (20)     1540 2015-06-25 18:59:58.000000 jsbeautifier-v1.5.8/jsbeautifier/unpackers/tests/testjavascriptobfuscator.py
+-rw-r--r--   0 lnewman    (501) staff       (20)     1163 2015-06-25 18:59:58.000000 jsbeautifier-v1.5.8/jsbeautifier/unpackers/tests/testmyobfuscate.py
+-rw-r--r--   0 lnewman    (501) staff       (20)     1177 2015-06-25 18:59:58.000000 jsbeautifier-v1.5.8/jsbeautifier/unpackers/tests/testpacker.py
+-rw-r--r--   0 lnewman    (501) staff       (20)      994 2015-06-25 18:59:58.000000 jsbeautifier-v1.5.8/jsbeautifier/unpackers/tests/testurlencode.py
+-rw-r--r--   0 lnewman    (501) staff       (20)      982 2015-06-25 18:59:58.000000 jsbeautifier-v1.5.8/jsbeautifier/unpackers/urlencode.py
+-rw-r--r--   0 lnewman    (501) staff       (20)      353 2015-06-25 19:34:13.000000 jsbeautifier-v1.5.8/PKG-INFO
+-rwxr-xr-x   0 lnewman    (501) staff       (20)      724 2015-06-25 18:59:58.000000 jsbeautifier-v1.5.8/setup.py
```

### Comparing `jsbeautifier-1.9.1/jsbeautifier/tests/testindentation.py` & `jsbeautifier-v1.5.8/jsbeautifier/tests/testindentation.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,28 @@
 import re
 import unittest
 import jsbeautifier
 
-
 class TestJSBeautifierIndentation(unittest.TestCase):
     def test_tabs(self):
         test_fragment = self.decodesto
 
-        self.options.indent_with_tabs = 1
-        test_fragment('{tabs()}', "{\n\ttabs()\n}")
+        self.options.indent_with_tabs = 1;
+        test_fragment('{tabs()}', "{\n\ttabs()\n}");
 
     def test_function_indent(self):
         test_fragment = self.decodesto
 
-        self.options.indent_with_tabs = 1
-        self.options.keep_function_indentation = 1
-        test_fragment(
-            'var foo = function(){ bar() }();',
-            "var foo = function() {\n\tbar()\n}();")
-
-        self.options.tabs = 1
-        self.options.keep_function_indentation = 0
-        test_fragment(
-            'var foo = function(){ baz() }();',
-            "var foo = function() {\n\tbaz()\n}();")
+        self.options.indent_with_tabs = 1;
+        self.options.keep_function_indentation = 1;
+        test_fragment('var foo = function(){ bar() }();', "var foo = function() {\n\tbar()\n}();");
+
+        self.options.tabs = 1;
+        self.options.keep_function_indentation = 0;
+        test_fragment('var foo = function(){ baz() }();', "var foo = function() {\n\tbaz()\n}();");
 
     def decodesto(self, input, expectation=None):
         self.assertEqual(
             jsbeautifier.beautify(input, self.options), expectation or input)
 
     @classmethod
     def setUpClass(cls):
```

### Comparing `jsbeautifier-1.9.1/jsbeautifier/unpackers/__init__.py` & `jsbeautifier-v1.5.8/jsbeautifier/unpackers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,21 +8,19 @@
 import pkgutil
 import re
 from jsbeautifier.unpackers import evalbased
 
 # NOTE: AT THE MOMENT, IT IS DEACTIVATED FOR YOUR SECURITY: it runs js!
 BLACKLIST = ['jsbeautifier.unpackers.evalbased']
 
-
 class UnpackingError(Exception):
     """Badly packed source or general error. Argument is a
     meaningful description."""
     pass
 
-
 def getunpackers():
     """Scans the unpackers dir, finds unpackers and add them to UNPACKERS list.
     An unpacker will be loaded only if it is a valid python module (name must
     adhere to naming conventions) and it is not blacklisted (i.e. inserted
     into BLACKLIST."""
     path = __path__
     prefix = __name__ + '.'
@@ -33,29 +31,26 @@
             try:
                 module = __import__(modname, fromlist=interface)
             except ImportError:
                 raise UnpackingError('Bad unpacker: %s' % modname)
             else:
                 unpackers.append(module)
 
-    return sorted(unpackers, key=lambda mod: mod.PRIORITY)
-
+    return sorted(unpackers, key = lambda mod: mod.PRIORITY)
 
 UNPACKERS = getunpackers()
 
-
 def run(source, evalcode=False):
     """Runs the applicable unpackers and return unpacked source as a string."""
     for unpacker in [mod for mod in UNPACKERS if mod.detect(source)]:
         source = unpacker.unpack(source)
     if evalcode and evalbased.detect(source):
         source = evalbased.unpack(source)
     return source
 
-
 def filtercomments(source):
     """NOT USED: strips trailing comments and put them at the top."""
     trailing_comments = []
     comment = True
 
     while comment:
         if re.search(r'^\s*\/\*', source):
```

### Comparing `jsbeautifier-1.9.1/jsbeautifier/unpackers/evalbased.py` & `jsbeautifier-v1.5.8/jsbeautifier/unpackers/evalbased.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #
 # Unpacker for eval() based packers, a part of javascript beautifier
-# by Einar Lielmanis <einar@beautifier.io>
+# by Einar Lielmanis <einar@jsbeautifier.org>
 #
 #     written by Stefano Sanfilippo <a.little.coder@gmail.com>
 #
 # usage:
 #
 # if detect(some_string):
 #     unpacked = unpack(some_string)
@@ -14,27 +14,23 @@
 Works only if a JS interpreter (e.g. Mozilla's Rhino) is installed and
 properly set up on host."""
 
 from subprocess import PIPE, Popen
 
 PRIORITY = 3
 
-
 def detect(source):
     """Detects if source is likely to be eval() packed."""
     return source.strip().lower().startswith('eval(function(')
 
-
 def unpack(source):
     """Runs source and return resulting code."""
     return jseval('print %s;' % source[4:]) if detect(source) else source
 
 # In case of failure, we'll just return the original, without crashing on user.
-
-
 def jseval(script):
     """Run code in the JS interpreter and return output."""
     try:
         interpreter = Popen(['js'], stdin=PIPE, stdout=PIPE)
     except OSError:
         return script
     result, errors = interpreter.communicate(script)
```

### Comparing `jsbeautifier-1.9.1/jsbeautifier/unpackers/javascriptobfuscator.py` & `jsbeautifier-v1.5.8/jsbeautifier/unpackers/javascriptobfuscator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
 # simple unpacker/deobfuscator for scripts messed up with
 # javascriptobfuscator.com
 #
-#     written by Einar Lielmanis <einar@beautifier.io>
+#     written by Einar Lielmanis <einar@jsbeautifier.org>
 #     rewritten in Python by Stefano Sanfilippo <a.little.coder@gmail.com>
 #
 # Will always return valid javascript: if `detect()` is false, `code` is
 # returned, unmodified.
 #
 # usage:
 #
@@ -16,42 +16,39 @@
 
 """deobfuscator for scripts messed up with JavascriptObfuscator.com"""
 
 import re
 
 PRIORITY = 1
 
-
 def smartsplit(code):
     """Split `code` at " symbol, only if it is not escaped."""
     strings = []
     pos = 0
     while pos < len(code):
         if code[pos] == '"':
-            word = ''  # new word
+            word = '' # new word
             pos += 1
             while pos < len(code):
                 if code[pos] == '"':
                     break
                 if code[pos] == '\\':
                     word += '\\'
                     pos += 1
                 word += code[pos]
                 pos += 1
             strings.append('"%s"' % word)
         pos += 1
     return strings
 
-
 def detect(code):
     """Detects if `code` is JavascriptObfuscator.com packed."""
     # prefer `is not` idiom, so that a true boolean is returned
     return (re.search(r'^var _0x[a-f0-9]+ ?\= ?\[', code) is not None)
 
-
 def unpack(code):
     """Unpacks JavascriptObfuscator.com packed code."""
     if detect(code):
         matches = re.search(r'var (_0x[a-f\d]+) ?\= ?\[(.*?)\];', code)
         if matches:
             variable = matches.group(1)
             dictionary = smartsplit(matches.group(2))
```

### Comparing `jsbeautifier-1.9.1/jsbeautifier/unpackers/myobfuscate.py` & `jsbeautifier-v1.5.8/jsbeautifier/unpackers/myobfuscate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #
 # deobfuscator for scripts messed up with myobfuscate.com
-# by Einar Lielmanis <einar@beautifier.io>
+# by Einar Lielmanis <einar@jsbeautifier.org>
 #
 #     written by Stefano Sanfilippo <a.little.coder@gmail.com>
 #
 # usage:
 #
 # if detect(some_string):
 #     unpacked = unpack(some_string)
@@ -47,40 +47,36 @@
 CAVEAT = """//
 // Unpacker warning: be careful when using myobfuscate.com for your projects:
 // scripts obfuscated by the free online version call back home.
 //
 
 """
 
-SIGNATURE = (
-    r'["\x41\x42\x43\x44\x45\x46\x47\x48\x49\x4A\x4B\x4C\x4D\x4E\x4F'
-    r'\x50\x51\x52\x53\x54\x55\x56\x57\x58\x59\x5A\x61\x62\x63\x64\x65'
-    r'\x66\x67\x68\x69\x6A\x6B\x6C\x6D\x6E\x6F\x70\x71\x72\x73\x74\x75'
-    r'\x76\x77\x78\x79\x7A\x30\x31\x32\x33\x34\x35\x36\x37\x38\x39\x2B'
-    r'\x2F\x3D","","\x63\x68\x61\x72\x41\x74","\x69\x6E\x64\x65\x78'
-    r'\x4F\x66","\x66\x72\x6F\x6D\x43\x68\x61\x72\x43\x6F\x64\x65","'
-    r'\x6C\x65\x6E\x67\x74\x68"]')
-
+SIGNATURE = (r'["\x41\x42\x43\x44\x45\x46\x47\x48\x49\x4A\x4B\x4C\x4D\x4E\x4F'
+             r'\x50\x51\x52\x53\x54\x55\x56\x57\x58\x59\x5A\x61\x62\x63\x64\x65'
+             r'\x66\x67\x68\x69\x6A\x6B\x6C\x6D\x6E\x6F\x70\x71\x72\x73\x74\x75'
+             r'\x76\x77\x78\x79\x7A\x30\x31\x32\x33\x34\x35\x36\x37\x38\x39\x2B'
+             r'\x2F\x3D","","\x63\x68\x61\x72\x41\x74","\x69\x6E\x64\x65\x78'
+             r'\x4F\x66","\x66\x72\x6F\x6D\x43\x68\x61\x72\x43\x6F\x64\x65","'
+             r'\x6C\x65\x6E\x67\x74\x68"]')
 
 def detect(source):
     """Detects MyObfuscate.com packer."""
     return SIGNATURE in source
 
-
 def unpack(source):
     """Unpacks js code packed with MyObfuscate.com"""
     if not detect(source):
         return source
     payload = unquote(_filter(source))
     match = re.search(r"^var _escape\='<script>(.*)<\/script>'",
                       payload, re.DOTALL)
     polished = match.group(1) if match else source
     return CAVEAT + polished
 
-
 def _filter(source):
     """Extracts and decode payload (original file) from `source`"""
     try:
         varname = re.search(r'eval\(\w+\(\w+\((\w+)\)\)\);', source).group(1)
         reverse = re.search(r"var +%s *\= *'(.*)';" % varname, source).group(1)
     except AttributeError:
         raise UnpackingError('Malformed MyObfuscate data.')
```

### Comparing `jsbeautifier-1.9.1/jsbeautifier/unpackers/packer.py` & `jsbeautifier-v1.5.8/jsbeautifier/unpackers/packer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #
 # Unpacker for Dean Edward's p.a.c.k.e.r, a part of javascript beautifier
-# by Einar Lielmanis <einar@beautifier.io>
+# by Einar Lielmanis <einar@jsbeautifier.org>
 #
 #     written by Stefano Sanfilippo <a.little.coder@gmail.com>
 #
 # usage:
 #
 # if detect(some_string):
 #     unpacked = unpack(some_string)
@@ -14,39 +14,17 @@
 
 import re
 import string
 from jsbeautifier.unpackers import UnpackingError
 
 PRIORITY = 1
 
-
 def detect(source):
-    global beginstr
-    global endstr
-    beginstr = ''
-    endstr = ''
-    begin_offset = -1
     """Detects whether `source` is P.A.C.K.E.R. coded."""
-    mystr = re.search('eval[ ]*\([ ]*function[ ]*\([ ]*p[ ]*,[ ]*a[ ]*,[ ]*c['
-                      ' ]*,[ ]*k[ ]*,[ ]*e[ ]*,[ ]*', source)
-    if(mystr):
-        begin_offset = mystr.start()
-        beginstr = source[:begin_offset]
-    if(begin_offset != -1):
-        """ Find endstr"""
-        source_end = source[begin_offset:]
-        if(source_end.split("')))", 1)[0] == source_end):
-            try:
-                endstr = source_end.split("}))", 1)[1]
-            except IndexError:
-                endstr = ''
-        else:
-            endstr = source_end.split("')))", 1)[1]
-    return (mystr is not None)
-
+    return source.replace(' ', '').startswith('eval(function(p,a,c,k,e,')
 
 def unpack(source):
     """Unpacks P.A.C.K.E.R. packed js code."""
     payload, symtab, radix, count = _filterargs(source)
 
     if count != len(symtab):
         raise UnpackingError('Malformed p.a.c.k.e.r. symtab.')
@@ -54,89 +32,74 @@
     try:
         unbase = Unbaser(radix)
     except TypeError:
         raise UnpackingError('Unknown p.a.c.k.e.r. encoding.')
 
     def lookup(match):
         """Look up symbols in the synthetic symtab."""
-        word = match.group(0)
+        word  = match.group(0)
         return symtab[unbase(word)] or word
 
     source = re.sub(r'\b\w+\b', lookup, payload)
     return _replacestrings(source)
 
-
 def _filterargs(source):
     """Juice from a source file the four args needed by decoder."""
-    juicers = [
-        (r"}\('(.*)', *(\d+|\[\]), *(\d+), *'(.*)'\.split\('\|'\), *(\d+), *(.*)\)\)"),
-        (r"}\('(.*)', *(\d+|\[\]), *(\d+), *'(.*)'\.split\('\|'\)"),
-    ]
+    juicers = [ (r"}\('(.*)', *(\d+), *(\d+), *'(.*)'\.split\('\|'\), *(\d+), *(.*)\)\)"),
+                (r"}\('(.*)', *(\d+), *(\d+), *'(.*)'\.split\('\|'\)"),
+              ]
     for juicer in juicers:
         args = re.search(juicer, source, re.DOTALL)
         if args:
             a = args.groups()
-            if a[1] == "[]":
-                a = list(a)
-                a[1] = 62
-                a = tuple(a)
             try:
                 return a[0], a[3].split('|'), int(a[1]), int(a[2])
             except ValueError:
                 raise UnpackingError('Corrupted p.a.c.k.e.r. data.')
 
     # could not find a satisfying regex
-    raise UnpackingError(
-        'Could not make sense of p.a.c.k.e.r data (unexpected code structure)')
+    raise UnpackingError('Could not make sense of p.a.c.k.e.r data (unexpected code structure)')
+
 
 
 def _replacestrings(source):
-    global beginstr
-    global endstr
     """Strip string lookup table (list) and replace values in source."""
     match = re.search(r'var *(_\w+)\=\["(.*?)"\];', source, re.DOTALL)
 
     if match:
         varname, strings = match.groups()
         startpoint = len(match.group(0))
         lookup = strings.split('","')
         variable = '%s[%%d]' % varname
         for index, value in enumerate(lookup):
             source = source.replace(variable % index, '"%s"' % value)
         return source[startpoint:]
-    return beginstr + source + endstr
+    return source
 
 
 class Unbaser(object):
     """Functor for a given base. Will efficiently convert
     strings to natural numbers."""
-    ALPHABET = {
-        62: '0123456789abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ',
-        95: (' !"#$%&\'()*+,-./0123456789:;<=>?@ABCDEFGHIJKLMNOPQRSTUVWXYZ'
-             '[\\]^_`abcdefghijklmnopqrstuvwxyz{|}~')
+    ALPHABET  = {
+        62 : '0123456789abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ',
+        95 : (' !"#$%&\'()*+,-./0123456789:;<=>?@ABCDEFGHIJKLMNOPQRSTUVWXYZ'
+              '[\]^_`abcdefghijklmnopqrstuvwxyz{|}~')
     }
 
     def __init__(self, base):
         self.base = base
 
-        # fill elements 37...61, if necessary
-        if 36 < base < 62:
-            if not hasattr(self.ALPHABET, self.ALPHABET[62][:base]):
-                self.ALPHABET[base] = self.ALPHABET[62][:base]
-        # attrs = self.ALPHABET
-        # print ', '.join("%s: %s" % item for item in attrs.items())
         # If base can be handled by int() builtin, let it do it for us
         if 2 <= base <= 36:
             self.unbase = lambda string: int(string, base)
         else:
             # Build conversion dictionary cache
             try:
-                self.dictionary = dict(
-                    (cipher, index) for index, cipher in enumerate(
-                        self.ALPHABET[base]))
+                self.dictionary = dict((cipher, index) for
+                    index, cipher in enumerate(self.ALPHABET[base]))
             except KeyError:
                 raise TypeError('Unsupported base encoding.')
 
             self.unbase = self._dictunbaser
 
     def __call__(self, string):
         return self.unbase(string)
```

### Comparing `jsbeautifier-1.9.1/jsbeautifier/unpackers/tests/testmyobfuscate.py` & `jsbeautifier-v1.5.8/jsbeautifier/unpackers/tests/testmyobfuscate.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,35 +9,32 @@
 from jsbeautifier.unpackers.myobfuscate import detect, unpack
 from jsbeautifier.unpackers.tests import __path__ as path
 
 INPUT = os.path.join(path[0], 'test-myobfuscate-input.js')
 OUTPUT = os.path.join(path[0], 'test-myobfuscate-output.js')
 
 # pylint: disable=R0904
-
-
 class TestMyObfuscate(unittest.TestCase):
     # pylint: disable=C0103
     """MyObfuscate obfuscator testcase."""
     @classmethod
     def setUpClass(cls):
         """Load source files (encoded and decoded version) for tests."""
         with open(INPUT, 'r') as data:
             cls.input = data.read()
         with open(OUTPUT, 'r') as data:
             cls.output = data.read()
 
     def test_detect(self):
         """Test detect() function."""
-        def detected(source): return self.assertTrue(detect(source))
+        detected = lambda source: self.assertTrue(detect(source))
 
         detected(self.input)
 
     def test_unpack(self):
         """Test unpack() function."""
-        def check(inp, out): return self.assertEqual(unpack(inp), out)
+        check = lambda inp, out: self.assertEqual(unpack(inp), out)
 
         check(self.input, self.output)
 
-
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `jsbeautifier-1.9.1/jsbeautifier/unpackers/tests/testpacker.py` & `jsbeautifier-v1.5.8/jsbeautifier/unpackers/tests/testpacker.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,44 +4,31 @@
 
 """Tests for P.A.C.K.E.R. unpacker."""
 
 import unittest
 from jsbeautifier.unpackers.packer import detect, unpack
 
 # pylint: disable=R0904
-
-
 class TestPacker(unittest.TestCase):
     """P.A.C.K.E.R. testcase."""
-
     def test_detect(self):
         """Test detect() function."""
-        def positive(source): return self.assertTrue(detect(source))
-
-        def negative(source): return self.assertFalse(detect(source))
+        positive = lambda source: self.assertTrue(detect(source))
+        negative = lambda source: self.assertFalse(detect(source))
 
         negative('')
         negative('var a = b')
         positive('eval(function(p,a,c,k,e,r')
         positive('eval ( function(p, a, c, k, e, r')
 
     def test_unpack(self):
         """Test unpack() function."""
-        def check(inp, out):
-            return detect(inp) and self.assertEqual(unpack(inp), out)
+        check = lambda inp, out: self.assertEqual(unpack(inp), out)
 
         check("eval(function(p,a,c,k,e,r){e=String;if(!''.replace(/^/,String)"
               "){while(c--)r[c]=k[c]||c;k=[function(e){return r[e]}];e="
               "function(){return'\\\\w+'};c=1};while(c--)if(k[c])p=p.replace("
               "new RegExp('\\\\b'+e(c)+'\\\\b','g'),k[c]);return p}('0 2=1',"
               "62,3,'var||a'.split('|'),0,{}))", 'var a=1')
-        check("function test (){alert ('This is a test!')}; "
-              "eval(function(p,a,c,k,e,r){e=String;if(!''.replace(/^/,String))"
-              "{while(c--)r[c]=k[c]||c;k=[function(e){return r[e]}];e=function"
-              "(){return'\\w+'};c=1};while(c--)if(k[c])p=p.replace(new RegExp("
-              "'\\b'+e(c)+'\\b','g'),k[c]);return p}('0 2=1',3,3,"
-              "'var||a'.split('|'),0,{}))",
-              "function test (){alert ('This is a test!')}; var a=1")
-
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `jsbeautifier-1.9.1/jsbeautifier/unpackers/tests/testurlencode.py` & `jsbeautifier-v1.5.8/jsbeautifier/unpackers/tests/testurlencode.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,41 +5,32 @@
 """Tests for urlencoded unpacker."""
 
 import unittest
 
 from jsbeautifier.unpackers.urlencode import detect, unpack
 
 # pylint: disable=R0904
-
-
 class TestUrlencode(unittest.TestCase):
     """urlencode test case."""
-
     def test_detect(self):
         """Test detect() function."""
-        def encoded(source): return self.assertTrue(detect(source))
-
-        def unencoded(source): return self.assertFalse(detect(source))
+        encoded = lambda source: self.assertTrue(detect(source))
+        unencoded = lambda source: self.assertFalse(detect(source))
 
         unencoded('')
         unencoded('var a = b')
         encoded('var%20a+=+b')
         encoded('var%20a=b')
         encoded('var%20%21%22')
 
     def test_unpack(self):
         """Test unpack function."""
-        def equals(
-            source,
-            result): return self.assertEqual(
-            unpack(source),
-            result)
+        equals = lambda source, result: self.assertEqual(unpack(source), result)
 
         equals('', '')
         equals('abcd', 'abcd')
         equals('var a = b', 'var a = b')
         equals('var%20a=b', 'var a=b')
         equals('var%20a+=+b', 'var a = b')
 
-
 if __name__ == '__main__':
     unittest.main()
```

