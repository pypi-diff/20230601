# Comparing `tmp/dhint-0.0.8.tar.gz` & `tmp/dhint-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dhint-0.0.8.tar", max compression
+gzip compressed data, was "dhint-0.0.9.tar", max compression
```

## Comparing `dhint-0.0.8.tar` & `dhint-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      256 2023-05-30 02:04:47.119981 dhint-0.0.8/dhint/__init__.py
--rw-r--r--   0        0        0      127 2023-05-29 21:25:54.398280 dhint-0.0.8/dhint/base/__init__.py
--rw-r--r--   0        0        0      311 2023-05-29 21:26:44.999717 dhint-0.0.8/dhint/base/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     9562 2023-05-30 03:21:12.102496 dhint-0.0.8/dhint/base/__pycache__/_meta.cpython-39.pyc
--rw-r--r--   0        0        0     2019 2023-05-29 20:55:46.212056 dhint-0.0.8/dhint/base/__pycache__/base_enum.cpython-39.pyc
--rw-r--r--   0        0        0     1620 2023-05-29 21:06:46.698181 dhint-0.0.8/dhint/base/__pycache__/collections.cpython-39.pyc
--rw-r--r--   0        0        0     1359 2023-05-30 03:23:36.868582 dhint-0.0.8/dhint/base/__pycache__/datamodel.cpython-39.pyc
--rw-r--r--   0        0        0    10159 2023-05-29 21:22:24.209570 dhint-0.0.8/dhint/base/__pycache__/descriptor.cpython-39.pyc
--rw-r--r--   0        0        0     1245 2023-05-30 03:24:01.964377 dhint-0.0.8/dhint/base/__pycache__/detamodel.cpython-39.pyc
--rw-r--r--   0        0        0     6465 2023-05-30 03:14:59.458340 dhint-0.0.8/dhint/base/_meta.py
--rw-r--r--   0        0        0     1125 2023-05-29 20:55:46.168796 dhint-0.0.8/dhint/base/base_enum.py
--rw-r--r--   0        0        0      837 2023-05-29 21:06:13.237219 dhint-0.0.8/dhint/base/collections.py
--rw-r--r--   0        0        0      620 2023-05-30 03:23:36.816298 dhint-0.0.8/dhint/base/datamodel.py
--rw-r--r--   0        0        0     8454 2023-05-29 21:22:24.128278 dhint-0.0.8/dhint/base/descriptor.py
--rw-r--r--   0        0        0      669 2023-05-30 03:24:01.912479 dhint-0.0.8/dhint/base/detamodel.py
--rw-r--r--   0        0        0     4068 2023-05-27 02:24:55.001024 dhint-0.0.8/dhint/collections.py
--rw-r--r--   0        0        0     5667 2023-05-29 00:53:58.892079 dhint-0.0.8/dhint/descriptors.py
--rw-r--r--   0        0        0     3171 2023-05-26 02:38:50.034497 dhint-0.0.8/dhint/function_types.py
--rw-r--r--   0        0        0     2504 2023-05-29 21:49:14.357625 dhint-0.0.8/dhint/functions.py
--rw-r--r--   0        0        0     1034 2023-05-30 02:16:18.133584 dhint-0.0.8/dhint/hints.py
--rw-r--r--   0        0        0     1467 2023-05-30 03:14:59.459815 dhint-0.0.8/dhint/json_encoder.py
--rw-r--r--   0        0        0      375 2023-05-24 11:39:53.142615 dhint-0.0.8/dhint/protocols.py
--rw-r--r--   0        0        0     1466 2023-05-26 12:08:08.808018 dhint-0.0.8/dhint/subdescriptor.py
--rw-r--r--   0        0        0     9889 2023-05-30 02:04:47.117134 dhint-0.0.8/dhint/type_hint.py
--rw-r--r--   0        0        0      330 2023-05-30 03:14:59.456137 dhint-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      630 2023-05-30 04:02:35.179364 dhint-0.0.8/setup.py
--rw-r--r--   0        0        0      382 2023-05-30 04:02:35.179774 dhint-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      256 2023-05-30 02:04:47.119981 dhint-0.0.9/dhint/__init__.py
+-rw-r--r--   0        0        0      127 2023-05-29 21:25:54.398280 dhint-0.0.9/dhint/base/__init__.py
+-rw-r--r--   0        0        0      311 2023-05-29 21:26:44.999717 dhint-0.0.9/dhint/base/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     9562 2023-05-30 03:21:12.102496 dhint-0.0.9/dhint/base/__pycache__/_meta.cpython-39.pyc
+-rw-r--r--   0        0        0     2019 2023-05-29 20:55:46.212056 dhint-0.0.9/dhint/base/__pycache__/base_enum.cpython-39.pyc
+-rw-r--r--   0        0        0     1620 2023-05-29 21:06:46.698181 dhint-0.0.9/dhint/base/__pycache__/collections.cpython-39.pyc
+-rw-r--r--   0        0        0     1359 2023-05-30 03:23:36.868582 dhint-0.0.9/dhint/base/__pycache__/datamodel.cpython-39.pyc
+-rw-r--r--   0        0        0    10159 2023-05-29 21:22:24.209570 dhint-0.0.9/dhint/base/__pycache__/descriptor.cpython-39.pyc
+-rw-r--r--   0        0        0     1245 2023-05-30 03:24:01.964377 dhint-0.0.9/dhint/base/__pycache__/detamodel.cpython-39.pyc
+-rw-r--r--   0        0        0     6465 2023-05-30 03:14:59.458340 dhint-0.0.9/dhint/base/_meta.py
+-rw-r--r--   0        0        0     1125 2023-05-29 20:55:46.168796 dhint-0.0.9/dhint/base/base_enum.py
+-rw-r--r--   0        0        0      837 2023-05-29 21:06:13.237219 dhint-0.0.9/dhint/base/collections.py
+-rw-r--r--   0        0        0      620 2023-05-30 03:23:36.816298 dhint-0.0.9/dhint/base/datamodel.py
+-rw-r--r--   0        0        0     8722 2023-06-01 17:07:27.299538 dhint-0.0.9/dhint/base/descriptor.py
+-rw-r--r--   0        0        0      669 2023-05-30 03:24:01.912479 dhint-0.0.9/dhint/base/detamodel.py
+-rw-r--r--   0        0        0     4067 2023-05-31 00:03:46.096954 dhint-0.0.9/dhint/collections.py
+-rw-r--r--   0        0        0     6510 2023-06-01 17:07:27.301834 dhint-0.0.9/dhint/descriptors.py
+-rw-r--r--   0        0        0     3171 2023-05-26 02:38:50.034497 dhint-0.0.9/dhint/function_types.py
+-rw-r--r--   0        0        0     2504 2023-05-29 21:49:14.357625 dhint-0.0.9/dhint/functions.py
+-rw-r--r--   0        0        0     1034 2023-05-30 02:16:18.133584 dhint-0.0.9/dhint/hints.py
+-rw-r--r--   0        0        0     1467 2023-05-30 03:14:59.459815 dhint-0.0.9/dhint/json_encoder.py
+-rw-r--r--   0        0        0      375 2023-05-24 11:39:53.142615 dhint-0.0.9/dhint/protocols.py
+-rw-r--r--   0        0        0     1466 2023-05-26 12:08:08.808018 dhint-0.0.9/dhint/subdescriptor.py
+-rw-r--r--   0        0        0     9889 2023-05-30 02:04:47.117134 dhint-0.0.9/dhint/type_hint.py
+-rw-r--r--   0        0        0      330 2023-06-01 17:07:27.295943 dhint-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      630 2023-06-01 17:07:36.411066 dhint-0.0.9/setup.py
+-rw-r--r--   0        0        0      382 2023-06-01 17:07:36.411291 dhint-0.0.9/PKG-INFO
```

### Comparing `dhint-0.0.8/dhint/base/__pycache__/_meta.cpython-39.pyc` & `dhint-0.0.9/dhint/base/__pycache__/_meta.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dhint-0.0.8/dhint/base/__pycache__/base_enum.cpython-39.pyc` & `dhint-0.0.9/dhint/base/__pycache__/base_enum.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dhint-0.0.8/dhint/base/__pycache__/collections.cpython-39.pyc` & `dhint-0.0.9/dhint/base/__pycache__/collections.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dhint-0.0.8/dhint/base/__pycache__/datamodel.cpython-39.pyc` & `dhint-0.0.9/dhint/base/__pycache__/datamodel.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dhint-0.0.8/dhint/base/__pycache__/descriptor.cpython-39.pyc` & `dhint-0.0.9/dhint/base/__pycache__/descriptor.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dhint-0.0.8/dhint/base/__pycache__/detamodel.cpython-39.pyc` & `dhint-0.0.9/dhint/base/__pycache__/detamodel.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dhint-0.0.8/dhint/base/_meta.py` & `dhint-0.0.9/dhint/base/_meta.py`

 * *Files identical despite different names*

### Comparing `dhint-0.0.8/dhint/base/base_enum.py` & `dhint-0.0.9/dhint/base/base_enum.py`

 * *Files identical despite different names*

### Comparing `dhint-0.0.8/dhint/base/collections.py` & `dhint-0.0.9/dhint/base/collections.py`

 * *Files identical despite different names*

### Comparing `dhint-0.0.8/dhint/base/datamodel.py` & `dhint-0.0.9/dhint/base/datamodel.py`

 * *Files identical despite different names*

### Comparing `dhint-0.0.8/dhint/base/descriptor.py` & `dhint-0.0.9/dhint/base/descriptor.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 __all__ = ['BaseDescriptor']
 
 from abc import ABC
 from typing import Callable, Optional, Any, ClassVar, Union
 from dataclasses import MISSING
 
 
