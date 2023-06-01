# Comparing `tmp/nonebot_plugin_bilichat-2.1.0.tar.gz` & `tmp/nonebot_plugin_bilichat-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilichat-2.1.0.tar", last modified: Mon May 29 06:30:09 2023, max compression
+gzip compressed data, was "nonebot_plugin_bilichat-2.1.1.tar", last modified: Thu Jun  1 09:16:10 2023, max compression
```

## Comparing `nonebot_plugin_bilichat-2.1.0.tar` & `nonebot_plugin_bilichat-2.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    34523 2023-05-29 06:29:57.137055 nonebot_plugin_bilichat-2.1.0/LICENSE
--rw-r--r--   0        0        0    11827 2023-05-29 06:29:57.137055 nonebot_plugin_bilichat-2.1.0/README.md
--rw-r--r--   0        0        0     8102 2023-05-29 06:29:57.145055 nonebot_plugin_bilichat-2.1.0/nonebot_plugin_bilichat/__init__.py
--rw-r--r--   0        0        0     4805 2023-05-29 06:29:57.145055 nonebot_plugin_bilichat-2.1.0/nonebot_plugin_bilichat/config.py
--rw-r--r--   0        0        0      513 2023-05-29 06:29:57.145055 nonebot_plugin_bilichat-2.1.0/nonebot_plugin_bilichat/lib/b23_extract.py
--rw-r--r--   0        0        0     6226 2023-05-29 06:29:57.145055 nonebot_plugin_bilichat-2.1.0/nonebot_plugin_bilichat/lib/bcut_asr.py
--rw-r--r--   0        0        0     4806 2023-05-29 06:29:57.145055 nonebot_plugin_bilichat-2.1.0/nonebot_plugin_bilichat/lib/bilibili_request.py
--rw-r--r--   0        0        0      871 2023-05-29 06:29:57.145055 nonebot_plugin_bilichat-2.1.0/nonebot_plugin_bilichat/lib/column_resolve.py
--rw-r--r--   0        0        0     6439 2023-05-29 06:29:57.145055 nonebot_plugin_bilichat-2.1.0/nonebot_plugin_bilichat/lib/content_resolve.py
--rw-r--r--   0        0        0     8900 2023-05-29 06:29:57.145055 nonebot_plugin_bilichat-2.1.0/nonebot_plugin_bilichat/lib/draw_bili_image.py
--rw-r--r--   0        0        0     3800 2023-05-29 06:29:57.145055 nonebot_plugin_bilichat-2.1.0/nonebot_plugin_bilichat/lib/fonts_provider.py
--rw-r--r--   0        0        0      399 2023-05-29 06:29:57.145055 nonebot_plugin_bilichat-2.1.0/nonebot_plugin_bilichat/lib/store.py
--rw-r--r--   0        0        0     1868 2023-05-29 06:29:57.145055 nonebot_plugin_bilichat-2.1.0/nonebot_plugin_bilichat/lib/strings.py
--rw-r--r--   0        0        0     4102 2023-05-29 06:29:57.145055 nonebot_plugin_bilichat-2.1.0/nonebot_plugin_bilichat/lib/video_subtitle.py
--rw-r--r--   0        0        0      341 2023-05-29 06:29:57.145055 nonebot_plugin_bilichat-2.1.0/nonebot_plugin_bilichat/model/arguments.py
--rw-r--r--   0        0        0     2854 2023-05-29 06:29:57.145055 nonebot_plugin_bilichat-2.1.0/nonebot_plugin_bilichat/model/bcut_asr.py
--rw-r--r--   0        0        0     1127 2023-05-29 06:29:57.145055 nonebot_plugin_bilichat-2.1.0/nonebot_plugin_bilichat/model/cache.py
--rw-r--r--   0        0        0      387 2023-05-29 06:29:57.145055 nonebot_plugin_bilichat-2.1.0/nonebot_plugin_bilichat/model/content.py
--rw-r--r--   0        0        0      503 2023-05-29 06:29:57.145055 nonebot_plugin_bilichat-2.1.0/nonebot_plugin_bilichat/model/exception.py
--rw-r--r--   0        0        0    27359 2023-05-29 06:29:57.149055 nonebot_plugin_bilichat-2.1.0/nonebot_plugin_bilichat/model/newbing.py
--rw-r--r--   0        0        0      323 2023-05-29 06:29:57.149055 nonebot_plugin_bilichat-2.1.0/nonebot_plugin_bilichat/model/openai.py
--rw-r--r--   0        0        0      261 2023-05-29 06:29:57.149055 nonebot_plugin_bilichat-2.1.0/nonebot_plugin_bilichat/optional.py
--rw-r--r--   0        0        0   248896 2023-05-29 06:29:57.149055 nonebot_plugin_bilichat-2.1.0/nonebot_plugin_bilichat/static/bing_apology.jpg
--rw-r--r--   0        0        0     1363 2023-05-29 06:29:57.149055 nonebot_plugin_bilichat-2.1.0/nonebot_plugin_bilichat/summary/__init__.py
--rw-r--r--   0        0        0     5825 2023-05-29 06:29:57.149055 nonebot_plugin_bilichat-2.1.0/nonebot_plugin_bilichat/summary/newbing_summarise.py
--rw-r--r--   0        0        0     4916 2023-05-29 06:29:57.149055 nonebot_plugin_bilichat-2.1.0/nonebot_plugin_bilichat/summary/openai.py
--rw-r--r--   0        0        0     2343 2023-05-29 06:29:57.149055 nonebot_plugin_bilichat-2.1.0/nonebot_plugin_bilichat/summary/openai_summarise.py
--rw-r--r--   0        0        0     1448 2023-05-29 06:29:57.149055 nonebot_plugin_bilichat-2.1.0/nonebot_plugin_bilichat/summary/text_to_image.py
--rw-r--r--   0        0        0     1780 2023-05-29 06:29:57.149055 nonebot_plugin_bilichat-2.1.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py
--rw-r--r--   0        0        0     1447 2023-05-29 06:30:09.097490 nonebot_plugin_bilichat-2.1.0/pyproject.toml
--rw-r--r--   0        0        0    13164 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-01 09:15:55.218753 nonebot_plugin_bilichat-2.1.1/LICENSE
+-rw-r--r--   0        0        0    11827 2023-06-01 09:15:55.218753 nonebot_plugin_bilichat-2.1.1/README.md
+-rw-r--r--   0        0        0     8268 2023-06-01 09:15:55.226753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/__init__.py
+-rw-r--r--   0        0        0     4805 2023-06-01 09:15:55.226753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/config.py
+-rw-r--r--   0        0        0      513 2023-06-01 09:15:55.226753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/lib/b23_extract.py
+-rw-r--r--   0        0        0     6226 2023-06-01 09:15:55.226753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/lib/bcut_asr.py
+-rw-r--r--   0        0        0     4806 2023-06-01 09:15:55.226753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/lib/bilibili_request.py
+-rw-r--r--   0        0        0      871 2023-06-01 09:15:55.226753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/lib/column_resolve.py
+-rw-r--r--   0        0        0     6439 2023-06-01 09:15:55.226753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/lib/content_resolve.py
+-rw-r--r--   0        0        0     8900 2023-06-01 09:15:55.226753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/lib/draw_bili_image.py
+-rw-r--r--   0        0        0     3800 2023-06-01 09:15:55.226753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/lib/fonts_provider.py
+-rw-r--r--   0        0        0      399 2023-06-01 09:15:55.226753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/lib/store.py
+-rw-r--r--   0        0        0     1868 2023-06-01 09:15:55.230753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/lib/strings.py
+-rw-r--r--   0        0        0     4102 2023-06-01 09:15:55.230753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/lib/video_subtitle.py
+-rw-r--r--   0        0        0      341 2023-06-01 09:15:55.230753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/model/arguments.py
+-rw-r--r--   0        0        0     2854 2023-06-01 09:15:55.230753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/model/bcut_asr.py
+-rw-r--r--   0        0        0     1127 2023-06-01 09:15:55.230753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/model/cache.py
+-rw-r--r--   0        0        0      387 2023-06-01 09:15:55.230753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/model/content.py
+-rw-r--r--   0        0        0      503 2023-06-01 09:15:55.230753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/model/exception.py
+-rw-r--r--   0        0        0    27359 2023-06-01 09:15:55.230753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/model/newbing.py
+-rw-r--r--   0        0        0      323 2023-06-01 09:15:55.230753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/model/openai.py
+-rw-r--r--   0        0        0      261 2023-06-01 09:15:55.230753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/optional.py
+-rw-r--r--   0        0        0   248896 2023-06-01 09:15:55.230753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/static/bing_apology.jpg
+-rw-r--r--   0        0        0     1363 2023-06-01 09:15:55.230753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/summary/__init__.py
+-rw-r--r--   0        0        0     5825 2023-06-01 09:15:55.230753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/summary/newbing_summarise.py
+-rw-r--r--   0        0        0     4916 2023-06-01 09:15:55.230753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/summary/openai.py
+-rw-r--r--   0        0        0     2343 2023-06-01 09:15:55.230753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/summary/openai_summarise.py
+-rw-r--r--   0        0        0     1448 2023-06-01 09:15:55.230753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/summary/text_to_image.py
+-rw-r--r--   0        0        0     1780 2023-06-01 09:15:55.230753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/wordcloud/wordcloud.py
+-rw-r--r--   0        0        0     1470 2023-06-01 09:16:10.054911 nonebot_plugin_bilichat-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0    13195 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-2.1.1/PKG-INFO
```

### Comparing `nonebot_plugin_bilichat-2.1.0/LICENSE` & `nonebot_plugin_bilichat-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.1.0/README.md` & `nonebot_plugin_bilichat-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.1.0/nonebot_plugin_bilichat/__init__.py` & `nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import contextlib
 import re
 import shlex
 from itertools import chain
