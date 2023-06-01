# Comparing `tmp/hdlib-0.1.3.tar.gz` & `tmp/hdlib-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdlib-0.1.3.tar", last modified: Thu Jun  1 00:03:52 2023, max compression
+gzip compressed data, was "hdlib-0.1.4.tar", last modified: Thu Jun  1 16:20:08 2023, max compression
```

## Comparing `hdlib-0.1.3.tar` & `hdlib-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-06-01 00:03:52.743301 hdlib-0.1.3/
--rw-r--r--   0 fabio      (501) staff       (20)     1068 2022-04-25 18:30:15.000000 hdlib-0.1.3/LICENSE
--rw-r--r--   0 fabio      (501) staff       (20)     8445 2023-06-01 00:03:52.741468 hdlib-0.1.3/PKG-INFO
--rw-r--r--   0 fabio      (501) staff       (20)     7811 2023-05-31 23:33:33.000000 hdlib-0.1.3/README.md
-drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-06-01 00:03:52.596617 hdlib-0.1.3/hdlib/
--rw-r--r--   0 fabio      (501) staff       (20)      102 2023-05-31 22:32:46.000000 hdlib-0.1.3/hdlib/__init__.py
--rw-r--r--   0 fabio      (501) staff       (20)     2489 2023-05-31 21:27:15.000000 hdlib-0.1.3/hdlib/arithmetic.py
--rw-r--r--   0 fabio      (501) staff       (20)    18474 2023-05-31 23:32:49.000000 hdlib-0.1.3/hdlib/space.py
-drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-06-01 00:03:52.696604 hdlib-0.1.3/hdlib.egg-info/
--rw-r--r--   0 fabio      (501) staff       (20)     8445 2023-06-01 00:03:52.000000 hdlib-0.1.3/hdlib.egg-info/PKG-INFO
--rw-r--r--   0 fabio      (501) staff       (20)      264 2023-06-01 00:03:52.000000 hdlib-0.1.3/hdlib.egg-info/SOURCES.txt
--rw-r--r--   0 fabio      (501) staff       (20)        1 2023-06-01 00:03:52.000000 hdlib-0.1.3/hdlib.egg-info/dependency_links.txt
--rw-r--r--   0 fabio      (501) staff       (20)        1 2023-06-01 00:03:52.000000 hdlib-0.1.3/hdlib.egg-info/not-zip-safe
--rw-r--r--   0 fabio      (501) staff       (20)       14 2023-06-01 00:03:52.000000 hdlib-0.1.3/hdlib.egg-info/requires.txt
--rw-r--r--   0 fabio      (501) staff       (20)        6 2023-06-01 00:03:52.000000 hdlib-0.1.3/hdlib.egg-info/top_level.txt
--rw-r--r--   0 fabio      (501) staff       (20)       38 2023-06-01 00:03:52.743990 hdlib-0.1.3/setup.cfg
--rw-r--r--   0 fabio      (501) staff       (20)     1195 2023-05-31 01:45:31.000000 hdlib-0.1.3/setup.py
-drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-06-01 00:03:52.737342 hdlib-0.1.3/test/
--rw-r--r--   0 fabio      (501) staff       (20)     6578 2023-05-31 23:16:43.000000 hdlib-0.1.3/test/test.py
+drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-06-01 16:20:08.356872 hdlib-0.1.4/
+-rw-r--r--   0 fabio      (501) staff       (20)     1068 2022-04-25 18:30:15.000000 hdlib-0.1.4/LICENSE
+-rw-r--r--   0 fabio      (501) staff       (20)     9027 2023-06-01 16:20:08.355404 hdlib-0.1.4/PKG-INFO
+-rw-r--r--   0 fabio      (501) staff       (20)     8393 2023-06-01 16:15:34.000000 hdlib-0.1.4/README.md
+drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-06-01 16:20:08.157300 hdlib-0.1.4/hdlib/
+-rw-r--r--   0 fabio      (501) staff       (20)      102 2023-06-01 13:34:35.000000 hdlib-0.1.4/hdlib/__init__.py
+-rw-r--r--   0 fabio      (501) staff       (20)     2480 2023-06-01 14:38:17.000000 hdlib-0.1.4/hdlib/arithmetic.py
+-rw-r--r--   0 fabio      (501) staff       (20)     2241 2023-06-01 14:42:50.000000 hdlib-0.1.4/hdlib/parser.py
+-rw-r--r--   0 fabio      (501) staff       (20)    20192 2023-06-01 15:29:21.000000 hdlib-0.1.4/hdlib/space.py
+drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-06-01 16:20:08.309007 hdlib-0.1.4/hdlib.egg-info/
+-rw-r--r--   0 fabio      (501) staff       (20)     9027 2023-06-01 16:20:07.000000 hdlib-0.1.4/hdlib.egg-info/PKG-INFO
+-rw-r--r--   0 fabio      (501) staff       (20)      280 2023-06-01 16:20:07.000000 hdlib-0.1.4/hdlib.egg-info/SOURCES.txt
+-rw-r--r--   0 fabio      (501) staff       (20)        1 2023-06-01 16:20:07.000000 hdlib-0.1.4/hdlib.egg-info/dependency_links.txt
+-rw-r--r--   0 fabio      (501) staff       (20)        1 2023-06-01 16:20:07.000000 hdlib-0.1.4/hdlib.egg-info/not-zip-safe
+-rw-r--r--   0 fabio      (501) staff       (20)       14 2023-06-01 16:20:07.000000 hdlib-0.1.4/hdlib.egg-info/requires.txt
+-rw-r--r--   0 fabio      (501) staff       (20)        6 2023-06-01 16:20:07.000000 hdlib-0.1.4/hdlib.egg-info/top_level.txt
+-rw-r--r--   0 fabio      (501) staff       (20)       38 2023-06-01 16:20:08.357214 hdlib-0.1.4/setup.cfg
+-rw-r--r--   0 fabio      (501) staff       (20)     1195 2023-05-31 01:45:31.000000 hdlib-0.1.4/setup.py
+drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-06-01 16:20:08.331489 hdlib-0.1.4/test/
+-rw-r--r--   0 fabio      (501) staff       (20)     6578 2023-05-31 23:16:43.000000 hdlib-0.1.4/test/test.py
```

### Comparing `hdlib-0.1.3/LICENSE` & `hdlib-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hdlib-0.1.3/PKG-INFO` & `hdlib-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdlib
-Version: 0.1.3
+Version: 0.1.4
 Summary: Hyperdimensional Computing Library for building Vector Symbolic Architectures in Python
 Home-page: http://github.com/cumbof/hdlib
 Author: Fabio Cumbo
 Author-email: fabio.cumbo@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
