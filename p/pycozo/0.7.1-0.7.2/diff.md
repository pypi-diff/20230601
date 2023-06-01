# Comparing `tmp/pycozo-0.7.1.tar.gz` & `tmp/pycozo-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycozo-0.7.1.tar", last modified: Wed May 10 07:48:33 2023, max compression
+gzip compressed data, was "pycozo-0.7.2.tar", last modified: Thu Jun  1 03:11:18 2023, max compression
```

## Comparing `pycozo-0.7.1.tar` & `pycozo-0.7.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 zh217      (501) staff       (20)        0 2023-05-10 07:48:33.908328 pycozo-0.7.1/
--rw-r--r--   0 zh217      (501) staff       (20)    16724 2022-11-30 04:19:19.000000 pycozo-0.7.1/LICENSE.txt
--rw-r--r--   0 zh217      (501) staff       (20)      469 2023-05-10 07:48:33.908214 pycozo-0.7.1/PKG-INFO
--rw-r--r--   0 zh217      (501) staff       (20)     8781 2023-05-08 07:24:36.000000 pycozo-0.7.1/README.md
-drwxr-xr-x   0 zh217      (501) staff       (20)        0 2023-05-10 07:48:33.907387 pycozo-0.7.1/pycozo/
--rw-r--r--   0 zh217      (501) staff       (20)      284 2022-11-30 04:32:35.000000 pycozo-0.7.1/pycozo/__init__.py
--rw-r--r--   0 zh217      (501) staff       (20)     6676 2023-05-08 10:26:40.000000 pycozo-0.7.1/pycozo/builder.py
--rw-r--r--   0 zh217      (501) staff       (20)    13343 2023-05-08 07:55:16.000000 pycozo-0.7.1/pycozo/client.py
--rw-r--r--   0 zh217      (501) staff       (20)     4619 2022-12-28 04:03:29.000000 pycozo-0.7.1/pycozo/ext_impl.py
--rw-r--r--   0 zh217      (501) staff       (20)      378 2022-11-30 04:32:35.000000 pycozo-0.7.1/pycozo/ipyext.py
--rw-r--r--   0 zh217      (501) staff       (20)      677 2022-11-30 04:32:35.000000 pycozo-0.7.1/pycozo/ipyext_direct.py
--rw-r--r--   0 zh217      (501) staff       (20)     2363 2023-05-08 05:14:33.000000 pycozo-0.7.1/pycozo/test_builder.py
--rw-r--r--   0 zh217      (501) staff       (20)     2046 2023-01-21 11:49:23.000000 pycozo-0.7.1/pycozo/test_client.py
-drwxr-xr-x   0 zh217      (501) staff       (20)        0 2023-05-10 07:48:33.908049 pycozo-0.7.1/pycozo.egg-info/
--rw-r--r--   0 zh217      (501) staff       (20)      469 2023-05-10 07:48:33.000000 pycozo-0.7.1/pycozo.egg-info/PKG-INFO
--rw-r--r--   0 zh217      (501) staff       (20)      338 2023-05-10 07:48:33.000000 pycozo-0.7.1/pycozo.egg-info/SOURCES.txt
--rw-r--r--   0 zh217      (501) staff       (20)        1 2023-05-10 07:48:33.000000 pycozo-0.7.1/pycozo.egg-info/dependency_links.txt
--rw-r--r--   0 zh217      (501) staff       (20)       77 2023-05-10 07:48:33.000000 pycozo-0.7.1/pycozo.egg-info/requires.txt
--rw-r--r--   0 zh217      (501) staff       (20)        7 2023-05-10 07:48:33.000000 pycozo-0.7.1/pycozo.egg-info/top_level.txt
--rw-r--r--   0 zh217      (501) staff       (20)       38 2023-05-10 07:48:33.908367 pycozo-0.7.1/setup.cfg
--rw-r--r--   0 zh217      (501) staff       (20)      920 2023-05-10 07:14:53.000000 pycozo-0.7.1/setup.py
+drwxr-xr-x   0 zh217      (501) staff       (20)        0 2023-06-01 03:11:18.731153 pycozo-0.7.2/
+-rw-r--r--   0 zh217      (501) staff       (20)    16724 2022-11-30 04:19:19.000000 pycozo-0.7.2/LICENSE.txt
+-rw-r--r--   0 zh217      (501) staff       (20)      469 2023-06-01 03:11:18.731026 pycozo-0.7.2/PKG-INFO
+-rw-r--r--   0 zh217      (501) staff       (20)     8781 2023-06-01 02:09:09.000000 pycozo-0.7.2/README.md
+drwxr-xr-x   0 zh217      (501) staff       (20)        0 2023-06-01 03:11:18.730123 pycozo-0.7.2/pycozo/
+-rw-r--r--   0 zh217      (501) staff       (20)      284 2022-11-30 04:32:35.000000 pycozo-0.7.2/pycozo/__init__.py
+-rw-r--r--   0 zh217      (501) staff       (20)     6788 2023-06-01 02:09:09.000000 pycozo-0.7.2/pycozo/builder.py
+-rw-r--r--   0 zh217      (501) staff       (20)    13645 2023-06-01 02:09:09.000000 pycozo-0.7.2/pycozo/client.py
+-rw-r--r--   0 zh217      (501) staff       (20)     4619 2022-12-28 04:03:29.000000 pycozo-0.7.2/pycozo/ext_impl.py
+-rw-r--r--   0 zh217      (501) staff       (20)      378 2022-11-30 04:32:35.000000 pycozo-0.7.2/pycozo/ipyext.py
+-rw-r--r--   0 zh217      (501) staff       (20)      677 2022-11-30 04:32:35.000000 pycozo-0.7.2/pycozo/ipyext_direct.py
+-rw-r--r--   0 zh217      (501) staff       (20)     2363 2023-06-01 02:09:09.000000 pycozo-0.7.2/pycozo/test_builder.py
+-rw-r--r--   0 zh217      (501) staff       (20)     2046 2023-01-21 11:49:23.000000 pycozo-0.7.2/pycozo/test_client.py
+drwxr-xr-x   0 zh217      (501) staff       (20)        0 2023-06-01 03:11:18.730828 pycozo-0.7.2/pycozo.egg-info/
+-rw-r--r--   0 zh217      (501) staff       (20)      469 2023-06-01 03:11:18.000000 pycozo-0.7.2/pycozo.egg-info/PKG-INFO
+-rw-r--r--   0 zh217      (501) staff       (20)      338 2023-06-01 03:11:18.000000 pycozo-0.7.2/pycozo.egg-info/SOURCES.txt
+-rw-r--r--   0 zh217      (501) staff       (20)        1 2023-06-01 03:11:18.000000 pycozo-0.7.2/pycozo.egg-info/dependency_links.txt
+-rw-r--r--   0 zh217      (501) staff       (20)       77 2023-06-01 03:11:18.000000 pycozo-0.7.2/pycozo.egg-info/requires.txt
+-rw-r--r--   0 zh217      (501) staff       (20)        7 2023-06-01 03:11:18.000000 pycozo-0.7.2/pycozo.egg-info/top_level.txt
+-rw-r--r--   0 zh217      (501) staff       (20)       38 2023-06-01 03:11:18.731193 pycozo-0.7.2/setup.cfg
+-rw-r--r--   0 zh217      (501) staff       (20)      920 2023-06-01 02:09:09.000000 pycozo-0.7.2/setup.py
```

### Comparing `pycozo-0.7.1/LICENSE.txt` & `pycozo-0.7.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pycozo-0.7.1/README.md` & `pycozo-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `pycozo-0.7.1/pycozo/builder.py` & `pycozo-0.7.2/pycozo/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,15 +233,23 @@
 class Cond:
     clauses: list[(Expr, Expr)]
 
     def __str__(self):
         return 'cond ' + ', '.join(f'{k}, {v}, ' for k, v in self.clauses)
 
 
-Atom: TypeAlias = Expr | Cond | Bind | RuleApply | StoredRuleApply | StoredRuleNamedApply | Conjunction | Disjunction | Negation
+@dataclass
+class RawAtom:
+    script: str
+
+    def __str__(self):
+        return f'({self.script})'
+
+
+Atom: TypeAlias = Expr | Cond | Bind | RuleApply | StoredRuleApply | StoredRuleNamedApply | Conjunction | Disjunction | Negation | RawAtom
 
 
 @dataclass
 class FixedRule:
     head: RuleHead
     rule_name: str
     inputs: list[RuleApply | StoredRuleApply | StoredRuleNamedApply] = field(default_factory=list)
```

