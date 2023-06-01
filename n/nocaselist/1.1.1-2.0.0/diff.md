# Comparing `tmp/nocaselist-1.1.1.tar.gz` & `tmp/nocaselist-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nocaselist-1.1.1.tar", last modified: Sun Feb 26 15:26:26 2023, max compression
+gzip compressed data, was "nocaselist-2.0.0.tar", last modified: Thu Jun  1 14:28:09 2023, max compression
```

## Comparing `nocaselist-1.1.1.tar` & `nocaselist-2.0.0.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2023-02-26 15:26:26.701341 nocaselist-1.1.1/
--rw-r--r--   0 maiera     (501) staff       (20)      424 2022-08-04 11:04:17.000000 nocaselist-1.1.1/INSTALL.md
--rw-r--r--   0 maiera     (501) staff       (20)    11357 2022-08-04 11:04:17.000000 nocaselist-1.1.1/LICENSE
--rw-r--r--   0 maiera     (501) staff       (20)      263 2023-02-26 15:26:26.000000 nocaselist-1.1.1/MANIFEST.in
--rw-r--r--   0 maiera     (501) staff       (20)     4581 2023-02-26 15:26:26.700626 nocaselist-1.1.1/PKG-INFO
--rw-r--r--   0 maiera     (501) staff       (20)     3081 2023-02-26 14:40:27.000000 nocaselist-1.1.1/README.rst
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2023-02-26 15:26:26.690294 nocaselist-1.1.1/nocaselist/
--rw-r--r--   0 maiera     (501) staff       (20)      191 2022-08-04 11:04:17.000000 nocaselist-1.1.1/nocaselist/__init__.py
--rw-r--r--   0 maiera     (501) staff       (20)    20968 2023-02-26 15:26:11.000000 nocaselist-1.1.1/nocaselist/_nocaselist.py
--rw-r--r--   0 maiera     (501) staff       (20)      321 2023-02-26 15:26:13.000000 nocaselist-1.1.1/nocaselist/_version.py
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2023-02-26 15:26:26.693856 nocaselist-1.1.1/nocaselist.egg-info/
--rw-r--r--   0 maiera     (501) staff       (20)     4581 2023-02-26 15:26:26.000000 nocaselist-1.1.1/nocaselist.egg-info/PKG-INFO
--rw-r--r--   0 maiera     (501) staff       (20)      599 2023-02-26 15:26:26.000000 nocaselist-1.1.1/nocaselist.egg-info/SOURCES.txt
--rw-r--r--   0 maiera     (501) staff       (20)        1 2023-02-26 15:26:26.000000 nocaselist-1.1.1/nocaselist.egg-info/dependency_links.txt
--rw-r--r--   0 maiera     (501) staff       (20)      510 2023-02-26 15:26:26.000000 nocaselist-1.1.1/nocaselist.egg-info/requires.txt
--rw-r--r--   0 maiera     (501) staff       (20)       11 2023-02-26 15:26:26.000000 nocaselist-1.1.1/nocaselist.egg-info/top_level.txt
--rw-r--r--   0 maiera     (501) staff       (20)        1 2023-02-26 15:26:26.000000 nocaselist-1.1.1/nocaselist.egg-info/zip-safe
--rw-r--r--   0 maiera     (501) staff       (20)      655 2023-02-26 15:26:11.000000 nocaselist-1.1.1/requirements.txt
--rw-r--r--   0 maiera     (501) staff       (20)       38 2023-02-26 15:26:26.701478 nocaselist-1.1.1/setup.cfg
--rwxr-xr-x   0 maiera     (501) staff       (20)     6742 2023-02-26 15:26:11.000000 nocaselist-1.1.1/setup.py
--rw-r--r--   0 maiera     (501) staff       (20)     1744 2023-02-26 15:26:11.000000 nocaselist-1.1.1/test-requirements.txt
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2023-02-26 15:26:26.694652 nocaselist-1.1.1/tests/
--rw-r--r--   0 maiera     (501) staff       (20)        0 2020-07-19 13:03:24.000000 nocaselist-1.1.1/tests/__init__.py
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2023-02-26 15:26:26.695101 nocaselist-1.1.1/tests/installtest/
--rwxr-xr-x   0 maiera     (501) staff       (20)    12821 2022-08-04 11:04:17.000000 nocaselist-1.1.1/tests/installtest/test_install.sh
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2023-02-26 15:26:26.697208 nocaselist-1.1.1/tests/unittest/
--rw-r--r--   0 maiera     (501) staff       (20)        0 2020-07-19 13:03:24.000000 nocaselist-1.1.1/tests/unittest/__init__.py
--rw-r--r--   0 maiera     (501) staff       (20)    82895 2023-02-26 15:26:11.000000 nocaselist-1.1.1/tests/unittest/test_nocaselist.py
--rw-r--r--   0 maiera     (501) staff       (20)      401 2020-07-19 13:03:24.000000 nocaselist-1.1.1/tests/unittest/test_package.py
-drwxr-xr-x   0 maiera     (501) staff       (20)        0 2023-02-26 15:26:26.699562 nocaselist-1.1.1/tests/utils/
--rw-r--r--   0 maiera     (501) staff       (20)        0 2020-07-21 04:12:03.000000 nocaselist-1.1.1/tests/utils/__init__.py
--rw-r--r--   0 maiera     (501) staff       (20)     3444 2022-08-04 11:04:17.000000 nocaselist-1.1.1/tests/utils/import_installed.py
--rw-r--r--   0 maiera     (501) staff       (20)     7204 2023-02-26 14:41:25.000000 nocaselist-1.1.1/tests/utils/simplified_test_function.py
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2023-06-01 14:28:09.024378 nocaselist-2.0.0/
+-rw-r--r--   0 maiera     (501) staff       (20)      424 2022-08-04 11:04:17.000000 nocaselist-2.0.0/INSTALL.md
+-rw-r--r--   0 maiera     (501) staff       (20)    11357 2022-08-04 11:04:17.000000 nocaselist-2.0.0/LICENSE
+-rw-r--r--   0 maiera     (501) staff       (20)      263 2023-06-01 14:28:08.000000 nocaselist-2.0.0/MANIFEST.in
+-rw-r--r--   0 maiera     (501) staff       (20)     4242 2023-06-01 14:28:09.023658 nocaselist-2.0.0/PKG-INFO
+-rw-r--r--   0 maiera     (501) staff       (20)     2976 2023-05-01 07:33:49.000000 nocaselist-2.0.0/README.rst
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2023-06-01 14:28:09.012162 nocaselist-2.0.0/nocaselist/
+-rw-r--r--   0 maiera     (501) staff       (20)      191 2022-08-04 11:04:17.000000 nocaselist-2.0.0/nocaselist/__init__.py
+-rw-r--r--   0 maiera     (501) staff       (20)    21704 2023-06-01 05:24:41.000000 nocaselist-2.0.0/nocaselist/_nocaselist.py
+-rw-r--r--   0 maiera     (501) staff       (20)      326 2023-06-01 14:25:52.000000 nocaselist-2.0.0/nocaselist/_version.py
+-rw-r--r--   0 maiera     (501) staff       (20)        0 2023-06-01 05:24:41.000000 nocaselist-2.0.0/nocaselist/py.typed
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2023-06-01 14:28:09.015369 nocaselist-2.0.0/nocaselist.egg-info/
+-rw-r--r--   0 maiera     (501) staff       (20)     4242 2023-06-01 14:28:08.000000 nocaselist-2.0.0/nocaselist.egg-info/PKG-INFO
+-rw-r--r--   0 maiera     (501) staff       (20)      619 2023-06-01 14:28:08.000000 nocaselist-2.0.0/nocaselist.egg-info/SOURCES.txt
+-rw-r--r--   0 maiera     (501) staff       (20)        1 2023-06-01 14:28:08.000000 nocaselist-2.0.0/nocaselist.egg-info/dependency_links.txt
+-rw-r--r--   0 maiera     (501) staff       (20)      195 2023-06-01 14:28:08.000000 nocaselist-2.0.0/nocaselist.egg-info/requires.txt
+-rw-r--r--   0 maiera     (501) staff       (20)       11 2023-06-01 14:28:08.000000 nocaselist-2.0.0/nocaselist.egg-info/top_level.txt
+-rw-r--r--   0 maiera     (501) staff       (20)        1 2023-06-01 14:28:08.000000 nocaselist-2.0.0/nocaselist.egg-info/zip-safe
+-rw-r--r--   0 maiera     (501) staff       (20)      750 2023-06-01 05:24:41.000000 nocaselist-2.0.0/requirements.txt
+-rw-r--r--   0 maiera     (501) staff       (20)       38 2023-06-01 14:28:09.024546 nocaselist-2.0.0/setup.cfg
+-rwxr-xr-x   0 maiera     (501) staff       (20)     6647 2023-06-01 05:24:41.000000 nocaselist-2.0.0/setup.py
+-rw-r--r--   0 maiera     (501) staff       (20)     1155 2023-06-01 05:24:41.000000 nocaselist-2.0.0/test-requirements.txt
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2023-06-01 14:28:09.015811 nocaselist-2.0.0/tests/
+-rw-r--r--   0 maiera     (501) staff       (20)        0 2020-07-19 13:03:24.000000 nocaselist-2.0.0/tests/__init__.py
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2023-06-01 14:28:09.016300 nocaselist-2.0.0/tests/installtest/
+-rwxr-xr-x   0 maiera     (501) staff       (20)    12821 2022-08-04 11:04:17.000000 nocaselist-2.0.0/tests/installtest/test_install.sh
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2023-06-01 14:28:09.020290 nocaselist-2.0.0/tests/unittest/
+-rw-r--r--   0 maiera     (501) staff       (20)        0 2020-07-19 13:03:24.000000 nocaselist-2.0.0/tests/unittest/__init__.py
+-rw-r--r--   0 maiera     (501) staff       (20)    85041 2023-06-01 05:24:41.000000 nocaselist-2.0.0/tests/unittest/test_nocaselist.py
+-rw-r--r--   0 maiera     (501) staff       (20)      401 2020-07-19 13:03:24.000000 nocaselist-2.0.0/tests/unittest/test_package.py
+drwxr-xr-x   0 maiera     (501) staff       (20)        0 2023-06-01 14:28:09.022591 nocaselist-2.0.0/tests/utils/
+-rw-r--r--   0 maiera     (501) staff       (20)        0 2020-07-21 04:12:03.000000 nocaselist-2.0.0/tests/utils/__init__.py
+-rw-r--r--   0 maiera     (501) staff       (20)     3444 2022-08-04 11:04:17.000000 nocaselist-2.0.0/tests/utils/import_installed.py
+-rw-r--r--   0 maiera     (501) staff       (20)     7138 2023-06-01 05:24:41.000000 nocaselist-2.0.0/tests/utils/simplified_test_function.py
```

### Comparing `nocaselist-1.1.1/LICENSE` & `nocaselist-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nocaselist-1.1.1/PKG-INFO` & `nocaselist-2.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nocaselist
-Version: 1.1.1
+Version: 2.0.0
 Summary: A case-insensitive list for Python
 Home-page: https://github.com/pywbem/nocaselist
 Author: Andreas Maier
 Author-email: andreas.r.maier@gmx.de
 Maintainer: Andreas Maier
 Maintainer-email: andreas.r.maier@gmx.de
 License: Apache Software License 2.0
