# Comparing `tmp/folder_tree_generator-0.1.6.tar.gz` & `tmp/folder_tree_generator-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "folder_tree_generator-0.1.6.tar", max compression
+gzip compressed data, was "folder_tree_generator-0.1.7.tar", max compression
```

## Comparing `folder_tree_generator-0.1.6.tar` & `folder_tree_generator-0.1.7.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1061 2023-04-12 06:31:17.603547 folder_tree_generator-0.1.6/LICENSE
--rw-r--r--   0        0        0     2459 2023-06-01 07:36:02.389051 folder_tree_generator-0.1.6/README.md
--rw-r--r--   0        0        0        0 2023-06-01 07:35:42.561025 folder_tree_generator-0.1.6/folder_tree_generator/__init__.py
--rw-r--r--   0        0        0     3102 2023-06-01 07:28:20.762716 folder_tree_generator-0.1.6/folder_tree_generator/folder_tree_generator.py
--rw-r--r--   0        0        0      562 2023-06-01 07:35:47.330186 folder_tree_generator-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     3181 1970-01-01 00:00:00.000000 folder_tree_generator-0.1.6/setup.py
--rw-r--r--   0        0        0     2920 1970-01-01 00:00:00.000000 folder_tree_generator-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-04-12 06:31:17.603547 folder_tree_generator-0.1.7/LICENSE
+-rw-r--r--   0        0        0     2459 2023-06-01 07:36:02.389051 folder_tree_generator-0.1.7/README.md
+-rw-r--r--   0        0        0     3102 2023-06-01 07:28:20.762716 folder_tree_generator-0.1.7/folder_tree_generator/folder_tree_generator.py
+-rw-r--r--   0        0        0      562 2023-06-01 07:43:55.295639 folder_tree_generator-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     3181 1970-01-01 00:00:00.000000 folder_tree_generator-0.1.7/setup.py
+-rw-r--r--   0        0        0     2920 1970-01-01 00:00:00.000000 folder_tree_generator-0.1.7/PKG-INFO
```

### Comparing `folder_tree_generator-0.1.6/LICENSE` & `folder_tree_generator-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `folder_tree_generator-0.1.6/README.md` & `folder_tree_generator-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `folder_tree_generator-0.1.6/folder_tree_generator/folder_tree_generator.py` & `folder_tree_generator-0.1.7/folder_tree_generator/folder_tree_generator.py`

 * *Files identical despite different names*

### Comparing `folder_tree_generator-0.1.6/setup.py` & `folder_tree_generator-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['folder_tree_generator']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'folder-tree-generator',
-    'version': '0.1.6',
+    'version': '0.1.7',
     'description': 'Takes a folder path and outputs a text representation of the folders and files, supports ignore files.',
     'long_description': '# Folder Tree Generator\n\n\n[![PyPI version](https://badge.fury.io/py/folder-tree-generator.svg)](https://badge.fury.io/py/folder-tree-generator)\n\n![Test](https://github.com/seandearnaley/folder-tree-generator/workflows/Run%20pytest/badge.svg)\n\n\nFolder Tree Generator is a Python module that takes a folder path and outputs a text representation of the folders and files. It supports ignore files, such as `.gitignore`, to exclude certain files or folders from the output.\n\ntypical string output:\n\n```text\nmy_project/\n|-- .gitignore\n|-- main.py\n|-- utils.py\n|-- data/\n|   |-- input.txt\n|   |-- output.txt\n```\n\n## Why?\n\nI needed a way to generate folder structures in a standard text format that I could copy and paste into GPT without including all the build artifacts, eg. repository structures for code analysis.  If you wanted to make your own ignore file it should be a simple adapation of a gitignore file, in 90% of my use cases, the gitignore is sufficient.\n\n## Installation\n\nYou can install the module from PyPI using pip:\n\n```bash\npip install folder-tree-generator\n```\n\n## Usage\n\nYou can use the module as a command-line tool or import it in your Python script.\n\n### Command-line usage\n\n```bash\npython -m folder_tree_generator/folder_tree_generator /path/to/your/folder\n```\n\n### Python script usage\n\n```python\nfrom folder_tree_generator import generate_tree\n\noutput_text = generate_tree("/path/to/your/folder")\nprint(output_text)\n```\n\n## Configuration\n\nBy default, the module looks for a `.gitignore` file in the root folder to determine which files and folders to ignore. You can change the ignore file name by passing an optional argument to the `generate_tree` function:\n\n```python\noutput_text = generate_tree("/path/to/your/folder", ignore_file_name=".myignore")\n```\n\n## Development\n\nTo set up the development environment, clone the repository and install the required dependencies using Poetry:\n\n```bash\ngit clone https://github.com/seandearnaley/folder-tree-generator.git\ncd folder-tree-generator\npoetry install\n```\n\nTo run the tests, use the following command:\n\n```bash\npoetry run pytest\n```\n\nMake sure to update the README.md file with these changes.\n\n## Contributing\n\nContributions are welcome! Please feel free to submit a pull request or open an issue on the [GitHub repository](https://github.com/seandearnaley/folder-tree-generator).\n\n## License\n\nThis project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.',
     'author': 'Sean Dearnaley',
     'author_email': 'SeanDearnaley@outlook.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `folder_tree_generator-0.1.6/PKG-INFO` & `folder_tree_generator-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: folder-tree-generator
-Version: 0.1.6
+Version: 0.1.7
 Summary: Takes a folder path and outputs a text representation of the folders and files, supports ignore files.
 Author: Sean Dearnaley
 Author-email: SeanDearnaley@outlook.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

