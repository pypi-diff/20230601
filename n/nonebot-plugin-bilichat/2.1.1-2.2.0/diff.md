# Comparing `tmp/nonebot_plugin_bilichat-2.1.1.tar.gz` & `tmp/nonebot_plugin_bilichat-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilichat-2.1.1.tar", last modified: Thu Jun  1 09:16:10 2023, max compression
+gzip compressed data, was "nonebot_plugin_bilichat-2.2.0.tar", last modified: Thu Jun  1 15:18:15 2023, max compression
```

## Comparing `nonebot_plugin_bilichat-2.1.1.tar` & `nonebot_plugin_bilichat-2.2.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    34523 2023-06-01 09:15:55.218753 nonebot_plugin_bilichat-2.1.1/LICENSE
--rw-r--r--   0        0        0    11827 2023-06-01 09:15:55.218753 nonebot_plugin_bilichat-2.1.1/README.md
--rw-r--r--   0        0        0     8268 2023-06-01 09:15:55.226753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/__init__.py
--rw-r--r--   0        0        0     4805 2023-06-01 09:15:55.226753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/config.py
--rw-r--r--   0        0        0      513 2023-06-01 09:15:55.226753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/lib/b23_extract.py
--rw-r--r--   0        0        0     6226 2023-06-01 09:15:55.226753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/lib/bcut_asr.py
--rw-r--r--   0        0        0     4806 2023-06-01 09:15:55.226753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/lib/bilibili_request.py
--rw-r--r--   0        0        0      871 2023-06-01 09:15:55.226753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/lib/column_resolve.py
--rw-r--r--   0        0        0     6439 2023-06-01 09:15:55.226753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/lib/content_resolve.py
--rw-r--r--   0        0        0     8900 2023-06-01 09:15:55.226753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/lib/draw_bili_image.py
--rw-r--r--   0        0        0     3800 2023-06-01 09:15:55.226753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/lib/fonts_provider.py
--rw-r--r--   0        0        0      399 2023-06-01 09:15:55.226753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/lib/store.py
--rw-r--r--   0        0        0     1868 2023-06-01 09:15:55.230753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/lib/strings.py
--rw-r--r--   0        0        0     4102 2023-06-01 09:15:55.230753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/lib/video_subtitle.py
--rw-r--r--   0        0        0      341 2023-06-01 09:15:55.230753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/model/arguments.py
--rw-r--r--   0        0        0     2854 2023-06-01 09:15:55.230753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/model/bcut_asr.py
--rw-r--r--   0        0        0     1127 2023-06-01 09:15:55.230753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/model/cache.py
--rw-r--r--   0        0        0      387 2023-06-01 09:15:55.230753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/model/content.py
--rw-r--r--   0        0        0      503 2023-06-01 09:15:55.230753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/model/exception.py
--rw-r--r--   0        0        0    27359 2023-06-01 09:15:55.230753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/model/newbing.py
--rw-r--r--   0        0        0      323 2023-06-01 09:15:55.230753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/model/openai.py
--rw-r--r--   0        0        0      261 2023-06-01 09:15:55.230753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/optional.py
--rw-r--r--   0        0        0   248896 2023-06-01 09:15:55.230753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/static/bing_apology.jpg
--rw-r--r--   0        0        0     1363 2023-06-01 09:15:55.230753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/summary/__init__.py
--rw-r--r--   0        0        0     5825 2023-06-01 09:15:55.230753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/summary/newbing_summarise.py
--rw-r--r--   0        0        0     4916 2023-06-01 09:15:55.230753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/summary/openai.py
--rw-r--r--   0        0        0     2343 2023-06-01 09:15:55.230753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/summary/openai_summarise.py
--rw-r--r--   0        0        0     1448 2023-06-01 09:15:55.230753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/summary/text_to_image.py
--rw-r--r--   0        0        0     1780 2023-06-01 09:15:55.230753 nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/wordcloud/wordcloud.py
--rw-r--r--   0        0        0     1470 2023-06-01 09:16:10.054911 nonebot_plugin_bilichat-2.1.1/pyproject.toml
--rw-r--r--   0        0        0    13195 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-01 15:18:03.956801 nonebot_plugin_bilichat-2.2.0/LICENSE
+-rw-r--r--   0        0        0    11979 2023-06-01 15:18:03.956801 nonebot_plugin_bilichat-2.2.0/README.md
+-rw-r--r--   0        0        0     8467 2023-06-01 15:18:03.964801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/__init__.py
+-rw-r--r--   0        0        0     4842 2023-06-01 15:18:03.964801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/config.py
+-rw-r--r--   0        0        0      513 2023-06-01 15:18:03.964801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/lib/b23_extract.py
+-rw-r--r--   0        0        0     6226 2023-06-01 15:18:03.964801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/lib/bcut_asr.py
+-rw-r--r--   0        0        0     4806 2023-06-01 15:18:03.964801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/lib/bilibili_request.py
+-rw-r--r--   0        0        0      871 2023-06-01 15:18:03.964801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/lib/column_resolve.py
+-rw-r--r--   0        0        0     6439 2023-06-01 15:18:03.964801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/lib/content_resolve.py
+-rw-r--r--   0        0        0     8900 2023-06-01 15:18:03.964801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/lib/draw_bili_image.py
+-rw-r--r--   0        0        0     3800 2023-06-01 15:18:03.964801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/lib/fonts_provider.py
+-rw-r--r--   0        0        0      399 2023-06-01 15:18:03.964801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/lib/store.py
+-rw-r--r--   0        0        0     1868 2023-06-01 15:18:03.964801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/lib/strings.py
+-rw-r--r--   0        0        0     4102 2023-06-01 15:18:03.964801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/lib/video_subtitle.py
+-rw-r--r--   0        0        0      341 2023-06-01 15:18:03.964801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/model/arguments.py
+-rw-r--r--   0        0        0     2854 2023-06-01 15:18:03.964801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/model/bcut_asr.py
+-rw-r--r--   0        0        0     1127 2023-06-01 15:18:03.964801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/model/cache.py
+-rw-r--r--   0        0        0      387 2023-06-01 15:18:03.964801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/model/content.py
+-rw-r--r--   0        0        0      503 2023-06-01 15:18:03.964801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/model/exception.py
+-rw-r--r--   0        0        0    27359 2023-06-01 15:18:03.968801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/model/newbing.py
+-rw-r--r--   0        0        0      323 2023-06-01 15:18:03.968801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/model/openai.py
+-rw-r--r--   0        0        0      261 2023-06-01 15:18:03.968801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/optional.py
+-rw-r--r--   0        0        0   248896 2023-06-01 15:18:03.968801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/static/bing_apology.jpg
+-rw-r--r--   0        0        0     1363 2023-06-01 15:18:03.968801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/summary/__init__.py
+-rw-r--r--   0        0        0     5825 2023-06-01 15:18:03.968801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/summary/newbing_summarise.py
+-rw-r--r--   0        0        0     4916 2023-06-01 15:18:03.968801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/summary/openai.py
+-rw-r--r--   0        0        0     2343 2023-06-01 15:18:03.968801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/summary/openai_summarise.py
+-rw-r--r--   0        0        0     1448 2023-06-01 15:18:03.968801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/summary/text_to_image.py
+-rw-r--r--   0        0        0     1780 2023-06-01 15:18:03.968801 nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py
+-rw-r--r--   0        0        0     1470 2023-06-01 15:18:15.592819 nonebot_plugin_bilichat-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0    13347 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-2.2.0/PKG-INFO
```

### Comparing `nonebot_plugin_bilichat-2.1.1/LICENSE` & `nonebot_plugin_bilichat-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.1.1/README.md` & `nonebot_plugin_bilichat-2.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -140,14 +140,15 @@
 ### 通用配置项
 
 | 配置项 | 类型 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
 | bilichat_block              | bool      | False | 是否拦截事件(防止其他插件二次解析) |
 | bilichat_enable_private     | bool      | True  | 是否允许响应私聊 |
 | bilichat_enable_self        | bool      | False | 是否允许响应自身的消息 |