@@ -12,27 +12,23 @@
 Project-URL: Documentation, https://nocaselist.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/pywbem/nocaselist
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
+Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 License-File: LICENSE
 
 nocaselist - A case-insensitive list for Python
 ===============================================
 
@@ -72,16 +68,15 @@
     ['Alpha', 'Beta']
 
     >>> 'ALPHA' in list1  # Any lookup or comparison is case-insensitive
     True
 
 The `NocaseList`_ class supports the functionality of the built-in
 `list class of Python 3.8`_ on all Python versions it supports (except for being
-case-insensitive, of course). This includes the ``clear()`` and ``copy()``
-methods added in Python 3.3 to the built-in ``list`` class.
+case-insensitive, of course).
 
 .. _list class of Python 3.8: https://docs.python.org/3.8/library/stdtypes.html#list
 .. _NocaseList: https://nocaselist.readthedocs.io/en/stable/reference.html#nocaselist.NocaseList
 
 The case-insensitivity is achieved by matching any key values as their
 casefolded values. By default, the casefolding is performed with
 `str.casefold()`_ for unicode string keys and with `bytes.lower()`_ for byte
```

### Comparing `nocaselist-1.1.1/README.rst` & `nocaselist-2.0.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -37,16 +37,15 @@
     ['Alpha', 'Beta']
 
     >>> 'ALPHA' in list1  # Any lookup or comparison is case-insensitive
     True
 
 The `NocaseList`_ class supports the functionality of the built-in
 `list class of Python 3.8`_ on all Python versions it supports (except for being
-case-insensitive, of course). This includes the ``clear()`` and ``copy()``
-methods added in Python 3.3 to the built-in ``list`` class.
+case-insensitive, of course).
 
 .. _list class of Python 3.8: https://docs.python.org/3.8/library/stdtypes.html#list
 .. _NocaseList: https://nocaselist.readthedocs.io/en/stable/reference.html#nocaselist.NocaseList
 
 The case-insensitivity is achieved by matching any key values as their
 casefolded values. By default, the casefolding is performed with
 `str.casefold()`_ for unicode string keys and with `bytes.lower()`_ for byte
```

### Comparing `nocaselist-1.1.1/nocaselist/_nocaselist.py` & `nocaselist-2.0.0/nocaselist/_nocaselist.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,49 @@
 """
 This module provides class NocaseList.
 """
 
-from __future__ import print_function, absolute_import
-
 import sys
 import os
+from typing import Callable, AnyStr, Optional, Union
+try:
+    from typing import SupportsIndex  # type: ignore
+except ImportError:
+    from typing_extensions import SupportsIndex  # Python <=3.7
+try:
+    from typing import TypeAlias  # type: ignore
+except ImportError:
+    from typing_extensions import TypeAlias  # Python <=3.9
+if sys.version_info[0:2] >= (3, 9):
+    from collections.abc import Iterable  # type: ignore
+else:
+    # Before py39, collections.abc.Iterable did not support generic type
+    from typing import Iterable
 
 __all__ = ['NocaseList']
 
-if sys.version_info[0] == 2:
-    # pylint: disable=undefined-variable
-    _INTEGER_TYPES = (long, int)  # noqa: F821
-else:
-    _INTEGER_TYPES = (int,)
-
 # This env var is set when building the docs. It causes the methods
 # that are supposed to exist only in a particular Python version, not to be
 # removed, so they appear in the docs.
 BUILDING_DOCS = os.environ.get('BUILDING_DOCS', False)
 
+# Type for values in NocaseList
+Value: TypeAlias = Optional[AnyStr]
+
+# Type for returning single values or slices
+ValueOrNocaseList: TypeAlias = Union[Value, 'NocaseList']
+
+# Type for other argument in rich comparison methods
+OtherList: TypeAlias = Iterable[Value]  # pylint: disable=unsubscriptable-object
+
+# Type for index argument that can also specify a slice
+IndexOrSlice: TypeAlias = Union[SupportsIndex, slice]
+
 
 class NocaseList(list):
