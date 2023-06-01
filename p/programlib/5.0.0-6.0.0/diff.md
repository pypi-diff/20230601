# Comparing `tmp/programlib-5.0.0.tar.gz` & `tmp/programlib-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "programlib-5.0.0.tar", max compression
+gzip compressed data, was "programlib-6.0.0.tar", max compression
```

## Comparing `programlib-5.0.0.tar` & `programlib-6.0.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1082 2023-02-27 15:04:14.303270 programlib-5.0.0/LICENSE
--rw-r--r--   0        0        0     3335 2023-02-27 15:04:14.303270 programlib-5.0.0/README.md
--rw-r--r--   0        0        0       81 2023-02-27 15:04:14.303270 programlib-5.0.0/programlib/__init__.py
--rw-r--r--   0        0        0     4957 2023-02-27 15:04:14.303270 programlib-5.0.0/programlib/language.py
--rw-r--r--   0        0        0     4786 2023-02-27 15:04:14.303270 programlib-5.0.0/programlib/program.py
--rw-r--r--   0        0        0        0 2023-02-27 15:04:14.303270 programlib-5.0.0/programlib/programs/.gitkeep
--rw-r--r--   0        0        0      468 2023-02-27 15:04:14.303270 programlib-5.0.0/pyproject.toml
--rw-r--r--   0        0        0     4052 1970-01-01 00:00:00.000000 programlib-5.0.0/setup.py
--rw-r--r--   0        0        0     4092 1970-01-01 00:00:00.000000 programlib-5.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-06-01 16:28:29.466859 programlib-6.0.0/LICENSE
+-rw-r--r--   0        0        0     3836 2023-06-01 16:28:29.466859 programlib-6.0.0/README.md
+-rw-r--r--   0        0        0       81 2023-06-01 16:28:29.466859 programlib-6.0.0/programlib/__init__.py
+-rw-r--r--   0        0        0     2154 2023-06-01 16:28:29.466859 programlib-6.0.0/programlib/agent.py
+-rw-r--r--   0        0        0     4957 2023-06-01 16:28:29.466859 programlib-6.0.0/programlib/language.py
+-rw-r--r--   0        0        0     4039 2023-06-01 16:28:29.466859 programlib-6.0.0/programlib/program.py
+-rw-r--r--   0        0        0        0 2023-06-01 16:28:29.466859 programlib-6.0.0/programlib/programs/.gitkeep
+-rw-r--r--   0        0        0      484 2023-06-01 16:28:29.466859 programlib-6.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4581 1970-01-01 00:00:00.000000 programlib-6.0.0/PKG-INFO
```

### Comparing `programlib-5.0.0/LICENSE` & `programlib-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `programlib-5.0.0/README.md` & `programlib-6.0.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -20,17 +20,26 @@
 
 ```python
 from programlib import Program
 program = Program(source_code, language='C++')
 ```
 
 This object has
-- a `run` method that runs the program and returns a list of strings it printed to `stdout`. You can optionally provide a list of input strings as well.
-- a `test` method that takes a list of test cases. A test case is a tuple of 2 lists: the first list is the input strings, the second is the expected output strings. The method returns percentage of output strings that matched expectations.
 - a `save` method that will save the source code to a file at the specified path.
+- a `run` method that runs the program and returns a list of strings it printed to `stdout`. You can optionally provide a list of input strings as well.
+- a `spawn` method that launches the program in an interactive mode. It returns an `Agent` object with and `act` method that takes a sequence of input strings and returns a list of strings printed to `stdout` in response.
+- a `test` method that takes a list of test cases. A test case is a tuple of 2 lists: the first list is the input strings, the second is the expected output strings. The method returns a full log of all test runs and updates `program.avg_score` and `program.test_pass_rate` attributes.
+
+To test the program on a Reinforcement Learning environment, call
+
+```python
+program.spawn().test(env)
+```
+
+where `env` is a `gym` environment. The method returns the rollout and updates `program.avg_score` to be the sum of rewards.
 
 See also `examples`.
 
 Currently supported programming languages out of the box are C++, Python, Java, Clojure, Ruby, Rust, Go, Haskell, Scala, Kotlin, PHP, C#, Swift, D, Julia, Clojure, Elixir and Erlang.
 See "Advanced usage" below for instructions on how to add other languages.
 
 ## Advanced usage
```

### Comparing `programlib-5.0.0/programlib/language.py` & `programlib-6.0.0/programlib/language.py`

 * *Files identical despite different names*

### Comparing `programlib-5.0.0/programlib/program.py` & `programlib-6.0.0/programlib/program.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from collections import namedtuple
 from statistics import mean, StatisticsError
 from typing import NamedTuple
 from uuid import uuid4
 from pathlib import Path
 from itertools import zip_longest
