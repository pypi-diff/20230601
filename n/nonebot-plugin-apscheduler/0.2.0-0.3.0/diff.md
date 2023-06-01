# Comparing `tmp/nonebot-plugin-apscheduler-0.2.0.tar.gz` & `tmp/nonebot_plugin_apscheduler-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-apscheduler-0.2.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_apscheduler-0.3.0.tar", max compression
```

## Comparing `nonebot-plugin-apscheduler-0.2.0.tar` & `nonebot_plugin_apscheduler-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1064 2022-10-02 15:18:38.885439 nonebot-plugin-apscheduler-0.2.0/LICENSE
--rw-r--r--   0        0        0     1844 2022-10-02 15:18:38.885439 nonebot-plugin-apscheduler-0.2.0/README.md
--rw-r--r--   0        0        0      973 2022-10-02 15:18:38.885439 nonebot-plugin-apscheduler-0.2.0/nonebot_plugin_apscheduler/__init__.py
--rw-r--r--   0        0        0      308 2022-10-02 15:18:38.885439 nonebot-plugin-apscheduler-0.2.0/nonebot_plugin_apscheduler/config.py
--rw-r--r--   0        0        0     1049 2022-10-02 15:18:38.885439 nonebot-plugin-apscheduler-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2636 1970-01-01 00:00:00.000000 nonebot-plugin-apscheduler-0.2.0/setup.py
--rw-r--r--   0        0        0     2636 1970-01-01 00:00:00.000000 nonebot-plugin-apscheduler-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-01 09:16:43.958431 nonebot_plugin_apscheduler-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1838 2023-06-01 09:16:43.958431 nonebot_plugin_apscheduler-0.3.0/README.md
+-rw-r--r--   0        0        0     1473 2023-06-01 09:16:43.958431 nonebot_plugin_apscheduler-0.3.0/nonebot_plugin_apscheduler/__init__.py
+-rw-r--r--   0        0        0      308 2023-06-01 09:16:43.958431 nonebot_plugin_apscheduler-0.3.0/nonebot_plugin_apscheduler/config.py
+-rw-r--r--   0        0        0     1028 2023-06-01 09:16:43.962431 nonebot_plugin_apscheduler-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2676 1970-01-01 00:00:00.000000 nonebot_plugin_apscheduler-0.3.0/PKG-INFO
```

### Comparing `nonebot-plugin-apscheduler-0.2.0/LICENSE` & `nonebot_plugin_apscheduler-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-apscheduler-0.2.0/README.md` & `nonebot_plugin_apscheduler-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <p align="center">
-  <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
+  <a href="https://nonebot.dev/"><img src="https://nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
 </p>
 
 <div align="center">
 
 # NoneBot Plugin APScheduler
 
 _✨ NoneBot APScheduler 定时任务插件 ✨_
```

### Comparing `nonebot-plugin-apscheduler-0.2.0/nonebot_plugin_apscheduler/__init__.py` & `nonebot_plugin_apscheduler-0.3.0/nonebot_plugin_apscheduler/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,31 @@
 import logging
 
 from nonebot import get_driver
+from nonebot.plugin import PluginMetadata
 from nonebot.log import LoguruHandler, logger
 from apscheduler.schedulers.asyncio import AsyncIOScheduler
 
 from .config import Config
 
+__plugin_meta__ = PluginMetadata(
+    name="定时任务",
+    description="APScheduler 定时任务插件",
+    usage=(
+        '声明依赖: `require("nonebot_plugin_apscheduler")\n'
+        "导入调度器: `from nonebot_plugin_apscheduler import scheduler`\n"
+        "添加任务: `scheduler.add_job(...)`\n"
+    ),
+    type="library",
+    homepage="https://github.com/nonebot/plugin-apscheduler",
+    config=Config,
+    supported_adapters=None,
+)
+
+
 driver = get_driver()
 global_config = driver.config
 plugin_config = Config(**global_config.dict())
 
 scheduler = AsyncIOScheduler()
 scheduler.configure(plugin_config.apscheduler_config)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nonebot-plugin-apscheduler-0.2.0/pyproject.toml` & `nonebot_plugin_apscheduler-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,46 @@
 [tool.poetry]
 name = "nonebot-plugin-apscheduler"
