# Comparing `tmp/matchscraper-0.2.1.tar.gz` & `tmp/matchscraper-0.2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matchscraper-0.2.1.tar", last modified: Thu Jun  1 08:00:00 2023, max compression
+gzip compressed data, was "matchscraper-0.2.1.1.tar", last modified: Thu Jun  1 10:35:55 2023, max compression
```

## Comparing `matchscraper-0.2.1.tar` & `matchscraper-0.2.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 claromes  (1000) claromes  (1000)        0 2023-06-01 08:00:00.466453 matchscraper-0.2.1/
--rw-r--r--   0 claromes  (1000) claromes  (1000)       18 2023-06-01 07:10:51.000000 matchscraper-0.2.1/MANIFEST.in
--rw-r--r--   0 claromes  (1000) claromes  (1000)     2693 2023-06-01 08:00:00.466453 matchscraper-0.2.1/PKG-INFO
--rw-r--r--   0 claromes  (1000) claromes  (1000)     1106 2023-06-01 07:29:09.000000 matchscraper-0.2.1/README.md
-drwxr-xr-x   0 claromes  (1000) claromes  (1000)        0 2023-06-01 08:00:00.466453 matchscraper-0.2.1/matchscraper/
--rw-r--r--   0 claromes  (1000) claromes  (1000)        0 2023-05-30 03:08:55.000000 matchscraper-0.2.1/matchscraper/__init__.py
--rw-r--r--   0 claromes  (1000) claromes  (1000)     1446 2023-06-01 07:29:09.000000 matchscraper-0.2.1/matchscraper/__main__.py
--rw-r--r--   0 claromes  (1000) claromes  (1000)      268 2023-05-30 03:08:55.000000 matchscraper-0.2.1/matchscraper/items.py
--rw-r--r--   0 claromes  (1000) claromes  (1000)     3660 2023-05-30 03:08:55.000000 matchscraper-0.2.1/matchscraper/middlewares.py
--rw-r--r--   0 claromes  (1000) claromes  (1000)      366 2023-05-30 03:08:55.000000 matchscraper-0.2.1/matchscraper/pipelines.py
--rw-r--r--   0 claromes  (1000) claromes  (1000)     3317 2023-06-01 07:29:09.000000 matchscraper-0.2.1/matchscraper/settings.py
-drwxr-xr-x   0 claromes  (1000) claromes  (1000)        0 2023-06-01 08:00:00.466453 matchscraper-0.2.1/matchscraper/spiders/
--rw-r--r--   0 claromes  (1000) claromes  (1000)      161 2023-05-30 03:08:55.000000 matchscraper-0.2.1/matchscraper/spiders/__init__.py
--rw-r--r--   0 claromes  (1000) claromes  (1000)     1658 2023-06-01 07:29:09.000000 matchscraper-0.2.1/matchscraper/spiders/competition.py
--rw-r--r--   0 claromes  (1000) claromes  (1000)     5136 2023-06-01 07:29:09.000000 matchscraper-0.2.1/matchscraper/spiders/match.py
--rw-r--r--   0 claromes  (1000) claromes  (1000)     1620 2023-06-01 07:29:09.000000 matchscraper-0.2.1/matchscraper/utils.py
--rw-r--r--   0 claromes  (1000) claromes  (1000)       21 2023-06-01 07:57:54.000000 matchscraper-0.2.1/matchscraper/version.py
-drwxr-xr-x   0 claromes  (1000) claromes  (1000)        0 2023-06-01 08:00:00.466453 matchscraper-0.2.1/matchscraper.egg-info/
--rw-r--r--   0 claromes  (1000) claromes  (1000)     2693 2023-06-01 08:00:00.000000 matchscraper-0.2.1/matchscraper.egg-info/PKG-INFO
--rw-r--r--   0 claromes  (1000) claromes  (1000)      555 2023-06-01 08:00:00.000000 matchscraper-0.2.1/matchscraper.egg-info/SOURCES.txt
--rw-r--r--   0 claromes  (1000) claromes  (1000)        1 2023-06-01 08:00:00.000000 matchscraper-0.2.1/matchscraper.egg-info/dependency_links.txt
--rw-r--r--   0 claromes  (1000) claromes  (1000)       56 2023-06-01 08:00:00.000000 matchscraper-0.2.1/matchscraper.egg-info/entry_points.txt
--rw-r--r--   0 claromes  (1000) claromes  (1000)       14 2023-06-01 08:00:00.000000 matchscraper-0.2.1/matchscraper.egg-info/requires.txt
--rw-r--r--   0 claromes  (1000) claromes  (1000)       13 2023-06-01 08:00:00.000000 matchscraper-0.2.1/matchscraper.egg-info/top_level.txt
--rw-r--r--   0 claromes  (1000) claromes  (1000)      267 2023-05-30 03:08:55.000000 matchscraper-0.2.1/scrapy.cfg
--rw-r--r--   0 claromes  (1000) claromes  (1000)       38 2023-06-01 08:00:00.476453 matchscraper-0.2.1/setup.cfg
--rw-r--r--   0 claromes  (1000) claromes  (1000)     1762 2023-06-01 07:57:16.000000 matchscraper-0.2.1/setup.py
+drwxr-xr-x   0 claromes  (1000) claromes  (1000)        0 2023-06-01 10:35:55.476300 matchscraper-0.2.1.1/
+-rw-r--r--   0 claromes  (1000) claromes  (1000)       18 2023-06-01 07:10:51.000000 matchscraper-0.2.1.1/MANIFEST.in
+-rw-r--r--   0 claromes  (1000) claromes  (1000)     3186 2023-06-01 10:35:55.476300 matchscraper-0.2.1.1/PKG-INFO
+-rw-r--r--   0 claromes  (1000) claromes  (1000)     1501 2023-06-01 10:32:04.000000 matchscraper-0.2.1.1/README.md
+drwxr-xr-x   0 claromes  (1000) claromes  (1000)        0 2023-06-01 10:35:55.476300 matchscraper-0.2.1.1/matchscraper/
+-rw-r--r--   0 claromes  (1000) claromes  (1000)        0 2023-05-30 03:08:55.000000 matchscraper-0.2.1.1/matchscraper/__init__.py
+-rw-r--r--   0 claromes  (1000) claromes  (1000)      268 2023-05-30 03:08:55.000000 matchscraper-0.2.1.1/matchscraper/items.py
+-rw-r--r--   0 claromes  (1000) claromes  (1000)     1988 2023-06-01 10:26:07.000000 matchscraper-0.2.1.1/matchscraper/main.py
+-rw-r--r--   0 claromes  (1000) claromes  (1000)     3660 2023-05-30 03:08:55.000000 matchscraper-0.2.1.1/matchscraper/middlewares.py
+-rw-r--r--   0 claromes  (1000) claromes  (1000)      366 2023-05-30 03:08:55.000000 matchscraper-0.2.1.1/matchscraper/pipelines.py
+-rw-r--r--   0 claromes  (1000) claromes  (1000)     3317 2023-06-01 07:29:09.000000 matchscraper-0.2.1.1/matchscraper/settings.py
+drwxr-xr-x   0 claromes  (1000) claromes  (1000)        0 2023-06-01 10:35:55.476300 matchscraper-0.2.1.1/matchscraper/spiders/
+-rw-r--r--   0 claromes  (1000) claromes  (1000)      161 2023-05-30 03:08:55.000000 matchscraper-0.2.1.1/matchscraper/spiders/__init__.py
+-rw-r--r--   0 claromes  (1000) claromes  (1000)     1662 2023-06-01 10:05:53.000000 matchscraper-0.2.1.1/matchscraper/spiders/competition.py
+-rw-r--r--   0 claromes  (1000) claromes  (1000)     5144 2023-06-01 10:08:33.000000 matchscraper-0.2.1.1/matchscraper/spiders/match.py
+-rw-r--r--   0 claromes  (1000) claromes  (1000)     1620 2023-06-01 07:29:09.000000 matchscraper-0.2.1.1/matchscraper/utils.py
+-rw-r--r--   0 claromes  (1000) claromes  (1000)       23 2023-06-01 09:01:15.000000 matchscraper-0.2.1.1/matchscraper/version.py
+drwxr-xr-x   0 claromes  (1000) claromes  (1000)        0 2023-06-01 10:35:55.476300 matchscraper-0.2.1.1/matchscraper.egg-info/
+-rw-r--r--   0 claromes  (1000) claromes  (1000)     3186 2023-06-01 10:35:55.000000 matchscraper-0.2.1.1/matchscraper.egg-info/PKG-INFO
+-rw-r--r--   0 claromes  (1000) claromes  (1000)      551 2023-06-01 10:35:55.000000 matchscraper-0.2.1.1/matchscraper.egg-info/SOURCES.txt
+-rw-r--r--   0 claromes  (1000) claromes  (1000)        1 2023-06-01 10:35:55.000000 matchscraper-0.2.1.1/matchscraper.egg-info/dependency_links.txt
+-rw-r--r--   0 claromes  (1000) claromes  (1000)       57 2023-06-01 10:35:55.000000 matchscraper-0.2.1.1/matchscraper.egg-info/entry_points.txt
+-rw-r--r--   0 claromes  (1000) claromes  (1000)       14 2023-06-01 10:35:55.000000 matchscraper-0.2.1.1/matchscraper.egg-info/requires.txt
+-rw-r--r--   0 claromes  (1000) claromes  (1000)       13 2023-06-01 10:35:55.000000 matchscraper-0.2.1.1/matchscraper.egg-info/top_level.txt
+-rw-r--r--   0 claromes  (1000) claromes  (1000)      267 2023-05-30 03:08:55.000000 matchscraper-0.2.1.1/scrapy.cfg
+-rw-r--r--   0 claromes  (1000) claromes  (1000)       38 2023-06-01 10:35:55.476300 matchscraper-0.2.1.1/setup.cfg
+-rw-r--r--   0 claromes  (1000) claromes  (1000)     1763 2023-06-01 10:24:34.000000 matchscraper-0.2.1.1/setup.py
```

### Comparing `matchscraper-0.2.1/PKG-INFO` & `matchscraper-0.2.1.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matchscraper
-Version: 0.2.1
+Version: 0.2.1.1
 Summary: CLI tool to get volleyball match statistics from the Web Competition by Data Project websites
 Home-page: https://github.com/claromes/matchscraper
 Author: claromes
 License: UNKNOWN
 Project-URL: Documentation, https://claromes.github.io/matchscraper/
 Project-URL: Issue Tracker, https://github.com/claromes/matchscraper/issues
 Description: # Matchscraper