@@ -108,28 +108,28 @@
 ```
 
 > **Note**
 > In this last example, similarly to Vector objects, a Space object is built by loading the content of a pickle file. Space objects can be saved to pickle files with the `dump()` method as in the following example: `space.dump(to_file="~/space.pkl")`
 
 Here is the list of Space class methods:
 
-| Method       | Signature                                       | Description  |
-|:-------------|:------------------------------------------------|:-------------|
-| `memory`     |                                                 | Return a list with Vector IDs |
-| `get`        | `names: list, tags: list`                       | Return a list of Vector objects based on a list of Vector IDs or tags |
-| `insert`     | `vector: Vector`                                | Insert a Vector object into the Space |
-| `bulkInsert` | `names: list, tags: list`                       | Automatically create a Vector object for each of the ID in the input `names` list and finally insert them into the Space. Also tag vectors based on tags in the `tags` list of lists. Tags in position `i` are assigned to the Vector object whose name is in position `i` of the `vectors` list |
-| `remove`     | `name: str`                                     | Remove a Vector object from the Space based on its ID |
-| `add_tag`    | `name: str, tag: str`                           | Assign a tag to a Vector object in the Space |
-| `remove_tag` | `name: str, tag: str`                           | Remove a tag to a Vector object in the Space |
-| `link`       | `name1: str, name2: str`                        | Link two vectors in the Space. Note that links are directed |
-| `set_root`   | `name: str`                                     | Vector links can be used to define a tree structure. Set a specific vector as root |
-| `find`       | `vector: Vector, threshold: float, method: str` | Given a specific Vector object, search for the closest Vector in the Space according to a specific distance metric: `cosine`, `hamming`, or `euclidean` |
-| `find_all`   | `vector: Vector, threshold: float, method: str` | Report the distance between the input Vector object and all the other Vectors in the Space |
-| `dump`       | `to_file: str`                                  | Dump the Space object to a pickle file |
+| Method        | Signature                                       | Description  |
+|:--------------|:------------------------------------------------|:-------------|
+| `memory`      |                                                 | Return a list with Vector IDs |
+| `get`         | `names: list, tags: list`                       | Return a list of Vector objects based on a list of Vector IDs or tags |
+| `insert`      | `vector: Vector`                                | Insert a Vector object into the Space |
+| `bulk_insert` | `names: list, tags: list`                       | Automatically create a Vector object for each of the ID in the input `names` list and finally insert them into the Space. Also tag vectors based on tags in the `tags` list of lists. Tags in position `i` are assigned to the Vector object whose name is in position `i` of the `vectors` list |
+| `remove`      | `name: str`                                     | Remove a Vector object from the Space based on its ID |
+| `add_tag`     | `name: str, tag: str`                           | Assign a tag to a Vector object in the Space |
+| `remove_tag`  | `name: str, tag: str`                           | Remove a tag to a Vector object in the Space |
+| `link`        | `name1: str, name2: str`                        | Link two vectors in the Space. Note that links are directed |
+| `set_root`    | `name: str`                                     | Vector links can be used to define a tree structure. Set a specific vector as root |
+| `find`        | `vector: Vector, threshold: float, method: str` | Given a specific Vector object, search for the closest Vector in the Space according to a specific distance metric: `cosine`, `hamming`, or `euclidean` |
+| `find_all`    | `vector: Vector, threshold: float, method: str` | Report the distance between the input Vector object and all the other Vectors in the Space |
+| `dump`        | `to_file: str`                                  | Dump the Space object to a pickle file |
 
 ### Arithmetic Operations
 
 A Vector Symbolic Architecture (a.k.a. Hyperdimensional Computing) is composed of vectors in the hyperdimensional space and a series of arithmetic operations to manipulate vectors.
 
 The `hdlib` library provides three operators under the `arithmetic` module: `bundle`, `bind`, and `permute`.
 
@@ -137,12 +137,21 @@
 
 | Operator       | Properties  |
 |:---------------|:------------|
 | `bundle`       | (i) The resulting vector is similar to the input vectors, (ii) the more vectors are involved in bundling, the harder it is to determine the component vectors, and (iii) if several copies of any vector are included in bundling, the resulting vector is closer to the dominant vector than to the other components |
 | `bind`         | (i) Invertible (unbind), (ii) it distributes over bundling, (iii) it preserves the distance, and (iv) the resulting vector is dissimilar to the input vectors |
 | `permute`      | (i) Invertible, (ii) it distributes over bundling and any elementwise operation, (iii) it preserves the distance, and (iv) the resulting vector is dissimilar to the input vectors |
 
+### Utilities
+
+The `hdlib` library also provides a set of utilities for dealing with input datasets collected under the `parser` module:
+
+| Method          | Signature                 | Description  |
+|:----------------|:--------------------------|:-------------|
+| `load_dataset`  | `filepath: str, sep: str` | Given a numerical matrix file, load the list of samples, features, classes, and the matrix with numerical data |
+| `split_dataset` | `points: int, folds: int` | Given a number of data points and the number of folds, split a dataset into different folds |
+
 ## Contributing
 
 Long-term discussion and bug reports are maintained via GitHub Issues, while code review is managed via GitHub Pull Requests.
 
 Please, (i) be sure that there are no existing issues/PR concerning the same bug or improvement before opening a new issue/PR; (ii) write a clear and concise description of what the bug/PR is about; (iii) specifying the list of steps to reproduce the behavior in addition to versions and other technical details is highly recommended.
```

