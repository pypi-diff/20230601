# Comparing `tmp/nonebug-0.3.3.tar.gz` & `tmp/nonebug-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebug-0.3.3.tar", max compression
+gzip compressed data, was "nonebug-0.3.4.tar", max compression
```

## Comparing `nonebug-0.3.3.tar` & `nonebug-0.3.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1064 2023-04-24 08:05:01.258998 nonebug-0.3.3/LICENSE
--rw-r--r--   0        0        0     1673 2023-04-24 08:05:01.258998 nonebug-0.3.3/README.md
--rw-r--r--   0        0        0      137 2023-04-24 08:05:01.258998 nonebug-0.3.3/nonebug/__init__.py
--rw-r--r--   0        0        0      153 2023-04-24 08:05:01.258998 nonebug-0.3.3/nonebug/app.py
--rw-r--r--   0        0        0     1176 2023-04-24 08:05:01.258998 nonebug-0.3.3/nonebug/base.py
--rw-r--r--   0        0        0      706 2023-04-24 08:05:01.258998 nonebug-0.3.3/nonebug/fixture.py
--rw-r--r--   0        0        0      204 2023-04-24 08:05:01.258998 nonebug-0.3.3/nonebug/mixin/__init__.py
--rw-r--r--   0        0        0     7404 2023-04-24 08:05:01.258998 nonebug-0.3.3/nonebug/mixin/call_api/__init__.py
--rw-r--r--   0        0        0     1738 2023-04-24 08:05:01.258998 nonebug-0.3.3/nonebug/mixin/call_api/fake.py
--rw-r--r--   0        0        0      517 2023-04-24 08:05:01.258998 nonebug-0.3.3/nonebug/mixin/call_api/model.py
--rw-r--r--   0        0        0     1903 2023-04-24 08:05:01.258998 nonebug-0.3.3/nonebug/mixin/dependent.py
--rw-r--r--   0        0        0     1315 2023-04-24 08:05:01.258998 nonebug-0.3.3/nonebug/mixin/driver.py
--rw-r--r--   0        0        0    11098 2023-04-24 08:05:01.258998 nonebug-0.3.3/nonebug/mixin/process/__init__.py
--rw-r--r--   0        0        0     2783 2023-04-24 08:05:01.258998 nonebug-0.3.3/nonebug/mixin/process/fake.py
--rw-r--r--   0        0        0     1330 2023-04-24 08:05:01.258998 nonebug-0.3.3/nonebug/mixin/process/model.py
--rw-r--r--   0        0        0     2930 2023-04-24 08:05:01.258998 nonebug-0.3.3/nonebug/provider.py
--rw-r--r--   0        0        0     1838 2023-04-24 08:05:01.262999 nonebug-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     2651 1970-01-01 00:00:00.000000 nonebug-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-01 13:41:20.319218 nonebug-0.3.4/LICENSE
+-rw-r--r--   0        0        0     1966 2023-06-01 13:41:20.319218 nonebug-0.3.4/README.md
+-rw-r--r--   0        0        0      137 2023-06-01 13:41:20.319218 nonebug-0.3.4/nonebug/__init__.py
+-rw-r--r--   0        0        0      153 2023-06-01 13:41:20.319218 nonebug-0.3.4/nonebug/app.py
+-rw-r--r--   0        0        0     1176 2023-06-01 13:41:20.319218 nonebug-0.3.4/nonebug/base.py
+-rw-r--r--   0        0        0      706 2023-06-01 13:41:20.319218 nonebug-0.3.4/nonebug/fixture.py
+-rw-r--r--   0        0        0      204 2023-06-01 13:41:20.319218 nonebug-0.3.4/nonebug/mixin/__init__.py
+-rw-r--r--   0        0        0     7807 2023-06-01 13:41:20.319218 nonebug-0.3.4/nonebug/mixin/call_api/__init__.py
+-rw-r--r--   0        0        0     1738 2023-06-01 13:41:20.319218 nonebug-0.3.4/nonebug/mixin/call_api/fake.py
+-rw-r--r--   0        0        0      587 2023-06-01 13:41:20.319218 nonebug-0.3.4/nonebug/mixin/call_api/model.py
+-rw-r--r--   0        0        0     1903 2023-06-01 13:41:20.319218 nonebug-0.3.4/nonebug/mixin/dependent.py
+-rw-r--r--   0        0        0     1315 2023-06-01 13:41:20.319218 nonebug-0.3.4/nonebug/mixin/driver.py
+-rw-r--r--   0        0        0    11098 2023-06-01 13:41:20.319218 nonebug-0.3.4/nonebug/mixin/process/__init__.py
+-rw-r--r--   0        0        0     2783 2023-06-01 13:41:20.319218 nonebug-0.3.4/nonebug/mixin/process/fake.py
+-rw-r--r--   0        0        0     1330 2023-06-01 13:41:20.319218 nonebug-0.3.4/nonebug/mixin/process/model.py
+-rw-r--r--   0        0        0     2930 2023-06-01 13:41:20.319218 nonebug-0.3.4/nonebug/provider.py
+-rw-r--r--   0        0        0     1886 2023-06-01 13:41:20.319218 nonebug-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     2938 1970-01-01 00:00:00.000000 nonebug-0.3.4/PKG-INFO
```

### Comparing `nonebug-0.3.3/LICENSE` & `nonebug-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebug-0.3.3/README.md` & `nonebug-0.3.4/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <!-- markdownlint-disable MD033 MD041 -->
 
 <p align="center">