-from typing import Union, cast
+from typing import Tuple, Union, cast
 
 from nonebot.adapters import MessageSegment
 from nonebot.adapters.mirai2 import Bot as Mirai_Bot
 from nonebot.adapters.mirai2.event import FriendMessage as Mirai_PME
 from nonebot.adapters.mirai2.event import GroupMessage as Mirai_GME
 from nonebot.adapters.mirai2.event import MessageEvent as Mirai_ME
 from nonebot.adapters.onebot.v11 import Bot as V11_Bot
@@ -16,19 +16,18 @@
 from nonebot.adapters.onebot.v12 import Bot as V12_Bot
 from nonebot.adapters.onebot.v12 import ChannelMessageEvent as V12_CME
 from nonebot.adapters.onebot.v12 import GroupMessageEvent as V12_GME
 from nonebot.adapters.onebot.v12 import MessageEvent as V12_ME
 from nonebot.adapters.onebot.v12 import PrivateMessageEvent as V12_PME
 from nonebot.adapters.qqguild import Bot as QG_Bot
 from nonebot.adapters.qqguild.event import MessageEvent as QG_ME
-from nonebot.consts import REGEX_GROUP, REGEX_STR
 from nonebot.exception import FinishedException
 from nonebot.log import logger
 from nonebot.matcher import Matcher