-    # pylint: disable=line-too-long
     """
     A case-insensitive and case-preserving list.
 
     The list is case-insensitive: Whenever items of the list are looked up by
     value or item values are compared, that is done case-insensitively. The
     case-insensitivity is defined by performing the lookup or comparison on the
     result of the :meth:`__casefold__` method on the on list items.
@@ -41,166 +58,162 @@
     facilitate type checks.
 
     The implementation maintains a second list with the casefolded items of
     the inherited list, and ensures that both lists are in sync.
 
     The list supports serialization via the Python :mod:`py:pickle` module.
     To save space and time, only the originally cased list is serialized.
-    """  # noqa E401
-    # pylint: enable=line-too-long
+    """
 
     # Methods not implemented:
     #
     # * __getattribute__(self, name): The method inherited from object is used;
     #   no reason to have a different implementation.
     #
     # * __sizeof__(self): The method inherited from list is used; no reason
     #   to have a different implementation.
     #
+    # * __len__(self): The method inherited from list is used; no reason
+    #   to have a different implementation.
+    #
     # __repr__(): The method inherited from list is used; no reason
     #   to have a different implementation.
     #
     # __getitem__(): The method inherited from list is used; no reason
     #   to have a different implementation.
     #
     # __iter__(): The method inherited from list is used; no reason
     #   to have a different implementation.
 
-    def __init__(self, iterable=()):
+    def __init__(self, iterable=()) -> None:
         """
         Initialize the list with the items in the specified iterable.
         """
         super(NocaseList, self).__init__(iterable)
 
         # The _casefolded_list attribute is a list with the same items as the
         # original (inherited) list, except they are casefolded using the
         # __casefold__() method.
 
         # The following is an optimization based on the assumption that in
         # many cases, casefolding the input list is more expensive than
         # copying it (plus the overhead to check that).
         if isinstance(iterable, NocaseList):
-            try:
-                # pylint: disable=protected-access
-                self._casefolded_list = iterable._casefolded_list.copy()
-            except AttributeError:  # No copy() on Python 2
-                self._casefolded_list = self._new_casefolded_list(self)
+            # pylint: disable=protected-access
+            casefolded_list = iterable._casefolded_list.copy()
         else:
-            self._casefolded_list = self._new_casefolded_list(self)
+            casefolded_list = self._new_casefolded_list(self)
+        self._casefolded_list: list = casefolded_list
 
-    def _new_casefolded_list(self, lst):
+    def _new_casefolded_list(self, lst: OtherList) -> list:
         """
         Return a casefolded list from the input list.
         """
         result = []
         for value in lst:
             result.append(self._casefolded_value(value))
         return result
 
-    def _casefolded_value(self, value):
+    def _casefolded_value(self, value: Value) -> Value:
         """
         This method returns the casefolded value and handles the case of value
-        being `None`.
+        being `None`. The value may be a string or an list/tuple of strings.
         """
         if value is None:
             return None
+        if isinstance(value, (list, tuple)):
+            return [self._casefolded_value(v) for v in value]
         return self.__casefold__(value)
 
     @staticmethod
-    def __casefold__(value):
+    def __casefold__(value: AnyStr) -> AnyStr:
         """
         This method implements the case-insensitive behavior of the class.
 
         It returns a case-insensitive form of the input value by calling a
         "casefold method" on the value. The input value will not be `None`.
 
-        The casefold method called by this method is :meth:`py2:str.lower` on
-        Python 2, and on Python 3 it is :meth:`py:str.casefold`, falling back
-        to :meth:`py:bytes.lower` if it does not exist.
+        The casefold method called by this method is :meth:`py:str.casefold`.
+        If that method does not exist on the key value (e.g. because it is a
+        byte string), :meth:`py:bytes.lower` is called, for compatibility with
+        earlier versions of the package.
 
         This method can be overridden by users in order to change the
         case-insensitive behavior of the class.
         See :ref:`Overriding the default casefold method` for details.
 
         Parameters:
-          value (str or unicode or bytes): Input value. Will not be `None`.
+          value (str or bytes): Input value. Will not be `None`.
 
         Returns:
-          str or unicode or bytes: Case-insensitive form of the input value.
+          str or bytes: Case-insensitive form of the input value.
 
         Raises:
           AttributeError: The value does not have the casefold method.
         """
         try:
-            return value.casefold()
+            return value.casefold()  # type: ignore
         except AttributeError:
-            # Either Python 2, or Python 3 and a byte string key
             return value.lower()
 
     def __getstate__(self):
         """
         Called when pickling the object, see :meth:`py:object.__getstate__`.
 
         In order to save space and time, only the list with the originally
         cased items is saved, but not the second list with the casefolded
         items.
-
-        On Python 2, the 'pickle' module does not call :meth:`__setstate__`,
-        so this optimzation has only be implemented for Python 3.
         """
         # This copies the state of the inherited list even though it is
         # not visible in self.__dict__.
         state = self.__dict__.copy()
         del state['_casefolded_list']
         return state
 
     def __setstate__(self, state):
         """
         Called when unpickling the object, see :meth:`py:object.__setstate__`.
-
-        On Python 2, the 'pickle' module does not call this method, so this
-        optimzation has only be implemented for Python 3.
         """
         self.__dict__.update(state)
         self._casefolded_list = self._new_casefolded_list(self)
 
-    def __setitem__(self, index, value):
+    def __setitem__(self, index: IndexOrSlice, value: Value) -> None:
         """
-        Update the value of the item at an existing index in the list.
+        Update the value of the item at an existing index or slice in the list.
 
         Invoked using ``ncl[index] = value``.
 
         Raises:
           AttributeError: The value does not have the casefold method.
         """
-        super(NocaseList, self).__setitem__(index, value)
-        self._casefolded_list[index] = self._casefolded_value(value)
+        super(NocaseList, self).__setitem__(index, value)  # type: ignore
+        self._casefolded_list[index] = self._casefolded_value(value)  # type: ignore # noqa: E501 pylint: disable=line-too-long
 
-    def __delitem__(self, index):
+    def __delitem__(self, index: IndexOrSlice) -> None:
         """
-        Delete an item at an existing index from the list.
+        Delete an item at an existing index or slice from the list.
 
         Invoked using ``del ncl[index]``.
         """
         super(NocaseList, self).__delitem__(index)
         del self._casefolded_list[index]
 
-    def __contains__(self, value):
+    def __contains__(self, value: Value) -> bool:
         """
         Return a boolean indicating whether the list contains at least one
         item with the value, by looking it up case-insensitively.
 
         Invoked using ``value in ncl``.
 
         Raises:
           AttributeError: The value does not have the casefold method.
         """
         return self._casefolded_value(value) in self._casefolded_list
 
-    def __add__(self, other):
+    def __add__(self, other: OtherList) -> 'NocaseList':
         """
         Return a new :class:`NocaseList` object that contains the items from
         the left hand operand (``self``) and the items from the right hand
         operand (``other``).
 
         The right hand operand (``other``) must be an instance of
         :class:`py:list` (including :class:`NocaseList`) or :class:`py:tuple`.
@@ -215,15 +228,15 @@
             raise TypeError(
                 "Can only concatenate list or tuple (not {t}) to NocaseList".
                 format(t=type(other)))
         lst = self.copy()
         lst.extend(other)
         return lst
 
-    def __iadd__(self, other):
+    def __iadd__(self, other: OtherList) -> 'NocaseList':
         """
         Extend the left hand operand (``self``) by the items from the right
         hand operand (``other``).
 
         The ``other`` parameter must be an iterable but is otherwise not
         restricted in type. Thus, if it is a string, the characters of the
         string are added as distinct items to the list.
@@ -231,241 +244,242 @@
         Invoked using ``ncl += other``.
         """
         # Note: It is unusual that the method has to return self, but it was
         # verified that this is necessary.
         self.extend(other)
         return self
 
-    def __mul__(self, number):
+    def __mul__(self, number: int) -> 'NocaseList':  # type: ignore
         """
         Return a new :class:`NocaseList` object that contains the items from
         the left hand operand (``self``) as many times as specified by the right
         hand operand (``number``).
 
         A number <= 0 causes the returned list to be empty.
 
         The left hand operand (``self``) is not changed.
 
         Invoked using ``ncl * number``.
         """
-        if not isinstance(number, _INTEGER_TYPES):
+        # Despite using type hints, passing a non-int object does not raise
+        # any exception, so we still need to check the type:
+        if not isinstance(number, int):
             raise TypeError(
                 "Cannot multiply NocaseList by non-integer of type {t}".
                 format(t=type(number)))
         lst = NocaseList()
         for _ in range(0, number):
             lst.extend(self)
         return lst
 
-    def __rmul__(self, number):
+    def __rmul__(self, number: int) -> 'NocaseList':  # type: ignore
         """
         Return a new :class:`NocaseList` object that contains the items from
         the right hand operand (``self``) as many times as specified by the left
         hand operand (``number``).
 
         A number <= 0 causes the returned list to be empty.
 
         The right hand operand (``self``) is not changed.
 
         Invoked using ``number * ncl``.
         """
         lst = self * number  # Delegates to __mul__()
         return lst
 
