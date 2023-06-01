# Comparing `tmp/animegifs-0.5.4.tar.gz` & `tmp/animegifs-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "animegifs-0.5.4.tar", last modified: Tue May 23 23:33:14 2023, max compression
+gzip compressed data, was "animegifs-0.6.0.tar", last modified: Thu Jun  1 17:23:04 2023, max compression
```

## Comparing `animegifs-0.5.4.tar` & `animegifs-0.6.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 23:33:14.481083 animegifs-0.5.4/
--rw-rw-rw-   0        0        0     1086 2022-05-19 16:45:41.000000 animegifs-0.5.4/LICENSE
--rw-rw-rw-   0        0        0     1258 2023-05-23 23:33:14.480082 animegifs-0.5.4/PKG-INFO
--rw-rw-rw-   0        0        0      662 2023-05-23 16:46:53.000000 animegifs-0.5.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 23:33:14.460080 animegifs-0.5.4/animegifs/
--rw-rw-rw-   0        0        0        0 2023-05-09 23:54:36.000000 animegifs-0.5.4/animegifs/__init__.py
--rw-rw-rw-   0        0        0     1096 2023-05-23 16:46:53.000000 animegifs-0.5.4/animegifs/animegifs.py
-drwxrwxrwx   0        0        0        0 2023-05-23 23:33:14.478085 animegifs-0.5.4/animegifs/distutils/
--rw-rw-rw-   0        0        0        0 2023-05-09 23:54:59.000000 animegifs-0.5.4/animegifs/distutils/__init__.py
--rw-rw-rw-   0        0        0     1186 2023-05-10 14:18:41.000000 animegifs-0.5.4/animegifs/distutils/errors.py
--rw-rw-rw-   0        0        0      779 2023-05-23 16:46:53.000000 animegifs-0.5.4/animegifs/distutils/gifs.py
-drwxrwxrwx   0        0        0        0 2023-05-23 23:33:14.469081 animegifs-0.5.4/animegifs.egg-info/
--rw-rw-rw-   0        0        0     1258 2023-05-23 23:33:14.000000 animegifs-0.5.4/animegifs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      325 2023-05-23 23:33:14.000000 animegifs-0.5.4/animegifs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 23:33:14.000000 animegifs-0.5.4/animegifs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-05-23 23:33:14.000000 animegifs-0.5.4/animegifs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-23 23:33:14.000000 animegifs-0.5.4/animegifs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-23 23:33:14.481083 animegifs-0.5.4/setup.cfg
--rw-rw-rw-   0        0        0     1072 2023-05-23 16:46:53.000000 animegifs-0.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 17:23:04.551180 animegifs-0.6.0/
+-rw-rw-rw-   0        0        0     1086 2022-05-19 16:45:41.000000 animegifs-0.6.0/LICENSE
+-rw-rw-rw-   0        0        0     1968 2023-06-01 17:23:04.550180 animegifs-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1338 2023-06-01 16:28:39.000000 animegifs-0.6.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 17:23:04.532178 animegifs-0.6.0/animegifs/
+-rw-rw-rw-   0        0        0        0 2023-05-09 23:54:36.000000 animegifs-0.6.0/animegifs/__init__.py
+-rw-rw-rw-   0        0        0     3316 2023-06-01 16:13:07.000000 animegifs-0.6.0/animegifs/animegifs.py
+drwxrwxrwx   0        0        0        0 2023-06-01 17:23:04.548180 animegifs-0.6.0/animegifs/distutils/
+-rw-rw-rw-   0        0        0        0 2023-05-09 23:54:59.000000 animegifs-0.6.0/animegifs/distutils/__init__.py
+-rw-rw-rw-   0        0        0     1586 2023-06-01 16:01:08.000000 animegifs-0.6.0/animegifs/distutils/errors.py
+-rw-rw-rw-   0        0        0     1418 2023-06-01 16:28:39.000000 animegifs-0.6.0/animegifs/distutils/gifs.py
+drwxrwxrwx   0        0        0        0 2023-06-01 17:23:04.540181 animegifs-0.6.0/animegifs.egg-info/
+-rw-rw-rw-   0        0        0     1968 2023-06-01 17:23:04.000000 animegifs-0.6.0/animegifs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      325 2023-06-01 17:23:04.000000 animegifs-0.6.0/animegifs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 17:23:04.000000 animegifs-0.6.0/animegifs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-06-01 17:23:04.000000 animegifs-0.6.0/animegifs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-01 17:23:04.000000 animegifs-0.6.0/animegifs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 17:23:04.551180 animegifs-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1130 2023-06-01 16:46:00.000000 animegifs-0.6.0/setup.py
```

### Comparing `animegifs-0.5.4/LICENSE` & `animegifs-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `animegifs-0.5.4/PKG-INFO` & `animegifs-0.6.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animegifs
-Version: 0.5.4
+Version: 0.6.0
 Summary: Get random anime gifs by category.
 Home-page: https://github.com/MarcoSa-2000/animegifs
 Author: Marco-Sa2000
 Author-email: grest0grest@gmail.com
 License: MIT
 Keywords: anime,gif,python,anime-gif,discord
 Platform: UNKNOWN
@@ -15,27 +15,38 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # animegifs.py
 Get random anime gifs by category. Use Python (intended (for now) for Discord).
 
-WIP - updated in time to time. Versions below v0.5.3 aren't expected to work flawlessly or at all.
+WIP - updated in time to time. Versions below v0.5.3 aren't expected to work flawlessly or at all. Version below v0.6 will not have the gifs library updated anymore.
 
 `pip install animegifs`
 
 # HOW TO USE
-
 ```py
