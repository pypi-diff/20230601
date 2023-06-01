# Comparing `tmp/nonebot-plugin-alconna-0.6.1.tar.gz` & `tmp/nonebot-plugin-alconna-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-alconna-0.6.1.tar", last modified: Tue May 30 09:10:17 2023, max compression
+gzip compressed data, was "nonebot-plugin-alconna-0.7.0.tar", last modified: Thu Jun  1 09:05:07 2023, max compression
```

## Comparing `nonebot-plugin-alconna-0.6.1.tar` & `nonebot-plugin-alconna-0.7.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524011 nonebot-plugin-alconna-0.6.1/LICENSE
--rw-r--r--   0        0        0     1135 2023-05-30 09:08:03.666783 nonebot-plugin-alconna-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     8401 2023-05-18 16:06:27.910527 nonebot-plugin-alconna-0.6.1/README.md
--rw-r--r--   0        0        0     1241 2023-05-18 15:49:31.978140 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/__init__.py
--rw-r--r--   0        0        0      383 2023-05-11 04:41:26.166268 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/__init__.py
--rw-r--r--   0        0        0      523 2023-05-10 10:09:15.599546 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/bilibili.py
--rw-r--r--   0        0        0     1007 2023-05-10 10:09:15.573188 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/console.py
--rw-r--r--   0        0        0     1661 2023-05-10 10:09:15.609172 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/ding.py
--rw-r--r--   0        0        0     2141 2023-05-10 10:09:15.564123 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/feishu.py
--rw-r--r--   0        0        0      519 2023-05-10 10:09:15.541809 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/github.py
--rw-r--r--   0        0        0     1163 2023-05-10 10:09:15.636179 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/kook.py
--rw-r--r--   0        0        0      761 2023-05-10 10:09:15.651191 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/minecraft.py
--rw-r--r--   0        0        0     3155 2023-05-10 10:09:15.519983 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/mirai.py
--rw-r--r--   0        0        0     1088 2023-05-10 10:09:15.628175 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/ntchat.py
--rw-r--r--   0        0        0     3177 2023-05-10 10:09:15.618177 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/onebot11.py
--rw-r--r--   0        0        0     2517 2023-05-10 10:09:15.661217 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/onebot12.py
--rw-r--r--   0        0        0     3227 2023-05-10 10:09:15.529594 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/qqguild.py
--rw-r--r--   0        0        0     3126 2023-05-10 10:09:15.670151 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/telegram.py
--rw-r--r--   0        0        0      581 2023-05-10 10:09:15.553296 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/argv.py
--rw-r--r--   0        0        0      405 2023-05-10 09:00:57.054628 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/config.py
--rw-r--r--   0        0        0      180 2023-05-10 08:33:24.079951 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/consts.py
--rw-r--r--   0        0        0      109 2023-05-11 15:42:43.320472 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/i18n/.config.json
--rw-r--r--   0        0        0      301 2023-05-11 15:42:18.920450 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/i18n/en-US.json
--rw-r--r--   0        0        0      262 2023-05-11 15:42:18.885191 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/i18n/zh-CN.json
--rw-r--r--   0        0        0     2277 2023-05-30 09:08:03.646906 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/matcher.py
--rw-r--r--   0        0        0     1093 2023-05-30 09:08:03.613798 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/matcher.pyi
--rw-r--r--   0        0        0     1478 2023-05-26 08:51:03.247079 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/model.py
--rw-r--r--   0        0        0     3830 2023-05-26 08:51:03.151926 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/params.py
--rw-r--r--   0        0        0     8721 2023-05-30 09:08:03.602783 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/rule.py
--rw-r--r--   0        0        0     2092 2023-05-30 09:08:03.637783 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/typings.py
--rw-r--r--   0        0        0     8484 1970-01-01 00:00:00.000000 nonebot-plugin-alconna-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524011 nonebot-plugin-alconna-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1524 2023-06-01 08:47:38.630190 nonebot-plugin-alconna-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     8521 2023-06-01 08:55:17.953962 nonebot-plugin-alconna-0.7.0/README.md
+-rw-r--r--   0        0        0     1789 2023-06-01 08:53:41.996763 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/__init__.py
+-rw-r--r--   0        0        0      383 2023-05-11 04:41:26.166268 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/__init__.py
+-rw-r--r--   0        0        0      523 2023-05-31 10:32:51.256024 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/bilibili.py
+-rw-r--r--   0        0        0     1052 2023-05-31 10:32:51.263057 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/console.py
+-rw-r--r--   0        0        0     1661 2023-05-31 10:32:51.272058 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/ding.py
+-rw-r--r--   0        0        0     2120 2023-05-31 10:32:51.280029 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/feishu.py
+-rw-r--r--   0        0        0      519 2023-05-31 10:32:51.286108 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/github.py
+-rw-r--r--   0        0        0     1163 2023-05-31 10:32:51.293032 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/kook.py
+-rw-r--r--   0        0        0      761 2023-05-31 10:32:51.300025 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/minecraft.py
+-rw-r--r--   0        0        0     3129 2023-05-31 10:32:51.308024 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/mirai.py
+-rw-r--r--   0        0        0     1088 2023-05-31 10:32:51.314025 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/ntchat.py
+-rw-r--r--   0        0        0     3151 2023-05-31 10:32:51.321077 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/onebot11.py
+-rw-r--r--   0        0        0     2496 2023-05-31 10:32:51.327029 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/onebot12.py
+-rw-r--r--   0        0        0     3251 2023-05-31 10:32:51.334314 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/qqguild.py
+-rw-r--r--   0        0        0     3116 2023-05-31 10:32:51.341066 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/telegram.py
+-rw-r--r--   0        0        0      579 2023-05-31 10:32:51.160062 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/argv.py
+-rw-r--r--   0        0        0      405 2023-05-31 10:32:51.165611 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/config.py
+-rw-r--r--   0        0        0      182 2023-05-31 10:31:14.855148 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/consts.py
+-rw-r--r--   0        0        0      109 2023-05-11 15:42:43.320472 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/i18n/.config.json
+-rw-r--r--   0        0        0      301 2023-05-11 15:42:18.920450 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/i18n/en-US.json
+-rw-r--r--   0        0        0      262 2023-05-11 15:42:18.885191 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/i18n/zh-CN.json
+-rw-r--r--   0        0        0     2277 2023-06-01 08:39:16.821566 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/matcher.py
+-rw-r--r--   0        0        0     1091 2023-05-31 10:32:51.198463 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/matcher.pyi
+-rw-r--r--   0        0        0     1478 2023-05-31 10:32:51.204511 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/model.py
+-rw-r--r--   0        0        0     3830 2023-05-31 10:32:51.214457 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/params.py
+-rw-r--r--   0        0        0     8722 2023-05-31 10:32:51.231456 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/rule.py
+-rw-r--r--   0        0        0     2094 2023-05-31 10:32:51.240029 nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/typings.py
+-rw-r--r--   0        0        0     8601 1970-01-01 00:00:00.000000 nonebot-plugin-alconna-0.7.0/PKG-INFO
```

### Comparing `nonebot-plugin-alconna-0.6.1/LICENSE` & `nonebot-plugin-alconna-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.6.1/pyproject.toml` & `nonebot-plugin-alconna-0.7.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [project]
 name = "nonebot-plugin-alconna"
