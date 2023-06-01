# Comparing `tmp/Baozun-Winrobot-0.0.1.tar.gz` & `tmp/baozun_winrobot-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Baozun-Winrobot-0.0.1.tar", last modified: Thu Jun  1 08:19:05 2023, max compression
+gzip compressed data, was "dist/baozun_winrobot-0.0.2.tar", last modified: Thu Jun  1 10:23:19 2023, max compression
```

## Comparing `Baozun-Winrobot-0.0.1.tar` & `baozun_winrobot-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,11 @@
-drwxr-xr-x   0 wcgz-dz-100285   (501) staff       (20)        0 2023-06-01 08:19:05.613318 Baozun-Winrobot-0.0.1/
-drwxr-xr-x   0 wcgz-dz-100285   (501) staff       (20)        0 2023-06-01 08:19:05.612498 Baozun-Winrobot-0.0.1/Baozun_Winrobot.egg-info/
--rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)       81 2023-06-01 08:19:05.000000 Baozun-Winrobot-0.0.1/Baozun_Winrobot.egg-info/PKG-INFO
--rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)      202 2023-06-01 08:19:05.000000 Baozun-Winrobot-0.0.1/Baozun_Winrobot.egg-info/SOURCES.txt
--rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)        1 2023-06-01 08:19:05.000000 Baozun-Winrobot-0.0.1/Baozun_Winrobot.egg-info/dependency_links.txt
--rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)        1 2023-06-01 08:06:03.000000 Baozun-Winrobot-0.0.1/Baozun_Winrobot.egg-info/not-zip-safe
--rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)        1 2023-06-01 08:19:05.000000 Baozun-Winrobot-0.0.1/Baozun_Winrobot.egg-info/top_level.txt
--rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)       81 2023-06-01 08:19:05.612996 Baozun-Winrobot-0.0.1/PKG-INFO
--rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)       38 2023-06-01 08:19:05.613416 Baozun-Winrobot-0.0.1/setup.cfg
--rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)      283 2023-06-01 08:18:59.000000 Baozun-Winrobot-0.0.1/setup.py
+drwxr-xr-x   0 wcgz-dz-100285   (501) staff       (20)        0 2023-06-01 10:23:19.469315 baozun_winrobot-0.0.2/
+drwxr-xr-x   0 wcgz-dz-100285   (501) staff       (20)        0 2023-06-01 10:23:19.467274 baozun_winrobot-0.0.2/Baozun_Winrobot.egg-info/
+-rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)       81 2023-06-01 10:23:19.000000 baozun_winrobot-0.0.2/Baozun_Winrobot.egg-info/PKG-INFO
+-rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)      406 2023-06-01 10:23:19.000000 baozun_winrobot-0.0.2/Baozun_Winrobot.egg-info/SOURCES.txt
+-rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)        1 2023-06-01 10:23:19.000000 baozun_winrobot-0.0.2/Baozun_Winrobot.egg-info/dependency_links.txt
+-rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)        1 2023-06-01 08:06:03.000000 baozun_winrobot-0.0.2/Baozun_Winrobot.egg-info/not-zip-safe
+-rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)        1 2023-06-01 10:23:19.000000 baozun_winrobot-0.0.2/Baozun_Winrobot.egg-info/top_level.txt
+-rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)       81 2023-06-01 10:23:19.468204 baozun_winrobot-0.0.2/PKG-INFO
+-rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)       11 2023-06-01 10:21:00.000000 baozun_winrobot-0.0.2/README.md
+-rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)       38 2023-06-01 10:23:19.469538 baozun_winrobot-0.0.2/setup.cfg
+-rw-r--r--   0 wcgz-dz-100285   (501) staff       (20)      283 2023-06-01 10:22:17.000000 baozun_winrobot-0.0.2/setup.py
```

