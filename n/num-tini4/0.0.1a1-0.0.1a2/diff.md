# Comparing `tmp/num_tini4-0.0.1a1.tar.gz` & `tmp/num_tini4-0.0.1a2.tar.gz`

## Comparing `num_tini4-0.0.1a1.tar` & `num_tini4-0.0.1a2.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 num_tini4-0.0.1a1/.github/workflows/codecov.yml
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 num_tini4-0.0.1a1/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 num_tini4-0.0.1a1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 num_tini4-0.0.1a1/src/Num_Tini4/__init__.py
--rw-r--r--   0        0        0    20793 2020-02-02 00:00:00.000000 num_tini4-0.0.1a1/src/Num_Tini4/num.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 num_tini4-0.0.1a1/src/Num_Tini4/primes.py
--rw-r--r--   0        0        0   117225 2020-02-02 00:00:00.000000 num_tini4-0.0.1a1/tests/test_num.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 num_tini4-0.0.1a1/.gitignore
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 num_tini4-0.0.1a1/LICENSE
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 num_tini4-0.0.1a1/README.md
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 num_tini4-0.0.1a1/pyproject.toml
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 num_tini4-0.0.1a1/PKG-INFO
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 num_tini4-0.0.1a2/.github/workflows/codecov.yml
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 num_tini4-0.0.1a2/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 num_tini4-0.0.1a2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 num_tini4-0.0.1a2/src/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 num_tini4-0.0.1a2/src/num_tini4/__init__.py
+-rw-r--r--   0        0        0    20793 2020-02-02 00:00:00.000000 num_tini4-0.0.1a2/src/num_tini4/num.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 num_tini4-0.0.1a2/src/num_tini4/primes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 num_tini4-0.0.1a2/tests/__init__.py
+-rw-r--r--   0        0        0   117225 2020-02-02 00:00:00.000000 num_tini4-0.0.1a2/tests/test_num.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 num_tini4-0.0.1a2/.gitignore
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 num_tini4-0.0.1a2/LICENSE
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 num_tini4-0.0.1a2/README.md
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 num_tini4-0.0.1a2/pyproject.toml
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 num_tini4-0.0.1a2/PKG-INFO
```

### Comparing `num_tini4-0.0.1a1/.github/workflows/codecov.yml` & `num_tini4-0.0.1a2/.github/workflows/codecov.yml`

 * *Files identical despite different names*

### Comparing `num_tini4-0.0.1a1/.github/workflows/pylint.yml` & `num_tini4-0.0.1a2/.github/workflows/pylint.yml`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 on: [push]
 
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.11"]
+        python-version: ["3.10", "3.11"]
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v3
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
```

### Comparing `num_tini4-0.0.1a1/.github/workflows/python-publish.yml` & `num_tini4-0.0.1a2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `num_tini4-0.0.1a1/src/Num_Tini4/num.py` & `num_tini4-0.0.1a2/src/num_tini4/num.py`

 * *Files identical despite different names*

### Comparing `num_tini4-0.0.1a1/tests/test_num.py` & `num_tini4-0.0.1a2/tests/test_num.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 
-from src.Num_Tini4.num import Num
+from src.num_tini4.num import Num
 
 
 class TestNumEnum(unittest.TestCase):
     def setUp(self):
         pass
 
     def test_sign(self):  # todo
```

### Comparing `num_tini4-0.0.1a1/README.md` & `num_tini4-0.0.1a2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 [![Pylint](https://github.com/Tini4/Num/actions/workflows/pylint.yml/badge.svg)](https://github.com/Tini4/Num/actions/workflows/pylint.yml)
 [![codecov](https://codecov.io/gh/Tini4/Num/branch/master/graph/badge.svg?token=BILTI4331O)](https://codecov.io/gh/Tini4/Num)
 
 Python precise number type.
 
 ```python
-from src.Num_Tini4.num import Num
+from src.num_tini4.num import Num
 
 number1 = Num()
 number2 = Num()
 
 number1.set_num({2: 1, 3: 2}, sign=Num.Sign.NEGATIVE)  # 18
 number2.set_num({11: -1})  # 1/11
```

### Comparing `num_tini4-0.0.1a1/pyproject.toml` & `num_tini4-0.0.1a2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
-name = "Num_Tini4"
-version = "0.0.1a1"
+name = "num_tini4"
+version = "0.0.1a2"
 authors = [
   { name="Tini4", email="tilen.jurican@gmail.com" },
 ]
 description = "Python precise number type."
 readme = "README.md"
-requires-python = ">=3.11"
+requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 1 - Planning",
     "Programming Language :: Python :: 3.11",
     "License :: Other/Proprietary License",
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering :: Mathematics",
 ]
```

### Comparing `num_tini4-0.0.1a1/PKG-INFO` & `num_tini4-0.0.1a2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
-Name: Num_Tini4
-Version: 0.0.1a1
+Name: num_tini4
+Version: 0.0.1a2
 Summary: Python precise number type.
 Project-URL: Homepage, https://github.com/Tini4/Num
 Project-URL: Bug Tracker, https://github.com/Tini4/Num/issues
 Author-email: Tini4 <tilen.jurican@gmail.com>
 License-File: LICENSE
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Mathematics
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # Example Package
 
 This is a simple example package. You can use
 [Github-flavored Markdown](https://guides.github.com/features/mastering-markdown/)
 to write your content.
@@ -25,15 +25,15 @@
 
 [![Pylint](https://github.com/Tini4/Num/actions/workflows/pylint.yml/badge.svg)](https://github.com/Tini4/Num/actions/workflows/pylint.yml)
 [![codecov](https://codecov.io/gh/Tini4/Num/branch/master/graph/badge.svg?token=BILTI4331O)](https://codecov.io/gh/Tini4/Num)
 
 Python precise number type.
 
 ```python
-from src.Num_Tini4.num import Num
+from src.num_tini4.num import Num
 
 number1 = Num()
 number2 = Num()
 
 number1.set_num({2: 1, 3: 2}, sign=Num.Sign.NEGATIVE)  # 18
 number2.set_num({11: -1})  # 1/11
```