-from nonebot.params import Depends
+from nonebot.params import Depends, RegexGroup, RegexStr
 from nonebot.plugin import PluginMetadata, on_regex, require
 from nonebot.rule import Rule
 from nonebot.typing import T_State
 
 from .config import __version__, plugin_config
 from .lib.b23_extract import b23_extract
 from .lib.content_resolve import get_column_basic, get_content_cache, get_video_basic
@@ -55,14 +54,16 @@
 
 FUTUER_FUCTIONS = ENABLE_SUMMARY or plugin_config.bilichat_word_cloud
 
 __plugin_meta__ = PluginMetadata(
     name="nonebot-plugin-bilichat",
     description="一个通过 OpenAI 来对b站视频进行总结插件",
     usage="直接发送视频链接即可",
+    homepage="https://github.com/Aunly/nonebot-plugin-bilichat",
+    supported_adapters={"~onebot.v11", "~onebot.v12", "~qqguild", "~mirai2"},
     extra={
         "author": "djkcyl & Well404",
         "version": __version__,
         "priority": 1,
     },
 )
 
@@ -115,21 +116,21 @@
             )
         ),  # type: ignore
         namespace=Options(),
     )[0]
 
 
 @bili.handle()
-async def get_bili_number_re(state: T_State):
-    state["bili_number"] = state[REGEX_STR]
+async def get_bili_number_re(state: T_State, bili_number: str = RegexStr()):
+    state["bili_number"] = bili_number
 
 
 @b23.handle()
