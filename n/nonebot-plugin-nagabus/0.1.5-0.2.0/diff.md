# Comparing `tmp/nonebot_plugin_nagabus-0.1.5.tar.gz` & `tmp/nonebot_plugin_nagabus-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_nagabus-0.1.5.tar", max compression
+gzip compressed data, was "nonebot_plugin_nagabus-0.2.0.tar", max compression
```

## Comparing `nonebot_plugin_nagabus-0.1.5.tar` & `nonebot_plugin_nagabus-0.2.0.tar`

### file list

```diff
@@ -1,35 +1,34 @@
--rw-r--r--   0        0        0    35184 2022-12-04 13:51:12.448000 nonebot_plugin_nagabus-0.1.5/LICENSE
--rw-r--r--   0        0        0     1131 2023-05-28 14:51:33.780852 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/__init__.py
--rw-r--r--   0        0        0      129 2023-05-27 04:29:09.849196 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/ac.py
--rw-r--r--   0        0        0     1197 2023-05-28 14:51:33.775850 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/config.py
--rw-r--r--   0        0        0        4 2023-05-26 13:11:24.775555 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/data/__init__.py
--rw-r--r--   0        0        0      116 2023-05-26 11:41:42.946553 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/data/base.py
--rw-r--r--   0        0        0      317 2023-05-26 11:41:42.956553 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/data/mjs.py
--rw-r--r--   0        0        0     1697 2023-05-27 07:16:52.720509 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/data/naga.py
--rw-r--r--   0        0        0      775 2023-05-26 11:41:42.960551 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/data/session.py
--rw-r--r--   0        0        0      713 2023-05-26 15:21:27.421204 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/data/utils/__init__.py
--rw-r--r--   0        0        0      761 2023-02-13 05:42:01.843000 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/data/utils/utc_datetime.py
--rw-r--r--   0        0        0       43 2023-05-28 14:51:33.785849 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/errors.py
--rw-r--r--   0        0        0       95 2023-05-28 01:19:53.575323 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/matchers/__init__.py
--rw-r--r--   0        0        0      189 2023-05-30 02:32:55.940589 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/matchers/errors.py
--rw-r--r--   0        0        0        0 2023-05-30 02:22:08.333037 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/matchers/interceptors/__init__.py
--rw-r--r--   0        0        0     1090 2023-05-30 02:32:55.906573 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/matchers/interceptors/access_control.py
--rw-r--r--   0        0        0     2392 2023-05-30 02:32:55.934567 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/matchers/interceptors/handle_error.py
--rw-r--r--   0        0        0     4810 2023-05-30 02:36:34.180268 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/matchers/naga_analyze.py
--rw-r--r--   0        0        0     2415 2023-05-30 02:32:55.921568 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/matchers/naga_statistic.py
--rw-r--r--   0        0        0     2278 2023-05-27 02:48:33.707764 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/migrations/24aec3c56623_.py
--rw-r--r--   0        0        0     1350 2023-05-27 07:17:07.623159 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/migrations/ab4d80c20047_.py
--rw-r--r--   0        0        0     1009 2023-05-26 15:21:27.440185 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/mjs/__init__.py
--rw-r--r--   0        0        0      176 2023-05-25 15:39:25.419279 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/naga/__init__.py
--rw-r--r--   0        0        0     3758 2023-05-27 13:45:54.389899 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/naga/api.py
--rw-r--r--   0        0        0     3089 2023-05-29 12:30:46.127834 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/naga/fake_api.py
--rw-r--r--   0        0        0     1066 2023-05-27 02:48:01.485010 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/naga/model.py
--rw-r--r--   0        0        0    20455 2023-05-30 02:38:14.130387 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/naga/service.py
--rw-r--r--   0        0        0        0 2023-05-25 16:04:02.955709 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/utils/__init__.py
--rw-r--r--   0        0        0     1092 2023-05-25 16:06:56.701500 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/utils/integer.py
--rw-r--r--   0        0        0        0 2023-05-26 12:48:40.974521 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/utils/mapping.py
--rw-r--r--   0        0        0      101 2023-05-25 08:09:22.247000 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/utils/nonebot.py
--rw-r--r--   0        0        0       68 2023-05-26 15:50:47.559077 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/utils/tz.py
--rw-r--r--   0        0        0      677 2023-05-30 02:38:28.516027 nonebot_plugin_nagabus-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1789 2023-05-28 03:26:24.309853 nonebot_plugin_nagabus-0.1.5/README.md
--rw-r--r--   0        0        0     2592 1970-01-01 00:00:00.000000 nonebot_plugin_nagabus-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    35184 2022-12-04 13:51:12.448000 nonebot_plugin_nagabus-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1237 2023-06-01 03:26:14.711563 nonebot_plugin_nagabus-0.2.0/nonebot_plugin_nagabus/__init__.py
+-rw-r--r--   0        0        0      129 2023-05-27 04:29:09.849196 nonebot_plugin_nagabus-0.2.0/nonebot_plugin_nagabus/ac.py
+-rw-r--r--   0        0        0     1197 2023-05-28 14:51:33.775850 nonebot_plugin_nagabus-0.2.0/nonebot_plugin_nagabus/config.py
+-rw-r--r--   0        0        0        4 2023-05-26 13:11:24.775555 nonebot_plugin_nagabus-0.2.0/nonebot_plugin_nagabus/data/__init__.py
+-rw-r--r--   0        0        0      116 2023-05-26 11:41:42.946553 nonebot_plugin_nagabus-0.2.0/nonebot_plugin_nagabus/data/base.py
+-rw-r--r--   0        0        0      317 2023-05-26 11:41:42.956553 nonebot_plugin_nagabus-0.2.0/nonebot_plugin_nagabus/data/mjs.py
+-rw-r--r--   0        0        0     1697 2023-06-01 02:59:37.618752 nonebot_plugin_nagabus-0.2.0/nonebot_plugin_nagabus/data/naga.py
+-rw-r--r--   0        0        0      775 2023-05-26 11:41:42.960551 nonebot_plugin_nagabus-0.2.0/nonebot_plugin_nagabus/data/session.py
+-rw-r--r--   0        0        0      713 2023-05-26 15:21:27.421204 nonebot_plugin_nagabus-0.2.0/nonebot_plugin_nagabus/data/utils/__init__.py
+-rw-r--r--   0        0        0      761 2023-02-13 05:42:01.843000 nonebot_plugin_nagabus-0.2.0/nonebot_plugin_nagabus/data/utils/utc_datetime.py
+-rw-r--r--   0        0        0       43 2023-05-28 14:51:33.785849 nonebot_plugin_nagabus-0.2.0/nonebot_plugin_nagabus/errors.py
+-rw-r--r--   0        0        0       95 2023-05-28 01:19:53.575323 nonebot_plugin_nagabus-0.2.0/nonebot_plugin_nagabus/matchers/__init__.py
+-rw-r--r--   0        0        0      189 2023-05-30 02:32:55.940589 nonebot_plugin_nagabus-0.2.0/nonebot_plugin_nagabus/matchers/errors.py
+-rw-r--r--   0        0        0        0 2023-05-30 02:22:08.333037 nonebot_plugin_nagabus-0.2.0/nonebot_plugin_nagabus/matchers/interceptors/__init__.py
+-rw-r--r--   0        0        0     2873 2023-06-01 03:15:37.986641 nonebot_plugin_nagabus-0.2.0/nonebot_plugin_nagabus/matchers/interceptors/handle_error.py
+-rw-r--r--   0        0        0     4828 2023-06-01 03:15:38.024057 nonebot_plugin_nagabus-0.2.0/nonebot_plugin_nagabus/matchers/naga_analyze.py
+-rw-r--r--   0        0        0     2420 2023-06-01 03:34:15.583151 nonebot_plugin_nagabus-0.2.0/nonebot_plugin_nagabus/matchers/naga_statistic.py
+-rw-r--r--   0        0        0     2278 2023-05-27 02:48:33.707764 nonebot_plugin_nagabus-0.2.0/nonebot_plugin_nagabus/migrations/24aec3c56623_.py
+-rw-r--r--   0        0        0     1350 2023-05-27 07:17:07.623159 nonebot_plugin_nagabus-0.2.0/nonebot_plugin_nagabus/migrations/ab4d80c20047_.py
+-rw-r--r--   0        0        0     1009 2023-05-26 15:21:27.440185 nonebot_plugin_nagabus-0.2.0/nonebot_plugin_nagabus/mjs/__init__.py
+-rw-r--r--   0        0        0      176 2023-05-25 15:39:25.419279 nonebot_plugin_nagabus-0.2.0/nonebot_plugin_nagabus/naga/__init__.py
+-rw-r--r--   0        0        0     3758 2023-05-27 13:45:54.389899 nonebot_plugin_nagabus-0.2.0/nonebot_plugin_nagabus/naga/api.py
+-rw-r--r--   0        0        0     3089 2023-05-29 12:30:46.127834 nonebot_plugin_nagabus-0.2.0/nonebot_plugin_nagabus/naga/fake_api.py
+-rw-r--r--   0        0        0     1066 2023-05-27 02:48:01.485010 nonebot_plugin_nagabus-0.2.0/nonebot_plugin_nagabus/naga/model.py
+-rw-r--r--   0        0        0    20455 2023-05-30 02:38:14.130387 nonebot_plugin_nagabus-0.2.0/nonebot_plugin_nagabus/naga/service.py
+-rw-r--r--   0        0        0        0 2023-05-25 16:04:02.955709 nonebot_plugin_nagabus-0.2.0/nonebot_plugin_nagabus/utils/__init__.py
+-rw-r--r--   0        0        0     1092 2023-05-25 16:06:56.701500 nonebot_plugin_nagabus-0.2.0/nonebot_plugin_nagabus/utils/integer.py
+-rw-r--r--   0        0        0        0 2023-05-26 12:48:40.974521 nonebot_plugin_nagabus-0.2.0/nonebot_plugin_nagabus/utils/mapping.py
+-rw-r--r--   0        0        0      101 2023-05-25 08:09:22.247000 nonebot_plugin_nagabus-0.2.0/nonebot_plugin_nagabus/utils/nonebot.py
+-rw-r--r--   0        0        0       68 2023-05-26 15:50:47.559077 nonebot_plugin_nagabus-0.2.0/nonebot_plugin_nagabus/utils/tz.py
+-rw-r--r--   0        0        0      987 2023-06-01 03:30:00.479528 nonebot_plugin_nagabus-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1789 2023-05-28 03:26:24.309853 nonebot_plugin_nagabus-0.2.0/README.md
+-rw-r--r--   0        0        0     2763 1970-01-01 00:00:00.000000 nonebot_plugin_nagabus-0.2.0/PKG-INFO
```

### Comparing `nonebot_plugin_nagabus-0.1.5/LICENSE` & `nonebot_plugin_nagabus-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/__init__.py` & `nonebot_plugin_nagabus-0.2.0/nonebot_plugin_nagabus/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -29,14 +29,17 @@
     description='为群友提供NAGA拼车服务',
     usage=help_text
 )
 
 from nonebot import logger, require
 
 require("nonebot_plugin_access_control")