+| bilichat_only_self          | bool      | False | 是否仅响应自身的消息，开启后会**覆盖全部其他规则**（人机合一特供） |
 | bilichat_enable_channel     | bool      | True  | 是否允许响应频道的消息 |
 | bilichat_enable_unkown_src  | bool      | False | 是否允许响应未知来源的消息 |
 | bilichat_whitelist          | list[str] | []    | **响应**的群聊(频道)名单, 会覆盖黑名单 |
 | bilichat_blacklist          | list[str] | []    | **不响应**的群聊(频道)名单 |
 | bilichat_dynamic_font       | str       | None  | 视频信息及词云图片使用的字体 |
 | bilichat_cd_time            | int       | 120   | 对同一视频的响应冷却时间(防止刷屏) |
 | bilichat_neterror_retry     | int       | 3     | 对部分网络请求错误的尝试次数 |
```

#### html2text {}

```diff
@@ -31,19 +31,21 @@
 æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
 ["nonebot_plugin_bilichat"]  ## âï¸ éç½® å¨ nonebot2
 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çéç½®, éç½®åä¸º**éå¿é¡»é¡¹**
 ### éç¨éç½®é¡¹ | éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | |:-----:|:----:
 |:----:|:----:| | bilichat_block | bool | False | æ¯å¦æ¦æªäºä»¶
 (é²æ­¢å¶ä»æä»¶äºæ¬¡è§£æ) | | bilichat_enable_private | bool | True |
 æ¯å¦åè®¸ååºç§è | | bilichat_enable_self | bool | False |