-    def __imul__(self, number):
+    def __imul__(self, number: int) -> 'NocaseList':  # type: ignore
         """
         Change the left hand operand (``self``) so that it contains the items
         from the original left hand operand (``self``) as many times as
         specified by the right hand operand (``number``).
 
         A number <= 0 will empty the left hand operand.
 
         Invoked using ``ncl *= number``.
         """
-        # Note: It is unusual that the method has to return self, but it was
-        # verified that this is necessary.
-        if not isinstance(number, _INTEGER_TYPES):
+        # Despite using type hints, passing a non-int object does not raise
+        # any exception, so we still need to check the type:
+        if not isinstance(number, int):
             raise TypeError(
                 "Cannot multiply NocaseList by non-integer of type {t}".
                 format(t=type(number)))
         if number <= 0:
             del self[:]
             del self._casefolded_list[:]
         else:
             self_items = list(self)
             for _ in range(0, number - 1):
                 self.extend(self_items)
+        # Note: It is unusual that the method has to return self, but it was
+        # verified that this is necessary.
         return self
 
-    def __reversed__(self):
+    def __reversed__(self) -> 'NocaseList':  # type: ignore
         """
         Return a shallow copy of the list that has its items reversed in order.
 
         Invoked using ``reversed(ncl)``.
         """
         lst = self.copy()
         lst.reverse()
         return lst
 
-    def __eq__(self, other):
+    def __eq__(self, other: object) -> bool:
         """
         Return a boolean indicating whether the list and the other list are
         equal, by comparing corresponding list items case-insensitively.
 
         The other list may be a :class:`NocaseList` object or any other
         iterable. In all cases, the comparison takes place case-insensitively.
 
         Invoked using e.g. ``ncl == other``.
 
         Raises:
           AttributeError: A value in the other list does not have the casefold
             method.
         """
         if isinstance(other, NocaseList):
-            other = other._casefolded_list  # pylint: disable=protected-access
-        else:
-            other = self._new_casefolded_list(other)
-        return self._casefolded_list == other
+            # pylint: disable=protected-access
+            return self._casefolded_list == other._casefolded_list
+
+        if isinstance(other, Iterable):
+            return self._casefolded_list == self._new_casefolded_list(other)
+
+        return NotImplemented
 
-    def __ne__(self, other):
+    def __ne__(self, other: object) -> bool:
         """
         Return a boolean indicating whether the list and the other list are
         not equal, by comparing corresponding list items case-insensitively.
 
         The other list may be a :class:`NocaseList` object or any other
         iterable. In all cases, the comparison takes place case-insensitively.
 
         Invoked using e.g. ``ncl != other``.
 
         Raises:
           AttributeError: A value in the other list does not have the casefold
             method.
         """
-        if isinstance(other, NocaseList):
-            other = other._casefolded_list  # pylint: disable=protected-access
-        else:
-            other = self._new_casefolded_list(other)
-        return self._casefolded_list != other
+        eq = self.__eq__(other)
+        if eq is NotImplemented:
+            return NotImplemented
+        return not eq
 
-    def __gt__(self, other):
+    def __gt__(self, other: object) -> bool:
         """
         Return a boolean indicating whether the list is greater than the other
         list, by comparing corresponding list items case-insensitively.
 
         The other list may be a :class:`NocaseList` object or any other
         iterable. In all cases, the comparison takes place case-insensitively.
 
         Invoked using e.g. ``ncl > other``.
 
         Raises:
           AttributeError: A value in the other list does not have the casefold
             method.
         """
         if isinstance(other, NocaseList):
-            other = other._casefolded_list  # pylint: disable=protected-access
-        else:
-            other = self._new_casefolded_list(other)
-        return self._casefolded_list > other
+            # pylint: disable=protected-access
+            return self._casefolded_list > other._casefolded_list
+
+        if isinstance(other, Iterable):
+            return self._casefolded_list > self._new_casefolded_list(other)
+
+        return NotImplemented
 
-    def __lt__(self, other):
+    def __lt__(self, other: object) -> bool:
         """
         Return a boolean indicating whether the list is less than the other
         list, by comparing corresponding list items case-insensitively.
 
         The other list may be a :class:`NocaseList` object or any other
         iterable. In all cases, the comparison takes place case-insensitively.
 
         Invoked using e.g. ``ncl < other``.
 
         Raises:
           AttributeError: A value in the other list does not have the casefold
             method.
         """
         if isinstance(other, NocaseList):
-            other = other._casefolded_list  # pylint: disable=protected-access
-        else:
-            other = self._new_casefolded_list(other)
-        return self._casefolded_list < other
+            # pylint: disable=protected-access
+            return self._casefolded_list < other._casefolded_list
+
+        if isinstance(other, Iterable):
+            return self._casefolded_list < self._new_casefolded_list(other)
+
+        return NotImplemented
 
-    def __ge__(self, other):
+    def __ge__(self, other: object) -> bool:
         """
         Return a boolean indicating whether the list is greater than or
         equal to the other list, by comparing corresponding list items
         case-insensitively.
 
         The other list may be a :class:`NocaseList` object or any other
         iterable. In all cases, the comparison takes place case-insensitively.
 
         Invoked using e.g. ``ncl >= other``.
 
         Raises:
           AttributeError: A value in the other list does not have the casefold
             method.
         """
-        if isinstance(other, NocaseList):
-            other = other._casefolded_list  # pylint: disable=protected-access
-        else:
-            other = self._new_casefolded_list(other)
-        return self._casefolded_list >= other
+        lt = self.__lt__(other)
+        if lt is NotImplemented:
+            return NotImplemented
+        return not lt
 
-    def __le__(self, other):
+    def __le__(self, other: object) -> bool:
         """
         Return a boolean indicating whether the list is less than or
         equal to the other list, by comparing corresponding list items
         case-insensitively.
 
         The other list may be a :class:`NocaseList` object or any other
         iterable. In all cases, the comparison takes place case-insensitively.
 
         Invoked using e.g. ``ncl <= other``.
 
         Raises:
           AttributeError: A value in the other list does not have the casefold
             method.
         """
-        if isinstance(other, NocaseList):
-            other = other._casefolded_list  # pylint: disable=protected-access
-        else:
-            other = self._new_casefolded_list(other)
-        return self._casefolded_list <= other
+        gt = self.__gt__(other)
+        if gt is NotImplemented:
+            return NotImplemented
+        return not gt
 
-    def count(self, value):
+    def count(self, value: Value) -> int:
         """
         Return the number of times the specified value occurs in the list,
         comparing the value and the list items case-insensitively.
 
         Raises:
           AttributeError: The value does not have the casefold method.
         """
         return self._casefolded_list.count(self._casefolded_value(value))
 
-    def copy(self):
+    def copy(self) -> 'NocaseList':
         """
         Return a shallow copy of the list.
-
-        Note: This method is supported on Python 2 and Python 3, even though
-        the built-in list class only supports it on Python 3.
         """
         return NocaseList(self)
 
-    def clear(self):
+    def clear(self) -> None:
         """
         Remove all items from the list (and return None).
-
-        Note: This method is supported on Python 2 and Python 3, even though
-        the built-in list class only supports it on Python 3.
         """
-        try:
-            super(NocaseList, self).clear()
-            self._casefolded_list.clear()
-        except AttributeError:
-            del self[:]
-            del self._casefolded_list[:]
+        super(NocaseList, self).clear()
+        self._casefolded_list.clear()
 
-    def index(self, value, start=0, stop=9223372036854775807):
+    def index(self, value: Value, start: SupportsIndex = 0,
+              stop: SupportsIndex = 9223372036854775807) -> int:
         """
         Return the index of the first item that is equal to the specified
         value, comparing the value and the list items case-insensitively.
 
         The search is limited to the index range defined by the specified
         ``start`` and ``stop`` parameters, whereby ``stop`` is the index
         of the first item after the search range.
@@ -473,83 +487,84 @@
         Raises:
           AttributeError: The value does not have the casefold method.
           ValueError: No such item is found.
         """
         return self._casefolded_list.index(
             self._casefolded_value(value), start, stop)
 
-    def append(self, value):
+    def append(self, value: Value) -> None:
         """
         Append the specified value as a new item to the end of the list
         (and return None).
 
         Raises:
           AttributeError: The value does not have the casefold method.
         """
         super(NocaseList, self).append(value)
         self._casefolded_list.append(self._casefolded_value(value))
 
