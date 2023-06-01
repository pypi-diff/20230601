# Comparing `tmp/omnata_cli-0.1.2.tar.gz` & `tmp/omnata_cli-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omnata_cli-0.1.2.tar", max compression
+gzip compressed data, was "omnata_cli-0.1.3.tar", max compression
```

## Comparing `omnata_cli-0.1.2.tar` & `omnata_cli-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    26526 2023-06-01 06:34:59.710435 omnata_cli-0.1.2/LICENSE
--rw-r--r--   0        0        0       49 2023-06-01 06:34:59.710435 omnata_cli-0.1.2/README.md
--rw-r--r--   0        0        0      498 2023-06-01 06:34:59.710435 omnata_cli-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1130 2023-06-01 06:34:59.710435 omnata_cli-0.1.2/src/omnata_cli/__init__.py
--rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 omnata_cli-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    26526 2023-06-01 06:40:43.113456 omnata_cli-0.1.3/LICENSE
+-rw-r--r--   0        0        0       49 2023-06-01 06:40:43.113456 omnata_cli-0.1.3/README.md
+-rw-r--r--   0        0        0      501 2023-06-01 06:40:43.113456 omnata_cli-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1130 2023-06-01 06:40:43.113456 omnata_cli-0.1.3/src/omnata_cli/__init__.py
+-rw-r--r--   0        0        0      499 1970-01-01 00:00:00.000000 omnata_cli-0.1.3/PKG-INFO
```

### Comparing `omnata_cli-0.1.2/LICENSE` & `omnata_cli-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `omnata_cli-0.1.2/src/omnata_cli/__init__.py` & `omnata_cli-0.1.3/src/omnata_cli/__init__.py`

 * *Files identical despite different names*