@@ -22,19 +22,31 @@
         ## Installation
         
         ```shell
         pip3 install matchscraper
         ```
         
         ## Usage
-        ```shell
+        ```
         matchscraper --fed cbv --match 1623
         ```
         
-        ```shell
+        ```
+                            .
+                            |`.
+                            |  `.
+                            |-_  `.
+                            |  -_  `._
+        ____________________|____-_ _|_______________,
+        ',                         -_|                ',
+          ',                         |                  ',
+            ',                       |                    ',
+              ',_____________________|______________________',
+        	    Matchscraper
+        
         Matchscraper: started!
         
         Matchscraper: data/1623_22-10-28_home_fluminense.csv file was created!
         
         Matchscraper: data/1623_22-10-28_guest_barueri-volleyball-club.csv file was created!
         
         Matchscraper: finished!
```

### Comparing `matchscraper-0.2.1/matchscraper/middlewares.py` & `matchscraper-0.2.1.1/matchscraper/middlewares.py`

 * *Files identical despite different names*

### Comparing `matchscraper-0.2.1/matchscraper/settings.py` & `matchscraper-0.2.1.1/matchscraper/settings.py`

 * *Files identical despite different names*

### Comparing `matchscraper-0.2.1/matchscraper/spiders/competition.py` & `matchscraper-0.2.1.1/matchscraper/spiders/competition.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,10 +34,10 @@
     def closed(spider, reason):
         src = 'data/competition_matches.csv'
         dst = 'data/{}_competition_matches.csv'.format(spider.competition_id)
 
         try:
             os.rename(src, dst)
 
