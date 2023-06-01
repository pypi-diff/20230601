# Comparing `tmp/clandestined-1.0.1.tar.gz` & `tmp/clandestined-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/clandestined-1.0.1.tar", last modified: Tue Jun 30 13:19:28 2015, max compression
+gzip compressed data, was "clandestined-1.1.0.tar", last modified: Thu Jun  1 18:07:15 2023, max compression
```

## Comparing `clandestined-1.0.1.tar` & `clandestined-1.1.0.tar`

### file list

```diff
@@ -1,9 +1,17 @@
-drwxr-xr-x   0 edurbin    (501) wheel        (0)        0 2015-06-30 13:19:28.000000 clandestined-1.0.1/
-drwxr-xr-x   0 edurbin    (501) wheel        (0)        0 2015-06-30 13:19:28.000000 clandestined-1.0.1/clandestined/
--rw-r--r--   0 edurbin    (501) wheel        (0)       63 2015-06-30 12:50:08.000000 clandestined-1.0.1/clandestined/__init__.py
--rw-r--r--   0 edurbin    (501) wheel        (0)     3546 2015-06-30 13:14:28.000000 clandestined-1.0.1/clandestined/clandestined.py
--rw-r--r--   0 edurbin    (501) wheel        (0)     1886 2015-06-30 13:14:28.000000 clandestined-1.0.1/clandestined/murmur3.py
-drwxr-xr-x   0 edurbin    (501) wheel        (0)        0 2015-06-30 13:19:28.000000 clandestined-1.0.1/ext/
--rw-r--r--   0 edurbin    (501) wheel        (0)     3626 2015-06-30 13:14:28.000000 clandestined-1.0.1/ext/_murmur3.c
--rw-r--r--   0 edurbin    (501) wheel        (0)      294 2015-06-30 13:19:28.000000 clandestined-1.0.1/PKG-INFO
--rw-r--r--   0 edurbin    (501) wheel        (0)      824 2015-06-30 13:14:28.000000 clandestined-1.0.1/setup.py
+drwxr-xr-x   0 ee         (501) staff       (20)        0 2023-06-01 18:07:15.966835 clandestined-1.1.0/
+-rw-r--r--   0 ee         (501) staff       (20)     1087 2023-06-01 17:58:29.000000 clandestined-1.1.0/LICENSE
+-rw-r--r--   0 ee         (501) staff       (20)      266 2023-06-01 18:07:15.966737 clandestined-1.1.0/PKG-INFO
+-rw-r--r--   0 ee         (501) staff       (20)     3762 2023-06-01 17:58:29.000000 clandestined-1.1.0/README.md
+drwxr-xr-x   0 ee         (501) staff       (20)        0 2023-06-01 18:07:15.966100 clandestined-1.1.0/clandestined/
+-rw-r--r--   0 ee         (501) staff       (20)       63 2023-06-01 17:58:29.000000 clandestined-1.1.0/clandestined/__init__.py
+-rw-r--r--   0 ee         (501) staff       (20)     3546 2023-06-01 17:58:29.000000 clandestined-1.1.0/clandestined/clandestined.py
+-rw-r--r--   0 ee         (501) staff       (20)     1886 2023-06-01 17:58:29.000000 clandestined-1.1.0/clandestined/murmur3.py
+drwxr-xr-x   0 ee         (501) staff       (20)        0 2023-06-01 18:07:15.966507 clandestined-1.1.0/clandestined.egg-info/
+-rw-r--r--   0 ee         (501) staff       (20)      266 2023-06-01 18:07:15.000000 clandestined-1.1.0/clandestined.egg-info/PKG-INFO
+-rw-r--r--   0 ee         (501) staff       (20)      263 2023-06-01 18:07:15.000000 clandestined-1.1.0/clandestined.egg-info/SOURCES.txt
+-rw-r--r--   0 ee         (501) staff       (20)        1 2023-06-01 18:07:15.000000 clandestined-1.1.0/clandestined.egg-info/dependency_links.txt
+-rw-r--r--   0 ee         (501) staff       (20)       13 2023-06-01 18:07:15.000000 clandestined-1.1.0/clandestined.egg-info/top_level.txt
+drwxr-xr-x   0 ee         (501) staff       (20)        0 2023-06-01 18:07:15.966601 clandestined-1.1.0/ext/
+-rw-r--r--   0 ee         (501) staff       (20)     3655 2023-06-01 18:06:02.000000 clandestined-1.1.0/ext/_murmur3.c
+-rw-r--r--   0 ee         (501) staff       (20)       38 2023-06-01 18:07:15.966863 clandestined-1.1.0/setup.cfg
+-rw-r--r--   0 ee         (501) staff       (20)      813 2023-06-01 18:06:54.000000 clandestined-1.1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `clandestined-1.0.1/clandestined/clandestined.py` & `clandestined-1.1.0/clandestined/clandestined.py`

 * *Files identical despite different names*

### Comparing `clandestined-1.0.1/clandestined/murmur3.py` & `clandestined-1.1.0/clandestined/murmur3.py`

 * *Files identical despite different names*

### Comparing `clandestined-1.0.1/ext/_murmur3.c` & `clandestined-1.1.0/ext/_murmur3.c`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#define PY_SSIZE_T_CLEAN
 #include <Python.h>
 
 #include <stdint.h>
 #include <string.h>
 
 #ifdef PYPY_VERSION
 #define COMPILING_IN_PYPY 1
@@ -9,15 +10,15 @@
 #else
 #define COMPILING_IN_PYPY 0
 #define COMPILING_IN_CPYTHON 1
 #endif
 // MurmurHash3 was written by Austin Appleby, and is placed in the public
 // domain. The author hereby disclaims copyright to this source code.
 
-uint32_t murmur3_32(const char *key, uint32_t len, uint32_t seed) {
+uint32_t murmur3_32(const char *key, Py_ssize_t len, uint32_t seed) {
     static const uint32_t c1 = 0xcc9e2d51;
     static const uint32_t c2 = 0x1b873593;
     static const uint32_t r1 = 15;
     static const uint32_t r2 = 13;
     static const uint32_t m = 5;
     static const uint32_t n = 0xe6546b64;
  
@@ -139,15 +140,15 @@
     return m;
 #endif
 }
 
 static PyObject *clandestined_murmur3_32(PyObject *self, PyObject *args)
 {
     const char *key;
-    uint32_t len;
+    Py_ssize_t len;
     uint32_t seed = 0;
 
     if (!PyArg_ParseTuple(args, "s#|i", &key, &len, &seed)) {
         return NULL;
     }
 
     uint32_t value = murmur3_32(key, len, seed);
```

### Comparing `clandestined-1.0.1/setup.py` & `clandestined-1.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,17 +10,17 @@
     extra_compile_args.append("-Wno-error=declaration-after-statement")
 
 requirements = []
 test_requirements = []
 
 setup(
     name='clandestined',
-    version='1.0.1',
+    version='1.1.0',
     license='MIT',
-    author="Ernest W. Durbin III",
+    author="Ee Durbin",
     author_email='ewdurbin@gmail.com',
     description='rendezvous hashing implementation based on murmur3 hash',
     url='https://github.com/ewdurbin/clandestined-python',
     packages=['clandestined'],
     ext_modules=[Extension('clandestined._murmur3', ['ext/_murmur3.c'],
                            extra_compile_args=extra_compile_args)],
     scripts=[],
```

