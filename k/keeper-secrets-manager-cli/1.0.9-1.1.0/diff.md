# Comparing `tmp/keeper-secrets-manager-cli-1.0.9.tar.gz` & `tmp/keeper-secrets-manager-cli-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keeper-secrets-manager-cli-1.0.9.tar", last modified: Sun Mar 27 19:55:51 2022, max compression
+gzip compressed data, was "keeper-secrets-manager-cli-1.1.0.tar", last modified: Wed May 31 23:12:07 2023, max compression
```

## Comparing `keeper-secrets-manager-cli-1.0.9.tar` & `keeper-secrets-manager-cli-1.1.0.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-27 19:55:51.458314 keeper-secrets-manager-cli-1.0.9/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-27 19:55:26.000000 keeper-secrets-manager-cli-1.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1461 2022-03-27 19:55:51.458314 keeper-secrets-manager-cli-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      232 2022-03-27 19:55:26.000000 keeper-secrets-manager-cli-1.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-27 19:55:51.458314 keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli/
--rw-r--r--   0 runner    (1001) docker     (121)     6181 2022-03-27 19:55:26.000000 keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    34797 2022-03-27 19:55:26.000000 keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4327 2022-03-27 19:55:26.000000 keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli/common.py
--rw-r--r--   0 runner    (1001) docker     (121)      467 2022-03-27 19:55:26.000000 keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli/exception.py
--rw-r--r--   0 runner    (1001) docker     (121)     4759 2022-03-27 19:55:26.000000 keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli/exec.py
--rw-r--r--   0 runner    (1001) docker     (121)     2682 2022-03-27 19:55:26.000000 keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli/export.py
--rw-r--r--   0 runner    (1001) docker     (121)     2659 2022-03-27 19:55:26.000000 keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli/init.py
--rw-r--r--   0 runner    (1001) docker     (121)    15146 2022-03-27 19:55:26.000000 keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli/profile.py
--rw-r--r--   0 runner    (1001) docker     (121)    29699 2022-03-27 19:55:26.000000 keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli/secret.py
--rw-r--r--   0 runner    (1001) docker     (121)     8188 2022-03-27 19:55:26.000000 keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli/table.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-27 19:55:51.458314 keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1461 2022-03-27 19:55:50.000000 keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      750 2022-03-27 19:55:51.000000 keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-27 19:55:50.000000 keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-03-27 19:55:51.000000 keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-27 19:55:50.000000 keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      194 2022-03-27 19:55:51.000000 keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-03-27 19:55:51.000000 keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-27 19:55:51.458314 keeper-secrets-manager-cli-1.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2203 2022-03-27 19:55:26.000000 keeper-secrets-manager-cli-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:12:07.956893 keeper-secrets-manager-cli-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 23:11:49.000000 keeper-secrets-manager-cli-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-31 23:12:07.956893 keeper-secrets-manager-cli-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-05-31 23:11:49.000000 keeper-secrets-manager-cli-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:12:07.956893 keeper-secrets-manager-cli-1.1.0/keeper_secrets_manager_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     6237 2023-05-31 23:11:49.000000 keeper-secrets-manager-cli-1.1.0/keeper_secrets_manager_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45038 2023-05-31 23:11:49.000000 keeper-secrets-manager-cli-1.1.0/keeper_secrets_manager_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-05-31 23:11:49.000000 keeper-secrets-manager-cli-1.1.0/keeper_secrets_manager_cli/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11554 2023-05-31 23:11:49.000000 keeper-secrets-manager-cli-1.1.0/keeper_secrets_manager_cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-31 23:11:49.000000 keeper-secrets-manager-cli-1.1.0/keeper_secrets_manager_cli/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-05-31 23:11:49.000000 keeper-secrets-manager-cli-1.1.0/keeper_secrets_manager_cli/exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-05-31 23:11:49.000000 keeper-secrets-manager-cli-1.1.0/keeper_secrets_manager_cli/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-05-31 23:11:49.000000 keeper-secrets-manager-cli-1.1.0/keeper_secrets_manager_cli/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19224 2023-05-31 23:11:49.000000 keeper-secrets-manager-cli-1.1.0/keeper_secrets_manager_cli/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30918 2023-05-31 23:11:49.000000 keeper-secrets-manager-cli-1.1.0/keeper_secrets_manager_cli/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54547 2023-05-31 23:11:49.000000 keeper-secrets-manager-cli-1.1.0/keeper_secrets_manager_cli/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8189 2023-05-31 23:11:49.000000 keeper-secrets-manager-cli-1.1.0/keeper_secrets_manager_cli/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:12:07.956893 keeper-secrets-manager-cli-1.1.0/keeper_secrets_manager_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-31 23:12:07.000000 keeper-secrets-manager-cli-1.1.0/keeper_secrets_manager_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-31 23:12:07.000000 keeper-secrets-manager-cli-1.1.0/keeper_secrets_manager_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 23:12:07.000000 keeper-secrets-manager-cli-1.1.0/keeper_secrets_manager_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-31 23:12:07.000000 keeper-secrets-manager-cli-1.1.0/keeper_secrets_manager_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 23:12:07.000000 keeper-secrets-manager-cli-1.1.0/keeper_secrets_manager_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-31 23:12:07.000000 keeper-secrets-manager-cli-1.1.0/keeper_secrets_manager_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-31 23:12:07.000000 keeper-secrets-manager-cli-1.1.0/keeper_secrets_manager_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 23:12:07.956893 keeper-secrets-manager-cli-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-31 23:11:49.000000 keeper-secrets-manager-cli-1.1.0/setup.py
```

### Comparing `keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli/__init__.py` & `keeper-secrets-manager-cli-1.1.0/keeper_secrets_manager_cli/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,112 +1,120 @@
 # -*- coding: utf-8 -*-
 #  _  __
-# | |/ /___ ___ _ __  ___ _ _ ®
+# | |/ /___ ___ _ __  ___ _ _ (R)
 # | ' </ -_) -_) '_ \/ -_) '_|
 # |_|\_\___\___| .__/\___|_|
 #              |_|
 #
 # Keeper Secrets Manager
 # Copyright 2021 Keeper Security Inc.
 # Contact: ops@keepersecurity.com
 #
 
 from keeper_secrets_manager_core import SecretsManager
 from keeper_secrets_manager_core.core import KSMCache
 from keeper_secrets_manager_core.storage import InMemoryKeyValueStorage
 from keeper_secrets_manager_core.configkeys import ConfigKeys
 from keeper_secrets_manager_cli.common import find_ksm_path
+from keeper_secrets_manager_cli.exception import KsmCliException
 from keeper_secrets_manager_helper.record_type import RecordType
 from distutils.util import strtobool
 from .exception import KsmCliException
 from .profile import Profile
