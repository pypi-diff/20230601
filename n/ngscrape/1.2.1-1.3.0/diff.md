# Comparing `tmp/ngscrape-1.2.1.tar.gz` & `tmp/ngscrape-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngscrape-1.2.1.tar", last modified: Wed May 31 00:39:59 2023, max compression
+gzip compressed data, was "ngscrape-1.3.0.tar", last modified: Wed May 31 22:33:19 2023, max compression
```

## Comparing `ngscrape-1.2.1.tar` & `ngscrape-1.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 00:39:59.562269 ngscrape-1.2.1/
--rw-rw-rw-   0        0        0    35184 2023-05-27 22:41:04.000000 ngscrape-1.2.1/LICENSE
--rw-rw-rw-   0        0        0    43961 2023-05-31 00:39:59.561262 ngscrape-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      738 2023-05-31 00:36:52.000000 ngscrape-1.2.1/pyproject.toml
--rw-rw-rw-   0        0        0     2924 2023-05-31 00:39:25.000000 ngscrape-1.2.1/readme.md
--rw-rw-rw-   0        0        0       42 2023-05-31 00:39:59.563262 ngscrape-1.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-31 00:39:59.528265 ngscrape-1.2.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-31 00:39:59.534277 ngscrape-1.2.1/src/ngscrape/
--rw-rw-rw-   0        0        0     7907 2023-05-31 00:38:10.000000 ngscrape-1.2.1/src/ngscrape/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 00:39:59.559283 ngscrape-1.2.1/src/ngscrape.egg-info/
--rw-rw-rw-   0        0        0    43961 2023-05-31 00:39:59.000000 ngscrape-1.2.1/src/ngscrape.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-05-31 00:39:59.000000 ngscrape-1.2.1/src/ngscrape.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 00:39:59.000000 ngscrape-1.2.1/src/ngscrape.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-05-31 00:39:59.000000 ngscrape-1.2.1/src/ngscrape.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-31 00:39:59.000000 ngscrape-1.2.1/src/ngscrape.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 22:33:18.998954 ngscrape-1.3.0/
+-rw-rw-rw-   0        0        0    35184 2023-05-27 22:41:04.000000 ngscrape-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0    44094 2023-05-31 22:33:18.997950 ngscrape-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      738 2023-05-31 22:32:59.000000 ngscrape-1.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0     3057 2023-05-31 22:32:29.000000 ngscrape-1.3.0/readme.md
+-rw-rw-rw-   0        0        0       42 2023-05-31 22:33:18.998954 ngscrape-1.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-31 22:33:18.960959 ngscrape-1.3.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-31 22:33:18.968954 ngscrape-1.3.0/src/ngscrape/
+-rw-rw-rw-   0        0        0    11108 2023-05-31 22:32:32.000000 ngscrape-1.3.0/src/ngscrape/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 22:33:18.994953 ngscrape-1.3.0/src/ngscrape.egg-info/
+-rw-rw-rw-   0        0        0    44094 2023-05-31 22:33:18.000000 ngscrape-1.3.0/src/ngscrape.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-05-31 22:33:18.000000 ngscrape-1.3.0/src/ngscrape.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 22:33:18.000000 ngscrape-1.3.0/src/ngscrape.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-31 22:33:18.000000 ngscrape-1.3.0/src/ngscrape.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-31 22:33:18.000000 ngscrape-1.3.0/src/ngscrape.egg-info/top_level.txt
```

### Comparing `ngscrape-1.2.1/LICENSE` & `ngscrape-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ngscrape-1.2.1/PKG-INFO` & `ngscrape-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngscrape
-Version: 1.2.1
+Version: 1.3.0
 Summary: Newgrounds flash game scraper powered by bs4 and requests
 Author-email: aeiea <dpthn@proton.me>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -680,14 +680,17 @@
 NGScrape is licensed under the GNU Affero General Public License v3.0. If a copy is not included with this file, you can find one at https://www.gnu.org/licenses/agpl-3.0.en.html.
 
 Please star is this was useful!
 
 Functions:
 - `__init__(debug: bool = False) -> None`
     - Start a new NGScrape Instance.
+    - Parameters:
+        - debug (bool) = False: Enable/Disable debug mode
+        - cache (bool) = False: Enable/Disable caching
 - `scrape_game_by_url(url: str, download: str, filename: str) -> None`
     - Scrape a flash game by url.
     - Parameters:
         - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
         - download (str): The directory to download the file to.
         - filename (str): The name of the downloaded file.
     - Example parameters:
@@ -700,15 +703,15 @@
         - NGScrape: Downloaded swf file to testdir/game.swf
 - `scrape_desc_by_url(self, url: str) -> str`
     - Scrape a flash game's description by url. Returns the description of the game.
     - Parameters:
         - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
     - Example parameters:
         - `url = 'https://www.newgrounds.com/portal/view/59593'`
-    - Example output with debug mode:`
+    - Example output with debug mode:
         - NGScrape: Made request to `https://www.newgrounds.com/portal/view/59593` and got status code `200`
         - NGScrape: Found game description "Blast FBI agents in this Metal Slug style shooter!"
 - `scrape_card_by_url(self, url: str, download: str, filename: str) -> str`
     - Scrape a flash game's card by url. The file extention will be automatically determined. Returns the name of the card file.
     - Parameters:
         - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
         - download (str): The directory to download the file to.
@@ -716,8 +719,8 @@
     - Example parameters:
         - `url = 'https://www.newgrounds.com/portal/view/59593'`
         - `download = 'testdir'`
         - `filename = 'card'`
     - Example output with debug mode:
         - NGScrape: Made request to `https://www.newgrounds.com/portal/view/59593` and got status code `200`
         - NGScrape: Found card link `https://picon.ngfiles.com/59000/flash_59593_card.png?f1607717241`
