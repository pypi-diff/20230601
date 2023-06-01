# Comparing `tmp/atsphinx-footnotes-0.1.1.tar.gz` & `tmp/atsphinx_footnotes-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atsphinx-footnotes-0.1.1.tar", last modified: Thu May  4 18:46:23 2023, max compression
+gzip compressed data, was "atsphinx_footnotes-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `atsphinx-footnotes-0.1.1.tar` & `atsphinx_footnotes-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0      560 2023-05-04 18:46:18.388256 atsphinx-footnotes-0.1.1/.editorconfig
--rw-r--r--   0        0        0     3338 2023-05-04 18:46:18.388256 atsphinx-footnotes-0.1.1/.gitignore
--rw-r--r--   0        0        0      543 2023-05-04 18:46:18.388256 atsphinx-footnotes-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      286 2023-05-04 18:46:18.388256 atsphinx-footnotes-0.1.1/CHANGES.rst
--rw-r--r--   0        0        0     9161 2023-05-04 18:46:18.388256 atsphinx-footnotes-0.1.1/LICENSE
--rw-r--r--   0        0        0      907 2023-05-04 18:46:18.388256 atsphinx-footnotes-0.1.1/README.rst
--rw-r--r--   0        0        0      634 2023-05-04 18:46:18.388256 atsphinx-footnotes-0.1.1/docs/Makefile
--rw-r--r--   0        0        0      517 2023-05-04 18:46:18.388256 atsphinx-footnotes-0.1.1/docs/conf.py
--rw-r--r--   0        0        0     1103 2023-05-04 18:46:18.388256 atsphinx-footnotes-0.1.1/docs/index.rst
--rw-r--r--   0        0        0      800 2023-05-04 18:46:18.388256 atsphinx-footnotes-0.1.1/docs/make.bat
--rw-r--r--   0        0        0      998 2023-05-04 18:46:18.388256 atsphinx-footnotes-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      354 2023-05-04 18:46:18.388256 atsphinx-footnotes-0.1.1/setup.cfg
--rw-r--r--   0        0        0      777 2023-05-04 18:46:18.388256 atsphinx-footnotes-0.1.1/src/atsphinx/footnotes.py
--rw-r--r--   0        0        0     1775 1970-01-01 00:00:00.000000 atsphinx-footnotes-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      517 2023-06-01 14:46:21.996898 atsphinx_footnotes-0.2.0/.editorconfig
+-rw-r--r--   0        0        0     3338 2023-06-01 14:46:21.996898 atsphinx_footnotes-0.2.0/.gitignore
+-rw-r--r--   0        0        0      543 2023-06-01 14:46:21.996898 atsphinx_footnotes-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      459 2023-06-01 14:46:21.996898 atsphinx_footnotes-0.2.0/CHANGES.rst
+-rw-r--r--   0        0        0     9161 2023-06-01 14:46:21.996898 atsphinx_footnotes-0.2.0/LICENSE
+-rw-r--r--   0        0        0      907 2023-06-01 14:46:21.996898 atsphinx_footnotes-0.2.0/README.rst
+-rw-r--r--   0        0        0      634 2023-06-01 14:46:22.000898 atsphinx_footnotes-0.2.0/docs/Makefile
+-rw-r--r--   0        0        0       14 2023-06-01 14:46:22.000898 atsphinx_footnotes-0.2.0/docs/_static/.gitignore
+-rw-r--r--   0        0        0       14 2023-06-01 14:46:22.000898 atsphinx_footnotes-0.2.0/docs/_templates/.gitignore
+-rw-r--r--   0        0        0      712 2023-06-01 14:46:22.000898 atsphinx_footnotes-0.2.0/docs/conf.py
+-rw-r--r--   0        0        0     1006 2023-06-01 14:46:22.000898 atsphinx_footnotes-0.2.0/docs/index.rst
+-rw-r--r--   0        0        0      800 2023-06-01 14:46:22.000898 atsphinx_footnotes-0.2.0/docs/make.bat
+-rw-r--r--   0        0        0     1007 2023-06-01 14:46:22.000898 atsphinx_footnotes-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      354 2023-06-01 14:46:22.000898 atsphinx_footnotes-0.2.0/setup.cfg
+-rw-r--r--   0        0        0      985 2023-06-01 14:46:22.000898 atsphinx_footnotes-0.2.0/src/atsphinx/footnotes.py
+-rw-r--r--   0        0        0     1795 1970-01-01 00:00:00.000000 atsphinx_footnotes-0.2.0/PKG-INFO
```

### Comparing `atsphinx-footnotes-0.1.1/.editorconfig` & `atsphinx_footnotes-0.2.0/.editorconfig`

 * *Files 15% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 charset = utf-8
 end_of_line = lf
 indent_style = space
 insert_final_newline = true
 trim_trailing_whitespace = false
 
 # Windows files
-[*.{vbs,bat}]
+[*.{bat}]
 indent_style = space
 indent_size = 4
 end_of_line = crlf
 charset = sjis
 
 # 2 space indentation
-[*.{yml,js,jsx,ts,tsx,json,rst,html,css,nim,nims,nimble,nimf,md,toml}]
+[*.{yml,js,json,rst,html,css,md,toml}]
 indent_size = 2
 
 # 4 space indentation
-[*.{py,php}]
+[*.{py}]
 indent_size = 4
 
 # Tab indentation (no size specified)
-[Makefile,*.{go,cfg}]
+[Makefile,*.{cfg}]
 indent_style = tab
```

