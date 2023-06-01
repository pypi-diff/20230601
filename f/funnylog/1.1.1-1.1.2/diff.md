# Comparing `tmp/funnylog-1.1.1.tar.gz` & `tmp/funnylog-1.1.2.tar.gz`

## Comparing `funnylog-1.1.1.tar` & `funnylog-1.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    13178 2020-02-02 00:00:00.000000 funnylog-1.1.1/funnylog/__init__.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 funnylog-1.1.1/funnylog/__version__.py
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 funnylog-1.1.1/funnylog/conf.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 funnylog-1.1.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 funnylog-1.1.1/LICENSE
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 funnylog-1.1.1/README.md
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 funnylog-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 funnylog-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    13278 2020-02-02 00:00:00.000000 funnylog-1.1.2/funnylog/__init__.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 funnylog-1.1.2/funnylog/__version__.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 funnylog-1.1.2/funnylog/conf.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 funnylog-1.1.2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 funnylog-1.1.2/LICENSE
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 funnylog-1.1.2/README.md
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 funnylog-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 funnylog-1.1.2/PKG-INFO
```

### Comparing `funnylog-1.1.1/funnylog/__init__.py` & `funnylog-1.1.2/funnylog/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,15 +240,15 @@
     def __init__(self, level):
         """
         日志配置
         :param level: case 路径
         """
         # 清空其他日志配置
         logging.root.handlers = []
-        log_path = os.path.join(setting.LOG_PATH, "logs")
+        log_path = os.path.join(setting.LOG_FILE_PATH, "logs")
         if not os.path.exists(log_path):
             os.makedirs(log_path)
         log_path_debug = (
                 log_path + rf'/{time.strftime("%Y-%m-%d", time.localtime())}_debug.log'
         )  # debug级别日志路径
         logfile_error = (
                 log_path + rf'/{time.strftime("%Y-%m-%d", time.localtime())}_error.log'
@@ -333,18 +333,21 @@
         """debug"""
         if len(logging.root.handlers) == 0:
             logger(setting.LOG_LEVEL)
         if auteadd:
             current_frame = sys._getframe(1) if hasattr(sys, "_getframe") else None
             message = f"[{current_frame.f_code.co_name}]: {message}"
         # 判断是否用例直接调用底层基础方法，则输出info日志
-        current_frame1 = sys._getframe(2) if hasattr(sys, "_getframe") else None
-        if current_frame1.f_code.co_name.startswith("test_"):
-            logging.info(message)
-        else:
+        try:
+            current_frame1 = sys._getframe(2) if hasattr(sys, "_getframe") else None
+            if current_frame1.f_code.co_name.startswith("test_"):
+                logging.info(message)
+            else:
+                logging.debug(message)
+        except ValueError:
             logging.debug(message)
 
     @staticmethod
     def error(message, auteadd=True):
         """error"""
         if len(logging.root.handlers) == 0:
             logger(setting.LOG_LEVEL)
```

### Comparing `funnylog-1.1.1/.gitignore` & `funnylog-1.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `funnylog-1.1.1/LICENSE` & `funnylog-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `funnylog-1.1.1/pyproject.toml` & `funnylog-1.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `funnylog-1.1.1/PKG-INFO` & `funnylog-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funnylog
-Version: 1.1.1
+Version: 1.1.2
 Summary: PaddleOCR-RPC
 Project-URL: Source, https://github.com/funny-test/funnylog
 Project-URL: Documentation, https://funny-test.github.io/funnylog
 Author-email: mikigo <1964191531@qq.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: funnylog Version: 1.1.1 Summary: PaddleOCR-RPC
+Metadata-Version: 2.1 Name: funnylog Version: 1.1.2 Summary: PaddleOCR-RPC
 Project-URL: Source, https://github.com/funny-test/funnylog Project-URL:
 Documentation, https://funny-test.github.io/funnylog Author-email: mikigo
 <1964191531@qq.com> License-File: LICENSE Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Requires-Python: >=3.7
 Requires-Dist: allure-pytest Provides-Extra: doc Requires-Dist: mkdocs-
 material; extra == 'doc' Provides-Extra: test Requires-Dist: pytest; extra ==
```