+#v0.5.3>
+from animegifs import animegifs
 
+gifs = animegifs.Animegifs()
+
+gif = gifs.get_gif(category) #return the url of the gif.
+```
+
+```py
+#v0.6>
 from animegifs import animegifs
 
 gifs = animegifs.Animegifs()
 
-gif = gifs.get_gif(category)
+gif = gifs.get_gif(category) #return the url of the gif.
+mal = gifs.get_mal(gif) #get url of the gif's anime myanimelist page.
+title = gifs.get_animetitle(gif) #get the title of the gif's anime.
+malid = gifs.get_malId(gif) #get the ID of the gif's anime myanimelist page.
 ```
 
 **Category list:** 
 
 * Attack
 * Bite
 * Bloodsuck
@@ -60,11 +71,34 @@
 * Kill
 * Kiss
 * Lick
 * Love
 * Marry
 * Nosebleed
 * Nuzzle
+* Pat
+* Peck
+* Poke
+* Popcorn
+* Pout
+* Punch
+* Punish
+* Run
+* Sad
+* Scared
+* Shoot
+* Shrug
+* Sip
+* Slap
+* Smirk
+* Sorry
+* Spank
+* Stare
+
+**Special Category List**
+
+* Random
+* Steal-magic
 
 WIP.
```

### Comparing `animegifs-0.5.4/animegifs/distutils/errors.py` & `animegifs-0.6.0/animegifs/distutils/errors.py`

 * *Files 25% similar despite different names*

```diff
@@ -27,7 +27,18 @@
     You can check valid categories at: https://github.com/MarcoSa-2000/animegifs
     """
 
     def __init__(self, category, error="Not a valid category."):
         self.category = category
         self.error = error
         super().__init__(self.error)
+
+class MethodNotUpdated(Exception):
+    """
+    The method for get the gif's <title, mal link, mal id> is not yet supported for that gif url.
+    Usually means is just in work in progress and will be available soon.
+    """
+
+    def __init__(self, gif, error="Method not yet available for this gif."):
+        self.gif = gif
+        self.error = error
+        super().__init__(self.error)
```

### Comparing `animegifs-0.5.4/animegifs.egg-info/PKG-INFO` & `animegifs-0.6.0/animegifs.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animegifs
-Version: 0.5.4
+Version: 0.6.0
 Summary: Get random anime gifs by category.
 Home-page: https://github.com/MarcoSa-2000/animegifs
 Author: Marco-Sa2000
 Author-email: grest0grest@gmail.com
 License: MIT
 Keywords: anime,gif,python,anime-gif,discord
 Platform: UNKNOWN
@@ -15,27 +15,38 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # animegifs.py
 Get random anime gifs by category. Use Python (intended (for now) for Discord).
 
-WIP - updated in time to time. Versions below v0.5.3 aren't expected to work flawlessly or at all.
+WIP - updated in time to time. Versions below v0.5.3 aren't expected to work flawlessly or at all. Version below v0.6 will not have the gifs library updated anymore.
 
 `pip install animegifs`
 
 # HOW TO USE
-
 ```py
+#v0.5.3>
+from animegifs import animegifs
 
+gifs = animegifs.Animegifs()
+
+gif = gifs.get_gif(category) #return the url of the gif.
+```
+
+```py
+#v0.6>
 from animegifs import animegifs
 
 gifs = animegifs.Animegifs()
 
-gif = gifs.get_gif(category)
+gif = gifs.get_gif(category) #return the url of the gif.
+mal = gifs.get_mal(gif) #get url of the gif's anime myanimelist page.
+title = gifs.get_animetitle(gif) #get the title of the gif's anime.
+malid = gifs.get_malId(gif) #get the ID of the gif's anime myanimelist page.
 ```
 
 **Category list:** 
 
 * Attack
 * Bite
 * Bloodsuck
@@ -60,11 +71,34 @@
 * Kill
 * Kiss
 * Lick
 * Love
 * Marry
 * Nosebleed
 * Nuzzle
+* Pat
+* Peck
+* Poke
+* Popcorn
+* Pout
+* Punch
+* Punish
+* Run
+* Sad
+* Scared
+* Shoot
+* Shrug
+* Sip
+* Slap
+* Smirk
+* Sorry
+* Spank
+* Stare
+
+**Special Category List**
+
+* Random
+* Steal-magic
 
 WIP.
```

### Comparing `animegifs-0.5.4/setup.py` & `animegifs-0.6.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,30 +4,32 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 LONG_DESCRIPTION = long_description
-VERSION = '0.5.4'
+VERSION = '0.6.0'
 
 setup(
     name='animegifs',
     package_dir={"anime_gifs": "animegifs"},
     packages=["animegifs", "animegifs.distutils"],
     version=VERSION,
     description='Get random anime gifs by category.',
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     author='Marco-Sa2000',
     author_email='grest0grest@gmail.com',
     license='MIT',
     url="https://github.com/MarcoSa-2000/animegifs",
     install_requires=[
-       'requests==2.28.2,<=2.29.0'
+       'requests==2.28.2,<=2.29.0',
+       'mal-api==0.5.3',
+       'PyJWT>=2.4.0,<=2.7.0'
     ],
     python_requires='>=3.8',
     classifiers=[
         "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: MIT License",
         "Operating System :: Microsoft :: Windows"],
     keywords=['anime', 'gif', 'python', 'anime-gif', 'discord'],
```