-            print('\x1b[6;30;42m' + '\nMatchscraper: {} file was created!'.format(dst) + '\x1b[0m\n')
+            print('\x1b[6;30;42m' + '\n Matchscraper: {} file was created! '.format(dst) + '\x1b[0m\n')
         except(FileExistsError):
-            print('\x1b[6;30;43m' + '\nMatchscraper: file {} already exists.\n{} was created or renamed!'.format(dst, src) + '\x1b[0m\n')
+            print('\x1b[6;30;43m' + '\n Matchscraper: file {} already exists.\n{} was created or renamed! '.format(dst, src) + '\x1b[0m\n')
```

### Comparing `matchscraper-0.2.1/matchscraper/spiders/match.py` & `matchscraper-0.2.1.1/matchscraper/spiders/match.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,17 +56,17 @@
     def closed(spider, reason):
         src = 'data/home_stats.csv'
         dst = 'data/{}-{}-home-{}.csv'.format(spider.match_id, spider.match_date, spider.home_team)
 
         try:
             os.rename(src, dst)
 
-            print('\x1b[6;30;42m' + '\nMatchscraper: {} file was created!'.format(dst) + '\x1b[0m\n')
+            print('\x1b[6;30;42m' + '\n Matchscraper: {} file was created! '.format(dst) + '\x1b[0m\n')
         except(FileExistsError):
