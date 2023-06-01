# Comparing `tmp/ezcord-0.2.1.tar.gz` & `tmp/ezcord-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezcord-0.2.1.tar", last modified: Fri May 19 12:49:00 2023, max compression
+gzip compressed data, was "ezcord-0.2.2.tar", last modified: Thu Jun  1 16:03:30 2023, max compression
```

## Comparing `ezcord-0.2.1.tar` & `ezcord-0.2.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:49:00.961672 ezcord-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-19 12:48:47.000000 ezcord-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-19 12:48:47.000000 ezcord-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-19 12:49:00.957672 ezcord-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-19 12:48:47.000000 ezcord-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-19 12:48:47.000000 ezcord-0.2.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:49:00.953672 ezcord-0.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-19 12:48:47.000000 ezcord-0.2.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-19 12:48:47.000000 ezcord-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-19 12:48:47.000000 ezcord-0.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 12:49:00.961672 ezcord-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:49:00.953672 ezcord-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:49:00.957672 ezcord-0.2.1/src/ezcord/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-19 12:48:47.000000 ezcord-0.2.1/src/ezcord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10427 2023-05-19 12:48:47.000000 ezcord-0.2.1/src/ezcord/bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-05-19 12:48:47.000000 ezcord-0.2.1/src/ezcord/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-05-19 12:48:47.000000 ezcord-0.2.1/src/ezcord/emb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-19 12:48:47.000000 ezcord-0.2.1/src/ezcord/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:49:00.957672 ezcord-0.2.1/src/ezcord/internal/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-19 12:48:47.000000 ezcord-0.2.1/src/ezcord/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-19 12:48:47.000000 ezcord-0.2.1/src/ezcord/internal/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-05-19 12:48:47.000000 ezcord-0.2.1/src/ezcord/internal/embed_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-19 12:48:47.000000 ezcord-0.2.1/src/ezcord/internal/funcutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:49:00.957672 ezcord-0.2.1/src/ezcord/internal/language/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-19 12:48:47.000000 ezcord-0.2.1/src/ezcord/internal/language/de.json
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-19 12:48:47.000000 ezcord-0.2.1/src/ezcord/internal/language/en.json
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-19 12:48:47.000000 ezcord-0.2.1/src/ezcord/internal/language/languages.py
--rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-05-19 12:48:47.000000 ezcord-0.2.1/src/ezcord/internal/ready_style.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-05-19 12:48:47.000000 ezcord-0.2.1/src/ezcord/internal/translation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9736 2023-05-19 12:48:47.000000 ezcord-0.2.1/src/ezcord/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-05-19 12:48:47.000000 ezcord-0.2.1/src/ezcord/times.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-19 12:48:47.000000 ezcord-0.2.1/src/ezcord/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:49:00.957672 ezcord-0.2.1/src/ezcord.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-19 12:49:00.000000 ezcord-0.2.1/src/ezcord.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-19 12:49:00.000000 ezcord-0.2.1/src/ezcord.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 12:49:00.000000 ezcord-0.2.1/src/ezcord.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-19 12:49:00.000000 ezcord-0.2.1/src/ezcord.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-19 12:49:00.000000 ezcord-0.2.1/src/ezcord.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:03:30.886761 ezcord-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-01 16:03:19.000000 ezcord-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-01 16:03:19.000000 ezcord-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-01 16:03:30.886761 ezcord-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-01 16:03:19.000000 ezcord-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-01 16:03:19.000000 ezcord-0.2.2/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:03:30.882761 ezcord-0.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-01 16:03:19.000000 ezcord-0.2.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-01 16:03:19.000000 ezcord-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-01 16:03:19.000000 ezcord-0.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 16:03:30.886761 ezcord-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:03:30.878760 ezcord-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:03:30.882761 ezcord-0.2.2/src/ezcord/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-01 16:03:19.000000 ezcord-0.2.2/src/ezcord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13087 2023-06-01 16:03:19.000000 ezcord-0.2.2/src/ezcord/bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-06-01 16:03:19.000000 ezcord-0.2.2/src/ezcord/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11006 2023-06-01 16:03:19.000000 ezcord-0.2.2/src/ezcord/emb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-01 16:03:19.000000 ezcord-0.2.2/src/ezcord/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:03:30.882761 ezcord-0.2.2/src/ezcord/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-01 16:03:19.000000 ezcord-0.2.2/src/ezcord/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-06-01 16:03:19.000000 ezcord-0.2.2/src/ezcord/internal/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-06-01 16:03:19.000000 ezcord-0.2.2/src/ezcord/internal/embed_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-01 16:03:19.000000 ezcord-0.2.2/src/ezcord/internal/funcutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:03:30.886761 ezcord-0.2.2/src/ezcord/internal/language/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-01 16:03:19.000000 ezcord-0.2.2/src/ezcord/internal/language/de.json
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-01 16:03:19.000000 ezcord-0.2.2/src/ezcord/internal/language/en.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-01 16:03:19.000000 ezcord-0.2.2/src/ezcord/internal/language/languages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-06-01 16:03:19.000000 ezcord-0.2.2/src/ezcord/internal/ready_style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-06-01 16:03:19.000000 ezcord-0.2.2/src/ezcord/internal/translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11487 2023-06-01 16:03:19.000000 ezcord-0.2.2/src/ezcord/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-06-01 16:03:19.000000 ezcord-0.2.2/src/ezcord/times.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-01 16:03:19.000000 ezcord-0.2.2/src/ezcord/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:03:30.882761 ezcord-0.2.2/src/ezcord.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-01 16:03:30.000000 ezcord-0.2.2/src/ezcord.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-01 16:03:30.000000 ezcord-0.2.2/src/ezcord.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 16:03:30.000000 ezcord-0.2.2/src/ezcord.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-01 16:03:30.000000 ezcord-0.2.2/src/ezcord.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-01 16:03:30.000000 ezcord-0.2.2/src/ezcord.egg-info/top_level.txt
```

### Comparing `ezcord-0.2.1/LICENSE` & `ezcord-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ezcord-0.2.1/PKG-INFO` & `ezcord-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezcord
-Version: 0.2.1
+Version: 0.2.2
 Summary: An easy-to-use extension for the Pycord library
 Author: tibue99
 License: MIT
 Project-URL: GitHub, https://github.com/tibue99/ezcord
 Project-URL: Documentation, https://ezcord.readthedocs.io
 Keywords: discord,pycord,py-cord
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ezcord-0.2.1/README.md` & `ezcord-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `ezcord-0.2.1/pyproject.toml` & `ezcord-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ezcord-0.2.1/src/ezcord/bot.py` & `ezcord-0.2.2/src/ezcord/bot.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from __future__ import annotations
 
 import logging
 import os
-import warnings
 from pathlib import Path
 from typing import Any
 
 import aiohttp
 import discord
 from discord.ext import bridge, commands
 
 from .emb import error as error_emb
-from .enums import ReadyEvent
+from .enums import CogLog, ReadyEvent
 from .logs import DEFAULT_LOG, custom_log, set_log
 from .times import dc_timestamp
 
 from .internal import (  # isort: skip
     READY_TITLE,
     load_lang,
     print_custom_ready,
@@ -42,15 +41,16 @@
         Enable log messages. Defaults to ``True``.
     error_handler:
         Enable the error handler. Defaults to ``True``.
     error_webhook_url:
         The webhook URL to send error messages to. Defaults to ``None``.
 
         .. note::
-            You need to enable the error handler for the webhook to work.
+            You can disable the default error handler, but still provide an error webhook URL.
+            This will send an error report to the webhook, but it won't send an error message to the user.
     ignored_errors:
         A list of error types to ignore. Defaults to ``None``.
     full_error_traceback:
         Whether to send the full error traceback. If this is ``False``,
         only the most recent traceback will be sent. Defaults to ``False``.
     language:
         The language to use for user output.
@@ -75,102 +75,167 @@
         full_error_traceback: bool = False,
         language: str = "en",
         ready_event: ReadyEvent | None = ReadyEvent.default,
         **kwargs,
     ):
         super().__init__(intents=intents, **kwargs)
 
-        if error_handler and error_webhook_url:
+        if error_webhook_url:
             os.environ.setdefault("ERROR_WEBHOOK_URL", error_webhook_url)
 
         if debug:
             self.logger = set_log(DEFAULT_LOG)
         else:
             self.logger = logging.getLogger(DEFAULT_LOG)
             self.logger.addHandler(logging.NullHandler())
 
+        self.error_handler = error_handler
         self.error_webhook_url = error_webhook_url
         self.ignored_errors = ignored_errors or []
         self.full_error_traceback = full_error_traceback
         load_lang(language)
         set_lang(language) if language != {} else set_lang("en")
 
-        if error_handler:
+        if error_handler or error_webhook_url:
             self.add_listener(self._error_event, "on_application_command_error")
-        elif error_webhook_url:
-            warnings.warn("You need to enable the error handler for the webhook to work.")
 
         self.ready_event = ready_event
         if ready_event:
             self.add_listener(self._ready_event, "on_ready")
 
-    def _cog_log(self, name: str, custom_logs: bool | str):
+    def _send_cog_log(
+        self,
+        custom_log_level: str | None,
+        log_format: str,
+        color: str | None,
+    ):
+        if custom_log_level:
+            custom_log(custom_log_level, log_format, color=color, level=logging.INFO)
+        else:
+            self.logger.info(log_format)
+
+    def _cog_log(
+        self,
+        cog_name: str,
+        custom_log_level: str | None,
+        log_format: CogLog | str | None,
+        directory: str,
+        color: str | None = None,
+        subdir: bool = False,
+    ):
         """Sends a log message for a loaded cog."""
-        if custom_logs:
-            custom_log("COG", f"Loaded {name}", color=custom_logs, level=logging.INFO)
+
+        if not log_format or "{sum}" in log_format:
+            return
+
+        log_format = log_format.replace("{cog}", cog_name)
+        log_format = log_format.replace("{path}", f"{directory}.{cog_name}" if subdir else cog_name)
+        log_format = log_format.replace("{directory}", f"{directory}")
+
+        self._send_cog_log(custom_log_level, log_format, color=color)
+
+    def _cog_count_log(
+        self,
+        custom_log_level: str | None,
+        log_format: CogLog | str | None,
+        count: int,
+        color: str | None = None,
+        directory: str | None = None,
+    ):
+        """Sends a log message for the number of loaded cogs in a directory or in total."""
+
+        if not log_format or "{cog}" in log_format or "{path}" in log_format:
+            return
+        if directory and "{directory}" not in log_format:
+            return
+        if count == 0:
+            return
+        if count == 1:
+            log_format = log_format.replace("cogs", "cog")
+
+        if directory and "{sum}" in log_format and "{directory}" in log_format:
+            log_format = log_format.replace("{sum}", str(count))
+            log_format = log_format.replace("{directory}", directory)
+        elif not directory and "{sum}" in log_format and "{directory}" not in log_format:
+            log_format = log_format.replace("{sum}", str(count))
         else:
-            self.logger.info(f"Loaded {name}")
+            return
+
+        self._send_cog_log(custom_log_level, log_format, color=color)
 
     def load_cogs(
         self,
         *directories: str,
         subdirectories: bool = False,
         ignored_cogs: list[str] | None = None,
-        log: bool = True,
-        custom_logs: bool | str = True,
-        log_directories: bool = False,
+        log: CogLog | str | None = CogLog.default,
+        custom_log_level: str | None = "COG",
+        log_color: str | None = None,
     ):
         """Load all cogs in the given directories.
 
         Parameters
         ----------
         *directories:
             Names of the directories to load cogs from.
             Defaults to ``"cogs"``.
         subdirectories:
             Whether to load cogs from subdirectories.
             Defaults to ``False``.
         ignored_cogs:
             A list of cogs to ignore. Defaults to ``None``.
         log:
-            Whether to log the loaded cogs. Defaults to ``True``.
-        custom_logs:
-            Whether to use a custom log format for cogs. Defaults to ``True``.
-            You can also pass in a custom color.
-        log_directories:
-            Whether to include the directory name in log messages. Defaults to ``False``.
+            The log format for cogs. Defaults to :attr:`.CogLog.default`.
+            If this is ``None``, logs will be disabled.
+        custom_log_level:
+            The name of the custom log level for cogs. Defaults to ``COG``.
+        log_color:
+            The color to use for cog logs. This will only have an effect if ``custom_log_level`` is enabled.
+            If this is ``None``, a default color will be used.
         """
         ignored_cogs = ignored_cogs or []
         if not directories:
             directories = ("cogs",)
 
+        loaded_cogs = 0
         for directory in directories:
             path = Path(directory)
 
+            loaded_root_cogs = 0
             for filename in os.listdir(directory):
                 name = filename[:-3]
                 if filename.endswith(".py") and name not in ignored_cogs:
                     self.load_extension(f"{'.'.join(path.parts)}.{name}")
-                    if not log:
-                        continue
-                    self._cog_log(f"{name}", custom_logs)
+                    loaded_root_cogs += 1
+                    self._cog_log(f"{name}", custom_log_level, log, directory, log_color)
+
+            loaded_cogs += loaded_root_cogs
+            self._cog_count_log(custom_log_level, log, loaded_root_cogs, log_color, directory)
 
             if subdirectories:
                 for element in os.scandir(directory):
                     if not element.is_dir():
                         continue
 
+                    loaded_dir_cogs = 0
+                    dirname = element.name
+
                     for sub_file in os.scandir(element.path):
                         name = sub_file.name[:-3]
                         if sub_file.name.endswith(".py") and name not in ignored_cogs:
-                            self.load_extension(f"{'.'.join(path.parts)}.{element.name}.{name}")
-                            dirname = f"{element.name}." if log_directories else ""
-                            if not log:
-                                continue
-                            self._cog_log(f"{dirname}{name}", custom_logs)
+                            self.load_extension(f"{'.'.join(path.parts)}.{dirname}.{name}")
+                            loaded_dir_cogs += 1
+                            self._cog_log(
+                                f"{name}", custom_log_level, log, dirname, log_color, subdir=True
+                            )
+
+                    self._cog_count_log(custom_log_level, log, loaded_dir_cogs, log_color, dirname)
+                    loaded_cogs += loaded_dir_cogs
+
+        self._cog_count_log(custom_log_level, log, loaded_cogs, log_color)
 
     def ready(
         self,
         *,
         title: str = READY_TITLE,
         style: ReadyEvent = ReadyEvent.default,
         default_info: bool = True,
@@ -204,36 +269,40 @@
 
     async def _error_event(self, ctx: discord.ApplicationContext, error: discord.DiscordException):
         """The event that handles application command errors."""
         if type(error) in self.ignored_errors:
             return
 
         if isinstance(error, commands.CommandOnCooldown):
-            seconds = round(ctx.command.get_cooldown_retry_after(ctx))
-            cooldown_txt = t("cooldown", dc_timestamp(seconds))
-            await error_emb(ctx, cooldown_txt, title="Cooldown")
+            if self.error_handler:
+                seconds = round(ctx.command.get_cooldown_retry_after(ctx))
+                cooldown_txt = t("cooldown", dc_timestamp(seconds))
+                await error_emb(ctx, cooldown_txt, title=t("cooldown_title"))
 
         elif isinstance(error, commands.BotMissingPermissions):
-            perms = "\n".join(error.missing_permissions)
-            perm_txt = f"{t('no_perm_desc')} ```\n{perms}```"
-            await error_emb(ctx, perm_txt, title=t("no_perm_title"))
+            if self.error_handler:
+                perms = "\n".join(error.missing_permissions)
+                perm_txt = f"{t('no_perms')} ```\n{perms}```"
+                await error_emb(ctx, perm_txt, title=t("no_perms_title"))
 
         else:
             if "original" in error.__dict__ and not self.full_error_traceback:
                 original_error = error.__dict__["original"]
                 error_msg = f"{original_error.__class__.__name__}: {error.__cause__}"
                 error = original_error
             else:
                 error_msg = f"{error}"
 
-            error_txt = f"{t('error', f'```{error_msg}```')}"
-            try:
-                await error_emb(ctx, error_txt, title="Error")
-            except discord.HTTPException:
-                pass
+            if self.error_handler:
+                error_txt = f"{t('error', f'```{error_msg}```')}"
+                try:
+                    await error_emb(ctx, error_txt, title=t("error_title"))
+                except discord.HTTPException:
+                    # invalid interaction, probably took too long to respond
+                    pass
 
             webhook_sent = False
             if self.error_webhook_url:
                 description = get_error_text(ctx, error)
                 webhook_sent = await self._send_error_webhook(description)
 
             self.logger.exception(
```

