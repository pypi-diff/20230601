# Comparing `tmp/madtypes-0.0.6.tar.gz` & `tmp/madtypes-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "madtypes-0.0.6.tar", last modified: Wed May 31 12:15:56 2023, max compression
+gzip compressed data, was "madtypes-0.0.7.tar", last modified: Thu Jun  1 09:13:06 2023, max compression
```

## Comparing `madtypes-0.0.6.tar` & `madtypes-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:15:56.367192 madtypes-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     8369 2023-05-31 12:15:56.367192 madtypes-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7881 2023-05-31 12:15:45.000000 madtypes-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:15:56.367192 madtypes-0.0.6/madtypes/
--rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-05-31 12:15:45.000000 madtypes-0.0.6/madtypes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:15:56.367192 madtypes-0.0.6/madtypes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8369 2023-05-31 12:15:56.000000 madtypes-0.0.6/madtypes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-31 12:15:56.000000 madtypes-0.0.6/madtypes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 12:15:56.000000 madtypes-0.0.6/madtypes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-31 12:15:56.000000 madtypes-0.0.6/madtypes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 12:15:56.367192 madtypes-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-31 12:15:45.000000 madtypes-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:15:56.367192 madtypes-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    15579 2023-05-31 12:15:45.000000 madtypes-0.0.6/tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:13:06.890889 madtypes-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     9030 2023-06-01 09:13:06.890889 madtypes-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-06-01 09:12:55.000000 madtypes-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:13:06.886889 madtypes-0.0.7/madtypes/
+-rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-06-01 09:12:55.000000 madtypes-0.0.7/madtypes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:13:06.890889 madtypes-0.0.7/madtypes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9030 2023-06-01 09:13:06.000000 madtypes-0.0.7/madtypes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-01 09:13:06.000000 madtypes-0.0.7/madtypes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 09:13:06.000000 madtypes-0.0.7/madtypes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-01 09:13:06.000000 madtypes-0.0.7/madtypes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 09:13:06.890889 madtypes-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-01 09:12:55.000000 madtypes-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:13:06.890889 madtypes-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    16945 2023-06-01 09:12:55.000000 madtypes-0.0.7/tests/test_schema.py
```

### Comparing `madtypes-0.0.6/PKG-INFO` & `madtypes-0.0.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: madtypes
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python typing that raise TypeError at runtime
 Home-page: https://github.com/6r17/madtypes
 Author: 6r17
 Author-email: patrick.borowy@proton.me
 Keywords: typing,json,json-schema
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -231,15 +231,14 @@
     with pytest.raises(TypeError):
         Item()
 
 
 
 ```
 
-
 ### Multiple inheritance
 
 Sometimes technical contraints should not be rendered publicly, and you still want
 to use the existing class definitions.
 
 For instance one of those occurances is multiple objects that have different
 realities in the code, but have the same buisness organisation.
@@ -270,14 +269,36 @@
         "type": "object",
         "properties": {"foo": {"type": "string"}, "bar": {"type": "string"}},
         "required": ["foo", "bar"],
     }
 
 ```
 
+- ### Dynamicly remove a field
+
+It is possible to dynamicly remove a field from a class using the `subtract_fields(args: tuple[str])` decorator which will return a new class without the provided fields.
+
+```python
+
+def test_class_field_substraction():
+    class Item(Schema):
+        name: str
+        age: int
+
+    ageLessItem = subtract_fields("age")(Item)
+    # we can dynamicly create a new class by substracting fields from it
+    assert len(ageLessItem.get_fields()) == 1
+    with pytest.raises(TypeError):
+        ageLessItem(name="foo", age=2)
+    ageLessItem(name="foo")
+    with pytest.raises(AttributeError):
+        assert getattr(Item, "age")
+
+```
+
 - ### Immutables
 
 ```python
 from madtypes import Immutable # Immutable inherits from Schema
 
 class Foo(Immutable):
     name: str
```

### Comparing `madtypes-0.0.6/README.md` & `madtypes-0.0.7/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -216,15 +216,14 @@
     with pytest.raises(TypeError):
         Item()
 
 
 
 ```
 
-
 ### Multiple inheritance
 
 Sometimes technical contraints should not be rendered publicly, and you still want
 to use the existing class definitions.
 
 For instance one of those occurances is multiple objects that have different
 realities in the code, but have the same buisness organisation.
@@ -255,14 +254,36 @@
         "type": "object",
         "properties": {"foo": {"type": "string"}, "bar": {"type": "string"}},
         "required": ["foo", "bar"],
     }
 
 ```
 