### Comparing `hdlib-0.1.3/README.md` & `hdlib-0.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -90,28 +90,28 @@
 ```
 
 > **Note**
 > In this last example, similarly to Vector objects, a Space object is built by loading the content of a pickle file. Space objects can be saved to pickle files with the `dump()` method as in the following example: `space.dump(to_file="~/space.pkl")`
 
 Here is the list of Space class methods:
 
-| Method       | Signature                                       | Description  |
-|:-------------|:------------------------------------------------|:-------------|
-| `memory`     |                                                 | Return a list with Vector IDs |
-| `get`        | `names: list, tags: list`                       | Return a list of Vector objects based on a list of Vector IDs or tags |
-| `insert`     | `vector: Vector`                                | Insert a Vector object into the Space |
-| `bulkInsert` | `names: list, tags: list`                       | Automatically create a Vector object for each of the ID in the input `names` list and finally insert them into the Space. Also tag vectors based on tags in the `tags` list of lists. Tags in position `i` are assigned to the Vector object whose name is in position `i` of the `vectors` list |
-| `remove`     | `name: str`                                     | Remove a Vector object from the Space based on its ID |
-| `add_tag`    | `name: str, tag: str`                           | Assign a tag to a Vector object in the Space |
-| `remove_tag` | `name: str, tag: str`                           | Remove a tag to a Vector object in the Space |
-| `link`       | `name1: str, name2: str`                        | Link two vectors in the Space. Note that links are directed |
-| `set_root`   | `name: str`                                     | Vector links can be used to define a tree structure. Set a specific vector as root |
-| `find`       | `vector: Vector, threshold: float, method: str` | Given a specific Vector object, search for the closest Vector in the Space according to a specific distance metric: `cosine`, `hamming`, or `euclidean` |
-| `find_all`   | `vector: Vector, threshold: float, method: str` | Report the distance between the input Vector object and all the other Vectors in the Space |
-| `dump`       | `to_file: str`                                  | Dump the Space object to a pickle file |
+| Method        | Signature                                       | Description  |
+|:--------------|:------------------------------------------------|:-------------|
+| `memory`      |                                                 | Return a list with Vector IDs |
+| `get`         | `names: list, tags: list`                       | Return a list of Vector objects based on a list of Vector IDs or tags |
+| `insert`      | `vector: Vector`                                | Insert a Vector object into the Space |
+| `bulk_insert` | `names: list, tags: list`                       | Automatically create a Vector object for each of the ID in the input `names` list and finally insert them into the Space. Also tag vectors based on tags in the `tags` list of lists. Tags in position `i` are assigned to the Vector object whose name is in position `i` of the `vectors` list |
+| `remove`      | `name: str`                                     | Remove a Vector object from the Space based on its ID |
+| `add_tag`     | `name: str, tag: str`                           | Assign a tag to a Vector object in the Space |
+| `remove_tag`  | `name: str, tag: str`                           | Remove a tag to a Vector object in the Space |
+| `link`        | `name1: str, name2: str`                        | Link two vectors in the Space. Note that links are directed |
+| `set_root`    | `name: str`                                     | Vector links can be used to define a tree structure. Set a specific vector as root |
+| `find`        | `vector: Vector, threshold: float, method: str` | Given a specific Vector object, search for the closest Vector in the Space according to a specific distance metric: `cosine`, `hamming`, or `euclidean` |
+| `find_all`    | `vector: Vector, threshold: float, method: str` | Report the distance between the input Vector object and all the other Vectors in the Space |
+| `dump`        | `to_file: str`                                  | Dump the Space object to a pickle file |
 
 ### Arithmetic Operations
 
 A Vector Symbolic Architecture (a.k.a. Hyperdimensional Computing) is composed of vectors in the hyperdimensional space and a series of arithmetic operations to manipulate vectors.
 
 The `hdlib` library provides three operators under the `arithmetic` module: `bundle`, `bind`, and `permute`.
 
@@ -119,12 +119,21 @@
 
 | Operator       | Properties  |
 |:---------------|:------------|
 | `bundle`       | (i) The resulting vector is similar to the input vectors, (ii) the more vectors are involved in bundling, the harder it is to determine the component vectors, and (iii) if several copies of any vector are included in bundling, the resulting vector is closer to the dominant vector than to the other components |
 | `bind`         | (i) Invertible (unbind), (ii) it distributes over bundling, (iii) it preserves the distance, and (iv) the resulting vector is dissimilar to the input vectors |
 | `permute`      | (i) Invertible, (ii) it distributes over bundling and any elementwise operation, (iii) it preserves the distance, and (iv) the resulting vector is dissimilar to the input vectors |
 
+### Utilities
+
+The `hdlib` library also provides a set of utilities for dealing with input datasets collected under the `parser` module:
+
+| Method          | Signature                 | Description  |
+|:----------------|:--------------------------|:-------------|
+| `load_dataset`  | `filepath: str, sep: str` | Given a numerical matrix file, load the list of samples, features, classes, and the matrix with numerical data |
+| `split_dataset` | `points: int, folds: int` | Given a number of data points and the number of folds, split a dataset into different folds |
+
 ## Contributing
 
 Long-term discussion and bug reports are maintained via GitHub Issues, while code review is managed via GitHub Pull Requests.
 
 Please, (i) be sure that there are no existing issues/PR concerning the same bug or improvement before opening a new issue/PR; (ii) write a clear and concise description of what the bug/PR is about; (iii) specifying the list of steps to reproduce the behavior in addition to versions and other technical details is highly recommended.
```

