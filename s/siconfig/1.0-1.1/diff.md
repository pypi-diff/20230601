# Comparing `tmp/siconfig-1.0.tar.gz` & `tmp/siconfig-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "siconfig-1.0.tar", last modified: Thu Jun  1 13:36:59 2023, max compression
+gzip compressed data, was "siconfig-1.1.tar", last modified: Thu Jun  1 13:47:44 2023, max compression
```

## Comparing `siconfig-1.0.tar` & `siconfig-1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 13:36:59.615827 siconfig-1.0/
--rw-rw-rw-   0        0        0       98 2023-06-01 13:36:59.615827 siconfig-1.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-01 13:36:59.618827 siconfig-1.0/setup.cfg
--rw-rw-rw-   0        0        0      163 2023-06-01 13:36:26.000000 siconfig-1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-01 13:36:59.601835 siconfig-1.0/siconfig/
--rw-rw-rw-   0        0        0      351 2023-06-01 12:46:18.000000 siconfig-1.0/siconfig/ErrorTypes.py
--rw-rw-rw-   0        0        0       32 2023-06-01 13:30:40.000000 siconfig-1.0/siconfig/__init__.py
--rw-rw-rw-   0        0        0     2709 2023-06-01 13:28:45.000000 siconfig-1.0/siconfig/siconfig.py
-drwxrwxrwx   0        0        0        0 2023-06-01 13:36:59.613829 siconfig-1.0/siconfig.egg-info/
--rw-rw-rw-   0        0        0       98 2023-06-01 13:36:59.000000 siconfig-1.0/siconfig.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      211 2023-06-01 13:36:59.000000 siconfig-1.0/siconfig.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 13:36:59.000000 siconfig-1.0/siconfig.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-01 13:36:59.000000 siconfig-1.0/siconfig.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-01 13:47:44.586476 siconfig-1.1/
+-rw-rw-rw-   0        0        0       98 2023-06-01 13:47:44.587475 siconfig-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-01 13:47:44.588475 siconfig-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      163 2023-06-01 13:47:29.000000 siconfig-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 13:47:44.575485 siconfig-1.1/siconfig/
+-rw-rw-rw-   0        0        0      351 2023-06-01 12:46:18.000000 siconfig-1.1/siconfig/ErrorTypes.py
+-rw-rw-rw-   0        0        0       32 2023-06-01 13:30:40.000000 siconfig-1.1/siconfig/__init__.py
+-rw-rw-rw-   0        0        0     3181 2023-06-01 13:46:29.000000 siconfig-1.1/siconfig/siconfig.py
+drwxrwxrwx   0        0        0        0 2023-06-01 13:47:44.585476 siconfig-1.1/siconfig.egg-info/
+-rw-rw-rw-   0        0        0       98 2023-06-01 13:47:44.000000 siconfig-1.1/siconfig.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      211 2023-06-01 13:47:44.000000 siconfig-1.1/siconfig.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 13:47:44.000000 siconfig-1.1/siconfig.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-01 13:47:44.000000 siconfig-1.1/siconfig.egg-info/top_level.txt
```

### Comparing `siconfig-1.0/siconfig/siconfig.py` & `siconfig-1.1/siconfig/siconfig.py`

 * *Files 6% similar despite different names*

```diff
@@ -79,8 +79,21 @@
                     old_data.append(line.replace('\n', ''))
                 else:
                     line = line.split('=')
                     old_data.append(f'{line[0]}={value}')
         remove(self.r(self.cpath))
         with open(self.r(self.cpath), 'w') as cconfig:
             for new_data in old_data:
+                cconfig.write(f'{new_data}\n')
+    
+    
+    @init_check
+    def remove_key(self, key: str):
+        old_data = list()
+        with open(self.r(self.cpath), 'r') as cconfig:
+            for line in cconfig.readlines():
+                if not key in line:
+                    old_data.append(line.replace('\n', ''))
+        remove(self.r(self.cpath))
+        with open(self.r(self.cpath), 'w') as cconfig:
+            for new_data in old_data:
                 cconfig.write(f'{new_data}\n')
```