-require("nonebot_plugin_majsoul")
 require("nonebot_plugin_datastore")
+require("nonebot_plugin_get_nickname")
+require("nonebot_plugin_majsoul")
+require("nonebot_plugin_saa")
+require("nonebot_plugin_session")
 
 try:
     from . import matchers
 except ConfigError as e:
     logger.exception(e)
```

### Comparing `nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/config.py` & `nonebot_plugin_nagabus-0.2.0/nonebot_plugin_nagabus/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/data/naga.py` & `nonebot_plugin_nagabus-0.2.0/nonebot_plugin_nagabus/data/naga.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/data/session.py` & `nonebot_plugin_nagabus-0.2.0/nonebot_plugin_nagabus/data/session.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/data/utils/__init__.py` & `nonebot_plugin_nagabus-0.2.0/nonebot_plugin_nagabus/data/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/data/utils/utc_datetime.py` & `nonebot_plugin_nagabus-0.2.0/nonebot_plugin_nagabus/data/utils/utc_datetime.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/matchers/naga_analyze.py` & `nonebot_plugin_nagabus-0.2.0/nonebot_plugin_nagabus/matchers/naga_analyze.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,84 +1,79 @@
 import re
 from urllib.parse import urlparse, parse_qs
 
-from nonebot import on_command, Bot
-from nonebot.adapters.onebot.v11 import MessageEvent, Message, MessageSegment
+from nonebot import on_command
 from nonebot.internal.matcher import Matcher