### Comparing `hdlib-0.1.3/hdlib/arithmetic.py` & `hdlib-0.1.4/hdlib/arithmetic.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         raise Exception("Vectors must have the same size")
 
     if vector1.vtype != vector2.vtype:
         raise Exception("Vector types are not compatible")
 
     vector = vector1.vector + vector2.vector
 
-    tags = list(set(vector1.tags).union(set(vector2.tags)))
+    tags = set(vector1.tags).union(set(vector2.tags))
 
     return Vector(size=vector1.size, vector=vector, tags=tags, vtype=vector1.vtype, seed=vector1.seed)
 
 
 def bind(vector1: Vector, vector2: Vector) -> Vector:
     """
     Bind vectors
@@ -53,30 +53,30 @@
         raise Exception("Vectors must have the same size")
 
     if vector1.vtype != vector2.vtype:
         raise Exception("Vector types are not compatible")
 
     vector = vector1.vector * vector2.vector
 
-    tags = list(set(vector1.tags).union(set(vector2.tags)))
+    tags = set(vector1.tags).union(set(vector2.tags))
 
     return Vector(size=vector1.size, vector=vector, tags=tags, vtype=vector1.vtype, seed=vector1.seed)
 
 
-def permute(vector: Vector, rotateby: int=1) -> Vector:
+def permute(vector: Vector, rotate_by: int=1) -> Vector:
     """
     Permute vector
 
     Properties:
     > Invertible
     > It distributes over bundling and any elementwise operation
     > It preserves the distance
     > The resulting vector is dissimilar to the input vectors
 
     :param vector:      Vector object