-æ¯å¦åè®¸ååºèªèº«çæ¶æ¯ | | bilichat_enable_channel | bool | True |
-æ¯å¦åè®¸ååºé¢éçæ¶æ¯ | | bilichat_enable_unkown_src | bool | False
-| æ¯å¦åè®¸ååºæªç¥æ¥æºçæ¶æ¯ | | bilichat_whitelist | list[str] |
-[] | **ååº**çç¾¤è(é¢é)åå, ä¼è¦çé»åå | |
-bilichat_blacklist | list[str] | [] | **ä¸ååº**çç¾¤è(é¢é)åå | |
+æ¯å¦åè®¸ååºèªèº«çæ¶æ¯ | | bilichat_only_self | bool | False |
+æ¯å¦ä»ååºèªèº«çæ¶æ¯ï¼å¼å¯åä¼**è¦çå¨é¨å¶ä»è§å**ï¼äººæºåä¸ç¹ä¾ï¼
+| | bilichat_enable_channel | bool | True | æ¯å¦åè®¸ååºé¢éçæ¶æ¯ |
+| bilichat_enable_unkown_src | bool | False |
+æ¯å¦åè®¸ååºæªç¥æ¥æºçæ¶æ¯ | | bilichat_whitelist | list[str] | []
+| **ååº**çç¾¤è(é¢é)åå, ä¼è¦çé»åå | | bilichat_blacklist
+| list[str] | [] | **ä¸ååº**çç¾¤è(é¢é)åå | |
 bilichat_dynamic_font | str | None | è§é¢ä¿¡æ¯åè¯äºå¾çä½¿ç¨çå­ä½
 | | bilichat_cd_time | int | 120 | å¯¹åä¸è§é¢çååºå·å´æ¶é´
 (é²æ­¢å·å±) | | bilichat_neterror_retry | int | 3 |
 å¯¹é¨åç½ç»è¯·æ±éè¯¯çå°è¯æ¬¡æ° | | bilichat_use_bcut_asr | bool |
 True | æ¯å¦å¨**æ²¡æå­å¹æ¶**è°ç¨å¿åªæ¥å£çæå­å¹ | æ³¨: 1.
 ç±äº OneBot
 åè®®æªè§å®æ¯å¦åºä¸æ¥èªèº«äºä»¶ï¼å æ­¤å¨ä¸åçåºæ¯ä¸è½å¦è·åèªèº«äºä»¶å¹¶ä¸ä¸å®ï¼`bilichat_enable_self`
```

### Comparing `nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/__init__.py` & `nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,21 @@
         "priority": 1,
     },
 )
 
 
 async def _bili_check(bot: BOT, event: MESSAGE_EVENT, state: T_State):
     # check if self msg
-    if str(event.get_user_id()) == str(bot.self_id) and not plugin_config.bilichat_enable_self:
+    if str(event.get_user_id()) == str(bot.self_id):
+        if plugin_config.bilichat_only_self:
+            state["_uid_"] = event.get_session_id()
+            return True
+        elif not plugin_config.bilichat_enable_self:
+            return False
+    elif plugin_config.bilichat_only_self:
         return False
     # private msg use user id
     if isinstance(event, (V11_PME, V12_PME, Mirai_PME)):
         state["_uid_"] = event.get_user_id()
         return plugin_config.bilichat_enable_private
     # group msg use group id
     elif isinstance(event, (V11_GME, V12_GME)):