-
 class BaseDescriptor(ABC):
     FIELD_TYPE: ClassVar[Optional[type]] = None
     HTML_TAG: ClassVar[Optional[str]] = None
     INPUT_TYPE: ClassVar[Optional[str]] = None
     FROZEN: ClassVar[Optional[bool]] = None
     DATALIST: ClassVar[Optional[bool]] = None
+    HTMX: ClassVar[Optional[bool]] = None
+
     
     def __init__(self, *args, **kwargs):
         self.args: tuple[str] = tuple([str(item) for item in args if all([isinstance(item, str), (item != '')])])
         self._label: Optional[str] = kwargs.pop('label', None)
         self._hash: Optional[bool] = kwargs.pop('hash', None)
         self._compare: bool = kwargs.pop('compare', True)
         self._private: bool = kwargs.pop('private', False)
@@ -120,20 +121,20 @@
         return self.__get__(instance)
     
     @property
     def metadata(self):
         return self._metadata
     
     @property
-    def htmlx(self):
-        return self._htmx
+    def htmx(self):
+        return True if any([self._htmx is True, self.HTMX is True]) else False
     
     @property
     def datalist(self):
-        return self.DATALIST or self._datalist
+        return True if any([self._datalist is True, self.DATALIST is True]) else False
     
     @property
     def datalist_id(self):
         return f'{self.public_name}-list'
     
     @property
     def field_bs_class(self):