+from programlib.agent import Agent
 
 from programlib import language_
 
 def correctness(expected_outputs, outputs):
     assert expected_outputs, 'expected_outputs is empty. Cannot test program correctness.'
 
     try:
@@ -16,43 +17,14 @@
                     in zip_longest(expected_outputs, outputs))
     except StatisticsError:
         return 0
 
 TestRun = namedtuple('TestRun', ['input_lines', 'expected_output_lines', 
                                  'output_lines', 'exit_status', 'correctness'])
 
-class Agent():
-    """
-    Agent: represents a running program that can be interacted with
-    """
-
-    def __init__(self, program, process, lines_per_message=1):
-        self.program = program
-        self.process = process
-        self.lines_per_message = lines_per_message
-        
-        self.program.stdout = ''
-
-    def act(self, input_lines):
-        for line in input_lines:
-            self.process.sendline(line)
-        
-        for line_idx in range(self.lines_per_message):
-            line = self.process.readline()
-            line = line.decode()
-            self.program.stdout += line
-            yield line.strip()
-    
-    def close(self):
-        self.process.close()
-        self.program.exitstatus = self.process.exitstatus
-    
-    def __del__(self):
-        self.close()
-
 class Program():
     """
     Program object: represents a runnable program in some programming language
     """
 
     def __init__(self, source, name=None, language='C++', 
                        workdir=Path(__file__).parent / 'programs'):
@@ -87,21 +59,21 @@
         Raw stdout and stderr data will always be stored in `program.stdout` and `program.stderr` attributes
         """
 
         self.stdout, self.exitstatus = self.language.run(self.workdir, self.name, input_lines)
         assert force or not self.exitstatus, f'Exit status {self.exitstatus}'
         return self.stdout.splitlines()
     
-    def spawn(self, lines_per_message=1):
+    def spawn(self, delimiter='\n'):
         """
         Launch the program and get a process object to communicate with it interactively
         """
 
         process = self.language.spawn(self.workdir, self.name)
-        return Agent(self, process)
+        return Agent(self, process, delimiter=delimiter)
 
     def test(self, test_cases, force=True):
         """
         Test the program against a list of input output pairs
 
         If 'force=True', program outputs will be checked even if there are errors on stderr
         If 'cache=True', all the test logs will be stored in `program.test_runs` attribute
```

### Comparing `programlib-5.0.0/setup.py` & `programlib-6.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,96 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: programlib
+Version: 6.0.0
+Summary: Programs as Objects
+License: MIT
+Author: Vadim Liventsev
+Author-email: dev@vadim.me
+Requires-Python: >=3.8,<4.0
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Compilers
+Requires-Dist: gym (>=0.26.2,<0.27.0)
+Requires-Dist: pexpect (>=4.8.0,<5.0.0)
+Description-Content-Type: text/markdown
+
+# Programlib: programs as objects
+
+Programlib is a tool that turns programs in any programming language into convenient Python objects, letting you run any string as a C++/Python/Clojure/etc program from a Python script.
+This project is aimed to help develop automatic programming and genetic software improvement systems, though many other applications are possible.
+
+## Installation
+
+Programlib can be installed with
+
+```
+pip install programlib
+```
+
+However, you have to also make sure that the programming languages you want to use are installed.
+By default, programlib uses command line tools that come with the programming languages, i.e. `python3` or `javac`.
+
+## Standard usage
+
+Create a program object with
+
+```python
+from programlib import Program
+program = Program(source_code, language='C++')
+```
+
+This object has
+- a `save` method that will save the source code to a file at the specified path.
+- a `run` method that runs the program and returns a list of strings it printed to `stdout`. You can optionally provide a list of input strings as well.
+- a `spawn` method that launches the program in an interactive mode. It returns an `Agent` object with and `act` method that takes a sequence of input strings and returns a list of strings printed to `stdout` in response.
+- a `test` method that takes a list of test cases. A test case is a tuple of 2 lists: the first list is the input strings, the second is the expected output strings. The method returns a full log of all test runs and updates `program.avg_score` and `program.test_pass_rate` attributes.
+
+To test the program on a Reinforcement Learning environment, call
+
+```python
+program.spawn().test(env)
+```
+
+where `env` is a `gym` environment. The method returns the rollout and updates `program.avg_score` to be the sum of rewards.
+
+See also `examples`.
+
+Currently supported programming languages out of the box are C++, Python, Java, Clojure, Ruby, Rust, Go, Haskell, Scala, Kotlin, PHP, C#, Swift, D, Julia, Clojure, Elixir and Erlang.
+See "Advanced usage" below for instructions on how to add other languages.
+
+## Advanced usage
+
+### Language configuration
+
+When you create a program object with a language name like `language='C++'`, `programlib` retrieves an appropriate language configuration from it's database.
+If you have a different opinion on how to compile or run in this language or want to use a language that is not supported out of the box, you can create your own language configuration object:
+
+```python
+from programlib import Program, Language
+language = Language(
+        build_cmd='g++ {name}.cpp -o {name}',
+        run_cmd='./{name}',
+        source='{name}.cpp',
+        artefacts=['{name}']
+    )
+program = Program(source_code, language=language)
+```
+
+`source` parameter describes the naming convention for the source file (usually `{name}.extension`). Make sure that this parameter contains a `{name}` placeholder, so that `programlib` can keep track of several source files at the same time.
+`build_cmd` and `run_cmd` respectively instruct `programlib` which commands to use to compile and run the program in this language.
+`artefacts` is a list of all the files produced by `build_cmd` command.
+It is needed to clean up the artefacts when the program object is destroyed.
+
+### Error handling
+
+Any output written to `stderr` is considered an error.
+By default, any errors at build time or run time will lead to an exception being raised, with 2 exceptions:
+- `test` function that catches exceptions during test cases execution and marks these tests as failed.
+- Setting `program.run(force=True)` or `program.test(force=True)` will make `programlib` ignore all errors.
 
