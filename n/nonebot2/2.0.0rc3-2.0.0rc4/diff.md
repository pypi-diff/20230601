# Comparing `tmp/nonebot2-2.0.0rc3.tar.gz` & `tmp/nonebot2-2.0.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot2-2.0.0rc3.tar", max compression
+gzip compressed data, was "nonebot2-2.0.0rc4.tar", max compression
```

## Comparing `nonebot2-2.0.0rc3.tar` & `nonebot2-2.0.0rc4.tar`

### file list

```diff
@@ -1,53 +1,54 @@
--rw-r--r--   0        0        0     1078 2023-01-22 08:17:39.873753 nonebot2-2.0.0rc3/LICENSE
--rw-r--r--   0        0        0    15282 2023-01-22 08:17:39.873753 nonebot2-2.0.0rc3/README.md
--rw-r--r--   0        0        0    11212 2023-01-22 08:17:39.873753 nonebot2-2.0.0rc3/nonebot/__init__.py
--rw-r--r--   0        0        0      742 2023-01-22 08:17:39.873753 nonebot2-2.0.0rc3/nonebot/adapters/__init__.py
--rw-r--r--   0        0        0     8447 2023-01-22 08:17:39.873753 nonebot2-2.0.0rc3/nonebot/config.py
--rw-r--r--   0        0        0     1921 2023-01-22 08:17:39.877753 nonebot2-2.0.0rc3/nonebot/consts.py
--rw-r--r--   0        0        0     6877 2023-01-22 08:17:39.877753 nonebot2-2.0.0rc3/nonebot/dependencies/__init__.py
--rw-r--r--   0        0        0     1623 2023-01-22 08:17:39.877753 nonebot2-2.0.0rc3/nonebot/dependencies/utils.py
--rw-r--r--   0        0        0     1312 2023-01-22 08:17:39.877753 nonebot2-2.0.0rc3/nonebot/drivers/__init__.py
--rw-r--r--   0        0        0     5563 2023-01-22 08:17:39.877753 nonebot2-2.0.0rc3/nonebot/drivers/aiohttp.py
--rw-r--r--   0        0        0    10108 2023-01-22 08:17:39.877753 nonebot2-2.0.0rc3/nonebot/drivers/fastapi.py
--rw-r--r--   0        0        0     2105 2023-01-22 08:17:39.877753 nonebot2-2.0.0rc3/nonebot/drivers/httpx.py
--rw-r--r--   0        0        0     5035 2023-01-22 08:17:39.877753 nonebot2-2.0.0rc3/nonebot/drivers/none.py
--rw-r--r--   0        0        0     8975 2023-01-22 08:17:39.877753 nonebot2-2.0.0rc3/nonebot/drivers/quart.py
--rw-r--r--   0        0        0     3940 2023-01-22 08:17:39.877753 nonebot2-2.0.0rc3/nonebot/drivers/websockets.py
--rw-r--r--   0        0        0     6394 2023-01-22 08:17:39.877753 nonebot2-2.0.0rc3/nonebot/exception.py
--rw-r--r--   0        0        0        0 2023-01-22 08:17:39.877753 nonebot2-2.0.0rc3/nonebot/internal/__init__.py
--rw-r--r--   0        0        0      253 2023-01-22 08:17:39.877753 nonebot2-2.0.0rc3/nonebot/internal/adapter/__init__.py
--rw-r--r--   0        0        0     3655 2023-01-22 08:17:39.877753 nonebot2-2.0.0rc3/nonebot/internal/adapter/adapter.py
--rw-r--r--   0        0        0     5076 2023-01-22 08:17:39.877753 nonebot2-2.0.0rc3/nonebot/internal/adapter/bot.py
--rw-r--r--   0        0        0     2566 2023-01-22 08:17:39.877753 nonebot2-2.0.0rc3/nonebot/internal/adapter/event.py
--rw-r--r--   0        0        0     9500 2023-01-22 08:17:39.877753 nonebot2-2.0.0rc3/nonebot/internal/adapter/message.py
--rw-r--r--   0        0        0     6325 2023-01-22 08:17:39.877753 nonebot2-2.0.0rc3/nonebot/internal/adapter/template.py
--rw-r--r--   0        0        0     1123 2023-01-22 08:17:39.877753 nonebot2-2.0.0rc3/nonebot/internal/driver/__init__.py
--rw-r--r--   0        0        0     8072 2023-01-22 08:17:39.877753 nonebot2-2.0.0rc3/nonebot/internal/driver/driver.py
--rw-r--r--   0        0        0    11086 2023-01-22 08:17:39.877753 nonebot2-2.0.0rc3/nonebot/internal/driver/model.py
--rw-r--r--   0        0        0      464 2023-01-22 08:17:39.877753 nonebot2-2.0.0rc3/nonebot/internal/matcher/__init__.py
--rw-r--r--   0        0        0     2760 2023-01-22 08:17:39.877753 nonebot2-2.0.0rc3/nonebot/internal/matcher/manager.py
--rw-r--r--   0        0        0    25404 2023-01-22 08:17:39.877753 nonebot2-2.0.0rc3/nonebot/internal/matcher/matcher.py
--rw-r--r--   0        0        0      731 2023-01-22 08:17:39.877753 nonebot2-2.0.0rc3/nonebot/internal/matcher/provider.py
--rw-r--r--   0        0        0    11892 2023-01-22 08:17:39.877753 nonebot2-2.0.0rc3/nonebot/internal/params.py
--rw-r--r--   0        0        0     4298 2023-01-22 08:17:39.877753 nonebot2-2.0.0rc3/nonebot/internal/permission.py
--rw-r--r--   0        0        0     3130 2023-01-22 08:17:39.877753 nonebot2-2.0.0rc3/nonebot/internal/rule.py
--rw-r--r--   0        0        0     2487 2023-01-22 08:17:39.877753 nonebot2-2.0.0rc3/nonebot/log.py
--rw-r--r--   0        0        0      989 2023-01-22 08:17:39.877753 nonebot2-2.0.0rc3/nonebot/matcher.py
--rw-r--r--   0        0        0    10148 2023-01-22 08:17:39.877753 nonebot2-2.0.0rc3/nonebot/message.py
--rw-r--r--   0        0        0     5839 2023-01-22 08:17:39.877753 nonebot2-2.0.0rc3/nonebot/params.py
--rw-r--r--   0        0        0     3047 2023-01-22 08:17:39.877753 nonebot2-2.0.0rc3/nonebot/permission.py
--rw-r--r--   0        0        0     5544 2023-01-22 08:17:39.877753 nonebot2-2.0.0rc3/nonebot/plugin/__init__.py
--rw-r--r--   0        0        0     5286 2023-01-22 08:17:39.877753 nonebot2-2.0.0rc3/nonebot/plugin/load.py
--rw-r--r--   0        0        0     8424 2023-01-22 08:17:39.877753 nonebot2-2.0.0rc3/nonebot/plugin/manager.py
--rw-r--r--   0        0        0    30681 2023-01-22 08:17:39.877753 nonebot2-2.0.0rc3/nonebot/plugin/on.py
--rw-r--r--   0        0        0    14695 2023-01-22 08:17:39.877753 nonebot2-2.0.0rc3/nonebot/plugin/on.pyi
--rw-r--r--   0        0        0     1475 2023-01-22 08:17:39.877753 nonebot2-2.0.0rc3/nonebot/plugin/plugin.py
--rw-r--r--   0        0        0      290 2023-01-22 08:17:39.877753 nonebot2-2.0.0rc3/nonebot/plugins/echo.py
--rw-r--r--   0        0        0      878 2023-01-22 08:17:39.877753 nonebot2-2.0.0rc3/nonebot/plugins/single_session.py
--rw-r--r--   0        0        0        0 2023-01-22 08:17:39.877753 nonebot2-2.0.0rc3/nonebot/py.typed
--rw-r--r--   0        0        0    20850 2023-01-22 08:17:39.877753 nonebot2-2.0.0rc3/nonebot/rule.py
--rw-r--r--   0        0        0     4822 2023-01-22 08:17:39.877753 nonebot2-2.0.0rc3/nonebot/typing.py
--rw-r--r--   0        0        0     5562 2023-01-22 08:17:39.877753 nonebot2-2.0.0rc3/nonebot/utils.py
--rw-r--r--   0        0        0     2747 2023-01-22 08:17:39.877753 nonebot2-2.0.0rc3/pyproject.toml
--rw-r--r--   0        0        0    17106 1970-01-01 00:00:00.000000 nonebot2-2.0.0rc3/setup.py
--rw-r--r--   0        0        0    17170 1970-01-01 00:00:00.000000 nonebot2-2.0.0rc3/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-04-01 03:59:23.818395 nonebot2-2.0.0rc4/LICENSE
+-rw-r--r--   0        0        0    15189 2023-04-01 03:59:23.818395 nonebot2-2.0.0rc4/README.md
+-rw-r--r--   0        0        0    12147 2023-04-01 03:59:23.818395 nonebot2-2.0.0rc4/nonebot/__init__.py
+-rw-r--r--   0        0        0      742 2023-04-01 03:59:23.818395 nonebot2-2.0.0rc4/nonebot/adapters/__init__.py
+-rw-r--r--   0        0        0     8480 2023-04-01 03:59:23.818395 nonebot2-2.0.0rc4/nonebot/config.py
+-rw-r--r--   0        0        0     2148 2023-04-01 03:59:23.818395 nonebot2-2.0.0rc4/nonebot/consts.py
+-rw-r--r--   0        0        0     6877 2023-04-01 03:59:23.818395 nonebot2-2.0.0rc4/nonebot/dependencies/__init__.py
+-rw-r--r--   0        0        0     1623 2023-04-01 03:59:23.818395 nonebot2-2.0.0rc4/nonebot/dependencies/utils.py
+-rw-r--r--   0        0        0     1312 2023-04-01 03:59:23.818395 nonebot2-2.0.0rc4/nonebot/drivers/__init__.py
+-rw-r--r--   0        0        0     1439 2023-04-01 03:59:23.818395 nonebot2-2.0.0rc4/nonebot/drivers/_lifespan.py
+-rw-r--r--   0        0        0     5573 2023-04-01 03:59:23.818395 nonebot2-2.0.0rc4/nonebot/drivers/aiohttp.py
+-rw-r--r--   0        0        0    10258 2023-04-01 03:59:23.818395 nonebot2-2.0.0rc4/nonebot/drivers/fastapi.py
+-rw-r--r--   0        0        0     2115 2023-04-01 03:59:23.818395 nonebot2-2.0.0rc4/nonebot/drivers/httpx.py
+-rw-r--r--   0        0        0     4417 2023-04-01 03:59:23.818395 nonebot2-2.0.0rc4/nonebot/drivers/none.py
+-rw-r--r--   0        0        0     8985 2023-04-01 03:59:23.818395 nonebot2-2.0.0rc4/nonebot/drivers/quart.py
+-rw-r--r--   0        0        0     3950 2023-04-01 03:59:23.818395 nonebot2-2.0.0rc4/nonebot/drivers/websockets.py
+-rw-r--r--   0        0        0     6394 2023-04-01 03:59:23.818395 nonebot2-2.0.0rc4/nonebot/exception.py
+-rw-r--r--   0        0        0        0 2023-04-01 03:59:23.818395 nonebot2-2.0.0rc4/nonebot/internal/__init__.py
+-rw-r--r--   0        0        0      253 2023-04-01 03:59:23.818395 nonebot2-2.0.0rc4/nonebot/internal/adapter/__init__.py
+-rw-r--r--   0        0        0     3747 2023-04-01 03:59:23.818395 nonebot2-2.0.0rc4/nonebot/internal/adapter/adapter.py
+-rw-r--r--   0        0        0     5076 2023-04-01 03:59:23.818395 nonebot2-2.0.0rc4/nonebot/internal/adapter/bot.py
+-rw-r--r--   0        0        0     2567 2023-04-01 03:59:23.818395 nonebot2-2.0.0rc4/nonebot/internal/adapter/event.py
+-rw-r--r--   0        0        0     9500 2023-04-01 03:59:23.818395 nonebot2-2.0.0rc4/nonebot/internal/adapter/message.py
+-rw-r--r--   0        0        0     6322 2023-04-01 03:59:23.818395 nonebot2-2.0.0rc4/nonebot/internal/adapter/template.py
+-rw-r--r--   0        0        0     1123 2023-04-01 03:59:23.818395 nonebot2-2.0.0rc4/nonebot/internal/driver/__init__.py
+-rw-r--r--   0        0        0     8526 2023-04-01 03:59:23.818395 nonebot2-2.0.0rc4/nonebot/internal/driver/driver.py
+-rw-r--r--   0        0        0    11086 2023-04-01 03:59:23.818395 nonebot2-2.0.0rc4/nonebot/internal/driver/model.py
+-rw-r--r--   0        0        0      464 2023-04-01 03:59:23.818395 nonebot2-2.0.0rc4/nonebot/internal/matcher/__init__.py
+-rw-r--r--   0        0        0     2760 2023-04-01 03:59:23.818395 nonebot2-2.0.0rc4/nonebot/internal/matcher/manager.py
+-rw-r--r--   0        0        0    26149 2023-04-01 03:59:23.818395 nonebot2-2.0.0rc4/nonebot/internal/matcher/matcher.py
+-rw-r--r--   0        0        0      731 2023-04-01 03:59:23.818395 nonebot2-2.0.0rc4/nonebot/internal/matcher/provider.py
+-rw-r--r--   0        0        0    12389 2023-04-01 03:59:23.818395 nonebot2-2.0.0rc4/nonebot/internal/params.py
+-rw-r--r--   0        0        0     5623 2023-04-01 03:59:23.818395 nonebot2-2.0.0rc4/nonebot/internal/permission.py
+-rw-r--r--   0        0        0     3130 2023-04-01 03:59:23.818395 nonebot2-2.0.0rc4/nonebot/internal/rule.py
+-rw-r--r--   0        0        0     2479 2023-04-01 03:59:23.818395 nonebot2-2.0.0rc4/nonebot/log.py
+-rw-r--r--   0        0        0      989 2023-04-01 03:59:23.818395 nonebot2-2.0.0rc4/nonebot/matcher.py
+-rw-r--r--   0        0        0    10148 2023-04-01 03:59:23.818395 nonebot2-2.0.0rc4/nonebot/message.py
+-rw-r--r--   0        0        0     6083 2023-04-01 03:59:23.818395 nonebot2-2.0.0rc4/nonebot/params.py
+-rw-r--r--   0        0        0     3047 2023-04-01 03:59:23.818395 nonebot2-2.0.0rc4/nonebot/permission.py
+-rw-r--r--   0        0        0     5544 2023-04-01 03:59:23.818395 nonebot2-2.0.0rc4/nonebot/plugin/__init__.py
+-rw-r--r--   0        0        0     5417 2023-04-01 03:59:23.818395 nonebot2-2.0.0rc4/nonebot/plugin/load.py
+-rw-r--r--   0        0        0     8694 2023-04-01 03:59:23.818395 nonebot2-2.0.0rc4/nonebot/plugin/manager.py
+-rw-r--r--   0        0        0    29283 2023-04-01 03:59:23.818395 nonebot2-2.0.0rc4/nonebot/plugin/on.py
+-rw-r--r--   0        0        0    15563 2023-04-01 03:59:23.818395 nonebot2-2.0.0rc4/nonebot/plugin/on.pyi
+-rw-r--r--   0        0        0     1481 2023-04-01 03:59:23.818395 nonebot2-2.0.0rc4/nonebot/plugin/plugin.py
+-rw-r--r--   0        0        0      290 2023-04-01 03:59:23.818395 nonebot2-2.0.0rc4/nonebot/plugins/echo.py
+-rw-r--r--   0        0        0      878 2023-04-01 03:59:23.818395 nonebot2-2.0.0rc4/nonebot/plugins/single_session.py
+-rw-r--r--   0        0        0        0 2023-04-01 03:59:23.818395 nonebot2-2.0.0rc4/nonebot/py.typed
+-rw-r--r--   0        0        0    21917 2023-04-01 03:59:23.818395 nonebot2-2.0.0rc4/nonebot/rule.py
+-rw-r--r--   0        0        0     4822 2023-04-01 03:59:23.818395 nonebot2-2.0.0rc4/nonebot/typing.py
+-rw-r--r--   0        0        0     6179 2023-04-01 03:59:23.822395 nonebot2-2.0.0rc4/nonebot/utils.py
+-rw-r--r--   0        0        0     2724 2023-04-01 03:59:23.822395 nonebot2-2.0.0rc4/pyproject.toml
+-rw-r--r--   0        0        0    17006 1970-01-01 00:00:00.000000 nonebot2-2.0.0rc4/setup.py
+-rw-r--r--   0        0        0    17090 1970-01-01 00:00:00.000000 nonebot2-2.0.0rc4/PKG-INFO
```

### Comparing `nonebot2-2.0.0rc3/LICENSE` & `nonebot2-2.0.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot2-2.0.0rc3/README.md` & `nonebot2-2.0.0rc4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -67,36 +67,34 @@
     <img src="https://discordapp.com/api/guilds/847819937858584596/widget.png?style=shield" alt="Discord Server">
   </a>
 </p>
 
 <p align="center">
   <a href="https://v2.nonebot.dev/">文档</a>
   ·
-  <a href="https://v2.nonebot.dev/docs/start/installation">安装</a>
-  ·
-  <a href="https://v2.nonebot.dev/docs/tutorial/create-project">开始使用</a>
+  <a href="https://v2.nonebot.dev/docs/quick-start">快速上手</a>
   ·
   <a href="#插件">文档打不开？</a>
 </p>
 
 <p align="center">
-  <a href="https://asciinema.org/a/464654">
+  <a href="https://asciinema.org/a/569440">
     <img src="https://v2.nonebot.dev/img/setup.svg">
   </a>
 </p>
 
 ## 简介
 
 NoneBot2 是一个现代、跨平台、可扩展的 Python 聊天机器人框架，它基于 Python 的类型注解和异步特性，能够为你的需求实现提供便捷灵活的支持。
 
 ## 特色
 
 - 异步优先：基于 Python 的异步特性，即使是~~非常~~大量的消息，也能吞吐自如
 - 易于开发：配合 NB-CLI 脚手架，代码编写上手简单，没有过多的冗余代码，可以让开发者专注于业务逻辑
