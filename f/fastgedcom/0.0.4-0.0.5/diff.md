# Comparing `tmp/fastgedcom-0.0.4.tar.gz` & `tmp/fastgedcom-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastgedcom-0.0.4.tar", last modified: Fri May 26 20:37:58 2023, max compression
+gzip compressed data, was "fastgedcom-0.0.5.tar", last modified: Thu Jun  1 19:20:02 2023, max compression
```

## Comparing `fastgedcom-0.0.4.tar` & `fastgedcom-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 20:37:58.297807 fastgedcom-0.0.4/
--rw-rw-rw-   0        0        0     1090 2023-05-22 23:10:18.000000 fastgedcom-0.0.4/LICENSE
--rw-rw-rw-   0        0        0       24 2023-05-25 13:57:11.000000 fastgedcom-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     3874 2023-05-26 20:37:58.296810 fastgedcom-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3030 2023-05-26 20:32:34.000000 fastgedcom-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 20:37:58.274048 fastgedcom-0.0.4/fastgedcom/
--rw-rw-rw-   0        0        0      236 2023-05-26 17:04:30.000000 fastgedcom-0.0.4/fastgedcom/__init__.py
--rw-rw-rw-   0        0        0     6908 2023-05-26 17:50:33.000000 fastgedcom-0.0.4/fastgedcom/base.py
--rw-rw-rw-   0        0        0     5045 2023-05-26 17:07:54.000000 fastgedcom-0.0.4/fastgedcom/family_aid.py
--rw-rw-rw-   0        0        0     5508 2023-05-26 17:11:25.000000 fastgedcom-0.0.4/fastgedcom/helpers.py
--rw-rw-rw-   0        0        0     2858 2023-05-26 16:55:14.000000 fastgedcom-0.0.4/fastgedcom/parser.py
--rw-rw-rw-   0        0        0        0 2023-05-25 13:48:45.000000 fastgedcom-0.0.4/fastgedcom/py.typed
-drwxrwxrwx   0        0        0        0 2023-05-26 20:37:58.294808 fastgedcom-0.0.4/fastgedcom.egg-info/
--rw-rw-rw-   0        0        0     3874 2023-05-26 20:37:58.000000 fastgedcom-0.0.4/fastgedcom.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      370 2023-05-26 20:37:58.000000 fastgedcom-0.0.4/fastgedcom.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 20:37:58.000000 fastgedcom-0.0.4/fastgedcom.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-26 20:37:58.000000 fastgedcom-0.0.4/fastgedcom.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       24 2023-05-26 20:37:58.000000 fastgedcom-0.0.4/fastgedcom.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-26 20:37:58.000000 fastgedcom-0.0.4/fastgedcom.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-26 20:37:58.297807 fastgedcom-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1312 2023-05-26 20:21:00.000000 fastgedcom-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 19:20:02.447515 fastgedcom-0.0.5/
+-rw-rw-rw-   0        0        0     1090 2023-05-22 23:10:18.000000 fastgedcom-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0       24 2023-05-25 13:57:11.000000 fastgedcom-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     4231 2023-06-01 19:20:02.447515 fastgedcom-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3312 2023-06-01 19:19:11.000000 fastgedcom-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 19:20:02.394227 fastgedcom-0.0.5/fastgedcom/
+-rw-rw-rw-   0        0        0        0 2023-06-01 18:47:09.000000 fastgedcom-0.0.5/fastgedcom/__init__.py
+-rw-rw-rw-   0        0        0     9376 2023-06-01 18:47:09.000000 fastgedcom-0.0.5/fastgedcom/base.py
+-rw-rw-rw-   0        0        0     7607 2023-06-01 18:47:09.000000 fastgedcom-0.0.5/fastgedcom/family_aid.py
+-rw-rw-rw-   0        0        0     6033 2023-06-01 18:47:09.000000 fastgedcom-0.0.5/fastgedcom/helpers.py
+-rw-rw-rw-   0        0        0     4055 2023-06-01 18:47:09.000000 fastgedcom-0.0.5/fastgedcom/parser.py
+-rw-rw-rw-   0        0        0        0 2023-05-25 13:48:45.000000 fastgedcom-0.0.5/fastgedcom/py.typed
+drwxrwxrwx   0        0        0        0 2023-06-01 19:20:02.429462 fastgedcom-0.0.5/fastgedcom.egg-info/
+-rw-rw-rw-   0        0        0     4231 2023-06-01 19:20:01.000000 fastgedcom-0.0.5/fastgedcom.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      455 2023-06-01 19:20:02.000000 fastgedcom-0.0.5/fastgedcom.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 19:20:01.000000 fastgedcom-0.0.5/fastgedcom.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-01 19:12:40.000000 fastgedcom-0.0.5/fastgedcom.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       56 2023-06-01 19:20:01.000000 fastgedcom-0.0.5/fastgedcom.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-01 19:20:01.000000 fastgedcom-0.0.5/fastgedcom.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 19:20:02.447515 fastgedcom-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1408 2023-06-01 19:17:07.000000 fastgedcom-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 19:20:02.437001 fastgedcom-0.0.5/test/
+-rw-rw-rw-   0        0        0      581 2023-06-01 18:47:09.000000 fastgedcom-0.0.5/test/test_base.py
+-rw-rw-rw-   0        0        0     3630 2023-06-01 18:47:09.000000 fastgedcom-0.0.5/test/test_date_helpers.py
+-rw-rw-rw-   0        0        0      592 2023-06-01 18:47:09.000000 fastgedcom-0.0.5/test/test_helpers.py
+-rw-rw-rw-   0        0        0     2758 2023-06-01 18:47:09.000000 fastgedcom-0.0.5/test/test_parser.py
```

### Comparing `fastgedcom-0.0.4/LICENSE` & `fastgedcom-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fastgedcom-0.0.4/PKG-INFO` & `fastgedcom-0.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,117 +1,124 @@
 Metadata-Version: 2.1
 Name: fastgedcom