-async def get_bili_number_b23(state: T_State):
-    bililink = await b23_extract(state[REGEX_GROUP])
+async def get_bili_number_b23(state: T_State, b23: Tuple = RegexGroup()):
+    bililink = await b23_extract(list(b23))
     if matched := re.search(
         r"av(\d{1,15})|BV(1[A-Za-z0-9]{2}4.1.7[A-Za-z0-9]{2})|cv(\d{1,16})", bililink  # type: ignore
     ):
         state["bili_number"] = matched.group()
     else:
         logger.info(f"{bililink} is not video or column")
         raise FinishedException
```

### Comparing `nonebot_plugin_bilichat-2.1.0/nonebot_plugin_bilichat/config.py` & `nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.1.0/nonebot_plugin_bilichat/lib/b23_extract.py` & `nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/lib/b23_extract.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.1.0/nonebot_plugin_bilichat/lib/bcut_asr.py` & `nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/lib/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.1.0/nonebot_plugin_bilichat/lib/bilibili_request.py` & `nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/lib/bilibili_request.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.1.0/nonebot_plugin_bilichat/lib/column_resolve.py` & `nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/lib/column_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.1.0/nonebot_plugin_bilichat/lib/content_resolve.py` & `nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/lib/content_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.1.0/nonebot_plugin_bilichat/lib/draw_bili_image.py` & `nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/lib/draw_bili_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.1.0/nonebot_plugin_bilichat/lib/fonts_provider.py` & `nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/lib/fonts_provider.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.1.0/nonebot_plugin_bilichat/lib/strings.py` & `nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/lib/strings.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.1.0/nonebot_plugin_bilichat/lib/video_subtitle.py` & `nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/lib/video_subtitle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.1.0/nonebot_plugin_bilichat/model/bcut_asr.py` & `nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/model/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.1.0/nonebot_plugin_bilichat/model/cache.py` & `nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/model/cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.1.0/nonebot_plugin_bilichat/model/newbing.py` & `nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/model/newbing.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.1.0/nonebot_plugin_bilichat/static/bing_apology.jpg` & `nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/static/bing_apology.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.1.0/nonebot_plugin_bilichat/summary/__init__.py` & `nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/summary/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.1.0/nonebot_plugin_bilichat/summary/newbing_summarise.py` & `nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/summary/newbing_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.1.0/nonebot_plugin_bilichat/summary/openai.py` & `nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/summary/openai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.1.0/nonebot_plugin_bilichat/summary/openai_summarise.py` & `nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/summary/openai_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.1.0/nonebot_plugin_bilichat/summary/text_to_image.py` & `nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/summary/text_to_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.1.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py` & `nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/wordcloud/wordcloud.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.1.0/pyproject.toml` & `nonebot_plugin_bilichat-2.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -18,29 +18,30 @@
     "py311",
 ]
 include = "\\.pyi?$"
 extend-exclude = ""
 
 [project]
 name = "nonebot-plugin-bilichat"
-version = "2.1.0"
+version = "2.1.1"
 description = "一个通过 OpenAI 来对b站视频进行总结插件"
 authors = [
     { name = "djkcyl", email = "cyl@cyllive.cn" },
     { name = "Well404", email = "well_404@outlook.com" },
 ]
 dependencies = [
     "httpx>=0.23.3",
     "bilireq>=0.2.4",
     "qrcode>=7.4.2",
     "pillow>=9.5.0",
     "lxml>=4.9.2",
     "nonebot-plugin-localstore>=0.4.1",
     "nonebot-adapter-onebot>=2.2.2",
     "nonebot-plugin-segbuilder>=0.2.0",
+    "nonebot2>=2.0.0",
 ]
 requires-python = ">=3.8,<4.0"
 readme = "README.md"
 
 [project.license]
 text = "AGPL3.0"
```

### Comparing `nonebot_plugin_bilichat-2.1.0/PKG-INFO` & `nonebot_plugin_bilichat-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilichat
-Version: 2.1.0
+Version: 2.1.1
 Summary: 一个通过 OpenAI 来对b站视频进行总结插件
 Author-Email: djkcyl <cyl@cyllive.cn>, Well404 <well_404@outlook.com>
 License: AGPL3.0
 Requires-Python: <4.0,>=3.8
 Requires-Dist: httpx>=0.23.3
 Requires-Dist: bilireq>=0.2.4
 Requires-Dist: qrcode>=7.4.2
 Requires-Dist: pillow>=9.5.0
 Requires-Dist: lxml>=4.9.2
 Requires-Dist: nonebot-plugin-localstore>=0.4.1
 Requires-Dist: nonebot-adapter-onebot>=2.2.2
 Requires-Dist: nonebot-plugin-segbuilder>=0.2.0