### Comparing `atsphinx-footnotes-0.1.1/.gitignore` & `atsphinx_footnotes-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `atsphinx-footnotes-0.1.1/.pre-commit-config.yaml` & `atsphinx_footnotes-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `atsphinx-footnotes-0.1.1/LICENSE` & `atsphinx_footnotes-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `atsphinx-footnotes-0.1.1/README.rst` & `atsphinx_footnotes-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `atsphinx-footnotes-0.1.1/docs/Makefile` & `atsphinx_footnotes-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `atsphinx-footnotes-0.1.1/docs/make.bat` & `atsphinx_footnotes-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `atsphinx-footnotes-0.1.1/pyproject.toml` & `atsphinx_footnotes-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -17,19 +17,20 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Topic :: Documentation :: Sphinx",
 ]
 readme = "README.rst"
 dependencies = [
-  "Sphinx",
+  "sphinx",
 ]
 dynamic = ["version", "description"]
 
 [project.optional-dependencies]
+doc = []
 test = [
   "pytest ==7.*",
 ]
 
 [project.urls]
 Home = "https://github.com/atsphinx/footnotes"
```

### Comparing `atsphinx-footnotes-0.1.1/src/atsphinx/footnotes.py` & `atsphinx_footnotes-0.2.0/src/atsphinx/footnotes.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 """Powered footnotes extension for Sphinx."""
 from docutils import nodes
 from sphinx.application import Sphinx
+from sphinx.locale import _
 
-__version__ = "0.1.1"
+__version__ = "0.2.0"
 
 
 def collect_footnotes(app: Sphinx, doctree: nodes.document):
     """Collect and display later all footnotes."""
     footnotes = nodes.section()
+    rubric = getattr(app.config, "footnotes_rubric", None)
+    if rubric is None:
+        rubric = _("Footnotes")
     for footnote in doctree.traverse(nodes.footnote):
         footnote.parent.remove(footnote)
         footnotes.append(footnote)
     if len(footnotes.children):
-        footnotes.insert(0, nodes.rubric(text="Footnotes"))
+        footnotes.insert(0, nodes.rubric(text=rubric))
         doctree.append(footnotes)
 
 
 def setup(app: Sphinx):  # noqa: D103
+    app.add_config_value("footnotes_rubric", None, "env", [str, None])
     app.connect("doctree-read", collect_footnotes)
     return {
         "version": __version__,
         "env_version": 1,
         "parallel_read_safe": True,
         "parallel_write_safe": True,
     }
```

### Comparing `atsphinx-footnotes-0.1.1/PKG-INFO` & `atsphinx_footnotes-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: atsphinx-footnotes
-Version: 0.1.1
+Version: 0.2.0
 Summary: Powered footnotes extension for Sphinx.
 Author-email: Kazuya Takei <myself@attakei.net>
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Sphinx
 Classifier: Framework :: Sphinx :: Extension
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Documentation :: Sphinx
-Requires-Dist: Sphinx
+Requires-Dist: sphinx
 Requires-Dist: pytest ==7.* ; extra == "test"
 Project-URL: Home, https://github.com/atsphinx/footnotes
+Provides-Extra: doc
 Provides-Extra: test
 
 ==================
 atsphinx-footnotes
 ==================
 
 Powered footnote tools for Sphinx.
```

