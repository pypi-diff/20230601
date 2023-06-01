# Comparing `tmp/lidipy-0.1.0.tar.gz` & `tmp/lidipy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lidipy-0.1.0.tar", max compression
+gzip compressed data, was "lidipy-0.1.1.tar", max compression
```

## Comparing `lidipy-0.1.0.tar` & `lidipy-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1067 2023-06-01 09:15:30.484204 lidipy-0.1.0/LICENSE
--rw-r--r--   0        0        0     3042 2023-06-01 09:15:30.484204 lidipy-0.1.0/README.md
--rw-r--r--   0        0        0      973 2023-06-01 09:15:30.484204 lidipy-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       36 2023-06-01 09:15:30.484204 lidipy-0.1.0/src/lidipy/__init__.py
--rw-r--r--   0        0        0     1446 2023-06-01 09:15:30.484204 lidipy-0.1.0/src/lidipy/container.py
--rw-r--r--   0        0        0       96 2023-06-01 09:15:30.484204 lidipy-0.1.0/src/lidipy/exceptions.py
--rw-r--r--   0        0        0     3437 1970-01-01 00:00:00.000000 lidipy-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-01 10:35:45.704356 lidipy-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4075 2023-06-01 10:35:45.704356 lidipy-0.1.1/README.md
+-rw-r--r--   0        0        0      973 2023-06-01 10:35:45.704356 lidipy-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       36 2023-06-01 10:35:45.704356 lidipy-0.1.1/src/lidipy/__init__.py
+-rw-r--r--   0        0        0     1446 2023-06-01 10:35:45.704356 lidipy-0.1.1/src/lidipy/container.py
+-rw-r--r--   0        0        0       96 2023-06-01 10:35:45.704356 lidipy-0.1.1/src/lidipy/exceptions.py
+-rw-r--r--   0        0        0     4470 1970-01-01 00:00:00.000000 lidipy-0.1.1/PKG-INFO
```

### Comparing `lidipy-0.1.0/LICENSE` & `lidipy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lidipy-0.1.0/README.md` & `lidipy-0.1.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+[![Coverage Status](https://coveralls.io/repos/github/AlTosterino/Lidi/badge.svg?branch=main)](https://coveralls.io/github/AlTosterino/Lidi?branch=main)
+
 # Lidi (LIghtweight Dependency Injector)
 
 Lidi is a lightweight dependency injector designed to simplify dependency management in your Python projects.
 It provides a simple and intuitive API for binding classes and resolving dependencies.
 
 ## Installation
 
@@ -25,100 +27,140 @@
     pass
 
 
 class Child:
     pass
 
 
-lidipy = Lidi()
+lidi = Lidi()
 # bind instance
-lidipy.bind(Parent, Child())
+lidi.bind(Parent, Child())
 
 # or bind a callable
-lidipy.bind(Parent, Child)
+lidi.bind(Parent, Child)
 ```
 
 ### Singleton Binding
 
 If you want to bind a class as a singleton, you can pass the `singleton` parameter as `True` when calling the `bind()` method:
 
 ```python
-lidipy.bind(Parent, Child(), singleton=True)
+lidi.bind(Parent, Child(), singleton=True)
 ```
 
 With singleton binding, the same instance of the class will be returned every time it is resolved.
 
 ### Resolving Dependencies
 
 To resolve a class and its dependencies, you can use the `resolve()` method of the Lidi class:
 
 ```python
-instance = lidipy.resolve(Parent) # instance is Child()
+instance = lidi.resolve(Parent) # instance is Child()
 ```
 
 If the class was bound as a singleton, the same instance will be returned each time it is resolved.
 
 ### Deferred Resolution
 
 Lidi also supports deferred resolution using the resolve_defer() method. This method returns a callable that, when invoked, resolves the class:
 
 ```python
-deferred_resolve = lidipy.resolve_defer(Parent)
+deferred_resolve = lidi.resolve_defer(Parent)
 instance = deferred_resolve()
 ```
 
 Deferred resolution can be useful when you want to defer the instantiation of a class until it is actually needed.
 
 ### Handling Missing Bindings
 
 If a binding is missing for a requested type, a `BindingMissing` exception will be raised.
 You can handle this exception and provide appropriate error handling in your application.
 
 ```python
 from lidipy import BindingMissing
 
 try:
-    instance = lidipy.resolve(Mother)
+    instance = lidi.resolve(Mother)
 except BindingMissing as e:
     print(e)  # Outputs: "Binding missing for type: Mother"
 ```
 
 ### Usage with Dataclasses
 
 Lidi can be used seamlessly with Python's dataclasses. Here's an example of how to use dataclasses with Lidi:
 
 ```python
 from dataclasses import dataclass
 from lidipy import Lidi
 
-lidipy = Lidi()
+lidi = Lidi()
 
 
-@dataclass
+@dataclass(frozen=True)
 class Config:
     db_url: str
-
+    
+# Bind Config
+lidi.bind(Config, Config(db_url="example.com:5432"))
 
 @dataclass
 class Database:
-    config: Config = lidipy.resolve(Config)
+    config: Config = lidi.resolve(Config)
 
     def connect(self):
         print(f"Connecting to database at {self.config.db_url}")
 
 
-# Bind the dependencies
-lidipy.bind(Config, Config(db_url="example.com:5432"))
-lidipy.bind(Database, Database)
+# Bind Database
+lidi.bind(Database, Database)
 
 # Resolve the dataclass with dependencies
-database = lidipy.resolve(Database)
+database = lidi.resolve(Database)
 database.connect()  # Output: Connecting to database at example.com:5432
 ```
 
+## Dynamic binds on runtine
+
+Lidi supports bindings change on runtime, here's an example:
+
+```python
+from dataclasses import dataclass, field
+from lidipy import Lidi
+
+lidi = Lidi()
+
+
+@dataclass
+class Config:
+    db_url: str
+
+
+@dataclass
+class Database:
+    config: Config = field(default_factory=lidi.resolve_defer(Config))
+
+    def connect(self):
+        print(f"Connecting to database at {self.config.db_url}")
+
+
+# Bind the initial dependencies
+lidi.bind(Config, Config(db_url="example.com:5432"))
+lidi.bind(Database, Database)
+
+# Initial resolve
+database = lidi.resolve(Database)
+database.connect()  # Output: Connecting to database at example.com:5432
+
+# Dynamically change binding
+lidi.bind(Config, Config(db_url="other-example.com:5432"))
+
+# Second resolve
+database = lidi.resolve(Database)
+database.connect()  # Output: Connecting to database at other-example.com:5432
+```
 ## Contributing
 
 Contributions are welcome! If you find a bug or want to suggest an improvement, please open an issue or submit a pull request on the GitHub repository.
 
 ## License
 
 Lidi is licensed under the MIT License.
```

### Comparing `lidipy-0.1.0/pyproject.toml` & `lidipy-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lidipy"
-version = "0.1.0"
+version = "0.1.1"
 description = "Lidi is a lightweight dependency injector designed to simplify dependency management in your Python projects."
 authors = ["AlTosterino <altosterino@gmail.com>"]
 readme = "README.md"
 packages = [{include = "lidipy", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `lidipy-0.1.0/src/lidipy/container.py` & `lidipy-0.1.1/src/lidipy/container.py`

 * *Files identical despite different names*

### Comparing `lidipy-0.1.0/PKG-INFO` & `lidipy-0.1.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: lidipy
-Version: 0.1.0
+Version: 0.1.1
 Summary: Lidi is a lightweight dependency injector designed to simplify dependency management in your Python projects.
 Author: AlTosterino
 Author-email: altosterino@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
+[![Coverage Status](https://coveralls.io/repos/github/AlTosterino/Lidi/badge.svg?branch=main)](https://coveralls.io/github/AlTosterino/Lidi?branch=main)
+
 # Lidi (LIghtweight Dependency Injector)
 
 Lidi is a lightweight dependency injector designed to simplify dependency management in your Python projects.
 It provides a simple and intuitive API for binding classes and resolving dependencies.
 
 ## Installation
 
@@ -36,100 +38,140 @@
     pass
 
 
 class Child:
     pass
 
 
-lidipy = Lidi()
+lidi = Lidi()
 # bind instance
-lidipy.bind(Parent, Child())
+lidi.bind(Parent, Child())
 
 # or bind a callable
-lidipy.bind(Parent, Child)
+lidi.bind(Parent, Child)
 ```
 
 ### Singleton Binding
 
 If you want to bind a class as a singleton, you can pass the `singleton` parameter as `True` when calling the `bind()` method:
 
 ```python
-lidipy.bind(Parent, Child(), singleton=True)
+lidi.bind(Parent, Child(), singleton=True)
 ```
 
 With singleton binding, the same instance of the class will be returned every time it is resolved.
 
 ### Resolving Dependencies
 
 To resolve a class and its dependencies, you can use the `resolve()` method of the Lidi class:
 
 ```python
-instance = lidipy.resolve(Parent) # instance is Child()
+instance = lidi.resolve(Parent) # instance is Child()
 ```
 
 If the class was bound as a singleton, the same instance will be returned each time it is resolved.
 
 ### Deferred Resolution
 
 Lidi also supports deferred resolution using the resolve_defer() method. This method returns a callable that, when invoked, resolves the class:
 
 ```python
-deferred_resolve = lidipy.resolve_defer(Parent)
+deferred_resolve = lidi.resolve_defer(Parent)
 instance = deferred_resolve()
 ```
 
 Deferred resolution can be useful when you want to defer the instantiation of a class until it is actually needed.
 
 ### Handling Missing Bindings
 
 If a binding is missing for a requested type, a `BindingMissing` exception will be raised.
 You can handle this exception and provide appropriate error handling in your application.
 
 ```python
 from lidipy import BindingMissing
 
 try:
-    instance = lidipy.resolve(Mother)
+    instance = lidi.resolve(Mother)
 except BindingMissing as e:
     print(e)  # Outputs: "Binding missing for type: Mother"
 ```
 
 ### Usage with Dataclasses
 
 Lidi can be used seamlessly with Python's dataclasses. Here's an example of how to use dataclasses with Lidi:
 
 ```python
 from dataclasses import dataclass
 from lidipy import Lidi
 
-lidipy = Lidi()
+lidi = Lidi()
 
 
-@dataclass
+@dataclass(frozen=True)
 class Config:
     db_url: str
-
+    
+# Bind Config
+lidi.bind(Config, Config(db_url="example.com:5432"))
 
 @dataclass
 class Database:
-    config: Config = lidipy.resolve(Config)
+    config: Config = lidi.resolve(Config)
 
     def connect(self):
         print(f"Connecting to database at {self.config.db_url}")
 
 
-# Bind the dependencies
-lidipy.bind(Config, Config(db_url="example.com:5432"))
-lidipy.bind(Database, Database)
+# Bind Database
+lidi.bind(Database, Database)
 
 # Resolve the dataclass with dependencies
-database = lidipy.resolve(Database)
+database = lidi.resolve(Database)
 database.connect()  # Output: Connecting to database at example.com:5432
 ```
 
+## Dynamic binds on runtine
+
+Lidi supports bindings change on runtime, here's an example:
+
+```python
+from dataclasses import dataclass, field
+from lidipy import Lidi
+
+lidi = Lidi()
+
+
+@dataclass
+class Config:
+    db_url: str
+
+
+@dataclass
+class Database:
+    config: Config = field(default_factory=lidi.resolve_defer(Config))
+
+    def connect(self):
+        print(f"Connecting to database at {self.config.db_url}")
+
+
+# Bind the initial dependencies
+lidi.bind(Config, Config(db_url="example.com:5432"))
+lidi.bind(Database, Database)
+
+# Initial resolve
+database = lidi.resolve(Database)
+database.connect()  # Output: Connecting to database at example.com:5432
+
+# Dynamically change binding
+lidi.bind(Config, Config(db_url="other-example.com:5432"))
+
+# Second resolve
+database = lidi.resolve(Database)
+database.connect()  # Output: Connecting to database at other-example.com:5432
+```
 ## Contributing
 
 Contributions are welcome! If you find a bug or want to suggest an improvement, please open an issue or submit a pull request on the GitHub repository.
 
 ## License
 
 Lidi is licensed under the MIT License.
```