-Version: 0.0.4
-Summary: A gedcom tool to parse, browse and modify gedcom files
-Home-page: https://github.com/GatienBouyer/fastgedcom
+Version: 0.0.5
+Summary: A lightweight tool to parse, browse and edit gedcom files.
 Author: Gatien Bouyer
 Author-email: gatien.bouyer.dev@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/GatienBouyer/fastgedcom/issues
 Project-URL: Source, https://github.com/GatienBouyer/fastgedcom
+Project-URL: Documentation, https://fastgedcom.readthedocs.io/en/latest/
 Keywords: fastgedcom gedcom parser genealogy
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Sociology :: Genealogy
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # FastGedcom
 
-A gedcom tool to parse, browse and modify gedcom files
+A lightweight tool to parse, browse and edit gedcom files.
 
 ```bash
 pip install fastgedcom
 ```
 
 Want to open a gedcom file?
 ```python
 from fastgedcom.parser import guess_encoding, parse
 
 gedcom_file = "my_gedcom_file.ged"
 with open(gedcom_file, "r", encoding=guess_encoding(gedcom_file)) as f:
 	document, warnings = parse(f)
 
-print(warnings) # in case of duplicate record reference
+if warnings: print(warnings) # in case of duplicate record reference
 ```
 
 
-Simple to write! Free to chose the fields, the data, and the formatting.
+Easy to write! Free choice of fields, data, and formatting.
 ```python
 from fastgedcom.helpers import format_date
 
 birth_date = (document["@I1@"] > "BIRT") >= "DATE"
 print(format_date(birth_date))
 ```
 
 A field is missing? FakeLine to the rescue. Like a TrueLine, but no error, no value, and no error handling code!
 ```python
 from fastgedcom.base import is_true
 
-indi = document["@I1"]
+indi = document["@I1@"]
 death_date = (indi > "DEAT") >= "DATE"
 if death_date != "": print(format_date(death_date)) 
-if not is_true(indi): print("It was not even present!")
+if not is_true(indi): print("@I1@ was not even present!")
 ```
 
 Don't like magic operator overload? Use standard methods!
 ```python
 indi = document.get_record("@I1@")
 surname = indi.get_sub_line("NAME").get_sub_line_payload("SURN")
 ```
 
