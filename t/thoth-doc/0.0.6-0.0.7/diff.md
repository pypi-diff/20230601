# Comparing `tmp/thoth_doc-0.0.6.tar.gz` & `tmp/thoth_doc-0.0.7.tar.gz`

## Comparing `thoth_doc-0.0.6.tar` & `thoth_doc-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    28955 2020-02-02 00:00:00.000000 thoth_doc-0.0.6/Thoth.svg.png
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 thoth_doc-0.0.6/vscode.env
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 thoth_doc-0.0.6/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 thoth_doc-0.0.6/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 thoth_doc-0.0.6/.pytest_cache/README.md
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 thoth_doc-0.0.6/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 thoth_doc-0.0.6/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 thoth_doc-0.0.6/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 thoth_doc-0.0.6/.vscode/settings.json
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 thoth_doc-0.0.6/src/thoth_doc/__init__.py
--rw-r--r--   0        0        0     3971 2020-02-02 00:00:00.000000 thoth_doc-0.0.6/src/thoth_doc/main.py
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 thoth_doc-0.0.6/src/thoth_doc/parsers.py
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 thoth_doc-0.0.6/src/thoth_doc/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 thoth_doc-0.0.6/tests/__init__.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 thoth_doc-0.0.6/tests/test_parsers.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 thoth_doc-0.0.6/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 thoth_doc-0.0.6/LICENSE
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 thoth_doc-0.0.6/README.md
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 thoth_doc-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 thoth_doc-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0    28955 2020-02-02 00:00:00.000000 thoth_doc-0.0.7/Thoth.svg.png
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 thoth_doc-0.0.7/vscode.env
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 thoth_doc-0.0.7/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 thoth_doc-0.0.7/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 thoth_doc-0.0.7/.pytest_cache/README.md
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 thoth_doc-0.0.7/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 thoth_doc-0.0.7/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 thoth_doc-0.0.7/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 thoth_doc-0.0.7/.vscode/settings.json
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 thoth_doc-0.0.7/src/thoth_doc/__init__.py
+-rw-r--r--   0        0        0     4283 2020-02-02 00:00:00.000000 thoth_doc-0.0.7/src/thoth_doc/main.py
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 thoth_doc-0.0.7/src/thoth_doc/parsers.py
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 thoth_doc-0.0.7/src/thoth_doc/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 thoth_doc-0.0.7/tests/__init__.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 thoth_doc-0.0.7/tests/test_parsers.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 thoth_doc-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 thoth_doc-0.0.7/LICENSE
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 thoth_doc-0.0.7/README.md
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 thoth_doc-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 thoth_doc-0.0.7/PKG-INFO
```

### Comparing `thoth_doc-0.0.6/Thoth.svg.png` & `thoth_doc-0.0.7/Thoth.svg.png`

 * *Files identical despite different names*

### Comparing `thoth_doc-0.0.6/src/thoth_doc/main.py` & `thoth_doc-0.0.7/src/thoth_doc/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,16 +15,27 @@
         cwd = os.getcwd()
         if path and path.startswith('/'):
             path = path[1:]
         return f'{cwd}/{self.compiled_docs_folder}/{path}' if path else f'{cwd}/{self.compiled_docs_folder}'
 
     def _compile_lines(self, markdown_lines):
         compiled_markdown = ''
+        skip = False
 
         for line in markdown_lines:
+            if line.startswith('[ignore]'):
+                skip = True
+                continue
+            elif line.startswith('[endignore]'):
+                skip = False
+                continue
+            elif skip:
+                compiled_markdown += line
+                continue
+
             for parser in self.parsers + self._default_parsers:
                 parsed = parser(line)
                 if parsed is not None:
                     compiled_markdown += parsed
                     break
             if parsed is None:
                 compiled_markdown += line
```

### Comparing `thoth_doc-0.0.6/src/thoth_doc/parsers.py` & `thoth_doc-0.0.7/src/thoth_doc/parsers.py`

 * *Files identical despite different names*

### Comparing `thoth_doc-0.0.6/src/thoth_doc/utils.py` & `thoth_doc-0.0.7/src/thoth_doc/utils.py`

 * *Files identical despite different names*

### Comparing `thoth_doc-0.0.6/tests/test_parsers.py` & `thoth_doc-0.0.7/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `thoth_doc-0.0.6/LICENSE` & `thoth_doc-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `thoth_doc-0.0.6/README.md` & `thoth_doc-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `thoth_doc-0.0.6/pyproject.toml` & `thoth_doc-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "thoth_doc"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Lev", email="smj510black@gmail.com" },
 ]
 description = "Dependency-free, lightweight docstring parser"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `thoth_doc-0.0.6/PKG-INFO` & `thoth_doc-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thoth_doc
-Version: 0.0.6
+Version: 0.0.7
 Summary: Dependency-free, lightweight docstring parser
 Project-URL: Homepage, https://github.com/mariownyou/thoth-doc
 Project-URL: Bug Tracker, https://github.com/mariownyou/thoth-doc/issues
 Author-email: Lev <smj510black@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

