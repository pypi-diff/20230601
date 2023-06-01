# Comparing `tmp/dashadmdv_custom_serializer-0.2.0.tar.gz` & `tmp/dashadmdv_custom_serializer-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dashadmdv_custom_serializer-0.2.0.tar", last modified: Thu Jun  1 19:48:31 2023, max compression
+gzip compressed data, was "dashadmdv_custom_serializer-0.3.0.tar", last modified: Thu Jun  1 19:59:57 2023, max compression
```

## Comparing `dashadmdv_custom_serializer-0.2.0.tar` & `dashadmdv_custom_serializer-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 19:48:31.514333 dashadmdv_custom_serializer-0.2.0/
--rw-rw-rw-   0        0        0      182 2023-06-01 19:48:31.514333 dashadmdv_custom_serializer-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0        5 2023-05-22 20:00:25.000000 dashadmdv_custom_serializer-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 19:48:31.498709 dashadmdv_custom_serializer-0.2.0/dashadmdv_custom_serializer.egg-info/
--rw-rw-rw-   0        0        0      182 2023-06-01 19:48:31.000000 dashadmdv_custom_serializer-0.2.0/dashadmdv_custom_serializer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-06-01 19:48:31.000000 dashadmdv_custom_serializer-0.2.0/dashadmdv_custom_serializer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 19:48:31.000000 dashadmdv_custom_serializer-0.2.0/dashadmdv_custom_serializer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 19:48:31.000000 dashadmdv_custom_serializer-0.2.0/dashadmdv_custom_serializer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 19:48:31.514333 dashadmdv_custom_serializer-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      485 2023-06-01 19:48:13.000000 dashadmdv_custom_serializer-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 19:59:57.532405 dashadmdv_custom_serializer-0.3.0/
+-rw-rw-rw-   0        0        0      182 2023-06-01 19:59:57.532405 dashadmdv_custom_serializer-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0        5 2023-05-22 20:00:25.000000 dashadmdv_custom_serializer-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 19:59:57.479005 dashadmdv_custom_serializer-0.3.0/custom_serializer/
+-rw-rw-rw-   0        0        0       51 2023-06-01 18:22:24.000000 dashadmdv_custom_serializer-0.3.0/custom_serializer/__init__.py
+-rw-rw-rw-   0        0        0      732 2023-06-01 18:17:27.000000 dashadmdv_custom_serializer-0.3.0/custom_serializer/custom_serializer.py
+drwxrwxrwx   0        0        0        0 2023-06-01 19:59:57.479005 dashadmdv_custom_serializer-0.3.0/custom_serializer/encoder/
+-rw-rw-rw-   0        0        0       65 2023-06-01 18:22:41.000000 dashadmdv_custom_serializer-0.3.0/custom_serializer/encoder/__init__.py
+-rw-rw-rw-   0        0        0      525 2023-06-01 18:18:41.000000 dashadmdv_custom_serializer-0.3.0/custom_serializer/encoder/constants.py
+-rw-rw-rw-   0        0        0     8938 2023-06-01 18:19:30.000000 dashadmdv_custom_serializer-0.3.0/custom_serializer/encoder/encoder.py
+-rw-rw-rw-   0        0        0      418 2023-06-01 18:17:06.000000 dashadmdv_custom_serializer-0.3.0/custom_serializer/serializer_factory.py
+drwxrwxrwx   0        0        0        0 2023-06-01 19:59:57.501143 dashadmdv_custom_serializer-0.3.0/custom_serializer/serializers/
+-rw-rw-rw-   0        0        0       63 2023-06-01 18:23:59.000000 dashadmdv_custom_serializer-0.3.0/custom_serializer/serializers/__init__.py
+-rw-rw-rw-   0        0        0     3230 2023-06-01 18:17:53.000000 dashadmdv_custom_serializer-0.3.0/custom_serializer/serializers/json_serializer.py
+-rw-rw-rw-   0        0        0     3226 2023-06-01 18:18:20.000000 dashadmdv_custom_serializer-0.3.0/custom_serializer/serializers/xml_serializer.py
+drwxrwxrwx   0        0        0        0 2023-06-01 19:59:57.532405 dashadmdv_custom_serializer-0.3.0/dashadmdv_custom_serializer.egg-info/
+-rw-rw-rw-   0        0        0      182 2023-06-01 19:59:57.000000 dashadmdv_custom_serializer-0.3.0/dashadmdv_custom_serializer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      584 2023-06-01 19:59:57.000000 dashadmdv_custom_serializer-0.3.0/dashadmdv_custom_serializer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 19:59:57.000000 dashadmdv_custom_serializer-0.3.0/dashadmdv_custom_serializer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-06-01 19:59:57.000000 dashadmdv_custom_serializer-0.3.0/dashadmdv_custom_serializer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 19:59:57.532405 dashadmdv_custom_serializer-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      554 2023-06-01 19:59:53.000000 dashadmdv_custom_serializer-0.3.0/setup.py
```

