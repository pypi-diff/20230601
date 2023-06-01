# Comparing `tmp/karuoflow-1.3.tar.gz` & `tmp/karuoflow-1.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "karuoflow-1.3.tar", last modified: Fri May 12 05:52:56 2023, max compression
+gzip compressed data, was "karuoflow-1.31.tar", last modified: Thu Jun  1 00:38:56 2023, max compression
```

## Comparing `karuoflow-1.3.tar` & `karuoflow-1.31.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 work      (1001) work      (1001)        0 2023-05-12 05:52:56.280072 karuoflow-1.3/
--rw-rw-r--   0 work      (1001) work      (1001)     1063 2023-05-12 05:20:22.000000 karuoflow-1.3/LICENSE
--rw-rw-r--   0 work      (1001) work      (1001)      286 2023-05-12 05:52:56.280072 karuoflow-1.3/PKG-INFO
--rw-rw-r--   0 work      (1001) work      (1001)       38 2023-05-12 05:20:22.000000 karuoflow-1.3/README.md
-drwxrwxr-x   0 work      (1001) work      (1001)        0 2023-05-12 05:52:56.278072 karuoflow-1.3/karuoflow/
--rw-rw-r--   0 work      (1001) work      (1001)     2169 2023-05-12 05:34:37.000000 karuoflow-1.3/karuoflow/__init__.py
--rw-rw-r--   0 work      (1001) work      (1001)     2558 2023-05-12 05:20:22.000000 karuoflow-1.3/karuoflow/datadef.py
-drwxrwxr-x   0 work      (1001) work      (1001)        0 2023-05-12 05:52:56.279072 karuoflow-1.3/karuoflow/db/
--rw-rw-r--   0 work      (1001) work      (1001)      151 2023-05-12 05:20:22.000000 karuoflow-1.3/karuoflow/db/__init__.py
--rw-rw-r--   0 work      (1001) work      (1001)      764 2023-05-12 05:20:22.000000 karuoflow-1.3/karuoflow/db/session.py
--rw-rw-r--   0 work      (1001) work      (1001)     7251 2023-05-12 05:20:22.000000 karuoflow-1.3/karuoflow/db/tables.py
--rw-rw-r--   0 work      (1001) work      (1001)     2510 2023-05-12 05:20:22.000000 karuoflow-1.3/karuoflow/error_code.py
--rw-rw-r--   0 work      (1001) work      (1001)    30609 2023-05-12 05:33:33.000000 karuoflow-1.3/karuoflow/flowapp.py
--rw-rw-r--   0 work      (1001) work      (1001)    19421 2023-05-12 05:20:22.000000 karuoflow-1.3/karuoflow/flowmodelagent.py
--rw-rw-r--   0 work      (1001) work      (1001)     6854 2023-05-12 05:20:22.000000 karuoflow-1.3/karuoflow/initflow.py
-drwxrwxr-x   0 work      (1001) work      (1001)        0 2023-05-12 05:52:56.280072 karuoflow-1.3/karuoflow/test/
--rw-rw-r--   0 work      (1001) work      (1001)        0 2023-05-12 05:20:22.000000 karuoflow-1.3/karuoflow/test/__init__.py
--rw-rw-r--   0 work      (1001) work      (1001)    11800 2023-05-12 05:49:21.000000 karuoflow-1.3/karuoflow/test/test_initenvironment.py
-drwxrwxr-x   0 work      (1001) work      (1001)        0 2023-05-12 05:52:56.279072 karuoflow-1.3/karuoflow.egg-info/
--rw-rw-r--   0 work      (1001) work      (1001)      286 2023-05-12 05:52:55.000000 karuoflow-1.3/karuoflow.egg-info/PKG-INFO
--rw-rw-r--   0 work      (1001) work      (1001)      466 2023-05-12 05:52:55.000000 karuoflow-1.3/karuoflow.egg-info/SOURCES.txt
--rw-rw-r--   0 work      (1001) work      (1001)        1 2023-05-12 05:52:55.000000 karuoflow-1.3/karuoflow.egg-info/dependency_links.txt
--rw-rw-r--   0 work      (1001) work      (1001)       26 2023-05-12 05:52:55.000000 karuoflow-1.3/karuoflow.egg-info/requires.txt
--rw-rw-r--   0 work      (1001) work      (1001)       10 2023-05-12 05:52:55.000000 karuoflow-1.3/karuoflow.egg-info/top_level.txt
--rw-rw-r--   0 work      (1001) work      (1001)       38 2023-05-12 05:52:56.280072 karuoflow-1.3/setup.cfg
--rw-rw-r--   0 work      (1001) work      (1001)      685 2023-05-12 05:20:22.000000 karuoflow-1.3/setup.py
+drwxrwxr-x   0 work      (1001) work      (1001)        0 2023-06-01 00:38:56.248937 karuoflow-1.31/
+-rw-rw-r--   0 work      (1001) work      (1001)     1063 2023-05-12 05:20:22.000000 karuoflow-1.31/LICENSE
+-rw-rw-r--   0 work      (1001) work      (1001)      287 2023-06-01 00:38:56.247937 karuoflow-1.31/PKG-INFO
+-rw-rw-r--   0 work      (1001) work      (1001)       38 2023-05-12 05:20:22.000000 karuoflow-1.31/README.md
+drwxrwxr-x   0 work      (1001) work      (1001)        0 2023-06-01 00:38:56.246937 karuoflow-1.31/karuoflow/
+-rw-rw-r--   0 work      (1001) work      (1001)     2269 2023-06-01 00:29:09.000000 karuoflow-1.31/karuoflow/__init__.py
+-rw-rw-r--   0 work      (1001) work      (1001)     2558 2023-05-12 05:20:22.000000 karuoflow-1.31/karuoflow/datadef.py
+drwxrwxr-x   0 work      (1001) work      (1001)        0 2023-06-01 00:38:56.247937 karuoflow-1.31/karuoflow/db/
+-rw-rw-r--   0 work      (1001) work      (1001)      151 2023-05-12 05:20:22.000000 karuoflow-1.31/karuoflow/db/__init__.py
+-rw-rw-r--   0 work      (1001) work      (1001)      764 2023-05-12 05:20:22.000000 karuoflow-1.31/karuoflow/db/session.py
+-rw-rw-r--   0 work      (1001) work      (1001)     7251 2023-05-12 05:20:22.000000 karuoflow-1.31/karuoflow/db/tables.py
+-rw-rw-r--   0 work      (1001) work      (1001)     2510 2023-05-12 05:20:22.000000 karuoflow-1.31/karuoflow/error_code.py
+-rw-rw-r--   0 work      (1001) work      (1001)    30685 2023-06-01 00:26:07.000000 karuoflow-1.31/karuoflow/flowapp.py
+-rw-rw-r--   0 work      (1001) work      (1001)    19421 2023-05-12 05:20:22.000000 karuoflow-1.31/karuoflow/flowmodelagent.py
+-rw-rw-r--   0 work      (1001) work      (1001)     6854 2023-05-12 05:20:22.000000 karuoflow-1.31/karuoflow/initflow.py
+drwxrwxr-x   0 work      (1001) work      (1001)        0 2023-06-01 00:38:56.247937 karuoflow-1.31/karuoflow/test/
+-rw-rw-r--   0 work      (1001) work      (1001)        0 2023-05-12 05:20:22.000000 karuoflow-1.31/karuoflow/test/__init__.py
+-rw-rw-r--   0 work      (1001) work      (1001)    11800 2023-05-12 05:49:21.000000 karuoflow-1.31/karuoflow/test/test_initenvironment.py
+drwxrwxr-x   0 work      (1001) work      (1001)        0 2023-06-01 00:38:56.246937 karuoflow-1.31/karuoflow.egg-info/
+-rw-rw-r--   0 work      (1001) work      (1001)      287 2023-06-01 00:38:56.000000 karuoflow-1.31/karuoflow.egg-info/PKG-INFO
+-rw-rw-r--   0 work      (1001) work      (1001)      466 2023-06-01 00:38:56.000000 karuoflow-1.31/karuoflow.egg-info/SOURCES.txt
+-rw-rw-r--   0 work      (1001) work      (1001)        1 2023-06-01 00:38:56.000000 karuoflow-1.31/karuoflow.egg-info/dependency_links.txt
+-rw-rw-r--   0 work      (1001) work      (1001)       26 2023-06-01 00:38:56.000000 karuoflow-1.31/karuoflow.egg-info/requires.txt
+-rw-rw-r--   0 work      (1001) work      (1001)       10 2023-06-01 00:38:56.000000 karuoflow-1.31/karuoflow.egg-info/top_level.txt
+-rw-rw-r--   0 work      (1001) work      (1001)       38 2023-06-01 00:38:56.248937 karuoflow-1.31/setup.cfg
+-rw-rw-r--   0 work      (1001) work      (1001)      685 2023-05-12 05:20:22.000000 karuoflow-1.31/setup.py
```

### Comparing `karuoflow-1.3/LICENSE` & `karuoflow-1.31/LICENSE`

 * *Files identical despite different names*

### Comparing `karuoflow-1.3/karuoflow/__init__.py` & `karuoflow-1.31/karuoflow/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,10 +28,11 @@
 @version 1.24 [2021-12-01] 修复bug，获取待审核列表时，排序未生效
 @version 1.25 [2022-03-10] 增加AppendSign 接口，供批量追加审核节点，（多能上会申请定制化场景需求）
 @version 1.26 [2022-03-14] 修正了查询已审核申请列表数据问题，该问题由关联查询引起，但模糊匹配仍然存在问题
 @version 1.27 [2022-03-14] 修正了1.26版本中join查询的条件bug
 @version 1.28 [2022-11-06] 针对sqlalchemy的缓存问题，对db操作包裹db_session.begin()事务上下文
 @version 1.29 [2022-11-06] 针对sqlalchemy的缓存问题，对db操作包裹db_session.begin()事务上下文，该机制因为在外部系统中传入了session，并在传入前开启了事务，因此会报错，先退回。
 @version 1.30 [2023-05-12] 增加更新ext_data字段的函数
