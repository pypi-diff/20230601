# Comparing `tmp/code_qa-0.1.0.tar.gz` & `tmp/code_qa-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "code_qa-0.1.0.tar", max compression
+gzip compressed data, was "code_qa-0.2.0.tar", max compression
```

## Comparing `code_qa-0.1.0.tar` & `code_qa-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11356 2023-06-01 11:29:07.858435 code_qa-0.1.0/LICENSE
--rw-r--r--   0        0        0      831 2023-06-01 13:34:06.116070 code_qa-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-01 11:28:22.025812 code_qa-0.1.0/code_qa/__init__.py
--rw-r--r--   0        0        0     1881 2023-06-01 13:30:54.044136 code_qa-0.1.0/code_qa/cli.py
--rw-r--r--   0        0        0      167 2023-06-01 11:57:41.557031 code_qa-0.1.0/code_qa/logger.py
--rw-r--r--   0        0        0     1125 2023-06-01 13:16:43.458823 code_qa-0.1.0/code_qa/utils.py
--rw-r--r--   0        0        0      484 2023-06-01 12:17:21.525216 code_qa-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1712 1970-01-01 00:00:00.000000 code_qa-0.1.0/setup.py
--rw-r--r--   0        0        0     1473 1970-01-01 00:00:00.000000 code_qa-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-06-01 11:29:07.858435 code_qa-0.2.0/LICENSE
+-rw-r--r--   0        0        0      830 2023-06-01 13:56:57.750398 code_qa-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-01 11:28:22.025812 code_qa-0.2.0/code_qa/__init__.py
+-rw-r--r--   0        0        0     1881 2023-06-01 13:30:54.044136 code_qa-0.2.0/code_qa/cli.py
+-rw-r--r--   0        0        0      167 2023-06-01 11:57:41.557031 code_qa-0.2.0/code_qa/logger.py
+-rw-r--r--   0        0        0     1149 2023-06-01 13:56:57.755987 code_qa-0.2.0/code_qa/utils.py
+-rw-r--r--   0        0        0      484 2023-06-01 13:57:02.643554 code_qa-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1711 1970-01-01 00:00:00.000000 code_qa-0.2.0/setup.py
+-rw-r--r--   0        0        0     1472 1970-01-01 00:00:00.000000 code_qa-0.2.0/PKG-INFO
```

### Comparing `code_qa-0.1.0/LICENSE` & `code_qa-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `code_qa-0.1.0/README.md` & `code_qa-0.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 ```
 code_qa init
 ```
 
 Ask questions about my code:
 
 ```
-code_qa query How can I test this?
+code_qa query How can I test this
 ```
 
 ## Ignoring Files
 
 If you want to ignore certain files, then create an `.codeqaignore` file and specify them. The file follows the same
 standard as `.gitignore`
```

### Comparing `code_qa-0.1.0/code_qa/cli.py` & `code_qa-0.2.0/code_qa/cli.py`

 * *Files identical despite different names*

### Comparing `code_qa-0.1.0/code_qa/utils.py` & `code_qa-0.2.0/code_qa/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import os
 
 import pathspec
 from langchain.document_loaders import TextLoader
 
 
 def load_files(root_path):
-    ignore_path = os.path.join(root_path, '.codeqaignore')
-    ignore = None
-    if os.path.exists(ignore_path):
-        with open(ignore_path) as f:
-            ignore = f.read()
-
-    spec = pathspec.PathSpec.from_lines('gitwildmatch', ignore.splitlines())
-
     # Get all files in current directory
     all_files = []
     for dirpath, dirnames, filenames in os.walk('.'):
         for filename in filenames:
             all_files.append(os.path.join(dirpath, filename))
 
-    # Filter files based on .gitignore patterns
-    files_to_load = [f for f in all_files if not spec.match_file(f)]
+    files_to_load = all_files
+    ignore_path = os.path.join(root_path, '.codeqaignore')
+    if os.path.exists(ignore_path):
+        with open(ignore_path) as f:
+            ignore = f.read()
+
+        spec = pathspec.PathSpec.from_lines('gitwildmatch', ignore.splitlines())
+
+        # Filter files based on .gitignore patterns
+        files_to_load = [f for f in all_files if not spec.match_file(f)]
 
     docs = []
     for file in files_to_load:
         try:
             print(file)
             loader = TextLoader(os.path.join(file), encoding='utf-8')
             docs.extend(loader.load_and_split())
```

### Comparing `code_qa-0.1.0/setup.py` & `code_qa-0.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,17 +16,17 @@
  'tiktoken>=0.4.0,<0.5.0']
 
 entry_points = \
 {'console_scripts': ['code_qa = code_qa.cli:main']}
 
 setup_kwargs = {
     'name': 'code-qa',
-    'version': '0.1.0',
+    'version': '0.2.0',
     'description': '',
-    'long_description': "# CodeQA\n\nCodeQA is a command-line tool that allows you to ask questions about a project. Gain insights and deepen your\nunderstanding of a repository's codebase effortlessly. It is built on top of LangChain.\n\n## Getting Started\n\nInstall Code QA:\n\n```bash\npip install code-qa\n```\n\nAdd your OpenAI token as virtual environment:\n\n```bash\nexport OPENAI_TOKEN=YOUR_TOKEN\n```\n\nGo to your project folder:\n\n```bash\ncd PATH/TO/MY/PROJECT\n```\n\nInitialise Code QA Index. This will generate an `code_qa` folder within your project:\n\n```\ncode_qa init\n```\n\nAsk questions about my code:\n\n```\ncode_qa query How can I test this?\n```\n\n## Ignoring Files\n\nIf you want to ignore certain files, then create an `.codeqaignore` file and specify them. The file follows the same\nstandard as `.gitignore`\n\n## License\nApache License Version 2.0, see `LICENSE`",
+    'long_description': "# CodeQA\n\nCodeQA is a command-line tool that allows you to ask questions about a project. Gain insights and deepen your\nunderstanding of a repository's codebase effortlessly. It is built on top of LangChain.\n\n## Getting Started\n\nInstall Code QA:\n\n```bash\npip install code-qa\n```\n\nAdd your OpenAI token as virtual environment:\n\n```bash\nexport OPENAI_TOKEN=YOUR_TOKEN\n```\n\nGo to your project folder:\n\n```bash\ncd PATH/TO/MY/PROJECT\n```\n\nInitialise Code QA Index. This will generate an `code_qa` folder within your project:\n\n```\ncode_qa init\n```\n\nAsk questions about my code:\n\n```\ncode_qa query How can I test this\n```\n\n## Ignoring Files\n\nIf you want to ignore certain files, then create an `.codeqaignore` file and specify them. The file follows the same\nstandard as `.gitignore`\n\n## License\nApache License Version 2.0, see `LICENSE`",
     'author': 'Steven Mi',
     'author_email': 'steven.mi@getyourguide.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `code_qa-0.1.0/PKG-INFO` & `code_qa-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: code-qa
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Author: Steven Mi
 Author-email: steven.mi@getyourguide.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -47,15 +47,15 @@
 ```
 code_qa init
 ```
 
 Ask questions about my code:
 
 ```
-code_qa query How can I test this?
+code_qa query How can I test this
 ```
 
 ## Ignoring Files
 
 If you want to ignore certain files, then create an `.codeqaignore` file and specify them. The file follows the same
 standard as `.gitignore`
```

