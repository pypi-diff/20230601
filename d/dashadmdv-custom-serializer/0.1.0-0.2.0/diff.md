# Comparing `tmp/dashadmdv-custom-serializer-0.1.0.tar.gz` & `tmp/dashadmdv_custom_serializer-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dashadmdv-custom-serializer-0.1.0.tar", last modified: Thu Jun  1 19:10:23 2023, max compression
+gzip compressed data, was "dashadmdv_custom_serializer-0.2.0.tar", last modified: Thu Jun  1 19:48:31 2023, max compression
```

## Comparing `dashadmdv-custom-serializer-0.1.0.tar` & `dashadmdv_custom_serializer-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 19:10:23.202320 dashadmdv-custom-serializer-0.1.0/
--rw-rw-rw-   0        0        0      182 2023-06-01 19:10:23.202320 dashadmdv-custom-serializer-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        5 2023-05-22 20:00:25.000000 dashadmdv-custom-serializer-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 19:10:23.200289 dashadmdv-custom-serializer-0.1.0/dashadmdv_custom_serializer.egg-info/
--rw-rw-rw-   0        0        0      182 2023-06-01 19:10:21.000000 dashadmdv-custom-serializer-0.1.0/dashadmdv_custom_serializer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-06-01 19:10:21.000000 dashadmdv-custom-serializer-0.1.0/dashadmdv_custom_serializer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 19:10:21.000000 dashadmdv-custom-serializer-0.1.0/dashadmdv_custom_serializer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 19:10:21.000000 dashadmdv-custom-serializer-0.1.0/dashadmdv_custom_serializer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 19:10:23.202320 dashadmdv-custom-serializer-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      485 2023-06-01 18:44:14.000000 dashadmdv-custom-serializer-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 19:48:31.514333 dashadmdv_custom_serializer-0.2.0/
+-rw-rw-rw-   0        0        0      182 2023-06-01 19:48:31.514333 dashadmdv_custom_serializer-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0        5 2023-05-22 20:00:25.000000 dashadmdv_custom_serializer-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 19:48:31.498709 dashadmdv_custom_serializer-0.2.0/dashadmdv_custom_serializer.egg-info/
+-rw-rw-rw-   0        0        0      182 2023-06-01 19:48:31.000000 dashadmdv_custom_serializer-0.2.0/dashadmdv_custom_serializer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-06-01 19:48:31.000000 dashadmdv_custom_serializer-0.2.0/dashadmdv_custom_serializer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 19:48:31.000000 dashadmdv_custom_serializer-0.2.0/dashadmdv_custom_serializer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 19:48:31.000000 dashadmdv_custom_serializer-0.2.0/dashadmdv_custom_serializer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 19:48:31.514333 dashadmdv_custom_serializer-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      485 2023-06-01 19:48:13.000000 dashadmdv_custom_serializer-0.2.0/setup.py
```

