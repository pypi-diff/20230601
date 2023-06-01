# Comparing `tmp/funnylog-1.0.1.tar.gz` & `tmp/funnylog-1.1.1.tar.gz`

## Comparing `funnylog-1.0.1.tar` & `funnylog-1.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    13092 2020-02-02 00:00:00.000000 funnylog-1.0.1/funnylog/__init__.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 funnylog-1.0.1/funnylog/__version__.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 funnylog-1.0.1/funnylog/conf.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 funnylog-1.0.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 funnylog-1.0.1/LICENSE
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 funnylog-1.0.1/README.md
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 funnylog-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 funnylog-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    13178 2020-02-02 00:00:00.000000 funnylog-1.1.1/funnylog/__init__.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 funnylog-1.1.1/funnylog/__version__.py
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 funnylog-1.1.1/funnylog/conf.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 funnylog-1.1.1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 funnylog-1.1.1/LICENSE
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 funnylog-1.1.1/README.md
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 funnylog-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 funnylog-1.1.1/PKG-INFO
```

### Comparing `funnylog-1.0.1/funnylog/__init__.py` & `funnylog-1.1.1/funnylog/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,35 +75,37 @@
         if len(args) == 0:
             return True
         # must be a regular method
         if args[0] == "self":
             return False
         return inspect.isfunction(value)
     return False
+
+
 def _trace(func):
     # pylint: disable=R0912
     @wraps(func)
     def wrapped(*a, **kw):
         try:
             # 对象实例化后调用类方法报错处理
             if (
-                # pylint: disable=protected-access
-                isinstance(a[0], inspect._findclass(func))
-                and func.__name__ != "__init__"
+                    # pylint: disable=protected-access
+                    isinstance(a[0], inspect._findclass(func))
+                    and func.__name__ != "__init__"
             ):
                 if func:
                     if any(
-                        [
-                            inspect.ismethod(func),
-                            is_static_method(
-                                # pylint: disable=protected-access
-                                inspect._findclass(func),
-                                func.__name__,
-                            ),
-                        ]
+                            [
+                                inspect.ismethod(func),
+                                is_static_method(
+                                    # pylint: disable=protected-access
+                                    inspect._findclass(func),
+                                    func.__name__,
+                                ),
+                            ]
                     ):
                         a = list(a)[1:]
         except IndexError:
             pass
         params = func_parameters(func, *a, **kw)
         # pylint: disable=unnecessary-lambda
         args = list(map(lambda x: represent(x), a))
@@ -111,15 +113,15 @@
             if not func.__name__.startswith("_"):
                 # 处理多行注释时候，换行空格过多
                 title = re.split(":param|@param|@return|:return", func.__doc__)[0]
                 title = "".join([ln.strip() for ln in title.split("\n")])
                 params_text = {}
                 # 获取方法的所有参数，并行程，{形参：实参} 的字典
                 for index, param in enumerate(
-                    inspect.signature(func).parameters.values()
+                        inspect.signature(func).parameters.values()
                 ):
                     if param.name == "self":
                         continue
                     params_text[param.name] = param.default
                     if args:
                         try:
                             params_text[param.name] = args[index]
@@ -148,46 +150,51 @@
             title = func.__name__
         logger.info(f"[{func.__name__}]: " f"{title}", auteadd=False)
         if func.__name__ != "__init__":
             with StepContext(title, params):
                 return func(*a, **kw)
         else:
             return func(*a, **kw)
+
     return wrapped
+
+
 def log(cls):
     """
     类日志装饰器
     :param cls:
     :return:
     """
     for name, obj in inspect.getmembers(
-        cls, lambda x: inspect.isfunction(x) or inspect.ismethod(x)
+            cls, lambda x: inspect.isfunction(x) or inspect.ismethod(x)
     ):
         try:
             class_name = obj.__qualname__.split(".")[0]
         except AttributeError:
             class_name = obj.__self__.__name__
         if name.startswith("_"):
             continue
         # else:
         if (
-            class_name.startswith(setting.CLASS_NAME_STARTSWITH)
-            or class_name.endswith(setting.CLASS_NAME_ENDSWITH)
-            or any(
-                (class_name.find(text) > -1 for text in setting.CLASS_NAME_CONTAIN)
-            )
+                class_name.startswith(setting.CLASS_NAME_STARTSWITH)
+                or class_name.endswith(setting.CLASS_NAME_ENDSWITH)
+                or any(
+            (class_name.find(text) > -1 for text in setting.CLASS_NAME_CONTAIN)
+        )
         ):
             if hasattr(getattr(cls, name), "__log"):
                 if not getattr(cls, name).__log:
                     setattr(cls, name, _trace(obj))
                     setattr(getattr(cls, name), "__log", True)
             else:
                 setattr(cls, name, _trace(obj))
                 setattr(getattr(cls, name), "__log", True)
     return cls