-    def extend(self, iterable):
+    def extend(self, values: Iterable) -> None:
         """
         Extend the list by the items in the specified iterable
         (and return None).
 
         Raises:
           AttributeError: A value in the iterable does not have the casefold
             method.
         """
-        super(NocaseList, self).extend(iterable)
+        super(NocaseList, self).extend(values)
         # The following is a circumvention for a behavior of the 'pickle' module
         # that during unpickling may call this method on an object that has
         # been created with __new__() without calling __init__().
         try:
-            for value in iterable:
+            for value in values:
                 self._casefolded_list.append(self._casefolded_value(value))
         except AttributeError:
             self._casefolded_list = self._new_casefolded_list(self)
 
-    def insert(self, index, value):
+    def insert(self, index: SupportsIndex, value: Value) -> None:
         """
         Insert a new item with specified value before the item at the specified
         index (and return None).
 
         Raises:
           AttributeError: The value does not have the casefold method.
         """
         super(NocaseList, self).insert(index, value)
         self._casefolded_list.insert(index, self._casefolded_value(value))
 
-    def pop(self, index=-1):
+    def pop(self, index: SupportsIndex = -1) -> Value:
         """
         Return the value of the item at the specified index and also remove it
         from the list.
         """
         self._casefolded_list.pop(index)
         return super(NocaseList, self).pop(index)
 
-    def remove(self, value):
+    def remove(self, value: Value) -> None:
         """
         Remove the first item from the list whose value is equal to the
         specified value (and return None), comparing the value and the list
         items case-insensitively.
 
         Raises:
           AttributeError: The value does not have the casefold method.
         """
         self._casefolded_list.remove(self._casefolded_value(value))
         super(NocaseList, self).remove(value)
 
-    def reverse(self):
+    def reverse(self) -> None:
         """
         Reverse the items in the list in place (and return None).
         """
         super(NocaseList, self).reverse()
         self._casefolded_list = self._new_casefolded_list(self)
 
-    def sort(self, key=None, reverse=False):
+    def sort(self, *, key: Optional[Callable] = None,
+             reverse: bool = False) -> None:
         """
         Sort the items in the list in place (and return None).
 
         The sort is stable, in that the order of two (case-insensitively) equal
         elements is maintained.
 
         By default, the list is sorted in ascending order of its casefolded
@@ -567,15 +582,7 @@
             # adding them to the list.
             if key:
                 return key(self._casefolded_value(value))
             return self._casefolded_value(value)
 
         super(NocaseList, self).sort(key=casefolded_key, reverse=reverse)
         self._casefolded_list = self._new_casefolded_list(self)
-
-
-# Remove methods that should only be present in a particular Python version.
-# If the documentation is being built, the methods are not removed in order to
-# show them in the documentation.
-if sys.version_info[0] == 2 and not BUILDING_DOCS:
-    del NocaseList.__setstate__
-    del NocaseList.__getstate__
```

### Comparing `nocaselist-1.1.1/nocaselist.egg-info/PKG-INFO` & `nocaselist-2.0.0/nocaselist.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nocaselist
-Version: 1.1.1
+Version: 2.0.0
 Summary: A case-insensitive list for Python
 Home-page: https://github.com/pywbem/nocaselist
 Author: Andreas Maier
 Author-email: andreas.r.maier@gmx.de
 Maintainer: Andreas Maier
 Maintainer-email: andreas.r.maier@gmx.de
 License: Apache Software License 2.0
@@ -12,27 +12,23 @@
 Project-URL: Documentation, https://nocaselist.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/pywbem/nocaselist
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
+Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 License-File: LICENSE
 
 nocaselist - A case-insensitive list for Python
 ===============================================
 
@@ -72,16 +68,15 @@
     ['Alpha', 'Beta']
 
     >>> 'ALPHA' in list1  # Any lookup or comparison is case-insensitive
     True
 
 The `NocaseList`_ class supports the functionality of the built-in
 `list class of Python 3.8`_ on all Python versions it supports (except for being
-case-insensitive, of course). This includes the ``clear()`` and ``copy()``
-methods added in Python 3.3 to the built-in ``list`` class.
+case-insensitive, of course).
 
 .. _list class of Python 3.8: https://docs.python.org/3.8/library/stdtypes.html#list
 .. _NocaseList: https://nocaselist.readthedocs.io/en/stable/reference.html#nocaselist.NocaseList
 
 The case-insensitivity is achieved by matching any key values as their
 casefolded values. By default, the casefolding is performed with
 `str.casefold()`_ for unicode string keys and with `bytes.lower()`_ for byte
```

### Comparing `nocaselist-1.1.1/setup.py` & `nocaselist-2.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 Python setup script for the nocaselist project.
 """
 
 import sys
 import os
 import io
 import re
-import setuptools
+from typing import Optional
+
+import setuptools  # type: ignore
 
 
 def get_version(version_file):
     """
     Execute the specified version file and return the value of the __version__
     global variable that is set in the version file.
 
@@ -57,16 +59,16 @@
     using pytest.
 
     Note on the class name: Because distutils.dist._show_help() shows the class
     name for the setup.py command name instead of invoking get_command_name(),
     the classes that get registered as commands must have the command name.
     """
 