### Comparing `pycozo-0.7.1/pycozo/client.py` & `pycozo-0.7.2/pycozo/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,54 +66,55 @@
             self.embedded.close()
 
     def _headers(self):
         return {
             'x-cozo-auth': self.auth
         }
 
-    def _client_request(self, script, params=None):
+    def _client_request(self, script, params=None, immutable=False):
         import requests
 
         r = requests.post(f'{self.host}/text-query', headers=self._headers(), json={
             'script': script,
-            'params': params or {}
+            'params': params or {},
+            'immutable': immutable
         })
         res = r.json()
         return self._format_return(res)
 
     def _format_return(self, res):
         if not res['ok']:
             raise QueryException(res)
 
         if self.pandas:
             return self.pandas.DataFrame(columns=res['headers'], data=res['rows'])
         else:
             return res
 
-    def _embedded_request(self, script, params=None):
+    def _embedded_request(self, script, params=None, immutable=False):
         try:
-            res = self.embedded.run_script(script, params or {})
+            res = self.embedded.run_script(script, params or {}, immutable)
         except Exception as e:
             raise QueryException(e.args[0]) from None
         if self.pandas:
             return self.pandas.DataFrame(columns=res['headers'], data=res['rows'])
         else:
             return res
 
-    def run(self, script, params=None):
+    def run(self, script, params=None, immutable=False):
         """Run a given CozoScript query.
 
         :param script: the query in CozoScript
         :param params: the named parameters for the query. If specified, must be a dict with string keys.
         :return: the query result as a dict, or a pandas dataframe if the `dataframe` option was true.
         """
         if self.embedded is None:
