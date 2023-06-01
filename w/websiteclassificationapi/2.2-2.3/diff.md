# Comparing `tmp/websiteclassificationapi-2.2.tar.gz` & `tmp/websiteclassificationapi-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\websiteclassificationapi-2.2.tar", last modified: Sat May 13 14:41:24 2023, max compression
+gzip compressed data, was "dist\websiteclassificationapi-2.3.tar", last modified: Thu Jun  1 08:32:09 2023, max compression
```

## Comparing `websiteclassificationapi-2.2.tar` & `websiteclassificationapi-2.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 14:41:24.000000 websiteclassificationapi-2.2/
--rw-rw-rw-   0        0        0    14125 2023-05-13 14:41:24.000000 websiteclassificationapi-2.2/PKG-INFO
--rw-rw-rw-   0        0        0    11262 2023-05-13 14:36:19.000000 websiteclassificationapi-2.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-13 14:41:24.000000 websiteclassificationapi-2.2/setup.cfg
--rw-rw-rw-   0        0        0     1379 2023-05-13 14:41:13.000000 websiteclassificationapi-2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-13 14:41:24.000000 websiteclassificationapi-2.2/test/
--rw-rw-rw-   0        0        0     2869 2022-08-29 10:19:49.000000 websiteclassificationapi-2.2/test/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-13 14:41:24.000000 websiteclassificationapi-2.2/websiteclassificationapi/
--rw-rw-rw-   0        0        0     2869 2022-08-29 10:19:49.000000 websiteclassificationapi-2.2/websiteclassificationapi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-13 14:41:24.000000 websiteclassificationapi-2.2/websiteclassificationapi.egg-info/
--rw-rw-rw-   0        0        0    14125 2023-05-13 14:41:24.000000 websiteclassificationapi-2.2/websiteclassificationapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-05-13 14:41:24.000000 websiteclassificationapi-2.2/websiteclassificationapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 14:41:24.000000 websiteclassificationapi-2.2/websiteclassificationapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-05-13 14:41:24.000000 websiteclassificationapi-2.2/websiteclassificationapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-01 08:32:09.000000 websiteclassificationapi-2.3/
+-rw-rw-rw-   0        0        0    14275 2023-06-01 08:32:09.000000 websiteclassificationapi-2.3/PKG-INFO
+-rw-rw-rw-   0        0        0    11412 2023-06-01 08:30:13.000000 websiteclassificationapi-2.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-01 08:32:09.000000 websiteclassificationapi-2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1379 2023-06-01 08:31:32.000000 websiteclassificationapi-2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:32:09.000000 websiteclassificationapi-2.3/test/
+-rw-rw-rw-   0        0        0     2869 2022-08-29 10:19:49.000000 websiteclassificationapi-2.3/test/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:32:09.000000 websiteclassificationapi-2.3/websiteclassificationapi/
+-rw-rw-rw-   0        0        0     2869 2022-08-29 10:19:49.000000 websiteclassificationapi-2.3/websiteclassificationapi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:32:09.000000 websiteclassificationapi-2.3/websiteclassificationapi.egg-info/
+-rw-rw-rw-   0        0        0    14275 2023-06-01 08:32:09.000000 websiteclassificationapi-2.3/websiteclassificationapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-06-01 08:32:09.000000 websiteclassificationapi-2.3/websiteclassificationapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 08:32:09.000000 websiteclassificationapi-2.3/websiteclassificationapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-06-01 08:32:09.000000 websiteclassificationapi-2.3/websiteclassificationapi.egg-info/top_level.txt
```

### Comparing `websiteclassificationapi-2.2/PKG-INFO` & `websiteclassificationapi-2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: websiteclassificationapi
-Version: 2.2
+Version: 2.3
 Summary: Website classification API
 Home-page: https://github.com/websitecategorization/websiteclassificationnapi
 Author-email: info@websitecategorizationapi.com
 License: UNKNOWN
 Description: # Website Classification API
         
         Python3 client library for [URL Classification](https://www.websitecategorizationapi.com). 
@@ -112,15 +112,15 @@
         
         Here is for example usage of Intercom across industry verticals: 
         
         ![Image1](https://user-images.githubusercontent.com/58834207/238138013-d59d68b8-d7e3-42d2-bdda-100924669b72.png)
         
         Based on 50 millions of usage points we built an AI recommender which can predict which technologies for company using a set of technologies. 
         
-        Here are e.g. recommendations for company using Mouse Flow: <table class="table" style="font-size:20px;line-height:30px"><thead><tr><th>Technology</th><th>AI Recommendation Score </th><th>Website</th></tr></thead><tbody><tr><td><a href="https://www.alpha-quantum.com/technologies/AppNexus">AppNexus</a></td><td>0.15</td><td>http://appnexus.com</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/Microsoft Clarity">Microsoft Clarity</a></td><td>0.14</td><td>https://clarity.microsoft.com</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/Osano">Osano</a></td><td>0.14</td><td>https://www.osano.com/</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/Jetpack">Jetpack</a></td><td>0.14</td><td>https://jetpack.com</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/Raphael">Raphael</a></td><td>0.14</td><td>https://dmitrybaranovskiy.github.io/raphael/</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/Svelte">Svelte</a></td><td>0.13</td><td>https://svelte.dev</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/AWS Certificate Manager">AWS Certificate Manager</a></td><td>0.12</td><td>https://aws.amazon.com/certificate-manager/</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/Extendify">Extendify</a></td><td>0.11</td><td>https://extendify.com</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/Kendo UI">Kendo UI</a></td><td>0.11</td><td>https://www.telerik.com/kendo-ui</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/Flywheel">Flywheel</a></td><td>0.11</td><td>https://getflywheel.com</td></tr></tbody></table>
+        Here are e.g. recommendations for company using Mouse Flow: <table class="table" style="font-size:20px;line-height:30px"><thead><tr><th>Technology</th><th>AI Recommendation Score </th><th>Website</th></tr></thead><tbody><tr><td><a href="https://www.alpha-quantum.com/technologies/websites-using-AppNexus">AppNexus</a></td><td>0.15</td><td>http://appnexus.com</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/websites-using-Microsoft Clarity">Microsoft Clarity</a></td><td>0.14</td><td>https://clarity.microsoft.com</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/websites-using-Osano">Osano</a></td><td>0.14</td><td>https://www.osano.com/</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/websites-using-Jetpack">Jetpack</a></td><td>0.14</td><td>https://jetpack.com</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/websites-using-Raphael">Raphael</a></td><td>0.14</td><td>https://dmitrybaranovskiy.github.io/raphael/</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/websites-using-Svelte">Svelte</a></td><td>0.13</td><td>https://svelte.dev</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/websites-using-AWS Certificate Manager">AWS Certificate Manager</a></td><td>0.12</td><td>https://aws.amazon.com/certificate-manager/</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/websites-using-Extendify">Extendify</a></td><td>0.11</td><td>https://extendify.com</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/websites-using-Kendo UI">Kendo UI</a></td><td>0.11</td><td>https://www.telerik.com/kendo-ui</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/websites-using-Flywheel">Flywheel</a></td><td>0.11</td><td>https://getflywheel.com</td></tr></tbody></table>
         
         
         
         
         
         ## Example classifications
```

### Comparing `websiteclassificationapi-2.2/README.md` & `websiteclassificationapi-2.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 
 Here is for example usage of Intercom across industry verticals: 
 
 ![Image1](https://user-images.githubusercontent.com/58834207/238138013-d59d68b8-d7e3-42d2-bdda-100924669b72.png)
 
 Based on 50 millions of usage points we built an AI recommender which can predict which technologies for company using a set of technologies. 
 
-Here are e.g. recommendations for company using Mouse Flow: <table class="table" style="font-size:20px;line-height:30px"><thead><tr><th>Technology</th><th>AI Recommendation Score </th><th>Website</th></tr></thead><tbody><tr><td><a href="https://www.alpha-quantum.com/technologies/AppNexus">AppNexus</a></td><td>0.15</td><td>http://appnexus.com</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/Microsoft Clarity">Microsoft Clarity</a></td><td>0.14</td><td>https://clarity.microsoft.com</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/Osano">Osano</a></td><td>0.14</td><td>https://www.osano.com/</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/Jetpack">Jetpack</a></td><td>0.14</td><td>https://jetpack.com</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/Raphael">Raphael</a></td><td>0.14</td><td>https://dmitrybaranovskiy.github.io/raphael/</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/Svelte">Svelte</a></td><td>0.13</td><td>https://svelte.dev</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/AWS Certificate Manager">AWS Certificate Manager</a></td><td>0.12</td><td>https://aws.amazon.com/certificate-manager/</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/Extendify">Extendify</a></td><td>0.11</td><td>https://extendify.com</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/Kendo UI">Kendo UI</a></td><td>0.11</td><td>https://www.telerik.com/kendo-ui</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/Flywheel">Flywheel</a></td><td>0.11</td><td>https://getflywheel.com</td></tr></tbody></table>
+Here are e.g. recommendations for company using Mouse Flow: <table class="table" style="font-size:20px;line-height:30px"><thead><tr><th>Technology</th><th>AI Recommendation Score </th><th>Website</th></tr></thead><tbody><tr><td><a href="https://www.alpha-quantum.com/technologies/websites-using-AppNexus">AppNexus</a></td><td>0.15</td><td>http://appnexus.com</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/websites-using-Microsoft Clarity">Microsoft Clarity</a></td><td>0.14</td><td>https://clarity.microsoft.com</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/websites-using-Osano">Osano</a></td><td>0.14</td><td>https://www.osano.com/</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/websites-using-Jetpack">Jetpack</a></td><td>0.14</td><td>https://jetpack.com</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/websites-using-Raphael">Raphael</a></td><td>0.14</td><td>https://dmitrybaranovskiy.github.io/raphael/</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/websites-using-Svelte">Svelte</a></td><td>0.13</td><td>https://svelte.dev</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/websites-using-AWS Certificate Manager">AWS Certificate Manager</a></td><td>0.12</td><td>https://aws.amazon.com/certificate-manager/</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/websites-using-Extendify">Extendify</a></td><td>0.11</td><td>https://extendify.com</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/websites-using-Kendo UI">Kendo UI</a></td><td>0.11</td><td>https://www.telerik.com/kendo-ui</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/websites-using-Flywheel">Flywheel</a></td><td>0.11</td><td>https://getflywheel.com</td></tr></tbody></table>
 
 
 
 
 
 ## Example classifications
```

### Comparing `websiteclassificationapi-2.2/setup.py` & `websiteclassificationapi-2.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 setup(
     # The name of project.
     # pip install websiteclassificationapi
     name="websiteclassificationapi",
 
     # The version of your project.
-    version="2.2",
+    version="2.3",
 
     packages=find_packages(exclude="tests"),
 
     description="Website classification API",
 
     long_description=README_MD,
```

### Comparing `websiteclassificationapi-2.2/test/__init__.py` & `websiteclassificationapi-2.3/test/__init__.py`

 * *Files identical despite different names*

### Comparing `websiteclassificationapi-2.2/websiteclassificationapi/__init__.py` & `websiteclassificationapi-2.3/websiteclassificationapi/__init__.py`

 * *Files identical despite different names*

### Comparing `websiteclassificationapi-2.2/websiteclassificationapi.egg-info/PKG-INFO` & `websiteclassificationapi-2.3/websiteclassificationapi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: websiteclassificationapi
-Version: 2.2
+Version: 2.3
 Summary: Website classification API
 Home-page: https://github.com/websitecategorization/websiteclassificationnapi
 Author-email: info@websitecategorizationapi.com
 License: UNKNOWN
 Description: # Website Classification API
         
         Python3 client library for [URL Classification](https://www.websitecategorizationapi.com). 
@@ -112,15 +112,15 @@
         
         Here is for example usage of Intercom across industry verticals: 
         
         ![Image1](https://user-images.githubusercontent.com/58834207/238138013-d59d68b8-d7e3-42d2-bdda-100924669b72.png)
         
         Based on 50 millions of usage points we built an AI recommender which can predict which technologies for company using a set of technologies. 
         
-        Here are e.g. recommendations for company using Mouse Flow: <table class="table" style="font-size:20px;line-height:30px"><thead><tr><th>Technology</th><th>AI Recommendation Score </th><th>Website</th></tr></thead><tbody><tr><td><a href="https://www.alpha-quantum.com/technologies/AppNexus">AppNexus</a></td><td>0.15</td><td>http://appnexus.com</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/Microsoft Clarity">Microsoft Clarity</a></td><td>0.14</td><td>https://clarity.microsoft.com</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/Osano">Osano</a></td><td>0.14</td><td>https://www.osano.com/</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/Jetpack">Jetpack</a></td><td>0.14</td><td>https://jetpack.com</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/Raphael">Raphael</a></td><td>0.14</td><td>https://dmitrybaranovskiy.github.io/raphael/</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/Svelte">Svelte</a></td><td>0.13</td><td>https://svelte.dev</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/AWS Certificate Manager">AWS Certificate Manager</a></td><td>0.12</td><td>https://aws.amazon.com/certificate-manager/</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/Extendify">Extendify</a></td><td>0.11</td><td>https://extendify.com</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/Kendo UI">Kendo UI</a></td><td>0.11</td><td>https://www.telerik.com/kendo-ui</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/Flywheel">Flywheel</a></td><td>0.11</td><td>https://getflywheel.com</td></tr></tbody></table>
+        Here are e.g. recommendations for company using Mouse Flow: <table class="table" style="font-size:20px;line-height:30px"><thead><tr><th>Technology</th><th>AI Recommendation Score </th><th>Website</th></tr></thead><tbody><tr><td><a href="https://www.alpha-quantum.com/technologies/websites-using-AppNexus">AppNexus</a></td><td>0.15</td><td>http://appnexus.com</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/websites-using-Microsoft Clarity">Microsoft Clarity</a></td><td>0.14</td><td>https://clarity.microsoft.com</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/websites-using-Osano">Osano</a></td><td>0.14</td><td>https://www.osano.com/</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/websites-using-Jetpack">Jetpack</a></td><td>0.14</td><td>https://jetpack.com</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/websites-using-Raphael">Raphael</a></td><td>0.14</td><td>https://dmitrybaranovskiy.github.io/raphael/</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/websites-using-Svelte">Svelte</a></td><td>0.13</td><td>https://svelte.dev</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/websites-using-AWS Certificate Manager">AWS Certificate Manager</a></td><td>0.12</td><td>https://aws.amazon.com/certificate-manager/</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/websites-using-Extendify">Extendify</a></td><td>0.11</td><td>https://extendify.com</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/websites-using-Kendo UI">Kendo UI</a></td><td>0.11</td><td>https://www.telerik.com/kendo-ui</td></tr><tr><td><a href="https://www.alpha-quantum.com/technologies/websites-using-Flywheel">Flywheel</a></td><td>0.11</td><td>https://getflywheel.com</td></tr></tbody></table>
         
         
         
         
         
         ## Example classifications
```