@@ -166,25 +167,26 @@
     
     @property
     def label_element(self):
         if not self.no_form:
             if not self.is_hidden:
                 return '<label id="{}" for="{}">{}</label>'.format(
                         f'{self.public_name}__label',
-                        self.public_name,
+                        f'{self.public_name}__field',
                         self.label
                 )
+        return ''
     
     @property
     def html_tag(self) -> Optional[str]:
-        return self.HTML_TAG or self._html_tag
+        return self._html_tag or self.HTML_TAG
     
     @property
     def input_type(self) -> Optional[str]:
-        return self.INPUT_TYPE or self._input_type
+        return self._input_type or self.INPUT_TYPE
     
     @property
     def fullname(self) -> str:
         return f'{self.owner_name}.{self.public_name}'
     
     @property
     def hash(self) -> Optional[bool]:
@@ -192,15 +194,15 @@
     
     @property
     def compare(self) -> bool:
         return self._compare
     
     @property
     def frozen(self):
-        return self.FROZEN or self._frozen
+        return True if any([self._frozen is True, self.FROZEN is True]) else False
     
     @property
     def private(self) -> bool:
         return self._private
     
     @property
     def repr(self) -> bool:
@@ -208,27 +210,27 @@
     
     @property
     def db(self) -> bool:
         return self._db
     
     @property
     def no_form(self) -> bool:
-        return any([self._form is False, self.HTML_TAG is None])
+        return not self._form
     
     @property
     def is_input(self):
-        return all([not self.no_form, self.html_tag == 'input'])
+        return True if any([self._html_tag == 'input', self.HTML_TAG == 'input']) else False
     
     @property
     def is_select(self):
-        return all([not self.no_form, self.html_tag == 'select'])
+        return True if any([self._html_tag == 'select', self.HTML_TAG == 'select']) else False
     
     @property
     def is_textarea(self):
-        return all([not self.no_form, self.html_tag == 'textarea'])
+        return True if any([self._html_tag == 'textarea', self.HTML_TAG == 'textarea']) else False
     
     @property
     def is_hidden(self):
         return all([self.is_input is True, self.input_type == 'hidden'])
     
     @property
     def is_range(self):