-    :param rotateby:    How many rotations
-    :return:            Input vector rotated "rotateby" times
+    :param rotate_by:   How many rotations
+    :return:            Input vector rotated "rotate_by" times
     """
 
-    rolled = np.roll(vector.vector, rotateby, axis=0)
+    rolled = np.roll(vector.vector, rotate_by, axis=0)
 
     return Vector(size=vector.size, vector=rolled, tags=vector.tags, vtype=vector.vtype, seed=vector.seed)
```

### Comparing `hdlib-0.1.3/hdlib/space.py` & `hdlib-0.1.4/hdlib/space.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Implementation of hyperdimensional Vector and Space
 """
 
+import errno
 import os
 import pickle
 import uuid
 
 import numpy as np
 from typing import List, Optional, Set, Tuple, Union
 
@@ -56,14 +57,20 @@
 
         except:
             raise TypeError("Vector name must be instance of a primitive")
 
         # Register random seed for reproducibility 
         self.seed = seed
 
+        # Take track of the hdlib version
+        self.version = __version__
+
+        if tags and not isinstance(tags, set):
+            raise TypeError("Tags must be a set")
+
         # Add tags
         self.tags = tags if tags else set()
 
         # Add links
         # Used to link Vectors by their names or IDs
         self.parents = set()
         self.children = set()