+from nonebot.internal.params import Depends
 from nonebot.params import CommandArg
+from nonebot_plugin_saa import MessageFactory
+from nonebot_plugin_session import extract_session, Session
+from nonebot_plugin_session.model import get_or_add_session_model
 
 from .errors import BadRequestError
-from .interceptors.access_control import access_control
 from .interceptors.handle_error import handle_error
 from ..ac import ac
 from ..naga import naga
 from ..naga.service import InvalidKyokuHonbaError
 from ..utils.integer import decode_integer
 from ..utils.nonebot import default_cmd_start
 
 analyze_srv = ac.create_subservice("analyze")
 
 
-async def analyze_majsoul(event: MessageEvent, matcher: Matcher, uuid: str, kyoku: int, honba: int):
+async def analyze_majsoul(matcher: Matcher, customer_id: int, uuid: str, kyoku: int, honba: int):
     try:
-        report, cost_np = await naga.analyze_majsoul(uuid, kyoku, honba, event.user_id)
-        msg = f"https://naga.dmv.nico/htmls/{report.report_id}.html?tw=0\n"
+        report, cost_np = await naga.analyze_majsoul(uuid, kyoku, honba, customer_id)
+        await MessageFactory(f"https://naga.dmv.nico/htmls/{report.report_id}.html?tw=0").send(reply=True)
 
         if cost_np == 0:
