# Comparing `tmp/kiwi_cogs-0.0.1.tar.gz` & `tmp/kiwi_cogs-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiwi_cogs-0.0.1.tar", max compression
+gzip compressed data, was "kiwi_cogs-0.1.0.tar", max compression
```

## Comparing `kiwi_cogs-0.0.1.tar` & `kiwi_cogs-0.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1068 2023-06-01 18:44:19.655025 kiwi_cogs-0.0.1/LICENSE
--rw-r--r--   0        0        0     1276 2023-06-01 18:44:19.655025 kiwi_cogs-0.0.1/README.md
--rw-r--r--   0        0        0      169 2023-06-01 18:44:19.659025 kiwi_cogs-0.0.1/kiwi_cogs/__init__.py
--rw-r--r--   0        0        0     2528 2023-06-01 18:44:19.659025 kiwi_cogs-0.0.1/kiwi_cogs/event.py
--rw-r--r--   0        0        0      210 2023-06-01 18:44:19.659025 kiwi_cogs-0.0.1/kiwi_cogs/exceptions.py
--rw-r--r--   0        0        0     7700 2023-06-01 18:44:19.659025 kiwi_cogs-0.0.1/kiwi_cogs/machine.py
--rw-r--r--   0        0        0    10253 2023-06-01 18:44:19.659025 kiwi_cogs-0.0.1/kiwi_cogs/state.py
--rw-r--r--   0        0        0     4098 2023-06-01 18:44:19.659025 kiwi_cogs-0.0.1/kiwi_cogs/transition.py
--rw-r--r--   0        0        0      465 2023-06-01 18:44:19.659025 kiwi_cogs-0.0.1/kiwi_cogs/utils.py
--rw-r--r--   0        0        0     2060 2023-06-01 18:44:19.659025 kiwi_cogs-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1997 1970-01-01 00:00:00.000000 kiwi_cogs-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-01 21:09:32.501623 kiwi_cogs-0.1.0/LICENSE
+-rw-r--r--   0        0        0     5738 2023-06-01 21:09:32.501623 kiwi_cogs-0.1.0/README.md
+-rw-r--r--   0        0        0      169 2023-06-01 21:09:32.501623 kiwi_cogs-0.1.0/kiwi_cogs/__init__.py
+-rw-r--r--   0        0        0     2528 2023-06-01 21:09:32.505623 kiwi_cogs-0.1.0/kiwi_cogs/event.py
+-rw-r--r--   0        0        0      210 2023-06-01 21:09:32.505623 kiwi_cogs-0.1.0/kiwi_cogs/exceptions.py
+-rw-r--r--   0        0        0     7700 2023-06-01 21:09:32.505623 kiwi_cogs-0.1.0/kiwi_cogs/machine.py
+-rw-r--r--   0        0        0    10253 2023-06-01 21:09:32.505623 kiwi_cogs-0.1.0/kiwi_cogs/state.py
+-rw-r--r--   0        0        0     4098 2023-06-01 21:09:32.505623 kiwi_cogs-0.1.0/kiwi_cogs/transition.py
+-rw-r--r--   0        0        0      465 2023-06-01 21:09:32.505623 kiwi_cogs-0.1.0/kiwi_cogs/utils.py
+-rw-r--r--   0        0        0     2060 2023-06-01 21:09:52.445905 kiwi_cogs-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6459 1970-01-01 00:00:00.000000 kiwi_cogs-0.1.0/PKG-INFO
```

### Comparing `kiwi_cogs-0.0.1/LICENSE` & `kiwi_cogs-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kiwi_cogs-0.0.1/kiwi_cogs/event.py` & `kiwi_cogs-0.1.0/kiwi_cogs/event.py`

 * *Files identical despite different names*

### Comparing `kiwi_cogs-0.0.1/kiwi_cogs/machine.py` & `kiwi_cogs-0.1.0/kiwi_cogs/machine.py`

 * *Files identical despite different names*

### Comparing `kiwi_cogs-0.0.1/kiwi_cogs/state.py` & `kiwi_cogs-0.1.0/kiwi_cogs/state.py`

 * *Files identical despite different names*

### Comparing `kiwi_cogs-0.0.1/kiwi_cogs/transition.py` & `kiwi_cogs-0.1.0/kiwi_cogs/transition.py`

 * *Files identical despite different names*

### Comparing `kiwi_cogs-0.0.1/pyproject.toml` & `kiwi_cogs-0.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kiwi_cogs"
-version = "0.0.1"
+version = "0.1.0"
 description = "A simple and easy to use state machine library "
 authors = ["David Hall <fdev@davidhall.tech>"]
 repository = "https://github.com/mopeyjellyfish/kiwi-cogs"
 documentation = "https://mopeyjellyfish.github.io/kiwi-cogs/"
 readme = "README.md"
 packages = [
   {include = "kiwi_cogs"}
```