```

### Comparing `nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/config.py` & `nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 
 class Config(BaseModel):
     # general
     bilichat_block: bool = False
     bilichat_enable_private: bool = True
     bilichat_enable_self: bool = False
+    bilichat_only_self: bool = False
     bilichat_enable_channel: bool = True
     bilichat_enable_unkown_src: bool = False
     bilichat_whitelist: List[str] = []
     bilichat_blacklist: List[str] = []
     bilichat_dynamic_font: Optional[str]
     bilichat_cd_time: int = 120
     bilichat_neterror_retry = 3
```

### Comparing `nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/lib/b23_extract.py` & `nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/lib/b23_extract.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/lib/bcut_asr.py` & `nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/lib/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/lib/bilibili_request.py` & `nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/lib/bilibili_request.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/lib/column_resolve.py` & `nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/lib/column_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/lib/content_resolve.py` & `nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/lib/content_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/lib/draw_bili_image.py` & `nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/lib/draw_bili_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/lib/fonts_provider.py` & `nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/lib/fonts_provider.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/lib/strings.py` & `nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/lib/strings.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/lib/video_subtitle.py` & `nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/lib/video_subtitle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/model/bcut_asr.py` & `nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/model/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/model/cache.py` & `nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/model/cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/model/newbing.py` & `nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/model/newbing.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/static/bing_apology.jpg` & `nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/static/bing_apology.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/summary/__init__.py` & `nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/summary/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/summary/newbing_summarise.py` & `nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/summary/newbing_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/summary/openai.py` & `nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/summary/openai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/summary/openai_summarise.py` & `nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/summary/openai_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/summary/text_to_image.py` & `nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/summary/text_to_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.1.1/nonebot_plugin_bilichat/wordcloud/wordcloud.py` & `nonebot_plugin_bilichat-2.2.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.1.1/pyproject.toml` & `nonebot_plugin_bilichat-2.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "py311",
 ]
 include = "\\.pyi?$"
 extend-exclude = ""
 
 [project]
 name = "nonebot-plugin-bilichat"