-            return self._client_request(script, params)
+            return self._client_request(script, params, immutable)
         else:
-            return self._embedded_request(script, params)
+            return self._embedded_request(script, params, immutable)
 
     def export_relations(self, relations):
         """Export the specified relations.
 
         :param relations: names of the relations in a list.
         :return: a dict with string keys for the names of relations, and values containing all the rows.
         """
@@ -159,15 +160,15 @@
         :param path: the path to write the backup into. For a remote database, this is a path on the remote machine.
         """
         if self.embedded:
             self.embedded.backup(path)
         else:
             import requests
 
-            r = requests.post(f'{self.host}/backup/', headers=self._headers(), json={'path': path})
+            r = requests.post(f'{self.host}/backup', headers=self._headers(), json={'path': path})
             res = r.json()
             if not res['ok']:
                 raise RuntimeError(res['message'])
 
     def register_callback(self, relation, callback):
         if self.embedded:
             return self.embedded.register_callback(relation, callback)
@@ -308,14 +309,17 @@
                 raise RuntimeError('Invalid data type for mutation')
 
     def _mutate(self, relation, data, op):
         cols_str, processed_data = self._process_mutate_data(data)
         q = f'?[{cols_str}] <- $data :{op} {relation} {{ {cols_str} }}'
         return self.run(q, {'data': processed_data})
 
+    def insert(self, relation, data):
+        return self._mutate(relation, data, 'insert')
+
     def put(self, relation, data):
         return self._mutate(relation, data, 'put')
 
     def update(self, relation, data):
         return self._mutate(relation, data, 'update')
 
     def rm(self, relation, data):
@@ -341,15 +345,18 @@
     """
 
     def __init__(self, resp):
         super().__init__()
         self.resp = resp
 
     def __repr__(self):
-        return self.resp.get('display') or self.resp.get('message') or str(self.resp)
+        if hasattr(self.resp, 'get'):
+            return self.resp.get('display') or self.resp.get('message') or str(self.resp)
+        else:
+            return str(self.resp)
 
     def __str__(self):
         return self.resp.get('message') or str(self.resp)
 
     def _repr_pretty_(self, p, cycle):
         p.text(repr(self))
```

### Comparing `pycozo-0.7.1/pycozo/ext_impl.py` & `pycozo-0.7.2/pycozo/ext_impl.py`

 * *Files identical despite different names*

### Comparing `pycozo-0.7.1/pycozo/ipyext_direct.py` & `pycozo-0.7.2/pycozo/ipyext_direct.py`

 * *Files identical despite different names*

### Comparing `pycozo-0.7.1/pycozo/test_builder.py` & `pycozo-0.7.2/pycozo/test_builder.py`

 * *Files identical despite different names*

### Comparing `pycozo-0.7.1/pycozo/test_client.py` & `pycozo-0.7.2/pycozo/test_client.py`

 * *Files identical despite different names*

### Comparing `pycozo-0.7.1/setup.py` & `pycozo-0.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.
 #  If a copy of the MPL was not distributed with this file,
 #  You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from setuptools import setup
 
-VERSION = '0.7.1'
+VERSION = '0.7.2'
 
 setup(
     name='pycozo',
     version=VERSION,
     packages=['pycozo'],
     url='',
     license='MPL-2.0',
```

