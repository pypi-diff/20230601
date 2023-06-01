# Comparing `tmp/python-automation-framework-0.0.9.tar.gz` & `tmp/python-automation-framework-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-automation-framework-0.0.9.tar", last modified: Tue May  9 19:32:49 2023, max compression
+gzip compressed data, was "python-automation-framework-0.1.0.tar", last modified: Thu Jun  1 15:09:08 2023, max compression
```

## Comparing `python-automation-framework-0.0.9.tar` & `python-automation-framework-0.1.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-05-09 19:32:49.795745 python-automation-framework-0.0.9/
--rw-r--r--   0 mikereiche   (502) staff       (20)     5387 2023-05-09 19:32:49.795584 python-automation-framework-0.0.9/PKG-INFO
--rw-r--r--   0 mikereiche   (502) staff       (20)     5137 2023-05-09 19:22:38.000000 python-automation-framework-0.0.9/README.md
-drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-05-09 19:32:49.793266 python-automation-framework-0.0.9/paf/
--rw-r--r--   0 mikereiche   (502) staff       (20)     7037 2023-05-09 19:19:06.000000 python-automation-framework-0.0.9/paf/assertion.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     3319 2023-05-09 19:04:45.000000 python-automation-framework-0.0.9/paf/common.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     2114 2023-05-09 11:20:20.000000 python-automation-framework-0.0.9/paf/component.py
--rw-r--r--   0 mikereiche   (502) staff       (20)      497 2023-05-09 08:02:43.000000 python-automation-framework-0.0.9/paf/config.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     2473 2023-05-05 10:53:33.000000 python-automation-framework-0.0.9/paf/control.py
--rw-r--r--   0 mikereiche   (502) staff       (20)      104 2023-04-14 17:12:01.000000 python-automation-framework-0.0.9/paf/dom.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     1913 2023-04-20 08:51:37.000000 python-automation-framework-0.0.9/paf/javascript.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     2257 2023-05-09 14:09:11.000000 python-automation-framework-0.0.9/paf/listener.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     2649 2023-05-04 17:04:40.000000 python-automation-framework-0.0.9/paf/locator.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     4345 2023-05-09 18:44:17.000000 python-automation-framework-0.0.9/paf/manager.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     3016 2023-05-09 19:21:48.000000 python-automation-framework-0.0.9/paf/page.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     2346 2023-05-04 20:56:52.000000 python-automation-framework-0.0.9/paf/request.py
--rw-r--r--   0 mikereiche   (502) staff       (20)      302 2023-05-09 18:25:16.000000 python-automation-framework-0.0.9/paf/types.py
--rw-r--r--   0 mikereiche   (502) staff       (20)    14434 2023-05-09 18:27:18.000000 python-automation-framework-0.0.9/paf/uielement.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     6689 2023-05-02 17:26:39.000000 python-automation-framework-0.0.9/paf/xpath.py
-drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-05-09 19:32:49.794025 python-automation-framework-0.0.9/python_automation_framework.egg-info/
--rw-r--r--   0 mikereiche   (502) staff       (20)     5387 2023-05-09 19:32:49.000000 python-automation-framework-0.0.9/python_automation_framework.egg-info/PKG-INFO
--rw-r--r--   0 mikereiche   (502) staff       (20)      668 2023-05-09 19:32:49.000000 python-automation-framework-0.0.9/python_automation_framework.egg-info/SOURCES.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)        1 2023-05-09 19:32:49.000000 python-automation-framework-0.0.9/python_automation_framework.egg-info/dependency_links.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)       46 2023-05-09 19:32:49.000000 python-automation-framework-0.0.9/python_automation_framework.egg-info/requires.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)        4 2023-05-09 19:32:49.000000 python-automation-framework-0.0.9/python_automation_framework.egg-info/top_level.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)       38 2023-05-09 19:32:49.795795 python-automation-framework-0.0.9/setup.cfg
--rw-r--r--   0 mikereiche   (502) staff       (20)      587 2023-05-09 19:31:57.000000 python-automation-framework-0.0.9/setup.py
-drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-05-09 19:32:49.795369 python-automation-framework-0.0.9/test/
--rw-r--r--   0 mikereiche   (502) staff       (20)     2021 2023-05-09 19:15:59.000000 python-automation-framework-0.0.9/test/test_component.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     1837 2023-05-09 19:20:32.000000 python-automation-framework-0.0.9/test/test_demo_mode.py
--rw-r--r--   0 mikereiche   (502) staff       (20)      524 2023-05-09 19:14:31.000000 python-automation-framework-0.0.9/test/test_javascript.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     3291 2023-05-09 11:19:43.000000 python-automation-framework-0.0.9/test/test_locator.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     3274 2023-05-09 19:15:53.000000 python-automation-framework-0.0.9/test/test_manager.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     1563 2023-05-09 19:22:08.000000 python-automation-framework-0.0.9/test/test_page.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     1124 2023-05-09 19:15:46.000000 python-automation-framework-0.0.9/test/test_request.py
--rw-r--r--   0 mikereiche   (502) staff       (20)     9699 2023-05-09 19:21:48.000000 python-automation-framework-0.0.9/test/test_uielement.py
+drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-06-01 15:09:08.655600 python-automation-framework-0.1.0/
+-rw-r--r--   0 mikereiche   (502) staff       (20)     5387 2023-06-01 15:09:08.655463 python-automation-framework-0.1.0/PKG-INFO
+-rw-r--r--   0 mikereiche   (502) staff       (20)     5137 2023-05-09 19:33:48.000000 python-automation-framework-0.1.0/README.md
+drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-06-01 15:09:08.652944 python-automation-framework-0.1.0/paf/
+-rw-r--r--   0 mikereiche   (502) staff       (20)     7037 2023-06-01 14:56:14.000000 python-automation-framework-0.1.0/paf/assertion.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     3319 2023-05-09 19:33:48.000000 python-automation-framework-0.1.0/paf/common.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2138 2023-06-01 15:07:19.000000 python-automation-framework-0.1.0/paf/component.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)      497 2023-05-09 19:33:48.000000 python-automation-framework-0.1.0/paf/config.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2473 2023-05-09 19:33:48.000000 python-automation-framework-0.1.0/paf/control.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)      104 2023-04-14 17:12:01.000000 python-automation-framework-0.1.0/paf/dom.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     1913 2023-04-20 08:51:37.000000 python-automation-framework-0.1.0/paf/javascript.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2502 2023-06-01 15:07:19.000000 python-automation-framework-0.1.0/paf/listener.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2649 2023-05-09 19:33:48.000000 python-automation-framework-0.1.0/paf/locator.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     4345 2023-05-09 19:33:48.000000 python-automation-framework-0.1.0/paf/manager.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     3131 2023-06-01 15:07:19.000000 python-automation-framework-0.1.0/paf/page.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2346 2023-05-09 19:33:48.000000 python-automation-framework-0.1.0/paf/request.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)      302 2023-05-09 19:33:48.000000 python-automation-framework-0.1.0/paf/types.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)    14599 2023-06-01 15:07:19.000000 python-automation-framework-0.1.0/paf/uielement.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     6689 2023-05-02 17:26:39.000000 python-automation-framework-0.1.0/paf/xpath.py
+drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-06-01 15:09:08.653998 python-automation-framework-0.1.0/python_automation_framework.egg-info/
+-rw-r--r--   0 mikereiche   (502) staff       (20)     5387 2023-06-01 15:09:08.000000 python-automation-framework-0.1.0/python_automation_framework.egg-info/PKG-INFO
+-rw-r--r--   0 mikereiche   (502) staff       (20)      668 2023-06-01 15:09:08.000000 python-automation-framework-0.1.0/python_automation_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)        1 2023-06-01 15:09:08.000000 python-automation-framework-0.1.0/python_automation_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)       46 2023-06-01 15:09:08.000000 python-automation-framework-0.1.0/python_automation_framework.egg-info/requires.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)        4 2023-06-01 15:09:08.000000 python-automation-framework-0.1.0/python_automation_framework.egg-info/top_level.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)       38 2023-06-01 15:09:08.655645 python-automation-framework-0.1.0/setup.cfg
+-rw-r--r--   0 mikereiche   (502) staff       (20)      587 2023-06-01 15:08:41.000000 python-automation-framework-0.1.0/setup.py
+drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-06-01 15:09:08.655263 python-automation-framework-0.1.0/test/
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2021 2023-05-09 19:15:59.000000 python-automation-framework-0.1.0/test/test_component.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     2049 2023-06-01 15:07:19.000000 python-automation-framework-0.1.0/test/test_demo_mode.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)      524 2023-05-09 19:33:48.000000 python-automation-framework-0.1.0/test/test_javascript.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     3291 2023-05-09 19:33:48.000000 python-automation-framework-0.1.0/test/test_locator.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     3274 2023-05-09 19:33:48.000000 python-automation-framework-0.1.0/test/test_manager.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     1563 2023-05-09 19:33:48.000000 python-automation-framework-0.1.0/test/test_page.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     1124 2023-05-09 19:33:48.000000 python-automation-framework-0.1.0/test/test_request.py
+-rw-r--r--   0 mikereiche   (502) staff       (20)     9791 2023-06-01 15:07:19.000000 python-automation-framework-0.1.0/test/test_uielement.py
```

### Comparing `python-automation-framework-0.0.9/PKG-INFO` & `python-automation-framework-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-automation-framework
-Version: 0.0.9
+Version: 0.1.0
 Summary: Automation framework for the WebDriver API
 Home-page: https://github.com/mreiche/python-automation-framework
 Author: Mike Reiche
 Description-Content-Type: text/markdown
 
 ![Tests Status](https://github.com/mreiche/python-automation-framework/actions/workflows/tests.yml/badge.svg)
 [![Code Coverage Status](https://codecov.io/github/mreiche/python-automation-framework/branch/main/graph/badge.svg)](https://app.codecov.io/github/mreiche/python-automation-framework)
```

### Comparing `python-automation-framework-0.0.9/README.md` & `python-automation-framework-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.9/paf/assertion.py` & `python-automation-framework-0.1.0/paf/assertion.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.9/paf/common.py` & `python-automation-framework-0.1.0/paf/common.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.9/paf/component.py` & `python-automation-framework-0.1.0/paf/component.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 from paf.common import HasParent, Locator
 from paf.types import COMPONENT, PAGE
 from paf.uielement import UiElement, PageObject, PageObjectList, UiElementTests
 
 
 class Component(PageObject[COMPONENT], PageObjectList[COMPONENT], HasParent, UiElementTests):
 
-    def highlight(self, color: Color = Color.from_string("#0f0"), seconds: float = 2):
-        self._ui_element.highlight(color, seconds)
-        return self
-
     def __init__(self, ui_element: UiElement):
         self._ui_element = ui_element
         ui_element._parent = self
 
-    def _find(self, by: Locator):
-        ui_element = self._ui_element.find(by)
+    def highlight(self, color: Color = Color.from_string("#0f0"), seconds: float = 2):
+        self._ui_element.highlight(color, seconds)
+        return self
+
+    def _find(self, by: Locator, name: str = None):
+        ui_element = self._ui_element.find(by, name)
         return ui_element
 
     @property
     def name(self):
         return f"{self.__class__.__name__}"
 
     @property
```

### Comparing `python-automation-framework-0.0.9/paf/control.py` & `python-automation-framework-0.1.0/paf/control.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.9/paf/javascript.py` & `python-automation-framework-0.1.0/paf/javascript.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.9/paf/listener.py` & `python-automation-framework-0.1.0/paf/listener.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,15 +75,23 @@
         action_name: str,
         ui_element: "UiElement",
         exception: Exception
     ):
         if not isinstance(exception, NotFoundException):
             self._highlight_with_color(ui_element, "#f00")
 
+    def assertion_passed(
+        self,
+        assertion: AbstractAssertion,
+        ui_element: "UiElement"
+    ):
+        if assertion.raise_exception:
+            self._highlight_with_color(ui_element, "#0f0")
+
     def assertion_failed_finally(
         self,
         assertion: AbstractAssertion,
         ui_element: "UiElement",
         exception: Exception
     ):
-        if not isinstance(exception, NotFoundException):
+        if not isinstance(exception, NotFoundException) and assertion.raise_exception:
             self._highlight_with_color(ui_element, "#f00")
```

### Comparing `python-automation-framework-0.0.9/paf/locator.py` & `python-automation-framework-0.1.0/paf/locator.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.9/paf/manager.py` & `python-automation-framework-0.1.0/paf/manager.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.9/paf/page.py` & `python-automation-framework-0.1.0/paf/page.py`

 * *Files 17% similar despite different names*

```diff
@@ -26,17 +26,22 @@
     def open(self, url: str):
         self._webdriver.get(url)
         return self
 
     def __str__(self):
         return self.name
 
-    def _find(self, by: Locator):
+    def _find(self, by: Locator, name: str = None):
         from paf.uielement import UiElement
-        return UiElement(by, webdriver=self._webdriver, parent=self)
+        return UiElement(
+            by=by,
+            webdriver=self._webdriver,
+            parent=self,
+            name=name,
+        )
 
     @property
     def name(self):
         return self.__class__.__name__
 
     @property
     def webdriver(self):
@@ -52,16 +57,16 @@
 
     def scroll_by(self, x: int = 0, y: int = 0):
         actions = ActionChains(self._webdriver)
         actions.scroll_by_amount(x, y).perform()
 
 
 class FinderPage(BasePage):
-    def find(self, by: Locator):
-        ui_element = self._find(by)
+    def find(self, by: Locator, name: str = None):
+        ui_element = self._find(by, name)
         ui_element._parent = None
         return ui_element
 
 
 class Page(BasePage):
     def __init__(self, webdriver: WebDriver):
         super().__init__(webdriver)
```

### Comparing `python-automation-framework-0.0.9/paf/request.py` & `python-automation-framework-0.1.0/paf/request.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.9/paf/uielement.py` & `python-automation-framework-0.1.0/paf/uielement.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,37 +126,40 @@
     def __init__(
         self,
         by: Locator,
         ui_element: "UiElement" = None,
         webdriver: WebDriver = None,
         parent: object = None,
         index: int = 0,
+        name: str = None,
     ):
 
         if isinstance(by, XPath):
             by = By.xpath(str(by))
         elif isinstance(by, str):
             by = By.css_selector(by)
 
         self._webdriver = webdriver
         self._ui_element = ui_element
         self._by = by
         self._index = index
         self._parent = parent
+        self._name = name
 
     @property
     def webdriver(self):
         return self._webdriver
 
-    def find(self, by: Locator):
+    def find(self, by: Locator, name: str = None):
         return UiElement(
             by=by,
             ui_element=self,
             webdriver=self._webdriver,
-            parent=self
+            parent=self,
+            name=name,
         )
 
     def __relative_selector(self, by: By):
         if by.by == SeleniumBy.XPATH and by.value.startswith("/"):
             return f".{by.value}"
         else:
             return by.value
@@ -300,15 +303,18 @@
         return self
 
     def __str__(self):
         return self.name
 
     @property
     def name(self):
-        return f"UiElement({self._by.__str__()})[{self._index}]"
+        if self._name:
+            return self._name
+        else:
+            return f"UiElement({self._by.__str__()})[{self._index}]"
 
     def scroll_into_view(self, x: int = 0, y: int = 0):
         self._action_sequence(lambda web_element: script.scroll_to_center(self._webdriver, web_element, Point(x, y)), __name__)
 
     def scroll_to_top(self, x: int = 0, y: int = 0):
         self._action_sequence(lambda web_element: script.scroll_to_top(self._webdriver, web_element, Point(x, y)), __name__)
```

### Comparing `python-automation-framework-0.0.9/paf/xpath.py` & `python-automation-framework-0.1.0/paf/xpath.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.9/python_automation_framework.egg-info/PKG-INFO` & `python-automation-framework-0.1.0/python_automation_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-automation-framework
-Version: 0.0.9
+Version: 0.1.0
 Summary: Automation framework for the WebDriver API
 Home-page: https://github.com/mreiche/python-automation-framework
 Author: Mike Reiche
 Description-Content-Type: text/markdown
 
 ![Tests Status](https://github.com/mreiche/python-automation-framework/actions/workflows/tests.yml/badge.svg)
 [![Code Coverage Status](https://codecov.io/github/mreiche/python-automation-framework/branch/main/graph/badge.svg)](https://app.codecov.io/github/mreiche/python-automation-framework)
```

### Comparing `python-automation-framework-0.0.9/python_automation_framework.egg-info/SOURCES.txt` & `python-automation-framework-0.1.0/python_automation_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.9/setup.py` & `python-automation-framework-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,13 +6,13 @@
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="python-automation-framework",
     description="Automation framework for the WebDriver API",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="0.0.9",
+    version="0.1.0",
     url="https://github.com/mreiche/python-automation-framework",
     author="Mike Reiche",
     packages=["paf"],
     install_requires=["inject>=4.3.1", "selenium>=4.8.3", "is-empty>=1.0.1"],
 )
```

### Comparing `python-automation-framework-0.0.9/test/test_component.py` & `python-automation-framework-0.1.0/test/test_component.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.9/test/test_demo_mode.py` & `python-automation-framework-0.1.0/test/test_demo_mode.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,26 +34,34 @@
     btn = finder.find("#button")
     btn.click()
     btn.expect.css("outline").be("rgb(255, 255, 0) solid 5px")
 
 
 def test_highlight_failed_assertion(finder: FinderPage, listener: Listener):
     btn = finder.find("#button")
-    btn.wait_for.text.be("Katze")
+
+    with pytest.raises(Exception):
+        btn.expect.text.be("Katze")
+
     btn.expect.css("outline").be("rgb(255, 0, 0) solid 5px")
     assert not btn.wait_for.text.raise_exception
 
 
+def test_highlight_passed_assertion(finder: FinderPage, listener: Listener):
+    btn = finder.find("#button")
+    btn.expect.value.be("click me")
+    btn.expect.css("outline").be("rgb(0, 255, 0) solid 5px")
+
+
 def test_highlight_not_found_log(finder: FinderPage, listener: Listener, caplog):
     inexistent = finder.find("#inexistent")
-    inexistent.wait_for.count.be(1)
 
     with pytest.raises(Exception):
         inexistent.click()
 
-    assert len(caplog.records) == 2
+    assert len(caplog.records) == 1
     for record in caplog.records:
         assert "Cannot highlight UiElement(By.css selector(#inexistent))[0]: Not found" in record.message
 
 
 def teardown_module():
     inject.instance(WebDriverManager).shutdown_all()
```

### Comparing `python-automation-framework-0.0.9/test/test_javascript.py` & `python-automation-framework-0.1.0/test/test_javascript.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.9/test/test_locator.py` & `python-automation-framework-0.1.0/test/test_locator.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.9/test/test_manager.py` & `python-automation-framework-0.1.0/test/test_manager.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.9/test/test_page.py` & `python-automation-framework-0.1.0/test/test_page.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.9/test/test_request.py` & `python-automation-framework-0.1.0/test/test_request.py`

 * *Files identical despite different names*

### Comparing `python-automation-framework-0.0.9/test/test_uielement.py` & `python-automation-framework-0.1.0/test/test_uielement.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,17 +25,19 @@
     assert p.name_path == 'UiElement(By.id(para1))[0]'
     assert p.name == p.name_path
     assert str(p) == p.name
     assert finder.webdriver == p.webdriver
 
     centered = finder.find(".centered")
     p2 = centered.find("#para2")
+    p_name = finder.find(By.id("para1"), "paragraph")
 
     assert p2.name == "UiElement(By.css selector(#para2))[0]"
     assert p2.name_path == "UiElement(By.css selector(.centered))[0] > " + p2.name
+    assert p_name.name == "paragraph"
 
 
 # def test_rect():
 #     finder = page_factory.create_page(FinderPage, create_webdriver())
 #     finder.open("https://testpages.herokuapp.com/styled/basic-web-page-test.html")
 #
 #     p = finder.find(By.id("para1"))
```