+from .config import Config
 import sys
 import os
 
 
 class KeeperCli:
 
     @staticmethod
     def get_client(**kwargs):
         return SecretsManager(**kwargs)
 
     def __init__(self, ini_file=None, profile_name=None, output=None, use_color=None, use_cache=None,
-                 record_type_dir=None, editor=None, editor_use_blocking=False, editor_process_name=None):
+                 record_type_dir=None, editor=None, editor_use_blocking=False, editor_process_name=None,
+                 global_config=None, log_level=None):
 
-        self.profile = Profile(cli=self, ini_file=ini_file)
+        self.log_level = os.environ.get("KSM_DEBUG", log_level)
+        # If set via the command line, make sure the environmental variable gets set.
+        if self.log_level is not None:
+            os.environ["KSM_DEBUG"] = self.log_level
+
+        self.profile = Profile(cli=self, ini_file=ini_file, config=global_config)
         self._client = None
 
-        self.log_level = os.environ.get("KSM_DEBUG", None)
         self.use_color = use_color
         self.record_type_dir = record_type_dir
 
         # The editor to launch ... however this might be a bat or cmd file, not the real application
         self.editor = editor
-        # Some application don't block. To enabling blocking the CLI, set this to True
+        # Some applications don't block. To enabling blocking the CLI, set this to True
         self.editor_use_blocking = editor_use_blocking
         # Blocking might be waiting until a process in the task list goes away. This is that process.
         self.editor_process_name = editor_process_name
 
         self.use_cache = use_cache
 
-        # If no config file is loaded, then don't init the SDK
-        if self.profile.is_loaded is True:
+        # If we have profiles
+        if self.profile.has_profiles is True:
 
             # If the profile is not set
             if profile_name is None:
                 profile_name = self.profile.get_active_profile_name()
 
                 # If we don't have a profile we can't do anything.
                 if profile_name is None:
                     raise ValueError("Cannot determine the active profile.")
 
             self.config = self.profile.get_profile_config(profile_name)
 
             config_storage = InMemoryKeyValueStorage()
-            config_storage.set(ConfigKeys.KEY_CLIENT_KEY, self.config.get("clientKey"))
-            config_storage.set(ConfigKeys.KEY_CLIENT_ID, self.config.get("clientId"))
-            config_storage.set(ConfigKeys.KEY_PRIVATE_KEY, self.config.get("privateKey"))
-            config_storage.set(ConfigKeys.KEY_APP_KEY, self.config.get("appKey"))
-            config_storage.set(ConfigKeys.KEY_HOSTNAME, self.config.get("hostname"))
-            config_storage.set(ConfigKeys.KEY_OWNER_PUBLIC_KEY, self.config.get("appOwnerPublicKey"))
+            config_storage.set(ConfigKeys.KEY_CLIENT_ID, self.config.client_id)
+            config_storage.set(ConfigKeys.KEY_PRIVATE_KEY, self.config.private_key)
+            config_storage.set(ConfigKeys.KEY_APP_KEY, self.config.app_key)
+            config_storage.set(ConfigKeys.KEY_HOSTNAME, self.config.hostname)
+            config_storage.set(ConfigKeys.KEY_OWNER_PUBLIC_KEY, self.config.app_owner_public_key)
 
-            common_profile = self.profile.get_profile_config(Profile.config_profile)
+            common_config = self.profile.get_common_config()
 
             # Get the active configuration
 
             # By default, don't use the cache.
             if self.use_cache is None:
-                self.use_cache = bool(strtobool(common_profile.get(Profile.cache_key, str(False))))
+                self.use_cache = bool(strtobool(str(common_config.cache)))
 
-            self._client = self.get_client(
-                config=config_storage,
-                log_level=self.log_level,
-                custom_post_function=KSMCache.caching_post_function if self.use_cache is True else None
-            )
+            try:
+                self._client = self.get_client(
+                    config=config_storage,
+                    log_level=self.log_level,
+                    custom_post_function=KSMCache.caching_post_function if self.use_cache is True else None
+                )
+            except Exception as err:
+                raise KsmCliException(str(err))
 
             # By default, use colors.
             if self.use_color is None:
-                self.use_color = bool(strtobool(common_profile.get(Profile.color_key, str(True))))
+                self.use_color = bool(strtobool(str(common_config.color)))
 
             if self.record_type_dir is None:
-                self.record_type_dir = common_profile.get(Profile.record_type_dir_key, None)
+                self.record_type_dir = common_config.record_type_dir
                 if self.record_type_dir is None:
                     self.record_type_dir = find_ksm_path("record_type", is_file=False)
 
-            # If the have a directory where record type schema files may exists, attempt to load
+            # If they have a directory where record type schema files may exist, attempt to load
             # them.
             if self.record_type_dir is not None and os.path.exists(self.record_type_dir) is True:
                 RecordType.find_and_load_record_type_schema_files(self.record_type_dir)
 
             # Get the editor to use for visual editing a record
             if self.editor is None:
-                self.editor = common_profile.get(Profile.editor_key, None)
-            self.editor_use_blocking = bool(strtobool(common_profile.get(Profile.editor_use_blocking_key,
-                                                                         str(editor_use_blocking))))
-            self.editor_process_name = common_profile.get(Profile.editor_process_name_key, editor_process_name)
+                self.editor = common_config.editor
+            self.editor_use_blocking = bool(strtobool(str(common_config.editor_use_blocking)))
+            self.editor_process_name = common_config.editor_process_name
         else:
             # Set the log level. We don't have the client to set the level, so set it here.
             if use_color is None:
                 self.use_color = True
 
         # Default to stdout if the output is not set.
         if output is None:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli/__main__.py` & `keeper-secrets-manager-cli-1.1.0/keeper_secrets_manager_cli/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #  _  __
-# | |/ /___ ___ _ __  ___ _ _ ®
+# | |/ /___ ___ _ __  ___ _ _ (R)
 # | ' </ -_) -_) '_ \/ -_) '_|
 # |_|\_\___\___| .__/\___|_|
 #              |_|
 #
 # Keeper Secrets Manager
 # Copyright 2021 Keeper Security Inc.
 # Contact: ops@keepersecurity.com
@@ -14,42 +14,49 @@
 from click_help_colors import HelpColorsGroup, HelpColorsCommand
 from click_repl import repl, exit as repl_exit
 from colorama import Fore, Style, init
 from . import KeeperCli
 from .exception import KsmCliException
 from .exec import Exec
 from .secret import Secret
+from .sync import Sync
 from .profile import Profile
 from .init import Init
+from .config import Config
 import sys
 import os
 import keeper_secrets_manager_core
 import traceback
 import importlib_metadata
 import difflib
 import typing as t
 from update_checker import UpdateChecker
 
 
+global_config = Config()
+
+
 # NOTE: For the CLI, all groups and command are lowercase. All arguments are lower case, so you cannot use
