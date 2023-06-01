# Comparing `tmp/jsfuzz-0.1.0.tar.gz` & `tmp/jsfuzz-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsfuzz-0.1.0.tar", max compression
+gzip compressed data, was "jsfuzz-0.1.1.tar", max compression
```

## Comparing `jsfuzz-0.1.0.tar` & `jsfuzz-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1066 2023-06-01 12:04:51.638267 jsfuzz-0.1.0/LICENSE
--rw-r--r--   0        0        0     1465 2023-06-01 12:04:51.638267 jsfuzz-0.1.0/README.md
--rw-r--r--   0        0        0     2039 2023-06-01 12:04:51.638267 jsfuzz-0.1.0/jsfuzz/inspector.py
--rw-r--r--   0        0        0      430 2023-06-01 12:04:51.642268 jsfuzz-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2004 1970-01-01 00:00:00.000000 jsfuzz-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-01 14:45:38.940480 jsfuzz-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1754 2023-06-01 14:45:38.940480 jsfuzz-0.1.1/README.md
+-rw-r--r--   0        0        0     2068 2023-06-01 14:45:38.940480 jsfuzz-0.1.1/jsfuzz/inspector.py
+-rw-r--r--   0        0        0      430 2023-06-01 14:45:38.940480 jsfuzz-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2293 1970-01-01 00:00:00.000000 jsfuzz-0.1.1/PKG-INFO
```

### Comparing `jsfuzz-0.1.0/LICENSE` & `jsfuzz-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jsfuzz-0.1.0/jsfuzz/inspector.py` & `jsfuzz-0.1.1/jsfuzz/inspector.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 def load(payload: str) -> object:
     return json.loads(payload)
 
 
 def similarity_score(node_path: str, node_value: str, value: str) -> float:
     parts = node_path.split(".")
     # iterate through all the node names along the path and calculate the best match
-    node_path_score = max([fuzz.ratio(part.lower(), value.lower()) for part in parts])
+    node_path_score = max([fuzz.partial_ratio(part.lower(), value.lower()) for part in parts])
 
-    node_value_score = fuzz.ratio(node_value.lower(), value.lower())
+    node_value_score = fuzz.partial_ratio(node_value.lower(), value.lower())
     return 0.7 * node_path_score + 0.3 * node_value_score
 
 
 def traverse(obj: object, path: str, candidates: list, value: str, top_k: int) -> list:
     if type(obj) == dict:
         for key in obj:
             candidates = traverse(obj[key], path=f"{path}.{key}", candidates=candidates, value=value, top_k=top_k)
@@ -36,24 +36,24 @@
             candidates[0] = (node_path, node_value, score)
 
         return sorted(candidates, key=lambda x: x[2])
     else:
         raise RuntimeError(f"Not supported Type: {type(obj)}")
 
 
-def search(payload: str, value: str) -> list:
+def search(payload: str, value: str, top_k=5) -> list:
     """
     fuzzy search for value inside a json payload
-    the top_k json nodes will be returned based on the similarity scores between this value and
+    the top_k json nodes (default to 5) will be returned based on the similarity scores between this value and
         - the path name to this node
         - the value contained in this node
     :param payload:
     :param value:
     :return:
     """
     candidates = []
-    max_candidates = 5
     obj = load(payload)
-    result = traverse(obj, path="$", candidates=candidates, value=value, top_k=max_candidates)
+    result = traverse(obj, path="$", candidates=candidates, value=value, top_k=top_k)
+    result.reverse()
     return result
```

### Comparing `jsfuzz-0.1.0/PKG-INFO` & `jsfuzz-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsfuzz
-Version: 0.1.0
+Version: 0.1.1
 Summary: Inspect json data and fuzzy search for values or key names
 License: MIT
 Author: Tung Dang
 Author-email: tung.dang@otto.de
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,14 +12,19 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: rapidfuzz (>=3.0.0,<4.0.0)
 Description-Content-Type: text/markdown
 
 # Fuzzy matching for JSON payload. Find json_path that matches best for your provided value
 
+## Install
+```bash
+$ pip install jsfuzz
+```
+
 ## Examples:
 
 
 ```json
 {
   "id": 11,
   "title": "perfume Oil",
@@ -39,16 +44,16 @@
   ]
 }
 ```
 
 ```python
 from jsfuzz import inspector
 
+# Default top_k=5 json paths will be returned
 result = inspector.search(payload, "brand")
-result.reverse()
 
 pprint(result)
 ====================
 
 Returns:
 
 [('$.brand', 'Impression of Acqua Di Gio', 75.80645161290323),
@@ -58,21 +63,25 @@
   'https://i.dummyjson.com/data/products/11/thumbnail.jpg',
   22.033898305084744),
  ('$.description', 'Mega Discount, Impression of A...', 20.657894736842106)]
 ```
 
 
 ```python
-result = inspector.search(payload, "65")
-result.reverse()
+result = inspector.search(payload, "65", top_k=10)
 
 pprint(result)
 ====================
 
 Returns:
 
 [('$.stock', '65', 30.0),
- ('$.rating', '4.26', 10.0),
+ ('$.rating', '4.26', 20.0),
+ ('$.thumbnail', 'https://i.dummyjson.com/data/products/11/thumbnail.jpg', 0.0),
+ ('$.category', 'fragrances', 0.0),
+ ('$.brand', 'Impression of Acqua Di Gio', 0.0),
  ('$.discountPercentage', '8.4', 0.0),
  ('$.price', '13', 0.0),
- ('$.description', 'Mega Discount, Impression of A...', 0.0)]
+ ('$.description', 'Mega Discount, Impression of A...', 0.0),
+ ('$.title', 'perfume Oil', 0.0),
+ ('$.id', '11', 0.0)]
 ```
```

