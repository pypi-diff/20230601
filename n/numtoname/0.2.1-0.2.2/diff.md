# Comparing `tmp/numtoname-0.2.1.tar.gz` & `tmp/numtoname-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numtoname-0.2.1.tar", last modified: Thu Jun  1 07:14:06 2023, max compression
+gzip compressed data, was "numtoname-0.2.2.tar", last modified: Thu Jun  1 07:21:07 2023, max compression
```

## Comparing `numtoname-0.2.1.tar` & `numtoname-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 07:14:06.900595 numtoname-0.2.1/
--rw-rw-rw-   0        0        0     1088 2023-05-25 23:57:32.000000 numtoname-0.2.1/LICENSE.txt
--rw-rw-rw-   0        0        0      693 2023-06-01 07:14:06.900595 numtoname-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      116 2023-05-26 00:55:44.000000 numtoname-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 07:14:06.881595 numtoname-0.2.1/numtoname/
--rw-rw-rw-   0        0        0     1092 2023-05-31 19:21:40.000000 numtoname-0.2.1/numtoname/__init__.py
--rw-rw-rw-   0        0        0    17206 2023-06-01 06:58:19.000000 numtoname-0.2.1/numtoname/functions.py
--rw-rw-rw-   0        0        0    12926 2023-06-01 07:08:40.000000 numtoname-0.2.1/numtoname/tests.py
-drwxrwxrwx   0        0        0        0 2023-06-01 07:14:06.898596 numtoname-0.2.1/numtoname.egg-info/
--rw-rw-rw-   0        0        0      693 2023-06-01 07:14:06.000000 numtoname-0.2.1/numtoname.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-06-01 07:14:06.000000 numtoname-0.2.1/numtoname.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 07:14:06.000000 numtoname-0.2.1/numtoname.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-01 07:14:06.000000 numtoname-0.2.1/numtoname.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-01 07:14:06.903596 numtoname-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1078 2023-06-01 07:12:28.000000 numtoname-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 07:21:07.927036 numtoname-0.2.2/
+-rw-rw-rw-   0        0        0     1088 2023-05-25 23:57:32.000000 numtoname-0.2.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      693 2023-06-01 07:21:07.927036 numtoname-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      116 2023-05-26 00:55:44.000000 numtoname-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 07:21:07.902015 numtoname-0.2.2/numtoname/
+-rw-rw-rw-   0        0        0     1092 2023-05-31 19:21:40.000000 numtoname-0.2.2/numtoname/__init__.py
+-rw-rw-rw-   0        0        0    17206 2023-06-01 07:19:40.000000 numtoname-0.2.2/numtoname/functions.py
+-rw-rw-rw-   0        0        0    12926 2023-06-01 07:08:40.000000 numtoname-0.2.2/numtoname/tests.py
+drwxrwxrwx   0        0        0        0 2023-06-01 07:21:07.924031 numtoname-0.2.2/numtoname.egg-info/
+-rw-rw-rw-   0        0        0      693 2023-06-01 07:21:07.000000 numtoname-0.2.2/numtoname.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-06-01 07:21:07.000000 numtoname-0.2.2/numtoname.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 07:21:07.000000 numtoname-0.2.2/numtoname.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-01 07:21:07.000000 numtoname-0.2.2/numtoname.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-01 07:21:07.930034 numtoname-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1078 2023-06-01 07:16:56.000000 numtoname-0.2.2/setup.py
```

### Comparing `numtoname-0.2.1/LICENSE.txt` & `numtoname-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `numtoname-0.2.1/PKG-INFO` & `numtoname-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: numtoname
-Version: 0.2.1
+Version: 0.2.2
 Summary: A python module to convert a number or list of numbers into a variable name or list of variable names
 Home-page: https://github.com/benjaminmesser/Numtoname
-Download-URL: https://github.com/benjaminmesser/Numtoname/archive/v_021.tar.gz
+Download-URL: https://github.com/benjaminmesser/Numtoname/archive/v_022.tar.gz
 Author: Ben Messer
 Author-email: benjamin.messer@outlook.com
 License: MIT
 Keywords: tools,development,naming
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `numtoname-0.2.1/numtoname/__init__.py` & `numtoname-0.2.2/numtoname/__init__.py`

 * *Files identical despite different names*

### Comparing `numtoname-0.2.1/numtoname/functions.py` & `numtoname-0.2.2/numtoname/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
                 break
         
         num += skipped_name_count
 
     return base_generate_name_fixed(num, alphabet, name_length)
 
 