-        - NGScrape: Downloaded `swf` file to `testdir/card.png`
+        - NGScrape: Downloaded `png` file to `testdir/card.png`
```

### Comparing `ngscrape-1.2.1/pyproject.toml` & `ngscrape-1.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "ngscrape"
-version = "1.2.1"
+version = "1.3.0"
 description = "Newgrounds flash game scraper powered by bs4 and requests"
 readme = "readme.md"
 authors = [{ name = "aeiea", email = "dpthn@proton.me" }]
 license = {file = "LICENSE"}
 classifiers = [
     "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
     "Programming Language :: Python",
```

### Comparing `ngscrape-1.2.1/readme.md` & `ngscrape-1.3.0/readme.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 NGScrape is licensed under the GNU Affero General Public License v3.0. If a copy is not included with this file, you can find one at https://www.gnu.org/licenses/agpl-3.0.en.html.
 
 Please star is this was useful!
 
 Functions:
 - `__init__(debug: bool = False) -> None`
     - Start a new NGScrape Instance.
+    - Parameters:
+        - debug (bool) = False: Enable/Disable debug mode
+        - cache (bool) = False: Enable/Disable caching
 - `scrape_game_by_url(url: str, download: str, filename: str) -> None`
     - Scrape a flash game by url.
     - Parameters:
         - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
         - download (str): The directory to download the file to.
         - filename (str): The name of the downloaded file.
     - Example parameters:
@@ -24,15 +27,15 @@
         - NGScrape: Downloaded swf file to testdir/game.swf
 - `scrape_desc_by_url(self, url: str) -> str`
     - Scrape a flash game's description by url. Returns the description of the game.
     - Parameters:
         - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
     - Example parameters:
         - `url = 'https://www.newgrounds.com/portal/view/59593'`
-    - Example output with debug mode:`
+    - Example output with debug mode:
         - NGScrape: Made request to `https://www.newgrounds.com/portal/view/59593` and got status code `200`
         - NGScrape: Found game description "Blast FBI agents in this Metal Slug style shooter!"
 - `scrape_card_by_url(self, url: str, download: str, filename: str) -> str`
     - Scrape a flash game's card by url. The file extention will be automatically determined. Returns the name of the card file.
     - Parameters:
         - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
         - download (str): The directory to download the file to.
@@ -40,8 +43,8 @@
     - Example parameters:
         - `url = 'https://www.newgrounds.com/portal/view/59593'`
         - `download = 'testdir'`
         - `filename = 'card'`
     - Example output with debug mode:
         - NGScrape: Made request to `https://www.newgrounds.com/portal/view/59593` and got status code `200`
         - NGScrape: Found card link `https://picon.ngfiles.com/59000/flash_59593_card.png?f1607717241`
-        - NGScrape: Downloaded `swf` file to `testdir/card.png`
+        - NGScrape: Downloaded `png` file to `testdir/card.png`
```

### Comparing `ngscrape-1.2.1/src/ngscrape.egg-info/PKG-INFO` & `ngscrape-1.3.0/src/ngscrape.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngscrape
-Version: 1.2.1
+Version: 1.3.0
 Summary: Newgrounds flash game scraper powered by bs4 and requests
 Author-email: aeiea <dpthn@proton.me>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -680,14 +680,17 @@
 NGScrape is licensed under the GNU Affero General Public License v3.0. If a copy is not included with this file, you can find one at https://www.gnu.org/licenses/agpl-3.0.en.html.
 
 Please star is this was useful!
 
 Functions:
 - `__init__(debug: bool = False) -> None`
     - Start a new NGScrape Instance.
+    - Parameters:
+        - debug (bool) = False: Enable/Disable debug mode
+        - cache (bool) = False: Enable/Disable caching
 - `scrape_game_by_url(url: str, download: str, filename: str) -> None`
     - Scrape a flash game by url.
     - Parameters:
         - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
         - download (str): The directory to download the file to.
         - filename (str): The name of the downloaded file.
     - Example parameters:
@@ -700,15 +703,15 @@
         - NGScrape: Downloaded swf file to testdir/game.swf
 - `scrape_desc_by_url(self, url: str) -> str`
     - Scrape a flash game's description by url. Returns the description of the game.
     - Parameters:
         - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
     - Example parameters:
         - `url = 'https://www.newgrounds.com/portal/view/59593'`
-    - Example output with debug mode:`
+    - Example output with debug mode:
         - NGScrape: Made request to `https://www.newgrounds.com/portal/view/59593` and got status code `200`
         - NGScrape: Found game description "Blast FBI agents in this Metal Slug style shooter!"
 - `scrape_card_by_url(self, url: str, download: str, filename: str) -> str`
     - Scrape a flash game's card by url. The file extention will be automatically determined. Returns the name of the card file.
     - Parameters:
         - url (str): The URL of the flash game. For example, the URL for Alien Homonid is `https://www.newgrounds.com/portal/view/59593`.
         - download (str): The directory to download the file to.
@@ -716,8 +719,8 @@
     - Example parameters:
         - `url = 'https://www.newgrounds.com/portal/view/59593'`
         - `download = 'testdir'`
         - `filename = 'card'`
     - Example output with debug mode:
         - NGScrape: Made request to `https://www.newgrounds.com/portal/view/59593` and got status code `200`
         - NGScrape: Found card link `https://picon.ngfiles.com/59000/flash_59593_card.png?f1607717241`
-        - NGScrape: Downloaded `swf` file to `testdir/card.png`
+        - NGScrape: Downloaded `png` file to `testdir/card.png`
```

