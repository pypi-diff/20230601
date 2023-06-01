# Comparing `tmp/nonebot_plugin_arkgacha-0.2.2.tar.gz` & `tmp/nonebot_plugin_arkgacha-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_arkgacha-0.2.2.tar", last modified: Thu May 18 05:20:05 2023, max compression
+gzip compressed data, was "nonebot_plugin_arkgacha-0.3.0.tar", last modified: Thu Jun  1 09:28:49 2023, max compression
```

## Comparing `nonebot_plugin_arkgacha-0.2.2.tar` & `nonebot_plugin_arkgacha-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    34522 2021-09-10 07:59:22.042000 nonebot_plugin_arkgacha-0.2.2/LICENSE
--rw-r--r--   0        0        0     2131 2023-05-13 08:16:56.047078 nonebot_plugin_arkgacha-0.2.2/README.md
--rw-r--r--   0        0        0     5978 2023-05-13 12:33:50.274594 nonebot_plugin_arkgacha-0.2.2/nonebot_plugin_arkgacha/__init__.py
--rw-r--r--   0        0        0      250 2023-05-13 08:21:01.844002 nonebot_plugin_arkgacha-0.2.2/nonebot_plugin_arkgacha/config.py
--rw-r--r--   0        0        0      704 2023-05-18 05:20:05.708900 nonebot_plugin_arkgacha-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2624 1970-01-01 00:00:00.000000 nonebot_plugin_arkgacha-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    34522 2021-09-10 07:59:22.042000 nonebot_plugin_arkgacha-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2131 2023-05-13 08:16:56.047078 nonebot_plugin_arkgacha-0.3.0/README.md
+-rw-r--r--   0        0        0     6180 2023-06-01 09:16:45.506306 nonebot_plugin_arkgacha-0.3.0/nonebot_plugin_arkgacha/__init__.py
+-rw-r--r--   0        0        0      250 2023-05-13 08:21:01.844002 nonebot_plugin_arkgacha-0.3.0/nonebot_plugin_arkgacha/config.py
+-rw-r--r--   0        0        0      679 2023-06-01 09:28:49.656286 nonebot_plugin_arkgacha-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2591 1970-01-01 00:00:00.000000 nonebot_plugin_arkgacha-0.3.0/PKG-INFO
```

### Comparing `nonebot_plugin_arkgacha-0.2.2/LICENSE` & `nonebot_plugin_arkgacha-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_arkgacha-0.2.2/README.md` & `nonebot_plugin_arkgacha-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_arkgacha-0.2.2/nonebot_plugin_arkgacha/__init__.py` & `nonebot_plugin_arkgacha-0.3.0/nonebot_plugin_arkgacha/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,18 +27,27 @@
 driver = get_driver()
 global_config = driver.config
 config = Config.parse_obj(global_config)
 
 __plugin_meta__ = PluginMetadata(
     name="明日方舟抽卡模拟",
     description="明模拟日方舟抽卡功能，支持模拟十连",
-    usage="方舟抽卡 / 方舟十连",
+    usage="""\
+方舟抽卡 [count = 10]
+方舟十连
+方舟抽卡帮助
+方舟卡池更新    
+""",
+    homepage="https://github.com/RF-Tar-Railt/nonebot-plugin-arkgacha",
+    type="application",
+    config=Config,
     extra={
         "author": "RF-Tar-Railt",
-        'priority': 16,
+        'priority': 3,
+        "version": "0.3.0",
     }
 )
 
 
 gacha = ArknightsGacha(config.arkgacha_pool_file or get_data_file("arkgacha", "pool.json"))
 user_cache_file = get_cache_file("arkgacha", "user.json")
 if not user_cache_file.exists():
```

### Comparing `nonebot_plugin_arkgacha-0.2.2/pyproject.toml` & `nonebot_plugin_arkgacha-0.3.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 [project]
 name = "nonebot-plugin-arkgacha"