+Requires-Dist: nonebot2>=2.0.0
 Requires-Dist: nonebot-plugin-sentry>=0.2.2; extra == "extra"
 Requires-Dist: jieba>=0.42.1; extra == "wordcloud"
 Requires-Dist: wordcloud>=1.8.2.2; extra == "wordcloud"
 Requires-Dist: tiktoken-async>=0.3.2; extra == "openai"
 Requires-Dist: minidynamicrender>=1.1.9; extra == "openai"
 Requires-Dist: EdgeGPT>=0.1.22.1; extra == "newbing"
 Requires-Dist: minidynamicrender>=1.1.9; extra == "newbing"
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 2.1.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 2.1.1 Summary:
 ä¸ä¸ªéè¿ OpenAI æ¥å¯¹bç«è§é¢è¿è¡æ»ç»æä»¶ Author-Email: djkcyl
 cyllive.cn>, Well404
 outlook.com> License: AGPL3.0 Requires-Python: <4.0,>=3.8 Requires-Dist:
 httpx>=0.23.3 Requires-Dist: bilireq>=0.2.4 Requires-Dist: qrcode>=7.4.2
 Requires-Dist: pillow>=9.5.0 Requires-Dist: lxml>=4.9.2 Requires-Dist: nonebot-
 plugin-localstore>=0.4.1 Requires-Dist: nonebot-adapter-onebot>=2.2.2 Requires-
-Dist: nonebot-plugin-segbuilder>=0.2.0 Requires-Dist: nonebot-plugin-
-sentry>=0.2.2; extra == "extra" Requires-Dist: jieba>=0.42.1; extra ==
-"wordcloud" Requires-Dist: wordcloud>=1.8.2.2; extra == "wordcloud" Requires-
-Dist: tiktoken-async>=0.3.2; extra == "openai" Requires-Dist:
-minidynamicrender>=1.1.9; extra == "openai" Requires-Dist: EdgeGPT>=0.1.22.1;
-extra == "newbing" Requires-Dist: minidynamicrender>=1.1.9; extra == "newbing"
-Requires-Dist: jieba>=0.42.1; extra == "all" Requires-Dist: wordcloud>=1.8.2.2;
-extra == "all" Requires-Dist: tiktoken-async>=0.3.2; extra == "all" Requires-
-Dist: EdgeGPT>=0.1.22.1; extra == "all" Requires-Dist:
+Dist: nonebot-plugin-segbuilder>=0.2.0 Requires-Dist: nonebot2>=2.0.0 Requires-
+Dist: nonebot-plugin-sentry>=0.2.2; extra == "extra" Requires-Dist:
+jieba>=0.42.1; extra == "wordcloud" Requires-Dist: wordcloud>=1.8.2.2; extra ==
+"wordcloud" Requires-Dist: tiktoken-async>=0.3.2; extra == "openai" Requires-
+Dist: minidynamicrender>=1.1.9; extra == "openai" Requires-Dist:
+EdgeGPT>=0.1.22.1; extra == "newbing" Requires-Dist: minidynamicrender>=1.1.9;
+extra == "newbing" Requires-Dist: jieba>=0.42.1; extra == "all" Requires-Dist:
+wordcloud>=1.8.2.2; extra == "all" Requires-Dist: tiktoken-async>=0.3.2; extra
+== "all" Requires-Dist: EdgeGPT>=0.1.22.1; extra == "all" Requires-Dist:
 minidynamicrender>=1.1.9; extra == "all" Provides-Extra: extra Provides-Extra:
 wordcloud Provides-Extra: openai Provides-Extra: newbing Provides-Extra: all
 Description-Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
     # nonebot-plugin-bilichat _â¨ å¤åè½çBç«è§é¢è§£æå·¥å· â¨_
 [license] [PyPI_-_Downloads] [pypi] [python] [pdm-managed] [Code_style:_black]
```