-    description = None  # Set by subclass
-    my_test_dirs = None  # Set by subclass
+    description: Optional[str] = None  # Set by subclass
+    my_test_dirs: Optional[list] = None  # Set by subclass
 
     user_options = [
         (
             'pytest-options=',  # '=' indicates it requires an argument
             None,  # no short option
             "additional options for pytest, as one argument"
         ),
@@ -138,24 +140,27 @@
 dependency_links = [req for req in requirements
                     if req and re.match(r'[^:]+://', req)]
 test_requirements = get_requirements('test-requirements.txt')
 
 package_version = get_version(os.path.join('nocaselist', '_version.py'))
 
 # Docs on setup():
-# * https://docs.python.org/2.7/distutils/apiref.html?
+# * https://docs.python.org/3/distutils/apiref.html?
 #   highlight=setup#distutils.core.setup
 # * https://setuptools.readthedocs.io/en/latest/setuptools.html#
 #   new-and-changed-setup-keywords
 setuptools.setup(
     name='nocaselist',
     version=package_version,
     packages=[
         'nocaselist',
     ],
+    package_data={
+        'nocaselist': ['py.typed']
+    },
     include_package_data=True,  # Includes MANIFEST.in files into sdist (only)
     scripts=[
         # add any scripts
     ],
     install_requires=install_requires,
     dependency_links=dependency_links,
     extras_require={
@@ -180,25 +185,21 @@
     },
 
     options={'bdist_wheel': {'universal': True}},
     zip_safe=True,  # This package can safely be installed from a zip file
     platforms='any',
 
     # Keep these Python versions in sync with nocaselist/__init__.py
-    python_requires='>=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*',
+    python_requires='>=3.6',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Topic :: Software Development :: Libraries :: Python Modules',
```

### Comparing `nocaselist-1.1.1/test-requirements.txt` & `nocaselist-2.0.0/test-requirements.txt`

 * *Files 27% similar despite different names*

```diff
@@ -6,47 +6,41 @@
 # Make sure that the minimum versions required in this file are consistent with
 # the minimum versions specified in minimum-constraints.txt.
 
 
 # Unit test direct dependencies (e.g. imports into testcases):
 
 # pytest
-# pytest 5.0.0 has removed support for Python < 3.5
-# pytest 4.3.1 solves an issue on Python 3 with minimum package levels
-# pytest 6.0.0 causes pylint to report "not-callable" issues
-pytest>=4.3.1,<5.0.0; python_version < '3.5'
-pytest>=4.3.1,!=6.0; python_version >= '3.5' and python_version <= '3.6'
-pytest>=4.4.0,!=6.0; python_version >= '3.7' and python_version <= '3.9'
-pytest>=6.2.5; python_version >= '3.10'
+# pytest 7.0.0 started using type hints
+pytest>=7.0.0
 
 
 # Install test direct dependencies:
 
 # virtualenv
-# Virtualenv 20.0.19 has an issue where it does not install pip on Python 3.4.
-# Virtualenv 20.0.32 has an issue where it raises AttributeError on Python 3.4.
 # tox 3.21.0 requires virtualenv!=20.0.[0-7],>=16.0.0 and requires py>=3.5
-virtualenv>=16.1.0,!=20.0.19,!=20.0.32; python_version <= '3.4'
-virtualenv>=20.1.0; python_version >= '3.5'
+virtualenv>=20.1.0
+
+# six (also used by virtualenv, tox, probably others)
+# virtualenv 20.0 requires six>=1.12.0 on py>=3.8
+# tox 3.17 requires six>=1.14.0
+six>=1.14.0
 
 
 # Indirect dependencies with special constraints:
 
 # packaging (used by pytest)
 packaging>=17.0
 
 # pluggy (used by pytest, tox)
 # Pluggy 0.12.0 has a bug causing pytest plugins to fail loading on py38
 # pytest 4.3.1 depends on pluggy>=0.7
 # tox 3.21.0 depends on pluggy>=0.12.0
 pluggy>=0.13.1
 
-# pathlib2 (used by virtualenv on py<3.4 on non-Windows)
-pathlib2<3,>=2.3.3; python_version < '3.4' and sys_platform != 'win32'
-
 
 # Additional indirect dependencies are not specified in this file:
 
 # appdirs
 # attrs
 # distlib
 # filelock
```

### Comparing `nocaselist-1.1.1/tests/installtest/test_install.sh` & `nocaselist-2.0.0/tests/installtest/test_install.sh`

 * *Files identical despite different names*

### Comparing `nocaselist-1.1.1/tests/unittest/test_nocaselist.py` & `nocaselist-2.0.0/tests/unittest/test_nocaselist.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from __future__ import absolute_import
 
 import sys
 import os
 import re
 import unicodedata
 import pickle
-import six
 import pytest
+import six  # type: ignore
 
 from ..utils.simplified_test_function import simplified_test_function
 
 # pylint: disable=wrong-import-position, wrong-import-order, invalid-name
 from ..utils.import_installed import import_installed
 nocaselist = import_installed('nocaselist')
 from nocaselist import NocaseList as _NocaseList  # noqa: E402
@@ -24,20 +24,14 @@
 
 # Controls whether the tests are run against a standard dict instead.
 TEST_AGAINST_LIST = bool(os.getenv('TEST_AGAINST_LIST'))
 
 if TEST_AGAINST_LIST:
     print("\nInfo: test_nocaselist.py tests run against standard list")
 
-# Indicates that the list to be tested has a copy() method
-LIST_HAS_COPY = not TEST_AGAINST_LIST or sys.version_info[0] == 3
-
-# Indicates that the list to be tested has a clear() method
-LIST_HAS_CLEAR = not TEST_AGAINST_LIST or sys.version_info[0] == 3
-
 # The list class being tested
 # pylint: disable=invalid-name
 NocaseList = list if TEST_AGAINST_LIST else _NocaseList
 
 # Flag indicating that standard dict is guaranteed to preserve order
 DICT_PRESERVES_ORDER = sys.version_info[0:2] >= (3, 7)
 
@@ -148,37 +142,37 @@
         None, None, True
     ),
 
     # Non-empty NocaseList
     (
         "List from list as positional arg",
         dict(
-            init_args=([u'Dog', b'Cat'],),
+            init_args=(['Dog', b'Cat'],),
             init_kwargs={},
-            exp_list=[u'Dog', b'Cat'],
+            exp_list=['Dog', b'Cat'],
             verify_order=True,
         ),
         None, None, True
     ),
     (
         "List from tuple as positional arg",
         dict(
-            init_args=((u'Dog', b'Cat'),),
+            init_args=(('Dog', b'Cat'),),
             init_kwargs={},
-            exp_list=[u'Dog', b'Cat'],
+            exp_list=['Dog', b'Cat'],
             verify_order=True,
         ),
         None, None, True
     ),
     (
         "List from dict as positional arg (uses only the keys)",
         dict(
-            init_args=({u'Dog': 'Kitten', b'Cat': 'Budgie'},),
+            init_args=({'Dog': 'Kitten', b'Cat': 'Budgie'},),
             init_kwargs={},
-            exp_list=[u'Dog', b'Cat'],
+            exp_list=['Dog', b'Cat'],
             verify_order=DICT_PRESERVES_ORDER,
         ),
         None, None, True
     ),
     (
         "List from string as positional arg (string chars become list items)",
         dict(
@@ -336,15 +330,15 @@
         ),
         TypeError, None, True
     ),
     (
         "Empty list, with unicode string as index (invalid type)",
         dict(
             nclist=NocaseList(),
-            index=u'',
+            index='',
             exp_value=None,
         ),
         TypeError, None, True
     ),
     (
         "Empty list, with byte string as index (invalid type)",
         dict(
@@ -364,60 +358,60 @@
         IndexError, None, True
     ),
 
     # Non-empty NocaseList
     (
         "List with two items, with None as index (invalid type)",
         dict(
-            nclist=NocaseList([u'Dog', b'Cat']),
+            nclist=NocaseList(['Dog', b'Cat']),
             index=None,
             exp_value=None,
         ),
         TypeError, None, True
     ),
     (
         "List with two items, with string as index (invalid type)",
         dict(
-            nclist=NocaseList([u'Dog', b'Cat']),
-            index=u'',
+            nclist=NocaseList(['Dog', b'Cat']),
+            index='',
             exp_value=None,
         ),
         TypeError, None, True
     ),
     (
         "List with two items, with non-existing index 2 (out of range)",
         dict(
-            nclist=NocaseList([u'Dog', b'Cat']),
+            nclist=NocaseList(['Dog', b'Cat']),
             index=2,
             exp_value=None,
         ),
         IndexError, None, True
     ),
     (
         "List with two items, with index 0",
         dict(
-            nclist=NocaseList([u'Dog', b'Cat']),
+            nclist=NocaseList(['Dog', b'Cat']),
             index=0,
             exp_value='Dog',
         ),
         None, None, True
     ),
     (
         "List with two items, with index 1",
         dict(
-            nclist=NocaseList([u'Dog', b'Cat']),
+            nclist=NocaseList(['Dog', b'Cat']),
             index=1,
             exp_value=b'Cat',
         ),
         None, None, True
     ),
     (
         "List with two items, with index -1",
         dict(
-            nclist=NocaseList([u'Dog', b'Cat']),
+            nclist=NocaseList(['Dog', b'Cat']),
             index=-1,
             exp_value=b'Cat',
         ),
         None, None, True
     ),
 ]
 
@@ -467,15 +461,15 @@
         ),
         TypeError, None, True
     ),
     (
         "Empty list, with unicode string as index (invalid type)",
         dict(
             nclist=NocaseList(),
-            index=u'',
+            index='',
             value=None,
             exp_nclist=None,
         ),
         TypeError, None, True
     ),
     (
         "Empty list, with byte string as index (invalid type)",
@@ -498,61 +492,81 @@
         IndexError, None, True
     ),
 
     # Non-empty NocaseList
     (
         "List with two items, with None as index (invalid type)",
         dict(
-            nclist=NocaseList([u'Dog', b'Cat']),
+            nclist=NocaseList(['Dog', b'Cat']),
             index=None,
-            value=u'Kitten',
+            value='Kitten',
             exp_nclist=None,
         ),
         TypeError, None, True
     ),
     (
         "List with two items, setting unicode string at index 0",
         dict(
-            nclist=NocaseList([u'Dog', u'Cat']),
+            nclist=NocaseList(['Dog', 'Cat']),
             index=0,
-            value=u'Newbie',
-            exp_nclist=NocaseList([u'Newbie', u'Cat']),
+            value='Newbie',
+            exp_nclist=NocaseList(['Newbie', 'Cat']),
         ),
         None, None, True
     ),
     (
         "List with two items, setting byte string at index 1",
         dict(
-            nclist=NocaseList([u'Dog', u'Cat']),
+            nclist=NocaseList(['Dog', 'Cat']),
             index=1,
             value=b'Newbie',
-            exp_nclist=NocaseList([u'Dog', b'Newbie']),
+            exp_nclist=NocaseList(['Dog', b'Newbie']),
         ),
         None, None, True
     ),
     (
         "List with two items, setting string at index -1",
         dict(
-            nclist=NocaseList([u'Dog', u'Cat']),
+            nclist=NocaseList(['Dog', 'Cat']),
             index=-1,
-            value=u'Newbie',
-            exp_nclist=NocaseList([u'Dog', u'Newbie']),
+            value='Newbie',
+            exp_nclist=NocaseList(['Dog', 'Newbie']),
         ),
         None, None, True
     ),
     (
         "List with two items, setting string at index 2 (out of range)",
         dict(
-            nclist=NocaseList([u'Dog', u'Cat']),
+            nclist=NocaseList(['Dog', 'Cat']),
             index=2,
-            value=u'Newbie',
+            value='Newbie',
             exp_nclist=None,
         ),
         IndexError, None, True
     ),
