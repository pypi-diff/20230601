# Comparing `tmp/pywebgo-0.0.5.tar.gz` & `tmp/pywebgo-0.0.6.tar.gz`

## Comparing `pywebgo-0.0.5.tar` & `pywebgo-0.0.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pywebgo-0.0.5/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pywebgo-0.0.5/src/pywebgo/__init__.py
--rw-r--r--   0        0        0    14906 2020-02-02 00:00:00.000000 pywebgo-0.0.5/src/pywebgo/controller.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 pywebgo-0.0.5/src/pywebgo/data.py
--rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 pywebgo-0.0.5/src/pywebgo/elements.py
--rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 pywebgo-0.0.5/src/pywebgo/utils.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 pywebgo-0.0.5/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 pywebgo-0.0.5/LICENSE
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pywebgo-0.0.5/README.md
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 pywebgo-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 pywebgo-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pywebgo-0.0.6/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pywebgo-0.0.6/src/pywebgo/__init__.py
+-rw-r--r--   0        0        0    14954 2020-02-02 00:00:00.000000 pywebgo-0.0.6/src/pywebgo/controller.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 pywebgo-0.0.6/src/pywebgo/data.py
+-rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 pywebgo-0.0.6/src/pywebgo/elements.py
+-rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 pywebgo-0.0.6/src/pywebgo/utils.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 pywebgo-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 pywebgo-0.0.6/LICENSE
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pywebgo-0.0.6/README.md
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 pywebgo-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 pywebgo-0.0.6/PKG-INFO
```

### Comparing `pywebgo-0.0.5/.github/workflows/python-publish.yml` & `pywebgo-0.0.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pywebgo-0.0.5/src/pywebgo/controller.py` & `pywebgo-0.0.6/src/pywebgo/controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from .elements import ElementsHandler
 from selenium import webdriver
 from selenium.common import NoSuchElementException
 from selenium.webdriver.support.select import Select
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions
 from selenium.webdriver.remote.webelement import WebElement
-from selenium.common.exceptions import NoAlertPresentException
 from selenium.webdriver.common.action_chains import ActionChains
+from selenium.common.exceptions import NoAlertPresentException, NoSuchWindowException
 
 
 class WebController(webdriver.Chrome):
     """
     Implements search, action execution and data retrieval successively for given element dictionaries.
 
     Inherits from *selenium.webdriver.Chrome*
@@ -197,15 +197,15 @@
         Handle any alert that may be present on the page.
         """
         try:
             alert = self.switch_to.alert
             alert.accept()
             # Retry the last operation
             self.execute_actions(web_element, element)
-        except NoAlertPresentException:
+        except (NoAlertPresentException, NoSuchWindowException):
             pass
 
     def load_page(self, url: str) -> None:
         """
         Load the web page from the given URL.
 
         :param url: URL of the web page to be loaded
```

### Comparing `pywebgo-0.0.5/src/pywebgo/data.py` & `pywebgo-0.0.6/src/pywebgo/data.py`

 * *Files identical despite different names*

### Comparing `pywebgo-0.0.5/src/pywebgo/elements.py` & `pywebgo-0.0.6/src/pywebgo/elements.py`

 * *Files identical despite different names*

### Comparing `pywebgo-0.0.5/src/pywebgo/utils.py` & `pywebgo-0.0.6/src/pywebgo/utils.py`

 * *Files identical despite different names*

### Comparing `pywebgo-0.0.5/.gitignore` & `pywebgo-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pywebgo-0.0.5/LICENSE` & `pywebgo-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pywebgo-0.0.5/pyproject.toml` & `pywebgo-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pywebgo"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Adil Zafar Khan", email="adilzafar66@gmail.com" },
 ]
 description = "A selenium client that automates web surfing with simple commands."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pywebgo-0.0.5/PKG-INFO` & `pywebgo-0.0.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywebgo
-Version: 0.0.5
+Version: 0.0.6
 Summary: A selenium client that automates web surfing with simple commands.
 Project-URL: Homepage, https://github.com/adilzafar66/pywebgo
 Project-URL: Bug Tracker, https://github.com/adilzafar66/pywebgo/issues
 Author-email: Adil Zafar Khan <adilzafar66@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

