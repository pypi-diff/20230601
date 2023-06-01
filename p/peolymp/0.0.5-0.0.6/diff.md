# Comparing `tmp/peolymp-0.0.5.tar.gz` & `tmp/peolymp-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peolymp-0.0.5.tar", last modified: Thu Feb 16 14:53:18 2023, max compression
+gzip compressed data, was "peolymp-0.0.6.tar", last modified: Thu Jun  1 16:36:43 2023, max compression
```

## Comparing `peolymp-0.0.5.tar` & `peolymp-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 14:53:18.030734 peolymp-0.0.5/
--rw-r--r--   0 root         (0) root         (0)      138 2023-02-16 14:53:18.030734 peolymp-0.0.5/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 14:53:18.030734 peolymp-0.0.5/peolymp/
--rw-r--r--   0 root         (0) root         (0)      269 2023-02-16 14:53:17.000000 peolymp-0.0.5/peolymp/__init__.py
--rw-r--r--   0 root         (0) root         (0)      302 2023-02-16 14:53:17.000000 peolymp-0.0.5/peolymp/abstract.py
--rw-r--r--   0 root         (0) root         (0)     1683 2023-02-16 14:53:17.000000 peolymp-0.0.5/peolymp/atlas.py
--rw-r--r--   0 root         (0) root         (0)      492 2023-02-16 14:53:17.000000 peolymp-0.0.5/peolymp/client.py
--rw-r--r--   0 root         (0) root         (0)      869 2023-02-16 14:53:17.000000 peolymp-0.0.5/peolymp/cognito.py
--rw-r--r--   0 root         (0) root         (0)     4219 2023-02-16 14:53:17.000000 peolymp-0.0.5/peolymp/community.py
--rw-r--r--   0 root         (0) root         (0)     5173 2023-02-16 14:53:17.000000 peolymp-0.0.5/peolymp/judge.py
--rw-r--r--   0 root         (0) root         (0)     2600 2023-02-16 14:53:17.000000 peolymp-0.0.5/peolymp/judge_contest.py
--rw-r--r--   0 root         (0) root         (0)     4807 2023-02-16 14:53:17.000000 peolymp-0.0.5/peolymp/ranker.py
--rw-r--r--   0 root         (0) root         (0)     1369 2023-02-16 14:53:17.000000 peolymp-0.0.5/peolymp/typewriter.py
--rw-r--r--   0 root         (0) root         (0)      597 2023-02-16 14:53:17.000000 peolymp-0.0.5/peolymp/universe.py
--rw-r--r--   0 root         (0) root         (0)     2520 2023-02-16 14:53:17.000000 peolymp-0.0.5/peolymp/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 14:53:18.030734 peolymp-0.0.5/peolymp.egg-info/
--rw-r--r--   0 root         (0) root         (0)      138 2023-02-16 14:53:17.000000 peolymp-0.0.5/peolymp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      396 2023-02-16 14:53:17.000000 peolymp-0.0.5/peolymp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-16 14:53:17.000000 peolymp-0.0.5/peolymp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-02-16 14:53:17.000000 peolymp-0.0.5/peolymp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-02-16 14:53:17.000000 peolymp-0.0.5/peolymp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-16 14:53:18.030734 peolymp-0.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      346 2023-02-16 14:53:17.000000 peolymp-0.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:36:43.114107 peolymp-0.0.6/
+-rw-r--r--   0 root         (0) root         (0)      138 2023-06-01 16:36:43.114107 peolymp-0.0.6/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:36:43.114107 peolymp-0.0.6/peolymp/
+-rw-r--r--   0 root         (0) root         (0)      269 2023-06-01 16:36:42.000000 peolymp-0.0.6/peolymp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      302 2023-06-01 16:36:42.000000 peolymp-0.0.6/peolymp/abstract.py
+-rw-r--r--   0 root         (0) root         (0)     1845 2023-06-01 16:36:42.000000 peolymp-0.0.6/peolymp/atlas.py
+-rw-r--r--   0 root         (0) root         (0)      492 2023-06-01 16:36:42.000000 peolymp-0.0.6/peolymp/client.py
+-rw-r--r--   0 root         (0) root         (0)      869 2023-06-01 16:36:42.000000 peolymp-0.0.6/peolymp/cognito.py
+-rw-r--r--   0 root         (0) root         (0)     4219 2023-06-01 16:36:42.000000 peolymp-0.0.6/peolymp/community.py
+-rw-r--r--   0 root         (0) root         (0)     5173 2023-06-01 16:36:42.000000 peolymp-0.0.6/peolymp/judge.py
+-rw-r--r--   0 root         (0) root         (0)     2600 2023-06-01 16:36:42.000000 peolymp-0.0.6/peolymp/judge_contest.py
+-rw-r--r--   0 root         (0) root         (0)     4807 2023-06-01 16:36:42.000000 peolymp-0.0.6/peolymp/ranker.py
+-rw-r--r--   0 root         (0) root         (0)     1369 2023-06-01 16:36:42.000000 peolymp-0.0.6/peolymp/typewriter.py
+-rw-r--r--   0 root         (0) root         (0)      597 2023-06-01 16:36:42.000000 peolymp-0.0.6/peolymp/universe.py
+-rw-r--r--   0 root         (0) root         (0)     2520 2023-06-01 16:36:42.000000 peolymp-0.0.6/peolymp/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:36:43.114107 peolymp-0.0.6/peolymp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      138 2023-06-01 16:36:43.000000 peolymp-0.0.6/peolymp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      396 2023-06-01 16:36:43.000000 peolymp-0.0.6/peolymp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 16:36:43.000000 peolymp-0.0.6/peolymp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-06-01 16:36:43.000000 peolymp-0.0.6/peolymp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-01 16:36:43.000000 peolymp-0.0.6/peolymp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-01 16:36:43.114107 peolymp-0.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      346 2023-06-01 16:36:42.000000 peolymp-0.0.6/setup.py
```

### Comparing `peolymp-0.0.5/peolymp/atlas.py` & `peolymp-0.0.6/peolymp/atlas.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from eolymp.atlas import statement_pb2, atlas_pb2
+from eolymp.atlas import statement_pb2, library_service_pb2
 from eolymp.atlas.atlas_http import AtlasClient
 
 from peolymp.abstract import AbstractAPI
 from peolymp.utils import get_many
 
 
 class AtlasAPI(AbstractAPI):