+
+
 class _ColoredFormatter(logging.Formatter):
     def formatMessage(self, record: logging.LogRecord) -> str:
         """Format a message from a record object."""
         if record.levelname == "INFO":
             record.levelname = "\033[1;97mINFO \033[0m"  # 白色
             record.message = re.sub(
                 r"(\[[a-zA-Z_]*?])?(.+)",
@@ -211,38 +218,44 @@
                 r"(\[[a-zA-Z_]*?])?(.+)",
                 r"\033[1;32m\1\033[0m\033[1;94m\2\033[0m",
                 record.message,
                 count=1,
             )
         message = super().formatMessage(record)
         return message
+
+
 # pylint: disable=R0903
 class IgnoreFilter(logging.Filter):
     """IgnoreFilter"""
+
     def filter(self, record):
         return record.name not in ("PIL.PngImagePlugin", "easyprocess")
+
+
 # pylint: disable=invalid-name
 class logger(metaclass=Singleton):
     """logger"""
     __author__ = "Litao <litaoa@uniontech.com>"
+
     def __init__(self, level):
         """
         日志配置
         :param level: case 路径
         """
         # 清空其他日志配置
         logging.root.handlers = []
-        log_path = os.path.join(setting.REPORT_PATH, "logs")
+        log_path = os.path.join(setting.LOG_PATH, "logs")
         if not os.path.exists(log_path):
             os.makedirs(log_path)
         log_path_debug = (
-            log_path + rf'/{time.strftime("%Y-%m-%d", time.localtime())}_debug.log'
+                log_path + rf'/{time.strftime("%Y-%m-%d", time.localtime())}_debug.log'
         )  # debug级别日志路径
         logfile_error = (
-            log_path + rf'/{time.strftime("%Y-%m-%d", time.localtime())}_error.log'
+                log_path + rf'/{time.strftime("%Y-%m-%d", time.localtime())}_error.log'
         )  # error级别日志路径
         # 路径不存在则创建
         if os.path.exists(log_path_debug):
             with open(log_path_debug, "w+", encoding="utf-8"):
                 pass
         if os.path.exists(logfile_error):
             with open(logfile_error, "w+", encoding="utf-8"):
@@ -290,61 +303,66 @@
         # 第四步，再创建一个handler，用于输出到控制台
         _ch = logging.StreamHandler()
         _ch.setLevel(level)  # 输出到console的log等级的开关
         _ch.addFilter(IgnoreFilter())
         # 第五步，定义handler的输出格式
         formatter = _ColoredFormatter(
             (
-             f"\033[1;31m{self.sys_arch}-{self.user_name}{self.ip_flag}\033[0m: "
-             "\033[93m%(asctime)s\033[0m | %(levelname)s | %(message)s"
+                f"\033[1;31m{self.sys_arch}-{self.user_name}{self.ip_flag}\033[0m: "
+                "\033[93m%(asctime)s\033[0m | %(levelname)s | %(message)s"
             ),
             datefmt=self.date_format,
         )
         _ch.setFormatter(formatter)
         # 第六步，将logger添加到handler里面
         self.logger.addHandler(_fh)
         self.logger.addHandler(fh_error)
         self.logger.addHandler(_ch)
+
     @staticmethod
     def info(message, auteadd=True):
         """info"""
         if len(logging.root.handlers) == 0:
             logger(setting.LOG_LEVEL)
         if auteadd:
             current_frame = sys._getframe(1) if hasattr(sys, "_getframe") else None
             message = f"[{current_frame.f_code.co_name}]: {message}"
         logging.info(message)
+
     @staticmethod
     def debug(message, auteadd=True):
         """debug"""
         if len(logging.root.handlers) == 0:
             logger(setting.LOG_LEVEL)
         if auteadd:
             current_frame = sys._getframe(1) if hasattr(sys, "_getframe") else None
             message = f"[{current_frame.f_code.co_name}]: {message}"
         # 判断是否用例直接调用底层基础方法，则输出info日志
         current_frame1 = sys._getframe(2) if hasattr(sys, "_getframe") else None
         if current_frame1.f_code.co_name.startswith("test_"):
             logging.info(message)
         else:
             logging.debug(message)
+
     @staticmethod
     def error(message, auteadd=True):
         """error"""
         if len(logging.root.handlers) == 0:
             logger(setting.LOG_LEVEL)
         if auteadd:
             current_frame = sys._getframe(1) if hasattr(sys, "_getframe") else None
             message = f"[{current_frame.f_code.co_name}]: {message}"
         logging.error(message)
+
     @staticmethod
     def exception(message):
         """exception"""
         if len(logging.root.handlers) == 0:
             logger(setting.LOG_LEVEL)
         logging.exception(message)
+
     @staticmethod
     def warning(message):
         """warning"""
         if len(logging.root.handlers) == 0:
             logger(setting.LOG_LEVEL)
-        logging.warning(message)
+        logging.warning(message)
```

### Comparing `funnylog-1.0.1/.gitignore` & `funnylog-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `funnylog-1.0.1/LICENSE` & `funnylog-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `funnylog-1.0.1/pyproject.toml` & `funnylog-1.1.1/pyproject.toml`

 * *Files identical despite different names*