-            print('\x1b[6;30;43m' + '\nMatchscraper: file {} already exists.\n{} was created or renamed!'.format(dst, src) + '\x1b[0m\n')
+            print('\x1b[6;30;43m' + '\n Matchscraper: file {} already exists.\n{} was created or renamed! '.format(dst, src) + '\x1b[0m\n')
 
 class GuestStatsSpider(scrapy.Spider):
     name = 'guest_stats'
 
     def __init__(self, fed_acronym='', match_id='', **kwargs):
         self.start_urls = [f'https://{fed_acronym}-web.dataproject.com/MatchStatistics.aspx?mID={match_id}']
         self.match_id = match_id
@@ -115,10 +115,10 @@
     def closed(spider, reason):
         src = 'data/guest_stats.csv'
         dst = 'data/{}-{}-guest-{}.csv'.format(spider.match_id, spider.match_date, spider.guest_team)
 
         try:
             os.rename(src, dst)
 
-            print('\x1b[6;30;42m' + '\nMatchscraper: {} file was created!'.format(dst) + '\x1b[0m\n')
+            print('\x1b[6;30;42m' + '\n Matchscraper: {} file was created! '.format(dst) + '\x1b[0m\n')
         except(FileExistsError):
-            print('\x1b[6;30;43m' + '\nMatchscraper: file {} already exists.\n{} was created or renamed!'.format(dst, src) + '\x1b[0m\n')
+            print('\x1b[6;30;43m' + '\n Matchscraper: file {} already exists.\n{} was created or renamed! '.format(dst, src) + '\x1b[0m\n')
```

### Comparing `matchscraper-0.2.1/matchscraper/utils.py` & `matchscraper-0.2.1.1/matchscraper/utils.py`

 * *Files identical despite different names*

### Comparing `matchscraper-0.2.1/matchscraper.egg-info/PKG-INFO` & `matchscraper-0.2.1.1/matchscraper.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matchscraper
-Version: 0.2.1
+Version: 0.2.1.1
 Summary: CLI tool to get volleyball match statistics from the Web Competition by Data Project websites
 Home-page: https://github.com/claromes/matchscraper
 Author: claromes
 License: UNKNOWN
 Project-URL: Documentation, https://claromes.github.io/matchscraper/
 Project-URL: Issue Tracker, https://github.com/claromes/matchscraper/issues
 Description: # Matchscraper
@@ -22,19 +22,31 @@
         ## Installation
         
         ```shell
         pip3 install matchscraper
         ```
         
         ## Usage
-        ```shell
+        ```
         matchscraper --fed cbv --match 1623
         ```
         
-        ```shell
+        ```
+                            .
+                            |`.
+                            |  `.
+                            |-_  `.
+                            |  -_  `._
+        ____________________|____-_ _|_______________,
+        ',                         -_|                ',
+          ',                         |                  ',
+            ',                       |                    ',
+              ',_____________________|______________________',
+        	    Matchscraper
+        
         Matchscraper: started!
         
         Matchscraper: data/1623_22-10-28_home_fluminense.csv file was created!
         
         Matchscraper: data/1623_22-10-28_guest_barueri-volleyball-club.csv file was created!
         
         Matchscraper: finished!
```

### Comparing `matchscraper-0.2.1/matchscraper.egg-info/SOURCES.txt` & `matchscraper-0.2.1.1/matchscraper.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 MANIFEST.in
 README.md
 scrapy.cfg
 setup.py
 matchscraper/__init__.py
-matchscraper/__main__.py
 matchscraper/items.py
+matchscraper/main.py
 matchscraper/middlewares.py
 matchscraper/pipelines.py
 matchscraper/settings.py
 matchscraper/utils.py
 matchscraper/version.py
 matchscraper.egg-info/PKG-INFO
 matchscraper.egg-info/SOURCES.txt
```

### Comparing `matchscraper-0.2.1/setup.py` & `matchscraper-0.2.1.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -39,11 +39,11 @@
         'Topic :: Scientific/Engineering :: Information Analysis',
         'Topic :: Utilities'
     ],
     python_requires='>=3.8',
     install_requires=install_requires,
     entry_points = {
 		'console_scripts': [
-			'matchscraper = matchscraper:__main__',
+			'matchscraper = matchscraper.main:main',
 		],
 	},
 )
```