-# -n and -N for an arg flag. If you add a command, you need to add it to the list of known commands so we can
-# do a best match.
+# -n and -N for an arg flag. If you add a command, you need to add it to the list of known commands, so we can
+# do a "best match."
 
 
 class AliasedGroup(HelpColorsGroup):
     known_commands = [
         "config",
         "color",
         "show",
         "exec",
         "profile",
         "active",
         "export",
         "import",
         "init",
+        "setup",
+        "sync",
         "secret",
         "totp",
         "download",
         "get",
         "list",
         "notation",
         "update",
@@ -74,14 +81,15 @@
         "g": "get",
         "l": "list",
         "t": "totp",
         "d": "download",
         "n": "notation",
         "u": "update",
         "v": "version",
+        "y": "sync",
         "exit": "quit",
         "pass": "password",
         "q": "quit",
         "help": "--help"
     }
 
     def get_command(self, ctx, cmd_name):
@@ -106,29 +114,33 @@
                 seq = difflib.SequenceMatcher(a=cmd_name, b=command)
                 if seq.ratio() > best_score:
                     best_score = seq.ratio()
                     best_command = command
 
             if best_score > 0.50:
                 cmd_name = best_command
-        return super().get_command(ctx, cmd_name)
+        return super().get_command(ctx, str(cmd_name))
 
     def parse_args(self, ctx, args: t.List[str]):
 
         """ Convert any argument case-insensitive.
 
         Lowercase any argument that starts with a -, except if it's 22 characters long. If it's 22 chars long, it
         most likely a record uid that starts a with -.
         """
 
         new_args: t.List[str] = []
         for item in args:
             # 22 is the length of the UID. We don't want to change the case of that if it starts with a -
             if item.startswith("-") and len(item) != 22:
-                item = item.lower()
+                item_parts = item.split("=")
+                item = item_parts[0].lower()
+                item_parts = item_parts[1:]
+                if len(item_parts) > 0:
+                    item += "=" + "=".join(item_parts)
             new_args.append(item)
 
         return super().parse_args(ctx, new_args)
 
 
 def _get_cli(**kwargs):
     return KeeperCli(**kwargs)
@@ -138,15 +150,15 @@
 
     # Unit test do not know their version
     versions = {
         "keeper-secrets-manager-core": "Unknown",
         "keeper-secrets-manager-cli": "Unknown"
     }
 
-    # Inside of the binaries, it's hard to get versions # so we create a versions.txt file in the build.
+    # In the binaries, it's hard to get versions # so we create a versions.txt file in the build.
     # If the versions.txt file exists, read the versions from that file.
 
     ksm_bin_path = os.path.dirname(__file__)
     # Get the directory of the executable file. If last directory is keeper_secrets_manager_cli, get the parent
     # directory. There is no keeper_secrets_manager_cli directory.
     if ksm_bin_path.endswith("keeper_secrets_manager_cli") is True:
         ksm_bin_path = os.path.dirname(ksm_bin_path)
@@ -179,16 +191,16 @@
     return UpdateChecker().check(module, versions[module])
 
 
 def base_command_help(f):
     doc = f.__doc__
 
     versions = get_versions()
-    cli_version = versions.get("keeper-secrets-manager-cli")
-    sdk_version = versions.get("keeper-secrets-manager-core")
+    cli_version = versions.get("keeper-secrets-manager-cli", "")
+    sdk_version = versions.get("keeper-secrets-manager-core", "")
 
     doc = "{} Version: {} ".format(
         Fore.RED + doc + Style.RESET_ALL,
         Fore.YELLOW + cli_version + Style.RESET_ALL
     )
     try:
         # The __doc__ stuff gets formatted so new line don't work, however long spaces will.
@@ -205,42 +217,91 @@
         pass
 
     f.__doc__ = doc
 
     return f
 
 
+class Mutex(click.Option):
+    def __init__(self, *args, **kwargs):
+        # Detect mutually exclusive or required options - search by key only or key and value
+        self.required_if:t.List[t.Tuple[str,str]] = kwargs.pop("required_if", [])
+        self.not_required_if:t.List[t.Tuple[str,str]] = kwargs.pop("not_required_if", [])
+
+        # at least one search parameter is required
+        assert self.required_if or self.not_required_if, "'required_if' and/or 'not_required_if' parameter required"
+
+        # if both params present they shouldn't overlap
+        if self.required_if and self.not_required_if:
+            overlap = [x for x in self.required_if if x in self.not_required_if]
+            assert not overlap, "'required_if' and 'not_required_if' parameters should not overlap in " + ", ".join("(%s)" % ",".join(x) for x in overlap)
+
+        exclusive_msg = ("Option is mutually exclusive with " + ", ".join("(%s)" % ",".join(tup) for tup in self.not_required_if) + ".") if self.not_required_if else ""
+        required_msg  = ("Option is required with " + ", ".join("(%s)" % ",".join(tup) for tup in self.required_if) + ".") if self.required_if else ""
+        kwargs["help"] = (kwargs.get("help", "") + " " + required_msg + " " + exclusive_msg).strip()
+
+        super(Mutex, self).__init__(*args, **kwargs)
+
+    def handle_parse_result(self, ctx, opts, args):
+        # ('option','value') - option present with the specified value assigned
+        # ('option',) - option present with or without any value
+        current_opt:bool = self.name in opts
+        for mutex_opt in self.not_required_if:
+            if mutex_opt and mutex_opt[0] in opts and (len(mutex_opt) == 1 or opts.get(mutex_opt[0], str(mutex_opt[1])+'_') == mutex_opt[1]):
+                if current_opt:
+                    raise click.UsageError("Illegal usage: '" + str(self.name) + "' is mutually exclusive with " + str(mutex_opt) + ".")
+                else:
+                    self.prompt = None
+        for mutex_opt in self.required_if:
+            if mutex_opt and mutex_opt[0] in opts and (len(mutex_opt) == 1 or opts.get(mutex_opt[0], str(mutex_opt[1])+'_') == mutex_opt[1]):
+                if not current_opt:
+                    raise click.UsageError("Illegal usage: '" + str(self.name) + "' is required with " + str(mutex_opt) + ".")
+                else:
+                    self.prompt = None
+        return super(Mutex, self).handle_parse_result(ctx, opts, args)
+
+
 # MAIN GROUP
 @click.group(
     cls=AliasedGroup,
     help_headers_color='yellow',
     help_options_color='green'
 )
 @click.option('--ini-file', type=str, help="INI config file.")
 @click.option('--profile-name', '-p', type=str, help='Config profile')
 @click.option('--output', '-o', type=str, help='Output [stdout|stderr|filename]', default='stdout')
 @click.option('--color/--no-color', '-c/-nc', default=None, help="Use color in table views, where applicable.")
 @click.option('--cache/--no-cache', default=None, help="Enable/disable record caching.")
+@click.option('--log-level', type=click.Choice(['DEBUG', 'INFO', 'WARNING', 'ERROR']), help="Debug log level.")
 @click.pass_context
 @base_command_help
-def cli(ctx, ini_file, profile_name, output, color, cache):
+def cli(ctx, ini_file, profile_name, output, color, cache, log_level):
     """Keeper Secrets Manager CLI
     """