-  <a href="https://v2.nonebot.dev/"><img src="https://github.com/nonebot/nonebug/raw/master/assets/logo.png" width="200" height="200" alt="nonebot"></a>
+  <a href="https://nonebot.dev/"><img src="https://github.com/nonebot/nonebug/raw/master/assets/logo.png" width="200" height="200" alt="nonebot"></a>
 </p>
 
 <div align="center">
 
 # NoneBug
 
 <!-- prettier-ignore-start -->
@@ -34,16 +34,32 @@
     <img src="https://img.shields.io/badge/telegram-botuniverse-blue?style=flat-square" alt="Telegram Channel">
   </a>
   <a href="https://discord.gg/VKtE6Gdc4h">
     <img src="https://discordapp.com/api/guilds/847819937858584596/widget.png?style=shield" alt="Discord Server">
   </a>
 </p>
 
+<p align="center">
+  <a href="https://nonebot.dev/docs/best-practice/testing/">文档</a>
+</p>
+
 ## 安装
 
 本工具为 [pytest](https://docs.pytest.org/en/stable/) 插件，需要配合 pytest 异步插件使用。
 
 ```bash
 poetry add nonebug pytest-asyncio -G test
 # 或者使用 anyio
 poetry add nonebug anyio -G test
 ```
+
+```bash
+pdm add nonebug pytest-asyncio -dG test
+# 或者使用 anyio
+pdm add nonebug anyio -dG test
+```
+
+```bash
+pip install nonebug pytest-asyncio
+# 或者使用 anyio
+pip install nonebug anyio
+```
```

#### html2text {}

```diff
@@ -1,9 +1,12 @@
                                    [nonebot]
                  # NoneBug   _â¨ NoneBot2 æµè¯æ¡æ¶ â¨_
 [license] [pypi] [python] [https://codecov.io/gh/nonebot/nonebug/branch/master/
                       graph/badge.svg?token=LDK2OFR231]
                  [QQ_Chat] [Telegram_Channel] [Discord_Server]
+                                    ææ¡£
 ## å®è£ æ¬å·¥å·ä¸º [pytest](https://docs.pytest.org/en/stable/
 ) æä»¶ï¼éè¦éå pytest å¼æ­¥æä»¶ä½¿ç¨ã ```bash poetry add nonebug
 pytest-asyncio -G test # æèä½¿ç¨ anyio poetry add nonebug anyio -G test
-```
+``` ```bash pdm add nonebug pytest-asyncio -dG test # æèä½¿ç¨ anyio pdm
+add nonebug anyio -dG test ``` ```bash pip install nonebug pytest-asyncio #
+æèä½¿ç¨ anyio pip install nonebug anyio ```
```