@@ -91,21 +98,25 @@
             elif ((self.vector == -1) | (self.vector == 1)).all():
                 self.vtype = "bipolar"
 
             else:
                 if warning:
                     print("Vector type can be binary or bipolar only")
 
-        elif from_file and os.path.isfile(from_file):
-            # Load vector from pickle file
-            with open(from_file, "rb") as pkl:
-                version, self.name, self.size, self.vector, self.vtype, self.parents, self.children, self.tags, self.seed = pickle.load(pkl)
+        elif from_file:
+            if not os.path.isfile(from_file):
+                raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), from_file)
 
-            if version != __version__:
-                print("Warning: the specified Space has been created with a different version of hdlib")
+            else:
+                # Load vector from pickle file
+                with open(from_file, "rb") as pkl:
+                    self.version, self.name, self.size, self.vector, self.vtype, self.parents, self.children, self.tags, self.seed = pickle.load(pkl)
+
+                if self.version != __version__:
+                    print("Warning: the specified Space has been created with a different version of hdlib")
 
         else:
             # Conditions on vector size
             # It must be an integer number greater than or equal to 10000
             # This size makes sure that vectors are quasi-orthogonal in space
             if not isinstance(size, int):
                 raise TypeError("Vector size must be an integer number")
@@ -144,14 +155,43 @@
         Get the vector size
 
         :return:    The length of vector
         """
 
         return self.size
 
+    def __str__(self) -> None:
+        """
+        Print the Vector object properties
+        """
+
+        return """
+            Class:   hdlib.space.Vector
+            Version: {}
+            Name:    {}
+            Seed:    {}
+            Size:    {}
+            Type:    {}
+            Tags:
+            
+            {}
+            
+            Vector:
+
+            {}
+        """.format(
+            self.version,
+            self.name,
+            self.seed,
+            self.size,
+            self.vtype,
+            np.array(list(self.tags)),
+            self.vector
+        )
+
     def dist(self, vector: "Vector", method: str="cosine") -> float:
         """
         Compute distance between vectors
 
         :param vector:      Vector object
         :param method:      Distance method: cosine, hamming, euclidean
         :return:            Distance
@@ -198,15 +238,15 @@
             # Dump the vector to a pickle file in the current working directory if not file path is provided
             to_file = os.path.join(os.getcwd, "{}.pkl".format(self.name))
 
         if os.path.isfile(to_file):
             raise Exception("The output file already exists!\n{}".format(to_file))
 
         with open(to_file, "wb") as pkl:
-            pickle.dump((__version__, self.name, self.size, self.vector, self.vtype, self.parents, self.children, self.tags, self.seed), pkl)
+            pickle.dump((self.version, self.name, self.size, self.vector, self.vtype, self.parents, self.children, self.tags, self.seed), pkl)
 
 
 class Space(object):
     """
     Vectors space
     """
 