-version = "2.1.1"
+version = "2.2.0"
 description = "一个通过 OpenAI 来对b站视频进行总结插件"
 authors = [
     { name = "djkcyl", email = "cyl@cyllive.cn" },
     { name = "Well404", email = "well_404@outlook.com" },
 ]
 dependencies = [
     "httpx>=0.23.3",
```

### Comparing `nonebot_plugin_bilichat-2.1.1/PKG-INFO` & `nonebot_plugin_bilichat-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilichat
-Version: 2.1.1
+Version: 2.2.0
 Summary: 一个通过 OpenAI 来对b站视频进行总结插件
 Author-Email: djkcyl <cyl@cyllive.cn>, Well404 <well_404@outlook.com>
 License: AGPL3.0
 Requires-Python: <4.0,>=3.8
 Requires-Dist: httpx>=0.23.3
 Requires-Dist: bilireq>=0.2.4
 Requires-Dist: qrcode>=7.4.2
@@ -175,14 +175,15 @@
 ### 通用配置项
 
 | 配置项 | 类型 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
 | bilichat_block              | bool      | False | 是否拦截事件(防止其他插件二次解析) |
 | bilichat_enable_private     | bool      | True  | 是否允许响应私聊 |
 | bilichat_enable_self        | bool      | False | 是否允许响应自身的消息 |
+| bilichat_only_self          | bool      | False | 是否仅响应自身的消息，开启后会**覆盖全部其他规则**（人机合一特供） |
 | bilichat_enable_channel     | bool      | True  | 是否允许响应频道的消息 |
 | bilichat_enable_unkown_src  | bool      | False | 是否允许响应未知来源的消息 |
 | bilichat_whitelist          | list[str] | []    | **响应**的群聊(频道)名单, 会覆盖黑名单 |
 | bilichat_blacklist          | list[str] | []    | **不响应**的群聊(频道)名单 |
 | bilichat_dynamic_font       | str       | None  | 视频信息及词云图片使用的字体 |
 | bilichat_cd_time            | int       | 120   | 对同一视频的响应冷却时间(防止刷屏) |
 | bilichat_neterror_retry     | int       | 3     | 对部分网络请求错误的尝试次数 |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 2.1.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 2.2.0 Summary:
 ä¸ä¸ªéè¿ OpenAI æ¥å¯¹bç«è§é¢è¿è¡æ»ç»æä»¶ Author-Email: djkcyl
 cyllive.cn>, Well404
 outlook.com> License: AGPL3.0 Requires-Python: <4.0,>=3.8 Requires-Dist:
 httpx>=0.23.3 Requires-Dist: bilireq>=0.2.4 Requires-Dist: qrcode>=7.4.2
 Requires-Dist: pillow>=9.5.0 Requires-Dist: lxml>=4.9.2 Requires-Dist: nonebot-
 plugin-localstore>=0.4.1 Requires-Dist: nonebot-adapter-onebot>=2.2.2 Requires-
 Dist: nonebot-plugin-segbuilder>=0.2.0 Requires-Dist: nonebot2>=2.0.0 Requires-
@@ -50,19 +50,21 @@
 æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
 ["nonebot_plugin_bilichat"]  ## âï¸ éç½® å¨ nonebot2
 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çéç½®, éç½®åä¸º**éå¿é¡»é¡¹**
 ### éç¨éç½®é¡¹ | éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | |:-----:|:----:
 |:----:|:----:| | bilichat_block | bool | False | æ¯å¦æ¦æªäºä»¶
 (é²æ­¢å¶ä»æä»¶äºæ¬¡è§£æ) | | bilichat_enable_private | bool | True |
 æ¯å¦åè®¸ååºç§è | | bilichat_enable_self | bool | False |
-æ¯å¦åè®¸ååºèªèº«çæ¶æ¯ | | bilichat_enable_channel | bool | True |
-æ¯å¦åè®¸ååºé¢éçæ¶æ¯ | | bilichat_enable_unkown_src | bool | False
-| æ¯å¦åè®¸ååºæªç¥æ¥æºçæ¶æ¯ | | bilichat_whitelist | list[str] |
-[] | **ååº**çç¾¤è(é¢é)åå, ä¼è¦çé»åå | |
-bilichat_blacklist | list[str] | [] | **ä¸ååº**çç¾¤è(é¢é)åå | |
+æ¯å¦åè®¸ååºèªèº«çæ¶æ¯ | | bilichat_only_self | bool | False |
+æ¯å¦ä»ååºèªèº«çæ¶æ¯ï¼å¼å¯åä¼**è¦çå¨é¨å¶ä»è§å**ï¼äººæºåä¸ç¹ä¾ï¼
+| | bilichat_enable_channel | bool | True | æ¯å¦åè®¸ååºé¢éçæ¶æ¯ |
+| bilichat_enable_unkown_src | bool | False |
+æ¯å¦åè®¸ååºæªç¥æ¥æºçæ¶æ¯ | | bilichat_whitelist | list[str] | []
+| **ååº**çç¾¤è(é¢é)åå, ä¼è¦çé»åå | | bilichat_blacklist
+| list[str] | [] | **ä¸ååº**çç¾¤è(é¢é)åå | |
 bilichat_dynamic_font | str | None | è§é¢ä¿¡æ¯åè¯äºå¾çä½¿ç¨çå­ä½
 | | bilichat_cd_time | int | 120 | å¯¹åä¸è§é¢çååºå·å´æ¶é´
 (é²æ­¢å·å±) | | bilichat_neterror_retry | int | 3 |
 å¯¹é¨åç½ç»è¯·æ±éè¯¯çå°è¯æ¬¡æ° | | bilichat_use_bcut_asr | bool |
 True | æ¯å¦å¨**æ²¡æå­å¹æ¶**è°ç¨å¿åªæ¥å£çæå­å¹ | æ³¨: 1.
 ç±äº OneBot
 åè®®æªè§å®æ¯å¦åºä¸æ¥èªèº«äºä»¶ï¼å æ­¤å¨ä¸åçåºæ¯ä¸è½å¦è·åèªèº«äºä»¶å¹¶ä¸ä¸å®ï¼`bilichat_enable_self`
```