### Comparing `nonebug-0.3.3/nonebug/base.py` & `nonebug-0.3.4/nonebug/base.py`

 * *Files identical despite different names*

### Comparing `nonebug-0.3.3/nonebug/fixture.py` & `nonebug-0.3.4/nonebug/fixture.py`

 * *Files identical despite different names*

### Comparing `nonebug-0.3.3/nonebug/mixin/call_api/__init__.py` & `nonebug-0.3.4/nonebug/mixin/call_api/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -128,31 +128,40 @@
         new_bot = self.create_bot(auto_connect=False)
         monkeypatch.setattr(bot, "send", getattr(new_bot, "send"))
 
     def should_call_api(
         self,
         api: str,
         data: Dict[str, Any],
-        result: Any,
+        result: Optional[Any] = None,
+        exception: Optional[Exception] = None,
         adapter: Optional["Adapter"] = None,
     ) -> Api:
-        model = Api(name=api, data=data, result=result, adapter=adapter)
+        model = Api(
+            name=api, data=data, result=result, exception=exception, adapter=adapter
+        )
         self.wait_list.put(model)
         return model
 
     def should_call_send(
         self,
         event: "Event",
         message: Union[str, "Message", "MessageSegment"],
-        result: Any,
+        result: Optional[Any] = None,
+        exception: Optional[Exception] = None,
         bot: Optional["Bot"] = None,
         **kwargs: Any,
     ) -> Send:
         model = Send(
-            event=event, message=message, kwargs=kwargs, result=result, bot=bot
+            event=event,
+            message=message,
+            kwargs=kwargs,
+            result=result,
+            exception=exception,
+            bot=bot,
         )
         self.wait_list.put(model)
         return model
 
     def got_call_api(self, adapter: "Adapter", api: str, **data: Any) -> Any:
         if self.wait_list.empty():
             pytest.fail(
@@ -167,14 +176,17 @@
             pytest.fail(
                 f"Application got api call {api} with data {data} but expected {model.data}"
             )
         if model.adapter and model.adapter != adapter:
             pytest.fail(
                 f"Application got api call {api} with adapter {adapter} but expected {model.adapter}"
             )
+
+        if model.exception is not None:
+            raise model.exception
         return model.result
 
     def got_call_send(
         self,
         bot: "Bot",
         event: "Event",
         message: Union[str, "Message", "MessageSegment"],
@@ -199,14 +211,17 @@
             pytest.fail(
                 f"Application got send call with kwargs {kwargs} but expected {model.kwargs}"
             )
         if model.bot and model.bot != bot:
             pytest.fail(
                 f"Application got send call with bot {bot} but expected {model.bot}"
             )
+
+        if model.exception is not None:
+            raise model.exception
         return model.result
 
     @contextlib.contextmanager
     def _prepare_api_context(self):
         from nonebot import get_driver
 
         with pytest.MonkeyPatch.context() as m:
```

### Comparing `nonebug-0.3.3/nonebug/mixin/call_api/fake.py` & `nonebug-0.3.4/nonebug/mixin/call_api/fake.py`

 * *Files identical despite different names*

### Comparing `nonebug-0.3.3/nonebug/mixin/call_api/model.py` & `nonebug-0.3.4/nonebug/mixin/call_api/model.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,17 +11,19 @@
 
 
 @dataclass
 class Api(Model):
     name: str
     data: Dict[str, Any]
     result: Any
+    exception: Optional[Exception]
     adapter: Optional["Adapter"]
 
 
 @dataclass
 class Send(Model):
     event: "Event"
     message: Union[str, "Message", "MessageSegment"]
     kwargs: Dict[str, Any]
     result: Any
+    exception: Optional[Exception]
     bot: Optional["Bot"]
```

### Comparing `nonebug-0.3.3/nonebug/mixin/dependent.py` & `nonebug-0.3.4/nonebug/mixin/dependent.py`

 * *Files identical despite different names*

### Comparing `nonebug-0.3.3/nonebug/mixin/driver.py` & `nonebug-0.3.4/nonebug/mixin/driver.py`

 * *Files identical despite different names*

### Comparing `nonebug-0.3.3/nonebug/mixin/process/__init__.py` & `nonebug-0.3.4/nonebug/mixin/process/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebug-0.3.3/nonebug/mixin/process/fake.py` & `nonebug-0.3.4/nonebug/mixin/process/fake.py`

 * *Files identical despite different names*

### Comparing `nonebug-0.3.3/nonebug/mixin/process/model.py` & `nonebug-0.3.4/nonebug/mixin/process/model.py`

 * *Files identical despite different names*

### Comparing `nonebug-0.3.3/nonebug/provider.py` & `nonebug-0.3.4/nonebug/provider.py`

 * *Files identical despite different names*

### Comparing `nonebug-0.3.3/pyproject.toml` & `nonebug-0.3.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 [tool.poetry]
 name = "nonebug"
-version = "0.3.3"
+version = "0.3.4"
 description = "nonebot2 test framework"
 authors = ["AkiraXie <l997460364@outlook.com>", "yanyongyu <yyy@nonebot.dev>"]
 license = "MIT"
 readme = "README.md"
-homepage = "https://v2.nonebot.dev/"
+homepage = "https://nonebot.dev/"
 repository = "https://github.com/nonebot/nonebug"
-documentation = "https://v2.nonebot.dev/"
+documentation = "https://nonebot.dev/"
 keywords = ["nonebot", "pytest", "test", "bot", "onebot", "cqhttp"]
 classifiers = ["Framework :: Pytest"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pytest = "^7.0.0"
 asgiref = "^3.4.0"
 nonebot2 = "^2.0.0-rc.2"
 typing-extensions = "^4.0.0"
 async-asgi-testclient = "^1.4.8"
 
 [tool.poetry.group.dev.dependencies]
+pycln = "^2.1.4"
 isort = "^5.10.1"
 black = "^23.1.0"
 nonemoji = "^0.1.3"
 pre-commit = "^3.0.0"
 nonebot2 = { git = "https://github.com/nonebot/nonebot2.git" }
 
 [tool.poetry.group.test.dependencies]
@@ -49,14 +50,18 @@
 profile = "black"
 line_length = 88
 length_sort = true
 skip_gitignore = true
 force_sort_within_sections = true
 extra_standard_library = ["typing_extensions"]
 
+[tool.pycln]
+path = "."
+all = false
+
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
     "def __repr__",
     "def __str__",
     "if __name__ == .__main__.:",
     "if (typing\\.)?TYPE_CHECKING( is True)?:",
```

### Comparing `nonebug-0.3.3/PKG-INFO` & `nonebug-0.3.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: nonebug
-Version: 0.3.3
+Version: 0.3.4
 Summary: nonebot2 test framework
-Home-page: https://v2.nonebot.dev/
+Home-page: https://nonebot.dev/
 License: MIT
 Keywords: nonebot,pytest,test,bot,onebot,cqhttp
 Author: AkiraXie
 Author-email: l997460364@outlook.com
 Requires-Python: >=3.8,<4.0
 Classifier: Framework :: Pytest
 Classifier: License :: OSI Approved :: MIT License
@@ -16,22 +16,22 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: asgiref (>=3.4.0,<4.0.0)
 Requires-Dist: async-asgi-testclient (>=1.4.8,<2.0.0)
 Requires-Dist: nonebot2 (>=2.0.0-rc.2,<3.0.0)
 Requires-Dist: pytest (>=7.0.0,<8.0.0)
 Requires-Dist: typing-extensions (>=4.0.0,<5.0.0)
-Project-URL: Documentation, https://v2.nonebot.dev/
+Project-URL: Documentation, https://nonebot.dev/
 Project-URL: Repository, https://github.com/nonebot/nonebug
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable MD033 MD041 -->
 
 <p align="center">
-  <a href="https://v2.nonebot.dev/"><img src="https://github.com/nonebot/nonebug/raw/master/assets/logo.png" width="200" height="200" alt="nonebot"></a>
+  <a href="https://nonebot.dev/"><img src="https://github.com/nonebot/nonebug/raw/master/assets/logo.png" width="200" height="200" alt="nonebot"></a>
 </p>
 
 <div align="center">
 
 # NoneBug
 
 <!-- prettier-ignore-start -->
@@ -60,17 +60,33 @@
     <img src="https://img.shields.io/badge/telegram-botuniverse-blue?style=flat-square" alt="Telegram Channel">
   </a>
   <a href="https://discord.gg/VKtE6Gdc4h">
     <img src="https://discordapp.com/api/guilds/847819937858584596/widget.png?style=shield" alt="Discord Server">
   </a>
 </p>
 
+<p align="center">
+  <a href="https://nonebot.dev/docs/best-practice/testing/">文档</a>
+</p>
+
 ## 安装
 
 本工具为 [pytest](https://docs.pytest.org/en/stable/) 插件，需要配合 pytest 异步插件使用。
 
 ```bash
 poetry add nonebug pytest-asyncio -G test
 # 或者使用 anyio
 poetry add nonebug anyio -G test
 ```
 
+```bash
+pdm add nonebug pytest-asyncio -dG test
+# 或者使用 anyio
+pdm add nonebug anyio -dG test
+```
+
+```bash
+pip install nonebug pytest-asyncio
+# 或者使用 anyio
+pip install nonebug anyio
+```
+
```

#### html2text {}

```diff
@@ -1,23 +1,26 @@
-Metadata-Version: 2.1 Name: nonebug Version: 0.3.3 Summary: nonebot2 test
-framework Home-page: https://v2.nonebot.dev/ License: MIT Keywords:
+Metadata-Version: 2.1 Name: nonebug Version: 0.3.4 Summary: nonebot2 test
+framework Home-page: https://nonebot.dev/ License: MIT Keywords:
 nonebot,pytest,test,bot,onebot,cqhttp Author: AkiraXie Author-email:
 l997460364@outlook.com Requires-Python: >=3.8,<4.0 Classifier: Framework ::
 Pytest Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: asgiref (>=3.4.0,<4.0.0) Requires-Dist: async-
 asgi-testclient (>=1.4.8,<2.0.0) Requires-Dist: nonebot2 (>=2.0.0-rc.2,<3.0.0)
 Requires-Dist: pytest (>=7.0.0,<8.0.0) Requires-Dist: typing-extensions
-(>=4.0.0,<5.0.0) Project-URL: Documentation, https://v2.nonebot.dev/ Project-
-URL: Repository, https://github.com/nonebot/nonebug Description-Content-Type:
-text/markdown
+(>=4.0.0,<5.0.0) Project-URL: Documentation, https://nonebot.dev/ Project-URL:
+Repository, https://github.com/nonebot/nonebug Description-Content-Type: text/
+markdown
                                    [nonebot]
                  # NoneBug   _â¨ NoneBot2 æµè¯æ¡æ¶ â¨_
 [license] [pypi] [python] [https://codecov.io/gh/nonebot/nonebug/branch/master/
                       graph/badge.svg?token=LDK2OFR231]
                  [QQ_Chat] [Telegram_Channel] [Discord_Server]
+                                    ææ¡£
 ## å®è£ æ¬å·¥å·ä¸º [pytest](https://docs.pytest.org/en/stable/
 ) æä»¶ï¼éè¦éå pytest å¼æ­¥æä»¶ä½¿ç¨ã ```bash poetry add nonebug
 pytest-asyncio -G test # æèä½¿ç¨ anyio poetry add nonebug anyio -G test
-```
+``` ```bash pdm add nonebug pytest-asyncio -dG test # æèä½¿ç¨ anyio pdm
+add nonebug anyio -dG test ``` ```bash pip install nonebug pytest-asyncio #
+æèä½¿ç¨ anyio pip install nonebug anyio ```
```