-            msg += "由于此前已解析过该局，本次解析消耗0NP"
             token = matcher.state["ac_token"]
             await token.retire()
+            await MessageFactory("由于此前已解析过该局，本次解析消耗0NP").send(reply=True)
         else:
-            msg += f"本次解析消耗{cost_np}NP"
-
-        await matcher.send(Message([
-            MessageSegment.reply(event.message_id),
-            MessageSegment.text(msg)
-        ]))
+            await MessageFactory(f"本次解析消耗{cost_np}NP").send(reply=True)
     except InvalidKyokuHonbaError as e:
         kyoku_honba = []
         for kyoku, honba in e.available_kyoku_honba:
             if kyoku <= 3:
                 kyoku_honba.append(f"东{kyoku + 1}局{honba}本场")
             elif kyoku <= 7:
                 kyoku_honba.append(f"南{kyoku - 3}局{honba}本场")
             else:
                 kyoku_honba.append(f"西{kyoku - 7}局{honba}本场")
 
         raise BadRequestError(f"请输入正确的场次与本场（{'、'.join(kyoku_honba)}）") from e
 
 
-async def analyze_tenhou(event: MessageEvent, matcher: Matcher, haihu_id: str, seat: int):
-    report, cost_np = await naga.analyze_tenhou(haihu_id, seat, event.user_id)
-    msg = f"https://naga.dmv.nico/htmls/{report.report_id}.html?tw=0\n"
+async def analyze_tenhou(matcher: Matcher, customer_id: int, haihu_id: str, seat: int):
+    report, cost_np = await naga.analyze_tenhou(haihu_id, seat, customer_id)
+    await MessageFactory(f"https://naga.dmv.nico/htmls/{report.report_id}.html?tw={seat}").send(reply=True)
 
     if cost_np == 0:
-        msg += "由于此前已解析过该局，本次解析消耗0NP"
         token = matcher.state["ac_token"]
         await token.retire()