+
     ctx.obj = {
-        "cli": _get_cli(ini_file=ini_file, profile_name=profile_name, output=output, use_color=color, use_cache=cache),
+        "cli": _get_cli(
+            ini_file=ini_file,
+            profile_name=profile_name,
+            output=output,
+            use_color=color,
+            use_cache=cache,
+            global_config=global_config,
+            log_level=log_level
+        ),
         "ini_file": ini_file,
         "profile_name": profile_name,
         "output": output,
         "use_color": color,
-        "use_cache": cache
+        "use_cache": cache,
+        "log_level": log_level
     }
 
 
 # PROFILE GROUP
-
 @click.group(
     name='profile',
     cls=AliasedGroup,
     help_headers_color='yellow',
     help_options_color='green'
 )
 def profile_command():
@@ -273,45 +334,137 @@
         print("NOTE: The INI file config was set on the top level command and also set on the init sub-command. The top"
               " level command parameter will be ignored for the init sub-command.", file=sys.stderr)
 
     Profile.init(
         token=token,
         server=hostname,
         ini_file=ini_file,
-        profile_name=profile_name
+        profile_name=profile_name,
+        launched_from_app=global_config.launched_from_app
     )
 
 
 @click.command(
+    name='setup',
+    cls=HelpColorsCommand,
+    help_options_color='blue'
+)
+@click.option('--type', '-t', required=True, type=click.Choice(['aws']), help="The type of the remote storage: aws/azure/gcp - currently only aws is supported.")
+@click.option('--secret', '-s', required=False, type=str, default='ksm-config', help="Secret's name or full URI in Secrets Manager.")
+@click.option('--credentials', '-c', required=False, type=click.Choice(['ec2instance', 'profile', 'keys']), default='ec2instance', help="The type of the credentials for the remote storage. Default value is ec2instance")
+@click.option('--credentials-profile', '-n', required=False, type=str, help="Profile name from local machine config.")
+@click.option('--aws-access-key-id', required=False, type=str, help="AWS Access Key ID.")
+@click.option('--aws-secret-access-key', required=False, type=str, help="AWS Secret Access Key.")
+@click.option('--region', required=False, type=str, help="AWS region.")
+@click.option('--fallback', '-f', is_flag=False, help='If credentials fail then fallback to default profile on the machine.')
+@click.option('--ini-file', type=str, help="INI config file to create.")
+@click.option('--profile-name', '-p', type=str, help='Config profile to create.')
+@click.pass_context
+def profile_setup_command(ctx, type, secret, credentials,
+                          credentials_profile,
+                          aws_access_key_id, aws_secret_access_key, region,
+                          fallback, ini_file, profile_name):
+    """Setup a profile to load config from remote storage"""
+
+    # Since the top level options are available for all commands,
+    # it might be confusing the setup command
+    if ctx.obj["ini_file"] is not None and ini_file is not None:
+        print("NOTE: The INI file config was set on the top level command and"
+              " also set on the setup sub-command. The top level command"
+              " parameter will be ignored for the setup sub-command.",
+              file=sys.stderr)
+
+    if type == 'aws':
+        if not secret:
+            secret = 'ksm-config'
+        if not credentials:
+            credentials = 'ec2instance'
+
+        # credentials options
+        # ec2instance: doesn't require additional options
+        # profile: accepts only --credentials-profile=NAME
+        # keys: requires both keys and region
+        if credentials == 'ec2instance':
+            if (credentials_profile or
+                    aws_access_key_id or aws_secret_access_key or region):
+                raise click.ClickException(
+                    "Unexpected options for --credentials=ec2instance "
+                    "which doesn't require additional parameters. Please "
+                    "do not pass other settings (profile/key/region)")
+            Profile.from_aws_ec2instance(
+                secret=secret,
+                fallback=fallback,
+                ini_file=ini_file,
+                profile_name=profile_name,
+                launched_from_app=global_config.launched_from_app)
+        elif credentials == 'profile':
+            credentials_profile = credentials_profile or ""
+            # accepts only one optional parameter -cp|credentials-profile=NAME
+            if aws_access_key_id or aws_secret_access_key or region:
+                raise click.ClickException(
+                    "Unexpected options for --credentials=profile "
+                    "which accepts only one optional parameter "
+                    "--credentials-profile=NAME "
+                    "Please do not pass any keys (key/region)")
+            Profile.from_aws_profile(
+                secret=secret,
+                fallback=fallback,
+                aws_profile=credentials_profile,
+                ini_file=ini_file,
+                profile_name=profile_name,
+                launched_from_app=global_config.launched_from_app)
+        elif credentials == 'keys':
+            if credentials_profile:
+                raise click.ClickException(
+                    f"With --credentials-profile={credentials_profile} "
+                    "must specify option --credentials=profile")
+            # requires: aws-access-key-id, aws-secret-access-key, region
+            if not (aws_access_key_id and aws_secret_access_key and region):
+                raise click.ClickException(
+                    "Missing options for --credentials=keys "
+                    "which requires both keys and region to be set with "
+                    "--aws-access-key-id, --aws-secret-access-key, --region")
+            Profile.from_aws_custom(
+                secret=secret,
+                fallback=fallback,
+                aws_access_key_id=aws_access_key_id,
+                aws_secret_access_key=aws_secret_access_key,
+                region=region,
+                ini_file=ini_file,
+                profile_name=profile_name,
+                launched_from_app=global_config.launched_from_app)
+
+
+@click.command(
     name='list',
     cls=HelpColorsCommand,
     help_options_color='blue'
 )
 @click.option('--json', is_flag=True, help='Return secret as JSON')
 @click.pass_context
 def profile_list_command(ctx, json):
     """List all profiles"""
 
     output = "text"
     if json is True:
         output = "json"
 
-    Profile(cli=ctx.obj["cli"]).list_profiles(output=output)
+    Profile(cli=ctx.obj["cli"], config=global_config).list_profiles(output=output)
 
 
 @click.command(
     name='active',
     cls=HelpColorsCommand,
     help_options_color='blue'
 )
 @click.argument('profile-name', type=str, required=True, nargs=1)
 @click.pass_context
 def profile_active_command(ctx, profile_name):
     """Set the active profile"""
