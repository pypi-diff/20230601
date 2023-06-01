# Comparing `tmp/siconfig-1.2.tar.gz` & `tmp/siconfig-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "siconfig-1.2.tar", last modified: Thu Jun  1 13:54:23 2023, max compression
+gzip compressed data, was "siconfig-1.3.tar", last modified: Thu Jun  1 15:46:12 2023, max compression
```

## Comparing `siconfig-1.2.tar` & `siconfig-1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 13:54:23.227905 siconfig-1.2/
--rw-rw-rw-   0        0        0       98 2023-06-01 13:54:23.227905 siconfig-1.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-01 13:54:23.228904 siconfig-1.2/setup.cfg
--rw-rw-rw-   0        0        0      164 2023-06-01 13:54:11.000000 siconfig-1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-01 13:54:23.218912 siconfig-1.2/siconfig/
--rw-rw-rw-   0        0        0      351 2023-06-01 12:46:18.000000 siconfig-1.2/siconfig/ErrorTypes.py
--rw-rw-rw-   0        0        0       32 2023-06-01 13:30:40.000000 siconfig-1.2/siconfig/__init__.py
--rw-rw-rw-   0        0        0     3226 2023-06-01 13:53:32.000000 siconfig-1.2/siconfig/siconfig.py
-drwxrwxrwx   0        0        0        0 2023-06-01 13:54:23.225906 siconfig-1.2/siconfig.egg-info/
--rw-rw-rw-   0        0        0       98 2023-06-01 13:54:23.000000 siconfig-1.2/siconfig.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      211 2023-06-01 13:54:23.000000 siconfig-1.2/siconfig.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 13:54:23.000000 siconfig-1.2/siconfig.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-01 13:54:23.000000 siconfig-1.2/siconfig.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-01 15:46:12.175932 siconfig-1.3/
+-rw-rw-rw-   0        0        0       98 2023-06-01 15:46:12.175932 siconfig-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-01 15:46:12.177930 siconfig-1.3/setup.cfg
+-rw-rw-rw-   0        0        0      164 2023-06-01 15:45:33.000000 siconfig-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 15:46:12.165934 siconfig-1.3/siconfig/
+-rw-rw-rw-   0        0        0      351 2023-06-01 12:46:18.000000 siconfig-1.3/siconfig/ErrorTypes.py
+-rw-rw-rw-   0        0        0       32 2023-06-01 13:30:40.000000 siconfig-1.3/siconfig/__init__.py
+-rw-rw-rw-   0        0        0     3233 2023-06-01 15:45:25.000000 siconfig-1.3/siconfig/siconfig.py
+drwxrwxrwx   0        0        0        0 2023-06-01 15:46:12.173934 siconfig-1.3/siconfig.egg-info/
+-rw-rw-rw-   0        0        0       98 2023-06-01 15:46:11.000000 siconfig-1.3/siconfig.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      211 2023-06-01 15:46:11.000000 siconfig-1.3/siconfig.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 15:46:11.000000 siconfig-1.3/siconfig.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-01 15:46:11.000000 siconfig-1.3/siconfig.egg-info/top_level.txt
```

### Comparing `siconfig-1.2/siconfig/siconfig.py` & `siconfig-1.3/siconfig/siconfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,19 +27,19 @@
     def r(self, fpath: str):
         return r"{}".format(fpath)
     
 
     # ОСНОВНЫЕ ФУНКЦИИ
     def init_config(self):
         folder, file = path.split(self.cpath)
-        if not path.exists(self.r(folder)):
-            if '.' in file:
+        if folder != '':
+            if not path.exists(self.r(folder)):
                 makedirs(self.r(folder))
-            else:
-                raise WrongPathError
+        if '.' not in file:
+            raise WrongPathError
         self.status = True
     
     
     @init_check
     def create_config(self, section: str, **pairs):
         with open(self.r(self.cpath), 'w') as cconfig:
             cconfig.write(f'[{section}]\n')
```