+        await MessageFactory("由于此前已解析过该局，本次解析消耗0NP").send(reply=True)
     else:
-        msg += f"本次解析消耗{cost_np}NP"
-
-    await matcher.send(Message([
-        MessageSegment.reply(event.message_id),
-        MessageSegment.text(msg)
-    ]))
+        await MessageFactory(f"本次解析消耗{cost_np}NP").send(reply=True)
 
 
 naga_analyze_matcher = on_command("naga", priority=10)
 
 uuid_reg = re.compile(r"\d{6}-[\da-fA-F]{8}-[\da-fA-F]{4}-[\da-fA-F]{4}-[\da-fA-F]{4}-[\da-fA-F]{12}")
 
 kyoku_honba_reg = re.compile(r"([东南西])([一二三四1234])局([0123456789零一两二三四五六七八九十百千万亿]+)本场")
 
 
 @naga_analyze_matcher.handle()
 @handle_error()
-@access_control(analyze_srv)
-async def naga_analyze(event: MessageEvent, matcher: Matcher, cmd_args=CommandArg()):
+@analyze_srv.patch_handler(retire_on_throw=True)
+async def naga_analyze(matcher: Matcher, cmd_args=CommandArg(),
+                       session: Session = Depends(extract_session)):
+    model = await get_or_add_session_model(session)
+
     args = cmd_args.extract_plain_text().split(' ')
     if "maj-soul" in args[0]:
         mat = uuid_reg.search(args[0])
         if not mat:
             raise BadRequestError("不正确的雀魂牌谱")
 
         uuid = mat.group(0)
@@ -99,29 +94,28 @@
                         kyoku += 8
 
                     honba = decode_integer(raw_honba)
                 except ValueError:
                     pass
 
         if kyoku is None or honba is None:
-            await analyze_majsoul(event, matcher, uuid, -1, -1)  # 让其发送该局的场次本场信息
+            await analyze_majsoul(matcher, model.id, uuid, -1, -1)  # 让其发送该局的场次本场信息
         else:
-            await analyze_majsoul(event, matcher, uuid, kyoku, honba)
+            await analyze_majsoul(matcher, model.id, uuid, kyoku, honba)
     elif "tenhou" in args[0]:
         tenhou_url = args[0].strip()
 
         _, _, _, _, tenhou_query, _ = urlparse(tenhou_url)
         tenhou_query = parse_qs(tenhou_query)
 
         haihu_id = tenhou_query["log"][0]
         seat = 0
         if "tw" in tenhou_query and len(tenhou_query["tw"]) > 0:
             seat = int(tenhou_query["tw"][0])
 
-        await analyze_tenhou(event, matcher, haihu_id, seat)
+        await analyze_tenhou(matcher, model.id, haihu_id, seat)
     else:
-        await matcher.send(Message([
-            MessageSegment.reply(event.message_id),
-            MessageSegment.text("用法：\n"
-                                f"{default_cmd_start}naga <雀魂牌谱链接> <东/南x局x本场>：消耗10NP解析雀魂小局\n"
-                                f"{default_cmd_start}naga <天凤牌谱链接>：消耗50NP解析天凤半庄")
-        ]))
+        await MessageFactory(
+            "用法：\n"
+            f"{default_cmd_start}naga <雀魂牌谱链接> <东/南x局x本场>：消耗10NP解析雀魂小局\n"
+            f"{default_cmd_start}naga <天凤牌谱链接>：消耗50NP解析天凤半庄"
+        ).send(reply=True)
```

### Comparing `nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/matchers/naga_statistic.py` & `nonebot_plugin_nagabus-0.2.0/nonebot_plugin_nagabus/matchers/naga_statistic.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,67 +1,64 @@
 from datetime import datetime
 from io import StringIO
+from typing import Optional
 
 from monthdelta import monthdelta
