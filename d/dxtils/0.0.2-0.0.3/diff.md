# Comparing `tmp/dxtils-0.0.2.tar.gz` & `tmp/dxtils-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxtils-0.0.2.tar", last modified: Wed May 31 18:32:09 2023, max compression
+gzip compressed data, was "dxtils-0.0.3.tar", last modified: Wed May 31 22:41:19 2023, max compression
```

## Comparing `dxtils-0.0.2.tar` & `dxtils-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 18:32:09.001939 dxtils-0.0.2/
--rw-rw-rw-   0        0        0      169 2023-05-31 18:32:08.994448 dxtils-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       23 2023-05-31 18:05:29.000000 dxtils-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 18:32:08.935978 dxtils-0.0.2/dxtils/
--rw-rw-rw-   0        0        0     1454 2023-05-31 18:30:30.000000 dxtils-0.0.2/dxtils/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-31 18:32:08.987936 dxtils-0.0.2/dxtils.egg-info/
--rw-rw-rw-   0        0        0      169 2023-05-31 18:32:07.000000 dxtils-0.0.2/dxtils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      160 2023-05-31 18:32:08.000000 dxtils-0.0.2/dxtils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 18:32:07.000000 dxtils-0.0.2/dxtils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-31 18:32:07.000000 dxtils-0.0.2/dxtils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      277 2023-05-31 18:30:36.000000 dxtils-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-31 18:32:09.002935 dxtils-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-31 22:41:19.870674 dxtils-0.0.3/
+-rw-rw-rw-   0        0        0      169 2023-05-31 22:41:19.864756 dxtils-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       23 2023-05-31 18:05:29.000000 dxtils-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 22:41:19.706336 dxtils-0.0.3/dxtils/
+-rw-rw-rw-   0        0        0     1892 2023-05-31 22:34:57.000000 dxtils-0.0.3/dxtils/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-31 22:41:19.860862 dxtils-0.0.3/dxtils.egg-info/
+-rw-rw-rw-   0        0        0      169 2023-05-31 22:41:17.000000 dxtils-0.0.3/dxtils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      160 2023-05-31 22:41:19.000000 dxtils-0.0.3/dxtils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 22:41:17.000000 dxtils-0.0.3/dxtils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-31 22:41:17.000000 dxtils-0.0.3/dxtils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      284 2023-05-31 22:39:46.000000 dxtils-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-31 22:41:19.871863 dxtils-0.0.3/setup.cfg
```

### Comparing `dxtils-0.0.2/dxtils/utils.py` & `dxtils-0.0.3/dxtils/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,38 @@
 import platform
 
+import requests as rq
 import undetected_chromedriver as uc
+from bs4 import BeautifulSoup
 from selenium.webdriver import Chrome, ChromeOptions
 from selenium.webdriver.chrome.service import Service
 from webdriver_manager.chrome import ChromeDriverManager
 from webdriver_manager.utils import read_version_from_cmd, PATTERN
 
 
 PLATFORM = platform.system()
 BRAVE_EXECUTABLE = "/Applications/Brave Browser.app/Contents/MacOS/Brave Browser"
+CHROMEDRIVERS_URL = "https://chromedriver.chromium.org/downloads"
+
+
+def get_sub_version(major_version: str) -> str:
+    soup = BeautifulSoup(rq.get(CHROMEDRIVERS_URL).text, "html.parser")
+    prefix = f"ChromeDriver {major_version}"
+    text = soup.find(text=lambda t: t and t.startswith(prefix))
+    return text.split()[1].strip()
 
 
 def set_up_driver(
     undetected: bool = False, kwargs_only: bool = False
 ) -> Chrome | uc.Chrome | dict:
     options = ChromeOptions()
     if PLATFORM != "Windows":
         version = read_version_from_cmd(
             f'"{BRAVE_EXECUTABLE}" --version', PATTERN["brave-browser"])
+        version = get_sub_version(version)
         driver_binary = ChromeDriverManager(version=version).install()
         options.binary_location = BRAVE_EXECUTABLE
         executable_path = BRAVE_EXECUTABLE
     else:
         driver_binary = ChromeDriverManager().install()
         executable_path = None        
     if not undetected:
```