-- 生而可靠：100% 类型注解覆盖，配合编辑器的类型推导功能，能将绝大多数的 Bug 杜绝在编辑器中 ([编辑器支持](https://v2.nonebot.dev/docs/start/editor-support))
+- 生而可靠：100% 类型注解覆盖，配合编辑器的类型推导功能，能将绝大多数的 Bug 杜绝在编辑器中 ([编辑器支持](https://v2.nonebot.dev/docs/editor-support))
 - 社区丰富：社区用户众多，直接和间接用户超过十万人，每天都有大量的活跃用户 ([社区资源](#社区资源))
 - 海纳百川：一个框架，支持多个聊天软件平台，可自定义通信协议
 
   |                                 协议名称                                  | 状态 |                                注释                                |
   | :-----------------------------------------------------------------------: | :--: | :----------------------------------------------------------------: |
   |                    [OneBot 协议](https://onebot.dev/)                     |  ✅  | 支持 QQ、TG、微信公众号等[平台](https://onebot.dev/ecosystem.html) |
   |              [Telegram](https://core.telegram.org/bots/api)               |  ✅  |                                                                    |
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
                                    [nonebot]
          # NoneBot   _â¨ è·¨å¹³å° Python å¼æ­¥æºå¨äººæ¡æ¶ â¨_
            [license] [pypi] [python] [codecov] [site] [pre-commit]
      [onebot] [onebot] [telegram] [feishu] [github] [QQé¢é]_[dingtalk]
        [QQ_Chat_Group] [QQ_Channel] [Telegram_Channel] [Discord_Server]
-            ææ¡£ Â· å®è£ Â· å¼å§ä½¿ç¨ Â· ææ¡£æä¸å¼ï¼
+                 ææ¡£ Â· å¿«éä¸æ Â· ææ¡£æä¸å¼ï¼
                     [https://v2.nonebot.dev/img/setup.svg]
 ## ç®ä» NoneBot2 æ¯ä¸ä¸ªç°ä»£ãè·¨å¹³å°ãå¯æ©å±ç Python
 èå¤©æºå¨äººæ¡æ¶ï¼å®åºäº Python
 çç±»åæ³¨è§£åå¼æ­¥ç¹æ§ï¼è½å¤ä¸ºä½ çéæ±å®ç°æä¾ä¾¿æ·çµæ´»çæ¯æã
 ## ç¹è² - å¼æ­¥ä¼åï¼åºäº Python
 çå¼æ­¥ç¹æ§ï¼å³ä½¿æ¯~~éå¸¸~~å¤§éçæ¶æ¯ï¼ä¹è½ååèªå¦ -
 æäºå¼åï¼éå NB-CLI
 èææ¶ï¼ä»£ç ç¼åä¸æç®åï¼æ²¡æè¿å¤çåä½ä»£ç ï¼å¯ä»¥è®©å¼åèä¸æ³¨äºä¸å¡é»è¾
 - çèå¯é ï¼100%
 ç±»åæ³¨è§£è¦çï¼éåç¼è¾å¨çç±»åæ¨å¯¼åè½ï¼è½å°ç»å¤§å¤æ°ç
-Bug æç»å¨ç¼è¾å¨ä¸­ ([ç¼è¾å¨æ¯æ](https://v2.nonebot.dev/docs/start/
+Bug æç»å¨ç¼è¾å¨ä¸­ ([ç¼è¾å¨æ¯æ](https://v2.nonebot.dev/docs/
 editor-support)) -
 ç¤¾åºä¸°å¯ï¼ç¤¾åºç¨æ·ä¼å¤ï¼ç´æ¥åé´æ¥ç¨æ·è¶è¿åä¸äººï¼æ¯å¤©é½æå¤§éçæ´»è·ç¨æ·
 ([ç¤¾åºèµæº](#ç¤¾åºèµæº)) -
 æµ·çº³ç¾å·ï¼ä¸ä¸ªæ¡æ¶ï¼æ¯æå¤ä¸ªèå¤©è½¯ä»¶å¹³å°ï¼å¯èªå®ä¹éä¿¡åè®®
 | åè®®åç§° | ç¶æ | æ³¨é | | :-----------------------------------------
 ------------------------------: | :--: | :-------------------------------------
 ---------------------------: | | [OneBot åè®®](https://onebot.dev/) | â |
```

### Comparing `nonebot2-2.0.0rc3/nonebot/__init__.py` & `nonebot2-2.0.0rc4/nonebot/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,32 +34,33 @@
 
 FrontMatter:
     sidebar_position: 0
     description: nonebot 模块
 """
 
 import os
-import importlib
 from importlib.metadata import version
-from typing import Any, Dict, Type, Optional
+from typing import Any, Dict, Type, Union, TypeVar, Optional, overload
 
 import loguru
 from pydantic.env_settings import DotenvType
 
-from nonebot.adapters import Bot
-from nonebot.utils import escape_tag
 from nonebot.config import Env, Config
 from nonebot.log import logger as logger
+from nonebot.adapters import Bot, Adapter
+from nonebot.utils import escape_tag, resolve_dot_notation
 from nonebot.drivers import Driver, ReverseDriver, combine_driver
 
 try:
     __version__ = version("nonebot2")
 except Exception:  # pragma: no cover
     __version__ = None
 
+A = TypeVar("A", bound=Adapter)
+
 _driver: Optional[Driver] = None
 
 
 def get_driver() -> Driver:
     """获取全局 {ref}`nonebot.drivers.Driver` 实例。
 
     可用于在计划任务的回调等情形中获取当前 {ref}`nonebot.drivers.Driver` 实例。
@@ -76,14 +77,64 @@
         ```
     """
     if _driver is None:
         raise ValueError("NoneBot has not been initialized.")
     return _driver
 
 
+@overload
+def get_adapter(name: str) -> Adapter:
+    ...
+
+
+@overload
+def get_adapter(name: Type[A]) -> A:
+    ...
+
+
+def get_adapter(name: Union[str, Type[Adapter]]) -> Adapter:
+    """获取已注册的 {ref}`nonebot.adapters.Adapter` 实例。
+
+    返回:
+        指定名称或类型的 {ref}`nonebot.adapters.Adapter` 对象
+
+    异常:
+        ValueError: 指定的 {ref}`nonebot.adapters.Adapter` 未注册
+        ValueError: 全局 {ref}`nonebot.drivers.Driver` 对象尚未初始化 ({ref}`nonebot.init <nonebot.init>` 尚未调用)
+
+    用法:
+        ```python
+        from nonebot.adapters.console import Adapter
+        adapter = nonebot.get_adapter(Adapter)
+        ```
+    """
+    adapters = get_adapters()
+    target = name if isinstance(name, str) else name.get_name()
+    if target not in adapters:
+        raise ValueError(f"Adapter {target} not registered.")
+    return adapters[target]
+
+
+def get_adapters() -> Dict[str, Adapter]:
+    """获取所有已注册的 {ref}`nonebot.adapters.Adapter` 实例。
+
+    返回:
+        所有 {ref}`nonebot.adapters.Adapter` 实例字典
+
+    异常:
+        ValueError: 全局 {ref}`nonebot.drivers.Driver` 对象尚未初始化 ({ref}`nonebot.init <nonebot.init>` 尚未调用)
+
+    用法:
+        ```python
+        adapters = nonebot.get_adapters()
+        ```
+    """
+    return get_driver()._adapters.copy()
+
+
 def get_app() -> Any:
     """获取全局 {ref}`nonebot.drivers.ReverseDriver` 对应的 Server App 对象。
 
     返回:
         Server App 对象
 
     异常:
@@ -171,39 +222,24 @@
         ```python
         bots = nonebot.get_bots()
         ```
     """
     return get_driver().bots
 
 
-def _resolve_dot_notation(
-    obj_str: str, default_attr: str, default_prefix: Optional[str] = None
-) -> Any:
-    modulename, _, cls = obj_str.partition(":")
-    if default_prefix is not None and modulename.startswith("~"):
-        modulename = default_prefix + modulename[1:]
-    module = importlib.import_module(modulename)
-    if not cls:
-        return getattr(module, default_attr)
-    instance = module
-    for attr_str in cls.split("."):
-        instance = getattr(instance, attr_str)
-    return instance
-
-
 def _resolve_combine_expr(obj_str: str) -> Type[Driver]:
     drivers = obj_str.split("+")
-    DriverClass = _resolve_dot_notation(
+    DriverClass = resolve_dot_notation(
         drivers[0], "Driver", default_prefix="nonebot.drivers."
     )
     if len(drivers) == 1:
         logger.trace(f"Detected driver {DriverClass} with no mixins.")
         return DriverClass
     mixins = [
-        _resolve_dot_notation(mixin, "Mixin", default_prefix="nonebot.drivers.")
+        resolve_dot_notation(mixin, "Mixin", default_prefix="nonebot.drivers.")
         for mixin in drivers[1:]
     ]
     logger.trace(f"Detected driver {DriverClass} with mixins {mixins}.")
     return combine_driver(DriverClass, *mixins)
 
 
 def _log_patcher(record: "loguru.Record"):
```

### Comparing `nonebot2-2.0.0rc3/nonebot/adapters/__init__.py` & `nonebot2-2.0.0rc4/nonebot/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.0.0rc3/nonebot/config.py` & `nonebot2-2.0.0rc4/nonebot/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 """
 import os
 from datetime import timedelta
 from ipaddress import IPv4Address
 from typing import TYPE_CHECKING, Any, Set, Dict, Tuple, Union, Mapping, Optional
 
 from pydantic.utils import deep_update
-from pydantic import Extra, BaseSettings, IPvAnyAddress
+from pydantic import Extra, Field, BaseSettings, IPvAnyAddress
 from pydantic.env_settings import (
     DotenvType,
     SettingsError,
     EnvSettingsSource,
     InitSettingsSource,
     SettingsSourceCallable,
 )
@@ -154,30 +154,30 @@
 
 class Config(BaseConfig):
     """NoneBot 主要配置。大小写不敏感。
 
     除了 NoneBot 的配置项外，还可以自行添加配置项到 `.env.{environment}` 文件中。
     这些配置将会在 json 反序列化后一起带入 `Config` 类中。
 
-    配置方法参考: [配置](https://v2.nonebot.dev/docs/tutorial/configuration)
+    配置方法参考: [配置](https://v2.nonebot.dev/docs/appendices/config)
     """
 
     _env_file: DotenvType = ".env", ".env.prod"
 
     # nonebot configs
     driver: str = "~fastapi"
     """NoneBot 运行所使用的 `Driver` 。继承自 {ref}`nonebot.drivers.Driver` 。
 
     配置格式为 `<module>[:<Driver>][+<module>[:<Mixin>]]*`。
 
     `~` 为 `nonebot.drivers.` 的缩写。
     """
     host: IPvAnyAddress = IPv4Address("127.0.0.1")  # type: ignore
     """NoneBot {ref}`nonebot.drivers.ReverseDriver` 服务端监听的 IP/主机名。"""
-    port: int = 8080
+    port: int = Field(default=8080, ge=1, le=65535)
     """NoneBot {ref}`nonebot.drivers.ReverseDriver` 服务端监听的端口。"""
     log_level: Union[int, str] = "INFO"
     """NoneBot 日志输出等级，可以为 `int` 类型等级或等级名称
 
     参考 [`loguru 日志等级`](https://loguru.readthedocs.io/en/stable/api/logger.html#levels)。
 
     :::tip 提示
```

### Comparing `nonebot2-2.0.0rc3/nonebot/consts.py` & `nonebot2-2.0.0rc4/nonebot/consts.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """本模块包含了 NoneBot 事件处理过程中使用到的常量。
 
 FrontMatter:
     sidebar_position: 9
     description: nonebot.consts 模块
 """
+import os
+import sys
 from typing import Literal
 
 # used by Matcher
 RECEIVE_KEY: Literal["_receive_{id}"] = "_receive_{id}"
 """`receive` 存储 key"""
 LAST_RECEIVE_KEY: Literal["_last_receive"] = "_last_receive"
 """`last_receive` 存储 key"""
@@ -26,14 +28,16 @@
 """命令元组存储 key"""
 RAW_CMD_KEY: Literal["raw_command"] = "raw_command"
 """命令文本存储 key"""
 CMD_ARG_KEY: Literal["command_arg"] = "command_arg"
 """命令参数存储 key"""
 CMD_START_KEY: Literal["command_start"] = "command_start"
 """命令开头存储 key"""
+CMD_WHITESPACE_KEY: Literal["command_whitespace"] = "command_whitespace"
+"""命令与参数间空白符存储 key"""
 
 SHELL_ARGS: Literal["_args"] = "_args"
 """shell 命令 parse 后参数字典存储 key"""
 SHELL_ARGV: Literal["_argv"] = "_argv"
 """shell 命令原始参数列表存储 key"""
 
 REGEX_MATCHED: Literal["_matched"] = "_matched"
@@ -48,7 +52,9 @@
 """响应触发前缀 key"""
 ENDSWITH_KEY: Literal["_endswith"] = "_endswith"
 """响应触发后缀 key"""
 FULLMATCH_KEY: Literal["_fullmatch"] = "_fullmatch"
 """响应触发完整消息 key"""
 KEYWORD_KEY: Literal["_keyword"] = "_keyword"
 """响应触发关键字 key"""
+
+WINDOWS = sys.platform.startswith("win") or (sys.platform == "cli" and os.name == "nt")
```

### Comparing `nonebot2-2.0.0rc3/nonebot/dependencies/__init__.py` & `nonebot2-2.0.0rc4/nonebot/dependencies/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.0.0rc3/nonebot/dependencies/utils.py` & `nonebot2-2.0.0rc4/nonebot/dependencies/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.0.0rc3/nonebot/drivers/__init__.py` & `nonebot2-2.0.0rc4/nonebot/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.0.0rc3/nonebot/drivers/aiohttp.py` & `nonebot2-2.0.0rc4/nonebot/drivers/aiohttp.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,18 +23,18 @@
 from nonebot.exception import WebSocketClosed
 from nonebot.drivers.none import Driver as NoneDriver
 from nonebot.drivers import WebSocket as BaseWebSocket
 from nonebot.drivers import HTTPVersion, ForwardMixin, ForwardDriver, combine_driver
 
 try:
     import aiohttp
-except ImportError:  # pragma: no cover
+except ModuleNotFoundError as e:  # pragma: no cover
     raise ImportError(
         "Please install aiohttp first to use this driver. `pip install nonebot2[aiohttp]`"
-    ) from None
+    ) from e
 
 
 class Mixin(ForwardMixin):
     """AIOHTTP Mixin"""
 
     @property
     @overrides(ForwardMixin)
```

### Comparing `nonebot2-2.0.0rc3/nonebot/drivers/fastapi.py` & `nonebot2-2.0.0rc4/nonebot/drivers/fastapi.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,36 +15,38 @@
     description: nonebot.drivers.fastapi 模块
 """
 
 
 import logging
 import contextlib
 from functools import wraps
-from typing import Any, Dict, List, Tuple, Union, Callable, Optional
+from typing import Any, Dict, List, Tuple, Union, Optional
 
 from pydantic import BaseSettings
 
 from nonebot.config import Env
 from nonebot.typing import overrides
 from nonebot.exception import WebSocketClosed
 from nonebot.internal.driver import FileTypes
 from nonebot.config import Config as NoneBotConfig
 from nonebot.drivers import Request as BaseRequest
 from nonebot.drivers import WebSocket as BaseWebSocket
 from nonebot.drivers import ReverseDriver, HTTPServerSetup, WebSocketServerSetup
 
+from ._lifespan import LIFESPAN_FUNC, Lifespan
+
 try:
     import uvicorn
     from fastapi.responses import Response
     from fastapi import FastAPI, Request, UploadFile, status
     from starlette.websockets import WebSocket, WebSocketState, WebSocketDisconnect
-except ImportError:  # pragma: no cover
+except ModuleNotFoundError as e:  # pragma: no cover
     raise ImportError(
         "Please install FastAPI by using `pip install nonebot2[fastapi]`"
-    ) from None
+    ) from e
 
 
 def catch_closed(func):
     @wraps(func)
     async def decorator(*args, **kwargs):
         try:
             return await func(*args, **kwargs)
@@ -88,15 +90,18 @@
     """FastAPI 驱动框架。"""
 
     def __init__(self, env: Env, config: NoneBotConfig):
         super(Driver, self).__init__(env, config)
 
         self.fastapi_config: Config = Config(**config.dict())
 
+        self._lifespan = Lifespan()
+
         self._server_app = FastAPI(
+            lifespan=self._lifespan_manager,
             openapi_url=self.fastapi_config.fastapi_openapi_url,
             docs_url=self.fastapi_config.fastapi_docs_url,
             redoc_url=self.fastapi_config.fastapi_redoc_url,
             **self.fastapi_config.fastapi_extra,
         )
 
     @property
@@ -144,22 +149,28 @@
         self._server_app.add_api_websocket_route(
             setup.path.path,
             _handle,
             name=setup.name,
         )
 
     @overrides(ReverseDriver)
-    def on_startup(self, func: Callable) -> Callable:
-        """参考文档: `Events <https://fastapi.tiangolo.com/advanced/events/#startup-event>`_"""
-        return self.server_app.on_event("startup")(func)
+    def on_startup(self, func: LIFESPAN_FUNC) -> LIFESPAN_FUNC:
+        return self._lifespan.on_startup(func)
 
     @overrides(ReverseDriver)
-    def on_shutdown(self, func: Callable) -> Callable:
-        """参考文档: `Events <https://fastapi.tiangolo.com/advanced/events/#shutdown-event>`_"""
-        return self.server_app.on_event("shutdown")(func)
+    def on_shutdown(self, func: LIFESPAN_FUNC) -> LIFESPAN_FUNC:
+        return self._lifespan.on_shutdown(func)
+
+    @contextlib.asynccontextmanager
+    async def _lifespan_manager(self, app: FastAPI):
+        await self._lifespan.startup()
+        try:
+            yield
+        finally:
+            await self._lifespan.shutdown()
 
     @overrides(ReverseDriver)
     def run(
         self,
         host: Optional[str] = None,
         port: Optional[int] = None,
         *,
```

### Comparing `nonebot2-2.0.0rc3/nonebot/drivers/httpx.py` & `nonebot2-2.0.0rc4/nonebot/drivers/httpx.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,18 +27,18 @@
     ForwardMixin,
     ForwardDriver,
     combine_driver,
 )
 
 try:
     import httpx
-except ImportError:  # pragma: no cover
+except ModuleNotFoundError as e:  # pragma: no cover
     raise ImportError(
         "Please install httpx by using `pip install nonebot2[httpx]`"
-    ) from None
+    ) from e
 
 
 class Mixin(ForwardMixin):
     """HTTPX Mixin"""
 
     @property
     @overrides(ForwardMixin)
```

### Comparing `nonebot2-2.0.0rc3/nonebot/drivers/none.py` & `nonebot2-2.0.0rc4/nonebot/drivers/none.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,36 +9,39 @@
     description: nonebot.drivers.none 模块
 """
 
 
 import signal
 import asyncio
 import threading
-from typing import Set, Union, Callable, Awaitable, cast
 
 from nonebot.log import logger
+from nonebot.consts import WINDOWS
 from nonebot.typing import overrides
 from nonebot.config import Env, Config
 from nonebot.drivers import Driver as BaseDriver
-from nonebot.utils import run_sync, is_coroutine_callable
 
-HOOK_FUNC = Union[Callable[[], None], Callable[[], Awaitable[None]]]
+from ._lifespan import LIFESPAN_FUNC, Lifespan
+
 HANDLED_SIGNALS = (
     signal.SIGINT,  # Unix signal 2. Sent by Ctrl+C.
     signal.SIGTERM,  # Unix signal 15. Sent by `kill <pid>`.
 )
+if WINDOWS:  # pragma: py-win32
+    HANDLED_SIGNALS += (signal.SIGBREAK,)  # Windows signal 21. Sent by Ctrl+Break.
 
 
 class Driver(BaseDriver):
     """None 驱动框架"""
 
     def __init__(self, env: Env, config: Config):
         super().__init__(env, config)
-        self.startup_funcs: Set[HOOK_FUNC] = set()
-        self.shutdown_funcs: Set[HOOK_FUNC] = set()
+
+        self._lifespan = Lifespan()
+
         self.should_exit: asyncio.Event = asyncio.Event()
         self.force_exit: bool = False
 
     @property
     @overrides(BaseDriver)
     def type(self) -> str:
         """驱动名称: `none`"""
@@ -47,28 +50,26 @@
     @property
     @overrides(BaseDriver)
     def logger(self):
         """none driver 使用的 logger"""
         return logger
 
     @overrides(BaseDriver)
-    def on_startup(self, func: HOOK_FUNC) -> HOOK_FUNC:
+    def on_startup(self, func: LIFESPAN_FUNC) -> LIFESPAN_FUNC:
         """
         注册一个启动时执行的函数
         """
-        self.startup_funcs.add(func)
-        return func
+        return self._lifespan.on_startup(func)
 
     @overrides(BaseDriver)
-    def on_shutdown(self, func: HOOK_FUNC) -> HOOK_FUNC:
+    def on_shutdown(self, func: LIFESPAN_FUNC) -> LIFESPAN_FUNC:
         """
         注册一个停止时执行的函数
         """
-        self.shutdown_funcs.add(func)
-        return func
+        return self._lifespan.on_shutdown(func)
 
     @overrides(BaseDriver)
     def run(self, *args, **kwargs):
         """启动 none driver"""
         super().run(*args, **kwargs)
         loop = asyncio.get_event_loop()
         loop.run_until_complete(self._serve())
@@ -78,54 +79,39 @@
         await self._startup()
         if self.should_exit.is_set():
             return
         await self._main_loop()
         await self._shutdown()
 
     async def _startup(self):
-        # run startup
-        cors = [
-            cast(Callable[..., Awaitable[None]], startup)()
-            if is_coroutine_callable(startup)
-            else run_sync(startup)()
-            for startup in self.startup_funcs
-        ]
-        if cors:
-            try:
-                await asyncio.gather(*cors)
-            except Exception as e:
-                logger.opt(colors=True, exception=e).error(
-                    "<r><bg #f8bbd0>Error when running startup function. "
-                    "Ignored!</bg #f8bbd0></r>"
-                )
+        try:
+            await self._lifespan.startup()
+        except Exception as e:
+            logger.opt(colors=True, exception=e).error(
+                "<r><bg #f8bbd0>Error when running startup function. "
+                "Ignored!</bg #f8bbd0></r>"
+            )
 
         logger.info("Application startup completed.")
 
     async def _main_loop(self):
         await self.should_exit.wait()
 
     async def _shutdown(self):
         logger.info("Shutting down")
 
         logger.info("Waiting for application shutdown.")
-        # run shutdown
-        cors = [
-            cast(Callable[..., Awaitable[None]], shutdown)()
-            if is_coroutine_callable(shutdown)
-            else run_sync(shutdown)()
-            for shutdown in self.shutdown_funcs
-        ]
-        if cors:
-            try:
-                await asyncio.gather(*cors)
-            except Exception as e:
-                logger.opt(colors=True, exception=e).error(
-                    "<r><bg #f8bbd0>Error when running shutdown function. "
-                    "Ignored!</bg #f8bbd0></r>"
-                )
+
+        try:
+            await self._lifespan.shutdown()
+        except Exception as e:
+            logger.opt(colors=True, exception=e).error(
+                "<r><bg #f8bbd0>Error when running shutdown function. "
+                "Ignored!</bg #f8bbd0></r>"
+            )
 
         for task in asyncio.all_tasks():
             if task is not asyncio.current_task() and not task.done():
                 task.cancel()
         await asyncio.sleep(0.1)
 
         tasks = [t for t in asyncio.all_tasks() if t is not asyncio.current_task()]
```

### Comparing `nonebot2-2.0.0rc3/nonebot/drivers/quart.py` & `nonebot2-2.0.0rc4/nonebot/drivers/quart.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,18 +33,18 @@
 try:
     import uvicorn
     from quart import request as _request
     from quart import websocket as _websocket
     from quart import Quart, Request, Response
     from quart.datastructures import FileStorage
     from quart import Websocket as QuartWebSocket
-except ImportError:  # pragma: no cover
+except ModuleNotFoundError as e:  # pragma: no cover
     raise ImportError(
         "Please install Quart by using `pip install nonebot2[quart]`"
-    ) from None
+    ) from e
 
 _AsyncCallable = TypeVar("_AsyncCallable", bound=Callable[..., Coroutine])
 
 
 def catch_closed(func):
     @wraps(func)
     async def decorator(*args, **kwargs):
```

### Comparing `nonebot2-2.0.0rc3/nonebot/drivers/websockets.py` & `nonebot2-2.0.0rc4/nonebot/drivers/websockets.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,18 +26,18 @@
 from nonebot.drivers.none import Driver as NoneDriver
 from nonebot.drivers import WebSocket as BaseWebSocket
 from nonebot.drivers import ForwardMixin, ForwardDriver, combine_driver
 
 try:
     from websockets.exceptions import ConnectionClosed
     from websockets.legacy.client import Connect, WebSocketClientProtocol
-except ImportError:  # pragma: no cover
+except ModuleNotFoundError as e:  # pragma: no cover
     raise ImportError(
         "Please install websockets by using `pip install nonebot2[websockets]`"
-    ) from None
+    ) from e
 
 logger = logging.Logger("websockets.client", "INFO")
 logger.addHandler(LoguruHandler())
 
 
 def catch_closed(func):
     @wraps(func)
```

### Comparing `nonebot2-2.0.0rc3/nonebot/exception.py` & `nonebot2-2.0.0rc4/nonebot/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.0.0rc3/nonebot/internal/adapter/adapter.py` & `nonebot2-2.0.0rc4/nonebot/internal/adapter/adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,16 +62,17 @@
         """告知 NoneBot {ref}`nonebot.adapters.Bot` 连接已断开。
 
         当有 {ref}`nonebot.adapters.Bot` 实例连接断开时调用。
 
         参数:
             bot: {ref}`nonebot.adapters.Bot` 实例
         """
+        if self.bots.pop(bot.self_id, None) is None:
+            raise RuntimeError(f"{bot} not found in adapter {self.get_name()}")
         self.driver._bot_disconnect(bot)
-        self.bots.pop(bot.self_id, None)
 
     def setup_http_server(self, setup: HTTPServerSetup):
         """设置一个 HTTP 服务器路由配置"""
         if not isinstance(self.driver, ReverseDriver):
             raise TypeError("Current driver does not support http server")
         self.driver.setup_http_server(setup)
```

### Comparing `nonebot2-2.0.0rc3/nonebot/internal/adapter/bot.py` & `nonebot2-2.0.0rc4/nonebot/internal/adapter/bot.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.0.0rc3/nonebot/internal/adapter/event.py` & `nonebot2-2.0.0rc4/nonebot/internal/adapter/event.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
     def get_log_string(self) -> str:
         """获取事件日志信息的方法。
 
         通常你不需要修改这个方法，只有当希望 NoneBot 隐藏该事件日志时，可以抛出 `NoLogException` 异常。
 
         异常:
-            NoLogException
+            NoLogException:
         """
         return f"[{self.get_event_name()}]: {self.get_event_description()}"
 
     @abc.abstractmethod
     def get_user_id(self) -> str:
         """获取事件主体 id 的方法，通常是用户 id 。"""
         raise NotImplementedError
```

### Comparing `nonebot2-2.0.0rc3/nonebot/internal/adapter/message.py` & `nonebot2-2.0.0rc4/nonebot/internal/adapter/message.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.0.0rc3/nonebot/internal/adapter/template.py` & `nonebot2-2.0.0rc4/nonebot/internal/adapter/template.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,18 +115,17 @@
         args: Sequence[Any],
         kwargs: Mapping[str, Any],
         used_args: Set[Union[int, str]],
         auto_arg_index: int = 0,
     ) -> Tuple[TF, int]:
         results: List[Any] = [self.factory()]
 
-        for (literal_text, field_name, format_spec, conversion) in self.parse(
+        for literal_text, field_name, format_spec, conversion in self.parse(
             format_string
         ):
-
             # output the literal text
             if literal_text:
                 results.append(literal_text)
 
             # if there's a field, output it
             if field_name is not None:
                 # this is some markup, find the object and do
```

### Comparing `nonebot2-2.0.0rc3/nonebot/internal/driver/__init__.py` & `nonebot2-2.0.0rc4/nonebot/internal/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.0.0rc3/nonebot/internal/driver/driver.py` & `nonebot2-2.0.0rc4/nonebot/internal/driver/driver.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 import abc
 import asyncio
-from contextlib import asynccontextmanager
+from contextlib import AsyncExitStack, asynccontextmanager
 from typing import TYPE_CHECKING, Any, Set, Dict, Type, Callable, AsyncGenerator
 
 from nonebot.log import logger
 from nonebot.config import Env, Config
 from nonebot.dependencies import Dependent
 from nonebot.exception import SkippedException
 from nonebot.utils import escape_tag, run_coro_with_catch
-from nonebot.typing import T_BotConnectionHook, T_BotDisconnectionHook
 from nonebot.internal.params import BotParam, DependParam, DefaultParam
+from nonebot.typing import (
+    T_DependencyCache,
+    T_BotConnectionHook,
+    T_BotDisconnectionHook,
+)
 
 from .model import Request, Response, WebSocket, HTTPServerSetup, WebSocketServerSetup
 
 if TYPE_CHECKING:
     from nonebot.internal.adapter import Bot, Adapter
 
 
@@ -131,51 +135,55 @@
     def _bot_connect(self, bot: "Bot") -> None:
         """在连接成功后，调用该函数来注册 bot 对象"""
         if bot.self_id in self._bots:
             raise RuntimeError(f"Duplicate bot connection with id {bot.self_id}")
         self._bots[bot.self_id] = bot
 
         async def _run_hook(bot: "Bot") -> None:
-            coros = list(
-                map(
-                    lambda x: run_coro_with_catch(x(bot=bot), (SkippedException,)),
-                    self._bot_connection_hook,
-                )
-            )
-            if coros:
-                try:
-                    await asyncio.gather(*coros)
-                except Exception as e:
-                    logger.opt(colors=True, exception=e).error(
-                        "<r><bg #f8bbd0>Error when running WebSocketConnection hook. "
-                        "Running cancelled!</bg #f8bbd0></r>"
+            dependency_cache: T_DependencyCache = {}
+            async with AsyncExitStack() as stack:
+                if coros := [
+                    run_coro_with_catch(
+                        hook(bot=bot, stack=stack, dependency_cache=dependency_cache),
+                        (SkippedException,),
                     )
+                    for hook in self._bot_connection_hook
+                ]:
+                    try:
+                        await asyncio.gather(*coros)
+                    except Exception as e:
+                        logger.opt(colors=True, exception=e).error(
+                            "<r><bg #f8bbd0>Error when running WebSocketConnection hook. "
+                            "Running cancelled!</bg #f8bbd0></r>"
+                        )
 
         asyncio.create_task(_run_hook(bot))
 
     def _bot_disconnect(self, bot: "Bot") -> None:
         """在连接断开后，调用该函数来注销 bot 对象"""
         if bot.self_id in self._bots:
             del self._bots[bot.self_id]
 
         async def _run_hook(bot: "Bot") -> None:
-            coros = list(
-                map(
-                    lambda x: run_coro_with_catch(x(bot=bot), (SkippedException,)),
-                    self._bot_disconnection_hook,
-                )
-            )
-            if coros:
-                try:
-                    await asyncio.gather(*coros)
-                except Exception as e:
-                    logger.opt(colors=True, exception=e).error(
-                        "<r><bg #f8bbd0>Error when running WebSocketDisConnection hook. "
-                        "Running cancelled!</bg #f8bbd0></r>"
+            dependency_cache: T_DependencyCache = {}
+            async with AsyncExitStack() as stack:
+                if coros := [
+                    run_coro_with_catch(
+                        hook(bot=bot, stack=stack, dependency_cache=dependency_cache),
+                        (SkippedException,),
                     )
+                    for hook in self._bot_disconnection_hook
+                ]:
+                    try:
+                        await asyncio.gather(*coros)
+                    except Exception as e:
+                        logger.opt(colors=True, exception=e).error(
+                            "<r><bg #f8bbd0>Error when running WebSocketDisConnection hook. "
+                            "Running cancelled!</bg #f8bbd0></r>"
+                        )
 
         asyncio.create_task(_run_hook(bot))
 
 
 class ForwardMixin(abc.ABC):
     """客户端混入基类。"""
```

### Comparing `nonebot2-2.0.0rc3/nonebot/internal/driver/model.py` & `nonebot2-2.0.0rc4/nonebot/internal/driver/model.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.0.0rc3/nonebot/internal/matcher/manager.py` & `nonebot2-2.0.0rc4/nonebot/internal/matcher/manager.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.0.0rc3/nonebot/internal/matcher/matcher.py` & `nonebot2-2.0.0rc4/nonebot/internal/matcher/matcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 from types import ModuleType
 from contextvars import ContextVar
+from typing_extensions import Self
 from datetime import datetime, timedelta
 from contextlib import AsyncExitStack, contextmanager
 from typing import (
     TYPE_CHECKING,
     Any,
     List,
     Type,
     Union,
     TypeVar,
     Callable,
+    ClassVar,
     Iterable,
     NoReturn,
     Optional,
     overload,
 )
 
 from nonebot.log import logger
 from nonebot.internal.rule import Rule
 from nonebot.dependencies import Dependent
-from nonebot.internal.permission import USER, User, Permission
+from nonebot.internal.permission import User, Permission
 from nonebot.internal.adapter import (
     Bot,
     Event,
     Message,
     MessageSegment,
     MessageTemplate,
 )
@@ -76,55 +78,55 @@
 class MatcherMeta(type):
     if TYPE_CHECKING:
         module_name: Optional[str]
         type: str
 
     def __repr__(self) -> str:
         return (
-            f"Matcher(type={self.type!r}"
+            f"{self.__name__}(type={self.type!r}"
             + (f", module={self.module_name}" if self.module_name else "")
             + ")"
         )
 
 
 class Matcher(metaclass=MatcherMeta):
     """事件响应器类"""
 
-    plugin: Optional["Plugin"] = None
+    plugin: ClassVar[Optional["Plugin"]] = None
     """事件响应器所在插件"""
-    module: Optional[ModuleType] = None
+    module: ClassVar[Optional[ModuleType]] = None
     """事件响应器所在插件模块"""
-    plugin_name: Optional[str] = None
+    plugin_name: ClassVar[Optional[str]] = None
     """事件响应器所在插件名"""
-    module_name: Optional[str] = None
+    module_name: ClassVar[Optional[str]] = None
     """事件响应器所在点分割插件模块路径"""
 
-    type: str = ""
+    type: ClassVar[str] = ""
     """事件响应器类型"""
-    rule: Rule = Rule()
+    rule: ClassVar[Rule] = Rule()
     """事件响应器匹配规则"""
-    permission: Permission = Permission()
+    permission: ClassVar[Permission] = Permission()
     """事件响应器触发权限"""
     handlers: List[Dependent[Any]] = []
     """事件响应器拥有的事件处理函数列表"""
-    priority: int = 1
+    priority: ClassVar[int] = 1
     """事件响应器优先级"""
     block: bool = False
     """事件响应器是否阻止事件传播"""
-    temp: bool = False
+    temp: ClassVar[bool] = False
     """事件响应器是否为临时"""
-    expire_time: Optional[datetime] = None
+    expire_time: ClassVar[Optional[datetime]] = None
     """事件响应器过期时间点"""
 
-    _default_state: T_State = {}
+    _default_state: ClassVar[T_State] = {}
     """事件响应器默认状态"""
 
-    _default_type_updater: Optional[Dependent[str]] = None
+    _default_type_updater: ClassVar[Optional[Dependent[str]]] = None
     """事件响应器类型更新函数"""
-    _default_permission_updater: Optional[Dependent[Permission]] = None
+    _default_permission_updater: ClassVar[Optional[Dependent[Permission]]] = None
     """事件响应器权限更新函数"""
 
     HANDLER_PARAM_TYPES = (
         DependParam,
         BotParam,
         EventParam,
         StateParam,
@@ -135,15 +137,15 @@
 
     def __init__(self):
         self.handlers = self.handlers.copy()
         self.state = self._default_state.copy()
 
     def __repr__(self) -> str:
         return (
-            f"Matcher(type={self.type!r}"
+            f"{self.__class__.__name__}(type={self.type!r}"
             + (f", module={self.module_name}" if self.module_name else "")
             + ")"
         )
 
     @classmethod
     def new(
         cls,
@@ -159,15 +161,15 @@
         module: Optional[ModuleType] = None,
         expire_time: Optional[Union[datetime, timedelta]] = None,
         default_state: Optional[T_State] = None,
         default_type_updater: Optional[Union[T_TypeUpdater, Dependent[str]]] = None,
         default_permission_updater: Optional[
             Union[T_PermissionUpdater, Dependent[Permission]]
         ] = None,
-    ) -> Type["Matcher"]:
+    ) -> Type[Self]:
         """
         创建一个新的事件响应器，并存储至 `matchers <#matchers>`_
 
         参数:
             type_: 事件响应器类型，与 `event.get_type()` 一致时触发，空字符串表示任意
             rule: 匹配规则
             permission: 权限
@@ -180,16 +182,16 @@
             default_state: 默认状态 `state`
             expire_time: 事件响应器最终有效时间点，过时即被删除
 
         返回:
             Type[Matcher]: 新的事件响应器类
         """
         NewMatcher = type(
-            "Matcher",
-            (Matcher,),
+            cls.__name__,
+            (cls,),
             {
                 "plugin": plugin,
                 "module": module,
                 "plugin_name": plugin and plugin.name,
                 "module_name": module and module.__name__,
                 "type": type_,
                 "rule": rule or Rule(),
@@ -373,15 +375,14 @@
             if matcher.get_receive(id, ...) is not ...:
                 return
             await matcher.reject()
 
         _parameterless = (Depends(_receive), *(parameterless or tuple()))
 
         def _decorator(func: T_Handler) -> T_Handler:
-
             if cls.handlers and cls.handlers[-1].call is func:
                 func_handler = cls.handlers[-1]
                 new_handler = Dependent(
                     call=func_handler.call,
                     params=func_handler.params,
                     parameterless=Dependent.parse_parameterless(
                         tuple(_parameterless), cls.HANDLER_PARAM_TYPES
@@ -421,15 +422,14 @@
             if matcher.get_arg(key, ...) is not ...:
                 return
             await matcher.reject(prompt)
 
         _parameterless = (Depends(_key_getter), *(parameterless or tuple()))
 
         def _decorator(func: T_Handler) -> T_Handler:
-
             if cls.handlers and cls.handlers[-1].call is func:
                 func_handler = cls.handlers[-1]
                 new_handler = Dependent(
                     call=func_handler.call,
                     params=func_handler.params,
                     parameterless=Dependent.parse_parameterless(
                         tuple(_parameterless), cls.HANDLER_PARAM_TYPES
@@ -641,31 +641,52 @@
     def get_target(self, default: Optional[T] = None) -> Optional[Union[str, T]]:
         return self.state.get(REJECT_TARGET, default)
 
     def stop_propagation(self):
         """阻止事件传播"""
         self.block = True
 
-    async def update_type(self, bot: Bot, event: Event) -> str:
+    async def update_type(
+        self,
+        bot: Bot,
+        event: Event,
+        stack: Optional[AsyncExitStack] = None,
+        dependency_cache: Optional[T_DependencyCache] = None,
+    ) -> str:
         updater = self.__class__._default_type_updater
         return (
-            await updater(bot=bot, event=event, state=self.state, matcher=self)
+            await updater(
+                bot=bot,
+                event=event,
+                state=self.state,
+                matcher=self,
+                stack=stack,
+                dependency_cache=dependency_cache,
+            )
             if updater
             else "message"
         )
 
-    async def update_permission(self, bot: Bot, event: Event) -> Permission:
+    async def update_permission(
+        self,
+        bot: Bot,
+        event: Event,
+        stack: Optional[AsyncExitStack] = None,
+        dependency_cache: Optional[T_DependencyCache] = None,
+    ) -> Permission:
         if updater := self.__class__._default_permission_updater:
-            return await updater(bot=bot, event=event, state=self.state, matcher=self)
-        permission = self.permission
-        if len(permission.checkers) == 1 and isinstance(
-            user_perm := tuple(permission.checkers)[0].call, User
-        ):
-            permission = user_perm.perm
-        return USER(event.get_session_id(), perm=permission)
+            return await updater(
+                bot=bot,
+                event=event,
+                state=self.state,
+                matcher=self,
+                stack=stack,
+                dependency_cache=dependency_cache,
+            )
+        return Permission(User.from_event(event, perm=self.permission))
 
     async def resolve_reject(self):
         handler = current_handler.get()
         self.handlers.insert(0, handler)
         if REJECT_CACHE_TARGET in self.state:
             self.state[REJECT_TARGET] = self.state[REJECT_CACHE_TARGET]
 
@@ -729,18 +750,20 @@
         dependency_cache: Optional[T_DependencyCache] = None,
     ):
         try:
             await self.simple_run(bot, event, state, stack, dependency_cache)
 
         except RejectedException:
             await self.resolve_reject()
-            type_ = await self.update_type(bot, event)
-            permission = await self.update_permission(bot, event)
+            type_ = await self.update_type(bot, event, stack, dependency_cache)
+            permission = await self.update_permission(
+                bot, event, stack, dependency_cache
+            )
 
-            Matcher.new(
+            self.new(
                 type_,
                 Rule(),
                 permission,
                 self.handlers,
                 temp=True,
                 priority=0,
                 block=True,
@@ -748,18 +771,20 @@
                 module=self.module,
                 expire_time=bot.config.session_expire_timeout,
                 default_state=self.state,
                 default_type_updater=self.__class__._default_type_updater,
                 default_permission_updater=self.__class__._default_permission_updater,
             )
         except PausedException:
-            type_ = await self.update_type(bot, event)
-            permission = await self.update_permission(bot, event)
+            type_ = await self.update_type(bot, event, stack, dependency_cache)
+            permission = await self.update_permission(
+                bot, event, stack, dependency_cache
+            )
 
-            Matcher.new(
+            self.new(
                 type_,
                 Rule(),
                 permission,
                 self.handlers,
                 temp=True,
                 priority=0,
                 block=True,
```

### Comparing `nonebot2-2.0.0rc3/nonebot/internal/matcher/provider.py` & `nonebot2-2.0.0rc4/nonebot/internal/matcher/provider.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.0.0rc3/nonebot/internal/params.py` & `nonebot2-2.0.0rc4/nonebot/internal/params.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import asyncio
 import inspect
+from typing_extensions import Annotated
 from contextlib import AsyncExitStack, contextmanager, asynccontextmanager
 from typing import TYPE_CHECKING, Any, Type, Tuple, Literal, Callable, Optional, cast
 
+from pydantic.typing import get_args, get_origin
 from pydantic.fields import Required, Undefined, ModelField
 
 from nonebot.dependencies.utils import check_field_type
 from nonebot.dependencies import Param, Dependent, CustomConfig
 from nonebot.typing import T_State, T_Handler, T_DependencyCache
 from nonebot.utils import (
     get_name,
@@ -74,29 +76,41 @@
     def __repr__(self) -> str:
         return f"Depends({self.extra['dependent']})"
 
     @classmethod
     def _check_param(
         cls, param: inspect.Parameter, allow_types: Tuple[Type[Param], ...]
     ) -> Optional["DependParam"]:
-        if isinstance(param.default, DependsInner):
-            dependency: T_Handler
-            if param.default.dependency is None:
-                assert param.annotation is not param.empty, "Dependency cannot be empty"
-                dependency = param.annotation
-            else:
-                dependency = param.default.dependency
-            sub_dependent = Dependent[Any].parse(
-                call=dependency,
-                allow_types=allow_types,
-            )
-            return cls(
-                Required, use_cache=param.default.use_cache, dependent=sub_dependent
+        type_annotation, depends_inner = param.annotation, None
+        if get_origin(param.annotation) is Annotated:
+            type_annotation, *extra_args = get_args(param.annotation)
+            depends_inner = next(
+                (x for x in extra_args if isinstance(x, DependsInner)), None
             )
 
+        depends_inner = (
+            param.default if isinstance(param.default, DependsInner) else depends_inner
+        )
+        if depends_inner is None:
+            return
+
+        dependency: T_Handler
+        if depends_inner.dependency is None:
+            assert (
+                type_annotation is not inspect.Signature.empty
+            ), "Dependency cannot be empty"
+            dependency = type_annotation
+        else:
+            dependency = depends_inner.dependency
+        sub_dependent = Dependent[Any].parse(
+            call=dependency,
+            allow_types=allow_types,
+        )
+        return cls(Required, use_cache=depends_inner.use_cache, dependent=sub_dependent)
+
     @classmethod
     def _check_parameterless(
         cls, value: Any, allow_types: Tuple[Type[Param], ...]
     ) -> Optional["Param"]:
         if isinstance(value, DependsInner):
             assert value.dependency, "Dependency cannot be empty"
             dependent = Dependent[Any].parse(
```

### Comparing `nonebot2-2.0.0rc3/nonebot/internal/permission.py` & `nonebot2-2.0.0rc4/nonebot/internal/permission.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+from typing_extensions import Self
 from contextlib import AsyncExitStack
 from typing import Set, Tuple, Union, NoReturn, Optional
 
 from nonebot.dependencies import Dependent
 from nonebot.utils import run_coro_with_catch
 from nonebot.exception import SkippedException
 from nonebot.typing import T_DependencyCache, T_PermissionChecker
@@ -53,15 +54,15 @@
     async def __call__(
         self,
         bot: Bot,
         event: Event,
         stack: Optional[AsyncExitStack] = None,
         dependency_cache: Optional[T_DependencyCache] = None,
     ) -> bool:
-        """检查是否满足某个权限
+        """检查是否满足某个权限。
 
         参数:
             bot: Bot 对象
             event: Event 对象
             stack: 异步上下文栈
             dependency_cache: 依赖缓存
         """
@@ -105,15 +106,15 @@
         elif isinstance(other, Permission):
             return Permission(*other.checkers, *self.checkers)
         else:
             return Permission(other, *self.checkers)
 
 
 class User:
-    """检查当前事件是否属于指定会话
+    """检查当前事件是否属于指定会话。
 
     参数:
         users: 会话 ID 元组
         perm: 需同时满足的权限
     """
 
     __slots__ = ("users", "perm")
@@ -136,17 +137,51 @@
             session = event.get_session_id()
         except Exception:
             return False
         return bool(
             session in self.users and (self.perm is None or await self.perm(bot, event))
         )
 
+    @classmethod
+    def _clean_permission(cls, perm: Permission) -> Optional[Permission]:
+        if len(perm.checkers) == 1 and isinstance(
+            user_perm := tuple(perm.checkers)[0].call, cls
+        ):
+            return user_perm.perm
+        return perm
+
+    @classmethod
+    def from_event(cls, event: Event, perm: Optional[Permission] = None) -> Self:
+        """从事件中获取会话 ID。
+
+        如果 `perm` 中仅有 `User` 类型的权限检查函数，则会去除原有的会话 ID 限制。
+
+        参数:
+            event: Event 对象
+            perm: 需同时满足的权限
+        """
+        return cls((event.get_session_id(),), perm=perm and cls._clean_permission(perm))
+
+    @classmethod
+    def from_permission(cls, *users: str, perm: Optional[Permission] = None) -> Self:
+        """指定会话与权限。
+
+        如果 `perm` 中仅有 `User` 类型的权限检查函数，则会去除原有的会话 ID 限制。
+
+        参数:
+            users: 会话白名单
+            perm: 需同时满足的权限
+        """
+        return cls(users, perm=perm and cls._clean_permission(perm))
+
 
 def USER(*users: str, perm: Optional[Permission] = None):
-    """匹配当前事件属于指定会话
+    """匹配当前事件属于指定会话。
+
+    如果 `perm` 中仅有 `User` 类型的权限检查函数，则会去除原有检查函数的会话 ID 限制。
 
     参数:
         user: 会话白名单
         perm: 需要同时满足的权限
     """
 
-    return Permission(User(users, perm))
+    return Permission(User.from_permission(*users, perm=perm))
```

### Comparing `nonebot2-2.0.0rc3/nonebot/internal/rule.py` & `nonebot2-2.0.0rc4/nonebot/internal/rule.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.0.0rc3/nonebot/log.py` & `nonebot2-2.0.0rc4/nonebot/log.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """本模块定义了 NoneBot 的日志记录 Logger。
 
 NoneBot 使用 [`loguru`][loguru] 来记录日志信息。
 
-自定义 logger 请参考 [自定义日志](https://v2.nonebot.dev/docs/tutorial/custom-logger)
+自定义 logger 请参考 [自定义日志](https://v2.nonebot.dev/docs/appendices/log)
 以及 [`loguru`][loguru] 文档。
 
 [loguru]: https://github.com/Delgan/loguru
 
 FrontMatter:
     sidebar_position: 7
     description: nonebot.log 模块
```

### Comparing `nonebot2-2.0.0rc3/nonebot/matcher.py` & `nonebot2-2.0.0rc4/nonebot/matcher.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.0.0rc3/nonebot/message.py` & `nonebot2-2.0.0rc4/nonebot/message.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.0.0rc3/nonebot/params.py` & `nonebot2-2.0.0rc4/nonebot/params.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     RAW_CMD_KEY,
     REGEX_GROUP,
     ENDSWITH_KEY,
     CMD_START_KEY,
     FULLMATCH_KEY,
     REGEX_MATCHED,
     STARTSWITH_KEY,
+    CMD_WHITESPACE_KEY,
 )
 
 
 async def _event_type(event: Event) -> str:
     return event.get_type()
 
 
@@ -110,14 +111,23 @@
 
 
 def CommandStart() -> str:
     """消息命令开头"""
     return Depends(_command_start)
 
 
+def _command_whitespace(state: T_State) -> str:
+    return state[PREFIX_KEY][CMD_WHITESPACE_KEY]
+
+
+def CommandWhitespace() -> str:
+    """消息命令与参数之间的空白"""
+    return Depends(_command_whitespace)
+
+
 def _shell_command_args(state: T_State) -> Any:
     return state[SHELL_ARGS]  # Namespace or ParserExit
 
 
 def ShellCommandArgs() -> Any:
     """shell 命令解析后的参数字典"""
     return Depends(_shell_command_args, use_cache=False)
```

### Comparing `nonebot2-2.0.0rc3/nonebot/permission.py` & `nonebot2-2.0.0rc4/nonebot/permission.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.0.0rc3/nonebot/plugin/__init__.py` & `nonebot2-2.0.0rc4/nonebot/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.0.0rc3/nonebot/plugin/load.py` & `nonebot2-2.0.0rc4/nonebot/plugin/load.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,22 +5,25 @@
     description: nonebot.plugin.load 模块
 """
 import json
 from pathlib import Path
 from types import ModuleType
 from typing import Set, Union, Iterable, Optional
 
-import tomlkit
-
 from nonebot.utils import path_to_module_name
 
 from .plugin import Plugin
 from .manager import PluginManager
 from . import _managers, get_plugin, _module_name_to_plugin_name
 
+try:  # pragma: py-gte-311
+    import tomllib  # pyright: reportMissingImports=false
+except ModuleNotFoundError:  # pragma: py-lt-311
+    import tomli as tomllib
+
 
 def load_plugin(module_path: Union[str, Path]) -> Optional[Plugin]:
     """加载单个插件，可以是本地插件或是通过 `pip` 安装的插件。
 
     参数:
         module_path: 插件名称 `path.to.your.plugin` 或插件路径 `pathlib.Path(path/to/your/plugin)`
     """
@@ -104,15 +107,15 @@
         ```
 
         ```python
         nonebot.load_from_toml("pyproject.toml")
         ```
     """
     with open(file_path, "r", encoding=encoding) as f:
-        data = tomlkit.parse(f.read())  # type: ignore
+        data = tomllib.loads(f.read())
 
     nonebot_data = data.get("tool", {}).get("nonebot")
     if nonebot_data is None:
         raise ValueError("Cannot find '[tool.nonebot]' in given toml file!")
     if not isinstance(nonebot_data, dict):
         raise TypeError("'[tool.nonebot]' must be a Table!")
     plugins = nonebot_data.get("plugins", [])
```

### Comparing `nonebot2-2.0.0rc3/nonebot/plugin/manager.py` & `nonebot2-2.0.0rc4/nonebot/plugin/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,22 +144,29 @@
             elif name in self._searched_plugin_names:
                 module = importlib.import_module(
                     path_to_module_name(self._searched_plugin_names[name])
                 )
             else:
                 raise RuntimeError(f"Plugin not found: {name}! Check your plugin name")
 
-            logger.opt(colors=True).success(
-                f'Succeeded to import "<y>{escape_tag(name)}</y>"'
-            )
-            if (plugin := getattr(module, "__plugin__", None)) is None:
+            if (
+                plugin := getattr(module, "__plugin__", None)
+            ) is None or not isinstance(plugin, Plugin):
                 raise RuntimeError(
                     f"Module {module.__name__} is not loaded as a plugin! "
                     "Make sure not to import it before loading."
                 )
+            logger.opt(colors=True).success(
+                f'Succeeded to load plugin "<y>{escape_tag(plugin.name)}</y>"'
+                + (
+                    f' from "<m>{escape_tag(plugin.module_name)}</m>"'
+                    if plugin.module_name != plugin.name
+                    else ""
+                )
+            )
             return plugin
         except Exception as e:
             logger.opt(colors=True, exception=e).error(
                 f'<r><bg #f8bbd0>Failed to import "{escape_tag(name)}"</bg #f8bbd0></r>'
             )
 
     def load_all_plugins(self) -> Set[Plugin]:
```

### Comparing `nonebot2-2.0.0rc3/nonebot/plugin/on.py` & `nonebot2-2.0.0rc4/nonebot/plugin/on.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,24 +24,52 @@
     keyword,
     endswith,
     fullmatch,
     startswith,
     shell_command,
 )
 
+from .plugin import Plugin
+from . import get_plugin_by_module_name
 from .manager import _current_plugin_chain
 
 
-def _store_matcher(matcher: Type[Matcher]) -> None:
-    # only store the matcher defined in the plugin
-    if plugins := _current_plugin_chain.get():
-        plugins[-1].matcher.add(matcher)
+def store_matcher(matcher: Type[Matcher]) -> None:
+    """存储一个事件响应器到插件。
 
+    参数:
+        matcher: 事件响应器
+    """
+    # only store the matcher defined when plugin loading
+    if plugin_chain := _current_plugin_chain.get():
+        plugin_chain[-1].matcher.add(matcher)
+
+
+def get_matcher_plugin(depth: int = 1) -> Optional[Plugin]:
+    """获取事件响应器定义所在插件。
+
+    参数:
+        depth: 调用栈深度
+    """
+    # matcher defined when plugin loading
+    if plugin_chain := _current_plugin_chain.get():
+        return plugin_chain[-1]
 
-def _get_matcher_module(depth: int = 1) -> Optional[ModuleType]:
+    # matcher defined when plugin running
+    if module := get_matcher_module(depth + 1):
+        if plugin := get_plugin_by_module_name(module.__name__):
+            return plugin
+
+
+def get_matcher_module(depth: int = 1) -> Optional[ModuleType]:
+    """获取事件响应器定义所在模块。
+
+    参数:
+        depth: 调用栈深度
+    """
     current_frame = inspect.currentframe()
     if current_frame is None:
         return None
     frame = inspect.getouterframes(current_frame)[depth + 1].frame
     return inspect.getmodule(frame)
 
 
@@ -67,192 +95,94 @@
         handlers: 事件处理函数列表
         temp: 是否为临时事件响应器（仅执行一次）
         expire_time: 事件响应器最终有效时间点，过时即被删除
         priority: 事件响应器优先级
         block: 是否阻止事件向更低优先级传递
         state: 默认 state
     """
-    plugin_chain = _current_plugin_chain.get()
     matcher = Matcher.new(
         type,
         Rule() & rule,
         Permission() | permission,
         temp=temp,
         expire_time=expire_time,
         priority=priority,
         block=block,
         handlers=handlers,
-        plugin=plugin_chain[-1] if plugin_chain else None,
-        module=_get_matcher_module(_depth + 1),
+        plugin=get_matcher_plugin(_depth + 1),
+        module=get_matcher_module(_depth + 1),
         default_state=state,
     )
-    _store_matcher(matcher)
+    store_matcher(matcher)
     return matcher
 
 
-def on_metaevent(
-    rule: Optional[Union[Rule, T_RuleChecker]] = None,
-    *,
-    handlers: Optional[List[Union[T_Handler, Dependent]]] = None,
-    temp: bool = False,
-    expire_time: Optional[Union[datetime, timedelta]] = None,
-    priority: int = 1,
-    block: bool = False,
-    state: Optional[T_State] = None,
-    _depth: int = 0,
-) -> Type[Matcher]:
+def on_metaevent(*args, _depth: int = 0, **kwargs) -> Type[Matcher]:
     """注册一个元事件响应器。
 
     参数:
         rule: 事件响应规则
+        permission: 事件响应权限
         handlers: 事件处理函数列表
         temp: 是否为临时事件响应器（仅执行一次）
         expire_time: 事件响应器最终有效时间点，过时即被删除
         priority: 事件响应器优先级
         block: 是否阻止事件向更低优先级传递
         state: 默认 state
     """
-    plugin_chain = _current_plugin_chain.get()
-    matcher = Matcher.new(
-        "meta_event",
-        Rule() & rule,
-        Permission(),
-        temp=temp,
-        expire_time=expire_time,
-        priority=priority,
-        block=block,
-        handlers=handlers,
-        plugin=plugin_chain[-1] if plugin_chain else None,
-        module=_get_matcher_module(_depth + 1),
-        default_state=state,
-    )
-    _store_matcher(matcher)
-    return matcher
+    return on("meta_event", *args, **kwargs, _depth=_depth + 1)
 
 
-def on_message(
-    rule: Optional[Union[Rule, T_RuleChecker]] = None,
-    permission: Optional[Union[Permission, T_PermissionChecker]] = None,
-    *,
-    handlers: Optional[List[Union[T_Handler, Dependent]]] = None,
-    temp: bool = False,
-    expire_time: Optional[Union[datetime, timedelta]] = None,
-    priority: int = 1,
-    block: bool = True,
-    state: Optional[T_State] = None,
-    _depth: int = 0,
-) -> Type[Matcher]:
+def on_message(*args, _depth: int = 0, **kwargs) -> Type[Matcher]:
     """注册一个消息事件响应器。
 
     参数:
         rule: 事件响应规则
         permission: 事件响应权限
         handlers: 事件处理函数列表
         temp: 是否为临时事件响应器（仅执行一次）
         expire_time: 事件响应器最终有效时间点，过时即被删除
         priority: 事件响应器优先级
         block: 是否阻止事件向更低优先级传递
         state: 默认 state
     """
-    plugin_chain = _current_plugin_chain.get()
-    matcher = Matcher.new(
-        "message",
-        Rule() & rule,
-        Permission() | permission,
-        temp=temp,
-        expire_time=expire_time,
-        priority=priority,
-        block=block,
-        handlers=handlers,
-        plugin=plugin_chain[-1] if plugin_chain else None,
-        module=_get_matcher_module(_depth + 1),
-        default_state=state,
-    )
-    _store_matcher(matcher)
-    return matcher
+    kwargs.setdefault("block", True)
+    return on("message", *args, **kwargs, _depth=_depth + 1)
 
 
-def on_notice(
-    rule: Optional[Union[Rule, T_RuleChecker]] = None,
-    *,
-    handlers: Optional[List[Union[T_Handler, Dependent]]] = None,
-    temp: bool = False,
-    expire_time: Optional[Union[datetime, timedelta]] = None,
-    priority: int = 1,
-    block: bool = False,
-    state: Optional[T_State] = None,
-    _depth: int = 0,
-) -> Type[Matcher]:
+def on_notice(*args, _depth: int = 0, **kwargs) -> Type[Matcher]:
     """注册一个通知事件响应器。
 
     参数:
         rule: 事件响应规则
+        permission: 事件响应权限
         handlers: 事件处理函数列表
         temp: 是否为临时事件响应器（仅执行一次）
         expire_time: 事件响应器最终有效时间点，过时即被删除
         priority: 事件响应器优先级
         block: 是否阻止事件向更低优先级传递
         state: 默认 state
     """
-    plugin_chain = _current_plugin_chain.get()
-    matcher = Matcher.new(
-        "notice",
-        Rule() & rule,
-        Permission(),
-        temp=temp,
-        expire_time=expire_time,
-        priority=priority,
-        block=block,
-        handlers=handlers,
-        plugin=plugin_chain[-1] if plugin_chain else None,
-        module=_get_matcher_module(_depth + 1),
-        default_state=state,
-    )
-    _store_matcher(matcher)
-    return matcher
+    return on("notice", *args, **kwargs, _depth=_depth + 1)
 
 
-def on_request(
-    rule: Optional[Union[Rule, T_RuleChecker]] = None,
-    *,
-    handlers: Optional[List[Union[T_Handler, Dependent]]] = None,
-    temp: bool = False,
-    expire_time: Optional[Union[datetime, timedelta]] = None,
-    priority: int = 1,
-    block: bool = False,
-    state: Optional[T_State] = None,
-    _depth: int = 0,
-) -> Type[Matcher]:
+def on_request(*args, _depth: int = 0, **kwargs) -> Type[Matcher]:
     """注册一个请求事件响应器。
 
     参数:
         rule: 事件响应规则
+        permission: 事件响应权限
         handlers: 事件处理函数列表
         temp: 是否为临时事件响应器（仅执行一次）
         expire_time: 事件响应器最终有效时间点，过时即被删除
         priority: 事件响应器优先级
         block: 是否阻止事件向更低优先级传递
         state: 默认 state
     """
-    plugin_chain = _current_plugin_chain.get()
-    matcher = Matcher.new(
-        "request",
-        Rule() & rule,
-        Permission(),
-        temp=temp,
-        expire_time=expire_time,
-        priority=priority,
-        block=block,
-        handlers=handlers,
-        plugin=plugin_chain[-1] if plugin_chain else None,
-        module=_get_matcher_module(_depth + 1),
-        default_state=state,
-    )
-    _store_matcher(matcher)
-    return matcher
+    return on("request", *args, **kwargs, _depth=_depth + 1)
 
 
 def on_startswith(
     msg: Union[str, Tuple[str, ...]],
     rule: Optional[Union[Rule, T_RuleChecker]] = None,
     ignorecase: bool = False,
     _depth: int = 0,
@@ -345,38 +275,42 @@
     return on_message(keyword(*keywords) & rule, **kwargs, _depth=_depth + 1)
 
 
 def on_command(
     cmd: Union[str, Tuple[str, ...]],
     rule: Optional[Union[Rule, T_RuleChecker]] = None,
     aliases: Optional[Set[Union[str, Tuple[str, ...]]]] = None,
+    force_whitespace: Optional[Union[str, bool]] = None,
     _depth: int = 0,
     **kwargs,
 ) -> Type[Matcher]:
     """注册一个消息事件响应器，并且当消息以指定命令开头时响应。
 
     命令匹配规则参考: `命令形式匹配 <rule.md#command-command>`_
 
     参数:
         cmd: 指定命令内容
         rule: 事件响应规则
         aliases: 命令别名
+        force_whitespace: 是否强制命令后必须有指定空白符
         permission: 事件响应权限
         handlers: 事件处理函数列表
         temp: 是否为临时事件响应器（仅执行一次）
         expire_time: 事件响应器最终有效时间点，过时即被删除
         priority: 事件响应器优先级
         block: 是否阻止事件向更低优先级传递
         state: 默认 state
     """
 
     commands = {cmd} | (aliases or set())
-    block = kwargs.pop("block", False)
+    kwargs.setdefault("block", False)
     return on_message(
-        command(*commands) & rule, block=block, **kwargs, _depth=_depth + 1
+        command(*commands, force_whitespace=force_whitespace) & rule,
+        **kwargs,
+        _depth=_depth + 1,
     )
 
 
 def on_shell_command(
     cmd: Union[str, Tuple[str, ...]],
     rule: Optional[Union[Rule, T_RuleChecker]] = None,
     aliases: Optional[Set[Union[str, Tuple[str, ...]]]] = None,
@@ -514,14 +448,15 @@
 
     def command(self, cmd: Union[str, Tuple[str, ...]], **kwargs) -> Type[Matcher]:
         """注册一个新的命令。新参数将会覆盖命令组默认值
 
         参数:
             cmd: 指定命令内容
             aliases: 命令别名
+            force_whitespace: 是否强制命令后必须有指定空白符
             rule: 事件响应规则
             permission: 事件响应权限
             handlers: 事件处理函数列表
             temp: 是否为临时事件响应器（仅执行一次）
             expire_time: 事件响应器最终有效时间点，过时即被删除
             priority: 事件响应器优先级
             block: 是否阻止事件向更低优先级传递
@@ -583,14 +518,15 @@
         return matcher
 
     def on_metaevent(self, **kwargs) -> Type[Matcher]:
         """注册一个元事件响应器。
 
         参数:
             rule: 事件响应规则
+            permission: 事件响应权限
             handlers: 事件处理函数列表
             temp: 是否为临时事件响应器（仅执行一次）
             expire_time: 事件响应器最终有效时间点，过时即被删除
             priority: 事件响应器优先级
             block: 是否阻止事件向更低优先级传递
             state: 默认 state
         """
@@ -618,14 +554,15 @@
         return matcher
 
     def on_notice(self, **kwargs) -> Type[Matcher]:
         """注册一个通知事件响应器。
 
         参数:
             rule: 事件响应规则
+            permission: 事件响应权限
             handlers: 事件处理函数列表
             temp: 是否为临时事件响应器（仅执行一次）
             expire_time: 事件响应器最终有效时间点，过时即被删除
             priority: 事件响应器优先级
             block: 是否阻止事件向更低优先级传递
             state: 默认 state
         """
@@ -635,14 +572,15 @@
         return matcher
 
     def on_request(self, **kwargs) -> Type[Matcher]:
         """注册一个请求事件响应器。
 
         参数:
             rule: 事件响应规则
+            permission: 事件响应权限
             handlers: 事件处理函数列表
             temp: 是否为临时事件响应器（仅执行一次）
             expire_time: 事件响应器最终有效时间点，过时即被删除
             priority: 事件响应器优先级
             block: 是否阻止事件向更低优先级传递
             state: 默认 state
         """
@@ -732,34 +670,38 @@
         self.matchers.append(matcher)
         return matcher
 
     def on_command(
         self,
         cmd: Union[str, Tuple[str, ...]],
         aliases: Optional[Set[Union[str, Tuple[str, ...]]]] = None,
+        force_whitespace: Optional[Union[str, bool]] = None,
         **kwargs,
     ) -> Type[Matcher]:
         """注册一个消息事件响应器，并且当消息以指定命令开头时响应。
 
         命令匹配规则参考: `命令形式匹配 <rule.md#command-command>`_
 
         参数:
             cmd: 指定命令内容
             aliases: 命令别名
+            force_whitespace: 是否强制命令后必须有指定空白符
             rule: 事件响应规则
             permission: 事件响应权限
             handlers: 事件处理函数列表
             temp: 是否为临时事件响应器（仅执行一次）
             expire_time: 事件响应器最终有效时间点，过时即被删除
             priority: 事件响应器优先级
             block: 是否阻止事件向更低优先级传递
             state: 默认 state
         """
         final_kwargs = self._get_final_kwargs(kwargs, exclude={"type"})
-        matcher = on_command(cmd, aliases=aliases, **final_kwargs)
+        matcher = on_command(
+            cmd, aliases=aliases, force_whitespace=force_whitespace, **final_kwargs
+        )
         self.matchers.append(matcher)
         return matcher
 
     def on_shell_command(
         self,
         cmd: Union[str, Tuple[str, ...]],
         aliases: Optional[Set[Union[str, Tuple[str, ...]]]] = None,
```

### Comparing `nonebot2-2.0.0rc3/nonebot/plugin/on.pyi` & `nonebot2-2.0.0rc4/nonebot/plugin/on.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 import re
+from types import ModuleType
 from datetime import datetime, timedelta
 from typing import Set, List, Type, Tuple, Union, Optional
 
 from nonebot.adapters import Event
 from nonebot.matcher import Matcher
 from nonebot.permission import Permission
 from nonebot.dependencies import Dependent
 from nonebot.rule import Rule, ArgumentParser
 from nonebot.typing import T_State, T_Handler, T_RuleChecker, T_PermissionChecker
 
+from .plugin import Plugin
+
+def store_matcher(matcher: Type[Matcher]) -> None: ...
+def get_matcher_plugin(depth: int = ...) -> Optional[Plugin]: ...
+def get_matcher_module(depth: int = ...) -> Optional[ModuleType]: ...
 def on(
     type: str = "",
     rule: Optional[Union[Rule, T_RuleChecker]] = ...,
     permission: Optional[Union[Permission, T_PermissionChecker]] = ...,
     *,
     handlers: Optional[List[Union[T_Handler, Dependent]]] = ...,
     temp: bool = ...,
     expire_time: Optional[Union[datetime, timedelta]] = ...,
     priority: int = ...,
     block: bool = ...,
     state: Optional[T_State] = ...,
 ) -> Type[Matcher]: ...
 def on_metaevent(
     rule: Optional[Union[Rule, T_RuleChecker]] = ...,
+    permission: Optional[Union[Permission, T_PermissionChecker]] = ...,
     *,
     handlers: Optional[List[Union[T_Handler, Dependent]]] = ...,
     temp: bool = ...,
     expire_time: Optional[Union[datetime, timedelta]] = ...,
     priority: int = ...,
     block: bool = ...,
     state: Optional[T_State] = ...,
@@ -40,24 +47,26 @@
     expire_time: Optional[Union[datetime, timedelta]] = ...,
     priority: int = ...,
     block: bool = ...,
     state: Optional[T_State] = ...,
 ) -> Type[Matcher]: ...
 def on_notice(
     rule: Optional[Union[Rule, T_RuleChecker]] = ...,
+    permission: Optional[Union[Permission, T_PermissionChecker]] = ...,
     *,
     handlers: Optional[List[Union[T_Handler, Dependent]]] = ...,
     temp: bool = ...,
     expire_time: Optional[Union[datetime, timedelta]] = ...,
     priority: int = ...,
     block: bool = ...,
     state: Optional[T_State] = ...,
 ) -> Type[Matcher]: ...
 def on_request(
     rule: Optional[Union[Rule, T_RuleChecker]] = ...,
+    permission: Optional[Union[Permission, T_PermissionChecker]] = ...,
     *,
     handlers: Optional[List[Union[T_Handler, Dependent]]] = ...,
     temp: bool = ...,
     expire_time: Optional[Union[datetime, timedelta]] = ...,
     priority: int = ...,
     block: bool = ...,
     state: Optional[T_State] = ...,
@@ -113,14 +122,15 @@
     block: bool = ...,
     state: Optional[T_State] = ...,
 ) -> Type[Matcher]: ...
 def on_command(
     cmd: Union[str, Tuple[str, ...]],
     rule: Optional[Union[Rule, T_RuleChecker]] = ...,
     aliases: Optional[Set[Union[str, Tuple[str, ...]]]] = ...,
+    force_whitespace: Optional[Union[str, bool]] = ...,
     *,
     permission: Optional[Union[Permission, T_PermissionChecker]] = ...,
     handlers: Optional[List[Union[T_Handler, Dependent]]] = ...,
     temp: bool = ...,
     expire_time: Optional[Union[datetime, timedelta]] = ...,
     priority: int = ...,
     block: bool = ...,
@@ -182,14 +192,15 @@
     ): ...
     def command(
         self,
         cmd: Union[str, Tuple[str, ...]],
         *,
         rule: Optional[Union[Rule, T_RuleChecker]] = ...,
         aliases: Optional[Set[Union[str, Tuple[str, ...]]]] = ...,
+        force_whitespace: Optional[Union[str, bool]] = ...,
         permission: Optional[Union[Permission, T_PermissionChecker]] = ...,
         handlers: Optional[List[Union[T_Handler, Dependent]]] = ...,
         temp: bool = ...,
         expire_time: Optional[Union[datetime, timedelta]] = ...,
         priority: int = ...,
         block: bool = ...,
         state: Optional[T_State] = ...,
@@ -237,14 +248,15 @@
         block: bool = ...,
         state: Optional[T_State] = ...,
     ) -> Type[Matcher]: ...
     def on_metaevent(
         self,
         *,
         rule: Optional[Union[Rule, T_RuleChecker]] = ...,
+        permission: Optional[Union[Permission, T_PermissionChecker]] = ...,
         handlers: Optional[List[Union[T_Handler, Dependent]]] = ...,
         temp: bool = ...,
         expire_time: Optional[Union[datetime, timedelta]] = ...,
         priority: int = ...,
         block: bool = ...,
         state: Optional[T_State] = ...,
     ) -> Type[Matcher]: ...
@@ -260,25 +272,27 @@
         block: bool = ...,
         state: Optional[T_State] = ...,
     ) -> Type[Matcher]: ...
     def on_notice(
         self,
         *,
         rule: Optional[Union[Rule, T_RuleChecker]] = ...,
+        permission: Optional[Union[Permission, T_PermissionChecker]] = ...,
         handlers: Optional[List[Union[T_Handler, Dependent]]] = ...,
         temp: bool = ...,
         expire_time: Optional[Union[datetime, timedelta]] = ...,
         priority: int = ...,
         block: bool = ...,
         state: Optional[T_State] = ...,
     ) -> Type[Matcher]: ...
     def on_request(
         self,
         *,
         rule: Optional[Union[Rule, T_RuleChecker]] = ...,
+        permission: Optional[Union[Permission, T_PermissionChecker]] = ...,
         handlers: Optional[List[Union[T_Handler, Dependent]]] = ...,
         temp: bool = ...,
         expire_time: Optional[Union[datetime, timedelta]] = ...,
         priority: int = ...,
         block: bool = ...,
         state: Optional[T_State] = ...,
     ) -> Type[Matcher]: ...
@@ -337,14 +351,15 @@
         block: bool = ...,
         state: Optional[T_State] = ...,
     ) -> Type[Matcher]: ...
     def on_command(
         self,
         cmd: Union[str, Tuple[str, ...]],
         aliases: Optional[Set[Union[str, Tuple[str, ...]]]] = ...,
+        force_whitespace: Optional[Union[str, bool]] = ...,
         *,
         rule: Optional[Union[Rule, T_RuleChecker]] = ...,
         permission: Optional[Union[Permission, T_PermissionChecker]] = ...,
         handlers: Optional[List[Union[T_Handler, Dependent]]] = ...,
         temp: bool = ...,
         expire_time: Optional[Union[datetime, timedelta]] = ...,
         priority: int = ...,
```

### Comparing `nonebot2-2.0.0rc3/nonebot/plugin/plugin.py` & `nonebot2-2.0.0rc4/nonebot/plugin/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,13 +43,13 @@
     module: ModuleType
     """插件模块对象"""
     module_name: str
     """点分割模块路径"""
     manager: "PluginManager"
     """导入该插件的插件管理器"""
     matcher: Set[Type[Matcher]] = field(default_factory=set)
-    """插件内定义的 `Matcher`"""
+    """插件加载时定义的 `Matcher`"""
     parent_plugin: Optional["Plugin"] = None
     """父插件"""
     sub_plugins: Set["Plugin"] = field(default_factory=set)
     """子插件集合"""
     metadata: Optional[PluginMetadata] = None
```

### Comparing `nonebot2-2.0.0rc3/nonebot/plugins/single_session.py` & `nonebot2-2.0.0rc4/nonebot/plugins/single_session.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.0.0rc3/nonebot/rule.py` & `nonebot2-2.0.0rc4/nonebot/rule.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,16 +35,16 @@
 from pygtrie import CharTrie
 
 from nonebot import get_driver
 from nonebot.log import logger
 from nonebot.typing import T_State
 from nonebot.exception import ParserExit
 from nonebot.internal.rule import Rule as Rule
-from nonebot.params import Command, EventToMe, CommandArg
 from nonebot.adapters import Bot, Event, Message, MessageSegment
+from nonebot.params import Command, EventToMe, CommandArg, CommandWhitespace
 from nonebot.consts import (
     CMD_KEY,
     REGEX_STR,
     PREFIX_KEY,
     REGEX_DICT,
     SHELL_ARGS,
     SHELL_ARGV,
@@ -53,25 +53,27 @@
     RAW_CMD_KEY,
     REGEX_GROUP,
     ENDSWITH_KEY,
     CMD_START_KEY,
     FULLMATCH_KEY,
     REGEX_MATCHED,
     STARTSWITH_KEY,
+    CMD_WHITESPACE_KEY,
 )
 
 T = TypeVar("T")
 
 CMD_RESULT = TypedDict(
     "CMD_RESULT",
     {
         "command": Optional[Tuple[str, ...]],
         "raw_command": Optional[str],
         "command_arg": Optional[Message[MessageSegment]],
         "command_start": Optional[str],
+        "command_whitespace": Optional[str],
     },
 )
 
 TRIE_VALUE = NamedTuple(
     "TRIE_VALUE", [("command_start", str), ("command", Tuple[str, ...])]
 )
 
@@ -87,34 +89,52 @@
             logger.warning(f'Duplicated prefix rule "{prefix}"')
             return
         cls.prefix[prefix] = value
 
     @classmethod
     def get_value(cls, bot: Bot, event: Event, state: T_State) -> CMD_RESULT:
         prefix = CMD_RESULT(
-            command=None, raw_command=None, command_arg=None, command_start=None
+            command=None,
+            raw_command=None,
+            command_arg=None,
+            command_start=None,
+            command_whitespace=None,
         )
         state[PREFIX_KEY] = prefix
         if event.get_type() != "message":
             return prefix
 
         message = event.get_message()
         message_seg: MessageSegment = message[0]
         if message_seg.is_text():
             segment_text = str(message_seg).lstrip()
             if pf := cls.prefix.longest_prefix(segment_text):
                 value: TRIE_VALUE = pf.value
                 prefix[RAW_CMD_KEY] = pf.key
                 prefix[CMD_START_KEY] = value.command_start
                 prefix[CMD_KEY] = value.command
+
                 msg = message.copy()
                 msg.pop(0)
-                new_message = msg.__class__(segment_text[len(pf.key) :].lstrip())
-                for new_segment in reversed(new_message):
-                    msg.insert(0, new_segment)
+
+                # check whitespace
+                arg_str = segment_text[len(pf.key) :]
+                arg_str_stripped = arg_str.lstrip()
+                has_arg = arg_str_stripped or msg
+                if (
+                    has_arg
+                    and (stripped_len := len(arg_str) - len(arg_str_stripped)) > 0
+                ):
+                    prefix[CMD_WHITESPACE_KEY] = arg_str[:stripped_len]
+
+                # construct command arg
+                if arg_str_stripped:
+                    new_message = msg.__class__(arg_str_stripped)
+                    for new_segment in reversed(new_message):
+                        msg.insert(0, new_segment)
                 prefix[CMD_ARG_KEY] = msg
 
         return prefix
 
 
 class StartswithRule:
     """检查消息纯文本是否以指定字符串开头。
@@ -140,16 +160,14 @@
             and self.ignorecase == other.ignorecase
         )
 
     def __hash__(self) -> int:
         return hash((frozenset(self.msg), self.ignorecase))
 
     async def __call__(self, event: Event, state: T_State) -> bool:
-        if event.get_type() != "message":
-            return False
         try:
             text = event.get_plaintext()
         except Exception:
             return False
         if match := re.match(
             f"^(?:{'|'.join(re.escape(prefix) for prefix in self.msg)})",
             text,
@@ -197,16 +215,14 @@
             and self.ignorecase == other.ignorecase
         )
 
     def __hash__(self) -> int:
         return hash((frozenset(self.msg), self.ignorecase))
 
     async def __call__(self, event: Event, state: T_State) -> bool:
-        if event.get_type() != "message":
-            return False
         try:
             text = event.get_plaintext()
         except Exception:
             return False
         if match := re.search(
             f"(?:{'|'.join(re.escape(suffix) for suffix in self.msg)})$",
             text,
@@ -254,16 +270,14 @@
             and self.ignorecase == other.ignorecase
         )
 
     def __hash__(self) -> int:
         return hash((frozenset(self.msg), self.ignorecase))
 
     async def __call__(self, event: Event, state: T_State) -> bool:
-        if event.get_type() != "message":
-            return False
         try:
             text = event.get_plaintext()
         except Exception:
             return False
         if not text:
             return False
         text = text.casefold() if self.ignorecase else text
@@ -306,16 +320,14 @@
             self.keywords
         ) == frozenset(other.keywords)
 
     def __hash__(self) -> int:
         return hash(frozenset(self.keywords))
 
     async def __call__(self, event: Event, state: T_State) -> bool:
-        if event.get_type() != "message":
-            return False
         try:
             text = event.get_plaintext()
         except Exception:
             return False
         if not text:
             return False
         if key := next((k for k in self.keywords if k in text), None):
@@ -335,48 +347,68 @@
 
 
 class CommandRule:
     """检查消息是否为指定命令。
 
     参数:
         cmds: 指定命令元组列表
+        force_whitespace: 是否强制命令后必须有指定空白符
     """
 
-    __slots__ = ("cmds",)
+    __slots__ = ("cmds", "force_whitespace")
 
-    def __init__(self, cmds: List[Tuple[str, ...]]):
+    def __init__(
+        self,
+        cmds: List[Tuple[str, ...]],
+        force_whitespace: Optional[Union[str, bool]] = None,
+    ):
         self.cmds = tuple(cmds)
+        self.force_whitespace = force_whitespace
 
     def __repr__(self) -> str:
         return f"Command(cmds={self.cmds})"
 
     def __eq__(self, other: object) -> bool:
         return isinstance(other, CommandRule) and frozenset(self.cmds) == frozenset(
             other.cmds
         )
 
     def __hash__(self) -> int:
         return hash((frozenset(self.cmds),))
 
-    async def __call__(self, cmd: Optional[Tuple[str, ...]] = Command()) -> bool:
-        return cmd in self.cmds
+    async def __call__(
+        self,
+        cmd: Optional[Tuple[str, ...]] = Command(),
+        cmd_whitespace: Optional[str] = CommandWhitespace(),
+    ) -> bool:
+        if cmd not in self.cmds:
+            return False
+        if self.force_whitespace is None:
+            return True
+        if isinstance(self.force_whitespace, str):
+            return self.force_whitespace == cmd_whitespace
+        return self.force_whitespace == (cmd_whitespace is not None)
 
 
-def command(*cmds: Union[str, Tuple[str, ...]]) -> Rule:
+def command(
+    *cmds: Union[str, Tuple[str, ...]],
+    force_whitespace: Optional[Union[str, bool]] = None,
+) -> Rule:
     """匹配消息命令。
 
     根据配置里提供的 {ref}``command_start` <nonebot.config.Config.command_start>`,
     {ref}``command_sep` <nonebot.config.Config.command_sep>` 判断消息是否为命令。
 
     可以通过 {ref}`nonebot.params.Command` 获取匹配成功的命令（例: `("test",)`），
     通过 {ref}`nonebot.params.RawCommand` 获取匹配成功的原始命令文本（例: `"/test"`），
     通过 {ref}`nonebot.params.CommandArg` 获取匹配成功的命令参数。
 
     参数:
         cmds: 命令文本或命令元组
+        force_whitespace: 是否强制命令后必须有指定空白符
 
     用法:
         使用默认 `command_start`, `command_sep` 配置
 
         命令 `("test",)` 可以匹配: `/test` 开头的消息
         命令 `("test", "sub")` 可以匹配: `/test.sub` 开头的消息
 
@@ -400,15 +432,15 @@
                 TrieRule.add_prefix(f"{start}{command[0]}", TRIE_VALUE(start, command))
         else:
             for start, sep in product(command_start, command_sep):
                 TrieRule.add_prefix(
                     f"{start}{sep.join(command)}", TRIE_VALUE(start, command)
                 )
 
-    return Rule(CommandRule(commands))
+    return Rule(CommandRule(commands, force_whitespace))
 
 
 class ArgumentParser(ArgParser):
     """`shell_like` 命令参数解析器，解析出错时不会退出程序。
 
     用法:
         用法与 `argparse.ArgumentParser` 相同，
@@ -505,15 +537,15 @@
         )
 
         if self.parser:
             t = parser_message.set("")
             try:
                 args = self.parser.parse_args(state[SHELL_ARGV])
                 state[SHELL_ARGS] = args
-            except ArgumentError as e:
+            except ArgumentError as e:  # pragma: py-gte-39
                 state[SHELL_ARGS] = ParserExit(status=2, message=str(e))
             except ParserExit as e:
                 state[SHELL_ARGS] = e
             finally:
                 parser_message.reset(t)
         return True
 
@@ -605,16 +637,14 @@
             and self.flags == other.flags
         )
 
     def __hash__(self) -> int:
         return hash((self.regex, self.flags))
 
     async def __call__(self, event: Event, state: T_State) -> bool:
-        if event.get_type() != "message":
-            return False
         try:
             msg = event.get_message()
         except Exception:
             return False
         if matched := re.search(self.regex, str(msg), self.flags):
             state[REGEX_MATCHED] = matched.group()
             state[REGEX_STR] = matched.group()
```

### Comparing `nonebot2-2.0.0rc3/nonebot/typing.py` & `nonebot2-2.0.0rc4/nonebot/typing.py`

 * *Files identical despite different names*

### Comparing `nonebot2-2.0.0rc3/nonebot/utils.py` & `nonebot2-2.0.0rc4/nonebot/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     description: nonebot.utils 模块
 """
 
 import re
 import json
 import asyncio
 import inspect
+import importlib
 import dataclasses
 from pathlib import Path
 from functools import wraps, partial
 from contextlib import asynccontextmanager
 from typing_extensions import ParamSpec, get_args, get_origin
 from typing import (
     Any,
@@ -163,21 +164,38 @@
     """获取对象的名称"""
     if inspect.isfunction(obj) or inspect.isclass(obj):
         return obj.__name__
     return obj.__class__.__name__
 
 
 def path_to_module_name(path: Path) -> str:
-    rel_path = path.resolve().relative_to(Path(".").resolve())
+    """转换路径为模块名"""
+    rel_path = path.resolve().relative_to(Path.cwd().resolve())
     if rel_path.stem == "__init__":
         return ".".join(rel_path.parts[:-1])
     else:
         return ".".join(rel_path.parts[:-1] + (rel_path.stem,))
 
 
+def resolve_dot_notation(
+    obj_str: str, default_attr: str, default_prefix: Optional[str] = None
+) -> Any:
+    """解析并导入点分表示法的对象"""
+    modulename, _, cls = obj_str.partition(":")
+    if default_prefix is not None and modulename.startswith("~"):
+        modulename = default_prefix + modulename[1:]
+    module = importlib.import_module(modulename)
+    if not cls:
+        return getattr(module, default_attr)
+    instance = module
+    for attr_str in cls.split("."):
+        instance = getattr(instance, attr_str)
+    return instance
+
+
 class DataclassEncoder(json.JSONEncoder):
     """在JSON序列化 {re}`nonebot.adapters._message.Message` (List[Dataclass]) 时使用的 `JSONEncoder`"""
 
     @overrides(json.JSONEncoder)
     def default(self, o):
         if dataclasses.is_dataclass(o):
             return {f.name: getattr(o, f.name) for f in dataclasses.fields(o)}
```

### Comparing `nonebot2-2.0.0rc3/pyproject.toml` & `nonebot2-2.0.0rc4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot2"
-version = "2.0.0rc3"
+version = "2.0.0rc4"
 description = "An asynchronous python bot framework."
 authors = ["yanyongyu <yyy@nonebot.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://v2.nonebot.dev/"
 repository = "https://github.com/nonebot/nonebot2"
 documentation = "https://v2.nonebot.dev/"
@@ -22,52 +22,53 @@
 include = ["nonebot/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 yarl = "^1.7.2"
 loguru = "^0.6.0"
 pygtrie = "^2.4.1"
-tomlkit = ">=0.10.0,<1.0.0"
-typing-extensions = ">=3.10.0,<5.0.0"
+typing-extensions = ">=4.0.0,<5.0.0"
+tomli = { version = "^2.0.1", python = "<3.11" }
 pydantic = { version = "^1.10.0", extras = ["dotenv"] }
 
 websockets = { version = "^10.0", optional = true }
 Quart = { version = ">=0.18.0,<1.0.0", optional = true }
-fastapi = { version = ">=0.87.0,!=0.89.0,<1.0.0", optional = true }
+fastapi = { version = ">=0.93.0,<1.0.0", optional = true }
 aiohttp = { version = "^3.7.4", extras = ["speedups"], optional = true }
 httpx = { version = ">=0.20.0,<1.0.0", extras = ["http2"], optional = true }
 uvicorn = { version = ">=0.20.0,<1.0.0", extras = ["standard"], optional = true }
 
 [tool.poetry.group.dev.dependencies]
 pycln = "^2.1.2"
 isort = "^5.10.1"
-black = "^22.1.0"
+black = "^23.1.0"
 nonemoji = "^0.1.2"
-pre-commit = "^2.16.0"
+pre-commit = "^3.0.0"
 
 [tool.poetry.group.test.dependencies]
+nonebug = "^0.3.0"
 pytest-cov = "^4.0.0"
 pytest-xdist = "^3.0.2"
-pytest-asyncio = "^0.20.0"
-nonebug = { git = "https://github.com/nonebot/nonebug.git" }
+pytest-asyncio = "^0.21.0"
+coverage-conditional-plugin = "^0.8.0"
 
 [tool.poetry.group.docs.dependencies]
-nb-autodoc = { git = "https://github.com/nonebot/nb-autodoc.git" }
+nb-autodoc = "^1.0.0a5"
 
 [tool.poetry.extras]
 httpx = ["httpx"]
 aiohttp = ["aiohttp"]
 websockets = ["websockets"]
 quart = ["quart", "uvicorn"]
 fastapi = ["fastapi", "uvicorn"]
 all = ["fastapi", "quart", "aiohttp", "httpx", "websockets", "uvicorn"]
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
-addopts = "--cov=nonebot --cov-report=term-missing"
+addopts = "--cov=nonebot --cov-append --cov-report=term-missing"
 filterwarnings = [
     "error",
     "ignore::DeprecationWarning",
 ]
 
 [tool.black]
 line-length = 88
```

### Comparing `nonebot2-2.0.0rc3/setup.py` & `nonebot2-2.0.0rc4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,37 +16,36 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['loguru>=0.6.0,<0.7.0',
  'pydantic[dotenv]>=1.10.0,<2.0.0',
  'pygtrie>=2.4.1,<3.0.0',
- 'tomlkit>=0.10.0,<1.0.0',
- 'typing-extensions>=3.10.0,<5.0.0',
+ 'typing-extensions>=4.0.0,<5.0.0',
  'yarl>=1.7.2,<2.0.0']
 
 extras_require = \
-{'aiohttp': ['aiohttp[speedups]>=3.7.4,<4.0.0'],
+{':python_version < "3.11"': ['tomli>=2.0.1,<3.0.0'],
+ 'aiohttp': ['aiohttp[speedups]>=3.7.4,<4.0.0'],
  'all': ['websockets>=10.0,<11.0',
          'Quart>=0.18.0,<1.0.0',
-         'fastapi>=0.87.0,!=0.89.0,<1.0.0',
+         'fastapi>=0.93.0,<1.0.0',
          'aiohttp[speedups]>=3.7.4,<4.0.0',
          'httpx[http2]>=0.20.0,<1.0.0',
          'uvicorn[standard]>=0.20.0,<1.0.0'],
- 'fastapi': ['fastapi>=0.87.0,!=0.89.0,<1.0.0',
-             'uvicorn[standard]>=0.20.0,<1.0.0'],
+ 'fastapi': ['fastapi>=0.93.0,<1.0.0', 'uvicorn[standard]>=0.20.0,<1.0.0'],
  'httpx': ['httpx[http2]>=0.20.0,<1.0.0'],
  'quart': ['Quart>=0.18.0,<1.0.0', 'uvicorn[standard]>=0.20.0,<1.0.0'],
  'websockets': ['websockets>=10.0,<11.0']}
 
 setup_kwargs = {
     'name': 'nonebot2',
-    'version': '2.0.0rc3',
+    'version': '2.0.0rc4',
     'description': 'An asynchronous python bot framework.',
-    'long_description': '<!-- markdownlint-disable MD033 MD041 -->\n<p align="center">\n  <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>\n</p>\n\n<div align="center">\n\n# NoneBot\n\n<!-- prettier-ignore-start -->\n<!-- markdownlint-disable-next-line MD036 -->\n_✨ 跨平台 Python 异步机器人框架 ✨_\n<!-- prettier-ignore-end -->\n\n</div>\n\n<p align="center">\n  <a href="https://raw.githubusercontent.com/nonebot/nonebot2/master/LICENSE">\n    <img src="https://img.shields.io/github/license/nonebot/nonebot2" alt="license">\n  </a>\n  <a href="https://pypi.python.org/pypi/nonebot2">\n    <img src="https://img.shields.io/pypi/v/nonebot2" alt="pypi">\n  </a>\n  <img src="https://img.shields.io/badge/python-3.8+-blue" alt="python">\n  <a href="https://codecov.io/gh/nonebot/nonebot2">\n    <img src="https://codecov.io/gh/nonebot/nonebot2/branch/master/graph/badge.svg?token=2P0G0VS7N4" alt="codecov"/>\n  </a>\n  <a href="https://github.com/nonebot/nonebot2/actions/workflows/website-deploy.yml">\n    <img src="https://github.com/nonebot/nonebot2/actions/workflows/website-deploy.yml/badge.svg?branch=master&event=push" alt="site"/>\n  </a>\n  <a href="https://results.pre-commit.ci/latest/github/nonebot/nonebot2/master">\n    <img src="https://results.pre-commit.ci/badge/github/nonebot/nonebot2/master.svg" alt="pre-commit" />\n  </a>\n  <br />\n  <a href="https://onebot.dev/">\n    <img src="https://img.shields.io/badge/OneBot-v11-black?style=social&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAEAAAABABAMAAABYR2ztAAAAIVBMVEUAAAAAAAADAwMHBwceHh4UFBQNDQ0ZGRkoKCgvLy8iIiLWSdWYAAAAAXRSTlMAQObYZgAAAQVJREFUSMftlM0RgjAQhV+0ATYK6i1Xb+iMd0qgBEqgBEuwBOxU2QDKsjvojQPvkJ/ZL5sXkgWrFirK4MibYUdE3OR2nEpuKz1/q8CdNxNQgthZCXYVLjyoDQftaKuniHHWRnPh2GCUetR2/9HsMAXyUT4/3UHwtQT2AggSCGKeSAsFnxBIOuAggdh3AKTL7pDuCyABcMb0aQP7aM4AnAbc/wHwA5D2wDHTTe56gIIOUA/4YYV2e1sg713PXdZJAuncdZMAGkAukU9OAn40O849+0ornPwT93rphWF0mgAbauUrEOthlX8Zu7P5A6kZyKCJy75hhw1Mgr9RAUvX7A3csGqZegEdniCx30c3agAAAABJRU5ErkJggg==" alt="onebot">\n  </a>\n  <a href="https://onebot.dev/">\n    <img src="https://img.shields.io/badge/OneBot-v12-black?style=social&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAEAAAABABAMAAABYR2ztAAAAIVBMVEUAAAAAAAADAwMHBwceHh4UFBQNDQ0ZGRkoKCgvLy8iIiLWSdWYAAAAAXRSTlMAQObYZgAAAQVJREFUSMftlM0RgjAQhV+0ATYK6i1Xb+iMd0qgBEqgBEuwBOxU2QDKsjvojQPvkJ/ZL5sXkgWrFirK4MibYUdE3OR2nEpuKz1/q8CdNxNQgthZCXYVLjyoDQftaKuniHHWRnPh2GCUetR2/9HsMAXyUT4/3UHwtQT2AggSCGKeSAsFnxBIOuAggdh3AKTL7pDuCyABcMb0aQP7aM4AnAbc/wHwA5D2wDHTTe56gIIOUA/4YYV2e1sg713PXdZJAuncdZMAGkAukU9OAn40O849+0ornPwT93rphWF0mgAbauUrEOthlX8Zu7P5A6kZyKCJy75hhw1Mgr9RAUvX7A3csGqZegEdniCx30c3agAAAABJRU5ErkJggg==" alt="onebot">\n  </a>\n  <a href="https://core.telegram.org/bots/api">\n    <img src="https://img.shields.io/badge/telegram-Bot-lightgrey?style=social&logo=telegram" alt="telegram">\n  </a>\n  <a href="https://open.feishu.cn/document/home/index">\n    <img src="https://img.shields.io/badge/%E9%A3%9E%E4%B9%A6-Bot-lightgrey?style=social&logo=data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiPz48c3ZnIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDQ4IDQ4IiBmaWxsPSJub25lIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciPjxwYXRoIGQ9Ik0xNyAyOUMyMSAyOSAyNSAyNi45MzM5IDI4IDIzLjQwNjVDMzYgMTQgNDEuNDI0MiAxNi44MTY2IDQ0IDE3Ljk5OThDMzguNSAyMC45OTk4IDQwLjUgMjkuNjIzMyAzMyAzNS45OTk4QzI4LjM4MiAzOS45MjU5IDIzLjQ5NDUgNDEuMDE0IDE5IDQxQzEyLjUyMzEgNDAuOTc5OSA2Ljg2MjI2IDM3Ljc2MzcgNCAzNS40MDYzVjE2Ljk5OTgiIHN0cm9rZT0iIzMzMyIgc3Ryb2tlLXdpZHRoPSI0IiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiLz48cGF0aCBkPSJNNS42NDgwOCAxNS44NjY5QzUuMDIyMzEgMTQuOTU2NyAzLjc3NzE1IDE0LjcyNjEgMi44NjY5NCAxNS4zNTE5QzEuOTU2NzMgMTUuOTc3NyAxLjcyNjE1IDE3LjIyMjggMi4zNTE5MiAxOC4xMzMxTDUuNjQ4MDggMTUuODY2OVpNMzYuMDAyMSAzNS43MzA5QzM2Ljk1OCAzNS4xNzc0IDM3LjI4NDMgMzMuOTUzOSAzNi43MzA5IDMyLjk5NzlDMzYuMTc3NCAzMi4wNDIgMzQuOTUzOSAzMS43MTU3IDMzLjk5NzkgMzIuMjY5MUwzNi4wMDIxIDM1LjczMDlaTTIuMzUxOTIgMTguMTMzMUM1LjI0MzUgMjIuMzM5IDEwLjc5OTIgMjguMTQ0IDE2Ljg4NjUgMzIuMjIzOUMxOS45MzQ1IDM0LjI2NjcgMjMuMjE3IDM1Ljk0NiAyNi40NDkgMzYuNzMyNEMyOS42OTQ2IDM3LjUyMiAzMy4wNDUxIDM3LjQ0MjggMzYuMDAyMSAzNS43MzA5TDMzLjk5NzkgMzIuMjY5MUMzMi4yMDQ5IDMzLjMwNzIgMjkuOTkyOSAzMy40NzggMjcuMzk0NyAzMi44NDU4QzI0Ljc4MyAzMi4yMTAzIDIxLjk0MDUgMzAuNzk1OCAxOS4xMTM1IDI4LjkwMTFDMTMuNDUwOCAyNS4xMDYgOC4yNTY1IDE5LjY2MSA1LjY0ODA4IDE1Ljg2NjlMMi4zNTE5MiAxOC4xMzMxWiIgZmlsbD0iIzMzMyIvPjxwYXRoIGQ9Ik0zMy41OTQ1IDE3QzMyLjgzOTggMTQuNzAyNyAzMC44NTQ5IDkuOTQwNTQgMjcuNTk0NSA3SDExLjU5NDVDMTUuMjE3MSAxMC42NzU3IDIzIDE2IDI3IDI0IiBzdHJva2U9IiMzMzMiIHN0cm9rZS13aWR0aD0iNCIgc3Ryb2tlLWxpbmVjYXA9InJvdW5kIiBzdHJva2UtbGluZWpvaW49InJvdW5kIi8+PC9zdmc+" alt="feishu">\n  </a>\n  <a href="https://docs.github.com/en/developers/apps">\n    <img src="https://img.shields.io/badge/GitHub-Bot-181717?style=social&logo=github" alt="github"/>\n  </a>\n  <a href="https://bot.q.qq.com/wiki/">\n    <img src="https://img.shields.io/badge/QQ%E9%A2%91%E9%81%93-Bot-lightgrey?style=social&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAxMTIuODIgMTMwLjg5Ij48ZyBkYXRhLW5hbWU9IuWbvuWxgiAyIj48ZyBkYXRhLW5hbWU9IuWbvuWxgiAxIj48cGF0aCBkPSJNNTUuNjMgMTMwLjhjLTcgMC0xMy45LjA4LTIwLjg2IDAtMTkuMTUtLjI1LTMxLjcxLTExLjQtMzQuMjItMzAuMy00LjA3LTMwLjY2IDE0LjkzLTU5LjIgNDQuODMtNjYuNjQgMi0uNTEgNS4yMS0uMzEgNS4yMS0xLjYzIDAtMi4xMy4xNC0yLjEzLjE0LTUuNTcgMC0uODktMS4zLTEuNDYtMi4yMi0yLjMxLTYuNzMtNi4yMy03LjY3LTEzLjQxLTEtMjAuMTggNS40LTUuNTIgMTEuODctNS40IDE3LjgtLjU5IDYuNDkgNS4yNiA2LjMxIDEzLjA4LS44NiAyMS0uNjguNzQtMS43OCAxLjYtMS43OCAyLjY3djQuMjFjMCAxLjM1IDIuMiAxLjYyIDQuNzkgMi4zNSAzMS4wOSA4LjY1IDQ4LjE3IDM0LjEzIDQ1IDY2LjM3LTEuNzYgMTguMTUtMTQuNTYgMzAuMjMtMzIuNyAzMC42My04LjAyLjE5LTE2LjA3LS4wMS0yNC4xMy0uMDF6IiBmaWxsPSIjMDI5OWZlIi8+PHBhdGggZD0iTTMxLjQ2IDExOC4zOGMtMTAuNS0uNjktMTYuOC02Ljg2LTE4LjM4LTE3LjI3LTMtMTkuNDIgMi43OC0zNS44NiAxOC40Ni00Ny44MyAxNC4xNi0xMC44IDI5Ljg3LTEyIDQ1LjM4LTMuMTkgMTcuMjUgOS44NCAyNC41OSAyNS44MSAyNCA0NS4yOS0uNDkgMTUuOS04LjQyIDIzLjE0LTI0LjM4IDIzLjUtNi41OS4xNC0xMy4xOSAwLTE5Ljc5IDAiIGZpbGw9IiNmZWZlZmUiLz48cGF0aCBkPSJNNDYuMDUgNzkuNThjLjA5IDUgLjIzIDkuODItNyA5Ljc3LTcuODItLjA2LTYuMS01LjY5LTYuMjQtMTAuMTktLjE1LTQuODItLjczLTEwIDYuNzMtOS44NHM2LjM3IDUuNTUgNi41MSAxMC4yNnoiIGZpbGw9IiMxMDlmZmUiLz48cGF0aCBkPSJNODAuMjcgNzkuMjdjLS41MyAzLjkxIDEuNzUgOS42NC01Ljg4IDEwLTcuNDcuMzctNi44MS00LjgyLTYuNjEtOS41LjItNC4zMi0xLjgzLTEwIDUuNzgtMTAuNDJzNi41OSA0Ljg5IDYuNzEgOS45MnoiIGZpbGw9IiMwODljZmUiLz48L2c+PC9nPjwvc3ZnPg==" alt="QQ频道">\n  <a href="https://ding-doc.dingtalk.com/document#/org-dev-guide/elzz1p">\n    <img src="https://img.shields.io/badge/%E9%92%89%E9%92%89-Bot-lightgrey?style=social&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAEAAAABACAMAAACdt4HsAAAAnFBMVEUAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAD4jUzeAAAAM3RSTlMAQKSRaA+/f0YyFevh29R3cyklIfrlyrGsn41tVUs48c/HqJm9uZdhX1otGwkF9IN8V1CX0Q+IAAABY0lEQVRYw+3V2W7CMBAF0JuNQAhhX9OEfYdu9///rUVWpagE27Ef2gfO+0zGozsKnv6bMGzAhkNytIe5gDdzrwtTCwrbI8x4/NF668NAxgI3Q3UtFi3TyPwNQtPLUUmDd8YfqGLNe4v22XwEYb5zoOuF5baHq2UHtsKe5ivWfGAwrWu2mC34QM0PoCAuqZdOmiwV+5BLyMRtZ7dTSEcs48rzWfzwptMLyzpApka1SJ5FtR4kfCqNIBPEVDmqoqgwUYY5plQOlf6UEjNoOPnuKB6wzDyCrks///TDza8+PnR109WQdxLo8RKWq0PPnuXG0OXKQ6wWLFnCg75uYYbhmMIVVdQ709q33aHbGIj6Duz+2k1HQFX9VwqmY8xYsEJll2ahvhWgsjYLHFRXvIi2Qb0jzMQCzC3FAoydxCma88UCzE3JCWwkjCNYyMUCzHX4DiuTMawEwwhW6hnshPhjZzzJfAH0YacpbmRd7QAAAABJRU5ErkJggg==" alt="dingtalk">\n  </a>\n  </a>\n  <br />\n  <a href="https://jq.qq.com/?_wv=1027&k=5OFifDh">\n    <img src="https://img.shields.io/badge/QQ%E7%BE%A4-768887710-orange?style=flat-square" alt="QQ Chat Group">\n  </a>\n  <a href="https://qun.qq.com/qqweb/qunpro/share?_wv=3&_wwv=128&appChannel=share&inviteCode=7b4a3&appChannel=share&businessType=9&from=246610&biz=ka">\n    <img src="https://img.shields.io/badge/QQ%E9%A2%91%E9%81%93-NoneBot-5492ff?style=flat-square" alt="QQ Channel">\n  </a>\n  <a href="https://t.me/botuniverse">\n    <img src="https://img.shields.io/badge/telegram-botuniverse-blue?style=flat-square" alt="Telegram Channel">\n  </a>\n  <a href="https://discord.gg/VKtE6Gdc4h">\n    <img src="https://discordapp.com/api/guilds/847819937858584596/widget.png?style=shield" alt="Discord Server">\n  </a>\n</p>\n\n<p align="center">\n  <a href="https://v2.nonebot.dev/">文档</a>\n  ·\n  <a href="https://v2.nonebot.dev/docs/start/installation">安装</a>\n  ·\n  <a href="https://v2.nonebot.dev/docs/tutorial/create-project">开始使用</a>\n  ·\n  <a href="#插件">文档打不开？</a>\n</p>\n\n<p align="center">\n  <a href="https://asciinema.org/a/464654">\n    <img src="https://v2.nonebot.dev/img/setup.svg">\n  </a>\n</p>\n\n## 简介\n\nNoneBot2 是一个现代、跨平台、可扩展的 Python 聊天机器人框架，它基于 Python 的类型注解和异步特性，能够为你的需求实现提供便捷灵活的支持。\n\n## 特色\n\n- 异步优先：基于 Python 的异步特性，即使是~~非常~~大量的消息，也能吞吐自如\n- 易于开发：配合 NB-CLI 脚手架，代码编写上手简单，没有过多的冗余代码，可以让开发者专注于业务逻辑\n- 生而可靠：100% 类型注解覆盖，配合编辑器的类型推导功能，能将绝大多数的 Bug 杜绝在编辑器中 ([编辑器支持](https://v2.nonebot.dev/docs/start/editor-support))\n- 社区丰富：社区用户众多，直接和间接用户超过十万人，每天都有大量的活跃用户 ([社区资源](#社区资源))\n- 海纳百川：一个框架，支持多个聊天软件平台，可自定义通信协议\n\n  |                                 协议名称                                  | 状态 |                                注释                                |\n  | :-----------------------------------------------------------------------: | :--: | :----------------------------------------------------------------: |\n  |                    [OneBot 协议](https://onebot.dev/)                     |  ✅  | 支持 QQ、TG、微信公众号等[平台](https://onebot.dev/ecosystem.html) |\n  |              [Telegram](https://core.telegram.org/bots/api)               |  ✅  |                                                                    |\n  |            [飞书](https://open.feishu.cn/document/home/index)             |  ✅  |                                                                    |\n  |           [GitHub](https://docs.github.com/en/developers/apps)            |  ✅  |                       GitHub APP & OAuth APP                       |\n  |                   [QQ 频道](https://bot.q.qq.com/wiki/)                   |  ✅  |                          官方接口调整较多                          |\n  |                [钉钉](https://open.dingtalk.com/document/)                |  🤗  |                          寻找 Maintainer                           |\n  |                                  Console                                  |  ✅  |                             控制台交互                             |\n  |                  [开黑啦](https://developer.kookapp.cn/)                  |  ↗️  |                             由社区贡献                             |\n  |           [Mirai](https://docs.mirai.mamoe.net/mirai-api-http/)           |  ↗️  |                             由社区贡献                             |\n  |        [Ntchat](https://github.com/JustUndertaker/adapter-ntchat)         |  ↗️  |                             由社区贡献                             |\n  | [MineCraft (Spigot)](https://github.com/17TheWord/nonebot-adapter-spigot) |  ↗️  |                             由社区贡献                             |\n  |        [BiliBili Live](https://github.com/wwweww/adapter-bilibili)        |  ↗️  |                             由社区贡献                             |\n\n- 坚实后盾：支持多种 web 框架，可自定义替换、组合\n\n  |                          驱动框架                          |  类型  |\n  | :--------------------------------------------------------: | :----: |\n  |          [FastAPI](https://fastapi.tiangolo.com/)          | 服务端 |\n  |   [Quart](https://pgjones.gitlab.io/quart/) (异步 Flask)   | 服务端 |\n  |       [aiohttp](https://docs.aiohttp.org/en/stable/)       | 客户端 |\n  |           [httpx](https://www.python-httpx.org/)           | 客户端 |\n  | [websockets](https://websockets.readthedocs.io/en/stable/) | 客户端 |\n\n更多：[概览](https://v2.nonebot.dev/docs/)\n\n## 什么不是 NoneBot2\n\nNoneBot2 不是某个平台或者协议的具体实现，它只负责和已有协议适配器通信，并处理接收到的事件。所以，“NoneBot 有 blabla 平台的 blabla 功能吗？”这种问题是与 NoneBot2 无关的。请在相应平台的功能文档中确认，或与相应平台的协议适配开发者联系。\n\nNoneBot2 不是 NoneBot1 的替代品。事实上，它们都在被积极的维护着。但是，如果你想尝试一些新功能，或者想要支持更多的平台，可以考虑使用 NoneBot2。\n\n> ~~NoneBot2 和 NoneBot1 的区别，就像是 VisualStudio Code 和 VisualStudio 一样~~\n\n## 即刻开始\n\n~~完整~~文档可以在 [这里](https://v2.nonebot.dev/) 查看。\n\n懒得看文档？下面是快速安装指南：\n\n1. 安装 [pipx](https://pypa.github.io/pipx/)\n\n   ```bash\n   python -m pip install --user pipx\n   python -m pipx ensurepath\n   ```\n\n2. 安装脚手架\n\n   ```bash\n   pipx install nb-cli\n   ```\n\n3. 使用脚手架创建项目\n\n   ```bash\n   nb create\n   ```\n\n4. 运行项目\n\n   ```bash\n   nb run\n   ```\n\n## 社区资源\n\n### 常见问题\n\n- [常见问题解答(FAQ)](https://faq.nonebot.dev/)\n- [论坛(Discussion)](https://discussions.nonebot.dev/)\n\n### 教程/实际项目/经验分享\n\n- [awesome-nonebot](https://github.com/nonebot/awesome-nonebot)\n\n### 插件\n\n此外，NoneBot2 还有丰富的官方以及第三方现成的插件供大家使用：\n\n- [NoneBot-Plugin-Docs](https://github.com/nonebot/nonebot2/tree/master/packages/nonebot-plugin-docs)：离线文档至本地项目使用 (别再说文档打不开了！)\n\n  在项目目录下执行：\n\n  ```bash\n  nb plugin install nonebot_plugin_docs\n  ```\n\n  或者尝试以下镜像：\n\n  - [文档镜像(中国境内)](https://nb2.baka.icu)\n  - [文档镜像(Vercel)](https://nonebot2-vercel-mirror.vercel.app)\n\n- 其他插件请查看 [商店](https://v2.nonebot.dev/store)\n\n## 许可证\n\n`NoneBot` 采用 `MIT` 许可证进行开源\n\n```text\nTHE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS\nFOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR\nCOPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER\nIN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN\nCONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n```\n\n## 贡献\n\n请参考 [贡献指南](./CONTRIBUTING.md)\n\n### 鸣谢\n\n感谢以下开发者对 NoneBot2 作出的贡献：\n\n<a href="https://github.com/nonebot/nonebot2/graphs/contributors">\n  <img src="https://contrib.rocks/image?repo=nonebot/nonebot2&max=1000" />\n</a>\n',
+    'long_description': '<!-- markdownlint-disable MD033 MD041 -->\n<p align="center">\n  <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>\n</p>\n\n<div align="center">\n\n# NoneBot\n\n<!-- prettier-ignore-start -->\n<!-- markdownlint-disable-next-line MD036 -->\n_✨ 跨平台 Python 异步机器人框架 ✨_\n<!-- prettier-ignore-end -->\n\n</div>\n\n<p align="center">\n  <a href="https://raw.githubusercontent.com/nonebot/nonebot2/master/LICENSE">\n    <img src="https://img.shields.io/github/license/nonebot/nonebot2" alt="license">\n  </a>\n  <a href="https://pypi.python.org/pypi/nonebot2">\n    <img src="https://img.shields.io/pypi/v/nonebot2" alt="pypi">\n  </a>\n  <img src="https://img.shields.io/badge/python-3.8+-blue" alt="python">\n  <a href="https://codecov.io/gh/nonebot/nonebot2">\n    <img src="https://codecov.io/gh/nonebot/nonebot2/branch/master/graph/badge.svg?token=2P0G0VS7N4" alt="codecov"/>\n  </a>\n  <a href="https://github.com/nonebot/nonebot2/actions/workflows/website-deploy.yml">\n    <img src="https://github.com/nonebot/nonebot2/actions/workflows/website-deploy.yml/badge.svg?branch=master&event=push" alt="site"/>\n  </a>\n  <a href="https://results.pre-commit.ci/latest/github/nonebot/nonebot2/master">\n    <img src="https://results.pre-commit.ci/badge/github/nonebot/nonebot2/master.svg" alt="pre-commit" />\n  </a>\n  <br />\n  <a href="https://onebot.dev/">\n    <img src="https://img.shields.io/badge/OneBot-v11-black?style=social&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAEAAAABABAMAAABYR2ztAAAAIVBMVEUAAAAAAAADAwMHBwceHh4UFBQNDQ0ZGRkoKCgvLy8iIiLWSdWYAAAAAXRSTlMAQObYZgAAAQVJREFUSMftlM0RgjAQhV+0ATYK6i1Xb+iMd0qgBEqgBEuwBOxU2QDKsjvojQPvkJ/ZL5sXkgWrFirK4MibYUdE3OR2nEpuKz1/q8CdNxNQgthZCXYVLjyoDQftaKuniHHWRnPh2GCUetR2/9HsMAXyUT4/3UHwtQT2AggSCGKeSAsFnxBIOuAggdh3AKTL7pDuCyABcMb0aQP7aM4AnAbc/wHwA5D2wDHTTe56gIIOUA/4YYV2e1sg713PXdZJAuncdZMAGkAukU9OAn40O849+0ornPwT93rphWF0mgAbauUrEOthlX8Zu7P5A6kZyKCJy75hhw1Mgr9RAUvX7A3csGqZegEdniCx30c3agAAAABJRU5ErkJggg==" alt="onebot">\n  </a>\n  <a href="https://onebot.dev/">\n    <img src="https://img.shields.io/badge/OneBot-v12-black?style=social&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAEAAAABABAMAAABYR2ztAAAAIVBMVEUAAAAAAAADAwMHBwceHh4UFBQNDQ0ZGRkoKCgvLy8iIiLWSdWYAAAAAXRSTlMAQObYZgAAAQVJREFUSMftlM0RgjAQhV+0ATYK6i1Xb+iMd0qgBEqgBEuwBOxU2QDKsjvojQPvkJ/ZL5sXkgWrFirK4MibYUdE3OR2nEpuKz1/q8CdNxNQgthZCXYVLjyoDQftaKuniHHWRnPh2GCUetR2/9HsMAXyUT4/3UHwtQT2AggSCGKeSAsFnxBIOuAggdh3AKTL7pDuCyABcMb0aQP7aM4AnAbc/wHwA5D2wDHTTe56gIIOUA/4YYV2e1sg713PXdZJAuncdZMAGkAukU9OAn40O849+0ornPwT93rphWF0mgAbauUrEOthlX8Zu7P5A6kZyKCJy75hhw1Mgr9RAUvX7A3csGqZegEdniCx30c3agAAAABJRU5ErkJggg==" alt="onebot">\n  </a>\n  <a href="https://core.telegram.org/bots/api">\n    <img src="https://img.shields.io/badge/telegram-Bot-lightgrey?style=social&logo=telegram" alt="telegram">\n  </a>\n  <a href="https://open.feishu.cn/document/home/index">\n    <img src="https://img.shields.io/badge/%E9%A3%9E%E4%B9%A6-Bot-lightgrey?style=social&logo=data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiPz48c3ZnIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDQ4IDQ4IiBmaWxsPSJub25lIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciPjxwYXRoIGQ9Ik0xNyAyOUMyMSAyOSAyNSAyNi45MzM5IDI4IDIzLjQwNjVDMzYgMTQgNDEuNDI0MiAxNi44MTY2IDQ0IDE3Ljk5OThDMzguNSAyMC45OTk4IDQwLjUgMjkuNjIzMyAzMyAzNS45OTk4QzI4LjM4MiAzOS45MjU5IDIzLjQ5NDUgNDEuMDE0IDE5IDQxQzEyLjUyMzEgNDAuOTc5OSA2Ljg2MjI2IDM3Ljc2MzcgNCAzNS40MDYzVjE2Ljk5OTgiIHN0cm9rZT0iIzMzMyIgc3Ryb2tlLXdpZHRoPSI0IiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiLz48cGF0aCBkPSJNNS42NDgwOCAxNS44NjY5QzUuMDIyMzEgMTQuOTU2NyAzLjc3NzE1IDE0LjcyNjEgMi44NjY5NCAxNS4zNTE5QzEuOTU2NzMgMTUuOTc3NyAxLjcyNjE1IDE3LjIyMjggMi4zNTE5MiAxOC4xMzMxTDUuNjQ4MDggMTUuODY2OVpNMzYuMDAyMSAzNS43MzA5QzM2Ljk1OCAzNS4xNzc0IDM3LjI4NDMgMzMuOTUzOSAzNi43MzA5IDMyLjk5NzlDMzYuMTc3NCAzMi4wNDIgMzQuOTUzOSAzMS43MTU3IDMzLjk5NzkgMzIuMjY5MUwzNi4wMDIxIDM1LjczMDlaTTIuMzUxOTIgMTguMTMzMUM1LjI0MzUgMjIuMzM5IDEwLjc5OTIgMjguMTQ0IDE2Ljg4NjUgMzIuMjIzOUMxOS45MzQ1IDM0LjI2NjcgMjMuMjE3IDM1Ljk0NiAyNi40NDkgMzYuNzMyNEMyOS42OTQ2IDM3LjUyMiAzMy4wNDUxIDM3LjQ0MjggMzYuMDAyMSAzNS43MzA5TDMzLjk5NzkgMzIuMjY5MUMzMi4yMDQ5IDMzLjMwNzIgMjkuOTkyOSAzMy40NzggMjcuMzk0NyAzMi44NDU4QzI0Ljc4MyAzMi4yMTAzIDIxLjk0MDUgMzAuNzk1OCAxOS4xMTM1IDI4LjkwMTFDMTMuNDUwOCAyNS4xMDYgOC4yNTY1IDE5LjY2MSA1LjY0ODA4IDE1Ljg2NjlMMi4zNTE5MiAxOC4xMzMxWiIgZmlsbD0iIzMzMyIvPjxwYXRoIGQ9Ik0zMy41OTQ1IDE3QzMyLjgzOTggMTQuNzAyNyAzMC44NTQ5IDkuOTQwNTQgMjcuNTk0NSA3SDExLjU5NDVDMTUuMjE3MSAxMC42NzU3IDIzIDE2IDI3IDI0IiBzdHJva2U9IiMzMzMiIHN0cm9rZS13aWR0aD0iNCIgc3Ryb2tlLWxpbmVjYXA9InJvdW5kIiBzdHJva2UtbGluZWpvaW49InJvdW5kIi8+PC9zdmc+" alt="feishu">\n  </a>\n  <a href="https://docs.github.com/en/developers/apps">\n    <img src="https://img.shields.io/badge/GitHub-Bot-181717?style=social&logo=github" alt="github"/>\n  </a>\n  <a href="https://bot.q.qq.com/wiki/">\n    <img src="https://img.shields.io/badge/QQ%E9%A2%91%E9%81%93-Bot-lightgrey?style=social&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAxMTIuODIgMTMwLjg5Ij48ZyBkYXRhLW5hbWU9IuWbvuWxgiAyIj48ZyBkYXRhLW5hbWU9IuWbvuWxgiAxIj48cGF0aCBkPSJNNTUuNjMgMTMwLjhjLTcgMC0xMy45LjA4LTIwLjg2IDAtMTkuMTUtLjI1LTMxLjcxLTExLjQtMzQuMjItMzAuMy00LjA3LTMwLjY2IDE0LjkzLTU5LjIgNDQuODMtNjYuNjQgMi0uNTEgNS4yMS0uMzEgNS4yMS0xLjYzIDAtMi4xMy4xNC0yLjEzLjE0LTUuNTcgMC0uODktMS4zLTEuNDYtMi4yMi0yLjMxLTYuNzMtNi4yMy03LjY3LTEzLjQxLTEtMjAuMTggNS40LTUuNTIgMTEuODctNS40IDE3LjgtLjU5IDYuNDkgNS4yNiA2LjMxIDEzLjA4LS44NiAyMS0uNjguNzQtMS43OCAxLjYtMS43OCAyLjY3djQuMjFjMCAxLjM1IDIuMiAxLjYyIDQuNzkgMi4zNSAzMS4wOSA4LjY1IDQ4LjE3IDM0LjEzIDQ1IDY2LjM3LTEuNzYgMTguMTUtMTQuNTYgMzAuMjMtMzIuNyAzMC42My04LjAyLjE5LTE2LjA3LS4wMS0yNC4xMy0uMDF6IiBmaWxsPSIjMDI5OWZlIi8+PHBhdGggZD0iTTMxLjQ2IDExOC4zOGMtMTAuNS0uNjktMTYuOC02Ljg2LTE4LjM4LTE3LjI3LTMtMTkuNDIgMi43OC0zNS44NiAxOC40Ni00Ny44MyAxNC4xNi0xMC44IDI5Ljg3LTEyIDQ1LjM4LTMuMTkgMTcuMjUgOS44NCAyNC41OSAyNS44MSAyNCA0NS4yOS0uNDkgMTUuOS04LjQyIDIzLjE0LTI0LjM4IDIzLjUtNi41OS4xNC0xMy4xOSAwLTE5Ljc5IDAiIGZpbGw9IiNmZWZlZmUiLz48cGF0aCBkPSJNNDYuMDUgNzkuNThjLjA5IDUgLjIzIDkuODItNyA5Ljc3LTcuODItLjA2LTYuMS01LjY5LTYuMjQtMTAuMTktLjE1LTQuODItLjczLTEwIDYuNzMtOS44NHM2LjM3IDUuNTUgNi41MSAxMC4yNnoiIGZpbGw9IiMxMDlmZmUiLz48cGF0aCBkPSJNODAuMjcgNzkuMjdjLS41MyAzLjkxIDEuNzUgOS42NC01Ljg4IDEwLTcuNDcuMzctNi44MS00LjgyLTYuNjEtOS41LjItNC4zMi0xLjgzLTEwIDUuNzgtMTAuNDJzNi41OSA0Ljg5IDYuNzEgOS45MnoiIGZpbGw9IiMwODljZmUiLz48L2c+PC9nPjwvc3ZnPg==" alt="QQ频道">\n  <a href="https://ding-doc.dingtalk.com/document#/org-dev-guide/elzz1p">\n    <img src="https://img.shields.io/badge/%E9%92%89%E9%92%89-Bot-lightgrey?style=social&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAEAAAABACAMAAACdt4HsAAAAnFBMVEUAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAD4jUzeAAAAM3RSTlMAQKSRaA+/f0YyFevh29R3cyklIfrlyrGsn41tVUs48c/HqJm9uZdhX1otGwkF9IN8V1CX0Q+IAAABY0lEQVRYw+3V2W7CMBAF0JuNQAhhX9OEfYdu9///rUVWpagE27Ef2gfO+0zGozsKnv6bMGzAhkNytIe5gDdzrwtTCwrbI8x4/NF668NAxgI3Q3UtFi3TyPwNQtPLUUmDd8YfqGLNe4v22XwEYb5zoOuF5baHq2UHtsKe5ivWfGAwrWu2mC34QM0PoCAuqZdOmiwV+5BLyMRtZ7dTSEcs48rzWfzwptMLyzpApka1SJ5FtR4kfCqNIBPEVDmqoqgwUYY5plQOlf6UEjNoOPnuKB6wzDyCrks///TDza8+PnR109WQdxLo8RKWq0PPnuXG0OXKQ6wWLFnCg75uYYbhmMIVVdQ709q33aHbGIj6Duz+2k1HQFX9VwqmY8xYsEJll2ahvhWgsjYLHFRXvIi2Qb0jzMQCzC3FAoydxCma88UCzE3JCWwkjCNYyMUCzHX4DiuTMawEwwhW6hnshPhjZzzJfAH0YacpbmRd7QAAAABJRU5ErkJggg==" alt="dingtalk">\n  </a>\n  </a>\n  <br />\n  <a href="https://jq.qq.com/?_wv=1027&k=5OFifDh">\n    <img src="https://img.shields.io/badge/QQ%E7%BE%A4-768887710-orange?style=flat-square" alt="QQ Chat Group">\n  </a>\n  <a href="https://qun.qq.com/qqweb/qunpro/share?_wv=3&_wwv=128&appChannel=share&inviteCode=7b4a3&appChannel=share&businessType=9&from=246610&biz=ka">\n    <img src="https://img.shields.io/badge/QQ%E9%A2%91%E9%81%93-NoneBot-5492ff?style=flat-square" alt="QQ Channel">\n  </a>\n  <a href="https://t.me/botuniverse">\n    <img src="https://img.shields.io/badge/telegram-botuniverse-blue?style=flat-square" alt="Telegram Channel">\n  </a>\n  <a href="https://discord.gg/VKtE6Gdc4h">\n    <img src="https://discordapp.com/api/guilds/847819937858584596/widget.png?style=shield" alt="Discord Server">\n  </a>\n</p>\n\n<p align="center">\n  <a href="https://v2.nonebot.dev/">文档</a>\n  ·\n  <a href="https://v2.nonebot.dev/docs/quick-start">快速上手</a>\n  ·\n  <a href="#插件">文档打不开？</a>\n</p>\n\n<p align="center">\n  <a href="https://asciinema.org/a/569440">\n    <img src="https://v2.nonebot.dev/img/setup.svg">\n  </a>\n</p>\n\n## 简介\n\nNoneBot2 是一个现代、跨平台、可扩展的 Python 聊天机器人框架，它基于 Python 的类型注解和异步特性，能够为你的需求实现提供便捷灵活的支持。\n\n## 特色\n\n- 异步优先：基于 Python 的异步特性，即使是~~非常~~大量的消息，也能吞吐自如\n- 易于开发：配合 NB-CLI 脚手架，代码编写上手简单，没有过多的冗余代码，可以让开发者专注于业务逻辑\n- 生而可靠：100% 类型注解覆盖，配合编辑器的类型推导功能，能将绝大多数的 Bug 杜绝在编辑器中 ([编辑器支持](https://v2.nonebot.dev/docs/editor-support))\n- 社区丰富：社区用户众多，直接和间接用户超过十万人，每天都有大量的活跃用户 ([社区资源](#社区资源))\n- 海纳百川：一个框架，支持多个聊天软件平台，可自定义通信协议\n\n  |                                 协议名称                                  | 状态 |                                注释                                |\n  | :-----------------------------------------------------------------------: | :--: | :----------------------------------------------------------------: |\n  |                    [OneBot 协议](https://onebot.dev/)                     |  ✅  | 支持 QQ、TG、微信公众号等[平台](https://onebot.dev/ecosystem.html) |\n  |              [Telegram](https://core.telegram.org/bots/api)               |  ✅  |                                                                    |\n  |            [飞书](https://open.feishu.cn/document/home/index)             |  ✅  |                                                                    |\n  |           [GitHub](https://docs.github.com/en/developers/apps)            |  ✅  |                       GitHub APP & OAuth APP                       |\n  |                   [QQ 频道](https://bot.q.qq.com/wiki/)                   |  ✅  |                          官方接口调整较多                          |\n  |                [钉钉](https://open.dingtalk.com/document/)                |  🤗  |                          寻找 Maintainer                           |\n  |                                  Console                                  |  ✅  |                             控制台交互                             |\n  |                  [开黑啦](https://developer.kookapp.cn/)                  |  ↗️  |                             由社区贡献                             |\n  |           [Mirai](https://docs.mirai.mamoe.net/mirai-api-http/)           |  ↗️  |                             由社区贡献                             |\n  |        [Ntchat](https://github.com/JustUndertaker/adapter-ntchat)         |  ↗️  |                             由社区贡献                             |\n  | [MineCraft (Spigot)](https://github.com/17TheWord/nonebot-adapter-spigot) |  ↗️  |                             由社区贡献                             |\n  |        [BiliBili Live](https://github.com/wwweww/adapter-bilibili)        |  ↗️  |                             由社区贡献                             |\n\n- 坚实后盾：支持多种 web 框架，可自定义替换、组合\n\n  |                          驱动框架                          |  类型  |\n  | :--------------------------------------------------------: | :----: |\n  |          [FastAPI](https://fastapi.tiangolo.com/)          | 服务端 |\n  |   [Quart](https://pgjones.gitlab.io/quart/) (异步 Flask)   | 服务端 |\n  |       [aiohttp](https://docs.aiohttp.org/en/stable/)       | 客户端 |\n  |           [httpx](https://www.python-httpx.org/)           | 客户端 |\n  | [websockets](https://websockets.readthedocs.io/en/stable/) | 客户端 |\n\n更多：[概览](https://v2.nonebot.dev/docs/)\n\n## 什么不是 NoneBot2\n\nNoneBot2 不是某个平台或者协议的具体实现，它只负责和已有协议适配器通信，并处理接收到的事件。所以，“NoneBot 有 blabla 平台的 blabla 功能吗？”这种问题是与 NoneBot2 无关的。请在相应平台的功能文档中确认，或与相应平台的协议适配开发者联系。\n\nNoneBot2 不是 NoneBot1 的替代品。事实上，它们都在被积极的维护着。但是，如果你想尝试一些新功能，或者想要支持更多的平台，可以考虑使用 NoneBot2。\n\n> ~~NoneBot2 和 NoneBot1 的区别，就像是 VisualStudio Code 和 VisualStudio 一样~~\n\n## 即刻开始\n\n~~完整~~文档可以在 [这里](https://v2.nonebot.dev/) 查看。\n\n懒得看文档？下面是快速安装指南：\n\n1. 安装 [pipx](https://pypa.github.io/pipx/)\n\n   ```bash\n   python -m pip install --user pipx\n   python -m pipx ensurepath\n   ```\n\n2. 安装脚手架\n\n   ```bash\n   pipx install nb-cli\n   ```\n\n3. 使用脚手架创建项目\n\n   ```bash\n   nb create\n   ```\n\n4. 运行项目\n\n   ```bash\n   nb run\n   ```\n\n## 社区资源\n\n### 常见问题\n\n- [常见问题解答(FAQ)](https://faq.nonebot.dev/)\n- [论坛(Discussion)](https://discussions.nonebot.dev/)\n\n### 教程/实际项目/经验分享\n\n- [awesome-nonebot](https://github.com/nonebot/awesome-nonebot)\n\n### 插件\n\n此外，NoneBot2 还有丰富的官方以及第三方现成的插件供大家使用：\n\n- [NoneBot-Plugin-Docs](https://github.com/nonebot/nonebot2/tree/master/packages/nonebot-plugin-docs)：离线文档至本地项目使用 (别再说文档打不开了！)\n\n  在项目目录下执行：\n\n  ```bash\n  nb plugin install nonebot_plugin_docs\n  ```\n\n  或者尝试以下镜像：\n\n  - [文档镜像(中国境内)](https://nb2.baka.icu)\n  - [文档镜像(Vercel)](https://nonebot2-vercel-mirror.vercel.app)\n\n- 其他插件请查看 [商店](https://v2.nonebot.dev/store)\n\n## 许可证\n\n`NoneBot` 采用 `MIT` 许可证进行开源\n\n```text\nTHE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS\nFOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR\nCOPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER\nIN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN\nCONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n```\n\n## 贡献\n\n请参考 [贡献指南](./CONTRIBUTING.md)\n\n### 鸣谢\n\n感谢以下开发者对 NoneBot2 作出的贡献：\n\n<a href="https://github.com/nonebot/nonebot2/graphs/contributors">\n  <img src="https://contrib.rocks/image?repo=nonebot/nonebot2&max=1000" />\n</a>\n',
     'author': 'yanyongyu',
     'author_email': 'yyy@nonebot.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://v2.nonebot.dev/',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,47 +1,48 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['nonebot',
 'nonebot.adapters', 'nonebot.dependencies', 'nonebot.drivers',
 'nonebot.internal', 'nonebot.internal.adapter', 'nonebot.internal.driver',
 'nonebot.internal.matcher', 'nonebot.plugin', 'nonebot.plugins'] package_data =
 \ {'': ['*']} install_requires = \ ['loguru>=0.6.0,<0.7.0', 'pydantic
-[dotenv]>=1.10.0,<2.0.0', 'pygtrie>=2.4.1,<3.0.0', 'tomlkit>=0.10.0,<1.0.0',
-'typing-extensions>=3.10.0,<5.0.0', 'yarl>=1.7.2,<2.0.0'] extras_require = \
-{'aiohttp': ['aiohttp[speedups]>=3.7.4,<4.0.0'], 'all':
-['websockets>=10.0,<11.0', 'Quart>=0.18.0,<1.0.0',
-'fastapi>=0.87.0,!=0.89.0,<1.0.0', 'aiohttp[speedups]>=3.7.4,<4.0.0', 'httpx
-[http2]>=0.20.0,<1.0.0', 'uvicorn[standard]>=0.20.0,<1.0.0'], 'fastapi':
-['fastapi>=0.87.0,!=0.89.0,<1.0.0', 'uvicorn[standard]>=0.20.0,<1.0.0'],
-'httpx': ['httpx[http2]>=0.20.0,<1.0.0'], 'quart': ['Quart>=0.18.0,<1.0.0',
-'uvicorn[standard]>=0.20.0,<1.0.0'], 'websockets': ['websockets>=10.0,<11.0']}
-setup_kwargs = { 'name': 'nonebot2', 'version': '2.0.0rc3', 'description': 'An
-asynchronous python bot framework.', 'long_description': '\n
+[dotenv]>=1.10.0,<2.0.0', 'pygtrie>=2.4.1,<3.0.0', 'typing-
+extensions>=4.0.0,<5.0.0', 'yarl>=1.7.2,<2.0.0'] extras_require = \ {':
+python_version < "3.11"': ['tomli>=2.0.1,<3.0.0'], 'aiohttp': ['aiohttp
+[speedups]>=3.7.4,<4.0.0'], 'all': ['websockets>=10.0,<11.0',
+'Quart>=0.18.0,<1.0.0', 'fastapi>=0.93.0,<1.0.0', 'aiohttp
+[speedups]>=3.7.4,<4.0.0', 'httpx[http2]>=0.20.0,<1.0.0', 'uvicorn
+[standard]>=0.20.0,<1.0.0'], 'fastapi': ['fastapi>=0.93.0,<1.0.0', 'uvicorn
+[standard]>=0.20.0,<1.0.0'], 'httpx': ['httpx[http2]>=0.20.0,<1.0.0'], 'quart':
+['Quart>=0.18.0,<1.0.0', 'uvicorn[standard]>=0.20.0,<1.0.0'], 'websockets':
+['websockets>=10.0,<11.0']} setup_kwargs = { 'name': 'nonebot2', 'version':
+'2.0.0rc4', 'description': 'An asynchronous python bot framework.',
+'long_description': '\n
                                 \n [nonebot]\n
 \n\n
   \n\n# NoneBot\n\n\n\n_â¨ è·¨å¹³å° Python å¼æ­¥æºå¨äººæ¡æ¶ â¨_\n\n\n
 \n\n
 \n \n_[license]\n\n \n_[pypi]\n\n [python]\n \n_[codecov]\n\n \n_[site]\n\n \n_
                                [pre-commit]\n\n
    \n \n_[onebot]\n\n \n_[onebot]\n\n \n_[telegram]\n\n \n_[feishu]\n\n \n_
                [github]\n\n \n_[QQé¢é]\n_\n_[dingtalk]\n\n\n
   \n \n_[QQ_Chat_Group]\n\n \n_[QQ_Channel]\n\n \n_[Telegram_Channel]\n\n \n_
                              [Discord_Server]\n\n
 \n\n
-    \n ææ¡£\n Â·\n å®è£\n Â·\n å¼å§ä½¿ç¨\n Â·\n ææ¡£æä¸å¼ï¼\n
+           \n ææ¡£\n Â·\n å¿«éä¸æ\n Â·\n ææ¡£æä¸å¼ï¼\n
 \n\n
                \n \n_[https://v2.nonebot.dev/img/setup.svg]\n\n
 \n\n## ç®ä»\n\nNoneBot2 æ¯ä¸ä¸ªç°ä»£ãè·¨å¹³å°ãå¯æ©å±ç Python
 èå¤©æºå¨äººæ¡æ¶ï¼å®åºäº Python
 çç±»åæ³¨è§£åå¼æ­¥ç¹æ§ï¼è½å¤ä¸ºä½ çéæ±å®ç°æä¾ä¾¿æ·çµæ´»çæ¯æã\n\n##
 ç¹è²\n\n- å¼æ­¥ä¼åï¼åºäº Python
 çå¼æ­¥ç¹æ§ï¼å³ä½¿æ¯~~éå¸¸~~å¤§éçæ¶æ¯ï¼ä¹è½ååèªå¦\n-
 æäºå¼åï¼éå NB-CLI
 èææ¶ï¼ä»£ç ç¼åä¸æç®åï¼æ²¡æè¿å¤çåä½ä»£ç ï¼å¯ä»¥è®©å¼åèä¸æ³¨äºä¸å¡é»è¾\n-
 çèå¯é ï¼100%
 ç±»åæ³¨è§£è¦çï¼éåç¼è¾å¨çç±»åæ¨å¯¼åè½ï¼è½å°ç»å¤§å¤æ°ç
-Bug æç»å¨ç¼è¾å¨ä¸­ ([ç¼è¾å¨æ¯æ](https://v2.nonebot.dev/docs/start/
+Bug æç»å¨ç¼è¾å¨ä¸­ ([ç¼è¾å¨æ¯æ](https://v2.nonebot.dev/docs/
 editor-support))\n-
 ç¤¾åºä¸°å¯ï¼ç¤¾åºç¨æ·ä¼å¤ï¼ç´æ¥åé´æ¥ç¨æ·è¶è¿åä¸äººï¼æ¯å¤©é½æå¤§éçæ´»è·ç¨æ·
 ([ç¤¾åºèµæº](#ç¤¾åºèµæº))\n-
 æµ·çº³ç¾å·ï¼ä¸ä¸ªæ¡æ¶ï¼æ¯æå¤ä¸ªèå¤©è½¯ä»¶å¹³å°ï¼å¯èªå®ä¹éä¿¡åè®®\n\n
 | åè®®åç§° | ç¶æ | æ³¨é |\n | :---------------------------------------
 --------------------------------: | :--: | :-----------------------------------
 -----------------------------: |\n | [OneBot åè®®](https://onebot.dev/) | â
```

### Comparing `nonebot2-2.0.0rc3/PKG-INFO` & `nonebot2-2.0.0rc4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot2
-Version: 2.0.0rc3
+Version: 2.0.0rc4
 Summary: An asynchronous python bot framework.
 Home-page: https://v2.nonebot.dev/
 License: MIT
 Keywords: bot,qq,qqbot,mirai,coolq
 Author: yanyongyu
 Author-email: yyy@nonebot.dev
 Requires-Python: >=3.8,<4.0
@@ -23,21 +23,21 @@
 Provides-Extra: all
 Provides-Extra: fastapi
 Provides-Extra: httpx
 Provides-Extra: quart
 Provides-Extra: websockets
 Requires-Dist: Quart (>=0.18.0,<1.0.0) ; extra == "quart" or extra == "all"
 Requires-Dist: aiohttp[speedups] (>=3.7.4,<4.0.0) ; extra == "aiohttp" or extra == "all"
-Requires-Dist: fastapi (>=0.87.0,!=0.89.0,<1.0.0) ; extra == "fastapi" or extra == "all"
+Requires-Dist: fastapi (>=0.93.0,<1.0.0) ; extra == "fastapi" or extra == "all"
 Requires-Dist: httpx[http2] (>=0.20.0,<1.0.0) ; extra == "httpx" or extra == "all"
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: pydantic[dotenv] (>=1.10.0,<2.0.0)
 Requires-Dist: pygtrie (>=2.4.1,<3.0.0)
-Requires-Dist: tomlkit (>=0.10.0,<1.0.0)
-Requires-Dist: typing-extensions (>=3.10.0,<5.0.0)
+Requires-Dist: tomli (>=2.0.1,<3.0.0) ; python_version < "3.11"
+Requires-Dist: typing-extensions (>=4.0.0,<5.0.0)
 Requires-Dist: uvicorn[standard] (>=0.20.0,<1.0.0) ; extra == "quart" or extra == "fastapi" or extra == "all"
 Requires-Dist: websockets (>=10.0,<11.0) ; extra == "websockets" or extra == "all"
 Requires-Dist: yarl (>=1.7.2,<2.0.0)
 Project-URL: Documentation, https://v2.nonebot.dev/
 Project-URL: Repository, https://github.com/nonebot/nonebot2
 Description-Content-Type: text/markdown
 
@@ -110,36 +110,34 @@
     <img src="https://discordapp.com/api/guilds/847819937858584596/widget.png?style=shield" alt="Discord Server">
   </a>
 </p>
 
 <p align="center">
   <a href="https://v2.nonebot.dev/">文档</a>
   ·
-  <a href="https://v2.nonebot.dev/docs/start/installation">安装</a>
-  ·
-  <a href="https://v2.nonebot.dev/docs/tutorial/create-project">开始使用</a>
+  <a href="https://v2.nonebot.dev/docs/quick-start">快速上手</a>
   ·
   <a href="#插件">文档打不开？</a>
 </p>
 
 <p align="center">
-  <a href="https://asciinema.org/a/464654">
+  <a href="https://asciinema.org/a/569440">
     <img src="https://v2.nonebot.dev/img/setup.svg">
   </a>
 </p>
 
 ## 简介
 
 NoneBot2 是一个现代、跨平台、可扩展的 Python 聊天机器人框架，它基于 Python 的类型注解和异步特性，能够为你的需求实现提供便捷灵活的支持。
 
 ## 特色
 
 - 异步优先：基于 Python 的异步特性，即使是~~非常~~大量的消息，也能吞吐自如
 - 易于开发：配合 NB-CLI 脚手架，代码编写上手简单，没有过多的冗余代码，可以让开发者专注于业务逻辑
-- 生而可靠：100% 类型注解覆盖，配合编辑器的类型推导功能，能将绝大多数的 Bug 杜绝在编辑器中 ([编辑器支持](https://v2.nonebot.dev/docs/start/editor-support))
+- 生而可靠：100% 类型注解覆盖，配合编辑器的类型推导功能，能将绝大多数的 Bug 杜绝在编辑器中 ([编辑器支持](https://v2.nonebot.dev/docs/editor-support))
 - 社区丰富：社区用户众多，直接和间接用户超过十万人，每天都有大量的活跃用户 ([社区资源](#社区资源))
 - 海纳百川：一个框架，支持多个聊天软件平台，可自定义通信协议
 
   |                                 协议名称                                  | 状态 |                                注释                                |
   | :-----------------------------------------------------------------------: | :--: | :----------------------------------------------------------------: |
   |                    [OneBot 协议](https://onebot.dev/)                     |  ✅  | 支持 QQ、TG、微信公众号等[平台](https://onebot.dev/ecosystem.html) |
   |              [Telegram](https://core.telegram.org/bots/api)               |  ✅  |                                                                    |
```

#### html2text {}

```diff
@@ -1,49 +1,49 @@
-Metadata-Version: 2.1 Name: nonebot2 Version: 2.0.0rc3 Summary: An asynchronous
+Metadata-Version: 2.1 Name: nonebot2 Version: 2.0.0rc4 Summary: An asynchronous
 python bot framework. Home-page: https://v2.nonebot.dev/ License: MIT Keywords:
 bot,qq,qqbot,mirai,coolq Author: yanyongyu Author-email: yyy@nonebot.dev
 Requires-Python: >=3.8,<4.0 Classifier: Development Status :: 5 - Production/
 Stable Classifier: Framework :: Robot Framework Classifier: Framework :: Robot
 Framework :: Library Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3 Provides-Extra: aiohttp Provides-Extra: all
 Provides-Extra: fastapi Provides-Extra: httpx Provides-Extra: quart Provides-
 Extra: websockets Requires-Dist: Quart (>=0.18.0,<1.0.0) ; extra == "quart" or
 extra == "all" Requires-Dist: aiohttp[speedups] (>=3.7.4,<4.0.0) ; extra ==
-"aiohttp" or extra == "all" Requires-Dist: fastapi (>=0.87.0,!=0.89.0,<1.0.0) ;
-extra == "fastapi" or extra == "all" Requires-Dist: httpx[http2]
-(>=0.20.0,<1.0.0) ; extra == "httpx" or extra == "all" Requires-Dist: loguru
-(>=0.6.0,<0.7.0) Requires-Dist: pydantic[dotenv] (>=1.10.0,<2.0.0) Requires-
-Dist: pygtrie (>=2.4.1,<3.0.0) Requires-Dist: tomlkit (>=0.10.0,<1.0.0)
-Requires-Dist: typing-extensions (>=3.10.0,<5.0.0) Requires-Dist: uvicorn
+"aiohttp" or extra == "all" Requires-Dist: fastapi (>=0.93.0,<1.0.0) ; extra ==
+"fastapi" or extra == "all" Requires-Dist: httpx[http2] (>=0.20.0,<1.0.0) ;
+extra == "httpx" or extra == "all" Requires-Dist: loguru (>=0.6.0,<0.7.0)
+Requires-Dist: pydantic[dotenv] (>=1.10.0,<2.0.0) Requires-Dist: pygtrie
+(>=2.4.1,<3.0.0) Requires-Dist: tomli (>=2.0.1,<3.0.0) ; python_version <
+"3.11" Requires-Dist: typing-extensions (>=4.0.0,<5.0.0) Requires-Dist: uvicorn
 [standard] (>=0.20.0,<1.0.0) ; extra == "quart" or extra == "fastapi" or extra
 == "all" Requires-Dist: websockets (>=10.0,<11.0) ; extra == "websockets" or
 extra == "all" Requires-Dist: yarl (>=1.7.2,<2.0.0) Project-URL: Documentation,
 https://v2.nonebot.dev/ Project-URL: Repository, https://github.com/nonebot/
 nonebot2 Description-Content-Type: text/markdown
                                    [nonebot]
          # NoneBot   _â¨ è·¨å¹³å° Python å¼æ­¥æºå¨äººæ¡æ¶ â¨_
            [license] [pypi] [python] [codecov] [site] [pre-commit]
      [onebot] [onebot] [telegram] [feishu] [github] [QQé¢é]_[dingtalk]
        [QQ_Chat_Group] [QQ_Channel] [Telegram_Channel] [Discord_Server]
-            ææ¡£ Â· å®è£ Â· å¼å§ä½¿ç¨ Â· ææ¡£æä¸å¼ï¼
+                 ææ¡£ Â· å¿«éä¸æ Â· ææ¡£æä¸å¼ï¼
                     [https://v2.nonebot.dev/img/setup.svg]
 ## ç®ä» NoneBot2 æ¯ä¸ä¸ªç°ä»£ãè·¨å¹³å°ãå¯æ©å±ç Python
 èå¤©æºå¨äººæ¡æ¶ï¼å®åºäº Python
 çç±»åæ³¨è§£åå¼æ­¥ç¹æ§ï¼è½å¤ä¸ºä½ çéæ±å®ç°æä¾ä¾¿æ·çµæ´»çæ¯æã
 ## ç¹è² - å¼æ­¥ä¼åï¼åºäº Python
 çå¼æ­¥ç¹æ§ï¼å³ä½¿æ¯~~éå¸¸~~å¤§éçæ¶æ¯ï¼ä¹è½ååèªå¦ -
 æäºå¼åï¼éå NB-CLI
 èææ¶ï¼ä»£ç ç¼åä¸æç®åï¼æ²¡æè¿å¤çåä½ä»£ç ï¼å¯ä»¥è®©å¼åèä¸æ³¨äºä¸å¡é»è¾
 - çèå¯é ï¼100%
 ç±»åæ³¨è§£è¦çï¼éåç¼è¾å¨çç±»åæ¨å¯¼åè½ï¼è½å°ç»å¤§å¤æ°ç
-Bug æç»å¨ç¼è¾å¨ä¸­ ([ç¼è¾å¨æ¯æ](https://v2.nonebot.dev/docs/start/
+Bug æç»å¨ç¼è¾å¨ä¸­ ([ç¼è¾å¨æ¯æ](https://v2.nonebot.dev/docs/
 editor-support)) -
 ç¤¾åºä¸°å¯ï¼ç¤¾åºç¨æ·ä¼å¤ï¼ç´æ¥åé´æ¥ç¨æ·è¶è¿åä¸äººï¼æ¯å¤©é½æå¤§éçæ´»è·ç¨æ·
 ([ç¤¾åºèµæº](#ç¤¾åºèµæº)) -
 æµ·çº³ç¾å·ï¼ä¸ä¸ªæ¡æ¶ï¼æ¯æå¤ä¸ªèå¤©è½¯ä»¶å¹³å°ï¼å¯èªå®ä¹éä¿¡åè®®
 | åè®®åç§° | ç¶æ | æ³¨é | | :-----------------------------------------
 ------------------------------: | :--: | :-------------------------------------
 ---------------------------: | | [OneBot åè®®](https://onebot.dev/) | â |
```