-from nonebot import on_command
-from nonebot.adapters.onebot.v11 import MessageEvent, Bot, GroupMessageEvent, Message, MessageSegment
-from nonebot.internal.matcher import Matcher
+from nonebot import on_command, Bot
+from nonebot_plugin_datastore.db import get_engine
+from nonebot_plugin_get_nickname import get_nickname
+from nonebot_plugin_saa import MessageFactory
+from nonebot_plugin_session import SessionIdType
+from nonebot_plugin_session.model import SessionModel
+from sqlalchemy.ext.asyncio import AsyncSession
 
 from .interceptors.handle_error import handle_error
 from ..ac import ac
 from ..naga import naga
 from ..utils.tz import TZ_TOKYO
 
 statistic_srv = ac.create_subservice("statistic")
 
 
-async def naga_statistic(bot: Bot, event: MessageEvent, matcher: Matcher, year: int, month: int):
+async def naga_statistic(bot: Bot, year: int, month: int):
     statistic = await naga.statistic(year, month)
 
-    nicknames = {}
-    if isinstance(event, GroupMessageEvent):
-        members = await bot.get_group_member_list(group_id=event.group_id)
-        for m in members:
-            nicknames[m['user_id']] = m['nickname']
-
     total_cost_np = 0
 
-    with StringIO() as sio:
-        for i, s in enumerate(statistic):
-            total_cost_np += s.cost_np
-
-            if s.customer_id in nicknames:
-                nickname = nicknames[s.customer_id]
-            else:
-                user = await bot.get_stranger_info(user_id=s.customer_id)
-                nickname = user['nickname']
-
-            sio.write(f"#{i + 1} {nickname}: {s.cost_np}NP\n")
-
-        msg = (f"{year}年{month}月共使用{total_cost_np}NP\n\n" + sio.getvalue()).strip()
-
-        await matcher.send(Message([
-            MessageSegment.reply(event.message_id),
-            MessageSegment.text(msg)
-        ]))
+    async with AsyncSession(get_engine()) as db_sess:
+        with StringIO() as sio:
+            for i, s in enumerate(statistic):
+                session_model: Optional[SessionModel] = await db_sess.get(SessionModel, s.customer_id)
+                session = session_model.session
+                if session.bot_type != bot.type:  # 来自其他平台的用户
+                    nickname = session.get_id(SessionIdType.USER, include_bot_type=False, include_bot_id=False)
+                else:
+                    nickname = await get_nickname(session, bot)
+                sio.write(f"#{i + 1} {nickname}: {s.cost_np}NP\n")
+
+                total_cost_np += s.cost_np
+
+            msg = (f"{year}年{month}月共使用{total_cost_np}NP\n\n" + sio.getvalue()).strip()
+
+            await MessageFactory(msg).send(reply=True)
 
 
 naga_statistic_this_month_matcher = on_command("naga本月使用情况", priority=5, block=True)
 statistic_srv.patch_matcher(naga_statistic_this_month_matcher)
 
 
 @naga_statistic_this_month_matcher.handle()
 @handle_error()
-async def naga_statistic_this_month(bot: Bot, event: MessageEvent, matcher: Matcher):
+async def naga_statistic_this_month(bot: Bot):
     cur = datetime.now(tz=TZ_TOKYO)
-    await naga_statistic(bot, event, matcher, cur.year, cur.month)
+    await naga_statistic(bot, cur.year, cur.month)
 
 
 naga_statistic_prev_month_matcher = on_command("naga上月使用情况", priority=5, block=True)
 statistic_srv.patch_matcher(naga_statistic_prev_month_matcher)
 
 
 @naga_statistic_prev_month_matcher.handle()
 @handle_error()
-async def naga_statistic_prev_month(bot: Bot, event: MessageEvent, matcher: Matcher):
+async def naga_statistic_prev_month(bot: Bot):
     prev_month = datetime.now(tz=TZ_TOKYO) - monthdelta(months=1)
