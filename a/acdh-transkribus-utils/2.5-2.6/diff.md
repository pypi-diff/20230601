# Comparing `tmp/acdh-transkribus-utils-2.5.tar.gz` & `tmp/acdh-transkribus-utils-2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acdh-transkribus-utils-2.5.tar", last modified: Tue Mar 28 13:04:28 2023, max compression
+gzip compressed data, was "acdh-transkribus-utils-2.6.tar", last modified: Thu Jun  1 11:02:02 2023, max compression
```

## Comparing `acdh-transkribus-utils-2.5.tar` & `acdh-transkribus-utils-2.6.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:04:28.297741 acdh-transkribus-utils-2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-03-28 13:04:18.000000 acdh-transkribus-utils-2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-28 13:04:18.000000 acdh-transkribus-utils-2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-03-28 13:04:28.297741 acdh-transkribus-utils-2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-03-28 13:04:18.000000 acdh-transkribus-utils-2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:04:28.297741 acdh-transkribus-utils-2.5/acdh_transkribus_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-03-28 13:04:28.000000 acdh-transkribus-utils-2.5/acdh_transkribus_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-03-28 13:04:28.000000 acdh-transkribus-utils-2.5/acdh_transkribus_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 13:04:28.000000 acdh-transkribus-utils-2.5/acdh_transkribus_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-28 13:04:28.000000 acdh-transkribus-utils-2.5/acdh_transkribus_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 13:04:28.000000 acdh-transkribus-utils-2.5/acdh_transkribus_utils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-28 13:04:28.000000 acdh-transkribus-utils-2.5/acdh_transkribus_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-28 13:04:28.000000 acdh-transkribus-utils-2.5/acdh_transkribus_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 13:04:28.297741 acdh-transkribus-utils-2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-03-28 13:04:19.000000 acdh-transkribus-utils-2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:04:28.297741 acdh-transkribus-utils-2.5/transkribus_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-28 13:04:18.000000 acdh-transkribus-utils-2.5/transkribus_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-03-28 13:04:18.000000 acdh-transkribus-utils-2.5/transkribus_utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-03-28 13:04:18.000000 acdh-transkribus-utils-2.5/transkribus_utils/mets.py
--rw-r--r--   0 runner    (1001) docker     (123)    17497 2023-03-28 13:04:18.000000 acdh-transkribus-utils-2.5/transkribus_utils/transkribus_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:02:02.749729 acdh-transkribus-utils-2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-01 11:01:52.000000 acdh-transkribus-utils-2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-01 11:01:52.000000 acdh-transkribus-utils-2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-06-01 11:02:02.749729 acdh-transkribus-utils-2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-06-01 11:01:52.000000 acdh-transkribus-utils-2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:02:02.745729 acdh-transkribus-utils-2.6/acdh_transkribus_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-06-01 11:02:02.000000 acdh-transkribus-utils-2.6/acdh_transkribus_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-01 11:02:02.000000 acdh-transkribus-utils-2.6/acdh_transkribus_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 11:02:02.000000 acdh-transkribus-utils-2.6/acdh_transkribus_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-01 11:02:02.000000 acdh-transkribus-utils-2.6/acdh_transkribus_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 11:02:02.000000 acdh-transkribus-utils-2.6/acdh_transkribus_utils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 11:02:02.000000 acdh-transkribus-utils-2.6/acdh_transkribus_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-01 11:02:02.000000 acdh-transkribus-utils-2.6/acdh_transkribus_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 11:02:02.749729 acdh-transkribus-utils-2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-01 11:01:52.000000 acdh-transkribus-utils-2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:02:02.749729 acdh-transkribus-utils-2.6/transkribus_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-01 11:01:52.000000 acdh-transkribus-utils-2.6/transkribus_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-01 11:01:52.000000 acdh-transkribus-utils-2.6/transkribus_utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-01 11:01:52.000000 acdh-transkribus-utils-2.6/transkribus_utils/iiif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-01 11:01:52.000000 acdh-transkribus-utils-2.6/transkribus_utils/mets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18559 2023-06-01 11:01:52.000000 acdh-transkribus-utils-2.6/transkribus_utils/transkribus_utils.py
```

### Comparing `acdh-transkribus-utils-2.5/LICENSE` & `acdh-transkribus-utils-2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `acdh-transkribus-utils-2.5/PKG-INFO` & `acdh-transkribus-utils-2.6/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: acdh-transkribus-utils
-Version: 2.5
-Summary: some utility function to interact with the Transkribus-API
-Home-page: https://github.com/acdh-oeaw/acdh-transkribus-utils
-Author: Peter Andorfer, Matthias Schlögl, Carl Friedrich Haak
-Author-email: peter.andorfer@oeaw.ac.at
-License: MIT
-Keywords: acdh-transkribus-utils
-Classifier: Development Status :: 3 - Alpha
-Classifier: Framework :: Django :: 2.0
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # acdh-transkribus-utils
 
 [![PyPI version](https://badge.fury.io/py/acdh-transkribus-utils.svg)](https://badge.fury.io/py/acdh-transkribus-utils)
 [![flake8 Lint](https://github.com/acdh-oeaw/acdh-transkribus-utils/actions/workflows/lint.yml/badge.svg)](https://github.com/acdh-oeaw/acdh-transkribus-utils/actions/workflows/lint.yml)
 [![Test](https://github.com/acdh-oeaw/acdh-transkribus-utils/actions/workflows/test.yml/badge.svg)](https://github.com/acdh-oeaw/acdh-transkribus-utils/actions/workflows/test.yml)
 [![codecov](https://codecov.io/gh/acdh-oeaw/acdh-transkribus-utils/branch/master/graph/badge.svg?token=QOY62C0X5Y)](https://codecov.io/gh/acdh-oeaw/acdh-transkribus-utils)
 
@@ -44,19 +23,56 @@
 export TRANSKRIBUS_USER=some@mail.com
 export TRANSKRIBUS_PASSWORD=verysecret
 ```
 (or create a file called `env.secret` similar to `env.dummy` and run  `source export_env_variables.sh`)
 you can pass in your credentials also as params e.g. 
 
 ```python
+import os
+
 from transkribus_utils.transkribus_utils import ACDHTranskribusUtils
 
-client = ACDHTranskribusUtils(user="some@mail.com", password="verysecret")
+
+tr_user = os.environ.get("TRANSKRIBUS_USER")
+tr_pw = os.environ.get("TRANSKRIBUS_PASSWORD")
+
+client = ACDHTranskribusUtils(user=tr_user, password=tr_pw)
+```
+
+### List all collections
+
+```python
+collections = client.list_collections()
+for x in collections[-7:]:
+    print(x["colId"], x["colName"])
+
+# 188933 bv-play
+# 188991 Kasten_blau_45_11
+# 190357 acdh-transkribus-utils
+# 193145 palm
+# 195363 Österreichische Bundesverfassung: Datenset A
+# 196428 Österreichische Bundesverfassung: Datenset B
+# 196429 Österreichische Bundesverfassung: Datenset C
 ```
 