-def generate_names_fixed(alphabet: str, name_length: int, invalid_names: list[str] = None, start_num: int = -1, end_num: int = -1, num_list: list[int] = None, warnings: bool = True) -> list[str]:
+def generate_names_fixed(alphabet: str, name_length: int, start_num: int = -1, end_num: int = -1, num_list: list[int] = None, invalid_names: list[str] = None, warnings: bool = True) -> list[str]:
     if alphabet is None or len(alphabet) < 1 or name_length < 1:
         return []
     
     if (start_num < 1 or start_num > end_num) and (num_list is None or len(num_list) < 1):
         return []
     
     if num_list is not None and (start_num != -1 or end_num != -1):  # Ensure that we have either start_num and end_num or num_list, not both
@@ -143,15 +143,15 @@
             running_total += len(alphabet) ** name_length
         else:
             break
     
     return base_generate_name_fixed(num - last_running_total, alphabet, name_length)
 
 
-def generate_names(alphabet: str, invalid_names: list[str] = None, start_num: int = -1, end_num: int = -1, num_list: list[int] = None, warnings: bool = True) -> list[str]:
+def generate_names(alphabet: str, start_num: int = -1, end_num: int = -1, num_list: list[int] = None, invalid_names: list[str] = None, warnings: bool = True) -> list[str]:
     if alphabet is None or len(alphabet) < 1:
         return []
     
     if (start_num < 1 or start_num > end_num) and (num_list is None or len(num_list) < 1):
         return []
     
     if num_list is not None and (start_num != -1 or end_num != -1):  # Ensure that we have either start_num and end_num or num_list, not both
@@ -169,65 +169,65 @@
 
 
 def generate_name_fixed_alpha(num: int, name_length: int, invalid_names: list[str] = None, warnings: bool = True) -> str:
     alphabet = 'abcdefghijklmnopqrstuvwxyz'
     return generate_name_fixed(num, alphabet, name_length, invalid_names = invalid_names, warnings = warnings)
 
 
-def generate_names_fixed_alpha(name_length: int, invalid_names: list[str] = None, start_num: int = -1, end_num: int = -1, num_list: list[int] = None, warnings: bool = True) -> list[str]:
+def generate_names_fixed_alpha(name_length: int, start_num: int = -1, end_num: int = -1, num_list: list[int] = None, invalid_names: list[str] = None, warnings: bool = True) -> list[str]:
     alphabet = 'abcdefghijklmnopqrstuvwxyz'
     return generate_names_fixed(alphabet, name_length, invalid_names = invalid_names, start_num = start_num, end_num = end_num, num_list = num_list, warnings = warnings)
     
 
 def generate_name_alpha(num: int, invalid_names: list[str] = None, warnings: bool = True) -> str:
     alphabet = 'abcdefghijklmnopqrstuvwxyz'
     return generate_name(num, alphabet, invalid_names = invalid_names, warnings = warnings)
 
 
-def generate_names_alpha(invalid_names: list[str] = None, start_num: int = -1, end_num: int = -1, num_list: list[int] = None, warnings: bool = True) -> list[str]:
+def generate_names_alpha(start_num: int = -1, end_num: int = -1, num_list: list[int] = None, invalid_names: list[str] = None, warnings: bool = True) -> list[str]:
     alphabet = 'abcdefghijklmnopqrstuvwxyz'
     return generate_names(alphabet, invalid_names = invalid_names, start_num = start_num, end_num = end_num, num_list = num_list, warnings = warnings)
 
 
 def generate_name_fixed_alpha2(num: int, name_length: int, invalid_names: list[str] = None, warnings: bool = True) -> str:
     alphabet = 'ABCDEFGHIJKLMNOPQRSTUVWXYZ'
     return generate_name_fixed(num, alphabet, name_length, invalid_names = invalid_names, warnings = warnings)
 
 
-def generate_names_fixed_alpha2(name_length: int, invalid_names: list[str] = None, start_num: int = -1, end_num: int = -1, num_list: list[int] = None, warnings: bool = True) -> list[str]:
+def generate_names_fixed_alpha2(name_length: int, start_num: int = -1, end_num: int = -1, num_list: list[int] = None, invalid_names: list[str] = None, warnings: bool = True) -> list[str]:
     alphabet = 'ABCDEFGHIJKLMNOPQRSTUVWXYZ'
     return generate_names_fixed(alphabet, name_length, invalid_names = invalid_names, start_num = start_num, end_num = end_num, num_list = num_list, warnings = warnings)
     
 
 def generate_name_alpha2(num: int, invalid_names: list[str] = None, warnings: bool = True) -> str:
     alphabet = 'ABCDEFGHIJKLMNOPQRSTUVWXYZ'
     return generate_name(num, alphabet, invalid_names = invalid_names, warnings = warnings)
 
 
