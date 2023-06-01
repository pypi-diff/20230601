# Comparing `tmp/django-plotly-wagtail-0.0.1.tar.gz` & `tmp/django-plotly-wagtail-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-plotly-wagtail-0.0.1.tar", last modified: Tue May  2 04:51:29 2023, max compression
+gzip compressed data, was "django-plotly-wagtail-0.0.2.tar", last modified: Thu Jun  1 05:21:05 2023, max compression
```

## Comparing `django-plotly-wagtail-0.0.1.tar` & `django-plotly-wagtail-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,22 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-02 04:51:29.034464 django-plotly-wagtail-0.0.1/
--rw-rw-r--   0 mark      (1000) mark      (1000)      911 2023-05-02 04:51:29.034464 django-plotly-wagtail-0.0.1/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)        0 2023-05-02 04:40:41.000000 django-plotly-wagtail-0.0.1/README.md
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-02 04:51:29.034464 django-plotly-wagtail-0.0.1/django_plotly_wagtail.egg-info/
--rw-rw-r--   0 mark      (1000) mark      (1000)      911 2023-05-02 04:51:29.000000 django-plotly-wagtail-0.0.1/django_plotly_wagtail.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      219 2023-05-02 04:51:29.000000 django-plotly-wagtail-0.0.1/django_plotly_wagtail.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2023-05-02 04:51:29.000000 django-plotly-wagtail-0.0.1/django_plotly_wagtail.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       10 2023-05-02 04:51:29.000000 django-plotly-wagtail-0.0.1/django_plotly_wagtail.egg-info/top_level.txt
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-02 04:51:29.034464 django-plotly-wagtail-0.0.1/dpwagtail/
--rw-rw-r--   0 mark      (1000) mark      (1000)       22 2023-05-02 04:44:02.000000 django-plotly-wagtail-0.0.1/dpwagtail/version.py
--rw-rw-r--   0 mark      (1000) mark      (1000)       38 2023-05-02 04:51:29.034464 django-plotly-wagtail-0.0.1/setup.cfg
--rw-rw-r--   0 mark      (1000) mark      (1000)     1304 2023-05-02 04:42:48.000000 django-plotly-wagtail-0.0.1/setup.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-06-01 05:21:05.156504 django-plotly-wagtail-0.0.2/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      912 2023-06-01 05:21:05.156504 django-plotly-wagtail-0.0.2/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)        0 2023-05-02 05:09:33.000000 django-plotly-wagtail-0.0.2/README.md
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-06-01 05:21:05.152504 django-plotly-wagtail-0.0.2/django_plotly_wagtail.egg-info/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      912 2023-06-01 05:21:05.000000 django-plotly-wagtail-0.0.2/django_plotly_wagtail.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      439 2023-06-01 05:21:05.000000 django-plotly-wagtail-0.0.2/django_plotly_wagtail.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2023-06-01 05:21:05.000000 django-plotly-wagtail-0.0.2/django_plotly_wagtail.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       38 2023-06-01 05:21:05.000000 django-plotly-wagtail-0.0.2/django_plotly_wagtail.egg-info/requires.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       10 2023-06-01 05:21:05.000000 django-plotly-wagtail-0.0.2/django_plotly_wagtail.egg-info/top_level.txt
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-06-01 05:21:05.156504 django-plotly-wagtail-0.0.2/dpwagtail/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      286 2023-05-22 03:21:57.000000 django-plotly-wagtail-0.0.2/dpwagtail/admin.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)       23 2023-05-20 06:34:41.000000 django-plotly-wagtail-0.0.2/dpwagtail/app_name.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1188 2023-06-01 04:40:13.000000 django-plotly-wagtail-0.0.2/dpwagtail/dash_apps.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     5212 2023-06-01 05:06:08.000000 django-plotly-wagtail-0.0.2/dpwagtail/models.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-06-01 05:21:05.156504 django-plotly-wagtail-0.0.2/dpwagtail/templatetags/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      468 2023-06-01 02:24:03.000000 django-plotly-wagtail-0.0.2/dpwagtail/templatetags/dpwagtail.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      301 2023-05-29 04:52:56.000000 django-plotly-wagtail-0.0.2/dpwagtail/urls.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      611 2023-05-22 07:20:30.000000 django-plotly-wagtail-0.0.2/dpwagtail/utils.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)       22 2023-06-01 05:20:48.000000 django-plotly-wagtail-0.0.2/dpwagtail/version.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      151 2023-05-22 06:45:32.000000 django-plotly-wagtail-0.0.2/dpwagtail/views.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)       38 2023-06-01 05:21:05.156504 django-plotly-wagtail-0.0.2/setup.cfg
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1388 2023-05-21 04:20:32.000000 django-plotly-wagtail-0.0.2/setup.py
```

### Comparing `django-plotly-wagtail-0.0.1/PKG-INFO` & `django-plotly-wagtail-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: django-plotly-wagtail
-Version: 0.0.1
+Version: 0.0.2
 Summary: Django Wagtail use of django-plotly-dash and plotly dash
 Home-page: https://gitlab.com/GibbsConsulting/django-plotly-wagtail
 Author: Gibbs Consulting
 Author-email: py.dpcms@gibbsconsulting.ca
 License: AGPL v3
 Project-URL: Source, https://gitlab.com/GibbsConsulting/django-plotly-wagtail
 Project-URL: Tracker, https://gitlab.com/GibbsConsulting/django-plotly-wagtail/issues
 Project-URL: Documentation, http://django-plotly-wagtail.readthedocs.io/
 Keywords: django plotly plotly-dash dash dashboard wagtail
 Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Dash
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 UNKNOWN
```

### Comparing `django-plotly-wagtail-0.0.1/django_plotly_wagtail.egg-info/PKG-INFO` & `django-plotly-wagtail-0.0.2/django_plotly_wagtail.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: django-plotly-wagtail
-Version: 0.0.1
+Version: 0.0.2
 Summary: Django Wagtail use of django-plotly-dash and plotly dash
 Home-page: https://gitlab.com/GibbsConsulting/django-plotly-wagtail
 Author: Gibbs Consulting
 Author-email: py.dpcms@gibbsconsulting.ca
 License: AGPL v3
 Project-URL: Source, https://gitlab.com/GibbsConsulting/django-plotly-wagtail
 Project-URL: Tracker, https://gitlab.com/GibbsConsulting/django-plotly-wagtail/issues
 Project-URL: Documentation, http://django-plotly-wagtail.readthedocs.io/
 Keywords: django plotly plotly-dash dash dashboard wagtail
 Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Dash
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 UNKNOWN
```

### Comparing `django-plotly-wagtail-0.0.1/setup.py` & `django-plotly-wagtail-0.0.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,26 +19,30 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Gibbs Consulting",
     author_email="py.dpcms@gibbsconsulting.ca",
     license='AGPL v3',
     packages=[
         'dpwagtail',
+        'dpwagtail.templatetags',
     ],
     include_package_data=True,
     classifiers = [
-    'Development Status :: 4 - Beta',
+    'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: GNU Affero General Public License v3',
     'Programming Language :: Python :: 3',
     'Framework :: Dash',
     ],
     keywords='django plotly plotly-dash dash dashboard wagtail',
     project_urls = {
     'Source': "https://gitlab.com/GibbsConsulting/django-plotly-wagtail",
     'Tracker': "https://gitlab.com/GibbsConsulting/django-plotly-wagtail/issues",
     'Documentation': 'http://django-plotly-wagtail.readthedocs.io/',
     },
-    install_requires = [#'django-plotly-dash',
+    install_requires = [
+        'django>3.2',
+        'django-plotly-dash',
+        'wagtail',
     ],
-    python_requires=">=3.8",
+    python_requires=">=3.9",
     )
```