-packages = \
-['programlib']
-
-package_data = \
-{'': ['*'], 'programlib': ['programs/*']}
-
-install_requires = \
-['pexpect>=4.8.0,<5.0.0']
-
-setup_kwargs = {
-    'name': 'programlib',
-    'version': '5.0.0',
-    'description': 'Programs as Objects',
-    'long_description': '# Programlib: programs as objects\n\nProgramlib is a tool that turns programs in any programming language into convenient Python objects, letting you run any string as a C++/Python/Clojure/etc program from a Python script.\nThis project is aimed to help develop automatic programming and genetic software improvement systems, though many other applications are possible.\n\n## Installation\n\nProgramlib can be installed with\n\n```\npip install programlib\n```\n\nHowever, you have to also make sure that the programming languages you want to use are installed.\nBy default, programlib uses command line tools that come with the programming languages, i.e. `python3` or `javac`.\n\n## Standard usage\n\nCreate a program object with\n\n```python\nfrom programlib import Program\nprogram = Program(source_code, language=\'C++\')\n```\n\nThis object has\n- a `run` method that runs the program and returns a list of strings it printed to `stdout`. You can optionally provide a list of input strings as well.\n- a `test` method that takes a list of test cases. A test case is a tuple of 2 lists: the first list is the input strings, the second is the expected output strings. The method returns percentage of output strings that matched expectations.\n- a `save` method that will save the source code to a file at the specified path.\n\nSee also `examples`.\n\nCurrently supported programming languages out of the box are C++, Python, Java, Clojure, Ruby, Rust, Go, Haskell, Scala, Kotlin, PHP, C#, Swift, D, Julia, Clojure, Elixir and Erlang.\nSee "Advanced usage" below for instructions on how to add other languages.\n\n## Advanced usage\n\n### Language configuration\n\nWhen you create a program object with a language name like `language=\'C++\'`, `programlib` retrieves an appropriate language configuration from it\'s database.\nIf you have a different opinion on how to compile or run in this language or want to use a language that is not supported out of the box, you can create your own language configuration object:\n\n```python\nfrom programlib import Program, Language\nlanguage = Language(\n        build_cmd=\'g++ {name}.cpp -o {name}\',\n        run_cmd=\'./{name}\',\n        source=\'{name}.cpp\',\n        artefacts=[\'{name}\']\n    )\nprogram = Program(source_code, language=language)\n```\n\n`source` parameter describes the naming convention for the source file (usually `{name}.extension`). Make sure that this parameter contains a `{name}` placeholder, so that `programlib` can keep track of several source files at the same time.\n`build_cmd` and `run_cmd` respectively instruct `programlib` which commands to use to compile and run the program in this language.\n`artefacts` is a list of all the files produced by `build_cmd` command.\nIt is needed to clean up the artefacts when the program object is destroyed.\n\n### Error handling\n\nAny output written to `stderr` is considered an error.\nBy default, any errors at build time or run time will lead to an exception being raised, with 2 exceptions:\n- `test` function that catches exceptions during test cases execution and marks these tests as failed.\n- Setting `program.run(force=True)` or `program.test(force=True)` will make `programlib` ignore all errors.\n\nYou can check `program.stdout` and `program.stderr` to see what the program printed to `stdout` and `stderr` during the last run (or, if in was never run, during build).',
-    'author': 'Vadim Liventsev',
-    'author_email': 'dev@vadim.me',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
+You can check `program.stdout` and `program.stderr` to see what the program printed to `stdout` and `stderr` during the last run (or, if in was never run, during build).
```