-version = "0.2.2"
+version = "0.3.0"
 description = "Plugin for Arknights gacha, support multi platform"
 authors = [
-    { name = "RF-Tar-Railt", email = "3165388245@qq.com" },
+    { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
-    "nonebot2>=2.0.0rc4",
-    "nonebot-plugin-alconna>=0.4.2",
+    "nonebot2>=2.0.0",
+    "nonebot-plugin-alconna>=0.7.0",
     "nonebot-plugin-send-anything-anywhere>=0.2.4",
     "arknights-toolkit<0.6.0, >=0.5.8",
     "nonebot-plugin-localstore>=0.4.1",
     "nonebot-plugin-apscheduler>=0.2.0",
-    "nepattern>=0.5.7",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
```

### Comparing `nonebot_plugin_arkgacha-0.2.2/PKG-INFO` & `nonebot_plugin_arkgacha-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-arkgacha
-Version: 0.2.2
+Version: 0.3.0
 Summary: Plugin for Arknights gacha, support multi platform
-Author-Email: RF-Tar-Railt <3165388245@qq.com>
+Author-Email: RF-Tar-Railt <rf_tar_railt@qq.com>
 License: MIT
 Requires-Python: >=3.8
-Requires-Dist: nonebot2>=2.0.0rc4
-Requires-Dist: nonebot-plugin-alconna>=0.4.2
+Requires-Dist: nonebot2>=2.0.0
+Requires-Dist: nonebot-plugin-alconna>=0.7.0
 Requires-Dist: nonebot-plugin-send-anything-anywhere>=0.2.4
 Requires-Dist: arknights-toolkit<0.6.0,>=0.5.8
 Requires-Dist: nonebot-plugin-localstore>=0.4.1
 Requires-Dist: nonebot-plugin-apscheduler>=0.2.0
-Requires-Dist: nepattern>=0.5.7
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
 </p>
 
 <div align="center">
```

#### html2text {}

```diff
@@ -1,15 +1,14 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-arkgacha Version: 0.2.2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-arkgacha Version: 0.3.0 Summary:
 Plugin for Arknights gacha, support multi platform Author-Email: RF-Tar-Railt
-<3165388245@qq.com> License: MIT Requires-Python: >=3.8 Requires-Dist:
-nonebot2>=2.0.0rc4 Requires-Dist: nonebot-plugin-alconna>=0.4.2 Requires-Dist:
-nonebot-plugin-send-anything-anywhere>=0.2.4 Requires-Dist: arknights-
-toolkit<0.6.0,>=0.5.8 Requires-Dist: nonebot-plugin-localstore>=0.4.1 Requires-
-Dist: nonebot-plugin-apscheduler>=0.2.0 Requires-Dist: nepattern>=0.5.7
-Description-Content-Type: text/markdown
+qq.com> License: MIT Requires-Python: >=3.8 Requires-Dist: nonebot2>=2.0.0
+Requires-Dist: nonebot-plugin-alconna>=0.7.0 Requires-Dist: nonebot-plugin-
+send-anything-anywhere>=0.2.4 Requires-Dist: arknights-toolkit<0.6.0,>=0.5.8
+Requires-Dist: nonebot-plugin-localstore>=0.4.1 Requires-Dist: nonebot-plugin-
+apscheduler>=0.2.0 Description-Content-Type: text/markdown
                                    [nonebot]
         # NoneBot Plugin Arkgacha _â¨ ææ¥æ¹èæ½å¡æ¨¡æå¨ â¨_
                            [license] [pypi] [python]
 è¯¥æä»¶æä¾äºæ¨¡æææ¥æ¹èæ½å¡çåè½ï¼åæ¬æ å¤´å½¢å¼çæ½å¡æ¨¡æä¸æ¨¡æåè¿
 éè¿ä½¿ç¨ [`saa`](https://github.com/felinae98/nonebot-plugin-send-anything-
 anywhere) æä»¶ééå¤å¹³å° ## å®è£ ```bash $ pip install nonebot-plugin-
 arkgacha ``` ```bash $ nb plugin install nonebot-plugin-arkgacha ```
```

