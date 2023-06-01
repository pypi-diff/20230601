# Comparing `tmp/vecs-0.2.4.tar.gz` & `tmp/vecs-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vecs-0.2.4.tar", last modified: Fri May 19 18:41:22 2023, max compression
+gzip compressed data, was "vecs-0.2.6.tar", last modified: Thu Jun  1 18:47:16 2023, max compression
```

## Comparing `vecs-0.2.4.tar` & `vecs-0.2.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-05-19 18:41:22.924553 vecs-0.2.4/
--rw-r--r--   0 oliverrice   (501) staff       (20)      743 2023-05-19 18:41:22.924449 vecs-0.2.4/PKG-INFO
--rw-r--r--   0 oliverrice   (501) staff       (20)     2349 2023-05-19 14:53:34.000000 vecs-0.2.4/README.md
--rw-r--r--   0 oliverrice   (501) staff       (20)      154 2023-05-12 13:47:40.000000 vecs-0.2.4/pyproject.toml
--rw-r--r--   0 oliverrice   (501) staff       (20)       38 2023-05-19 18:41:22.924592 vecs-0.2.4/setup.cfg
--rw-r--r--   0 oliverrice   (501) staff       (20)     2222 2023-05-19 14:54:31.000000 vecs-0.2.4/setup.py
-drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-05-19 18:41:22.922859 vecs-0.2.4/src/
-drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-05-19 18:41:22.923756 vecs-0.2.4/src/vecs/
--rw-r--r--   0 oliverrice   (501) staff       (20)      390 2023-05-19 18:40:57.000000 vecs-0.2.4/src/vecs/__init__.py
--rw-r--r--   0 oliverrice   (501) staff       (20)     1686 2023-05-16 19:39:23.000000 vecs-0.2.4/src/vecs/client.py
--rw-r--r--   0 oliverrice   (501) staff       (20)    13532 2023-05-19 18:19:01.000000 vecs-0.2.4/src/vecs/collection.py
--rw-r--r--   0 oliverrice   (501) staff       (20)      491 2023-05-16 18:21:37.000000 vecs-0.2.4/src/vecs/exc.py
-drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-05-19 18:41:22.924297 vecs-0.2.4/src/vecs.egg-info/
--rw-r--r--   0 oliverrice   (501) staff       (20)      743 2023-05-19 18:41:22.000000 vecs-0.2.4/src/vecs.egg-info/PKG-INFO
--rw-r--r--   0 oliverrice   (501) staff       (20)      271 2023-05-19 18:41:22.000000 vecs-0.2.4/src/vecs.egg-info/SOURCES.txt
--rw-r--r--   0 oliverrice   (501) staff       (20)        1 2023-05-19 18:41:22.000000 vecs-0.2.4/src/vecs.egg-info/dependency_links.txt
--rw-r--r--   0 oliverrice   (501) staff       (20)      157 2023-05-19 18:41:22.000000 vecs-0.2.4/src/vecs.egg-info/requires.txt
--rw-r--r--   0 oliverrice   (501) staff       (20)        5 2023-05-19 18:41:22.000000 vecs-0.2.4/src/vecs.egg-info/top_level.txt
+drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-06-01 18:47:16.811108 vecs-0.2.6/
+-rw-r--r--   0 oliverrice   (501) staff       (20)      743 2023-06-01 18:47:16.811000 vecs-0.2.6/PKG-INFO
+-rw-r--r--   0 oliverrice   (501) staff       (20)     2349 2023-05-19 14:53:34.000000 vecs-0.2.6/README.md
+-rw-r--r--   0 oliverrice   (501) staff       (20)      154 2023-05-12 13:47:40.000000 vecs-0.2.6/pyproject.toml
+-rw-r--r--   0 oliverrice   (501) staff       (20)       38 2023-06-01 18:47:16.811154 vecs-0.2.6/setup.cfg
+-rw-r--r--   0 oliverrice   (501) staff       (20)     2222 2023-05-19 14:54:31.000000 vecs-0.2.6/setup.py
+drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-06-01 18:47:16.809141 vecs-0.2.6/src/
+drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-06-01 18:47:16.810318 vecs-0.2.6/src/vecs/
+-rw-r--r--   0 oliverrice   (501) staff       (20)      390 2023-06-01 18:46:56.000000 vecs-0.2.6/src/vecs/__init__.py
+-rw-r--r--   0 oliverrice   (501) staff       (20)     1917 2023-06-01 18:46:56.000000 vecs-0.2.6/src/vecs/client.py
+-rw-r--r--   0 oliverrice   (501) staff       (20)    13736 2023-05-24 17:16:29.000000 vecs-0.2.6/src/vecs/collection.py
+-rw-r--r--   0 oliverrice   (501) staff       (20)      491 2023-05-16 18:21:37.000000 vecs-0.2.6/src/vecs/exc.py
+drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-06-01 18:47:16.810849 vecs-0.2.6/src/vecs.egg-info/
+-rw-r--r--   0 oliverrice   (501) staff       (20)      743 2023-06-01 18:47:16.000000 vecs-0.2.6/src/vecs.egg-info/PKG-INFO
+-rw-r--r--   0 oliverrice   (501) staff       (20)      271 2023-06-01 18:47:16.000000 vecs-0.2.6/src/vecs.egg-info/SOURCES.txt
+-rw-r--r--   0 oliverrice   (501) staff       (20)        1 2023-06-01 18:47:16.000000 vecs-0.2.6/src/vecs.egg-info/dependency_links.txt
+-rw-r--r--   0 oliverrice   (501) staff       (20)      157 2023-06-01 18:47:16.000000 vecs-0.2.6/src/vecs.egg-info/requires.txt
+-rw-r--r--   0 oliverrice   (501) staff       (20)        5 2023-06-01 18:47:16.000000 vecs-0.2.6/src/vecs.egg-info/top_level.txt
```

### Comparing `vecs-0.2.4/PKG-INFO` & `vecs-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vecs
-Version: 0.2.4
+Version: 0.2.6
 Summary: pgvector client
 Home-page: https://github.com/supabase/vecs
 Author: Oliver Rice
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
```

### Comparing `vecs-0.2.4/README.md` & `vecs-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `vecs-0.2.4/setup.py` & `vecs-0.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `vecs-0.2.4/src/vecs/client.py` & `vecs-0.2.6/src/vecs/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -46,7 +46,18 @@
 
     def delete_collection(self, name: str) -> None:
         """List all collections"""
         from vecs.collection import Collection
 
         Collection(name, -1, self)._drop()
         return