### Comparing `ezcord-0.2.1/src/ezcord/components.py` & `ezcord-0.2.2/src/ezcord/components.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
         super().__init__(*args, **kwargs)
 
     async def on_error(
         self, error: Exception, item: discord.ui.Item, interaction: discord.Interaction
     ) -> None:
         """Sends an error message to a webhook, if the URL was passed in :class:`.Bot`.
 
-        Executes all registered error handlers with the ``@on_view_error`` decorator.
+        Executes all registered error handlers with the ``@ezcord.event`` decorator.
         """
 
         description = get_error_text(interaction, error, item)
         webhook_sent = await _send_error_webhook(interaction, description)
 
         log.exception(
             f"Error in View **{type(item.view).__name__}**",
@@ -150,15 +150,15 @@
         """Returns ``True`` if all custom checks return ``True`` or if no custom checks are registered."""
         for coro in _view_checks:
             if not await coro(interaction):
                 return False
         return True
 
     async def on_check_failure(self, interaction: discord.Interaction) -> None:
-        """This method is called if :meth:`interaction_check` returns ``False``"""
+        """This method is called if :meth:`interaction_check` returns ``False``."""
         for coro in _view_check_failures:
             await coro(interaction)
 
     async def on_timeout(self) -> None:
         """Makes sure that items are only disabled if the message still has components.
 
         This is called when ``disable_on_timeout`` is set to ``True``.
@@ -182,15 +182,15 @@
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     async def on_error(self, error: Exception, interaction: discord.Interaction) -> None:
         """Sends an error message to a webhook, if the webhook URL was passed into :class:`.Bot`.
 
-        Executes all registered error handlers with the ``@on_modal_error`` decorator.
+        Executes all registered error handlers with the ``@ezcord.event`` decorator.
         """
 
         description = get_error_text(interaction, error, self)
         webhook_sent = await _send_error_webhook(interaction, description)
 
         log.exception(
             f"Error in Modal **{type(self).__name__}**",
```

### Comparing `ezcord-0.2.1/src/ezcord/internal/colors.py` & `ezcord-0.2.2/src/ezcord/internal/colors.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     logging.INFO: Fore.CYAN,
     logging.WARNING: Fore.YELLOW,
     logging.ERROR: Fore.RED,
     logging.CRITICAL: Fore.RED,
 }
 
 
-def get_escape_code(color_string: str | bool) -> str:
+def get_escape_code(color_string: str | None) -> str:
     """Converts a color string to an ansi escape code using colorama.
 
     If the string already is an escape code, it will be returned.
     """
     if not isinstance(color_string, str):
         return DEFAULT_COLOR
 
@@ -62,9 +62,10 @@
 
     if file:
         string = string.replace("***", "").replace("**", "")
         string = remove_escapes(string)
     else:
         string = replace_second(string, "***", color)  # text that contains multiple other colors
         string = replace_second(string, "**", color)
-    string = re.sub("```.*?```", "", string)  # remove codeblocks
+
+    string = re.sub("```.*?```", "", string, flags=re.DOTALL)  # remove codeblocks
     return string
```

### Comparing `ezcord-0.2.1/src/ezcord/internal/embed_templates.py` & `ezcord-0.2.2/src/ezcord/internal/embed_templates.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import json
 import os
 import traceback
 from functools import cache
 from pathlib import Path
 
 import discord
@@ -11,44 +13,49 @@
     "success_embed": Embed(color=Color.green()),
     "error_embed": Embed(color=Color.red()),
     "warn_embed": Embed(color=Color.gold()),
     "info_embed": Embed(color=Color.blue()),
 }
 
 
-def save_embeds(**kwargs: Embed):
+def save_embeds(**kwargs: Embed | str):
     """Save multiple embeds to a JSON file.
 
     If one of the default values is not included, a default template will be saved.
     """
     embeds = {}
     overrides = _TEMPLATES if len(kwargs) == 0 else kwargs
 
     for name, embed in overrides.items():
         if embed is None:
             embeds[name] = _TEMPLATES[name].to_dict()
+        elif isinstance(embed, str):
+            embeds[name] = embed
         else:
             embeds[name] = embed.to_dict()
 
     parent = Path(__file__).parent.absolute()
     with open(os.path.join(parent, "embeds.json"), "w") as file:
         json.dump(embeds, file, indent=2)
 
 
 @cache
-def load_embed(name: str) -> Embed:
+def load_embed(name: str) -> Embed | str:
     """Load an embed template from a JSON file."""
     parent = Path(__file__).parent.absolute()
     json_path = parent.joinpath("embeds.json")
     if not json_path.exists():
         save_embeds()
 
     with open(os.path.join(parent, "embeds.json")) as file:
         embeds = json.load(file)
 
+    if isinstance(embeds[name], str):
+        return embeds[name]
+
     try:
         return Embed.from_dict(embeds[name])
     except KeyError:
         if name in _TEMPLATES.keys():
             save_embeds()
             return load_embed()
         else:
@@ -56,14 +63,15 @@
 
 
 def get_error_text(
     ctx: discord.ApplicationContext | discord.Interaction,
     error: Exception,
     item: discord.ui.Item | discord.ui.Modal | None = None,
 ):
+    """Get the description for the webhook embed."""
     if item:
         if isinstance(item, discord.ui.Button) and item.label:
             location = f"- **Button:** {item.label}"
         elif ctx.type == discord.InteractionType.modal_submit:
             location = f"- **Modal:** {type(item).__name__}"
         else:
             location = f"- **Select Menu:** {type(item.view).__name__}"
```

### Comparing `ezcord-0.2.1/src/ezcord/internal/language/languages.py` & `ezcord-0.2.2/src/ezcord/internal/language/languages.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.2.1/src/ezcord/internal/ready_style.py` & `ezcord-0.2.2/src/ezcord/internal/ready_style.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Utility functions for the ready event."""
 
+from __future__ import annotations
+
 from itertools import cycle, islice
 
 import discord
 from colorama import Fore
 
 from .. import __version__
 from ..enums import ReadyEvent
@@ -59,15 +61,15 @@
     colors: list[str] | None = None,
 ):
     infos = get_default_info(bot) if default_info else {}
     colors = list(map(get_escape_code, colors or DEFAULT_COLORS))
 
     if new_info:
         for key, value in new_info.items():