-def generate_names_alpha2(invalid_names: list[str] = None, start_num: int = -1, end_num: int = -1, num_list: list[int] = None, warnings: bool = True) -> list[str]:
+def generate_names_alpha2(start_num: int = -1, end_num: int = -1, num_list: list[int] = None, invalid_names: list[str] = None, warnings: bool = True) -> list[str]:
     alphabet = 'ABCDEFGHIJKLMNOPQRSTUVWXYZ'
     return generate_names(alphabet, invalid_names = invalid_names, start_num = start_num, end_num = end_num, num_list = num_list, warnings = warnings)
 
 
 def generate_name_fixed_alpha3(num: int, name_length: int, invalid_names: list[str] = None, warnings: bool = True) -> str:
     alphabet = 'aAbBcCdDeEfFgGhHiIjJkKlLmMnNoOpPqQrRsStTuUvVwWxXyYzZ'
     return generate_name_fixed(num, alphabet, name_length, invalid_names = invalid_names, warnings = warnings)
 
 
-def generate_names_fixed_alpha3(name_length: int, invalid_names: list[str] = None, start_num: int = -1, end_num: int = -1, num_list: list[int] = None, warnings: bool = True) -> list[str]:
+def generate_names_fixed_alpha3(name_length: int, start_num: int = -1, end_num: int = -1, num_list: list[int] = None, invalid_names: list[str] = None, warnings: bool = True) -> list[str]:
     alphabet = 'aAbBcCdDeEfFgGhHiIjJkKlLmMnNoOpPqQrRsStTuUvVwWxXyYzZ'
     return generate_names_fixed(alphabet, name_length, invalid_names = invalid_names, start_num = start_num, end_num = end_num, num_list = num_list, warnings = warnings)
     
 
 def generate_name_alpha3(num: int, invalid_names: list[str] = None, warnings: bool = True) -> str:
     alphabet = 'aAbBcCdDeEfFgGhHiIjJkKlLmMnNoOpPqQrRsStTuUvVwWxXyYzZ'
     return generate_name(num, alphabet, invalid_names = invalid_names, warnings = warnings)
 
 
-def generate_names_alpha3(invalid_names: list[str] = None, start_num: int = -1, end_num: int = -1, num_list: list[int] = None, warnings: bool = True) -> list[str]:
+def generate_names_alpha3(start_num: int = -1, end_num: int = -1, num_list: list[int] = None, invalid_names: list[str] = None, warnings: bool = True) -> list[str]:
     alphabet = 'aAbBcCdDeEfFgGhHiIjJkKlLmMnNoOpPqQrRsStTuUvVwWxXyYzZ'
     return generate_names(alphabet, invalid_names = invalid_names, start_num = start_num, end_num = end_num, num_list = num_list, warnings = warnings)
 
 
 def num_from_name_fixed(name: str, alphabet: str, name_length: int, invalid_names: list[str] = None, warnings: bool = True) -> int:
     if name is None or len(name) < 1 or alphabet is None or len(alphabet) < 1 or name_length < 1:
         return -1
```

### Comparing `numtoname-0.2.1/numtoname/tests.py` & `numtoname-0.2.2/numtoname/tests.py`

 * *Files identical despite different names*

### Comparing `numtoname-0.2.1/numtoname.egg-info/PKG-INFO` & `numtoname-0.2.2/numtoname.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: numtoname
-Version: 0.2.1
+Version: 0.2.2
 Summary: A python module to convert a number or list of numbers into a variable name or list of variable names
 Home-page: https://github.com/benjaminmesser/Numtoname
-Download-URL: https://github.com/benjaminmesser/Numtoname/archive/v_021.tar.gz
+Download-URL: https://github.com/benjaminmesser/Numtoname/archive/v_022.tar.gz
 Author: Ben Messer
 Author-email: benjamin.messer@outlook.com
 License: MIT
 Keywords: tools,development,naming
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `numtoname-0.2.1/setup.py` & `numtoname-0.2.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from distutils.core import setup
 setup(
   name = 'numtoname',         # How you named your package folder (MyLib)
   packages = ['numtoname'],   # Chose the same as "name"
-  version = '0.2.1',
+  version = '0.2.2',
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'A python module to convert a number or list of numbers into a variable name or list of variable names',
   author = 'Ben Messer',
   author_email = 'benjamin.messer@outlook.com',
   url = 'https://github.com/benjaminmesser/Numtoname',
-  download_url = 'https://github.com/benjaminmesser/Numtoname/archive/v_021.tar.gz',
+  download_url = 'https://github.com/benjaminmesser/Numtoname/archive/v_022.tar.gz',
   keywords = ['tools', 'development', 'naming'],
   install_requires=[],
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',
```