-    await naga_statistic(bot, event, matcher, prev_month.year, prev_month.month)
+    await naga_statistic(bot, prev_month.year, prev_month.month)
```

### Comparing `nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/migrations/24aec3c56623_.py` & `nonebot_plugin_nagabus-0.2.0/nonebot_plugin_nagabus/migrations/24aec3c56623_.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/migrations/ab4d80c20047_.py` & `nonebot_plugin_nagabus-0.2.0/nonebot_plugin_nagabus/migrations/ab4d80c20047_.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/mjs/__init__.py` & `nonebot_plugin_nagabus-0.2.0/nonebot_plugin_nagabus/mjs/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/naga/api.py` & `nonebot_plugin_nagabus-0.2.0/nonebot_plugin_nagabus/naga/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/naga/fake_api.py` & `nonebot_plugin_nagabus-0.2.0/nonebot_plugin_nagabus/naga/fake_api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/naga/model.py` & `nonebot_plugin_nagabus-0.2.0/nonebot_plugin_nagabus/naga/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/naga/service.py` & `nonebot_plugin_nagabus-0.2.0/nonebot_plugin_nagabus/naga/service.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/utils/integer.py` & `nonebot_plugin_nagabus-0.2.0/nonebot_plugin_nagabus/utils/integer.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.5/pyproject.toml` & `nonebot_plugin_nagabus-0.2.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 [tool.poetry]
 name = "nonebot-plugin-nagabus"
-version = "0.1.5"
+version = "0.2.0"
 description = ""
 authors = ["ssttkkl <huang.wen.long@hotmail.com>"]
 readme = "README.md"
 packages = [{ include = "nonebot_plugin_nagabus" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 nonebot2 = "^2.0.0rc4"
 httpx = "^0.23.0"
 nonebot-adapter-onebot = "^2.2.3"
-nonebot-plugin-majsoul = "^0.2.0.post1"
+nonebot-plugin-access-control = ">=0.5.1"
 nonebot-plugin-datastore = "^0.6.3"
+nonebot-plugin-get-nickname = "^0.1.0"
+nonebot-plugin-majsoul = "^0.2.0.post1"
+nonebot-plugin-session = ">=0.0.3"
+nonebot-plugin-send-anything-anywhere = "^0.2.4"
 typing-extensions = "^4.6.2"
 pydantic = "^1.10.8"
 monthdelta = "^0.9.1"
-nonebot-plugin-access-control = "^0.4.2"
+
+[tool.poetry.group.dev.dependencies]
+nonebot2 = { extras = ["httpx", "fastapi"], version = "^2.0.0rc3" }
+nonebot-plugin-escape-url = "^0.1.0"
+nonebot-adapter-qqguild = "^0.2.2"
 
 [tool.nonebot]
 plugins = ["nonebot_plugin_nagabus"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_nagabus-0.1.5/README.md` & `nonebot_plugin_nagabus-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.5/PKG-INFO` & `nonebot_plugin_nagabus-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-nagabus
-Version: 0.1.5
+Version: 0.2.0
 Summary: 
 Author: ssttkkl
 Author-email: huang.wen.long@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.23.0,<0.24.0)
 Requires-Dist: monthdelta (>=0.9.1,<0.10.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.2.3,<3.0.0)
-Requires-Dist: nonebot-plugin-access-control (>=0.4.2,<0.5.0)
+Requires-Dist: nonebot-plugin-access-control (>=0.5.1)
 Requires-Dist: nonebot-plugin-datastore (>=0.6.3,<0.7.0)
+Requires-Dist: nonebot-plugin-get-nickname (>=0.1.0,<0.2.0)
 Requires-Dist: nonebot-plugin-majsoul (>=0.2.0.post1,<0.3.0)
+Requires-Dist: nonebot-plugin-send-anything-anywhere (>=0.2.4,<0.3.0)
+Requires-Dist: nonebot-plugin-session (>=0.0.3)
 Requires-Dist: nonebot2 (>=2.0.0rc4,<3.0.0)
 Requires-Dist: pydantic (>=1.10.8,<2.0.0)
 Requires-Dist: typing-extensions (>=4.6.2,<5.0.0)
 Description-Content-Type: text/markdown
 
 nonebot-plugin-nagabus
 ==========
```