+### List all documents from a given collection 
+
+```python
+col_id = 142911
+documents = client.list_docs(col_id)
+n = -3
+for x in documents[n:]:
+    print(x["docId"], x["title"], x["author"], x["nrOfPages"])
+
+# 950920 Kasten_blau_44_9_0050 Pfalz-Neuburg, Eleonore Magdalena Theresia von 1
+# 950921 Kasten_blau_44_9_0037 Pfalz, Johann Wilhelm Joseph Janaz von der 4
+# 950922 Kasten_blau_44_9_0239 Pfalz, Johann Wilhelm Joseph Janaz von der 1
+
+
+```
 ### Download METS files from Collection
 
 ```python
 from transkribus_utils.transkribus_utils import ACDHTranskribusUtils
 
 COL_ID = 51052
 client = ACDHTranskribusUtils()
@@ -64,8 +80,8 @@
 # downloads a METS for each document in the given collection into a folder `./{COL_ID}
 
 client.collection_to_mets(COL_ID, file_path='./foo')
 # downloads a METS for each document in the given collection into a folder `./foo/{COL_ID}
 
 client.collection_to_mets(COL_ID, filter_by_doc_ids=[230161, 230155])
 # downloads only METS for document with ID 230161 and 230155 into a folder `./{COL_ID}
-```
+```
```

### Comparing `acdh-transkribus-utils-2.5/setup.py` & `acdh-transkribus-utils-2.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md") as readme_file:
     readme = readme_file.read()
 
 
 setup(
     name="acdh-transkribus-utils",
-    version="v2.5",
+    version="v2.6",
     description="""some utility function to interact with the Transkribus-API""",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Peter Andorfer, Matthias Schlögl, Carl Friedrich Haak",
     author_email="peter.andorfer@oeaw.ac.at",
     url="https://github.com/acdh-oeaw/acdh-transkribus-utils",
     packages=[
```

### Comparing `acdh-transkribus-utils-2.5/transkribus_utils/cli.py` & `acdh-transkribus-utils-2.6/transkribus_utils/cli.py`

 * *Files identical despite different names*

### Comparing `acdh-transkribus-utils-2.5/transkribus_utils/mets.py` & `acdh-transkribus-utils-2.6/transkribus_utils/mets.py`

 * *Files identical despite different names*

### Comparing `acdh-transkribus-utils-2.5/transkribus_utils/transkribus_utils.py` & `acdh-transkribus-utils-2.6/transkribus_utils/transkribus_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import io
 import os
 import requests
 import lxml.etree as ET
 import re
 
 from .mets import get_title_from_mets, replace_img_urls_in_mets
+from .iiif import get_title_from_iiif
 
 base_url = "https://transkribus.eu/TrpServer/rest"
 nsmap = {"page": "http://schema.primaresearch.org/PAGE/gts/pagecontent/2013-07-15"}
 crowd_base_url = (
     "https://transkribus.eu/r/read/sandbox/application/?colId={}&docId={}&pageId={}"
 )
 
@@ -389,14 +390,39 @@
             if check_name:
                 s1 = self.search_for_document(f, col_id)
                 if len(s1) == 0:
                     self.upload_mets_file_from_url(
                         self.goobi_base_url.format(f), col_id=col_id
                     )
 
+    def upload_iiif_from_url(self, iiif_url, col_id):
+        """Takes an URL to a IIIF Manifest and posts that URL to Transkribus
+        :param iiif_url: URL of the IIIF Manifest
+        :param col_id: Transkribus CollectionID
+        """
+        # ToDo: check if document with same title already exists
+        doc_title = get_title_from_iiif(iiif_url)
+        doc_exists = self.search_for_document(title=doc_title, col_id=col_id)
+        if len(doc_exists) == 0:
+            res = requests.post(
+                f"{self.base_url}/collections/{col_id}/createDocFromIiifUrl",
+                cookies=self.login_cookie,
+                params={"fileName": iiif_url},
+            )
+            if res.status_code == 200:
+                return True
+            else:
+                print("Error: ", res.status_code, res.content)
+                return False
+        else:
+            print(
+                f"a document with title: {doc_title} already exists in collection {col_id}"
+            )
+            return False
+
     def __init__(
         self,
         user=None,
         password=None,
         transkribus_base_url=base_url,
         goobi_base_url=None,
     ) -> None:
```

