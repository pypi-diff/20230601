# Comparing `tmp/nonebot_plugin_access_control-0.5.0.post1.tar.gz` & `tmp/nonebot_plugin_access_control-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_access_control-0.5.0.post1.tar", max compression
+gzip compressed data, was "nonebot_plugin_access_control-0.5.1.tar", max compression
```

## Comparing `nonebot_plugin_access_control-0.5.0.post1.tar` & `nonebot_plugin_access_control-0.5.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1085 2022-07-09 13:18:24.594000 nonebot_plugin_access_control-0.5.0.post1/LICENSE
--rw-r--r--   0        0        0      955 2023-05-31 16:06:58.132001 nonebot_plugin_access_control-0.5.0.post1/pyproject.toml
--rw-r--r--   0        0        0    18867 2023-05-30 02:55:49.596711 nonebot_plugin_access_control-0.5.0.post1/README.MD
--rw-r--r--   0        0        0     1607 2023-05-31 16:07:52.519324 nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/__init__.py
--rw-r--r--   0        0        0      579 2023-05-30 02:34:22.187998 nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/config.py
--rw-r--r--   0        0        0      248 2023-02-14 09:17:25.623083 nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/errors.py
--rw-r--r--   0        0        0     2363 2023-02-14 08:19:30.714606 nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/event_bus.py
--rw-r--r--   0        0        0    10443 2023-03-13 03:19:06.942840 nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/matchers/__init__.py
--rw-r--r--   0        0        0     1005 2023-02-13 06:25:49.446680 nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/matchers/handle_error.py
--rw-r--r--   0        0        0     3263 2023-02-14 08:59:49.704358 nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/matchers/parser.py
--rw-r--r--   0        0        0     3693 2023-03-13 03:28:05.306313 nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/migrations/875c4dd8c271_.py
--rw-r--r--   0        0        0      172 2023-03-13 03:19:06.944840 nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/models/__init__.py
--rw-r--r--   0        0        0      461 2023-03-13 03:19:06.944840 nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/models/permission.py
--rw-r--r--   0        0        0     1754 2023-03-13 03:19:06.945840 nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/models/rate_limit.py
--rw-r--r--   0        0        0      119 2023-03-13 03:19:06.946840 nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/plugin_data.py
--rw-r--r--   0        0        0      159 2023-02-13 07:58:33.466319 nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/service/__init__.py
--rw-r--r--   0        0        0     8872 2023-05-30 03:15:13.076049 nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/service/base.py
--rw-r--r--   0        0        0        0 2023-02-13 08:30:50.046295 nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/service/impl/__init__.py
--rw-r--r--   0        0        0     8257 2023-03-13 03:19:06.946840 nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/service/impl/permission.py
--rw-r--r--   0        0        0    11920 2023-05-27 05:28:53.341561 nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/service/impl/rate_limit.py
--rw-r--r--   0        0        0       31 2023-02-13 07:07:23.516417 nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/service/interface/__init__.py
--rw-r--r--   0        0        0     2089 2023-05-30 02:47:39.681782 nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/service/interface/base.py
--rw-r--r--   0        0        0     1630 2023-02-14 07:23:00.750461 nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/service/interface/permission.py
--rw-r--r--   0        0        0     1948 2023-05-27 05:06:59.272662 nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/service/interface/rate_limit.py
--rw-r--r--   0        0        0      680 2023-02-13 08:40:31.774931 nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/service/interface/service.py
--rw-r--r--   0        0        0      334 2023-02-13 07:59:53.174308 nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/service/interface/subservice_owner.py
--rw-r--r--   0        0        0      882 2023-02-14 07:23:39.399678 nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/service/methods.py
--rw-r--r--   0        0        0     2392 2023-02-14 07:30:48.027513 nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/service/nonebot.py
--rw-r--r--   0        0        0       36 2023-02-14 06:34:31.631671 nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/service/permission/__init__.py
--rw-r--r--   0        0        0      224 2023-02-14 07:59:38.644831 nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/service/permission/permission.py
--rw-r--r--   0        0        0      907 2023-02-13 07:53:46.438693 nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/service/plugin.py
--rw-r--r--   0        0        0       74 2023-05-27 05:06:59.273662 nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/service/rate_limit/__init__.py
--rw-r--r--   0        0        0      318 2023-02-14 09:29:28.023174 nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/service/rate_limit/rule.py
--rw-r--r--   0        0        0      181 2023-05-27 05:06:59.273662 nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/service/rate_limit/token.py
--rw-r--r--   0        0        0      840 2023-02-13 07:54:44.558096 nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/service/subservice.py
--rw-r--r--   0        0        0     1645 2023-02-14 06:59:06.539473 nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/service/subservice_owner.py
--rw-r--r--   0        0        0       26 2023-02-20 02:15:08.129834 nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/subject/__init__.py
--rw-r--r--   0        0        0      501 2023-03-11 14:39:35.434800 nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/subject/extractor/__init__.py
--rw-r--r--   0        0        0      681 2023-02-20 02:03:55.940528 nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/subject/extractor/base.py
--rw-r--r--   0        0        0     2762 2023-05-31 16:03:44.287570 nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/subject/extractor/union.py
--rw-r--r--   0        0        0        0 2022-12-10 06:08:59.849075 nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/utils/__init__.py
--rw-r--r--   0        0        0      531 2023-03-13 03:19:06.948840 nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/utils/session.py
--rw-r--r--   0        0        0      425 2023-02-20 04:34:52.815055 nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/utils/superuser.py
--rw-r--r--   0        0        0     1015 2022-12-10 06:23:22.420137 nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/utils/tree.py
--rw-r--r--   0        0        0      324 2023-02-20 02:14:18.246077 nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control_onebot/__init__.py
--rw-r--r--   0        0        0        0 2023-02-20 01:49:13.238036 nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control_onebot/subject/__init__.py
--rw-r--r--   0        0        0       88 2023-02-20 02:08:23.170135 nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control_onebot/subject/extractor/__init__.py
--rw-r--r--   0        0        0     2094 2023-05-31 16:13:35.569687 nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control_onebot/subject/extractor/v11.py
--rw-r--r--   0        0        0     3072 2023-05-31 16:13:35.546685 nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control_onebot/subject/extractor/v12.py
--rw-r--r--   0        0        0    19266 1970-01-01 00:00:00.000000 nonebot_plugin_access_control-0.5.0.post1/PKG-INFO
+-rw-r--r--   0        0        0     1085 2022-07-09 13:18:24.594000 nonebot_plugin_access_control-0.5.1/LICENSE
+-rw-r--r--   0        0        0      949 2023-06-01 01:18:33.536786 nonebot_plugin_access_control-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0    18867 2023-05-30 02:55:49.596711 nonebot_plugin_access_control-0.5.1/README.MD
+-rw-r--r--   0        0        0     1633 2023-06-01 01:15:34.961098 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/__init__.py
+-rw-r--r--   0        0        0      579 2023-05-30 02:34:22.187998 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/config.py
+-rw-r--r--   0        0        0      248 2023-02-14 09:17:25.623083 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/errors.py
+-rw-r--r--   0        0        0     2363 2023-02-14 08:19:30.714606 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/event_bus.py
+-rw-r--r--   0        0        0    10794 2023-06-01 01:16:36.463425 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/matchers/__init__.py
+-rw-r--r--   0        0        0     1005 2023-02-13 06:25:49.446680 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/matchers/handle_error.py
+-rw-r--r--   0        0        0     3352 2023-06-01 01:13:05.751049 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/matchers/parser.py
+-rw-r--r--   0        0        0     3693 2023-03-13 03:28:05.306313 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/migrations/875c4dd8c271_.py
+-rw-r--r--   0        0        0      172 2023-03-13 03:19:06.944840 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/models/__init__.py
+-rw-r--r--   0        0        0      461 2023-03-13 03:19:06.944840 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/models/permission.py
+-rw-r--r--   0        0        0     1754 2023-03-13 03:19:06.945840 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/models/rate_limit.py
+-rw-r--r--   0        0        0      119 2023-03-13 03:19:06.946840 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/plugin_data.py
+-rw-r--r--   0        0        0      159 2023-02-13 07:58:33.466319 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/__init__.py
+-rw-r--r--   0        0        0     8872 2023-05-30 03:15:13.076049 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/base.py
+-rw-r--r--   0        0        0        0 2023-02-13 08:30:50.046295 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/impl/__init__.py
+-rw-r--r--   0        0        0     8257 2023-03-13 03:19:06.946840 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/impl/permission.py
+-rw-r--r--   0        0        0    11920 2023-05-27 05:28:53.341561 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/impl/rate_limit.py
+-rw-r--r--   0        0        0       31 2023-02-13 07:07:23.516417 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/interface/__init__.py
+-rw-r--r--   0        0        0     2089 2023-05-30 02:47:39.681782 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/interface/base.py
+-rw-r--r--   0        0        0     1630 2023-02-14 07:23:00.750461 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/interface/permission.py
+-rw-r--r--   0        0        0     1948 2023-05-27 05:06:59.272662 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/interface/rate_limit.py
+-rw-r--r--   0        0        0      680 2023-02-13 08:40:31.774931 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/interface/service.py
+-rw-r--r--   0        0        0      334 2023-02-13 07:59:53.174308 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/interface/subservice_owner.py
+-rw-r--r--   0        0        0      882 2023-02-14 07:23:39.399678 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/methods.py
+-rw-r--r--   0        0        0     2392 2023-02-14 07:30:48.027513 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/nonebot.py
+-rw-r--r--   0        0        0       36 2023-02-14 06:34:31.631671 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/permission/__init__.py
+-rw-r--r--   0        0        0      224 2023-02-14 07:59:38.644831 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/permission/permission.py
+-rw-r--r--   0        0        0      907 2023-02-13 07:53:46.438693 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/plugin.py
+-rw-r--r--   0        0        0       74 2023-05-27 05:06:59.273662 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/rate_limit/__init__.py
+-rw-r--r--   0        0        0      318 2023-02-14 09:29:28.023174 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/rate_limit/rule.py
+-rw-r--r--   0        0        0      181 2023-05-27 05:06:59.273662 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/rate_limit/token.py
+-rw-r--r--   0        0        0      840 2023-02-13 07:54:44.558096 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/subservice.py
+-rw-r--r--   0        0        0     1645 2023-02-14 06:59:06.539473 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/subservice_owner.py
+-rw-r--r--   0        0        0       26 2023-02-20 02:15:08.129834 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/subject/__init__.py
+-rw-r--r--   0        0        0      501 2023-03-11 14:39:35.434800 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/subject/extractor/__init__.py
+-rw-r--r--   0        0        0      681 2023-02-20 02:03:55.940528 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/subject/extractor/base.py
+-rw-r--r--   0        0        0     2954 2023-06-01 01:04:23.797927 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/subject/extractor/union.py
+-rw-r--r--   0        0        0        0 2022-12-10 06:08:59.849075 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/utils/__init__.py
+-rw-r--r--   0        0        0      531 2023-03-13 03:19:06.948840 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/utils/session.py
+-rw-r--r--   0        0        0      425 2023-02-20 04:34:52.815055 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/utils/superuser.py
+-rw-r--r--   0        0        0     1015 2022-12-10 06:23:22.420137 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/utils/tree.py
+-rw-r--r--   0        0        0      324 2023-02-20 02:14:18.246077 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control_onebot/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-20 01:49:13.238036 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control_onebot/subject/__init__.py
+-rw-r--r--   0        0        0       88 2023-02-20 02:08:23.170135 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control_onebot/subject/extractor/__init__.py
+-rw-r--r--   0        0        0     2094 2023-05-31 16:13:35.569687 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control_onebot/subject/extractor/v11.py
+-rw-r--r--   0        0        0     3072 2023-05-31 16:13:35.546685 nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control_onebot/subject/extractor/v12.py
+-rw-r--r--   0        0        0    19260 1970-01-01 00:00:00.000000 nonebot_plugin_access_control-0.5.1/PKG-INFO
```

### Comparing `nonebot_plugin_access_control-0.5.0.post1/LICENSE` & `nonebot_plugin_access_control-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.0.post1/pyproject.toml` & `nonebot_plugin_access_control-0.5.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-access-control"
-version = "0.5.0.post1"
+version = "0.5.1"
 description = ""
 authors = ["ssttkkl <huang.wen.long@hotmail.com>"]
 license = "MIT"
 readme = "README.MD"
 repository = "https://github.com/ssttkkl/nonebot-plugin-access-control"
 packages = [
     { include = "nonebot_plugin_access_control", from = "src" },
```

### Comparing `nonebot_plugin_access_control-0.5.0.post1/README.MD` & `nonebot_plugin_access_control-0.5.1/README.MD`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/__init__.py` & `nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,7 +42,9 @@
             if service.auto_created:
                 for matcher in plugin.matcher:
                     service.patch_matcher(matcher)
                 patched_plugins.append(plugin)
 
         logger.opt(colors=True).success(
             "auto patched plugin(s): " + ', '.join([f'<y>{p.name}</y>' for p in patched_plugins]))
+
+from . import matchers
```

### Comparing `nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/config.py` & `nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/event_bus.py` & `nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/event_bus.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/matchers/__init__.py` & `nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/matchers/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from argparse import Namespace
 from datetime import timedelta
 from io import StringIO
 from typing import Optional, cast
 
 from nonebot import on_shell_command
 from nonebot.exception import ParserExit
-from nonebot.internal.matcher import Matcher
+from nonebot.internal.matcher import Matcher, current_bot, current_event
 from nonebot.permission import SUPERUSER
 from nonebot.typing import T_State
 
 from .handle_error import handle_error
 from .parser import parser
 from ..service import Service, get_service_by_qualified_name
 from ..service.rate_limit import RateLimitRule
+from ..subject import extract_subjects
 from ..utils.tree import get_tree_summary
 
 
 def parse_integer(text: str, full: bool = True) -> int:
     num = 0
     for c in text:
         c_ord = ord(c) - ord('0')
@@ -25,20 +26,20 @@
         else:
             if full:
                 raise ValueError(f'\'{text}\' cannot parse as an integer')
             break
     return num
 
 
-cmd = on_shell_command("ac", parser=parser, permission=SUPERUSER)
+cmd = on_shell_command("ac", parser=parser, permission=SUPERUSER, priority=1)
 
 
 @cmd.handle()
 @handle_error()
-async def _(matcher: Matcher, state: T_State):
+async def ac(matcher: Matcher, state: T_State):
     args = state["_args"]
     if isinstance(args, ParserExit):
         await matcher.finish(args.message)
 
     args = cast(Namespace, args)
     if args.subcommand is None or args.subcommand == 'help':
         await handle_help(matcher)
@@ -59,14 +60,16 @@
         elif args.action == 'ls':
             await handle_limit_ls(matcher, args.subject, args.service)
         elif args.action == 'reset':
             await handle_limit_reset(matcher)
     elif args.subcommand == 'service':
         if args.action == 'ls':
             await handle_service_ls(matcher, args.service)
+    elif args.subcommand == 'subject':
+        await handle_subject(matcher)
 
 
 help_text = """
 /ac help：显示此帮助
 
 /ac permission allow --sbj <主体> --srv <服务>：为主体启用服务
 /ac permission deny --sbj <主体> --srv <服务>：为主体禁用服务
@@ -255,7 +258,14 @@
     for i in range(0, len(summary), 20):
         j = min(i + 20, len(summary))
         with StringIO() as sio:
             for s in summary[i:j]:
                 sio.write(s)
                 sio.write('\n')
             await matcher.send(sio.getvalue().strip())
+
+
+async def handle_subject(matcher: Matcher):
+    bot = current_bot.get()
+    event = current_event.get()
+    sbj = extract_subjects(bot, event)
+    await matcher.send('\n'.join(sbj))
```

### Comparing `nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/matchers/handle_error.py` & `nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/matchers/handle_error.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/matchers/parser.py` & `nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/matchers/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,7 +48,10 @@
 
 # ==== service ====
 service_parser = subparsers.add_parser("service", help="服务")
 service_subparsers = service_parser.add_subparsers(help="操作", dest="action", required=True)
 
 service_ls_parser = service_subparsers.add_parser("ls", help="列出服务与子服务层级")
 service_ls_parser.add_argument("--srv", "--service", help="服务", dest="service")
+
+# ==== subject ====
+subject_parser = subparsers.add_parser("subject", help="主体")
```

### Comparing `nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/migrations/875c4dd8c271_.py` & `nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/migrations/875c4dd8c271_.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/models/rate_limit.py` & `nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/models/rate_limit.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/service/base.py` & `nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/service/impl/permission.py` & `nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/impl/permission.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/service/impl/rate_limit.py` & `nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/impl/rate_limit.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/service/interface/base.py` & `nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/interface/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/service/interface/permission.py` & `nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/interface/permission.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/service/interface/rate_limit.py` & `nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/interface/rate_limit.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/service/interface/service.py` & `nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/interface/service.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/service/methods.py` & `nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/methods.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/service/nonebot.py` & `nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/nonebot.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/service/plugin.py` & `nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/plugin.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/service/subservice.py` & `nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/subservice.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/service/subservice_owner.py` & `nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/service/subservice_owner.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/subject/extractor/base.py` & `nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/subject/extractor/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/subject/extractor/union.py` & `nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/subject/extractor/union.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,24 +42,28 @@
         channel_id = session.id2
         guild_id = session.id3
 
         if user_id is not None:
             if channel_id is not None:
                 if guild_id is not None:
                     li.append(f"{session.platform}:g{guild_id}:c{channel_id}:{user_id}")
-                li.append(f"{session.platform}:c{channel_id}:{user_id}")
+                    li.append(f"{session.platform}:c{channel_id}:{user_id}")
+                else:
+                    li.append(f"{session.platform}:g{channel_id}:{user_id}")
 
             li.append(f"{session.platform}:{user_id}")
             if is_superuser(bot, event):
                 li.append("superuser")
 
         if channel_id is not None:
             if guild_id is not None:
                 li.append(f"{session.platform}:g{guild_id}:c{channel_id}")
-            li.append(f"{session.platform}:c{channel_id}")
+                li.append(f"{session.platform}:c{channel_id}")
+            else:
+                li.append(f"{session.platform}:g{channel_id}")
 
         if guild_id is not None:
             li.append(f"{session.platform}:g{guild_id}")
 
         if user_id is not None and channel_id is None and guild_id is None:
             li.append(f"{session.platform}:private")
```

### Comparing `nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/utils/session.py` & `nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/utils/session.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control/utils/tree.py` & `nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control/utils/tree.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control_onebot/subject/extractor/v11.py` & `nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control_onebot/subject/extractor/v11.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.0.post1/src/nonebot_plugin_access_control_onebot/subject/extractor/v12.py` & `nonebot_plugin_access_control-0.5.1/src/nonebot_plugin_access_control_onebot/subject/extractor/v12.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.5.0.post1/PKG-INFO` & `nonebot_plugin_access_control-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-access-control
-Version: 0.5.0.post1
+Version: 0.5.1
 Summary: 
 Home-page: https://github.com/ssttkkl/nonebot-plugin-access-control
 License: MIT
 Author: ssttkkl
 Author-email: huang.wen.long@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-access-control Version: 0.5.0.post1
+Metadata-Version: 2.1 Name: nonebot-plugin-access-control Version: 0.5.1
 Summary: Home-page: https://github.com/ssttkkl/nonebot-plugin-access-control
 License: MIT Author: ssttkkl Author-email: huang.wen.long@hotmail.com Requires-
 Python: >=3.9,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: nonebot-
 plugin-apscheduler (>=0.2.0,<0.3.0) Requires-Dist: nonebot-plugin-datastore
```