+
+    def disconnect(self) -> None:
+        self.engine.dispose()
+        return
+
+    def __enter__(self) -> "Client":
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self.disconnect()
+        return
```

### Comparing `vecs-0.2.4/src/vecs/collection.py` & `vecs-0.2.6/src/vecs/collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,22 +96,28 @@
         existing_collection_names = [x.name for x in existing_collections]
         if self.name not in existing_collection_names:
             raise CollectionNotFound("Collection with requested name not found")
         self.table.drop(self.client.engine)
         return self
 
     def upsert(self, vectors: Iterable[Tuple[str, Iterable[Numeric], Metadata]]):
-        stmt = postgresql.insert(self.table).values(vectors)
-        stmt = stmt.on_conflict_do_update(
-            index_elements=[self.table.c.id],
-            set_=dict(vec=stmt.excluded.vec, metadata=stmt.excluded.metadata),
-        )
+
+        chunk_size = 500
+
         with self.client.Session() as sess:
             with sess.begin():
-                sess.execute(stmt)
+                for chunk in flu(vectors).chunk(chunk_size):
+                    stmt = postgresql.insert(self.table).values(chunk)
+                    stmt = stmt.on_conflict_do_update(
+                        index_elements=[self.table.c.id],
+                        set_=dict(
+                            vec=stmt.excluded.vec, metadata=stmt.excluded.metadata
+                        ),
+                    )
+                    sess.execute(stmt)
         return
 
     def fetch(self, ids: Iterable[str]) -> List[Record]:
         if isinstance(ids, str):
             raise ArgError("ids must be a list of strings")
 
         chunk_size = 12
```

### Comparing `vecs-0.2.4/src/vecs.egg-info/PKG-INFO` & `vecs-0.2.6/src/vecs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vecs
-Version: 0.2.4
+Version: 0.2.6
 Summary: pgvector client
 Home-page: https://github.com/supabase/vecs
 Author: Oliver Rice
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
```