@@ -218,14 +258,16 @@
         :param vtype:       Vector type: bipolar or binary
         :param from_file:   Load a space from pickle file
         :return:            A Space object
         """
 
         self.space = dict()
 
+        self.version = __version__
+
         self.size = size
 
         if self.size < 10000:
             raise ValueError("Size of vectors in space must be greater than or equal to 10000")
 
         self.vtype = vtype.lower()
 
@@ -234,38 +276,69 @@
 
         self.tags = dict()
 
         # Vector links can be used to define a tree structure
         # Use this flag to mark a vector as root
         self.root = None
 
-        if from_file and os.path.isfile(from_file):
-            with open(from_file, "rb") as pkl:
-                version, self.size, self.vtype, self.space, self.root = pickle.load(pkl)
-
-            if version != __version__:
-                print("Warning: the specified Space has been created with a different version of hdlib")
-
-            for name in self.space:
-                if self.space[name].tags:
-                    for tag in self.space[name].tags:
-                        if tag not in self.tags:
-                            self.tags[tag] = set()
+        if from_file:
+            if not os.path.isfile(from_file):
+                raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), from_file)
 
-                        self.tags[tag].add(name)
+            else:
+                with open(from_file, "rb") as pkl:
+                    self.version, self.size, self.vtype, self.space, self.root = pickle.load(pkl)
+
+                if self.version != __version__:
+                    print("Warning: the specified Space has been created with a different version of hdlib")
+
+                for name in self.space:
+                    if self.space[name].tags:
+                        for tag in self.space[name].tags:
+                            if tag not in self.tags:
+                                self.tags[tag] = set()
+
+                            self.tags[tag].add(name)
 
     def __len__(self) -> int:
         """
         Get the space size
 
         :return:    The number of vectors in the space
         """
 
         return len(self.space)
 
+    def __str__(self) -> None:
+        """
+        Print the Vector object properties
+        """
+
+        return """
+            Class:   hdlib.space.Space
+            Version: {}
+            Size:    {}
+            Type:    {}
+            Vectors: {}
+            Tags:
+            
+            {}
+            
+            IDs:
+
+            {}
+        """.format(
+            self.version,
+            self.size,
+            self.vtype,
+            len(self.space),
+            np.array(list(self.tags.keys())),
+            np.array(list(self.space.keys()))
+        )
+
     def memory(self) -> List[str]:
         """
         Return names or IDs of vectors in space
 
         :return:    Names or IDs of vectors in space
         """
 
@@ -331,15 +404,15 @@
 
         for tag in vector.tags:
             if tag not in self.tags:
                 self.tags[tag] = set()
 
             self.tags[tag].add(vector.name)
 
-    def bulkInsert(
+    def bulk_insert(
         self,
         names: List[str],
         tags: Optional[List[List[Union[str, int, float]]]]=None,
         ignoreExisting: bool=True
     ) -> None:
         """
         Add vectors to the space
@@ -579,8 +652,8 @@
             # Dump the space to a pickle file in the current working directory if not file path is provided
             to_file = os.path.join(os.getcwd, "space.pkl")
 
         if os.path.isfile(to_file):
             raise Exception("The output file already exists!\n{}".format(to_file))
 
         with open(to_file, "wb") as pkl:
-            pickle.dump((__version__, self.size, self.vtype, self.space, self.root), pkl)
+            pickle.dump((self.version, self.size, self.vtype, self.space, self.root), pkl)
```

### Comparing `hdlib-0.1.3/hdlib.egg-info/PKG-INFO` & `hdlib-0.1.4/hdlib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdlib
-Version: 0.1.3
+Version: 0.1.4
 Summary: Hyperdimensional Computing Library for building Vector Symbolic Architectures in Python
 Home-page: http://github.com/cumbof/hdlib
 Author: Fabio Cumbo
 Author-email: fabio.cumbo@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