@@ -10,27 +10,31 @@
     def __init__(self, **kwargs):
         super(AtlasAPI, self).__init__(**kwargs)
         self.client = AtlasClient(self.http_client, url=self.get_url())
 
     def create_statement(self, prob_id, locale, title, link, source=""):
         s = statement_pb2.Statement(problem_id=prob_id, locale=locale, title=title, content="", download_link=link,
                                     format=statement_pb2.Statement.Format.TEX, source=source)
-        return self.client.CreateStatement(atlas_pb2.CreateStatementInput(problem_id=prob_id, statement=s)).statement_id
+        return self.client.CreateStatement(
+            library_service_pb2.CreateStatementInput(problem_id=prob_id, statement=s)).statement_id
 
     def update_statement(self, problem_id, statement):
         return self.client.UpdateStatement(
-            atlas_pb2.UpdateStatementInput(problem_id=problem_id, statement_id=statement.id, statement=statement))
+            library_service_pb2.UpdateStatementInput(problem_id=problem_id, statement_id=statement.id,
+                                                     statement=statement))
 
     def delete_statement(self, prob_id, statement_id):
-        self.client.DeleteStatement(atlas_pb2.DeleteStatementInput(statement_id=statement_id, problem_id=prob_id))
+        self.client.DeleteStatement(
+            library_service_pb2.DeleteStatementInput(statement_id=statement_id, problem_id=prob_id))
 
     def get_statements(self, prob_id):
-        return self.client.ListStatements(atlas_pb2.ListStatementsInput(problem_id=prob_id)).items
+        return self.client.ListStatements(library_service_pb2.ListStatementsInput(problem_id=prob_id)).items
 
     def get_problems(self):
         def __get_problems(offset, size):
-            return self.client.ListProblems(request=atlas_pb2.ListProblemsInput(offset=offset, size=size))
+            return self.client.ListProblems(request=library_service_pb2.ListProblemsInput(offset=offset, size=size))
 
         return get_many(__get_problems)
 
     def delete_testset(self, problem_id, testset_id):
-        return self.client.DeleteTestset(atlas_pb2.DeleteTestsetInput(problem_id=problem_id, testset_id=testset_id))
+        return self.client.DeleteTestset(
+            library_service_pb2.DeleteTestsetInput(problem_id=problem_id, testset_id=testset_id))
```

### Comparing `peolymp-0.0.5/peolymp/cognito.py` & `peolymp-0.0.6/peolymp/cognito.py`

 * *Files identical despite different names*

### Comparing `peolymp-0.0.5/peolymp/community.py` & `peolymp-0.0.6/peolymp/community.py`

 * *Files identical despite different names*

### Comparing `peolymp-0.0.5/peolymp/judge.py` & `peolymp-0.0.6/peolymp/judge.py`

 * *Files identical despite different names*

### Comparing `peolymp-0.0.5/peolymp/judge_contest.py` & `peolymp-0.0.6/peolymp/judge_contest.py`

 * *Files identical despite different names*

### Comparing `peolymp-0.0.5/peolymp/ranker.py` & `peolymp-0.0.6/peolymp/ranker.py`

 * *Files identical despite different names*

### Comparing `peolymp-0.0.5/peolymp/typewriter.py` & `peolymp-0.0.6/peolymp/typewriter.py`

 * *Files identical despite different names*

### Comparing `peolymp-0.0.5/peolymp/universe.py` & `peolymp-0.0.6/peolymp/universe.py`

 * *Files identical despite different names*

### Comparing `peolymp-0.0.5/peolymp/utils.py` & `peolymp-0.0.6/peolymp/utils.py`

 * *Files identical despite different names*