+- ### Dynamicly remove a field
+
+It is possible to dynamicly remove a field from a class using the `subtract_fields(args: tuple[str])` decorator which will return a new class without the provided fields.
+
+```python
+
+def test_class_field_substraction():
+    class Item(Schema):
+        name: str
+        age: int
+
+    ageLessItem = subtract_fields("age")(Item)
+    # we can dynamicly create a new class by substracting fields from it
+    assert len(ageLessItem.get_fields()) == 1
+    with pytest.raises(TypeError):
+        ageLessItem(name="foo", age=2)
+    ageLessItem(name="foo")
+    with pytest.raises(AttributeError):
+        assert getattr(Item, "age")
+
+```
+
 - ### Immutables
 
 ```python
 from madtypes import Immutable # Immutable inherits from Schema
 
 class Foo(Immutable):
     name: str
```

### Comparing `madtypes-0.0.6/madtypes/__init__.py` & `madtypes-0.0.7/madtypes/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -72,17 +72,54 @@
             return instance
 
         # Assign the overridden __new__ method to the class
         attrs["__new__"] = new_method
         return super().__new__(cls, name, bases, attrs)
 
 
+def subtract_fields(*fields):
+    def decorator(cls):
+        new_annotations = cls.__annotations__.copy()
+        new_cls_dict = dict(cls.__dict__)
+
+        for field in fields:
+            if field in new_annotations:
+                del new_annotations[field]
+            if field in new_cls_dict:
+                del new_cls_dict[field]  # pragma: no cover (tested by getattr)
+
+        new_cls_dict["__annotations__"] = new_annotations
+
+        new_cls = type(cls.__name__, cls.__bases__, new_cls_dict)
+        return new_cls
+
+    return decorator
+
+
 class Schema(dict):
+    @classmethod
+    def get_fields(cls):
+        fields = list(cls.__annotations__.items())
+
+        # Check if the class inherits from another Schema
+        for base in cls.__bases__:
+            if issubclass(base, Schema):
+                # Retrieve the fields from the parent class
+                fields.extend(base.get_fields())
+
+        return fields
+
     def __init__(self, **kwargs):
-        for key, value in self.__annotations__.items():
+        fields = dict(self.get_fields())
+        for key, value in kwargs.items():
+            if key not in fields:
+                raise TypeError(
+                    f"{key} is not a key for {type(self).__name__}"
+                )
+        for key, value in fields.items():
             if key in kwargs:
                 if type_check(kwargs[key], value):
                     super().__setitem__(key, kwargs[key])
                 else:
                     raise TypeError(
                         f"{kwargs[key]} is not an instance of {value}"
                     )
@@ -93,26 +130,14 @@
         if not self.is_valid(**kwargs):
             raise TypeError(f"{kwargs} did not pass object validation")
 
     def is_valid(self, **__kwargs__) -> bool:
         """Validation at Object scope, for validation based on multiple fields."""
         return True
 
-    @classmethod
-    def get_fields(cls):
-        fields = list(cls.__annotations__.items())
-
-        # Check if the class inherits from another Schema
-        for base in cls.__bases__:
-            if issubclass(base, Schema):
-                # Retrieve the fields from the parent class
-                fields.extend(base.get_fields())
-
-        return fields
-
     def __getattr__(self, name):
         if name in self:
             return self[name]
         # I don't know how to trigger the next line, it's more of an `in-case'
         return super().__getattribute__(name)  # pragma: no cover
 
     def __setattr__(self, name, value):
```

### Comparing `madtypes-0.0.6/madtypes.egg-info/PKG-INFO` & `madtypes-0.0.7/madtypes.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: madtypes
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python typing that raise TypeError at runtime
 Home-page: https://github.com/6r17/madtypes
 Author: 6r17
 Author-email: patrick.borowy@proton.me
 Keywords: typing,json,json-schema
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -231,15 +231,14 @@
     with pytest.raises(TypeError):
         Item()
 
 
 
 ```
 
-
 ### Multiple inheritance
 
 Sometimes technical contraints should not be rendered publicly, and you still want
 to use the existing class definitions.
 
 For instance one of those occurances is multiple objects that have different
 realities in the code, but have the same buisness organisation.
@@ -270,14 +269,36 @@
         "type": "object",
         "properties": {"foo": {"type": "string"}, "bar": {"type": "string"}},
         "required": ["foo", "bar"],
     }
 
 ```
 
