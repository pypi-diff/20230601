# Comparing `tmp/num_tini4-0.0.1a2.tar.gz` & `tmp/num_tini4-0.0.1a3.tar.gz`

## Comparing `num_tini4-0.0.1a2.tar` & `num_tini4-0.0.1a3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 num_tini4-0.0.1a2/.github/workflows/codecov.yml
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 num_tini4-0.0.1a2/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 num_tini4-0.0.1a2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 num_tini4-0.0.1a2/src/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 num_tini4-0.0.1a2/src/num_tini4/__init__.py
--rw-r--r--   0        0        0    20793 2020-02-02 00:00:00.000000 num_tini4-0.0.1a2/src/num_tini4/num.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 num_tini4-0.0.1a2/src/num_tini4/primes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 num_tini4-0.0.1a2/tests/__init__.py
--rw-r--r--   0        0        0   117225 2020-02-02 00:00:00.000000 num_tini4-0.0.1a2/tests/test_num.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 num_tini4-0.0.1a2/.gitignore
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 num_tini4-0.0.1a2/LICENSE
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 num_tini4-0.0.1a2/README.md
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 num_tini4-0.0.1a2/pyproject.toml
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 num_tini4-0.0.1a2/PKG-INFO
+-rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 num_tini4-0.0.1a3/README-dev.md
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 num_tini4-0.0.1a3/.github/workflows/codecov.yml
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 num_tini4-0.0.1a3/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 num_tini4-0.0.1a3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 num_tini4-0.0.1a3/src/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 num_tini4-0.0.1a3/src/num_tini4/__init__.py
+-rw-r--r--   0        0        0    20825 2020-02-02 00:00:00.000000 num_tini4-0.0.1a3/src/num_tini4/num.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 num_tini4-0.0.1a3/src/num_tini4/primes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 num_tini4-0.0.1a3/tests/__init__.py
+-rw-r--r--   0        0        0   117225 2020-02-02 00:00:00.000000 num_tini4-0.0.1a3/tests/test_num.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 num_tini4-0.0.1a3/.gitignore
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 num_tini4-0.0.1a3/LICENSE
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 num_tini4-0.0.1a3/README.md
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 num_tini4-0.0.1a3/pyproject.toml
+-rw-r--r--   0        0        0     3478 2020-02-02 00:00:00.000000 num_tini4-0.0.1a3/PKG-INFO
```

### Comparing `num_tini4-0.0.1a2/.github/workflows/codecov.yml` & `num_tini4-0.0.1a3/.github/workflows/codecov.yml`

 * *Files identical despite different names*

### Comparing `num_tini4-0.0.1a2/.github/workflows/pylint.yml` & `num_tini4-0.0.1a3/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `num_tini4-0.0.1a2/.github/workflows/python-publish.yml` & `num_tini4-0.0.1a3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `num_tini4-0.0.1a2/src/num_tini4/num.py` & `num_tini4-0.0.1a3/src/num_tini4/num.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,18 +22,18 @@
         """
         self.primes: dict[int, int] = {}
         self.special: dict[str, int] = {'pi': 0, 'e': 0, 'root': 1}  # TODO
         self.sign: Num.Sign = Num.Sign.POSITIVE
         self.case: Num.Case = Num.Case.UNDEFINED
 
     def __repr__(self):
-        return f"Num(primes={self.primes!r}, sign={self.sign!r}, case={self.case!r})"
+        return f"Num(primes={self.primes!r}, special={self.special!r}, sign={self.sign!r}, case={self.case!r})"
 
     def __str__(self):
-        return f'{self.case.name}, {self.sign.name}, {self.primes}'
+        return f'[{self.case.name}, {self.sign.name}, {self.primes}, {self.special}]'
 
     def _modify_prime_factorization(self, integer: int, sign: Sign):
         # if integer > PRIMES_TO:
         #     size_integer: int = int(log10(integer)) + 1
         #     size_primes: int = int(log10(PRIMES_TO)) + 1
         #
         #     over: int = size_integer - size_primes + 1
@@ -219,15 +219,15 @@
 
             if self.case is Num.Case.INFINITY:
                 return float('inf') * self.sign.value
 
             if self.case is Num.Case.UNDEFINED:
                 return float('nan')
 
-        out: float = self.sign.value
+        out: float = float(self.sign.value)
 
         for prime in self.primes:
             if self.primes[prime] > 0:
                 out *= prime ** self.primes[prime]
             else:
                 out /= prime ** -self.primes[prime]
 
@@ -710,9 +710,7 @@
     print(number2 != number2)
     print()
 
     # number1.set_num({2: 1, 3: -1, 11: 1})
     number1.set_num(case=Num.Case.UNDEFINED, sign=Num.Sign.NEGATIVE)
     print(float(number1))
     print(number1)
-
-    # test pylint
```

### Comparing `num_tini4-0.0.1a2/tests/test_num.py` & `num_tini4-0.0.1a3/tests/test_num.py`

 * *Files identical despite different names*

### Comparing `num_tini4-0.0.1a2/pyproject.toml` & `num_tini4-0.0.1a3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "num_tini4"
-version = "0.0.1a2"
+version = "0.0.1a3"
 authors = [
   { name="Tini4", email="tilen.jurican@gmail.com" },
 ]
 description = "Python precise number type."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 1 - Planning",
+    "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: Other/Proprietary License",
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering :: Mathematics",
 ]
 
 [project.urls]
```

