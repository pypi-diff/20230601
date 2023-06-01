# Comparing `tmp/data-harmonization-ai-dp-1.1.1.tar.gz` & `tmp/data-harmonization-ai-dp-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-harmonization-ai-dp-1.1.1.tar", last modified: Thu Jun  1 12:24:04 2023, max compression
+gzip compressed data, was "data-harmonization-ai-dp-2.0.0.tar", last modified: Thu Jun  1 12:34:35 2023, max compression
```

## Comparing `data-harmonization-ai-dp-1.1.1.tar` & `data-harmonization-ai-dp-2.0.0.tar`

### file list

```diff
@@ -1,34 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 12:24:04.749318 data-harmonization-ai-dp-1.1.1/
--rw-rw-rw-   0        0        0     1995 2023-06-01 12:24:04.747315 data-harmonization-ai-dp-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1579 2023-06-01 12:23:46.000000 data-harmonization-ai-dp-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 12:24:04.659908 data-harmonization-ai-dp-1.1.1/api/
-drwxrwxrwx   0        0        0        0 2023-06-01 12:24:04.697731 data-harmonization-ai-dp-1.1.1/api/mapper/
--rw-rw-rw-   0        0        0        0 2023-04-06 09:18:28.000000 data-harmonization-ai-dp-1.1.1/api/mapper/__init__.py
--rw-rw-rw-   0        0        0      131 2023-04-06 09:18:28.000000 data-harmonization-ai-dp-1.1.1/api/mapper/admin.py
--rw-rw-rw-   0        0        0     1932 2023-06-01 07:32:33.000000 data-harmonization-ai-dp-1.1.1/api/mapper/algo_functions.py
-drwxrwxrwx   0        0        0        0 2023-06-01 12:24:04.729364 data-harmonization-ai-dp-1.1.1/api/mapper/algos/
--rw-rw-rw-   0        0        0        0 2023-04-06 09:18:28.000000 data-harmonization-ai-dp-1.1.1/api/mapper/algos/__init__.py
--rw-rw-rw-   0        0        0     1660 2023-05-11 05:33:10.000000 data-harmonization-ai-dp-1.1.1/api/mapper/algos/fuzzywuzzy.py
--rw-rw-rw-   0        0        0     2929 2023-06-01 07:32:33.000000 data-harmonization-ai-dp-1.1.1/api/mapper/algos/fw_with_openai4.py
--rw-rw-rw-   0        0        0     1391 2023-06-01 11:48:28.000000 data-harmonization-ai-dp-1.1.1/api/mapper/algos/harmonizationWithSuggestionService.py
--rw-rw-rw-   0        0        0     2868 2023-06-01 07:32:33.000000 data-harmonization-ai-dp-1.1.1/api/mapper/algos/jw_with_openai.py
--rw-rw-rw-   0        0        0     2883 2023-06-01 07:32:33.000000 data-harmonization-ai-dp-1.1.1/api/mapper/algos/jw_with_openai4.py
--rw-rw-rw-   0        0        0     1962 2023-06-01 07:32:33.000000 data-harmonization-ai-dp-1.1.1/api/mapper/algos/openai.py
--rw-rw-rw-   0        0        0     2219 2023-06-01 07:32:33.000000 data-harmonization-ai-dp-1.1.1/api/mapper/algos/openaiGPT4.py
--rw-rw-rw-   0        0        0     1658 2023-05-11 05:33:10.000000 data-harmonization-ai-dp-1.1.1/api/mapper/algos/rapidfuzz.py
--rw-rw-rw-   0        0        0     1099 2023-06-01 09:46:55.000000 data-harmonization-ai-dp-1.1.1/api/mapper/algos/recursive_harmonization.py
--rw-rw-rw-   0        0        0     1778 2023-05-11 05:33:10.000000 data-harmonization-ai-dp-1.1.1/api/mapper/algos/stringmetric.py
--rw-rw-rw-   0        0        0      150 2023-04-06 09:18:28.000000 data-harmonization-ai-dp-1.1.1/api/mapper/apps.py
--rw-rw-rw-   0        0        0     1346 2023-06-01 07:32:33.000000 data-harmonization-ai-dp-1.1.1/api/mapper/models.py
--rw-rw-rw-   0        0        0      194 2023-04-06 09:18:28.000000 data-harmonization-ai-dp-1.1.1/api/mapper/serializers.py
--rw-rw-rw-   0        0        0       27 2023-04-06 09:18:28.000000 data-harmonization-ai-dp-1.1.1/api/mapper/tests.py
--rw-rw-rw-   0        0        0     1585 2023-06-01 07:32:33.000000 data-harmonization-ai-dp-1.1.1/api/mapper/views.py
-drwxrwxrwx   0        0        0        0 2023-06-01 12:24:04.745322 data-harmonization-ai-dp-1.1.1/data_harmonization_ai_dp.egg-info/
--rw-rw-rw-   0        0        0     1995 2023-06-01 12:24:04.000000 data-harmonization-ai-dp-1.1.1/data_harmonization_ai_dp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      833 2023-06-01 12:24:04.000000 data-harmonization-ai-dp-1.1.1/data_harmonization_ai_dp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 12:24:04.000000 data-harmonization-ai-dp-1.1.1/data_harmonization_ai_dp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-06-01 12:24:04.000000 data-harmonization-ai-dp-1.1.1/data_harmonization_ai_dp.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-01 12:24:04.000000 data-harmonization-ai-dp-1.1.1/data_harmonization_ai_dp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 12:24:04.750308 data-harmonization-ai-dp-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      837 2023-06-01 12:24:00.000000 data-harmonization-ai-dp-1.1.1/setup.py
--rw-rw-rw-   0        0        0     2594 2023-06-01 11:37:49.000000 data-harmonization-ai-dp-1.1.1/utility.py
+drwxrwxrwx   0        0        0        0 2023-06-01 12:34:35.866709 data-harmonization-ai-dp-2.0.0/
+-rw-rw-rw-   0        0        0     1995 2023-06-01 12:34:35.865532 data-harmonization-ai-dp-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1579 2023-06-01 12:23:46.000000 data-harmonization-ai-dp-2.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 12:34:35.782136 data-harmonization-ai-dp-2.0.0/api/
+-rw-rw-rw-   0        0        0        0 2023-04-06 09:18:28.000000 data-harmonization-ai-dp-2.0.0/api/__init__.py
+-rw-rw-rw-   0        0        0      399 2023-04-06 09:18:28.000000 data-harmonization-ai-dp-2.0.0/api/asgi.py
+drwxrwxrwx   0        0        0        0 2023-06-01 12:34:35.807920 data-harmonization-ai-dp-2.0.0/api/mapper/
+-rw-rw-rw-   0        0        0        0 2023-04-06 09:18:28.000000 data-harmonization-ai-dp-2.0.0/api/mapper/__init__.py
+-rw-rw-rw-   0        0        0      131 2023-04-06 09:18:28.000000 data-harmonization-ai-dp-2.0.0/api/mapper/admin.py
+-rw-rw-rw-   0        0        0     1932 2023-06-01 07:32:33.000000 data-harmonization-ai-dp-2.0.0/api/mapper/algo_functions.py
+drwxrwxrwx   0        0        0        0 2023-06-01 12:34:35.844759 data-harmonization-ai-dp-2.0.0/api/mapper/algos/
+-rw-rw-rw-   0        0        0        0 2023-04-06 09:18:28.000000 data-harmonization-ai-dp-2.0.0/api/mapper/algos/__init__.py
+-rw-rw-rw-   0        0        0     1660 2023-05-11 05:33:10.000000 data-harmonization-ai-dp-2.0.0/api/mapper/algos/fuzzywuzzy.py
+-rw-rw-rw-   0        0        0     2929 2023-06-01 07:32:33.000000 data-harmonization-ai-dp-2.0.0/api/mapper/algos/fw_with_openai4.py
+-rw-rw-rw-   0        0        0     1391 2023-06-01 11:48:28.000000 data-harmonization-ai-dp-2.0.0/api/mapper/algos/harmonizationWithSuggestionService.py
+-rw-rw-rw-   0        0        0     2868 2023-06-01 07:32:33.000000 data-harmonization-ai-dp-2.0.0/api/mapper/algos/jw_with_openai.py
+-rw-rw-rw-   0        0        0     2883 2023-06-01 07:32:33.000000 data-harmonization-ai-dp-2.0.0/api/mapper/algos/jw_with_openai4.py
+-rw-rw-rw-   0        0        0     1962 2023-06-01 07:32:33.000000 data-harmonization-ai-dp-2.0.0/api/mapper/algos/openai.py
+-rw-rw-rw-   0        0        0     2219 2023-06-01 07:32:33.000000 data-harmonization-ai-dp-2.0.0/api/mapper/algos/openaiGPT4.py
+-rw-rw-rw-   0        0        0     1658 2023-05-11 05:33:10.000000 data-harmonization-ai-dp-2.0.0/api/mapper/algos/rapidfuzz.py
+-rw-rw-rw-   0        0        0     1099 2023-06-01 09:46:55.000000 data-harmonization-ai-dp-2.0.0/api/mapper/algos/recursive_harmonization.py
+-rw-rw-rw-   0        0        0     1778 2023-05-11 05:33:10.000000 data-harmonization-ai-dp-2.0.0/api/mapper/algos/stringmetric.py
+-rw-rw-rw-   0        0        0      150 2023-04-06 09:18:28.000000 data-harmonization-ai-dp-2.0.0/api/mapper/apps.py
+-rw-rw-rw-   0        0        0     1346 2023-06-01 07:32:33.000000 data-harmonization-ai-dp-2.0.0/api/mapper/models.py
+-rw-rw-rw-   0        0        0      194 2023-04-06 09:18:28.000000 data-harmonization-ai-dp-2.0.0/api/mapper/serializers.py
+-rw-rw-rw-   0        0        0       27 2023-04-06 09:18:28.000000 data-harmonization-ai-dp-2.0.0/api/mapper/tests.py
+-rw-rw-rw-   0        0        0     1585 2023-06-01 07:32:33.000000 data-harmonization-ai-dp-2.0.0/api/mapper/views.py
+-rw-rw-rw-   0        0        0     4151 2023-06-01 12:31:23.000000 data-harmonization-ai-dp-2.0.0/api/settings.py
+-rw-rw-rw-   0        0        0      592 2023-05-19 07:48:38.000000 data-harmonization-ai-dp-2.0.0/api/urls.py
+-rw-rw-rw-   0        0        0      399 2023-04-06 09:18:28.000000 data-harmonization-ai-dp-2.0.0/api/wsgi.py
+drwxrwxrwx   0        0        0        0 2023-06-01 12:34:35.863042 data-harmonization-ai-dp-2.0.0/data_harmonization_ai_dp.egg-info/
+-rw-rw-rw-   0        0        0     1995 2023-06-01 12:34:35.000000 data-harmonization-ai-dp-2.0.0/data_harmonization_ai_dp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      901 2023-06-01 12:34:35.000000 data-harmonization-ai-dp-2.0.0/data_harmonization_ai_dp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 12:34:35.000000 data-harmonization-ai-dp-2.0.0/data_harmonization_ai_dp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-06-01 12:34:35.000000 data-harmonization-ai-dp-2.0.0/data_harmonization_ai_dp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-01 12:34:35.000000 data-harmonization-ai-dp-2.0.0/data_harmonization_ai_dp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 12:34:35.867707 data-harmonization-ai-dp-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      853 2023-06-01 12:33:46.000000 data-harmonization-ai-dp-2.0.0/setup.py
+-rw-rw-rw-   0        0        0     2594 2023-06-01 11:37:49.000000 data-harmonization-ai-dp-2.0.0/utility.py
```

### Comparing `data-harmonization-ai-dp-1.1.1/PKG-INFO` & `data-harmonization-ai-dp-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-harmonization-ai-dp
-Version: 1.1.1
+Version: 2.0.0
 Summary: Create data quality rules and apply them to datasets.
 Author: Himanshu
 Author-email: himanshu.tomar@decisionpoint.in
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `data-harmonization-ai-dp-1.1.1/README.md` & `data-harmonization-ai-dp-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `data-harmonization-ai-dp-1.1.1/api/mapper/algo_functions.py` & `data-harmonization-ai-dp-2.0.0/api/mapper/algo_functions.py`

 * *Files identical despite different names*

### Comparing `data-harmonization-ai-dp-1.1.1/api/mapper/algos/fuzzywuzzy.py` & `data-harmonization-ai-dp-2.0.0/api/mapper/algos/fuzzywuzzy.py`

 * *Files identical despite different names*

### Comparing `data-harmonization-ai-dp-1.1.1/api/mapper/algos/fw_with_openai4.py` & `data-harmonization-ai-dp-2.0.0/api/mapper/algos/fw_with_openai4.py`

 * *Files identical despite different names*

### Comparing `data-harmonization-ai-dp-1.1.1/api/mapper/algos/harmonizationWithSuggestionService.py` & `data-harmonization-ai-dp-2.0.0/api/mapper/algos/harmonizationWithSuggestionService.py`

 * *Files identical despite different names*

### Comparing `data-harmonization-ai-dp-1.1.1/api/mapper/algos/jw_with_openai.py` & `data-harmonization-ai-dp-2.0.0/api/mapper/algos/jw_with_openai.py`

 * *Files identical despite different names*

### Comparing `data-harmonization-ai-dp-1.1.1/api/mapper/algos/jw_with_openai4.py` & `data-harmonization-ai-dp-2.0.0/api/mapper/algos/jw_with_openai4.py`

 * *Files identical despite different names*

### Comparing `data-harmonization-ai-dp-1.1.1/api/mapper/algos/openai.py` & `data-harmonization-ai-dp-2.0.0/api/mapper/algos/openai.py`

 * *Files identical despite different names*

### Comparing `data-harmonization-ai-dp-1.1.1/api/mapper/algos/openaiGPT4.py` & `data-harmonization-ai-dp-2.0.0/api/mapper/algos/openaiGPT4.py`

 * *Files identical despite different names*

### Comparing `data-harmonization-ai-dp-1.1.1/api/mapper/algos/rapidfuzz.py` & `data-harmonization-ai-dp-2.0.0/api/mapper/algos/rapidfuzz.py`

 * *Files identical despite different names*

### Comparing `data-harmonization-ai-dp-1.1.1/api/mapper/algos/recursive_harmonization.py` & `data-harmonization-ai-dp-2.0.0/api/mapper/algos/recursive_harmonization.py`

 * *Files identical despite different names*

### Comparing `data-harmonization-ai-dp-1.1.1/api/mapper/algos/stringmetric.py` & `data-harmonization-ai-dp-2.0.0/api/mapper/algos/stringmetric.py`

 * *Files identical despite different names*

### Comparing `data-harmonization-ai-dp-1.1.1/api/mapper/models.py` & `data-harmonization-ai-dp-2.0.0/api/mapper/models.py`

 * *Files identical despite different names*

### Comparing `data-harmonization-ai-dp-1.1.1/api/mapper/views.py` & `data-harmonization-ai-dp-2.0.0/api/mapper/views.py`

 * *Files identical despite different names*

### Comparing `data-harmonization-ai-dp-1.1.1/data_harmonization_ai_dp.egg-info/PKG-INFO` & `data-harmonization-ai-dp-2.0.0/data_harmonization_ai_dp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-harmonization-ai-dp
-Version: 1.1.1
+Version: 2.0.0
 Summary: Create data quality rules and apply them to datasets.
 Author: Himanshu
 Author-email: himanshu.tomar@decisionpoint.in
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `data-harmonization-ai-dp-1.1.1/data_harmonization_ai_dp.egg-info/SOURCES.txt` & `data-harmonization-ai-dp-2.0.0/data_harmonization_ai_dp.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 README.md
 setup.py
 utility.py
+api/__init__.py
+api/asgi.py
+api/settings.py
+api/urls.py
+api/wsgi.py
 api/mapper/__init__.py
 api/mapper/admin.py
 api/mapper/algo_functions.py
 api/mapper/apps.py
 api/mapper/models.py
 api/mapper/serializers.py
 api/mapper/tests.py
```

### Comparing `data-harmonization-ai-dp-1.1.1/setup.py` & `data-harmonization-ai-dp-2.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 # COMMAND ----------
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read() 
     
 setuptools.setup(
     name="data-harmonization-ai-dp",
-    version="1.1.1",
+    version="2.0.0",
     author="Himanshu",
     author_email="himanshu.tomar@decisionpoint.in",
     description="Create data quality rules and apply them to datasets.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     py_modules=['utility'],
-    packages=['api.mapper','api.mapper.algos'],
+    packages=['api','api.mapper','api.mapper.algos'],
      
     classifiers=[
          "Programming Language :: Python :: 3",
          "License :: OSI Approved :: MIT License",
          "Operating System :: OS Independent",
     ],
-    install_requires=['openai','pandas','fuzzywuzzy','stringmetric','rapidfuzz'],
+    install_requires=['openai','pandas','fuzzywuzzy','stringmetric','rapidfuzz','IPython'],
     python_requires='>=3.8',
 )
```

### Comparing `data-harmonization-ai-dp-1.1.1/utility.py` & `data-harmonization-ai-dp-2.0.0/utility.py`

 * *Files identical despite different names*