-    Profile(cli=ctx.obj["cli"]).set_active(
+    Profile(cli=ctx.obj["cli"], config=global_config).set_active(
         profile_name=profile_name
     )
 
 
 @click.command(
     name='export',
     cls=HelpColorsCommand,
@@ -320,15 +473,15 @@
 @click.option('--plain', is_flag=True, help='Export the config not base64 encoded.')
 @click.option('--file-format', type=click.Choice(['ini', 'json'], case_sensitive=False), default='ini',
               help='File format to export.')
 @click.argument('profile-name', type=str, required=False, nargs=1)
 @click.pass_context
 def profile_export_command(ctx, plain, file_format, profile_name):
     """Create a new config file from a profile"""
-    Profile(cli=ctx.obj["cli"]).export_config(
+    Profile(cli=ctx.obj["cli"], config=global_config).export_config(
         plain=plain,
         file_format=file_format,
         profile_name=profile_name
     )
 
 
 @click.command(
@@ -337,30 +490,30 @@
     help_options_color='blue'
 )
 @click.option('--output-file', '-f', type=str, required=False, help='Create the config in a specific file location.')
 @click.argument('config-base64', type=str, required=True, nargs=1)
 @click.pass_context
 def profile_import_command(ctx, output_file, config_base64):
     """Import an encrypted config file"""
-    Profile(cli=ctx.obj["cli"]).import_config(
+    Profile(cli=ctx.obj["cli"], config=global_config).import_config(
         file=output_file,
-        config_base64=config_base64
+        config_base64=config_base64,
+        launched_from_app=global_config.launched_from_app
     )
 
 
 profile_command.add_command(profile_init_command)
+profile_command.add_command(profile_setup_command)
 profile_command.add_command(profile_list_command)
 profile_command.add_command(profile_active_command)
 profile_command.add_command(profile_export_command)
 profile_command.add_command(profile_import_command)
 
 
 # SECRET GROUP
-
-
 @click.group(
     name='secret',
     cls=AliasedGroup,
     help_headers_color='yellow',
     help_options_color='green'
 )
 @click.pass_context
@@ -400,17 +553,18 @@
 @click.option('--title', '-t', type=str, multiple=True, help='Title of record.')
 @click.option('--field', '-f', type=str, help='Field to get.')
 @click.option('--query', '-q', type=str, help='Perform a JSONPath query on results.')
 @click.option('--json', is_flag=True, help='Return secret as JSON')
 @click.option('--force-array', is_flag=True, help="Return secrets as array even if a single record.")
 @click.option('--unmask', is_flag=True, help="Show password like values in table views.")
 @click.option('--inflate/--deflate', default=True, help="Load in outside records.")
+@click.option('--raw', is_flag=True, help='Remove surrounding quotes on value when using query.')
 @click.argument('extra-uid', type=str, nargs=-1)
 @click.pass_context
-def secret_get_command(ctx, uid, title, field, query, json, force_array, unmask, inflate, extra_uid):
+def secret_get_command(ctx, uid, title, field, query, json, force_array, unmask, inflate, extra_uid, raw):
     """Get secret record(s)"""
 
     uid_list = []
     if uid is not None:
         for u in uid:
             uid_list.append(u)
     if extra_uid is not None:
@@ -435,15 +589,16 @@
         field=field,
         jsonpath_query=query,
         output_format=output,
         force_array=force_array,
         load_references=True,
         unmask=unmask,
         use_color=ctx.obj["cli"].use_color,
-        inflate=inflate
+        inflate=inflate,
+        raw=raw
     )
 
 
 @click.command(
     name='notation',
     cls=HelpColorsCommand,
     help_options_color='blue'
@@ -480,24 +635,29 @@
 
 @click.command(
     name='download',
     cls=HelpColorsCommand,
     help_options_color='blue'
 )
 @click.option('--uid', '-u', required=True, type=str, help="UID of the secret.")
-@click.option('--name', required=True, type=str, help='Name of the file to download.')
+@click.option('--name', type=str, help='Name of the file to download.')
+@click.option('--file-uid', type=str, help='Unique id of the file to download.')
 @click.option('--file-output', required=True, type=str, help="Where to write the file's content. "
                                                              "[filename|stdout|stderr]")
 @click.option('--create-folders', is_flag=True, help='Create folder for filename path.')
 @click.pass_context
-def secret_download_command(ctx, uid, name, file_output, create_folders):
+def secret_download_command(ctx, uid, name, file_uid, file_output, create_folders):
     """Download a file from a secret record"""
+    if name is None and file_uid is None:
+        raise KsmCliException("Either the name or file uid needs to be specified.")
+
     ctx.obj["secret"].download(
         uid=uid,
         name=name,
+        file_uid=file_uid,
         file_output=file_output,
         create_folders=create_folders
     )
 
 
 @click.command(
     name='totp',
@@ -765,16 +925,15 @@
     cls=AliasedGroup,
     help_headers_color='yellow',
     help_options_color='green'
 )
 @click.pass_context
 def config_command(ctx):
     """Configure the command line tool"""
-    ctx.obj["profile"] = Profile(cli=ctx.obj["cli"])
-    pass
+    ctx.obj["profile"] = Profile(cli=ctx.obj["cli"], config=global_config)
 
 
 @click.command(
     name='show',
     cls=HelpColorsCommand,
     help_options_color='blue'
 )
@@ -863,15 +1022,15 @@
     cls=AliasedGroup,
     help_headers_color='yellow',
     help_options_color='green'
 )
 @click.pass_context
 def init_command(ctx):
     """Initialize a configuration file for integrations"""
-    ctx.obj["profile"] = Profile(cli=ctx.obj["cli"])
+    ctx.obj["profile"] = Profile(cli=ctx.obj["cli"], config=global_config)
 
 
 @click.command(
     name='k8s',
     cls=HelpColorsCommand,
     help_options_color='blue'
 )
@@ -929,15 +1088,15 @@
         str(sys.version_info.micro)
     ])))
     print("Python Install: {}".format(sys.executable))
     print("CLI Version: {}".format(versions["keeper-secrets-manager-cli"]))
     print("CLI Install: {}".format(os.path.dirname(os.path.realpath(__file__))))
     print("SDK Version: {}".format(versions["keeper-secrets-manager-core"]))
     print("SDK Install: {}".format(os.path.dirname(os.path.realpath(keeper_secrets_manager_core.__file__))))
-    print("Config file: {}".format(ctx.obj["cli"].profile.ini_file))
+    print("Config file: {}".format(global_config.ini_file))
 
     try:
         if versions["keeper-secrets-manager-cli"] != "Unknown":
             update = update_available("keeper-secrets-manager-cli", versions)
             if update is not None:
                 print("Version {} is available for the CLI".format(update.available_version))
 
@@ -950,55 +1109,85 @@
 
 
 @click.command(
     name='shell',
     cls=HelpColorsCommand,
     help_options_color='blue'
 )
-def shell_command():
+@click.option('--app', is_flag=True, help='Launched from application.')
+def shell_command(app):
     """Run KSM in a shell"""
 
+    global global_config
+    global_config = Config()
+
+    # Flag that the application was launched as a Windows/macOS application.
+    global_config.launched_from_app = app
+
     # https://manytools.org/hacker-tools/ascii-banner/
     logo = """
 ██╗  ██╗███████╗███╗   ███╗     ██████╗██╗     ██╗
 ██║ ██╔╝██╔════╝████╗ ████║    ██╔════╝██║     ██║
 █████╔╝ ███████╗██╔████╔██║    ██║     ██║     ██║
 ██╔═██╗ ╚════██║██║╚██╔╝██║    ██║     ██║     ██║
 ██║  ██╗███████║██║ ╚═╝ ██║    ╚██████╗███████╗██║
 ╚═╝  ╚═╝╚══════╝╚═╝     ╚═╝     ╚═════╝╚══════╝╚═╝                                                                          
     """
     print(Fore.BLUE + logo + Style.RESET_ALL)
 
     versions = get_versions()
 