-version = "0.2.0"
+version = "0.3.0"
 description = "APScheduler Support for NoneBot2"
 authors = ["yanyongyu <yyy@nonebot.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/nonebot/plugin-apscheduler"
 repository = "https://github.com/nonebot/plugin-apscheduler"
 documentation = "https://github.com/nonebot/plugin-apscheduler#readme"
 
 [tool.poetry.dependencies]
 python = "^3.8"
+nonebot2 = "^2.0.0"
 apscheduler = "^3.7.0"
-nonebot2 = "^2.0.0-rc.1"
 
 [tool.poetry.group.dev.dependencies]
+pycln = "^2.1.4"
 isort = "^5.10.1"
 black = "^22.3.0"
 nonemoji = "^0.1.2"
 pre-commit = "^2.19.0"
-nonebot2 = { git = "https://github.com/nonebot/nonebot2.git" }
 
 [tool.black]
 line-length = 88
-target-version = ["py37", "py38", "py39", "py310"]
+target-version = ["py38", "py39", "py310"]
 include = '\.pyi?$'
 extend-exclude = '''
 '''
 
 [tool.isort]
 profile = "black"
 line_length = 88
 length_sort = true
 skip_gitignore = true
 force_sort_within_sections = true
 extra_standard_library = ["typing_extensions"]
 
+
+[tool.pycln]
+path = "."
+all = false
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot-plugin-apscheduler-0.2.0/setup.py` & `nonebot_plugin_apscheduler-0.3.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,165 +1,168 @@
-00000000: 2320 2d2a 2d20 636f 6469 6e67 3a20 7574  # -*- coding: ut
-00000010: 662d 3820 2d2a 2d0a 6672 6f6d 2073 6574  f-8 -*-.from set
-00000020: 7570 746f 6f6c 7320 696d 706f 7274 2073  uptools import s
-00000030: 6574 7570 0a0a 7061 636b 6167 6573 203d  etup..packages =
-00000040: 205c 0a5b 276e 6f6e 6562 6f74 5f70 6c75   \.['nonebot_plu
-00000050: 6769 6e5f 6170 7363 6865 6475 6c65 7227  gin_apscheduler'
-00000060: 5d0a 0a70 6163 6b61 6765 5f64 6174 6120  ]..package_data 
-00000070: 3d20 5c0a 7b27 273a 205b 272a 275d 7d0a  = \.{'': ['*']}.
-00000080: 0a69 6e73 7461 6c6c 5f72 6571 7569 7265  .install_require
-00000090: 7320 3d20 5c0a 5b27 6170 7363 6865 6475  s = \.['apschedu
-000000a0: 6c65 723e 3d33 2e37 2e30 2c3c 342e 302e  ler>=3.7.0,<4.0.
-000000b0: 3027 2c20 276e 6f6e 6562 6f74 323e 3d32  0', 'nonebot2>=2
-000000c0: 2e30 2e30 2d72 632e 312c 3c33 2e30 2e30  .0.0-rc.1,<3.0.0
-000000d0: 275d 0a0a 7365 7475 705f 6b77 6172 6773  ']..setup_kwargs
-000000e0: 203d 207b 0a20 2020 2027 6e61 6d65 273a   = {.    'name':
-000000f0: 2027 6e6f 6e65 626f 742d 706c 7567 696e   'nonebot-plugin
-00000100: 2d61 7073 6368 6564 756c 6572 272c 0a20  -apscheduler',. 
-00000110: 2020 2027 7665 7273 696f 6e27 3a20 2730     'version': '0
-00000120: 2e32 2e30 272c 0a20 2020 2027 6465 7363  .2.0',.    'desc
-00000130: 7269 7074 696f 6e27 3a20 2741 5053 6368  ription': 'APSch
-00000140: 6564 756c 6572 2053 7570 706f 7274 2066  eduler Support f
-00000150: 6f72 204e 6f6e 6542 6f74 3227 2c0a 2020  or NoneBot2',.  
-00000160: 2020 276c 6f6e 675f 6465 7363 7269 7074    'long_descript
-00000170: 696f 6e27 3a20 273c 7020 616c 6967 6e3d  ion': '<p align=
-00000180: 2263 656e 7465 7222 3e5c 6e20 203c 6120  "center">\n  <a 
-00000190: 6872 6566 3d22 6874 7470 733a 2f2f 7632  href="https://v2
-000001a0: 2e6e 6f6e 6562 6f74 2e64 6576 2f22 3e3c  .nonebot.dev/"><
-000001b0: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-000001c0: 2f76 322e 6e6f 6e65 626f 742e 6465 762f  /v2.nonebot.dev/
-000001d0: 6c6f 676f 2e70 6e67 2220 7769 6474 683d  logo.png" width=
-000001e0: 2232 3030 2220 6865 6967 6874 3d22 3230  "200" height="20
-000001f0: 3022 2061 6c74 3d22 6e6f 6e65 626f 7422  0" alt="nonebot"
-00000200: 3e3c 2f61 3e5c 6e3c 2f70 3e5c 6e5c 6e3c  ></a>\n</p>\n\n<
-00000210: 6469 7620 616c 6967 6e3d 2263 656e 7465  div align="cente
-00000220: 7222 3e5c 6e5c 6e23 204e 6f6e 6542 6f74  r">\n\n# NoneBot
-00000230: 2050 6c75 6769 6e20 4150 5363 6865 6475   Plugin APSchedu
-00000240: 6c65 725c 6e5c 6e5f e29c a820 4e6f 6e65  ler\n\n_... None
-00000250: 426f 7420 4150 5363 6865 6475 6c65 7220  Bot APScheduler 
-00000260: e5ae 9ae6 97b6 e4bb bbe5 8aa1 e68f 92e4  ................
-00000270: bbb6 20e2 9ca8 5f5c 6e5c 6e3c 2f64 6976  .. ..._\n\n</div
-00000280: 3e5c 6e5c 6e3c 7020 616c 6967 6e3d 2263  >\n\n<p align="c
-00000290: 656e 7465 7222 3e5c 6e20 203c 6120 6872  enter">\n  <a hr
-000002a0: 6566 3d22 6874 7470 733a 2f2f 7261 772e  ef="https://raw.
-000002b0: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
-000002c0: 742e 636f 6d2f 6e6f 6e65 626f 742f 706c  t.com/nonebot/pl
-000002d0: 7567 696e 2d61 7073 6368 6564 756c 6572  ugin-apscheduler
-000002e0: 2f6d 6173 7465 722f 4c49 4345 4e53 4522  /master/LICENSE"
-000002f0: 3e5c 6e20 2020 203c 696d 6720 7372 633d  >\n    <img src=
-00000300: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
-00000310: 656c 6473 2e69 6f2f 6769 7468 7562 2f6c  elds.io/github/l
-00000320: 6963 656e 7365 2f6e 6f6e 6562 6f74 2f70  icense/nonebot/p
-00000330: 6c75 6769 6e2d 6170 7363 6865 6475 6c65  lugin-apschedule
-00000340: 722e 7376 6722 2061 6c74 3d22 6c69 6365  r.svg" alt="lice
-00000350: 6e73 6522 3e5c 6e20 203c 2f61 3e5c 6e20  nse">\n  </a>\n 
-00000360: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
-00000370: 2f2f 7079 7069 2e70 7974 686f 6e2e 6f72  //pypi.python.or
-00000380: 672f 7079 7069 2f6e 6f6e 6562 6f74 2d70  g/pypi/nonebot-p
-00000390: 6c75 6769 6e2d 6170 7363 6865 6475 6c65  lugin-apschedule
-000003a0: 7222 3e5c 6e20 2020 203c 696d 6720 7372  r">\n    <img sr
-000003b0: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
-000003c0: 6869 656c 6473 2e69 6f2f 7079 7069 2f76  hields.io/pypi/v
-000003d0: 2f6e 6f6e 6562 6f74 2d70 6c75 6769 6e2d  /nonebot-plugin-
-000003e0: 6170 7363 6865 6475 6c65 722e 7376 6722  apscheduler.svg"
-000003f0: 2061 6c74 3d22 7079 7069 223e 5c6e 2020   alt="pypi">\n  
-00000400: 3c2f 613e 5c6e 2020 3c69 6d67 2073 7263  </a>\n  <img src
-00000410: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
-00000420: 6965 6c64 732e 696f 2f62 6164 6765 2f70  ields.io/badge/p
-00000430: 7974 686f 6e2d 332e 372b 2d62 6c75 652e  ython-3.7+-blue.
-00000440: 7376 6722 2061 6c74 3d22 7079 7468 6f6e  svg" alt="python
-00000450: 223e 5c6e 3c2f 703e 5c6e 5c6e 2323 20e4  ">\n</p>\n\n## .
-00000460: bdbf e794 a8e6 96b9 e5bc 8f5c 6e5c 6ee5  ...........\n\n.
-00000470: 8aa0 e8bd bde6 8f92 e4bb b6e5 908e e4bd  ................
-00000480: bfe7 94a8 2060 7265 7175 6972 6560 20e8  .... `require` .
-00000490: 8eb7 e58f 9620 6073 6368 6564 756c 6572  ..... `scheduler
-000004a0: 6020 e5af b9e8 b1a1 efbc 88e8 afb7 e6b3  ` ..............
-000004b0: a8e6 848f e68f 92e4 bbb6 e58a a0e8 bdbd  ................
-000004c0: e9a1 bae5 ba8f efbc 895c 6e5c 6e60 6060  .........\n\n```
-000004d0: 7079 7468 6f6e 5c6e 6672 6f6d 206e 6f6e  python\nfrom non
-000004e0: 6562 6f74 2069 6d70 6f72 7420 7265 7175  ebot import requ
-000004f0: 6972 655c 6e5c 6e72 6571 7569 7265 2822  ire\n\nrequire("
-00000500: 6e6f 6e65 626f 745f 706c 7567 696e 5f61  nonebot_plugin_a
-00000510: 7073 6368 6564 756c 6572 2229 5c6e 5c6e  pscheduler")\n\n
-00000520: 6672 6f6d 206e 6f6e 6562 6f74 5f70 6c75  from nonebot_plu
-00000530: 6769 6e5f 6170 7363 6865 6475 6c65 7220  gin_apscheduler 
-00000540: 696d 706f 7274 2073 6368 6564 756c 6572  import scheduler
-00000550: 5c6e 5c6e 4073 6368 6564 756c 6572 2e73  \n\n@scheduler.s
-00000560: 6368 6564 756c 6564 5f6a 6f62 2822 6372  cheduled_job("cr
-00000570: 6f6e 222c 2068 6f75 723d 222a 2f32 222c  on", hour="*/2",
-00000580: 2069 643d 2278 7878 222c 2061 7267 733d   id="xxx", args=
-00000590: 5b31 5d2c 206b 7761 7267 733d 7b22 6172  [1], kwargs={"ar
-000005a0: 6732 223a 2032 7d29 5c6e 6173 796e 6320  g2": 2})\nasync 
-000005b0: 6465 6620 7275 6e5f 6576 6572 795f 325f  def run_every_2_
-000005c0: 686f 7572 2861 7267 312c 2061 7267 3229  hour(arg1, arg2)
-000005d0: 3a5c 6e20 2020 2070 6173 735c 6e5c 6e73  :\n    pass\n\ns
-000005e0: 6368 6564 756c 6572 2e61 6464 5f6a 6f62  cheduler.add_job
-000005f0: 2872 756e 5f65 7665 7279 5f64 6179 5f66  (run_every_day_f
-00000600: 726f 6d5f 7072 6f67 7261 6d5f 7374 6172  rom_program_star
-00000610: 742c 2022 696e 7465 7276 616c 222c 2064  t, "interval", d
-00000620: 6179 733d 312c 2069 643d 2278 7878 2229  ays=1, id="xxx")
-00000630: 5c6e 6060 605c 6e5c 6e23 2320 e985 8de7  \n```\n\n## ....
-00000640: bdae e9a1 b95c 6e5c 6e23 2323 2061 7073  .....\n\n### aps
-00000650: 6368 6564 756c 6572 5f61 7574 6f73 7461  cheduler_autosta
-00000660: 7274 5c6e 5c6e e698 afe5 90a6 e887 aae5  rt\n\n..........
-00000670: 8aa8 e590 afe5 8aa8 2060 7363 6865 6475  ........ `schedu
-00000680: 6c65 7260 5c6e 5c6e 2323 2320 6170 7363  ler`\n\n### apsc
-00000690: 6865 6475 6c65 725f 6c6f 675f 6c65 7665  heduler_log_leve
-000006a0: 6c5c 6e5c 6e60 696e 7460 20e7 b1bb e59e  l\n\n`int` .....
-000006b0: 8be6 97a5 e5bf 97e7 ad89 e7ba a75c 6e5c  .............\n\
-000006c0: 6e2d 2060 5741 524e 494e 4760 203d 2060  n- `WARNING` = `
-000006d0: 3330 6020 28e9 bb98 e8ae a429 5c6e 2d20  30` (......)\n- 
-000006e0: 6049 4e46 4f60 203d 2060 3230 605c 6e2d  `INFO` = `20`\n-
-000006f0: 2060 4445 4255 4760 203d 2060 3130 6020   `DEBUG` = `10` 
-00000700: 28e5 8faa e69c 89e5 9ca8 e5bc 80e5 90af  (...............
-00000710: 206e 6f6e 6562 6f74 20e7 9a84 2064 6562   nonebot ... deb
-00000720: 7567 20e6 a8a1 e5bc 8fe6 898d e4bc 9ae6  ug .............
-00000730: 98be e7a4 ba20 6465 6275 6720 e697 a5e5  ..... debug ....
-00000740: bf97 295c 6e5c 6e23 2323 2061 7073 6368  ..)\n\n### apsch
-00000750: 6564 756c 6572 5f63 6f6e 6669 675c 6e5c  eduler_config\n\
-00000760: 6e60 6170 7363 6865 6475 6c65 7260 20e7  n`apscheduler` .
-00000770: 9a84 e79b b8e5 85b3 e985 8de7 bdae e380  ................
-00000780: 82e5 8f82 e880 8320 5be9 858d e7bd ae20  ....... [...... 
-00000790: 7363 6865 6475 6c65 725d 2868 7474 7073  scheduler](https
-000007a0: 3a2f 2f61 7073 6368 6564 756c 6572 2e72  ://apscheduler.r
-000007b0: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
-000007c0: 2f6c 6174 6573 742f 7573 6572 6775 6964  /latest/userguid
-000007d0: 652e 6874 6d6c 2373 6368 6564 756c 6572  e.html#scheduler
-000007e0: 2d63 6f6e 6669 6729 2c20 5be9 858d e7bd  -config), [.....
-000007f0: aee5 8f82 e695 b05d 2868 7474 7073 3a2f  .......](https:/
-00000800: 2f61 7073 6368 6564 756c 6572 2e72 6561  /apscheduler.rea
-00000810: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
-00000820: 6174 6573 742f 6d6f 6475 6c65 732f 7363  atest/modules/sc
-00000830: 6865 6475 6c65 7273 2f62 6173 652e 6874  hedulers/base.ht
-00000840: 6d6c 2361 7073 6368 6564 756c 6572 2e73  ml#apscheduler.s
-00000850: 6368 6564 756c 6572 732e 6261 7365 2e42  chedulers.base.B
-00000860: 6173 6553 6368 6564 756c 6572 295c 6e5c  aseScheduler)\n\
-00000870: 6ee9 858d e7bd aee9 9c80 e8a6 81e5 8c85  n...............
-00000880: e590 ab20 6070 7265 6669 783a 2061 7073  ... `prefix: aps
-00000890: 6368 6564 756c 6572 2e60 5c6e 5c6e e9bb  cheduler.`\n\n..
-000008a0: 98e8 aea4 e985 8de7 bdae efbc 9a5c 6e5c  .............\n\
-000008b0: 6e60 6060 6a73 6f6e 5c6e 7b20 2261 7073  n```json\n{ "aps
-000008c0: 6368 6564 756c 6572 2e74 696d 657a 6f6e  cheduler.timezon
-000008d0: 6522 3a20 2241 7369 612f 5368 616e 6768  e": "Asia/Shangh
-000008e0: 6169 2220 7d5c 6e60 6060 5c6e 272c 0a20  ai" }\n```\n',. 
-000008f0: 2020 2027 6175 7468 6f72 273a 2027 7961     'author': 'ya
-00000900: 6e79 6f6e 6779 7527 2c0a 2020 2020 2761  nyongyu',.    'a
-00000910: 7574 686f 725f 656d 6169 6c27 3a20 2779  uthor_email': 'y
-00000920: 7979 406e 6f6e 6562 6f74 2e64 6576 272c  yy@nonebot.dev',
-00000930: 0a20 2020 2027 6d61 696e 7461 696e 6572  .    'maintainer
-00000940: 273a 2027 4e6f 6e65 272c 0a20 2020 2027  ': 'None',.    '
-00000950: 6d61 696e 7461 696e 6572 5f65 6d61 696c  maintainer_email
-00000960: 273a 2027 4e6f 6e65 272c 0a20 2020 2027  ': 'None',.    '
-00000970: 7572 6c27 3a20 2768 7474 7073 3a2f 2f67  url': 'https://g
-00000980: 6974 6875 622e 636f 6d2f 6e6f 6e65 626f  ithub.com/nonebo
-00000990: 742f 706c 7567 696e 2d61 7073 6368 6564  t/plugin-apsched
-000009a0: 756c 6572 272c 0a20 2020 2027 7061 636b  uler',.    'pack
-000009b0: 6167 6573 273a 2070 6163 6b61 6765 732c  ages': packages,
-000009c0: 0a20 2020 2027 7061 636b 6167 655f 6461  .    'package_da
-000009d0: 7461 273a 2070 6163 6b61 6765 5f64 6174  ta': package_dat
-000009e0: 612c 0a20 2020 2027 696e 7374 616c 6c5f  a,.    'install_
-000009f0: 7265 7175 6972 6573 273a 2069 6e73 7461  requires': insta
-00000a00: 6c6c 5f72 6571 7569 7265 732c 0a20 2020  ll_requires,.   
-00000a10: 2027 7079 7468 6f6e 5f72 6571 7569 7265   'python_require
-00000a20: 7327 3a20 273e 3d33 2e38 2c3c 342e 3027  s': '>=3.8,<4.0'
-00000a30: 2c0a 7d0a 0a0a 7365 7475 7028 2a2a 7365  ,.}...setup(**se
-00000a40: 7475 705f 6b77 6172 6773 290a            tup_kwargs).
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 6e6f 6e65  : 2.1.Name: none
+00000020: 626f 742d 706c 7567 696e 2d61 7073 6368  bot-plugin-apsch
+00000030: 6564 756c 6572 0a56 6572 7369 6f6e 3a20  eduler.Version: 
+00000040: 302e 332e 300a 5375 6d6d 6172 793a 2041  0.3.0.Summary: A
+00000050: 5053 6368 6564 756c 6572 2053 7570 706f  PScheduler Suppo
+00000060: 7274 2066 6f72 204e 6f6e 6542 6f74 320a  rt for NoneBot2.
+00000070: 486f 6d65 2d70 6167 653a 2068 7474 7073  Home-page: https
+00000080: 3a2f 2f67 6974 6875 622e 636f 6d2f 6e6f  ://github.com/no
+00000090: 6e65 626f 742f 706c 7567 696e 2d61 7073  nebot/plugin-aps
+000000a0: 6368 6564 756c 6572 0a4c 6963 656e 7365  cheduler.License
+000000b0: 3a20 4d49 540a 4175 7468 6f72 3a20 7961  : MIT.Author: ya
+000000c0: 6e79 6f6e 6779 750a 4175 7468 6f72 2d65  nyongyu.Author-e
+000000d0: 6d61 696c 3a20 7979 7940 6e6f 6e65 626f  mail: yyy@nonebo
+000000e0: 742e 6465 760a 5265 7175 6972 6573 2d50  t.dev.Requires-P
+000000f0: 7974 686f 6e3a 203e 3d33 2e38 2c3c 342e  ython: >=3.8,<4.
+00000100: 300a 436c 6173 7369 6669 6572 3a20 4c69  0.Classifier: Li
+00000110: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
+00000120: 726f 7665 6420 3a3a 204d 4954 204c 6963  roved :: MIT Lic
+00000130: 656e 7365 0a43 6c61 7373 6966 6965 723a  ense.Classifier:
+00000140: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+00000150: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000160: 3a3a 2033 0a43 6c61 7373 6966 6965 723a  :: 3.Classifier:
+00000170: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+00000180: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000190: 3a3a 2033 2e38 0a43 6c61 7373 6966 6965  :: 3.8.Classifie
+000001a0: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+000001b0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+000001c0: 6e20 3a3a 2033 2e39 0a43 6c61 7373 6966  n :: 3.9.Classif
+000001d0: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+000001e0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+000001f0: 686f 6e20 3a3a 2033 2e31 300a 436c 6173  hon :: 3.10.Clas
+00000200: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
+00000210: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000220: 5079 7468 6f6e 203a 3a20 332e 3131 0a52  Python :: 3.11.R
+00000230: 6571 7569 7265 732d 4469 7374 3a20 6170  equires-Dist: ap
+00000240: 7363 6865 6475 6c65 7220 283e 3d33 2e37  scheduler (>=3.7
+00000250: 2e30 2c3c 342e 302e 3029 0a52 6571 7569  .0,<4.0.0).Requi
+00000260: 7265 732d 4469 7374 3a20 6e6f 6e65 626f  res-Dist: nonebo
+00000270: 7432 2028 3e3d 322e 302e 302c 3c33 2e30  t2 (>=2.0.0,<3.0
+00000280: 2e30 290a 5072 6f6a 6563 742d 5552 4c3a  .0).Project-URL:
+00000290: 2044 6f63 756d 656e 7461 7469 6f6e 2c20   Documentation, 
+000002a0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000002b0: 6f6d 2f6e 6f6e 6562 6f74 2f70 6c75 6769  om/nonebot/plugi
+000002c0: 6e2d 6170 7363 6865 6475 6c65 7223 7265  n-apscheduler#re
+000002d0: 6164 6d65 0a50 726f 6a65 6374 2d55 524c  adme.Project-URL
+000002e0: 3a20 5265 706f 7369 746f 7279 2c20 6874  : Repository, ht
+000002f0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000300: 2f6e 6f6e 6562 6f74 2f70 6c75 6769 6e2d  /nonebot/plugin-
+00000310: 6170 7363 6865 6475 6c65 720a 4465 7363  apscheduler.Desc
+00000320: 7269 7074 696f 6e2d 436f 6e74 656e 742d  ription-Content-
+00000330: 5479 7065 3a20 7465 7874 2f6d 6172 6b64  Type: text/markd
+00000340: 6f77 6e0a 0a3c 7020 616c 6967 6e3d 2263  own..<p align="c
+00000350: 656e 7465 7222 3e0a 2020 3c61 2068 7265  enter">.  <a hre
+00000360: 663d 2268 7474 7073 3a2f 2f6e 6f6e 6562  f="https://noneb
+00000370: 6f74 2e64 6576 2f22 3e3c 696d 6720 7372  ot.dev/"><img sr
+00000380: 633d 2268 7474 7073 3a2f 2f6e 6f6e 6562  c="https://noneb
+00000390: 6f74 2e64 6576 2f6c 6f67 6f2e 706e 6722  ot.dev/logo.png"
+000003a0: 2077 6964 7468 3d22 3230 3022 2068 6569   width="200" hei
+000003b0: 6768 743d 2232 3030 2220 616c 743d 226e  ght="200" alt="n
+000003c0: 6f6e 6562 6f74 223e 3c2f 613e 0a3c 2f70  onebot"></a>.</p
+000003d0: 3e0a 0a3c 6469 7620 616c 6967 6e3d 2263  >..<div align="c
+000003e0: 656e 7465 7222 3e0a 0a23 204e 6f6e 6542  enter">..# NoneB
+000003f0: 6f74 2050 6c75 6769 6e20 4150 5363 6865  ot Plugin APSche
+00000400: 6475 6c65 720a 0a5f e29c a820 4e6f 6e65  duler.._... None
+00000410: 426f 7420 4150 5363 6865 6475 6c65 7220  Bot APScheduler 
+00000420: e5ae 9ae6 97b6 e4bb bbe5 8aa1 e68f 92e4  ................
+00000430: bbb6 20e2 9ca8 5f0a 0a3c 2f64 6976 3e0a  .. ..._..</div>.
+00000440: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
+00000450: 7222 3e0a 2020 3c61 2068 7265 663d 2268  r">.  <a href="h
+00000460: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
+00000470: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
+00000480: 2f6e 6f6e 6562 6f74 2f70 6c75 6769 6e2d  /nonebot/plugin-
+00000490: 6170 7363 6865 6475 6c65 722f 6d61 7374  apscheduler/mast
+000004a0: 6572 2f4c 4943 454e 5345 223e 0a20 2020  er/LICENSE">.   
+000004b0: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
+000004c0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+000004d0: 6f2f 6769 7468 7562 2f6c 6963 656e 7365  o/github/license
+000004e0: 2f6e 6f6e 6562 6f74 2f70 6c75 6769 6e2d  /nonebot/plugin-
+000004f0: 6170 7363 6865 6475 6c65 722e 7376 6722  apscheduler.svg"
+00000500: 2061 6c74 3d22 6c69 6365 6e73 6522 3e0a   alt="license">.
+00000510: 2020 3c2f 613e 0a20 203c 6120 6872 6566    </a>.  <a href
+00000520: 3d22 6874 7470 733a 2f2f 7079 7069 2e70  ="https://pypi.p
+00000530: 7974 686f 6e2e 6f72 672f 7079 7069 2f6e  ython.org/pypi/n
+00000540: 6f6e 6562 6f74 2d70 6c75 6769 6e2d 6170  onebot-plugin-ap
+00000550: 7363 6865 6475 6c65 7222 3e0a 2020 2020  scheduler">.    
+00000560: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00000570: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000580: 2f70 7970 692f 762f 6e6f 6e65 626f 742d  /pypi/v/nonebot-
+00000590: 706c 7567 696e 2d61 7073 6368 6564 756c  plugin-apschedul
+000005a0: 6572 2e73 7667 2220 616c 743d 2270 7970  er.svg" alt="pyp
+000005b0: 6922 3e0a 2020 3c2f 613e 0a20 203c 696d  i">.  </a>.  <im
+000005c0: 6720 7372 633d 2268 7474 7073 3a2f 2f69  g src="https://i
+000005d0: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
+000005e0: 6467 652f 7079 7468 6f6e 2d33 2e37 2b2d  dge/python-3.7+-
+000005f0: 626c 7565 2e73 7667 2220 616c 743d 2270  blue.svg" alt="p
+00000600: 7974 686f 6e22 3e0a 3c2f 703e 0a0a 2323  ython">.</p>..##
+00000610: 20e4 bdbf e794 a8e6 96b9 e5bc 8f0a 0ae5   ...............
+00000620: 8aa0 e8bd bde6 8f92 e4bb b6e5 908e e4bd  ................
+00000630: bfe7 94a8 2060 7265 7175 6972 6560 20e8  .... `require` .
+00000640: 8eb7 e58f 9620 6073 6368 6564 756c 6572  ..... `scheduler
+00000650: 6020 e5af b9e8 b1a1 efbc 88e8 afb7 e6b3  ` ..............
+00000660: a8e6 848f e68f 92e4 bbb6 e58a a0e8 bdbd  ................
+00000670: e9a1 bae5 ba8f efbc 890a 0a60 6060 7079  ...........```py
+00000680: 7468 6f6e 0a66 726f 6d20 6e6f 6e65 626f  thon.from nonebo
+00000690: 7420 696d 706f 7274 2072 6571 7569 7265  t import require
+000006a0: 0a0a 7265 7175 6972 6528 226e 6f6e 6562  ..require("noneb
+000006b0: 6f74 5f70 6c75 6769 6e5f 6170 7363 6865  ot_plugin_apsche
+000006c0: 6475 6c65 7222 290a 0a66 726f 6d20 6e6f  duler")..from no
+000006d0: 6e65 626f 745f 706c 7567 696e 5f61 7073  nebot_plugin_aps
+000006e0: 6368 6564 756c 6572 2069 6d70 6f72 7420  cheduler import 
+000006f0: 7363 6865 6475 6c65 720a 0a40 7363 6865  scheduler..@sche
+00000700: 6475 6c65 722e 7363 6865 6475 6c65 645f  duler.scheduled_
+00000710: 6a6f 6228 2263 726f 6e22 2c20 686f 7572  job("cron", hour
+00000720: 3d22 2a2f 3222 2c20 6964 3d22 7878 7822  ="*/2", id="xxx"
+00000730: 2c20 6172 6773 3d5b 315d 2c20 6b77 6172  , args=[1], kwar
+00000740: 6773 3d7b 2261 7267 3222 3a20 327d 290a  gs={"arg2": 2}).
+00000750: 6173 796e 6320 6465 6620 7275 6e5f 6576  async def run_ev
+00000760: 6572 795f 325f 686f 7572 2861 7267 312c  ery_2_hour(arg1,
+00000770: 2061 7267 3229 3a0a 2020 2020 7061 7373   arg2):.    pass
+00000780: 0a0a 7363 6865 6475 6c65 722e 6164 645f  ..scheduler.add_
+00000790: 6a6f 6228 7275 6e5f 6576 6572 795f 6461  job(run_every_da
+000007a0: 795f 6672 6f6d 5f70 726f 6772 616d 5f73  y_from_program_s
+000007b0: 7461 7274 2c20 2269 6e74 6572 7661 6c22  tart, "interval"
+000007c0: 2c20 6461 7973 3d31 2c20 6964 3d22 7878  , days=1, id="xx
+000007d0: 7822 290a 6060 600a 0a23 2320 e985 8de7  x").```..## ....
+000007e0: bdae e9a1 b90a 0a23 2323 2061 7073 6368  .......### apsch
+000007f0: 6564 756c 6572 5f61 7574 6f73 7461 7274  eduler_autostart
+00000800: 0a0a e698 afe5 90a6 e887 aae5 8aa8 e590  ................
+00000810: afe5 8aa8 2060 7363 6865 6475 6c65 7260  .... `scheduler`
+00000820: 0a0a 2323 2320 6170 7363 6865 6475 6c65  ..### apschedule
+00000830: 725f 6c6f 675f 6c65 7665 6c0a 0a60 696e  r_log_level..`in
+00000840: 7460 20e7 b1bb e59e 8be6 97a5 e5bf 97e7  t` .............
+00000850: ad89 e7ba a70a 0a2d 2060 5741 524e 494e  .......- `WARNIN
+00000860: 4760 203d 2060 3330 6020 28e9 bb98 e8ae  G` = `30` (.....
+00000870: a429 0a2d 2060 494e 464f 6020 3d20 6032  .).- `INFO` = `2
+00000880: 3060 0a2d 2060 4445 4255 4760 203d 2060  0`.- `DEBUG` = `
+00000890: 3130 6020 28e5 8faa e69c 89e5 9ca8 e5bc  10` (...........
+000008a0: 80e5 90af 206e 6f6e 6562 6f74 20e7 9a84  .... nonebot ...
+000008b0: 2064 6562 7567 20e6 a8a1 e5bc 8fe6 898d   debug .........
+000008c0: e4bc 9ae6 98be e7a4 ba20 6465 6275 6720  ......... debug 
+000008d0: e697 a5e5 bf97 290a 0a23 2323 2061 7073  ......)..### aps
+000008e0: 6368 6564 756c 6572 5f63 6f6e 6669 670a  cheduler_config.
+000008f0: 0a60 6170 7363 6865 6475 6c65 7260 20e7  .`apscheduler` .
+00000900: 9a84 e79b b8e5 85b3 e985 8de7 bdae e380  ................
+00000910: 82e5 8f82 e880 8320 5be9 858d e7bd ae20  ....... [...... 
+00000920: 7363 6865 6475 6c65 725d 2868 7474 7073  scheduler](https
+00000930: 3a2f 2f61 7073 6368 6564 756c 6572 2e72  ://apscheduler.r
+00000940: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
+00000950: 2f6c 6174 6573 742f 7573 6572 6775 6964  /latest/userguid
+00000960: 652e 6874 6d6c 2373 6368 6564 756c 6572  e.html#scheduler
+00000970: 2d63 6f6e 6669 6729 2c20 5be9 858d e7bd  -config), [.....
+00000980: aee5 8f82 e695 b05d 2868 7474 7073 3a2f  .......](https:/
+00000990: 2f61 7073 6368 6564 756c 6572 2e72 6561  /apscheduler.rea
+000009a0: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
+000009b0: 6174 6573 742f 6d6f 6475 6c65 732f 7363  atest/modules/sc
+000009c0: 6865 6475 6c65 7273 2f62 6173 652e 6874  hedulers/base.ht
+000009d0: 6d6c 2361 7073 6368 6564 756c 6572 2e73  ml#apscheduler.s
+000009e0: 6368 6564 756c 6572 732e 6261 7365 2e42  chedulers.base.B
+000009f0: 6173 6553 6368 6564 756c 6572 290a 0ae9  aseScheduler)...
+00000a00: 858d e7bd aee9 9c80 e8a6 81e5 8c85 e590  ................
+00000a10: ab20 6070 7265 6669 783a 2061 7073 6368  . `prefix: apsch
+00000a20: 6564 756c 6572 2e60 0a0a e9bb 98e8 aea4  eduler.`........
+00000a30: e985 8de7 bdae efbc 9a0a 0a60 6060 6a73  ...........```js
+00000a40: 6f6e 0a7b 2022 6170 7363 6865 6475 6c65  on.{ "apschedule
+00000a50: 722e 7469 6d65 7a6f 6e65 223a 2022 4173  r.timezone": "As
+00000a60: 6961 2f53 6861 6e67 6861 6922 207d 0a60  ia/Shanghai" }.`
+00000a70: 6060 0a0a                                ``..
```