-            infos[key] = value
+            infos[str(key)] = str(value)
 
     print_ready(bot, style, infos, title, colors)
 
 
 def print_ready(
     bot: discord.Bot,
     style: ReadyEvent,
```

### Comparing `ezcord-0.2.1/src/ezcord/internal/translation.py` & `ezcord-0.2.2/src/ezcord/internal/translation.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,15 +100,18 @@
     while origin_file == Path(__file__).stem:
         n += 1
         origin_file = Path(inspect.stack()[n].filename).stem
 
     lang = get_lang()
 
     try:
-        return load_lang(lang)[origin_file][key].format(*args)
+        string = load_lang(lang)[origin_file][key]
+        if not string:
+            return None
+        return string.format(*args)
     except KeyError:
         # fallback to english if the key is not in the custom language file
         # provided by the user
         log.warn(f"Key '{key}' not found in language file '{lang}'. Falling back to 'en'.")
         return load_lang("en")[origin_file][key].format(*args)
```

### Comparing `ezcord-0.2.1/src/ezcord/logs.py` & `ezcord-0.2.2/src/ezcord/logs.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 """Some logging utilities that are used for bot logs."""
 
 from __future__ import annotations
 
 import asyncio
 import logging
 import os
+import re
 import sys
+from typing import Literal
 
 import aiohttp
 import discord
 from colorama import Fore
 
-from .enums import LogFormat
+from .enums import LogFormat, TimeFormat
 
 from .internal.colors import (  # isort: skip
     DEFAULT_COLOR,
     DEFAULT_LOG_COLORS,
     get_escape_code,
     replace_dc_format,
 )
 
 DEFAULT_LOG = "ezcord"
 log = logging.getLogger(DEFAULT_LOG)
 
 
 def custom_log(
-    key: str, message: str, *, color: str | bool = DEFAULT_COLOR, level: int = logging.INFO
+    key: str, message: str, *, color: str | None = DEFAULT_COLOR, level: int = logging.INFO
 ):
     """Log a message with a custom log level.
 
     Parameters
     ----------
     key:
         The name of the custom log level.
@@ -42,23 +44,39 @@
     """
     color = get_escape_code(color)
     logging.getLogger(DEFAULT_LOG).log(level, message, extra={"key": key, "color": color})
 
 
 def _format_log_colors(log_format: str, file: bool, final_colors: dict[int, str]) -> dict[int, str]:
     """Checks if the is sent to a file and formats the colors accordingly."""
+    format_colors = re.findall(r"{.*?}", log_format)
+
+    remove_attrs = ["{color}"]
+    for attr in remove_attrs:
+        format_colors = [x for x in format_colors if attr not in x]
+
     color_formats = {}
-    if "{color}" in log_format and "{color_end}" in log_format:
+    if "{end}" in log_format:
         for level in final_colors:
             if file:
-                color_formats[level] = log_format.format(color="", color_end="")
+                for substring in format_colors:
+                    log_format = log_format.replace(substring, "")
+
+                color_formats[level] = log_format.format(color="", end="")
             else:
-                color_formats[level] = log_format.format(
-                    color=final_colors[level], color_end=Fore.RESET
-                )
+                for substring in format_colors:
+                    if substring == "{end}":
+                        log_format = log_format.replace(substring, Fore.RESET, 1)
+                        continue
+
+                    log_format = log_format.replace(
+                        substring, get_escape_code(substring.strip("{}"))
+                    )
+
+                color_formats[level] = log_format.format(color=final_colors[level], end=Fore.RESET)
     else:
         for level in final_colors:
             color_formats[level] = final_colors[level] + log_format + Fore.RESET
 
     return color_formats
 
 
@@ -77,43 +95,35 @@
         for level in colors:
             final_colors[level] = get_escape_code(colors[level])
 
     return final_colors
 
 
 class _ColorFormatter(logging.Formatter):
-    """A logging formatter that adds colors to the output. This is used by :func:`set_log`.
-
-    Parameters
-    ----------
-    file:
-        Whether to log to a file.
-    log_format:
-        The log format.
-    time_format:
-        The time format.
-    colors:
-        Colors for the log levels.
-    """
+    """A logging formatter that adds colors to the output. This is used by :func:`set_log`."""
 
     def __init__(
         self,
         file: bool,
         log_format: str,
         time_format: str,
         dc_codeblocks: bool,
+        spacing: int,
+        space_after_level: bool,
         colors: dict[int, str] | str | None = None,
         *args,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
 
         self.file = file
         self.colors = colors
         self.dc_codeblocks = dc_codeblocks
+        self.spacing = spacing
+        self.space_after_level = space_after_level
         self.LOG_FORMAT = log_format
         self.TIME_FORMAT = time_format
 
     def format(self, record: logging.LogRecord):
         """Adds colors to log messages and formats them accordingly.
         Can be used with :func:`set_log`.
 
@@ -136,16 +146,27 @@
             else:
                 # if no color is set for a custom log level used by .log()
                 color_formats[record.levelno] = DEFAULT_COLOR
 
         color_log_formats = _format_log_colors(self.LOG_FORMAT, self.file, color_formats)
 
         log_format = color_log_formats.get(record.levelno)
+        spacing_name = record.__dict__["key"] if "key" in record.__dict__ else record.levelname
+        spaces = " " * (self.spacing - len(spacing_name))
+
+        if self.space_after_level:
+            # add space directly after log level
+            spacing_name = spacing_name + spaces
+            record.levelname = spacing_name
+        else:
+            # add space in front of log message
+            record.msg = spaces + record.msg
+
         if "key" in record.__dict__ and log_format:
-            log_format = log_format.replace("%(levelname)s", record.__dict__["key"])
+            log_format = log_format.replace("%(levelname)s", spacing_name)
 
         current_level_color = color_formats.get(record.levelno)
         new_record = logging.makeLogRecord(record.__dict__)
 
         # color new lines
         if isinstance(log_format, str) and log_format.endswith("//"):
             log_format = log_format.replace("//", "")
@@ -218,43 +239,52 @@
 
 def set_log(
     name: str = DEFAULT_LOG,
     log_level: int = logging.INFO,
     *,
     file: bool = False,
     log_format: str | LogFormat = LogFormat.default,
-    time_format: str = "%Y-%m-%d %H:%M:%S",
+    time_format: str | TimeFormat = TimeFormat.default,
     discord_log_level: int = logging.WARNING,
     webhook_url: str | None = None,
     dc_codeblocks: bool = True,
+    level_spacing: int = 8,
+    space_mode: Literal["auto", "always", "never"] = "auto",
     colors: dict[int, str] | str | None = None,
 ):
     """Creates a logger. If this logger already exists, it will return the existing logger.
 
+    This should be called before :class:`.Bot` is initialized.
+
     Parameters
     ----------
     name:
         The name of the logger.
     log_level:
         The log level for default log messages ``logging.INFO``.
     file:
         Whether to log to a file. Defaults to ``False``.
     log_format:
         The log format. Defaults to :attr:`.LogFormat.default`.
     time_format:
-        The time format. Defaults to ``%Y-%m-%d %H:%M:%S``.
+        The time format. Defaults to :attr:`.TimeFormat.default`.
     discord_log_level:
         The log level for discord log messages. Defaults to ``logging.WARNING``.
 
         .. note::
             For discord log messages, ``webhook_url`` is required.
     webhook_url:
         The discord webhook URL to send logs to. Defaults to ``None``.
     dc_codeblocks:
         Whether to use codeblocks for all Discord log messages. Defaults to ``True``.
+    level_spacing:
+        The length of the log level. If the log level is ``INFO`` and the spacing is ``8``, the log
+        level will be filled with 4 additional spaces, so that all log levels are 8 characters long.
+    space_mode:
+        Choose when to add spacing to the log level. Defaults to ``auto``.
     colors:
         A dictionary of log levels and their corresponding colors. If only one color is given,
         all log levels will be colored with that color.
 
         Example
         -------
         .. code-block:: python
@@ -284,15 +314,23 @@
         if not os.path.exists("logs"):
             os.mkdir("logs")
         filename = name.split(".")[-1]
         handler = logging.FileHandler(f"logs/{filename}.log", mode="w", encoding="utf-8")
     else:
         handler = logging.StreamHandler(sys.stdout)
 
-    color_formatter = _ColorFormatter(file, log_format, time_format, dc_codeblocks, colors)
+    space_after_level = True
+    if "%(levelname)s " not in log_format and "%(levelname)s{end} " not in log_format:
+        space_after_level = False
+        if space_mode == "never" or space_mode == "auto":
+            level_spacing = 0
+
+    color_formatter = _ColorFormatter(
+        file, log_format, time_format, dc_codeblocks, level_spacing, space_after_level, colors
+    )
 
     handler.setFormatter(color_formatter)
     handler.setLevel(log_level)
     logger.addHandler(handler)
 
     dc_format = "**%(levelname)s:** %(message)s"
     discord_handler = _DiscordHandler(webhook_url, dc_codeblocks, dc_format)
```

### Comparing `ezcord-0.2.1/src/ezcord/times.py` & `ezcord-0.2.2/src/ezcord/times.py`

 * *Files 24% similar despite different names*

```diff
@@ -27,21 +27,26 @@
 def convert_time(seconds: int | float, relative: bool = True) -> str:
     """Convert seconds to a human-readable time.
 
     Parameters
     ----------
     seconds:
         The amount of seconds to convert.
-    relative: :class:`bool`
+    relative:
         Whether to use relative time. Defaults to ``True``.
 
         .. hint::
             This is only needed for German translation and will
             not have any effect if the language is set to English.
 
+            >>> convert_time(450000, relative=True)  # Relative: Seit 5 Tagen
+            '5 Tagen'
+            >>> convert_time(450000, relative=False)  # Not relative: 5 Tage
+            '5 Tage'
+
     Returns
     -------
     :class:`str`
         A human-readable time.
     """
     if seconds < 60:
         return f"{round(seconds)} {tp('sec', round(seconds))}"
@@ -60,15 +65,15 @@
 
     This function calls :func:`convert_time`.
 
     Parameters
     ----------
     dt:
         The datetime or timedelta object to convert.
-    relative: :class:`bool`
+    relative:
         Whether to use relative time. Defaults to ``True``.
 
     Returns
     -------
     :class:`str`
         A human-readable time.
     """
@@ -97,29 +102,43 @@
     :class:`str`
         A Discord timestamp.
     """
     dt = utcnow() + timedelta(seconds=seconds)
     return format_dt(dt, style)
 
 
-def convert_to_seconds(s: str) -> int:
-    """Convert a string to seconds.
+def convert_to_seconds(string: str) -> int:
+    """Convert a string to seconds. Supports multiple units and decimal separators.
 
     Parameters
     ----------
-    s:
+    string:
         The string to convert.
 
+    Example
+    -------
+    >>> convert_to_seconds("1m 9s")
+    69
+    >>> convert_to_seconds("1.5m")
+    90
+    >>> convert_to_seconds("1,5 min")
+    90
+    >>> convert_to_seconds("1h 5m 10s")
+    3910
+
     Returns
     -------
     :class:`int`
         The amount of seconds.
     """
-    units = {"s": "seconds", "m": "minutes", "h": "hours", "d": "days", "w": "weeks"}
-    return int(
-        timedelta(
-            **{
-                units.get(m.group("unit").lower(), "seconds"): float(m.group("val"))
-                for m in re.finditer(r"(?P<val>\d+(\.\d+)?)(?P<unit>[smhdw]?)", s, flags=re.I)
-            }
-        ).total_seconds()
-    )
+    units = {"s": "seconds", "m": "minutes", "h": "hours", "d": "days", "t": "days", "w": "weeks"}
+
+    pattern = re.compile(r"(?P<value>\d+([.,]\d+)?) *(?P<unit>[smhdtw]?)", flags=re.IGNORECASE)
+    matches = pattern.finditer(string)
+
+    found_units = {}
+    for match in matches:
+        unit = match.group("unit").lower()
+        value = float(match.group("value").replace(",", "."))
+        found_units[units.get(unit, "seconds")] = value
+
+    return int(timedelta(**found_units).total_seconds())
```

### Comparing `ezcord-0.2.1/src/ezcord/utils.py` & `ezcord-0.2.2/src/ezcord/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,31 +2,35 @@
 
 import io
 import json
 
 import discord
 
 
-def create_json_file(dictionary: dict, filename: str = "data.json", **kwargs) -> discord.File:
+def create_json_file(
+    dictionary: dict, filename: str = "data.json", indent: int = 2, **kwargs
+) -> discord.File:
     """Create a :class:`discord.File` object from a dictionary.
 
     Parameters
     ----------
     dictionary:
         The dictionary to convert to a JSON file.
     filename:
         The filename to use for the JSON file.
+    indent:
+        The indent to use for the JSON file.
     **kwargs:
         Keyword arguments for :class:`discord.File`.
 
     Returns
     -------
     :class:`discord.File`
     """
-    content = json.dumps(dictionary, indent=2).encode()
+    content = json.dumps(dictionary, indent=indent).encode()
     return discord.File(io.BytesIO(content), filename=filename, **kwargs)
 
 
 def create_text_file(text: str, filename: str = "data.txt", **kwargs) -> discord.File:
     """Create a :class:`discord.File` object from a string.
 
     Parameters
```

### Comparing `ezcord-0.2.1/src/ezcord.egg-info/PKG-INFO` & `ezcord-0.2.2/src/ezcord.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezcord
-Version: 0.2.1
+Version: 0.2.2
 Summary: An easy-to-use extension for the Pycord library
 Author: tibue99
 License: MIT
 Project-URL: GitHub, https://github.com/tibue99/ezcord
 Project-URL: Documentation, https://ezcord.readthedocs.io
 Keywords: discord,pycord,py-cord
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ezcord-0.2.1/src/ezcord.egg-info/SOURCES.txt` & `ezcord-0.2.2/src/ezcord.egg-info/SOURCES.txt`

 * *Files identical despite different names*