-    print(Fore.CYAN + "Current Version: " + Fore.GREEN + versions.get("keeper-secrets-manager-cli") + Style.RESET_ALL)
+    print(Fore.CYAN + "Current Version: " + Fore.GREEN + versions.get("keeper-secrets-manager-cli", "") + Style.RESET_ALL)
     update = update_available("keeper-secrets-manager-cli", versions)
     if update is not None:
         print(Fore.YELLOW + "Version {} is available.".format(update.available_version) + Style.RESET_ALL)
 
     print("\nRunning in shell mode. Type 'quit' to exit.\n")
 
     KsmCliException.in_a_shell = True
     repl(click.get_current_context(), prompt_kwargs={
-        "message": u'KSM Shell (? for help) > '
+        "message": u'\nKSM Shell (? for help) > '
     })
 
 
 @click.command(
     name='quit',
     cls=HelpColorsCommand,
     help_options_color='blue'
 )
 def quit_command():
     """Quit shell mode"""
     repl_exit()
 
 
+# SYNC COMMAND
+@click.command(
+    name='sync',
+    cls=HelpColorsCommand,
+    help_options_color='blue'
+)
+@click.option('--credentials', '-c', type=str, metavar="UID", help="Keeper record with credentials to access destination key/value store.",
+    cls=Mutex,
+    # not_required_if=[('type','json')],
+    required_if=[('type','azure'), ('type','aws'), ('type','gcp')]
+)
+@click.option('--type', '-t', type=click.Choice(['aws', 'azure', 'gcp', 'json']), default='json', help="Type of the target key/value storage (aws, azure, gcp, json).", show_default=True)
+@click.option('--dry-run', '-n', is_flag=True, help='Perform a trial run with no changes made.')
+@click.option('--preserve-missing', '-p', is_flag=True, help='Preserve destination value when source value is deleted.')
+@click.option('--map', '-m', nargs=2, type=(str, str), multiple=True, required=True, metavar="<KEY NOTATION>...", help='Map destination key names to values using notation URI.')
+@click.pass_context
+def sync_command(ctx, credentials, type, dry_run, preserve_missing, map):
+    """Sync selected keys from Keeper vault to secure cloud based key value store"""
+    sync = Sync(cli=ctx.obj["cli"])
+    sync.sync_values(type=type, credentials=credentials, dry_run=dry_run, preserve_missing=preserve_missing, map=map)
+
+
 # TOP LEVEL COMMANDS
 cli.add_command(profile_command)
+cli.add_command(sync_command)
 cli.add_command(secret_command)
 cli.add_command(exec_command)
 cli.add_command(config_command)
 cli.add_command(init_command)
 cli.add_command(version_command)
 cli.add_command(shell_command)
 cli.add_command(quit_command)
```

### Comparing `keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli/common.py` & `keeper-secrets-manager-cli-1.1.0/keeper_secrets_manager_cli/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+# -*- coding: utf-8 -*-
+#  _  __
+# | |/ /___ ___ _ __  ___ _ _ (R)
+# | ' </ -_) -_) '_ \/ -_) '_|
+# |_|\_\___\___| .__/\___|_|
+#              |_|
+#
+# Keeper Secrets Manager
+# Copyright 2021 Keeper Security Inc.
+# Contact: ops@keepersecurity.com
+#
+
 import os
 import shutil
 import platform
 import subprocess
 import time
 import psutil
 
@@ -19,17 +31,17 @@
         # Linux
         [os.environ.get("HOME", not_set)],
 
         # This seems like where other applications like to store their configs.
         [os.environ.get("HOME", not_set), ".config", "ksm"],
 
         [os.environ.get("HOME", not_set), ".keeper"],
-        ["/etc"],
-        ["/etc", "ksm"],
-        ["/etc", "keeper"],
+        ["etc"],
+        ["etc", "ksm"],
+        ["etc", "keeper"],
 
         # Windows
         [os.environ.get("USERPROFILE", not_set)],
         [os.environ.get("APPDIR", not_set)],
         [os.environ.get("PROGRAMDATA", not_set), "Keeper"],
         [os.environ.get("PROGRAMFILES", not_set), "Keeper"],
     ]
```

### Comparing `keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli/exec.py` & `keeper-secrets-manager-cli-1.1.0/keeper_secrets_manager_cli/exec.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #  _  __
-# | |/ /___ ___ _ __  ___ _ _ ®
+# | |/ /___ ___ _ __  ___ _ _ (R)
 # | ' </ -_) -_) '_ \/ -_) '_|
 # |_|\_\___\___| .__/\___|_|
 #              |_|
 #
 # Keeper Secrets Manager
 # Copyright 2021 Keeper Security Inc.
 # Contact: ops@keepersecurity.com
@@ -47,15 +47,17 @@
             if env_value.startswith(SecretsManager.notation_prefix) is True:
                 try:
                     os.environ["_" + env_key] = "_" + env_value
                     os.environ[env_key] = self._get_secret(env_value)
                 except ValueError as err:
                     # TODO: Change the SDK to throw a different exception when might not be notation.
                     # If the notation isn't actually notation, skip it, don't raise an exception
-                    if str(err).startswith("Keeper url missing"):
+                    if str(err).startswith("Invalid format of Keeper notation") \
+                            or str(err).startswith("Keeper notation is invalid") \
+                            or str(err).startswith("Keeper url missing"):
                         self.logger.info("Possible notation for env key {} was not used.".format(env_key))
                     else:
                         raise KsmCliException(str(err))
 
     def inline_replace(self, cmd=None):
 
         if cmd is None:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli/init.py` & `keeper-secrets-manager-cli-1.1.0/keeper_secrets_manager_cli/init.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # -*- coding: utf-8 -*-
 #  _  __
-# | |/ /___ ___ _ __  ___ _ _ ®
+# | |/ /___ ___ _ __  ___ _ _ (R)
 # | ' </ -_) -_) '_ \/ -_) '_|
 # |_|\_\___\___| .__/\___|_|
 #              |_|
 #
 # Keeper Secrets Manager
 # Copyright 2021 Keeper Security Inc.
 # Contact: ops@keepersecurity.com
 #
 
 from keeper_secrets_manager_core import SecretsManager
 from keeper_secrets_manager_core.storage import InMemoryKeyValueStorage
 from keeper_secrets_manager_core.configkeys import ConfigKeys
 from .export import Export
+from .config import Config
 import subprocess
 import sys
 
 
 class Init:
 
     @staticmethod
@@ -30,27 +31,32 @@
         return InMemoryKeyValueStorage()
 
     def __init__(self, cli, token, hostname=None, skip_ssl_verify=False):
         self.cli = cli
         self.token = token
         self.skip_ssl_verify = skip_ssl_verify
 