-version = "0.6.1"
+version = "0.7.0"
 description = "Alconna Adapter for Nonebot"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0rc4",
     "arclet-alconna<2.0.0, >=1.7.7",
-    "arclet-alconna-tools<0.7.0, >=0.6.0",
+    "arclet-alconna-tools<0.7.0, >=0.6.1",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 keywords = [
     "command",
     "argparse",
     "cli",
@@ -30,14 +30,15 @@
 requires = [
     "pdm-pep517>=1.0",
 ]
 build-backend = "pdm.pep517.api"
 
 [tool.pdm.dev-dependencies]
 dev = [
+    "nonebot2>=2.0.0",
     "fix-future-annotations>=0.5.0",
     "nonebot-adapter-onebot>=2.2.3",
     "nonebot-adapter-feishu>=2.0.0b8",
     "nonebot-adapter-console>=0.3.2",
     "nonebot-adapter-ding>=2.0.0a16",
     "nonebot-adapter-mirai2>=0.0.22",
     "nonebot-adapter-minecraft>=0.1.1",
@@ -46,7 +47,32 @@
     "nonebot-adapter-telegram>=0.1.0b10",
 ]
 
 [tool.pdm.build]
 includes = [
     "src/nonebot_plugin_alconna",
 ]
+
+[tool.black]
+line-length = 88
+target-version = [
+    "py38",
+    "py39",
+    "py310",
+    "py311",
+]
+include = "\\.pyi?$"
+extend-exclude = ""
+
+[tool.isort]
+profile = "black"
+line_length = 88
+length_sort = false
+skip_gitignore = true
+force_sort_within_sections = true
+src_paths = [
+    "nonebot",
+    "tests",
+]
+extra_standard_library = [
+    "typing_extensions",
+]
```

### Comparing `nonebot-plugin-alconna-0.6.1/README.md` & `nonebot-plugin-alconna-0.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,17 @@
 ## 讨论
 
 QQ 交流群: [链接](https://jq.qq.com/?_wv=1027&k=PUPOnCSH)
 
 
 ## 使用方法
 
+Nonebot文档: [📖这里](https://nonebot.dev/docs/advanced/matcher#alconna)
+详细介绍: [📦这里](/docs.md)
+
 ### 消息解析
 
 ```python
 from nonebot.adapters.onebot.v12 import Message, MessageSegment
 from arclet.alconna import Alconna, Option, Args
 
 msg = Message("Hello! --foo 123")
```

### Comparing `nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/bilibili.py` & `nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/bilibili.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from nonebot.adapters.billibili.message import Message, BaseMessage
+from arclet.alconna import argv_config, set_default_argv_type
+from nonebot.adapters.billibili.message import BaseMessage, Message
 from nonebot_plugin_alconna.argv import MessageArgv
-from arclet.alconna import set_default_argv_type, argv_config
 
 
 class BiliMessageArgv(MessageArgv):
     ...
 
 
 set_default_argv_type(BiliMessageArgv)
```

### Comparing `nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/console.py` & `nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/console.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-from nonebot_plugin_alconna.typings import SegmentPattern
-from nonebot.adapters.console.message import MessageSegment, Message, BaseMessage
+from arclet.alconna import argv_config, set_default_argv_type
+from nonebot.adapters.console.message import BaseMessage
 from nonebot.adapters.console.message import Emoji as _Emoji
-from nonebot.adapters.console.message import Markup as _Markup
 from nonebot.adapters.console.message import Markdown as _Markdown
+from nonebot.adapters.console.message import Markup as _Markup
+from nonebot.adapters.console.message import Message, MessageSegment
 from nonebot_plugin_alconna.argv import MessageArgv
-from arclet.alconna import set_default_argv_type, argv_config
+from nonebot_plugin_alconna.typings import SegmentPattern
 
 
 class ConsoleMessageArgv(MessageArgv):
     ...
 
 
 set_default_argv_type(ConsoleMessageArgv)
```

### Comparing `nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/ding.py` & `nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/ding.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from nonebot_plugin_alconna.typings import SegmentPattern
-from nonebot.adapters.ding.message import MessageSegment, Message, BaseMessage
+from arclet.alconna import argv_config, set_default_argv_type
+from nonebot.adapters.ding.message import BaseMessage, Message, MessageSegment
 from nonebot_plugin_alconna.argv import MessageArgv
-from arclet.alconna import set_default_argv_type, argv_config
+from nonebot_plugin_alconna.typings import SegmentPattern
 
 
 class DingMessageArgv(MessageArgv):
     ...
 
 
 set_default_argv_type(DingMessageArgv)
```

### Comparing `nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/feishu.py` & `nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/feishu.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,13 @@
-from nonebot_plugin_alconna.typings import SegmentPattern
-from nepattern import (
-    BasePattern,
-    PatternModel,
-    UnionPattern,
-)
+from arclet.alconna import argv_config, set_default_argv_type
+from nepattern import BasePattern, PatternModel, UnionPattern
 from nepattern.main import INTEGER
-from nonebot.adapters.feishu.message import MessageSegment, BaseMessage, Message
+from nonebot.adapters.feishu.message import BaseMessage, Message, MessageSegment
 from nonebot_plugin_alconna.argv import MessageArgv
-from arclet.alconna import set_default_argv_type, argv_config
+from nonebot_plugin_alconna.typings import SegmentPattern
 
 
 class FeishuMessageArgv(MessageArgv):
     ...
 
 
 set_default_argv_type(FeishuMessageArgv)
```

### Comparing `nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/github.py` & `nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/github.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from nonebot.adapters.github.message import Message, BaseMessage
+from arclet.alconna import argv_config, set_default_argv_type
+from nonebot.adapters.github.message import BaseMessage, Message
 from nonebot_plugin_alconna.argv import MessageArgv
-from arclet.alconna import set_default_argv_type, argv_config
 
 
 class GHMessageArgv(MessageArgv):
     ...
 
 
 set_default_argv_type(GHMessageArgv)
```

### Comparing `nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/kook.py` & `nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/kook.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from nonebot_plugin_alconna.typings import SegmentPattern
-from nonebot.adapters.kaiheila.message import MessageSegment, Message, BaseMessage
+from arclet.alconna import argv_config, set_default_argv_type
+from nonebot.adapters.kaiheila.message import BaseMessage, Message, MessageSegment
 from nonebot_plugin_alconna.argv import MessageArgv
-from arclet.alconna import set_default_argv_type, argv_config
+from nonebot_plugin_alconna.typings import SegmentPattern
 
 
 class KookMessageArgv(MessageArgv):
     ...
 
 
 set_default_argv_type(KookMessageArgv)
```

### Comparing `nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/minecraft.py` & `nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/minecraft.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from nonebot_plugin_alconna.typings import SegmentPattern
+from arclet.alconna import argv_config, set_default_argv_type
+from nonebot.adapters.minecraft.message import BaseMessage, Message, MessageSegment
 from nonebot_plugin_alconna.argv import MessageArgv
-from nonebot.adapters.minecraft.message import MessageSegment, Message, BaseMessage
-from arclet.alconna import set_default_argv_type, argv_config
+from nonebot_plugin_alconna.typings import SegmentPattern
 
 
 class MinecraftMessageArgv(MessageArgv):
     ...
 
 
 set_default_argv_type(MinecraftMessageArgv)
```

### Comparing `nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/mirai.py` & `nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/mirai.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,13 @@
-from nonebot_plugin_alconna.typings import SegmentPattern
-from nepattern import (
-    URL,
-    BasePattern,
-    PatternModel,
-    UnionPattern,
-)
+from arclet.alconna import argv_config, set_default_argv_type
+from nepattern import URL, BasePattern, PatternModel, UnionPattern
 from nepattern.main import INTEGER
-from nonebot.adapters.mirai2.message import MessageSegment, BaseMessage, MessageChain
+from nonebot.adapters.mirai2.message import BaseMessage, MessageChain, MessageSegment
 from nonebot_plugin_alconna.argv import MessageArgv
-from arclet.alconna import set_default_argv_type, argv_config
+from nonebot_plugin_alconna.typings import SegmentPattern
 
 
 class MiraiMessageArgv(MessageArgv):
     ...
 
 
 set_default_argv_type(MiraiMessageArgv)
```

### Comparing `nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/ntchat.py` & `nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/ntchat.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from nonebot_plugin_alconna.typings import SegmentPattern
-from nonebot.adapters.ntchat.message import MessageSegment, BaseMessage, Message
+from arclet.alconna import argv_config, set_default_argv_type
+from nonebot.adapters.ntchat.message import BaseMessage, Message, MessageSegment
 from nonebot_plugin_alconna.argv import MessageArgv
-from arclet.alconna import set_default_argv_type, argv_config
+from nonebot_plugin_alconna.typings import SegmentPattern
 
 
 class WXMessageArgv(MessageArgv):
     ...
 
 
 set_default_argv_type(WXMessageArgv)
```

### Comparing `nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/onebot11.py` & `nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/onebot11.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,13 @@
-from nonebot_plugin_alconna.typings import SegmentPattern
-from nepattern import (
-    URL,
-    BasePattern,
-    PatternModel,
-    UnionPattern,
-)
+from arclet.alconna import argv_config, set_default_argv_type
+from nepattern import URL, BasePattern, PatternModel, UnionPattern
 from nepattern.main import INTEGER
-from nonebot.adapters.onebot.v11.message import MessageSegment, BaseMessage, Message
+from nonebot.adapters.onebot.v11.message import BaseMessage, Message, MessageSegment
 from nonebot_plugin_alconna.argv import MessageArgv
-from arclet.alconna import set_default_argv_type, argv_config
+from nonebot_plugin_alconna.typings import SegmentPattern
 
 
 class Ob11MessageArgv(MessageArgv):
     ...
 
 
 set_default_argv_type(Ob11MessageArgv)
```

### Comparing `nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/onebot12.py` & `nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/onebot12.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,13 @@
-from nonebot_plugin_alconna.typings import SegmentPattern
-from nepattern import (
-    BasePattern,
-    PatternModel,
-    UnionPattern,
-)
+from arclet.alconna import argv_config, set_default_argv_type
+from nepattern import BasePattern, PatternModel, UnionPattern
 from nepattern.main import INTEGER, URL
-from nonebot.adapters.onebot.v12.message import MessageSegment, BaseMessage, Message
+from nonebot.adapters.onebot.v12.message import BaseMessage, Message, MessageSegment
 from nonebot_plugin_alconna.argv import MessageArgv
-from arclet.alconna import set_default_argv_type, argv_config
+from nonebot_plugin_alconna.typings import SegmentPattern
 
 
 class Ob12MessageArgv(MessageArgv):
     ...
 
 
 set_default_argv_type(Ob12MessageArgv)
```

### Comparing `nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/qqguild.py` & `nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/qqguild.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,23 @@
-from nonebot_plugin_alconna.typings import SegmentPattern
-from nepattern import (
-    BasePattern,
-    PatternModel,
-    UnionPattern,
-)
+from arclet.alconna import argv_config, set_default_argv_type
+from nepattern import BasePattern, PatternModel, UnionPattern
 from nepattern.main import INTEGER, URL
-from nonebot.adapters.qqguild.message import MessageSegment, Message, BaseMessage
-from nonebot.adapters.qqguild.message import Emoji as _Emoji
-from nonebot.adapters.qqguild.message import MentionUser as _MentionUser
-from nonebot.adapters.qqguild.message import MentionChannel as _MentionChannel
-from nonebot.adapters.qqguild.message import MentionEveryone as _MentionEveryone
+from nonebot.adapters.qqguild.message import Ark as _Ark
 from nonebot.adapters.qqguild.message import Attachment as _Attachment
+from nonebot.adapters.qqguild.message import BaseMessage
 from nonebot.adapters.qqguild.message import Embed as _Embed
-from nonebot.adapters.qqguild.message import Ark as _Ark
+from nonebot.adapters.qqguild.message import Emoji as _Emoji
 from nonebot.adapters.qqguild.message import LocalImage as _LocalImage
+from nonebot.adapters.qqguild.message import MentionChannel as _MentionChannel
+from nonebot.adapters.qqguild.message import MentionEveryone as _MentionEveryone
+from nonebot.adapters.qqguild.message import MentionUser as _MentionUser
+from nonebot.adapters.qqguild.message import Message, MessageSegment
 from nonebot.adapters.qqguild.message import Reference as _Reference
 from nonebot_plugin_alconna.argv import MessageArgv
-from arclet.alconna import set_default_argv_type, argv_config
+from nonebot_plugin_alconna.typings import SegmentPattern
 
 
 class QQGuildMessageArgv(MessageArgv):
     ...
 
 
 set_default_argv_type(QQGuildMessageArgv)
```

### Comparing `nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/telegram.py` & `nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/adapters/telegram.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,19 @@
-from nonebot_plugin_alconna.typings import SegmentPattern
-from nonebot_plugin_alconna.argv import MessageArgv
-from arclet.alconna import set_default_argv_type, argv_config
-from nonebot.adapters.telegram.message import MessageSegment, Message, BaseMessage
-from nonebot.adapters.telegram.message import Entity, File, UnCombinFile
+from arclet.alconna import argv_config, set_default_argv_type
 from nepattern import UnionPattern
+from nonebot.adapters.telegram.message import (
+    BaseMessage,
+    Entity,
+    File,
+    Message,
+    MessageSegment,
+    UnCombinFile,
+)
+from nonebot_plugin_alconna.argv import MessageArgv
+from nonebot_plugin_alconna.typings import SegmentPattern
 
 
 class TelegramMessageArgv(MessageArgv):
     ...
 
 
 def is_text(x: MessageSegment):
```

### Comparing `nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/argv.py` & `nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/argv.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 
-from arclet.alconna.argv import set_default_argv_type, argv_config
 from arclet.alconna._internal._argv import Argv
-
+from arclet.alconna.argv import argv_config, set_default_argv_type
 from nonebot.adapters import Message
 
 
 class MessageArgv(Argv[Message]):
     @staticmethod
     def generate_token(data: list) -> int:
         return hash("".join(i.__repr__() for i in data))
```

### Comparing `nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/matcher.py` & `nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/matcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
 from arclet.alconna import Alconna, command_manager
-from arclet.alconna.tools import AlconnaString
+from arclet.alconna.tools import AlconnaFormat
 from nonebot.matcher import Matcher
 from nonebot.plugin.on import on_message
 from nonebot.rule import Rule
 from nonebot.typing import T_RuleChecker
 
-from .rule import alconna
 from .model import CompConfig
+from .rule import alconna
 from .typings import TConvert
 
 
 def on_alconna(
     command: Alconna | str,
     rule: Rule | T_RuleChecker | None = None,
     skip_for_unmatch: bool = True,
@@ -39,15 +39,15 @@
         temp: 是否为临时事件响应器（仅执行一次）
         expire_time: 事件响应器最终有效时间点，过时即被删除
         priority: 事件响应器优先级
         block: 是否阻止事件向更低优先级传递
         state: 默认 state
     """
     if isinstance(command, str):
-        command = AlconnaString(command)
+        command = AlconnaFormat(command)
     if aliases and command.command:
         command_manager.delete(command)
         aliases.add(str(command.command))
         command.command = "re:(" + "|".join(aliases) + ")"
         command._hash = command._calc_hash()
         command_manager.register(command)
     return on_message(
```

### Comparing `nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/matcher.pyi` & `nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/matcher.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 
 from arclet.alconna import Alconna
 from nonebot.dependencies import Dependent
 from nonebot.matcher import Matcher
 from nonebot.permission import Permission
 from nonebot.rule import Rule
 from nonebot.typing import T_Handler, T_PermissionChecker, T_RuleChecker, T_State
-from nonebot_plugin_alconna.typings import TConvert
 from nonebot_plugin_alconna.model import CompConfig
-
+from nonebot_plugin_alconna.typings import TConvert
 
 def on_alconna(
     command: Alconna | str,
     rule: Rule | T_RuleChecker | None = None,
     skip_for_unmatch: bool = True,
     auto_send_output: bool = False,
     output_converter: TConvert | None = None,
```

### Comparing `nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/model.py` & `nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass, field
-from typing import Generic, TypeVar, Optional, TypedDict
+from typing import Generic, Optional, TypedDict, TypeVar
 from typing_extensions import NotRequired
 
-from arclet.alconna import Arparma, Empty, Alconna
+from arclet.alconna import Alconna, Arparma, Empty
 from arclet.alconna.duplication import Duplication
 
 T = TypeVar("T")
 T_Duplication = TypeVar("T_Duplication", bound=Duplication)
 
 
 @dataclass
```

### Comparing `nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/params.py` & `nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/params.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Type, TypeVar, overload, Any, Callable
+from typing import Any, Callable, Optional, Type, TypeVar, overload
 from typing_extensions import Annotated
 
 from arclet.alconna import Arparma, Duplication, Empty
 from arclet.alconna.builtin import generate_duplication
 from nonebot.internal.matcher import Matcher as Matcher
 from nonebot.internal.params import Depends as Depends
 from nonebot.typing import T_State
```

### Comparing `nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/rule.py` & `nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import asyncio
-from typing import ClassVar, Optional, Union, Dict
+import traceback
+from typing import ClassVar, Dict, Optional, Union
 
 from arclet.alconna import (
     Alconna,
-    Arparma,
+    AllParam,
     Args,
+    Arparma,
+    CommandMeta,
     CompSession,
-    AllParam,
     command_manager,
     output_manager,
-    CommandMeta
 )
-import traceback
 from arclet.alconna.exceptions import SpecialOptionTriggered
 from nonebot import get_driver
 from nonebot.adapters import Bot, Event, Message
 from nonebot.internal.matcher import matchers
 from nonebot.internal.rule import Rule as Rule
-from nonebot.plugin.on import on_message
 from nonebot.params import EventMessage
+from nonebot.plugin.on import on_message
 from nonebot.typing import T_State
 from nonebot.utils import is_coroutine_callable, run_sync
 from tarina import lang
 
 from .config import Config
 from .consts import ALCONNA_RESULT
 from .model import CommandResult, CompConfig
```

### Comparing `nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/typings.py` & `nonebot-plugin-alconna-0.7.0/src/nonebot_plugin_alconna/typings.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
-from typing import Callable, Any, TypeVar, Generic, Literal, Awaitable, Union
+from typing import Any, Awaitable, Callable, Generic, Literal, TypeVar, Union
 from typing_extensions import ParamSpec, TypeAlias
+
+from nepattern import BasePattern, MatchFailed, PatternModel
+from nonebot.internal.adapter.message import Message, MessageSegment
 from tarina import lang
-from nepattern import BasePattern, PatternModel, MatchFailed
-from nonebot.internal.adapter.message import MessageSegment, Message
 
 TMS = TypeVar("TMS", bound=MessageSegment)
 P = ParamSpec("P")
 
 
 class SegmentPattern(BasePattern[TMS], Generic[TMS, P]):
     def __init__(
```

### Comparing `nonebot-plugin-alconna-0.6.1/PKG-INFO` & `nonebot-plugin-alconna-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-alconna
-Version: 0.6.1
+Version: 0.7.0
 Summary: Alconna Adapter for Nonebot
 License: MIT
 Keywords: command,argparse,cli,alconna,nonebot
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 Requires-Python: >=3.8
 Project-URL: repository, https://github.com/ArcletProject/nonebot-plugin-alconna
 Description-Content-Type: text/markdown
@@ -45,14 +45,17 @@
 ## 讨论
 
 QQ 交流群: [链接](https://jq.qq.com/?_wv=1027&k=PUPOnCSH)
 
 
 ## 使用方法
 
+Nonebot文档: [📖这里](https://nonebot.dev/docs/advanced/matcher#alconna)
+详细介绍: [📦这里](/docs.md)
+
 ### 消息解析
 
 ```python
 from nonebot.adapters.onebot.v12 import Message, MessageSegment
 from arclet.alconna import Alconna, Option, Args
 
 msg = Message("Hello! --foo 123")
```