+    (
+        "Updating string list at slice 0:2",
+        dict(
+            nclist=NocaseList(['A1', 'B2', 'C3', 'D4']),
+            index=slice(0, 2),
+            value=['XX', 'YY'],
+            exp_nclist=NocaseList(['XX', 'YY', 'C3', 'D4']),
+        ),
+        None, None, True
+    ),
+    (
+        "Updating string list at slice 0:2:2",
+        dict(
+            nclist=NocaseList(['A1', 'B2', 'C3', 'D4']),
+            index=slice(0, 4, 2),
+            value=['XX', 'YY'],
+            exp_nclist=NocaseList(['XX', 'B2', 'YY', 'D4']),
+        ),
+        None, None, True
+    ),
 ]
 
 
 @pytest.mark.parametrize(
     "desc, kwargs, exp_exc_types, exp_warn_types, condition",
     TESTCASES_NOCASELIST_SETITEM)
 @simplified_test_function
@@ -672,14 +686,32 @@
         dict(
             nclist=NocaseList(['Dog', 'Cat']),
             index=2,
             exp_nclist=None,
         ),
         IndexError, None, True
     ),
+    (
+        "Deleting string list at slice 0:2",
+        dict(
+            nclist=NocaseList(['A1', 'B2', 'C3', 'D4']),
+            index=slice(0, 2),
+            exp_nclist=NocaseList(['C3', 'D4']),
+        ),
+        None, None, True
+    ),
+    (
+        "Deleting string list at slice 0:2:2",
+        dict(
+            nclist=NocaseList(['A1', 'B2', 'C3', 'D4']),
+            index=slice(0, 4, 2),
+            exp_nclist=NocaseList(['B2', 'D4']),
+        ),
+        None, None, True
+    ),
 ]
 
 
 @pytest.mark.parametrize(
     "desc, kwargs, exp_exc_types, exp_warn_types, condition",
     TESTCASES_NOCASELIST_DELITEM)
 @simplified_test_function
@@ -784,15 +816,15 @@
         ),
         None if TEST_AGAINST_LIST else AttributeError, None, True
     ),
     (
         "Empty list, with non-existing empty unicode string value (not found)",
         dict(
             nclist=NocaseList(),
-            value=u'',
+            value='',
             exp_result=False,
         ),
         None, None, True
     ),
     (
         "Empty list, with non-existing empty byte string value (not found)",
         dict(
@@ -803,15 +835,15 @@
         None, None, True
     ),
     (
         "Empty list, with non-existing non-empty unicode string value "
         "(not found)",
         dict(
             nclist=NocaseList(),
-            value=u'Dog',
+            value='Dog',
             exp_result=False,
         ),
         None, None, True
     ),
     (
         "Empty list, with non-existing non-empty byte string value "
         "(not found)",
@@ -823,144 +855,144 @@
         None, None, True
     ),
 
     # Non-empty NocaseList
     (
         "List with two items, with None as value (no casefold method)",
         dict(
-            nclist=NocaseList([u'Dog', b'Cat']),
+            nclist=NocaseList(['Dog', b'Cat']),
             value=None,
             exp_result=False,
         ),
         None, None, True
     ),
     (
         "List with two items, with integer value 0 (no casefold method)",
         dict(
-            nclist=NocaseList([u'Dog', b'Cat']),
+            nclist=NocaseList(['Dog', b'Cat']),
             value=0,
             exp_result=False if TEST_AGAINST_LIST else None,
         ),
         None if TEST_AGAINST_LIST else AttributeError, None, True
     ),
     (
         "List with two items, with non-existing empty unicode string value "
         "(not found)",
         dict(
-            nclist=NocaseList([u'Dog', b'Cat']),
-            value=u'',
+            nclist=NocaseList(['Dog', b'Cat']),
+            value='',
             exp_result=False,
         ),
         None, None, True
     ),
     (
         "List with two items, with non-existing empty byte string value "
         "(not found)",
         dict(
-            nclist=NocaseList([u'Dog', b'Cat']),
+            nclist=NocaseList(['Dog', b'Cat']),
             value=b'',
             exp_result=False,
         ),
         None, None, True
     ),
     (
         "List with two items, with non-existing non-empty unicode string value "
         "(not found)",
         dict(
-            nclist=NocaseList([u'Dog', b'Cat']),
-            value=u'invalid',
+            nclist=NocaseList(['Dog', b'Cat']),
+            value='invalid',
             exp_result=False,
         ),
         None, None, True
     ),
     (
         "List with two items, with non-existing non-empty byte string value "
         "(not found)",
         dict(
-            nclist=NocaseList([u'Dog', b'Cat']),
+            nclist=NocaseList(['Dog', b'Cat']),
             value=b'invalid',
             exp_result=False,
         ),
         None, None, True
     ),
     (
         "List with two items, with existing unicode string value in original "
         "case",
         dict(
-            nclist=NocaseList([u'Dog', b'Cat']),
-            value=u'Dog',
+            nclist=NocaseList(['Dog', b'Cat']),
+            value='Dog',
             exp_result=True,
         ),
         None, None, True
     ),
     (
         "List with two items, with existing byte string value in original "
         "case",
         dict(
-            nclist=NocaseList([b'Dog', u'Cat']),
+            nclist=NocaseList([b'Dog', 'Cat']),
             value=b'Dog',
             exp_result=True,
         ),
         None, None, True
     ),
     (
         "List with two items, with existing unicode string value in "
         "non-original upper case",
         dict(
-            nclist=NocaseList([u'Dog', u'Cat']),
-            value=u'DOG',
+            nclist=NocaseList(['Dog', 'Cat']),
+            value='DOG',
             exp_result=not TEST_AGAINST_LIST,
         ),
         None, None, True
     ),
     (
         "List with two items, with existing byte string value in "
         "non-original upper case",
         dict(
-            nclist=NocaseList([b'Dog', u'Cat']),
+            nclist=NocaseList([b'Dog', 'Cat']),
             value=b'DOG',
             exp_result=not TEST_AGAINST_LIST,
         ),
         None, None, True
     ),
     (
         "List with two items, with existing unicode string value in "
         "non-original lower case",
         dict(
-            nclist=NocaseList([u'Dog', u'Cat']),
-            value=u'dog',
+            nclist=NocaseList(['Dog', 'Cat']),
+            value='dog',
             exp_result=not TEST_AGAINST_LIST,
         ),
         None, None, True
     ),
     (
         "List with two items, with existing byte string value in "
         "non-original lower case",
         dict(
-            nclist=NocaseList([b'Dog', u'Cat']),
+            nclist=NocaseList([b'Dog', 'Cat']),
             value=b'dog',
             exp_result=not TEST_AGAINST_LIST,
         ),
         None, None, True
     ),
     (
         "List with two items, with existing unicode string value in "
         "non-original mixed case",
         dict(
-            nclist=NocaseList([u'Dog', u'Cat']),
-            value=u'doG',
+            nclist=NocaseList(['Dog', 'Cat']),
+            value='doG',
             exp_result=not TEST_AGAINST_LIST,
         ),
         None, None, True
     ),
     (
         "List with two items, with existing byte string value in "
         "non-original mixed case",
         dict(
-            nclist=NocaseList([b'Dog', u'Cat']),
+            nclist=NocaseList([b'Dog', 'Cat']),
             value=b'doG',
             exp_result=not TEST_AGAINST_LIST,
         ),
         None, None, True
     ),
 ]
 