-        self.config = Init.init_config()
-        redeem_sm = Init.get_client(config=self.config, token=token, hostname=hostname,
+        redeem_sm = Init.get_client(config=Init.init_config(), token=token, hostname=hostname,
                                     verify_ssl_certs=not skip_ssl_verify)
         redeem_sm.get_secrets()
+        in_memory_config = redeem_sm.config
 
-        self.config_dict = {}
-        for e in ConfigKeys:
-            if self.config.contains(e):
-                self.config_dict[e.value] = self.config.get(e)
+        config = Config()
+        config.set_profile("NA",
+                           client_id=in_memory_config.get(ConfigKeys.KEY_CLIENT_ID),
+                           private_key=in_memory_config.get(ConfigKeys.KEY_PRIVATE_KEY),
+                           app_key=in_memory_config.get(ConfigKeys.KEY_APP_KEY),
+                           hostname=in_memory_config.get(ConfigKeys.KEY_HOSTNAME),
+                           app_owner_public_key=in_memory_config.get(ConfigKeys.KEY_OWNER_PUBLIC_KEY),
+                           server_public_key_id=in_memory_config.get(ConfigKeys.KEY_SERVER_PUBLIC_KEY_ID))
+        self.config = config.get_profile("NA")
 
     def get_k8s(self, name, namespace, apply=False, immutable=False):
 
-        base64_config = Export(config=self.config_dict, file_format="json", plain=False).run()
+        base64_config = Export(config=self.config, file_format="json", plain=False).run()
 
         if apply is True:
             subprocess.run([
                 "kubectl", "create", "secret", "generic", name,
                 "--from-literal=config={}".format(base64_config.decode())
             ])
             print("Created secret for KSM config.", file=sys.stderr)
@@ -62,20 +68,20 @@
                      "metadata:\n"\
                      "  name: {}\n"\
                      "  namespace: {}\n"\
                      "type: Opaque".format(base64_config.decode(), name, namespace)
 
             # Kubernetes v1.21
             if immutable is True:
-                secret += "immutable: True\n"
+                secret += "\nimmutable: True\n"
 
             print("", file=sys.stderr)
             self.cli.output(secret)
             print("", file=sys.stderr)
 
     def get_json(self, plain=False):
 
-        config_str = Export(config=self.config_dict, file_format="json", plain=plain).run()
+        config_str = Export(config=self.config, file_format="json", plain=plain).run()
 
         print("", file=sys.stderr)
         self.cli.output(config_str)
         print("", file=sys.stderr)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli/secret.py` & `keeper-secrets-manager-cli-1.1.0/keeper_secrets_manager_cli/secret.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #  _  __
-# | |/ /___ ___ _ __  ___ _ _ ®
+# | |/ /___ ___ _ __  ___ _ _ (R)
 # | ' </ -_) -_) '_ \/ -_) '_|
 # |_|\_\___\___| .__/\___|_|
 #              |_|
 #
 # Keeper Secrets Manager
 # Copyright 2021 Keeper Security Inc.
 # Contact: ops@keepersecurity.com
@@ -149,14 +149,15 @@
         ret = {
             "uid": record.uid,
             "title": record.title,
             "type": record.type,
             "fields": standard_fields,
             "custom_fields": custom_fields,
             "files": [{
+                "file_uid": x.f.get("fileUid"),
                 "name": x.name,
                 "title": x.title,
                 "type": x.type,
                 "last_modified": x.last_modified,
                 "size": x.size
             } for x in record.files]
         }
@@ -247,16 +248,22 @@
 
         if len(record_dict["files"]) > 0:
             ret += "\n"
             table = Table(use_color=use_color)
             table.add_column("File Name", allow_wrap=True, data_color=Fore.GREEN)
             table.add_column("Type")
             table.add_column("Size", align=ColumnAlign.RIGHT)
+            table.add_column("File UID")
             for file in record_dict["files"]:
-                row = [file["title"], file["type"], "{:n}".format(int(file["size"]))]
+                row = [
+                    file["title"],
+                    file["type"],
+                    "{:n}".format(int(file["size"])),
+                    file["file_uid"]
+                ]
                 table.add_row(row)
             ret += table.get_string() + "\n"
 
         ret += "\n"
 
         return ret
 
@@ -330,26 +337,35 @@
         if type(value) is not str:
             value = json.dumps(value)
 
         print("", file=sys.stderr)
         self.cli.output(value)
         print("", file=sys.stderr)
 
-    def _query_jsonpath(self, jsonpath_query, records, force_array):
+    def _query_jsonpath(self, jsonpath_query, records, force_array, raw):
         # Adjust records here so the JQ query works with the displayed JSON.
         record_list = Secret._adjust_records(records, force_array)
 
         try:
             results = self._get_jsonpath_results(record_list, jsonpath_query)
-            self.cli.output(json.dumps(results, indent=4))
+            output = json.dumps(results, indent=4)
+
+            # If the results was a string, converting it to JSON will place quotes around the value. That is
+            # bad when piping it into an env var. Just return the non-JSON results string.
+            if raw is True and isinstance(results, str) is True and output.startswith('"') is True and \
+                    output.endswith('"') is True:
+                output = results
+
+            self.cli.output(output)
         except Exception as err:
             raise KsmCliException("JSONPath failed: {}".format(err))
 
     def query(self, uids=None, titles=None, field=None, output_format='json', jsonpath_query=None,
-              force_array=False, load_references=False, unmask=False, use_color=None, inflate=True):
+              force_array=False, load_references=False, unmask=False, use_color=None, inflate=True,
+              raw=False):
 
         if use_color is None:
             use_color = self.cli.use_color
 
         if uids is None:
             uids = []
         if titles is None:
@@ -366,15 +382,19 @@
         records = []
         fetch_uids = None
 
         # If we are not searching by title, then set the fetch uid to the uids passed in.
         if len(titles) == 0:
             fetch_uids = uids
 
-        for record in self.cli.client.get_secrets(uids=fetch_uids):
+        secrets = self.cli.client.get_secrets(uids=fetch_uids)
+        if len(secrets) == 0 and fetch_uids is not None:
+            raise KsmCliException("Cannot find requested record(s).")
+
+        for record in secrets:
             add_record = False
 
             # If we are searching by title, the fetch_uids was None, we have all the records. We need to filter
             # them by the title or uids.
             if len(titles) > 0:
                 if record.title in titles or record.uid in uids:
                     add_record = True
@@ -395,14 +415,15 @@
             )
         # The user wants to use JSONPath to get the field(s) values.
         elif jsonpath_query is not None:
             self._query_jsonpath(
                 jsonpath_query=jsonpath_query,
                 records=records,
                 force_array=force_array,
+                raw=raw
             )
         else:
             return self.output_results(records=records, output_format=output_format, force_array=force_array,
                                        use_color=use_color)
 
     @staticmethod
     def _format_list(record_dict, use_color=True):
