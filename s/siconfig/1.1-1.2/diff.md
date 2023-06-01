# Comparing `tmp/siconfig-1.1.tar.gz` & `tmp/siconfig-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "siconfig-1.1.tar", last modified: Thu Jun  1 13:47:44 2023, max compression
+gzip compressed data, was "siconfig-1.2.tar", last modified: Thu Jun  1 13:54:23 2023, max compression
```

## Comparing `siconfig-1.1.tar` & `siconfig-1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 13:47:44.586476 siconfig-1.1/
--rw-rw-rw-   0        0        0       98 2023-06-01 13:47:44.587475 siconfig-1.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-01 13:47:44.588475 siconfig-1.1/setup.cfg
--rw-rw-rw-   0        0        0      163 2023-06-01 13:47:29.000000 siconfig-1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-01 13:47:44.575485 siconfig-1.1/siconfig/
--rw-rw-rw-   0        0        0      351 2023-06-01 12:46:18.000000 siconfig-1.1/siconfig/ErrorTypes.py
--rw-rw-rw-   0        0        0       32 2023-06-01 13:30:40.000000 siconfig-1.1/siconfig/__init__.py
--rw-rw-rw-   0        0        0     3181 2023-06-01 13:46:29.000000 siconfig-1.1/siconfig/siconfig.py
-drwxrwxrwx   0        0        0        0 2023-06-01 13:47:44.585476 siconfig-1.1/siconfig.egg-info/
--rw-rw-rw-   0        0        0       98 2023-06-01 13:47:44.000000 siconfig-1.1/siconfig.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      211 2023-06-01 13:47:44.000000 siconfig-1.1/siconfig.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 13:47:44.000000 siconfig-1.1/siconfig.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-01 13:47:44.000000 siconfig-1.1/siconfig.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-01 13:54:23.227905 siconfig-1.2/
+-rw-rw-rw-   0        0        0       98 2023-06-01 13:54:23.227905 siconfig-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-01 13:54:23.228904 siconfig-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      164 2023-06-01 13:54:11.000000 siconfig-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 13:54:23.218912 siconfig-1.2/siconfig/
+-rw-rw-rw-   0        0        0      351 2023-06-01 12:46:18.000000 siconfig-1.2/siconfig/ErrorTypes.py
+-rw-rw-rw-   0        0        0       32 2023-06-01 13:30:40.000000 siconfig-1.2/siconfig/__init__.py
+-rw-rw-rw-   0        0        0     3226 2023-06-01 13:53:32.000000 siconfig-1.2/siconfig/siconfig.py
+drwxrwxrwx   0        0        0        0 2023-06-01 13:54:23.225906 siconfig-1.2/siconfig.egg-info/
+-rw-rw-rw-   0        0        0       98 2023-06-01 13:54:23.000000 siconfig-1.2/siconfig.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      211 2023-06-01 13:54:23.000000 siconfig-1.2/siconfig.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 13:54:23.000000 siconfig-1.2/siconfig.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-01 13:54:23.000000 siconfig-1.2/siconfig.egg-info/top_level.txt
```

### Comparing `siconfig-1.1/siconfig/siconfig.py` & `siconfig-1.2/siconfig/siconfig.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,20 +56,21 @@
                 if regex.search(line) == None:
                     self.update_result(result, line)
         return result
     
     
     @init_check
     def get_key(self, key: str):
-        result = dict()
+        result = str()
         regex = re.compile(r'\[(.*?)\]')
         with open(self.r(self.cpath), 'r') as cconfig:
             for line in cconfig.readlines():
                 if regex.search(line) == None and key in line:
-                    self.update_result(result, line)
+                    line = line.split('=')
+                    result = line[1].replace('\n', '')
                     break
         return result
     
     
     @init_check
     def set_key(self, key: str, value: str):
         old_data = list()
```