@@ -108,28 +108,28 @@
 ```
 
 > **Note**
 > In this last example, similarly to Vector objects, a Space object is built by loading the content of a pickle file. Space objects can be saved to pickle files with the `dump()` method as in the following example: `space.dump(to_file="~/space.pkl")`
 
 Here is the list of Space class methods:
 
-| Method       | Signature                                       | Description  |
-|:-------------|:------------------------------------------------|:-------------|
-| `memory`     |                                                 | Return a list with Vector IDs |
-| `get`        | `names: list, tags: list`                       | Return a list of Vector objects based on a list of Vector IDs or tags |
-| `insert`     | `vector: Vector`                                | Insert a Vector object into the Space |
-| `bulkInsert` | `names: list, tags: list`                       | Automatically create a Vector object for each of the ID in the input `names` list and finally insert them into the Space. Also tag vectors based on tags in the `tags` list of lists. Tags in position `i` are assigned to the Vector object whose name is in position `i` of the `vectors` list |
-| `remove`     | `name: str`                                     | Remove a Vector object from the Space based on its ID |
-| `add_tag`    | `name: str, tag: str`                           | Assign a tag to a Vector object in the Space |
-| `remove_tag` | `name: str, tag: str`                           | Remove a tag to a Vector object in the Space |
-| `link`       | `name1: str, name2: str`                        | Link two vectors in the Space. Note that links are directed |
-| `set_root`   | `name: str`                                     | Vector links can be used to define a tree structure. Set a specific vector as root |
-| `find`       | `vector: Vector, threshold: float, method: str` | Given a specific Vector object, search for the closest Vector in the Space according to a specific distance metric: `cosine`, `hamming`, or `euclidean` |
-| `find_all`   | `vector: Vector, threshold: float, method: str` | Report the distance between the input Vector object and all the other Vectors in the Space |
-| `dump`       | `to_file: str`                                  | Dump the Space object to a pickle file |
+| Method        | Signature                                       | Description  |
+|:--------------|:------------------------------------------------|:-------------|
+| `memory`      |                                                 | Return a list with Vector IDs |
+| `get`         | `names: list, tags: list`                       | Return a list of Vector objects based on a list of Vector IDs or tags |
+| `insert`      | `vector: Vector`                                | Insert a Vector object into the Space |
+| `bulk_insert` | `names: list, tags: list`                       | Automatically create a Vector object for each of the ID in the input `names` list and finally insert them into the Space. Also tag vectors based on tags in the `tags` list of lists. Tags in position `i` are assigned to the Vector object whose name is in position `i` of the `vectors` list |
+| `remove`      | `name: str`                                     | Remove a Vector object from the Space based on its ID |
+| `add_tag`     | `name: str, tag: str`                           | Assign a tag to a Vector object in the Space |
+| `remove_tag`  | `name: str, tag: str`                           | Remove a tag to a Vector object in the Space |
+| `link`        | `name1: str, name2: str`                        | Link two vectors in the Space. Note that links are directed |
+| `set_root`    | `name: str`                                     | Vector links can be used to define a tree structure. Set a specific vector as root |
+| `find`        | `vector: Vector, threshold: float, method: str` | Given a specific Vector object, search for the closest Vector in the Space according to a specific distance metric: `cosine`, `hamming`, or `euclidean` |
+| `find_all`    | `vector: Vector, threshold: float, method: str` | Report the distance between the input Vector object and all the other Vectors in the Space |
+| `dump`        | `to_file: str`                                  | Dump the Space object to a pickle file |
 
 ### Arithmetic Operations
 
 A Vector Symbolic Architecture (a.k.a. Hyperdimensional Computing) is composed of vectors in the hyperdimensional space and a series of arithmetic operations to manipulate vectors.
 
 The `hdlib` library provides three operators under the `arithmetic` module: `bundle`, `bind`, and `permute`.
 
@@ -137,12 +137,21 @@
 
 | Operator       | Properties  |
 |:---------------|:------------|
 | `bundle`       | (i) The resulting vector is similar to the input vectors, (ii) the more vectors are involved in bundling, the harder it is to determine the component vectors, and (iii) if several copies of any vector are included in bundling, the resulting vector is closer to the dominant vector than to the other components |
 | `bind`         | (i) Invertible (unbind), (ii) it distributes over bundling, (iii) it preserves the distance, and (iv) the resulting vector is dissimilar to the input vectors |
 | `permute`      | (i) Invertible, (ii) it distributes over bundling and any elementwise operation, (iii) it preserves the distance, and (iv) the resulting vector is dissimilar to the input vectors |
 
+### Utilities
+
+The `hdlib` library also provides a set of utilities for dealing with input datasets collected under the `parser` module:
+
+| Method          | Signature                 | Description  |
+|:----------------|:--------------------------|:-------------|
+| `load_dataset`  | `filepath: str, sep: str` | Given a numerical matrix file, load the list of samples, features, classes, and the matrix with numerical data |
+| `split_dataset` | `points: int, folds: int` | Given a number of data points and the number of folds, split a dataset into different folds |
+
 ## Contributing
 
 Long-term discussion and bug reports are maintained via GitHub Issues, while code review is managed via GitHub Pull Requests.
 
 Please, (i) be sure that there are no existing issues/PR concerning the same bug or improvement before opening a new issue/PR; (ii) write a clear and concise description of what the bug/PR is about; (iii) specifying the list of steps to reproduce the behavior in addition to versions and other technical details is highly recommended.
```

### Comparing `hdlib-0.1.3/setup.py` & `hdlib-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `hdlib-0.1.3/test/test.py` & `hdlib-0.1.4/test/test.py`

 * *Files identical despite different names*