@@ -249,19 +251,22 @@
     @property
     def search(self):
         return self._search
     
     def options(self, default=None):
         if hasattr(self.field_type, 'options'):
             return self.field_type.options(default)
-        return None
+        return ''
     
     def datalist_element(self):
         if self.datalist:
             return '<datalist id="{}">{}</datalist>'.format(
                     self.datalist_id,
                     self.options()
             )
-        return None
+        return ''
+    
+
+
```

### Comparing `dhint-0.0.8/dhint/base/detamodel.py` & `dhint-0.0.9/dhint/base/detamodel.py`

 * *Files identical despite different names*

### Comparing `dhint-0.0.8/dhint/collections.py` & `dhint-0.0.9/dhint/collections.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,8 +145,7 @@
     def export(self):
         return self.data
     
     def asjson(self):
         return self.export()
 
 
-
```

### Comparing `dhint-0.0.8/dhint/descriptors.py` & `dhint-0.0.9/dhint/descriptors.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 __all__ = ['Descriptor', 'Validator', 'NumberValidator', 'StringValidator', 'DateTimeValidator', 'DateValidator',
            'TextAreaValidator', 'IntValidator', 'FloatValidator', 'SelfKeyValidator', 'DecimalValidator',
-           'AutoValidator', 'PasswordValidator', 'BytesValidator', 'AutoUpdateValidator', 'SelectValidator']
+           'AutoValidator', 'PasswordValidator', 'BytesValidator', 'AutoUpdateValidator', 'SelectValidator',
+           'SearchValidator', 'BoolValidator', 'InitVarValidator', 'RegexValidator']
 
 import datetime
 from decimal import Decimal
 from typing import Optional, Callable
 from .base import *
 from .type_hint import *
 
@@ -80,14 +81,19 @@
 class NumberValidator(DateTimeValidator):
     FIELD_TYPE = None
     INPUT_TYPE = 'number'
     
     def __init__(self, *args, **kwargs):
         self._step: Optional[float, int] = kwargs.pop('step', None)
         super().__init__(*args, **kwargs)
+        
+        
+    @property
+    def step(self):
+        return self._step
     
 
 class IntValidator(NumberValidator):
     FIELD_TYPE = int
 
 
 class FloatValidator(NumberValidator):
@@ -184,15 +190,43 @@
     @property
     def repr(self) -> bool:
         return False
         
     @property
     def func(self):
         return self._func
-    
-    
+
+
 class AutoUpdateValidator(AutoValidator):
     
     def __set__(self, instance, value):
         setattr(instance, self.private_name, value)
         setattr(instance, self.private_name, self.func(instance))
+
+
+class SearchValidator(AutoUpdateValidator):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self._func: Callable = kwargs.pop('func', lambda self: self.search_getter)
+        self._required = False
+        self._form = False
+        self._repr = False
+
+
+class RegexValidator(Validator):
+    HTML_TAG = 'input'
+    INPUT_TYPE = 'text'
+
+
+class BoolValidator(Validator):
+    HTML_TAG = 'input'
+    INPUT_TYPE = 'checkbox'
+    FIELD_TYPE = bool
+
+
+class InitVarValidator(Validator):
     
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self._db = False
+        self._repr = False
+        self._required = False
```

### Comparing `dhint-0.0.8/dhint/function_types.py` & `dhint-0.0.9/dhint/function_types.py`

 * *Files identical despite different names*

### Comparing `dhint-0.0.8/dhint/functions.py` & `dhint-0.0.9/dhint/functions.py`

 * *Files identical despite different names*

### Comparing `dhint-0.0.8/dhint/hints.py` & `dhint-0.0.9/dhint/hints.py`

 * *Files identical despite different names*

### Comparing `dhint-0.0.8/dhint/json_encoder.py` & `dhint-0.0.9/dhint/json_encoder.py`

 * *Files identical despite different names*

### Comparing `dhint-0.0.8/dhint/subdescriptor.py` & `dhint-0.0.9/dhint/subdescriptor.py`

 * *Files identical despite different names*

### Comparing `dhint-0.0.8/dhint/type_hint.py` & `dhint-0.0.9/dhint/type_hint.py`

 * *Files identical despite different names*

### Comparing `dhint-0.0.8/setup.py` & `dhint-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['Unidecode>=1.3.6,<2.0.0', 'typing-extensions>=4.6.2,<5.0.0']
 
 setup_kwargs = {
     'name': 'dhint',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': '',
     'long_description': None,
     'author': 'Daniel Arantes',
     'author_email': 'arantesdv@me.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