+@version 1.31 [2023-06-01] 修改AddSign函数的签名，增加传入name和node_label两个参数
 '''
 
-__version__ = 1.30
+__version__ = 1.31
```

### Comparing `karuoflow-1.3/karuoflow/datadef.py` & `karuoflow-1.31/karuoflow/datadef.py`

 * *Files identical despite different names*

### Comparing `karuoflow-1.3/karuoflow/db/session.py` & `karuoflow-1.31/karuoflow/db/session.py`

 * *Files identical despite different names*

### Comparing `karuoflow-1.3/karuoflow/db/tables.py` & `karuoflow-1.31/karuoflow/db/tables.py`

 * *Files identical despite different names*

### Comparing `karuoflow-1.3/karuoflow/error_code.py` & `karuoflow-1.31/karuoflow/error_code.py`

 * *Files identical despite different names*

### Comparing `karuoflow-1.3/karuoflow/flowapp.py` & `karuoflow-1.31/karuoflow/flowapp.py`

 * *Files 0% similar despite different names*

```diff
@@ -315,15 +315,15 @@
                 finally:
                     self.db_session.close()
         else:
             _result.setNotExists()
 
         return _result
 
-    def AddSign(self, jobid:int, reviewer:list, memo:str="", ext_prop:dict=None, method="or", oper_uid=0):
+    def AddSign(self, jobid:int, reviewer:list, memo:str="", ext_prop:dict=None, method="or", oper_uid=0, name=None, node_label=None):
         """
         对未结束的流程进行加签(实际是转签)
         """
         _result = OperResult()
         job_item = self.db_session.query(TblFlowJob).get(jobid)
         if job_item:
             if job_item.IsClosed() or job_item.stage < 1 or job_item.stage >= len(job_item.apply_rules):
@@ -334,22 +334,22 @@
                     # 追加加签序号是当前处理阶段的下一阶段。
                     # 即，把加签人加到下一个阶段。
                     _insert_sign_stage = job_item.stage + 1
                     _apply_rules_copy.insert(_insert_sign_stage, {
                         "id": 0,
                         "icon": "",
                         "memo": memo,
-                        "name": _apply_rules_copy[0]["name"],
+                        "name": name if name else _apply_rules_copy[0]["name"],
                         "catalog": _apply_rules_copy[0]["catalog"],
                         "subflow": _apply_rules_copy[0]["subflow"],
                         "ext_prop": ext_prop,
                         "reviewer": reviewer,
                         "method": method,
                         "create_tm": datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
-                        "node_label": f"加签自{oper_uid}"
+                        "node_label": node_label if node_label else f"加签自{oper_uid}"
                     })
                 job_item.apply_rules = _apply_rules_copy
                 try:
                     self.db_session.commit()
                     _result.setSuccess()
                 except Exception as e:
                     print(str(e))
```

### Comparing `karuoflow-1.3/karuoflow/flowmodelagent.py` & `karuoflow-1.31/karuoflow/flowmodelagent.py`

 * *Files identical despite different names*

### Comparing `karuoflow-1.3/karuoflow/initflow.py` & `karuoflow-1.31/karuoflow/initflow.py`

 * *Files identical despite different names*

### Comparing `karuoflow-1.3/karuoflow/test/test_initenvironment.py` & `karuoflow-1.31/karuoflow/test/test_initenvironment.py`

 * *Files identical despite different names*

### Comparing `karuoflow-1.3/setup.py` & `karuoflow-1.31/setup.py`

 * *Files identical despite different names*