@@ -423,21 +444,28 @@
         if output_format == 'text':
             self.cli.output(self._format_list(record_dict, use_color=use_color))
         elif output_format == 'json':
             records = [{"uid": x.get("uid"), "title": x.get("title"), "record_type": x.get("type")}
                        for x in record_dict]
             self.cli.output(json.dumps(records, indent=4))
 
-    def download(self, uid, name, file_output, create_folders=False):
+    def download(self, uid, name, file_uid, file_output, create_folders=False):
 
         record = self.cli.client.get_secrets(uids=[uid])
         if len(record) == 0:
             raise KsmCliException("Cannot find a record for UID {}. Cannot download {}".format(uid, name))
 
-        file = record[0].find_file_by_title(name)
+        file = None
+        if file_uid is not None:
+            for check_file in record[0].files:
+                if check_file.f.get("fileUid") == file_uid:
+                    file = check_file
+                    break
+        else:
+            file = record[0].find_file_by_title(name)
         if file is None:
             raise KsmCliException("Cannot find a file named {} for UID {}. Cannot download file".format(name, uid))
 
         if file_output == 'stdout':
             sys.stderr.buffer.write(file.get_file_data())
         elif file_output == 'stderr':
             sys.stderr.buffer.write(file.get_file_data())
@@ -528,18 +556,24 @@
 
     def update(self, uid, fields=None, custom_fields=None, fields_json=None, custom_fields_json=None):
 
         record = self.cli.client.get_secrets(uids=[uid])
         if len(record) == 0:
             raise KsmCliException("Cannot find a record for UID {}.".format(uid))
 
+        def _get_label(x):
+            label = x.get("label")
+            if label is None or label == "":
+                label = x.get("type")
+            return label
+
         # Get a list of all labels/type allowed.
         labels = {
-            "field": [x.get("label", x.get("type")) for x in record[0].dict.get("fields", [])],
-            "custom_field": [x.get("label", x.get("type")) for x in record[0].dict.get("custom", [])]
+            "field": [_get_label(x) for x in record[0].dict.get("fields", [])],
+            "custom_field": [_get_label(x) for x in record[0].dict.get("custom", [])]
         }
 
         data = [
             {"type": "field", "is_json": False, "values": fields},
             {"type": "custom_field", "is_json": False, "values": custom_fields},
             {"type": "field", "is_json": True, "values": fields_json},
             {"type": "custom_field", "is_json": True, "values": custom_fields_json},
@@ -564,15 +598,15 @@
         except Exception as err:
             raise KsmCliException("Could not save record: {}".format(err))
 
     def _check_if_can_add_records(self):
         # Check to see if appOwnerPublicKey is in the keeper.ini. It's a newly added key and if the
         # profile is too old we can't add a record.
         profile_config = self.cli.profile.get_profile_config(self.cli.profile.get_active_profile_name())
-        if profile_config.get("appOwnerPublicKey") is None:
+        if profile_config.app_owner_public_key is None:
             raise KsmCliException("Your profile is out of date. It is missing the application order key. "
                                   "To create a record you will need to init a profile with a new token.")
 
     def add_record_interactive(self, version, folder_uid, record_type, output_format,
                                password_generate_flag, title=None, notes=None, editor=None):
         self._check_if_can_add_records()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli/table.py` & `keeper-secrets-manager-cli-1.1.0/keeper_secrets_manager_cli/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #  _  __
-# | |/ /___ ___ _ __  ___ _ _ ®
+# | |/ /___ ___ _ __  ___ _ _ (R)
 # | ' </ -_) -_) '_ \/ -_) '_|
 # |_|\_\___\___| .__/\___|_|
 #              |_|
 #
 # Keeper Secrets Manager
 # Copyright 2021 Keeper Security Inc.
 # Contact: ops@keepersecurity.com
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `keeper-secrets-manager-cli-1.0.9/keeper_secrets_manager_cli.egg-info/SOURCES.txt` & `keeper-secrets-manager-cli-1.1.0/keeper_secrets_manager_cli.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 LICENSE
 README.md
 setup.py
 keeper_secrets_manager_cli/__init__.py
 keeper_secrets_manager_cli/__main__.py
 keeper_secrets_manager_cli/common.py
+keeper_secrets_manager_cli/config.py
 keeper_secrets_manager_cli/exception.py
 keeper_secrets_manager_cli/exec.py
 keeper_secrets_manager_cli/export.py
 keeper_secrets_manager_cli/init.py
 keeper_secrets_manager_cli/profile.py
 keeper_secrets_manager_cli/secret.py
+keeper_secrets_manager_cli/sync.py
 keeper_secrets_manager_cli/table.py
 keeper_secrets_manager_cli.egg-info/PKG-INFO
 keeper_secrets_manager_cli.egg-info/SOURCES.txt
 keeper_secrets_manager_cli.egg-info/dependency_links.txt
 keeper_secrets_manager_cli.egg-info/entry_points.txt
 keeper_secrets_manager_cli.egg-info/not-zip-safe
 keeper_secrets_manager_cli.egg-info/requires.txt
```

### Comparing `keeper-secrets-manager-cli-1.0.9/setup.py` & `keeper-secrets-manager-cli-1.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,61 +4,64 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 # Get the long description from the README.md file
 with open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 install_requires = [
-    'keeper-secrets-manager-core>=16.2.2',
+    'keeper-secrets-manager-core>=16.5.4',
     'keeper-secrets-manager-helper',
+    'keeper-secrets-manager-storage>=1.0.1',
     'prompt-toolkit~=2.0',
-    'click',
-    'click_help_colors',
-    'click-repl',
     'jsonpath-rw-ext',
     'colorama',
     'importlib_metadata',
+    'click',
+    'click_help_colors',
+    'click-repl',
     'pyyaml',
     'update-checker',
-    'psutil'
+    'psutil',
+    'boto3'
 ]
 
 # Version set in the keeper_secrets_manager_cli.version file.
 setup(
     name="keeper-secrets-manager-cli",
-    version="1.0.9",
+    version="1.1.0",
     description="Command line tool for Keeper Secrets Manager",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Keeper Security",
-    author_email="ops@keepersecurity.com",
+    author_email="sm@keepersecurity.com",
     url="https://github.com/Keeper-Security/secrets-manager",
     license="MIT",
     keywords="Keeper Password Secrets Manager SDK CLI",
     packages=find_packages(exclude=["tests", "tests.*"]),
     zip_safe=False,
     install_requires=install_requires,
-    python_requires='>=3.6',
+    python_requires='>=3.7',
     project_urls={
         "Bug Tracker": "https://github.com/Keeper-Security/secrets-manager/issues",
         "Documentation": "https://app.gitbook.com/"
                          "@keeper-security/s/secrets-manager/secrets-manager/secrets-manager-command-line-interface",
         "Source Code": "https://github.com/Keeper-Security/secrets-manager",
     },
     classifiers=[
-        "Development Status :: 1 - Planning",
+        "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Security",
     ],
     entry_points={
         "console_scripts": [
             "ksm=keeper_secrets_manager_cli.__main__:main"
         ]
     }
```