+- ### Dynamicly remove a field
+
+It is possible to dynamicly remove a field from a class using the `subtract_fields(args: tuple[str])` decorator which will return a new class without the provided fields.
+
+```python
+
+def test_class_field_substraction():
+    class Item(Schema):
+        name: str
+        age: int
+
+    ageLessItem = subtract_fields("age")(Item)
+    # we can dynamicly create a new class by substracting fields from it
+    assert len(ageLessItem.get_fields()) == 1
+    with pytest.raises(TypeError):
+        ageLessItem(name="foo", age=2)
+    ageLessItem(name="foo")
+    with pytest.raises(AttributeError):
+        assert getattr(Item, "age")
+
+```
+
 - ### Immutables
 
 ```python
 from madtypes import Immutable # Immutable inherits from Schema
 
 class Foo(Immutable):
     name: str
```

### Comparing `madtypes-0.0.6/setup.py` & `madtypes-0.0.7/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="madtypes",
-    version="0.0.6",
+    version="0.0.7",
     author="6r17",
     author_email="patrick.borowy@proton.me",
     description="Python typing that raise TypeError at runtime",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/6r17/madtypes",
     packages=find_packages(include=["madtypes"]),
```

### Comparing `madtypes-0.0.6/tests/test_schema.py` & `madtypes-0.0.7/tests/test_schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 from enum import Enum
 from typing import Optional
-from madtypes import json_schema, Schema, Annotation, Immutable, type_check
+from madtypes import (
+    json_schema,
+    Schema,
+    Annotation,
+    Immutable,
+    type_check,
+    subtract_fields,
+)
 import pytest
 import json
 
 
 class Gender(Schema):
     female: int
     male: int
@@ -573,34 +580,14 @@
                 "type": "string",
             }
         },
         "required": ["phone"],
     }
 
 
-def test_multiple_inheritance_json_schema():
-    class Foo(Schema):
-        foo: str
-
-    class Bar(Schema):
-        bar: str
-
-    class FooBar(Foo, Bar):
-        pass
-
-    assert len(FooBar.get_fields()) == 2
-    schema = json_schema(FooBar)
-    print(schema)
-    assert schema == {
-        "type": "object",
-        "properties": {"foo": {"type": "string"}, "bar": {"type": "string"}},
-        "required": ["foo", "bar"],
-    }
-
-
 def test_list_json_schema():
     class Foo(Schema):
         my_set: list[int]
 
     schema = json_schema(Foo)
     print(schema)
     assert schema == {
@@ -654,7 +641,86 @@
             "key": {"type": "string", "enum": ["Foo", "Bar", "Baz"]}
         },
         "required": ["key"],
     }
     Item(key=SomeEnum.FOO)
     with pytest.raises(TypeError):
         Item(key="Foo")
+
+
+def test_class_field_substraction():
+    class Item(Schema):
+        name: str
+        age: int
+
+    ageLessItem = subtract_fields("age")(Item)
+    # we can dynamicly create a new class by substracting fields from it
+    assert len(ageLessItem.get_fields()) == 1
+    with pytest.raises(TypeError):
+        ageLessItem(name="foo", age=2)
+    ageLessItem(name="foo")
+    with pytest.raises(AttributeError):
+        assert getattr(Item, "age")
+
+
+def test_json_schema_after_substraction():
+    class Item(Schema):
+        name: str
+        age: int
+
+    ageLessItem = subtract_fields("age")(Item)
+    schema = json_schema(ageLessItem)
+    print(schema)
+    assert schema == {
+        "type": "object",
+        "properties": {"name": {"type": "string"}},
+        "required": ["name"],
+    }
+
+
+def test_multiple_inheritance_json_schema():
+    class Foo(Schema):
+        foo: str
+
+    class Bar(Schema):
+        bar: str
+
+    class FooBar(Foo, Bar):
+        pass
+
+    assert len(FooBar.get_fields()) == 2
+    schema = json_schema(FooBar)
+    print(schema)
+    assert schema == {
+        "type": "object",
+        "properties": {"foo": {"type": "string"}, "bar": {"type": "string"}},
+        "required": ["foo", "bar"],
+    }
+
+
+def test_multiple_inheritance_integrity():
+    class Foo(Schema):
+        foo: str
+
+    class Bar(Schema):
+        bar: str
+
+    class FooBar(Foo, Bar):
+        pass
+
+    FooBar(foo="foo", bar="bar")
+
+
+def test_json_schema_after_edition_and_multiple_inheritance():
+    class Person(Schema):
+        name: str
+        age: int
+
+    class Contact(Schema):
+        phone: str
+
+    agelessPerson = subtract_fields("age")(Person)
+
+    class NamedContact(agelessPerson, Contact):
+        pass
+
+    NamedContact(name="foo", phone="baz")
```