@@ -1723,18 +1755,73 @@
             exp_gt=False,
             exp_lt=True,
         ),
         None, None, True
     ),
 ]
 
+TESTCASES_NOCASELIST_EQUAL = [
+
+    # Testcases for NocaseList.__eq__(), __ne__()
+    (
+        "List compared with integer (valid and False)",
+        dict(
+            obj1=NocaseList(['Cat', 'Dog']),
+            obj2=42,
+            exp_eq=False,
+            exp_gt=None,  # not used
+            exp_lt=None,  # not used
+        ),
+        None, None, True
+    ),
+    (
+        "Integer compared with list (valid and False)",
+        dict(
+            obj1=42,
+            obj2=NocaseList(['Cat', 'Dog']),
+            exp_eq=False,
+            exp_gt=None,  # not used
+            exp_lt=None,  # not used
+        ),
+        None, None, True
+    ),
+]
+
+TESTCASES_NOCASELIST_ORDER = [
+
+    # Testcases for NocaseList.__gt__(), __le__()
+    # Testcases for NocaseList.__lt__(), __ge__()
+    (
+        "List compared with integer (invalid)",
+        dict(
+            obj1=NocaseList(['Cat', 'Dog']),
+            obj2=42,
+            exp_eq=None,  # not used
+            exp_gt=None,
+            exp_lt=None,
+        ),
+        TypeError, None, True
+    ),
+    (
+        "Integer compared with list (invalid)",
+        dict(
+            obj1=42,
+            obj2=NocaseList(['Cat', 'Dog']),
+            exp_eq=None,  # not used
+            exp_gt=None,
+            exp_lt=None,
+        ),
+        TypeError, None, True
+    ),
+]
+
 
 @pytest.mark.parametrize(
     "desc, kwargs, exp_exc_types, exp_warn_types, condition",
-    TESTCASES_NOCASELIST_COMPARE)
+    TESTCASES_NOCASELIST_COMPARE + TESTCASES_NOCASELIST_EQUAL)  # type: ignore
 @simplified_test_function
 def test_NocaseList_eq(testcase, obj1, obj2, exp_eq, exp_gt, exp_lt):
     # pylint: disable=unused-argument
     """
     Test function for NocaseList.__eq__()
     """
 
@@ -1751,15 +1838,15 @@
 
     assert eq1 == exp_eq
     assert eq2 == exp_eq
 
 
 @pytest.mark.parametrize(
     "desc, kwargs, exp_exc_types, exp_warn_types, condition",
-    TESTCASES_NOCASELIST_COMPARE)
+    TESTCASES_NOCASELIST_COMPARE + TESTCASES_NOCASELIST_EQUAL)  # type: ignore
 @simplified_test_function
 def test_NocaseList_ne(testcase, obj1, obj2, exp_eq, exp_gt, exp_lt):
     # pylint: disable=unused-argument
     """
     Test function for NocaseList.__ne__()
     """
 
@@ -1778,15 +1865,15 @@
 
     assert ne1 == exp_ne
     assert ne2 == exp_ne
 
 
 @pytest.mark.parametrize(
     "desc, kwargs, exp_exc_types, exp_warn_types, condition",
-    TESTCASES_NOCASELIST_COMPARE)
+    TESTCASES_NOCASELIST_COMPARE + TESTCASES_NOCASELIST_ORDER)  # type: ignore
 @simplified_test_function
 def test_NocaseList_gt(testcase, obj1, obj2, exp_eq, exp_gt, exp_lt):
     # pylint: disable=unused-argument
     """
     Test function for NocaseList.__gt__()
     """
 
@@ -1801,15 +1888,15 @@
     assert testcase.exp_exc_types is None
 
     assert gt == exp_gt
 
 
 @pytest.mark.parametrize(
     "desc, kwargs, exp_exc_types, exp_warn_types, condition",
-    TESTCASES_NOCASELIST_COMPARE)
+    TESTCASES_NOCASELIST_COMPARE + TESTCASES_NOCASELIST_ORDER)  # type: ignore
 @simplified_test_function
 def test_NocaseList_lt(testcase, obj1, obj2, exp_eq, exp_gt, exp_lt):
     # pylint: disable=unused-argument
     """
     Test function for NocaseList.__lt__()
     """
 
@@ -1824,15 +1911,15 @@
     assert testcase.exp_exc_types is None
 
     assert lt == exp_lt
 
 
 @pytest.mark.parametrize(
     "desc, kwargs, exp_exc_types, exp_warn_types, condition",
-    TESTCASES_NOCASELIST_COMPARE)
+    TESTCASES_NOCASELIST_COMPARE + TESTCASES_NOCASELIST_ORDER)  # type: ignore
 @simplified_test_function
 def test_NocaseList_ge(testcase, obj1, obj2, exp_eq, exp_gt, exp_lt):
     # pylint: disable=unused-argument
     """
     Test function for NocaseList.__ge__()
     """
 
@@ -1849,15 +1936,15 @@
     assert testcase.exp_exc_types is None
 
     assert ge == exp_ge
 
 
 @pytest.mark.parametrize(
     "desc, kwargs, exp_exc_types, exp_warn_types, condition",
-    TESTCASES_NOCASELIST_COMPARE)
+    TESTCASES_NOCASELIST_COMPARE + TESTCASES_NOCASELIST_ORDER)  # type: ignore
 @simplified_test_function
 def test_NocaseList_le(testcase, obj1, obj2, exp_eq, exp_gt, exp_lt):
     # pylint: disable=unused-argument
     """
     Test function for NocaseList.__le__()
     """
 
@@ -1993,22 +2080,22 @@
     # * condition: Boolean condition for testcase to run, or 'pdb' for debugger
 
     (
         "Empty list",
         dict(
             nclist=NocaseList(),
         ),
-        None if LIST_HAS_COPY else AttributeError, None, True
+        None, None, True
     ),
     (
         "List with two items",
         dict(
             nclist=NocaseList(['Dog', 'Cat']),
         ),
-        None if LIST_HAS_COPY else AttributeError, None, True
+        None, None, True
     ),
 ]
 
 
 @pytest.mark.parametrize(
     "desc, kwargs, exp_exc_types, exp_warn_types, condition",
     TESTCASES_NOCASELIST_COPY)
@@ -2044,22 +2131,22 @@
     # * condition: Boolean condition for testcase to run, or 'pdb' for debugger
 
     (
         "Empty list",
         dict(
             nclist=NocaseList(),
         ),
-        None if LIST_HAS_CLEAR else AttributeError, None, True
+        None, None, True
     ),
     (
         "List with two items",
         dict(
             nclist=NocaseList(['Dog', 'Cat']),
         ),
-        None if LIST_HAS_CLEAR else AttributeError, None, True
+        None, None, True
     ),
 ]
 
 
 @pytest.mark.parametrize(
     "desc, kwargs, exp_exc_types, exp_warn_types, condition",
     TESTCASES_NOCASELIST_CLEAR)
@@ -2881,17 +2968,14 @@
     """
     Test function for overriding the casefold method.
     """
 
     if TEST_AGAINST_LIST:
         pytest.skip("The override test does not support testing with list")
 
-    if six.PY2:
-        pytest.skip("The override test does not support Python 2")
-
     class MyNocaseList(NocaseList):
         "Test class that overrides the casefold method"
 
         @staticmethod
         def __casefold__(value):
             return unicodedata.normalize('NFKD', value).casefold()
```

### Comparing `nocaselist-1.1.1/tests/utils/import_installed.py` & `nocaselist-2.0.0/tests/utils/import_installed.py`

 * *Files identical despite different names*

### Comparing `nocaselist-1.1.1/tests/utils/simplified_test_function.py` & `nocaselist-2.0.0/tests/utils/simplified_test_function.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,15 @@
 simplified_test_function - Pytest extension for simplifying test functions.
 """
 
 from __future__ import absolute_import
 
 import functools
 from collections import namedtuple
-try:
-    from inspect import Signature, Parameter
-except ImportError:  # py2
-    from funcsigs import Signature, Parameter
+from inspect import Signature, Parameter  # type: ignore
 import pytest
 
 __all__ = ['simplified_test_function']
 
 
 # Pytest determines the signature of the test function by unpacking any
 # wrapped functions (this is the default of the signature() function it
```