-Typehints for salvation!
+Typehints for salvation! Autocompletion and type checking make development so much easier.
 ```python
 from fastgedcom.base import Document, FakeLine, IndiRef, Record, is_true
 from fastgedcom.helpers import format_name
 
 def print_infos(gedcom: Document, indi: IndiRef) -> None:
 	record = gedcom[indi]
 	if is_true(record): print_name(record)
 
 def print_name(record: Record | FakeLine) -> None:
 	print(format_name(record >= "NAME"))
 
 print_infos(document, "@I1@")
 ```
 
-Iteration on families is fast. Don't blink!
+Iteration on families is fast. Save time!
 ```python
 from fastgedcom.family_aid import FamilyAid
 
 booster = FamilyAid(document)
 
 def number_of_ascendants(indi: Record | FakeLine) -> int:
 	if not is_true(indi): return 1
 	father, mother = booster.get_parents(indi.tag)
 	return 1+max(number_of_ascendants(father), number_of_ascendants(mother))
 
 def number_of_descendants(indi: IndiRef) -> int:
-	children = booster.get_children(indi)
+	children = booster.get_children_ref(indi)
 	return len(children) + sum(number_of_descendants(c) for c in children)
 
-print(number_of_ascendants(document["@I1@"]))
-print(number_of_descendants("@I1@"))
+print(max(number_of_ascendants(indi)
+	for indi in document.get_records("INDI")
+))
+print(max(number_of_descendants(indi.tag)
+	for indi in document.get_records("INDI")
+))
 ```
 
 You want to see more? [Here are some examples](https://github.com/GatienBouyer/fastgedcom/tree/main/examples)
 
-I promise you it is fast! I [test it](https://github.com/GatienBouyer/fastgedcom/tree/main/benchmarks) and I use it.
+The documentation of FastGedcom is available [here](https://fastgedcom.readthedocs.io/en/latest/) on ReadTheDocs.
+
+I promise you it is efficient! I [test it](https://github.com/GatienBouyer/fastgedcom/tree/main/benchmarks) and I use it.
 
 
 
 ## Feature details
 
-- Supports the read of gedcom files encoded in UTF-8 with and without BOM, UTF-16 (also named UNICODE), ANSI, and ANSEL.
-- ~~Supports the export to gedcom files encoded in UTF-8, UTF-16, and ANSI.~~
+- Supports reading of gedcom files encoded in UTF-8 with and without BOM, UTF-16 (also named UNICODE), ANSI, and ANSEL.
+- ~~Supports export of gedcom files encoded in UTF-8, UTF-16, and ANSI.~~
 
 ## Feedbacks
 
 Feedbacks are welcome, and they will be greatly appreciated!
 
 If you like this project, consider putting a star on [Github](https://github.com/GatienBouyer/fastgedcom), thank you!
```

### Comparing `fastgedcom-0.0.4/README.md` & `fastgedcom-0.0.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,95 +1,101 @@
 # FastGedcom
 
-A gedcom tool to parse, browse and modify gedcom files
+A lightweight tool to parse, browse and edit gedcom files.
 
 ```bash
 pip install fastgedcom
 ```
 
 Want to open a gedcom file?
 ```python
 from fastgedcom.parser import guess_encoding, parse
 
 gedcom_file = "my_gedcom_file.ged"
 with open(gedcom_file, "r", encoding=guess_encoding(gedcom_file)) as f:
 	document, warnings = parse(f)
 
-print(warnings) # in case of duplicate record reference
+if warnings: print(warnings) # in case of duplicate record reference
 ```
 
 
-Simple to write! Free to chose the fields, the data, and the formatting.
+Easy to write! Free choice of fields, data, and formatting.
 ```python
 from fastgedcom.helpers import format_date
 
 birth_date = (document["@I1@"] > "BIRT") >= "DATE"
 print(format_date(birth_date))
 ```
 
 A field is missing? FakeLine to the rescue. Like a TrueLine, but no error, no value, and no error handling code!
 ```python
 from fastgedcom.base import is_true
 
-indi = document["@I1"]
+indi = document["@I1@"]
 death_date = (indi > "DEAT") >= "DATE"
 if death_date != "": print(format_date(death_date)) 
-if not is_true(indi): print("It was not even present!")
+if not is_true(indi): print("@I1@ was not even present!")
 ```
 
 Don't like magic operator overload? Use standard methods!
 ```python
 indi = document.get_record("@I1@")
 surname = indi.get_sub_line("NAME").get_sub_line_payload("SURN")
 ```
 
-Typehints for salvation!
+Typehints for salvation! Autocompletion and type checking make development so much easier.
 ```python
 from fastgedcom.base import Document, FakeLine, IndiRef, Record, is_true
 from fastgedcom.helpers import format_name
 
 def print_infos(gedcom: Document, indi: IndiRef) -> None:
 	record = gedcom[indi]
 	if is_true(record): print_name(record)
 
 def print_name(record: Record | FakeLine) -> None:
 	print(format_name(record >= "NAME"))
 
 print_infos(document, "@I1@")
 ```
 
-Iteration on families is fast. Don't blink!
+Iteration on families is fast. Save time!
 ```python
 from fastgedcom.family_aid import FamilyAid
 
 booster = FamilyAid(document)
 
 def number_of_ascendants(indi: Record | FakeLine) -> int:
 	if not is_true(indi): return 1
 	father, mother = booster.get_parents(indi.tag)
 	return 1+max(number_of_ascendants(father), number_of_ascendants(mother))
 
 def number_of_descendants(indi: IndiRef) -> int:
-	children = booster.get_children(indi)
+	children = booster.get_children_ref(indi)
 	return len(children) + sum(number_of_descendants(c) for c in children)
 
-print(number_of_ascendants(document["@I1@"]))
-print(number_of_descendants("@I1@"))
+print(max(number_of_ascendants(indi)
+	for indi in document.get_records("INDI")
+))
+print(max(number_of_descendants(indi.tag)
+	for indi in document.get_records("INDI")
+))
 ```
 
 You want to see more? [Here are some examples](https://github.com/GatienBouyer/fastgedcom/tree/main/examples)
 
-I promise you it is fast! I [test it](https://github.com/GatienBouyer/fastgedcom/tree/main/benchmarks) and I use it.
+The documentation of FastGedcom is available [here](https://fastgedcom.readthedocs.io/en/latest/) on ReadTheDocs.
+
+I promise you it is efficient! I [test it](https://github.com/GatienBouyer/fastgedcom/tree/main/benchmarks) and I use it.
 
 
 
 ## Feature details
 
-- Supports the read of gedcom files encoded in UTF-8 with and without BOM, UTF-16 (also named UNICODE), ANSI, and ANSEL.
-- ~~Supports the export to gedcom files encoded in UTF-8, UTF-16, and ANSI.~~
+- Supports reading of gedcom files encoded in UTF-8 with and without BOM, UTF-16 (also named UNICODE), ANSI, and ANSEL.
+- ~~Supports export of gedcom files encoded in UTF-8, UTF-16, and ANSI.~~
 
 ## Feedbacks
 
 Feedbacks are welcome, and they will be greatly appreciated!
 
 If you like this project, consider putting a star on [Github](https://github.com/GatienBouyer/fastgedcom), thank you!
```

### Comparing `fastgedcom-0.0.4/fastgedcom.egg-info/PKG-INFO` & `fastgedcom-0.0.5/fastgedcom.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,117 +1,124 @@
 Metadata-Version: 2.1
 Name: fastgedcom
-Version: 0.0.4
-Summary: A gedcom tool to parse, browse and modify gedcom files
-Home-page: https://github.com/GatienBouyer/fastgedcom
+Version: 0.0.5
+Summary: A lightweight tool to parse, browse and edit gedcom files.
 Author: Gatien Bouyer
 Author-email: gatien.bouyer.dev@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/GatienBouyer/fastgedcom/issues
 Project-URL: Source, https://github.com/GatienBouyer/fastgedcom
+Project-URL: Documentation, https://fastgedcom.readthedocs.io/en/latest/
 Keywords: fastgedcom gedcom parser genealogy
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Sociology :: Genealogy
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # FastGedcom
 
-A gedcom tool to parse, browse and modify gedcom files
+A lightweight tool to parse, browse and edit gedcom files.
 
 ```bash
 pip install fastgedcom
 ```
 
 Want to open a gedcom file?
 ```python
 from fastgedcom.parser import guess_encoding, parse
 
 gedcom_file = "my_gedcom_file.ged"
 with open(gedcom_file, "r", encoding=guess_encoding(gedcom_file)) as f:
 	document, warnings = parse(f)
 
-print(warnings) # in case of duplicate record reference
+if warnings: print(warnings) # in case of duplicate record reference
 ```
 
 
-Simple to write! Free to chose the fields, the data, and the formatting.
+Easy to write! Free choice of fields, data, and formatting.
 ```python
 from fastgedcom.helpers import format_date
 
 birth_date = (document["@I1@"] > "BIRT") >= "DATE"
 print(format_date(birth_date))
 ```
 
 A field is missing? FakeLine to the rescue. Like a TrueLine, but no error, no value, and no error handling code!
 ```python
 from fastgedcom.base import is_true
 
-indi = document["@I1"]
+indi = document["@I1@"]
 death_date = (indi > "DEAT") >= "DATE"
 if death_date != "": print(format_date(death_date)) 
-if not is_true(indi): print("It was not even present!")
+if not is_true(indi): print("@I1@ was not even present!")
 ```
 
 Don't like magic operator overload? Use standard methods!
 ```python
 indi = document.get_record("@I1@")
 surname = indi.get_sub_line("NAME").get_sub_line_payload("SURN")
 ```
 
-Typehints for salvation!
+Typehints for salvation! Autocompletion and type checking make development so much easier.
 ```python
 from fastgedcom.base import Document, FakeLine, IndiRef, Record, is_true
 from fastgedcom.helpers import format_name
 
 def print_infos(gedcom: Document, indi: IndiRef) -> None:
 	record = gedcom[indi]
 	if is_true(record): print_name(record)
 
 def print_name(record: Record | FakeLine) -> None:
 	print(format_name(record >= "NAME"))
 
 print_infos(document, "@I1@")
 ```
 
-Iteration on families is fast. Don't blink!
+Iteration on families is fast. Save time!
 ```python
 from fastgedcom.family_aid import FamilyAid
 
 booster = FamilyAid(document)
 
 def number_of_ascendants(indi: Record | FakeLine) -> int:
 	if not is_true(indi): return 1
 	father, mother = booster.get_parents(indi.tag)
 	return 1+max(number_of_ascendants(father), number_of_ascendants(mother))
 
 def number_of_descendants(indi: IndiRef) -> int:
-	children = booster.get_children(indi)
+	children = booster.get_children_ref(indi)
 	return len(children) + sum(number_of_descendants(c) for c in children)
 
-print(number_of_ascendants(document["@I1@"]))
-print(number_of_descendants("@I1@"))
+print(max(number_of_ascendants(indi)
+	for indi in document.get_records("INDI")
+))
+print(max(number_of_descendants(indi.tag)
+	for indi in document.get_records("INDI")
+))
 ```
 
 You want to see more? [Here are some examples](https://github.com/GatienBouyer/fastgedcom/tree/main/examples)
 
-I promise you it is fast! I [test it](https://github.com/GatienBouyer/fastgedcom/tree/main/benchmarks) and I use it.
+The documentation of FastGedcom is available [here](https://fastgedcom.readthedocs.io/en/latest/) on ReadTheDocs.
+
+I promise you it is efficient! I [test it](https://github.com/GatienBouyer/fastgedcom/tree/main/benchmarks) and I use it.
 
 
 
 ## Feature details
 
-- Supports the read of gedcom files encoded in UTF-8 with and without BOM, UTF-16 (also named UNICODE), ANSI, and ANSEL.
-- ~~Supports the export to gedcom files encoded in UTF-8, UTF-16, and ANSI.~~
+- Supports reading of gedcom files encoded in UTF-8 with and without BOM, UTF-16 (also named UNICODE), ANSI, and ANSEL.
+- ~~Supports export of gedcom files encoded in UTF-8, UTF-16, and ANSI.~~
 
 ## Feedbacks
 
 Feedbacks are welcome, and they will be greatly appreciated!
 
 If you like this project, consider putting a star on [Github](https://github.com/GatienBouyer/fastgedcom), thank you!
```

### Comparing `fastgedcom-0.0.4/setup.py` & `fastgedcom-0.0.5/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,40 +1,44 @@
-from setuptools import setup
+from setuptools import setup #type: ignore[import]
 
 with open("Readme.md", "r") as f:
-    long_description = f.read()
+	long_description = f.read()
 
 with open("requirements.txt", "r") as f:
-    requirements = f.readlines()
+	requirements = f.readlines()
+
+with open("requirements-dev.txt", "r") as f:
+	requirements_dev = f.readlines()
 
 setup(
-    name="fastgedcom",
-    version="0.0.4",
-    description="A gedcom tool to parse, browse and modify gedcom files",
-    packages=["fastgedcom"],
-    package_data={"fastgedcom": ["py.typed"]},
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    zip_safe=False,
-    install_requires=requirements,
-    extras_require={
-        "dev": ["mypy", "twine"],
+	name="fastgedcom",
+	version="0.0.5",
+	description="A lightweight tool to parse, browse and edit gedcom files.",
+	packages=["fastgedcom"],
+	package_data={"fastgedcom": ["py.typed"]},
+	long_description=long_description,
+	long_description_content_type="text/markdown",
+	zip_safe=False,
+	install_requires=requirements,
+	extras_require={
+		"dev": requirements_dev,
 	},
-    python_requires=">=3.11",
-    url="https://github.com/GatienBouyer/fastgedcom",
-    author="Gatien Bouyer",
-    author_email="gatien.bouyer.dev@gmail.com",
-    license="MIT",
-    classifiers=[
-        "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.11",
-        "Topic :: Sociology :: Genealogy",
-        "Intended Audience :: Developers",
-        "Operating System :: OS Independent",
-        "Development Status :: 3 - Alpha",
-    ],
-    keywords='fastgedcom gedcom parser genealogy',
+	python_requires=">=3.10", # typing.TypeGuard, addded in 3.10, is need
+	author="Gatien Bouyer",
+	author_email="gatien.bouyer.dev@gmail.com",
+	license="MIT",
+	classifiers=[
+		"License :: OSI Approved :: MIT License",
+		"Programming Language :: Python :: 3.10",
+		"Programming Language :: Python :: 3.11",
+		"Topic :: Sociology :: Genealogy",
+		"Intended Audience :: Developers",
+		"Operating System :: OS Independent",
+		"Development Status :: 3 - Alpha",
+	],
+	keywords='fastgedcom gedcom parser genealogy',
 	project_urls={
-        'Bug Reports': 'https://github.com/GatienBouyer/fastgedcom/issues',
-        'Source': 'https://github.com/GatienBouyer/fastgedcom',
-    },
+		'Bug Reports': 'https://github.com/GatienBouyer/fastgedcom/issues',
+		'Source': 'https://github.com/GatienBouyer/fastgedcom',
+		'Documentation': 'https://fastgedcom.readthedocs.io/en/latest/',
+	},
 )
```

