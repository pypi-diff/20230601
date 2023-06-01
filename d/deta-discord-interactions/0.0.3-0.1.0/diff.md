# Comparing `tmp/deta-discord-interactions-0.0.3.tar.gz` & `tmp/deta-discord-interactions-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deta-discord-interactions-0.0.3.tar", last modified: Sun Sep 11 15:29:21 2022, max compression
+gzip compressed data, was "deta-discord-interactions-0.1.0.tar", last modified: Thu Jun  1 01:14:19 2023, max compression
```

## Comparing `deta-discord-interactions-0.0.3.tar` & `deta-discord-interactions-0.1.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxrwxrwx   0        0        0        0 2022-09-11 15:29:21.579252 deta-discord-interactions-0.0.3/
--rw-rw-rw-   0        0        0     1096 2022-08-22 23:01:27.000000 deta-discord-interactions-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     1479 2022-09-11 15:29:21.577252 deta-discord-interactions-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      734 2022-09-11 14:49:33.000000 deta-discord-interactions-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2022-09-11 15:29:21.298254 deta-discord-interactions-0.0.3/deta_discord_interactions/
--rw-rw-rw-   0        0        0     1722 2022-08-28 00:25:18.000000 deta-discord-interactions-0.0.3/deta_discord_interactions/__init__.py
--rw-rw-rw-   0        0        0     3329 2022-08-28 00:25:18.000000 deta-discord-interactions-0.0.3/deta_discord_interactions/client.py
--rw-rw-rw-   0        0        0    19158 2022-09-04 13:54:12.000000 deta-discord-interactions-0.0.3/deta_discord_interactions/command.py
--rw-rw-rw-   0        0        0    17395 2022-08-28 23:39:20.000000 deta-discord-interactions-0.0.3/deta_discord_interactions/context.py
--rw-rw-rw-   0        0        0    24976 2022-09-09 23:25:29.000000 deta-discord-interactions-0.0.3/deta_discord_interactions/discord.py
-drwxrwxrwx   0        0        0        0 2022-09-11 15:29:21.345252 deta-discord-interactions-0.0.3/deta_discord_interactions/enums/
--rw-rw-rw-   0        0        0      199 2022-09-04 14:09:17.000000 deta-discord-interactions-0.0.3/deta_discord_interactions/enums/__init__.py
--rw-rw-rw-   0        0        0     1315 2022-09-04 14:09:10.000000 deta-discord-interactions-0.0.3/deta_discord_interactions/enums/permissions.py
--rw-rw-rw-   0        0        0      295 2022-08-28 00:25:18.000000 deta-discord-interactions-0.0.3/deta_discord_interactions/enums/response_types.py
-drwxrwxrwx   0        0        0        0 2022-09-11 15:29:21.451255 deta-discord-interactions-0.0.3/deta_discord_interactions/models/
--rw-rw-rw-   0        0        0     1721 2022-08-28 00:25:18.000000 deta-discord-interactions-0.0.3/deta_discord_interactions/models/__init__.py
--rw-rw-rw-   0        0        0     1246 2022-08-28 00:25:18.000000 deta-discord-interactions-0.0.3/deta_discord_interactions/models/attachment.py
--rw-rw-rw-   0        0        0     2637 2022-08-29 00:03:19.000000 deta-discord-interactions-0.0.3/deta_discord_interactions/models/autocomplete.py
--rw-rw-rw-   0        0        0      869 2022-08-28 00:25:18.000000 deta-discord-interactions-0.0.3/deta_discord_interactions/models/channel.py
--rw-rw-rw-   0        0        0      150 2022-08-28 00:25:18.000000 deta-discord-interactions-0.0.3/deta_discord_interactions/models/command.py
--rw-rw-rw-   0        0        0     8582 2022-09-04 20:04:00.000000 deta-discord-interactions-0.0.3/deta_discord_interactions/models/component.py
--rw-rw-rw-   0        0        0     2831 2022-08-28 00:25:18.000000 deta-discord-interactions-0.0.3/deta_discord_interactions/models/embed.py
--rw-rw-rw-   0        0        0      822 2022-08-28 00:25:18.000000 deta-discord-interactions-0.0.3/deta_discord_interactions/models/interaction.py
--rw-rw-rw-   0        0        0     8241 2022-08-31 01:32:20.000000 deta-discord-interactions-0.0.3/deta_discord_interactions/models/message.py
--rw-rw-rw-   0        0        0     2922 2022-08-28 23:58:04.000000 deta-discord-interactions-0.0.3/deta_discord_interactions/models/modal.py
--rw-rw-rw-   0        0        0     5550 2022-08-29 00:04:37.000000 deta-discord-interactions-0.0.3/deta_discord_interactions/models/option.py
--rw-rw-rw-   0        0        0     2385 2022-08-28 00:25:18.000000 deta-discord-interactions-0.0.3/deta_discord_interactions/models/permission.py
--rw-rw-rw-   0        0        0     1002 2022-08-28 00:25:18.000000 deta-discord-interactions-0.0.3/deta_discord_interactions/models/role.py
--rw-rw-rw-   0        0        0     4445 2022-09-11 15:27:05.000000 deta-discord-interactions-0.0.3/deta_discord_interactions/models/user.py
--rw-rw-rw-   0        0        0     2063 2022-09-10 00:07:04.000000 deta-discord-interactions-0.0.3/deta_discord_interactions/models/utils.py
-drwxrwxrwx   0        0        0        0 2022-09-11 15:29:21.517254 deta-discord-interactions-0.0.3/deta_discord_interactions/tests/
--rw-rw-rw-   0        0        0        0 2022-08-28 00:25:18.000000 deta-discord-interactions-0.0.3/deta_discord_interactions/tests/__init__.py
--rw-rw-rw-   0        0        0      315 2022-08-28 00:25:18.000000 deta-discord-interactions-0.0.3/deta_discord_interactions/tests/conftest.py
--rw-rw-rw-   0        0        0     1900 2022-08-28 00:25:18.000000 deta-discord-interactions-0.0.3/deta_discord_interactions/tests/test_command.py
--rw-rw-rw-   0        0        0     5005 2022-08-28 00:25:18.000000 deta-discord-interactions-0.0.3/deta_discord_interactions/tests/test_component.py
--rw-rw-rw-   0        0        0     9542 2022-08-28 00:25:18.000000 deta-discord-interactions-0.0.3/deta_discord_interactions/tests/test_context.py
--rw-rw-rw-   0        0        0     3653 2022-08-28 00:25:18.000000 deta-discord-interactions-0.0.3/deta_discord_interactions/tests/test_flask.py
--rw-rw-rw-   0        0        0     1756 2022-08-28 00:25:18.000000 deta-discord-interactions-0.0.3/deta_discord_interactions/tests/test_full_quart.py
--rw-rw-rw-   0        0        0     2946 2022-08-28 00:25:18.000000 deta-discord-interactions-0.0.3/deta_discord_interactions/tests/test_handler.py
--rw-rw-rw-   0        0        0     4064 2022-08-28 00:25:18.000000 deta-discord-interactions-0.0.3/deta_discord_interactions/tests/test_options.py
--rw-rw-rw-   0        0        0      301 2022-08-28 00:25:18.000000 deta-discord-interactions-0.0.3/deta_discord_interactions/tests/test_ping.py
--rw-rw-rw-   0        0        0     1948 2022-08-28 00:25:18.000000 deta-discord-interactions-0.0.3/deta_discord_interactions/tests/test_quart.py
--rw-rw-rw-   0        0        0     2743 2022-08-28 00:25:18.000000 deta-discord-interactions-0.0.3/deta_discord_interactions/tests/test_register.py
--rw-rw-rw-   0        0        0     2671 2022-08-28 00:25:18.000000 deta-discord-interactions-0.0.3/deta_discord_interactions/tests/test_response.py
--rw-rw-rw-   0        0        0     3042 2022-08-28 00:25:18.000000 deta-discord-interactions-0.0.3/deta_discord_interactions/tests/test_subcommand.py
-drwxrwxrwx   0        0        0        0 2022-09-11 15:29:21.521254 deta-discord-interactions-0.0.3/deta_discord_interactions/utils/
--rw-rw-rw-   0        0        0      474 2022-08-28 00:25:18.000000 deta-discord-interactions-0.0.3/deta_discord_interactions/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-11 15:29:21.565259 deta-discord-interactions-0.0.3/deta_discord_interactions/utils/database/
--rw-rw-rw-   0        0        0      438 2022-09-10 02:52:21.000000 deta-discord-interactions-0.0.3/deta_discord_interactions/utils/database/__init__.py
--rw-rw-rw-   0        0        0     5675 2022-09-10 20:34:49.000000 deta-discord-interactions-0.0.3/deta_discord_interactions/utils/database/_local_base.py
--rw-rw-rw-   0        0        0     1421 2022-08-31 00:20:16.000000 deta-discord-interactions-0.0.3/deta_discord_interactions/utils/database/adapters.py
--rw-rw-rw-   0        0        0     2164 2022-09-02 21:50:52.000000 deta-discord-interactions-0.0.3/deta_discord_interactions/utils/database/bound_dict.py
--rw-rw-rw-   0        0        0     2449 2022-08-30 02:40:14.000000 deta-discord-interactions-0.0.3/deta_discord_interactions/utils/database/bound_list.py
--rw-rw-rw-   0        0        0     1450 2022-08-29 11:18:35.000000 deta-discord-interactions-0.0.3/deta_discord_interactions/utils/database/bound_meta.py
--rw-rw-rw-   0        0        0    13310 2022-09-10 22:10:42.000000 deta-discord-interactions-0.0.3/deta_discord_interactions/utils/database/database.py
--rw-rw-rw-   0        0        0      149 2022-09-07 04:03:12.000000 deta-discord-interactions-0.0.3/deta_discord_interactions/utils/database/exceptions.py
--rw-rw-rw-   0        0        0     5461 2022-09-10 22:53:43.000000 deta-discord-interactions-0.0.3/deta_discord_interactions/utils/database/query.py
--rw-rw-rw-   0        0        0     6262 2022-09-10 21:46:53.000000 deta-discord-interactions-0.0.3/deta_discord_interactions/utils/database/record.py
-drwxrwxrwx   0        0        0        0 2022-09-11 15:29:21.575250 deta-discord-interactions-0.0.3/deta_discord_interactions/utils/oauth/
--rw-rw-rw-   0        0        0      456 2022-09-09 02:55:36.000000 deta-discord-interactions-0.0.3/deta_discord_interactions/utils/oauth/__init__.py
--rw-rw-rw-   0        0        0     9509 2022-09-11 15:22:27.000000 deta-discord-interactions-0.0.3/deta_discord_interactions/utils/oauth/model.py
--rw-rw-rw-   0        0        0     8196 2022-09-10 21:39:37.000000 deta-discord-interactions-0.0.3/deta_discord_interactions/utils/oauth/oauth.py
-drwxrwxrwx   0        0        0        0 2022-09-11 15:29:21.338264 deta-discord-interactions-0.0.3/deta_discord_interactions.egg-info/
--rw-rw-rw-   0        0        0     1479 2022-09-11 15:29:21.000000 deta-discord-interactions-0.0.3/deta_discord_interactions.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2715 2022-09-11 15:29:21.000000 deta-discord-interactions-0.0.3/deta_discord_interactions.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-11 15:29:21.000000 deta-discord-interactions-0.0.3/deta_discord_interactions.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-08-27 15:46:21.000000 deta-discord-interactions-0.0.3/deta_discord_interactions.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       39 2022-09-11 15:29:21.000000 deta-discord-interactions-0.0.3/deta_discord_interactions.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2022-09-11 15:29:21.000000 deta-discord-interactions-0.0.3/deta_discord_interactions.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      729 2022-09-11 15:28:52.000000 deta-discord-interactions-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-09-11 15:29:21.580252 deta-discord-interactions-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      983 2022-09-11 15:29:04.000000 deta-discord-interactions-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 01:14:19.851996 deta-discord-interactions-0.1.0/
+-rw-rw-rw-   0        0        0     1096 2022-08-22 23:01:27.000000 deta-discord-interactions-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     1489 2023-06-01 01:14:19.849991 deta-discord-interactions-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      746 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 01:14:19.401510 deta-discord-interactions-0.1.0/deta_discord_interactions/
+-rw-rw-rw-   0        0        0     1722 2022-08-28 00:25:18.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/__init__.py
+-rw-rw-rw-   0        0        0     5605 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/client.py
+-rw-rw-rw-   0        0        0    19166 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/command.py
+-rw-rw-rw-   0        0        0    17819 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/context.py
+-rw-rw-rw-   0        0        0    26503 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/discord.py
+drwxrwxrwx   0        0        0        0 2023-06-01 01:14:19.456840 deta-discord-interactions-0.1.0/deta_discord_interactions/enums/
+-rw-rw-rw-   0        0        0      199 2022-09-04 14:09:17.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/enums/__init__.py
+-rw-rw-rw-   0        0        0     1315 2022-09-04 14:09:10.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/enums/permissions.py
+-rw-rw-rw-   0        0        0      295 2022-08-28 00:25:18.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/enums/response_types.py
+-rw-rw-rw-   0        0        0     4339 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/http.py
+drwxrwxrwx   0        0        0        0 2023-06-01 01:14:19.523985 deta-discord-interactions-0.1.0/deta_discord_interactions/models/
+-rw-rw-rw-   0        0        0     1721 2022-08-28 00:25:18.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/models/__init__.py
+-rw-rw-rw-   0        0        0     1246 2022-08-28 00:25:18.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/models/attachment.py
+-rw-rw-rw-   0        0        0     2655 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/models/autocomplete.py
+-rw-rw-rw-   0        0        0     1387 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/models/channel.py
+-rw-rw-rw-   0        0        0      150 2022-08-28 00:25:18.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/models/command.py
+-rw-rw-rw-   0        0        0     8596 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/models/component.py
+-rw-rw-rw-   0        0        0     2806 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/models/embed.py
+-rw-rw-rw-   0        0        0      822 2022-08-28 00:25:18.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/models/interaction.py
+-rw-rw-rw-   0        0        0     8113 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/models/message.py
+-rw-rw-rw-   0        0        0     2932 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/models/modal.py
+-rw-rw-rw-   0        0        0     5550 2022-08-29 00:04:37.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/models/option.py
+-rw-rw-rw-   0        0        0     2385 2022-08-28 00:25:18.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/models/permission.py
+-rw-rw-rw-   0        0        0     1234 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/models/role.py
+-rw-rw-rw-   0        0        0     5159 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/models/user.py
+-rw-rw-rw-   0        0        0     3505 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/models/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-01 01:14:19.760570 deta-discord-interactions-0.1.0/deta_discord_interactions/tests/
+-rw-rw-rw-   0        0        0        0 2022-08-28 00:25:18.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/tests/__init__.py
+-rw-rw-rw-   0        0        0     1288 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/tests/conftest.py
+-rw-rw-rw-   0        0        0     1900 2022-08-28 00:25:18.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/tests/test_command.py
+-rw-rw-rw-   0        0        0     5026 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/tests/test_component.py
+-rw-rw-rw-   0        0        0     9573 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/tests/test_context.py
+-rw-rw-rw-   0        0        0     8984 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/tests/test_database.py
+-rw-rw-rw-   0        0        0     2991 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/tests/test_handler.py
+-rw-rw-rw-   0        0        0     3151 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/tests/test_http.py
+-rw-rw-rw-   0        0        0     2142 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/tests/test_oauth.py
+-rw-rw-rw-   0        0        0     4064 2022-08-28 00:25:18.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/tests/test_options.py
+-rw-rw-rw-   0        0        0      301 2023-03-05 07:47:55.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/tests/test_ping.py
+-rw-rw-rw-   0        0        0     1986 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/tests/test_register.py
+-rw-rw-rw-   0        0        0     2687 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/tests/test_response.py
+-rw-rw-rw-   0        0        0     3042 2022-08-28 00:25:18.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/tests/test_subcommand.py
+-rw-rw-rw-   0        0        0     1549 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/tests/test_wsgi.py
+drwxrwxrwx   0        0        0        0 2023-06-01 01:14:19.764645 deta-discord-interactions-0.1.0/deta_discord_interactions/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 01:14:19.777267 deta-discord-interactions-0.1.0/deta_discord_interactions/utils/cooldown/
+-rw-rw-rw-   0        0        0     2745 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/utils/cooldown/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 01:14:19.833987 deta-discord-interactions-0.1.0/deta_discord_interactions/utils/database/
+-rw-rw-rw-   0        0        0      400 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/utils/database/__init__.py
+-rw-rw-rw-   0        0        0     6439 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/utils/database/_local_base.py
+-rw-rw-rw-   0        0        0     1469 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/utils/database/bound_meta.py
+-rw-rw-rw-   0        0        0    17784 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/utils/database/database.py
+-rw-rw-rw-   0        0        0      468 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/utils/database/exceptions.py
+-rw-rw-rw-   0        0        0     4838 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/utils/database/query.py
+drwxrwxrwx   0        0        0        0 2023-06-01 01:14:19.846978 deta-discord-interactions-0.1.0/deta_discord_interactions/utils/oauth/
+-rw-rw-rw-   0        0        0      506 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/utils/oauth/__init__.py
+-rw-rw-rw-   0        0        0    10089 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/utils/oauth/model.py
+-rw-rw-rw-   0        0        0     9292 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/deta_discord_interactions/utils/oauth/oauth.py
+drwxrwxrwx   0        0        0        0 2023-06-01 01:14:19.444738 deta-discord-interactions-0.1.0/deta_discord_interactions.egg-info/
+-rw-rw-rw-   0        0        0     1489 2023-06-01 01:14:19.000000 deta-discord-interactions-0.1.0/deta_discord_interactions.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2630 2023-06-01 01:14:19.000000 deta-discord-interactions-0.1.0/deta_discord_interactions.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 01:14:19.000000 deta-discord-interactions-0.1.0/deta_discord_interactions.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-08-27 15:46:21.000000 deta-discord-interactions-0.1.0/deta_discord_interactions.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       39 2023-06-01 01:14:19.000000 deta-discord-interactions-0.1.0/deta_discord_interactions.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-06-01 01:14:19.000000 deta-discord-interactions-0.1.0/deta_discord_interactions.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      797 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-01 01:14:19.852995 deta-discord-interactions-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      983 2023-06-01 01:13:01.000000 deta-discord-interactions-0.1.0/setup.py
```

### Comparing `deta-discord-interactions-0.0.3/LICENSE` & `deta-discord-interactions-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deta-discord-interactions-0.0.3/PKG-INFO` & `deta-discord-interactions-0.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deta-discord-interactions
-Version: 0.0.3
+Version: 0.1.0
 Summary: A web framework for Discord interactions specialized for usage in https://deta.sh
 Home-page: https://github.com/etrotta/flask-discord-interactions/tree/deta
 Author: etrotta
 Author-email: etrotta <etrotta@duck.com>
 License: MIT
 Project-URL: Homepage, https://github.com/etrotta/flask-discord-interactions/tree/deta
 Project-URL: Bug Tracker, https://github.com/etrotta/flask-discord-interactions/issues
@@ -14,17 +14,17 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Deta-Discord-Interactions
 
-This is a small web framework that lets you write Discord Application Commands using a decorator syntax similar to Flask's `@app.route()` or Discord.py's `@bot.command()`, specialized for usage in https://deta.sh
+This is a small web framework that lets you write Discord Application Commands using a decorator syntax similar to Flask's `@app.route()` or Discord.py's `@bot.command()`, specialized for usage in https://deta.space
 
-It is a fork of [flask-discord-interactions](https://pypi.org/project/Flask-Discord-Interactions/), but without requiring Flask and with some added features to make the usage of the library simpler.
+It is a fork of [flask-discord-interactions](https://pypi.org/project/Flask-Discord-Interactions/), but without requiring Flask and with some added features to make the usage of the library better on deta.
 
 ```
 @app.command()
 def ping(ctx):
     "Respond with a friendly 'pong'!"
     return "Pong!"
 ```
```

### Comparing `deta-discord-interactions-0.0.3/README.md` & `deta-discord-interactions-0.1.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Deta-Discord-Interactions
 
-This is a small web framework that lets you write Discord Application Commands using a decorator syntax similar to Flask's `@app.route()` or Discord.py's `@bot.command()`, specialized for usage in https://deta.sh
+This is a small web framework that lets you write Discord Application Commands using a decorator syntax similar to Flask's `@app.route()` or Discord.py's `@bot.command()`, specialized for usage in https://deta.space
 
-It is a fork of [flask-discord-interactions](https://pypi.org/project/Flask-Discord-Interactions/), but without requiring Flask and with some added features to make the usage of the library simpler.
+It is a fork of [flask-discord-interactions](https://pypi.org/project/Flask-Discord-Interactions/), but without requiring Flask and with some added features to make the usage of the library better on deta.
 
 ```
 @app.command()
 def ping(ctx):
     "Respond with a friendly 'pong'!"
     return "Pong!"
 ```
 
 The documentation of the original library is available on [readthedocs](https://flask-discord-interactions.readthedocs.io/).
-The documentation of the Fork is still Work in Progress.
+The documentation of the Fork is still Work in Progress.
```

### Comparing `deta-discord-interactions-0.0.3/deta_discord_interactions/__init__.py` & `deta-discord-interactions-0.1.0/deta_discord_interactions/__init__.py`

 * *Files identical despite different names*

### Comparing `deta-discord-interactions-0.0.3/deta_discord_interactions/command.py` & `deta-discord-interactions-0.1.0/deta_discord_interactions/command.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 import enum
 import inspect
 import itertools
 
-from typing import Callable, List, Dict, TYPE_CHECKING
+from typing import Callable, TYPE_CHECKING
 
 from deta_discord_interactions.context import Context
 from deta_discord_interactions.models import (
     Message,
     Modal,
     CommandOptionType,
     ApplicationCommandType,
@@ -34,28 +34,28 @@
     Attributes
     ----------
     command: Callable
         Function to call when the command is invoked.
     name: str
         Name for this command (appears in the Discord client). If omitted,
         infers the name based on the name of the function.
-    name_localizations: Dict[str, str]
+    name_localizations: dict[str, str]
         Localization dictionary for name field.
     description: str
         Description for this command (appears in the Discord client). If
         omitted, infers the description based on the docstring of the function,
         or sets the description to "No description", if ``ApplicationCommandType``
         is ``CHAT_INPUT``, else set description to ``None``.
-    description_localizations: Dict[str, str]
+    description_localizations: dict[str, str]
         Localization dictionary for description field.
-    options: List[Option]
+    options: list[Option]
         Array of options that can be passed to this command. If omitted,
         infers the options based on the function parameters and type
         annotations.
-    annotations: Dict[str, str]
+    annotations: dict[str, str]
         Dictionary of descriptions for each option provided. Use this only if
         you want the options to be inferred from the parameters and type
         annotations. Do not use with ``options``. If omitted, and if
         ``options`` is not provided, option descriptions default to
         "No description".
     type: int
         Type for this command (depend on the action in the Discord client).
@@ -72,21 +72,21 @@
 
     def __init__(
         self,
         command: Callable,
         name: str,
         description: str,
         *,
-        options: List[Option],
-        annotations: Dict[str, str],
+        options: list[Option],
+        annotations: dict[str, str],
         type: int = ApplicationCommandType.CHAT_INPUT,
         default_member_permissions: int = None,
         dm_permission: bool = None,
-        name_localizations: Dict[str, str] = None,
-        description_localizations: Dict[str, str] = None,
+        name_localizations: dict[str, str] = None,
+        description_localizations: dict[str, str] = None,
         discord: "DiscordInteractions" = None,
         autocomplete_handler: Callable = None,
     ):
         self.command = command
         self.name = name
         self.description = description
         self.options = options
@@ -347,67 +347,67 @@
     """
     Represents a Subgroup of slash commands.
 
     Attributes
     ----------
     name: str
         The name of this subgroup, shown in the Discord client.
-    name_localizations: Dict[str, str]
+    name_localizations: dict[str, str]
         A dict of localized names for this subgroup.
     description: str
         The description of this subgroup, shown in the Discord client.
-    description_localizations: Dict[str, str]
+    description_localizations: dict[str, str]
         A dict of localized descriptions for this subgroup.
     """
 
     def __init__(
         self,
         name: str,
         description: str,
         *,
-        name_localizations: Dict[str, str] = None,
-        description_localizations: Dict[str, str] = None,
+        name_localizations: dict[str, str] = None,
+        description_localizations: dict[str, str] = None,
     ):
         self.name = name
         self.description = description
-        self.subcommands = {}
+        self.subcommands: dict[str, Command] = {}
         self.type = ApplicationCommandType.CHAT_INPUT
         self.name_localizations = name_localizations
         self.description_localizations = description_localizations
 
         self.default_member_permissions = None
         self.dm_permission = None
 
     def command(
         self,
         name: str = None,
         description: str = None,
         *,
-        name_localizations: Dict[str, str] = None,
-        description_localizations: Dict[str, str] = None,
-        options: List[Option] = None,
-        annotations: Dict[str, str] = None,
+        name_localizations: dict[str, str] = None,
+        description_localizations: dict[str, str] = None,
+        options: list[Option] = None,
+        annotations: dict[str, str] = None,
     ):
         """
         Decorator to create a new Subcommand of this Subgroup.
 
         Parameters
         ----------
         name: str
             The name of the command, as displayed in the Discord client.
-        name_localizations: Dict[str, str]
+        name_localizations: dict[str, str]
             A dict of localized names for the command.
         description: str
             The description of the command.
-        description_localizations: Dict[str, str]
+        description_localizations: dict[str, str]
             A dict of localized descriptions for the command.
-        options: List[Option]
+        options: list[Option]
             A list of options for the command, overriding the function's
             keyword arguments.
-        annotations: Dict[str, str]
+        annotations: dict[str, str]
             If ``options`` is not provided, descriptions for each of the
             options defined in the function's keyword arguments.
         """
 
         def decorator(func: Callable) -> Command:
             subcommand = Command(
                 func,
@@ -427,15 +427,15 @@
     def options(self):
         """
         Returns an array of options that can be passed to this command.
         Computed based on the options of each subcommand or subcommand group.
 
         Returns
         -------
-        List[Option]
+        list[Option]
             The options for this command.
         """
         options = []
         for command in self.subcommands.values():
             data = command.dump()
             if isinstance(command, SlashCommandSubgroup):
                 data["type"] = CommandOptionType.SUB_COMMAND_GROUP
@@ -480,19 +480,19 @@
     """
     Represents a Subgroup of slash commands.
 
     Attributes
     ----------
     name: str
         The name of this subgroup, shown in the Discord client.
-    name_localizations: Dict[str, str]
+    name_localizations: dict[str, str]
         A dict of localized names for this subgroup.
     description: str
         The description of this subgroup, shown in the Discord client.
-    description_localizations: Dict[str, str]
+    description_localizations: dict[str, str]
         A dict of localized descriptions for this subgroup.
     default_member_permissions: int
         Permission integer setting permission defaults for a command
     dm_permission: int
         Indicates whether the command can be used in DMs
     """
 
@@ -517,30 +517,30 @@
         self.description_localizations = description_localizations
 
     def subgroup(
         self,
         name: str,
         description: str = "No description",
         *,
-        name_localizations: Dict[str, str] = None,
-        description_localizations: Dict[str, str] = None,
+        name_localizations: dict[str, str] = None,
+        description_localizations: dict[str, str] = None,
     ):
         """
         Create a new :class:`SlashCommandSubroup`
         (which can contain multiple subcommands)
 
         Parameters
         ----------
         name: str
             The name of the subgroup, as displayed in the Discord client.
-        name_localizations: Dict[str, str]
+        name_localizations: dict[str, str]
             A dict of localized names for the subgroup.
         description: str
             The description of the subgroup. Defaults to "No description".
-        description_localizations: Dict[str, str]
+        description_localizations: dict[str, str]
             A dict of localized descriptions for the subgroup.
         """
 
         group = SlashCommandSubgroup(
             name,
             description,
             name_localizations=name_localizations,
```

### Comparing `deta-discord-interactions-0.0.3/deta_discord_interactions/context.py` & `deta-discord-interactions-0.1.0/deta_discord_interactions/context.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass
-from typing import Callable, List, Optional, Union, TYPE_CHECKING
+from typing import Callable, Optional, Union, TYPE_CHECKING
 import inspect
 import itertools
 
 import requests
 
 from deta_discord_interactions.models import (
     LoadableDataclass,
@@ -63,69 +63,70 @@
     members
         :class:`Member` objects for each user specified as an option, if this
         command was invoked in a guild.
     channels
         :class:`Channel` objects for each channel specified as an option.
     roles
         :class:`Role` object for each role specified as an option.
-    target
-        The targeted :class:`User` or message.
+    target_user
+        The targeted :class:`User` if it is a User context menu command.
+    target_message
+        The targeted :class:`Message` if it is a Message context menu command.
     message
         The message that the invoked components are attached to.
         Only available on component interactions.
     locale
         The selected language of the invoking user.
     guild_locale
         The guild's preferred locale, if invoked in a guild.
     app_permissions
         Bitwise set of permissions the app or bot has within the channel the interaction was sent from.
     """
-
-    author: Union[Member, User] = None
+    author: Optional[User] = None
     id: str = None
     type: int = None
     command_type: int = None
     token: str = None
     channel_id: str = None
     guild_id: str = None
     options: list = None
     values: list = None
     components: list = None
     resolved: dict = None
     command_name: str = None
     command_id: str = None
-    members: List[Member] = None
-    channels: List[Channel] = None
-    roles: List[Role] = None
-    message: Message = None
+    members: Optional[list[Member]] = None
+    channels: Optional[list[Channel]] = None
+    roles: Optional[list[Role]] = None
+    message: Optional[Message] = None
     locale: Optional[str] = None
     guild_locale: Optional[str] = None
     app_permissions: Optional[str] = None
-    discord: "DiscordInteractions" = None
+    discord: Optional["DiscordInteractions"] = None
 
     custom_id: str = None
     primary_id: str = None
     handler_state: list = None
 
     target_id: str = None
-    target: Union[User, Message] = None
+    target_user: Optional[User] = None
+    target_message: Optional[Message] = None
 
     @classmethod
     def from_data(
         cls, discord: "DiscordInteractions" = None, data = None
     ):
         if data is None:
             data = {}
 
         result = cls(
             discord=discord,
             id=data.get("id"),
             type=data.get("type"),
-            command_type=data.get("data", {}).get("type")
-            or ApplicationCommandType.CHAT_INPUT,
+            command_type=data.get("data", {}).get("type") or ApplicationCommandType.CHAT_INPUT,
             token=data.get("token"),
             channel_id=data.get("channel_id"),
             guild_id=data.get("guild_id"),
             options=data.get("data", {}).get("options"),
             values=data.get("data", {}).get("values", []),
             components=data.get("data", {}).get("components", []),
             resolved=data.get("data", {}).get("resolved", {}),
@@ -237,40 +238,43 @@
         }
 
     def parse_target(self):
         """
         Parse the target of the incoming interaction.
 
         For User and Message commands, the target is the relevant user or
-        message. This method sets the `ctx.target` field.
+        message. This method sets the `ctx.target_user` or `ctx.target_message` field.
         """
         if self.command_type == ApplicationCommandType.USER:
             if self.target_id in self.members:
-                self.target = self.members[self.target_id]
+                self.target_user = self.members[self.target_id]
             else:
-                self.target = self.users[self.target_id]
+                self.target_user = self.users[self.target_id]
         elif self.command_type == ApplicationCommandType.MESSAGE:
-            self.target = self.messages[self.target_id]
-        else:
-            self.target = None
+            self.target_message = self.messages[self.target_id]
+
+    @property
+    def target(self) -> Union[Message, User, None]:
+        "Returns the target of this context"  # Partially for backwards compatibility
+        return self.target_message or self.target_user
 
     def parse_components(self):
         self.components = [Component.from_dict(c) for c in self.components]
 
     def create_args(self):
         """
         Create the arguments which will be passed to the function when the
         :class:`Command` is invoked.
         """
         if self.command_type == ApplicationCommandType.CHAT_INPUT:
             return self.create_args_chat_input()
         elif self.command_type == ApplicationCommandType.USER:
-            return [self.target], {}
+            return [self.target_user], {}
         elif self.command_type == ApplicationCommandType.MESSAGE:
-            return [self.target], {}
+            return [self.target_message], {}
 
     def create_autocomplete_args(self):
         """
         Create the arguments which will be passed to the function when the
         :class:`Command` autocomplete handler is invoked.
         """
         if self.command_type == ApplicationCommandType.CHAT_INPUT:
@@ -290,15 +294,14 @@
             kwargs = {}
 
             for option in data["options"]:
                 if option["type"] in [
                     CommandOptionType.SUB_COMMAND,
                     CommandOptionType.SUB_COMMAND_GROUP,
                 ]:
-
                     args.append(option["name"])
 
                     sub_args, sub_kwargs = create_args_recursive(option, resolved)
 
                     args += sub_args
                     kwargs.update(sub_kwargs)
```

### Comparing `deta-discord-interactions-0.0.3/deta_discord_interactions/discord.py` & `deta-discord-interactions-0.1.0/deta_discord_interactions/discord.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import time
-from typing import Callable, Dict, List, NoReturn
+from typing import Callable, NoReturn
 import json
 
 import requests
 
 from nacl.exceptions import BadSignatureError
 from nacl.signing import VerifyKey
 
@@ -17,15 +17,15 @@
 
 class AbortError(Exception):
     def __init__(self, http_code):
         self.http_code = http_code
 
 class PongResponse:
     def encode(self):
-        return json.dumps({"type": ResponseType.PONG}), "application/json"
+        return json.dumps({"type": ResponseType.PONG}).encode('UTF-8'), "application/json"
 
 
 class InteractionType:
     PING = 1
     APPLICATION_COMMAND = 2
     MESSAGE_COMPONENT = 3
     APPLICATION_COMMAND_AUTOCOMPLETE = 4
@@ -36,51 +36,51 @@
     """
     Represents a collection of :class:`ApplicationCommand` s.
 
     Useful for splitting a bot across multiple files.
     """
 
     def __init__(self):
-        self.discord_commands = {}
-        self.custom_id_handlers = {}
-        self.tasks = []
+        self.discord_commands: dict[str, Command] = {}
+        self.custom_id_handlers: dict[str, Callable] = {}
+        self.deta_actions: dict[str, Callable] = {}
 
     def add_command(
         self,
         command: Callable,
         name: str = None,
         description: str = None,
         *,
-        options: List[Option] = None,
-        annotations: Dict[str, str] = None,
+        options: list[Option] = None,
+        annotations: dict[str, str] = None,
         type: int = ApplicationCommandType.CHAT_INPUT,
         default_member_permissions: int = None,
         dm_permission: bool = None,
-        name_localizations: Dict[str, str] = None,
-        description_localizations: Dict[str, str] = None,
+        name_localizations: dict[str, str] = None,
+        description_localizations: dict[str, str] = None,
     ):
         """
         Create and add a new :class:`ApplicationCommand`.
 
         Parameters
         ----------
         command: Callable
             Function to execute when the command is run.
         name: str
             The name of the command, as displayed in the Discord client.
-        name_localizations: Dict[str, str]
+        name_localizations: dict[str, str]
             A dictionary of localizations for the name of the command.
         description: str
             The description of the command.
-        description_localizations: Dict[str, str]
+        description_localizations: dict[str, str]
             A dictionary of localizations for the description of the command.
-        options: List[Option]
+        options: list[Option]
             A list of options for the command, overriding the function's
             keyword arguments.
-        annotations: Dict[str, str]
+        annotations: dict[str, str]
             If ``options`` is not provided, descriptions for each of the
             options defined in the function's keyword arguments.
         type: int
             The class:`.ApplicationCommandType` of the command.
         default_member_permissions: int
             A permission integer defining the required permissions a user must have to run the command.
         dm_permission: bool
@@ -103,39 +103,39 @@
         return command
 
     def command(
         self,
         name: str = None,
         description: str = None,
         *,
-        options: List[Option] = None,
-        annotations: Dict[str, str] = None,
+        options: list[Option] = None,
+        annotations: dict[str, str] = None,
         type: int = ApplicationCommandType.CHAT_INPUT,
         default_member_permissions: int = None,
         dm_permission: bool = None,
-        name_localizations: Dict[str, str] = None,
-        description_localizations: Dict[str, str] = None,
+        name_localizations: dict[str, str] = None,
+        description_localizations: dict[str, str] = None,
     ) -> Callable[[Callable], Command]:
         """
         Decorator to create a new :class:`Command`.
 
         Parameters
         ----------
         name: str
             The name of the command, as displayed in the Discord client.
-        name_localizations: Dict[str, str]
+        name_localizations: dict[str, str]
             A dictionary of localizations for the name of the command.
         description: str
             The description of the command.
-        description_localizations: Dict[str, str]
+        description_localizations: dict[str, str]
             A dictionary of localizations for the description of the command.
-        options: List[Option]
+        options: list[Option]
             A list of options for the command, overriding the function's
             keyword arguments.
-        annotations: Dict[str, str]
+        annotations: dict[str, str]
             If ``options`` is not provided, descriptions for each of the
             options defined in the function's keyword arguments.
         type: int
             The ``ApplicationCommandType`` of the command.
         default_member_permissions: int
             A permission integer defining the required permissions a user must have to run the command
         dm_permission: bool
@@ -160,47 +160,47 @@
                 name_localizations=name_localizations,
                 description_localizations=description_localizations,
             )
             return command
 
         return decorator
 
-    def task(self):
+    def action(self, action_id: str):
         """
-        Decorator to add a new Task.
-        The Micro must be set to run on CRON for them to run at all.
+        Decorator to add a new Deta (Scheduled) Action.
+        You must remember to register it in the Spacefile for it to run.
         """
         def decorator(func):
-            self.tasks.append(func)
+            self.deta_actions[action_id] = func
             return func
         return decorator
 
     def command_group(
         self,
         name: str,
         description: str = "No description",
         *,
         default_member_permissions: int = None,
         dm_permission: bool = None,
-        name_localizations: Dict[str, str] = None,
-        description_localizations: Dict[str, str] = None,
+        name_localizations: dict[str, str] = None,
+        description_localizations: dict[str, str] = None,
     ):
         """
         Create a new :class:`SlashCommandGroup`
         (which can contain multiple subcommands)
 
         Parameters
         ----------
         name: str
             The name of the command group, as displayed in the Discord client.
-        name_localizations: Dict[str, str]
+        name_localizations: dict[str, str]
             A dictionary of localizations for the name of the command group.
         description: str
             The description of the command group.
-        description_localizations: Dict[str, str]
+        description_localizations: dict[str, str]
             A dictionary of localizations for the description of the command group.
         default_member_permissions: int
             A permission integer defining the required permissions a user must have to run the command
         dm_permission: bool
             Indicates whether the command can be used in DMs
 
         Returns
@@ -278,17 +278,14 @@
             self.discord_client_secret = os.environ["DISCORD_CLIENT_SECRET"]
             self.discord_scope = os.getenv("DISCORD_SCOPE", "applications.commands.update")
             self.DONT_REGISTER_WITH_DISCORD = os.getenv("DONT_REGISTER_WITH_DISCORD", False)
             self.DONT_VALIDATE_SIGNATURE = os.getenv("DONT_VALIDATE_SIGNATURE", False)
         except KeyError:
             raise Exception("Please fill in the .env files with your application's credentials.")
         self.__routes = {}
-        # For Deta Micro CRON
-        self._deta_type = "probably_wsgi"
-        self.lib = self.run_tasks
 
     def fetch_token(self):
         """
         Fetch an OAuth2 token from Discord using the ``CLIENT_ID`` and
         ``CLIENT_SECRET`` with the ``applications.commands.update`` scope. This
         can be used to register new application commands.
         """
@@ -324,34 +321,37 @@
     def auth_headers(self):
         """
         Get the Authorization header required for HTTP requests to the
         Discord API.
 
         Returns
         -------
-        Dict[str, str]
+        dict[str, str]
             The Authorization header.
         """
-
         if self.discord_token is None or time.time() > self.discord_token["expires_on"]:
             self.discord_token = self.fetch_token()
         return {"Authorization": f"Bearer {self.discord_token['access_token']}"}
 
-    def update_commands(self, guild_id: str = None):
+    def update_commands(self, guild_id: str = None, *, from_inside_a_micro: bool = False):
         """
         Update the list of commands registered with Discord.
         This method will overwrite all existing commands.
 
         Parameters
         ----------
         guild_id: str
             The ID of the Discord guild to register commands to. If omitted,
             the commands are registered globally.
+        from_inside_a_micro: bool
+            If you really want to update the commands from inside the micro, set this to True.
+            I would strongly advise against it though - at least, do not run this *every time* but from a specific command or route
         """
-        if os.getenv("DETA_RUNTIME") is not None:  # It *would* work, it's just a big waste and may slow down the bot overall
+        # It *would* work, it's just a big waste and may slow down the bot overall
+        if (os.getenv("DETA_SPACE_APP") is not None) and (from_inside_a_micro == False):
             raise Exception("Cannot register commands from inside a Deta Micro")
 
         if guild_id:
             url = (
                 f"{self.DISCORD_BASE_URL}/applications/"
                 f"{self.discord_client_id}/"
                 f"guilds/{guild_id}/commands"
@@ -425,15 +425,15 @@
         guild_id: str
             The ID of the guild to retrieve permissions from.
         command_id: str
             The ID of the command to retrieve permissions for.
 
         Returns
         -------
-        List[Permission]
+        list[Permission]
             A list of permission overwrites for the given command.
         """
 
         url = self.build_permission_overwrite_url(
             command,
             guild_id=guild_id,
             command_id=command_id,
@@ -445,15 +445,15 @@
         )
         response.raise_for_status()
 
         return [Permission.from_dict(perm) for perm in response.json()]
 
     def set_permission_overwrites(
         self,
-        permissions: List[Permission],
+        permissions: list[Permission],
         command: Command = None,
         *,
         guild_id: str,
         command_id: str = None,
     ):
         """
         Overwrite the list of permission overwrites in a specific guild for a
@@ -494,15 +494,15 @@
         ----------
         blueprint: DiscordInteractionsBlueprint
             The :class:`DiscordInteractionsBlueprint` to add
             :class:`Command` s from.
         """
         self.discord_commands.update(blueprint.discord_commands)
         self.custom_id_handlers.update(blueprint.custom_id_handlers)
-        self.tasks.extend(blueprint.tasks)
+        self.deta_actions.update(blueprint.deta_actions)
 
     def run_command(self, data: dict):
         """
         Run the corresponding :class:`Command` given incoming interaction
         data.
 
         Parameters
@@ -572,22 +572,21 @@
 
         command_name = data["data"]["name"]
 
         command = self.discord_commands[command_name]
 
         return command.make_context_and_run_autocomplete(discord=self, data=data)
 
-    def run_tasks(self, event):
-        """Runs all registered Tasks. 
-        If there are more than one registerd tasks, they may run asynchronously and out of order."""
-        from concurrent.futures import ThreadPoolExecutor
-        with ThreadPoolExecutor() as executor:
-            for task in self.tasks:
-                executor.submit(task)
-
+    def run_deta_action(self, event: dict[str, str]):
+        """Runs registered Deta Actions"""
+        action = self.deta_actions.get(event.get("id"))
+        if action is None:
+            self.abort(400, f"Deta event tried to run an unregistered action: {event!r}")
+        else:
+            return action(event)
 
     def verify_signature(self, request):
         """
         Verify the signature sent by Discord with incoming interactions.
 
         Parameters
         ----------
@@ -666,50 +665,74 @@
             return ['Hello World!'.encode('UTF-8')]
         """
         def decorator(function):
             self.__routes[route_path] = function
             return function
         return decorator
 
-    def __call__(self, environ, start_response):
+    def __call__(self, environ: dict, start_response: Callable):
         """
         Handles incoming interaction data
         (WSGI)
         """
         try:
             data = environ.copy()
             raw_data = environ["wsgi.input"].read()
             if raw_data:
                 data["json"] = json.loads(raw_data.decode("UTF-8"))
                 data["raw_data"] = raw_data
 
-            data["path"] = data.get("PATH_INFO", '') or '/'
+            data["path"] = data.get("PATH_INFO", '').split("?", 1)[0] or '/'
+
 
             if data["QUERY_STRING"]:
                 data["query_dict"] = dict(args.split('=', 1) for args in data["QUERY_STRING"].split("&"))
-
+            else:
+                data["query_dict"] = {}
+            ### Handle Discord
             if data['path'] == '/discord':
                 result = self.handle_interaction(data)
                 response, mimetype = result.encode()
                 status = "200 OK"
                 response_headers = [("Content-Type", mimetype)]
                 start_response(status, response_headers)
-                return [response.encode("UTF-8")]
-            elif (  # If you set it like `https://example.deta.dev` instead of `https://example.deta.dev/discord`
+                return [response]
+            ### Catch a common mistake
+            elif (  # If you set it like `https://example.deta.app` instead of `https://example.deta.app/discord`
                 data['path'] == '/' 
                 and '/' not in self.__routes 
                 and "Discord-Interactions" in data.get("HTTP_USER_AGENT")
                 and self.verify_signature(data)
             ):
                 raise Exception("Please set the path to `.../discord` on the Developer Portal, not just the Micro URL")
-            elif data['path'] not in self.__routes:
-                self.abort(404, 'Page not found')
-            else:
+            ### Deta special routes
+            elif data['path'] == "/__space/v0/actions":
+                event = data.get("json", {}).get("event")
+                if event is None:
+                    self.abort(400, 'Malformated deta space event')
+                result = self.run_deta_action(event)
+                if result:
+                    start_response("200 OK", [("Content-Type", "application/json")])
+                    return [json.dumps({"result": result}).encode("UTF-8")]
+                else:
+                    start_response('200 OK', [])
+                    return []
+            ### User defined routes (including Utils such as oauth)
+            elif data['path'] in self.__routes:
                 return self.__routes[data['path']](data, start_response, self.abort)
+            ### Unexpected route
+            else:
+                self.abort(404, 'Page not found')
         except AbortError as err:
             status = err.http_code
             response_headers = [("Content-Type", "application/json")]
             start_response(status, response_headers)
             return [json.dumps({"error": status}).encode("UTF-8")]
+        except Exception as err:
+            import traceback
+            traceback.print_exc()
+            print(f"Unexpected error: {err}", flush=True)
+            start_response('500 Internal Server Error', [("Content-Type", "application/json")])
+            return [json.dumps({"error": str(type(err))}).encode("UTF-8")]
 
     def abort(self, code: int, reason: str) -> NoReturn:
         raise AbortError(f"{code} {reason}")
```

### Comparing `deta-discord-interactions-0.0.3/deta_discord_interactions/enums/permissions.py` & `deta-discord-interactions-0.1.0/deta_discord_interactions/enums/permissions.py`

 * *Files identical despite different names*

### Comparing `deta-discord-interactions-0.0.3/deta_discord_interactions/models/__init__.py` & `deta-discord-interactions-0.1.0/deta_discord_interactions/models/__init__.py`

 * *Files identical despite different names*

### Comparing `deta-discord-interactions-0.0.3/deta_discord_interactions/models/attachment.py` & `deta-discord-interactions-0.1.0/deta_discord_interactions/models/attachment.py`

 * *Files identical despite different names*

### Comparing `deta-discord-interactions-0.0.3/deta_discord_interactions/models/autocomplete.py` & `deta-discord-interactions-0.1.0/deta_discord_interactions/models/autocomplete.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,25 +42,25 @@
 
     def encode(self):
         """
         Return this result as a complete interaction response.
 
         Returns
         -------
-        str
+        bytes
             The encoded JSON object.
         str
             The mimetype of the response (``application/json``).
         """
         data = {
             "type": ResponseType.APPLICATION_COMMAND_AUTOCOMPLETE_RESULT,
             "data": {"choices": self.choices},
         }
 
-        return json.dumps(data), "application/json"
+        return json.dumps(data).encode("UTF-8"), "application/json"
 
     @classmethod
     def from_return_value(cls, value: Union[dict, list, "AutocompleteResult"]):
         """
         Converts the return value of an autocomplete handler to an
         AutocompleteResult.
```

### Comparing `deta-discord-interactions-0.0.3/deta_discord_interactions/models/component.py` & `deta-discord-interactions-0.1.0/deta_discord_interactions/models/component.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass, asdict
-from typing import List, Union
+from typing import Optional, Union
 
 
 class ComponentType:
     ACTION_ROW = 1
     BUTTON = 2
     SELECT_MENU = 3
     TEXT_INPUT = 4
@@ -42,20 +42,20 @@
 @dataclass
 class CustomIdComponent(Component):
     """
     Represents a Message Component with a Custom ID.
 
     Parameters
     ----------
-    custom_id: str | List
+    custom_id: str | list
         The custom ID of the component. Strings represent a single ID, lists
         take advantage of newlines to store state alongside the ID.
     """
 
-    custom_id: Union[str, List] = None
+    custom_id: Union[str, list] = None
 
     def __post_init__(self):
         if isinstance(self.custom_id, list) or isinstance(self.custom_id, tuple):
             self.custom_id = "\n".join(str(item) for item in self.custom_id)
 
         if self.custom_id and len(self.custom_id) > 100:
             raise ValueError("custom_id has maximum 100 characters")
@@ -64,22 +64,22 @@
 @dataclass
 class ActionRow(Component):
     """
     Represents an ActionRow message component.
 
     Parameters
     ----------
-    components: List[Component]
+    components: list[Component]
         The message components to display in the action row.
         Limited to any of the following:
         - 5 Buttons
         - 1 Select Menu
     """
 
-    components: List[CustomIdComponent] = None
+    components: list[CustomIdComponent] = None
 
     type: int = ComponentType.ACTION_ROW
 
     @staticmethod
     def from_dict(data):
         components = [
             Component.from_dict(component) for component in data.get("components", [])
@@ -190,35 +190,35 @@
 @dataclass
 class SelectMenu(CustomIdComponent):
     """
     Represents a SelectMenu message component.
 
     Parameters
     ----------
-    options: List[SelectMenuOption]
+    options: list[SelectMenuOption]
         The options to display in the select menu.
     placeholder: str
         The placeholder displayed when the select menu is empty.
     min_values: int
         The minimum number of options that must be selected.
     max_values: int
         The maximum number of options that can be selected.
     disabled: bool
         Whether the select menu is disabled.
     values: list
         Selected options. Only present when receiving components from a modal.
     """
 
-    options: List[SelectMenuOption] = None
+    options: list[SelectMenuOption] = None
 
     placeholder: str = None
     min_values: int = 1
     max_values: int = 1
     disabled: bool = False
-    values: list = None
+    values: Optional[list] = None
 
     type: int = ComponentType.SELECT_MENU
 
     def __post_init__(self):
         super().__post_init__()
 
         if self.options and len(self.options) > 25:
```

### Comparing `deta-discord-interactions-0.0.3/deta_discord_interactions/models/embed.py` & `deta-discord-interactions-0.1.0/deta_discord_interactions/models/embed.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from dataclasses import dataclass, asdict
-from typing import List
 
 from deta_discord_interactions.models.utils import LoadableDataclass
 
 
 @dataclass
 class Footer(LoadableDataclass):
     "Represents the footer of an Embed."
@@ -86,15 +85,15 @@
     color: int = None
     footer: Footer = None
     image: Media = None
     thumbnail: Media = None
     video: Media = None
     provider: Provider = None
     author: Author = None
-    fields: List[Field] = None
+    fields: list[Field] = None
 
     def dump(self):
         """
         Returns this Embed as a dictionary, removing fields which are None.
 
         Returns
         -------
```

### Comparing `deta-discord-interactions-0.0.3/deta_discord_interactions/models/interaction.py` & `deta-discord-interactions-0.1.0/deta_discord_interactions/models/interaction.py`

 * *Files identical despite different names*

### Comparing `deta-discord-interactions-0.0.3/deta_discord_interactions/models/message.py` & `deta-discord-interactions-0.1.0/deta_discord_interactions/models/message.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import dataclasses
 import json
-from typing import List, Union
+from typing import Optional
 from datetime import datetime
 
 import requests_toolbelt
 
 from deta_discord_interactions.enums import ResponseType
 
 from deta_discord_interactions.models.utils import LoadableDataclass
@@ -57,51 +57,48 @@
         A list of files to attach to the message. Specify just one of
         ``file`` or ``files``. Only valid for outgoing webhooks.
     components
         An array of :class:`.Component` objects representing message
         components.
     """
 
-    content: str = None
+    content: Optional[str] = None
     tts: bool = False
-    embed: Union[Embed, dict] = None
-    embeds: List[Union[Embed, dict]] = None
+    embed: Embed = None
+    embeds: list[Embed] = None
     allowed_mentions: dict = dataclasses.field(
         default_factory=lambda: {"parse": ["roles", "users", "everyone"]}
     )
     deferred: bool = False
     ephemeral: bool = False
     update: bool = False
-    file: tuple = None
-    files: List[tuple] = None
-    components: List[Component] = None
+    file: Optional[tuple] = None
+    files: Optional[list[tuple]] = None
+    components: Optional[list[Component]] = None
 
     # These fields are only set on incoming messages
-    id: str = None
-    channel_id: str = None
-    timestamp: datetime = None
-    edited_timestamp: datetime = None
-    author: Member = None
-    interaction: MessageInteraction = None
+    id: Optional[str] = None
+    channel_id: Optional[str] = None
+    timestamp: Optional[datetime] = None
+    edited_timestamp: Optional[datetime] = None
+    author: Optional[Member] = None
+    interaction: Optional[MessageInteraction] = None
 
     def __post_init__(self):
-        if self.embed is not None and self.embeds is not None:
+        if self.embed and self.embeds:
             raise ValueError("Specify only one of embed or embeds")
-        if self.embed is not None:
+        if self.embed:
             self.embeds = [self.embed]
 
-        if self.file is not None and self.files is not None:
+        if self.file and self.files:
             raise ValueError("Specify only one of file or files")
-        if self.file is not None:
+        if self.file:
             self.files = [self.file]
 
-        if self.ephemeral and self.files is not None:
-            raise ValueError("Ephemeral Messages cannot include files.")
-
-        if self.embeds is not None:
+        if self.embeds:
             for i, embed in enumerate(self.embeds):
                 if not dataclasses.is_dataclass(embed):
                     self.embeds[i] = Embed.from_dict(embed)
 
         if self.update:
             if self.deferred:
                 self.response_type = ResponseType.DEFERRED_UPDATE_MESSAGE
@@ -140,36 +137,36 @@
 
     def dump_embeds(self):
         """
         Returns the embeds of this Message as a list of dicts.
 
         Returns
         -------
-        List[dict]
+        list[dict]
             A list of dicts representing the embeds.
         """
         return (
             [embed.dump() for embed in self.embeds] if self.embeds is not None else None
         )
 
     def dump_components(self):
         """
         Returns the message components as a list of dicts.
 
         Returns
         -------
-        List[dict]
+        list[dict]
             A list of dicts representing the components.
         """
         return (
             [c.dump() for c in self.components] if self.components is not None else None
         )
 
     @classmethod
-    def from_return_value(cls, result):
+    def from_return_value(cls, result) -> 'Message':
         """
         Convert a function return value into a Message object.
         Converts ``None`` to an empty Message, or any other type to ``str``
         as message content.
 
         Parameters
         ----------
@@ -203,16 +200,16 @@
         followup: bool
             Whether this is a followup message.
         **extra: str
             Extra fields to include in the payload, mainly for Webhooks
 
         Returns
         -------
-        string
-            A string containing the message data (either JSON or multipart).
+        bytes
+            Bytes containing the message data (either JSON or multipart).
         string
             The mimetype of the message data.
         """
 
         payload = {
             "content": self.content,
             "tts": self.tts,
@@ -239,10 +236,10 @@
             for i, file in enumerate(self.files):
                 fields.append((f"files[{i}]", file))
 
             multipart = requests_toolbelt.MultipartEncoder(
                 fields=fields,
             )
 
-            return (multipart.to_string().decode(), multipart.content_type)
+            return (multipart.to_string(), multipart.content_type)
         else:
-            return (payload_json, "application/json")
+            return (payload_json.encode('UTF-8'), "application/json")
```

### Comparing `deta-discord-interactions-0.0.3/deta_discord_interactions/models/modal.py` & `deta-discord-interactions-0.1.0/deta_discord_interactions/models/modal.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 
 from dataclasses import dataclass
-from typing import List, Union
+from typing import Union
 
 from deta_discord_interactions.models.utils import LoadableDataclass
 from deta_discord_interactions.models.component import Component, ComponentType
 from deta_discord_interactions.enums import ResponseType
 
 
 @dataclass
@@ -22,15 +22,15 @@
     components
         A list of :class:`ActionRow` objects representing the rows of the form.
         Must have at least 1 row, at most 5 rows.
     """
 
     custom_id: Union[str, list] = None
     title: str = None
-    components: List[Component] = None
+    components: list[Component] = None
 
     def __post_init__(self):
         # Verify Custom ID
         if self.custom_id is None:
             raise ValueError("Modals require a custom_id")
 
         if isinstance(self.custom_id, list) or isinstance(self.custom_id, tuple):
@@ -59,15 +59,15 @@
 
     def dump_components(self):
         """
         Returns the message components as a list of dicts.
 
         Returns
         -------
-        List[dict]
+        list[dict]
             The message components as a list of dicts.
         """
         return [c.dump() for c in self.components]
 
     def encode(self, followup: bool = False):
         """
         Return this ``Modal`` as a dict to be sent in response to an
@@ -90,8 +90,8 @@
             "data": {
                 "custom_id": self.custom_id,
                 "title": self.title,
                 "components": self.dump_components(),
             },
         }
 
-        return (json.dumps(payload), "application/json")
+        return (json.dumps(payload).encode("UTF-8"), "application/json")
```

### Comparing `deta-discord-interactions-0.0.3/deta_discord_interactions/models/option.py` & `deta-discord-interactions-0.1.0/deta_discord_interactions/models/option.py`

 * *Files identical despite different names*

### Comparing `deta-discord-interactions-0.0.3/deta_discord_interactions/models/permission.py` & `deta-discord-interactions-0.1.0/deta_discord_interactions/models/permission.py`

 * *Files identical despite different names*

### Comparing `deta-discord-interactions-0.0.3/deta_discord_interactions/models/role.py` & `deta-discord-interactions-0.1.0/deta_discord_interactions/models/role.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import dataclasses
+from typing import Optional
 
 from deta_discord_interactions.models.utils import LoadableDataclass
 
 
 @dataclasses.dataclass
 class Role(LoadableDataclass):
     """
@@ -24,17 +25,23 @@
         The permissions integer of the role.
     managed
         Whether the role is managed by an integration (bot).
     mentionable
         Whether the role can be mentioned by all users.
     tags
         Miscellaneous information about the role.
+    icon
+        Hash of the role's icon
+    unicode_emoji
+        Unicode emoji of the role (alternative to icons)
     """
 
     id: str = None
     name: str = None
     color: str = None
     hoist: bool = None
     position: int = None
     managed: bool = None
     mentionable: bool = None
-    tags: dict = None
+    tags: Optional[dict] = None
+    icon: Optional[str] = None
+    unicode_emoji: Optional[str] = None
```

### Comparing `deta-discord-interactions-0.0.3/deta_discord_interactions/models/user.py` & `deta-discord-interactions-0.1.0/deta_discord_interactions/models/user.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import dataclasses
+from datetime import datetime
+from typing import Optional
 
 from deta_discord_interactions.models.utils import LoadableDataclass
 
 
 @dataclasses.dataclass
 class User(LoadableDataclass):
     """
@@ -55,15 +57,15 @@
     # banner_color: str = None
     # accent_color: str = None
     locale: str = None
     verified: bool = None  # Only available via OAuth with email scope
     email: str = None  # Only available via OAuth with email scope
     flags: int = None
     premium_type: int = None
-    public_flags: int = None
+    public_flags: Optional[int] = None
 
     @classmethod
     def from_dict(cls, data):
         data = {**data, **data.get("user", {})}
         data["avatar_hash"] = data.get("avatar")
         return super().from_dict(data)
 
@@ -121,28 +123,37 @@
         The permissions integer of the user.
     deaf
         Whether the user has been server deafened.
     mute
         Whether the user has been server muted.
     pending
         Whether the user has passed the membership requirements of a guild.
+    communication_disabled_until
+        Timestamp when the member's timeout will expire (if existing)
     """
 
-    nick: str = None
-    roles: list = None
-    joined_at: str = None
-    premium_since: str = None
-    permissions: int = None
-    deaf: bool = None
-    mute: bool = None
-    pending: bool = None
+    pending: Optional[bool] = None
+    nick: Optional[str] = None
+    roles: Optional[list[str]] = None
+    permissions: Optional[int] = None
+    deaf: bool = False
+    mute: bool = False
+    joined_at: datetime = None
+    premium_since: Optional[datetime] = None
+    communication_disabled_until: Optional[datetime] = None
 
     def __post_init__(self):
         if isinstance(self.permissions, str):
             self.permissions = int(self.permissions)
+        if isinstance(self.joined_at, str):
+            self.joined_at = datetime.fromisoformat(self.joined_at)
+        if isinstance(self.premium_since, str):
+            self.premium_since = datetime.fromisoformat(self.premium_since)
+        if isinstance(self.communication_disabled_until, str):
+            self.communication_disabled_until = datetime.fromisoformat(self.communication_disabled_until)
 
     @property
     def display_name(self):
         """
         The displayed name of the user (their nickname, or if none exists,
         their username).
```

### Comparing `deta-discord-interactions-0.0.3/deta_discord_interactions/tests/test_command.py` & `deta-discord-interactions-0.1.0/deta_discord_interactions/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `deta-discord-interactions-0.0.3/deta_discord_interactions/tests/test_component.py` & `deta-discord-interactions-0.1.0/deta_discord_interactions/tests/test_component.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,20 +9,20 @@
     ButtonStyles,
     SelectMenu,
     SelectMenuOption,
 )
 
 
 def test_parse_arguments(discord, client):
-    @discord.custom_handler()
+    @discord.custom_handler('test_handler')
     def handler(ctx, string_arg, int_arg: int):
         return f"String: {string_arg}, type(int_arg): {type(int_arg)}"
 
     assert (
-        client.run_handler(handler, "hello!", "42").content
+        client.run_handler('test_handler', "hello!", "42").content
         == "String: hello!, type(int_arg): <class 'int'>"
     )
 
 
 def test_action_row(discord, client):
     @discord.command()
     def action_row(ctx):
```

### Comparing `deta-discord-interactions-0.0.3/deta_discord_interactions/tests/test_context.py` & `deta-discord-interactions-0.1.0/deta_discord_interactions/tests/test_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,15 +159,15 @@
             "version": 1
         }
     """
     )
 
     context = Context.from_data(data=data)
 
-    assert context.target.id == "809850198683418695"
+    assert context.target_user.id == "809850198683418695"
     assert context.target.display_name == "VoltyDemo"
 
 
 def test_message_command_context_parsing():
     # Test data taken from
     # https://discord.com/developers/docs/interactions/application-commands#message-commands-example-interaction
 
@@ -236,29 +236,29 @@
             "version": 1
         }
     """
     )
 
     context = Context.from_data(data=data)
 
-    assert context.target.id == "867793854505943041"
-    assert context.target.content == "some message"
+    assert context.target_message.id == "867793854505943041"
+    assert context.target_message.content == "some message"
     assert context.target.timestamp.day == 22
     assert context.target.author.display_name == "ian"
 
 
 def test_user_command_argument(discord, client):
-    @discord.command(type=ApplicationCommandType.MESSAGE)
+    @discord.command(type=ApplicationCommandType.USER)
     def greet(ctx, target):
         return f"Hello, {target.display_name}!"
 
-    with client.context(Context(target=Member(username="Test User"))):
+    with client.context(Context(target_user=Member(username="Test User"))):
         assert client.run("greet").content == "Hello, Test User!"
 
 
 def test_message_command_argument(discord, client):
     @discord.command(type=ApplicationCommandType.MESSAGE)
     def repeat(ctx, target):
         return f"I repeat, {target.content.lower()}"
 
-    with client.context(Context(target=Message(content="This is a test."))):
+    with client.context(Context(target_message=Message(content="This is a test."))):
         assert client.run("repeat").content == "I repeat, this is a test."
```

### Comparing `deta-discord-interactions-0.0.3/deta_discord_interactions/tests/test_handler.py` & `deta-discord-interactions-0.1.0/deta_discord_interactions/tests/test_handler.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from deta_discord_interactions import Message, ActionRow, Button, ButtonStyles
 
 
 def test_basic_handler(discord, client):
     click_count = 0
 
-    @discord.custom_handler()
+    @discord.custom_handler('click_handler')
     def handle_click(ctx):
         nonlocal click_count
         click_count += 1
 
         return Message(
             content=f"The button has been clicked {click_count} times",
             components=[
                 ActionRow(
                     components=[
                         Button(
                             style=ButtonStyles.PRIMARY,
-                            custom_id=handle_click,
+                            custom_id='click_handler',
                             label="Click Me!",
                         )
                     ]
                 )
             ],
             update=True,
         )
@@ -42,32 +42,32 @@
                         )
                     ]
                 )
             ],
         )
 
     client.run("click_counter")
-    discord.custom_id_handlers[handle_click](None)
+    discord.custom_id_handlers['click_handler'](None)
     assert click_count == 1
 
 
 def test_stateful_handler(discord, client):
-    @discord.custom_handler()
+    @discord.custom_handler('click_handler')
     def handle_click(ctx, click_count):
         click_count = int(click_count)
         click_count += 1
 
         return Message(
             content=f"{click_count} clicks",
             components=[
                 ActionRow(
                     components=[
                         Button(
                             style=ButtonStyles.PRIMARY,
-                            custom_id=[handle_click, click_count],
+                            custom_id=['click_handler', click_count],
                             label="Click Me!",
                         )
                     ]
                 )
             ],
             update=True,
         )
@@ -80,18 +80,18 @@
         return Message(
             content=f"The button has been clicked 0 times",
             components=[
                 ActionRow(
                     components=[
                         Button(
                             style=ButtonStyles.PRIMARY,
-                            custom_id=[handle_click, 0],
+                            custom_id=['click_handler', 0],
                             label="Click Me!",
                         )
                     ]
                 )
             ],
         )
 
     client.run("click_counter")
-    response = discord.custom_id_handlers[handle_click](None, 0)
+    response = discord.custom_id_handlers['click_handler'](None, 0)
     assert response.content == "1 clicks"
```

### Comparing `deta-discord-interactions-0.0.3/deta_discord_interactions/tests/test_options.py` & `deta-discord-interactions-0.1.0/deta_discord_interactions/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `deta-discord-interactions-0.0.3/deta_discord_interactions/tests/test_register.py` & `deta-discord-interactions-0.1.0/deta_discord_interactions/tests/test_register.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,108 +1,70 @@
-from flask import Flask
-
+"""Not sure if particularly useful without any asserts, but at least checks that no exceptions are raised while creating and dumping stuff."""
 from deta_discord_interactions import DiscordInteractions
 from deta_discord_interactions.context import ApplicationCommandType
 
-
-def test_register_command():
-    app = Flask(__name__)
-    app.config["DONT_VALIDATE_SIGNATURE"] = True
-    app.config["DONT_REGISTER_WITH_DISCORD"] = True
-
-    discord = DiscordInteractions(app)
-
+def test_register_command(discord: DiscordInteractions):
     @discord.command()
     def ping(ctx):
         return "pong"
 
     discord.update_commands()
 
 
-def test_register_user_command():
-    app = Flask(__name__)
-    app.config["DONT_VALIDATE_SIGNATURE"] = True
-    app.config["DONT_REGISTER_WITH_DISCORD"] = True
-
-    discord = DiscordInteractions(app)
-
+def test_register_user_command(discord: DiscordInteractions):
     @discord.command(type=ApplicationCommandType.USER)
     def ping(ctx):
         return "pong"
 
     @discord.command(type=ApplicationCommandType.USER)
-    def PING(ctx):
+    def ping2(ctx):
         return "pong"
 
     @discord.command(name="user test", type=ApplicationCommandType.USER)
-    def ping(ctx):
+    def ping3(ctx):
         return "pong"
 
     discord.update_commands()
 
 
-def test_register_message_command():
-    app = Flask(__name__)
-    app.config["DONT_VALIDATE_SIGNATURE"] = True
-    app.config["DONT_REGISTER_WITH_DISCORD"] = True
-
-    discord = DiscordInteractions(app)
-
+def test_register_message_command(discord: DiscordInteractions):
     @discord.command(type=ApplicationCommandType.MESSAGE)
     def ping(ctx):
         return "pong"
 
     @discord.command(type=ApplicationCommandType.MESSAGE)
-    def PING(ctx):
+    def ping2(ctx):
         return "pong"
 
     @discord.command(name="user test", type=ApplicationCommandType.MESSAGE)
-    def ping(ctx):
+    def ping3(ctx):
         return "pong"
 
     discord.update_commands()
 
 
-def test_register_subcommand():
-    app = Flask(__name__)
-    app.config["DONT_VALIDATE_SIGNATURE"] = True
-    app.config["DONT_REGISTER_WITH_DISCORD"] = True
-
-    discord = DiscordInteractions(app)
-
+def test_register_subcommand(discord: DiscordInteractions):
     group = discord.command_group("group")
 
     @group.command()
     def subcommand(ctx):
         return "pong"
 
     discord.update_commands()
 
 
-def test_register_options():
-    app = Flask(__name__)
-    app.config["DONT_VALIDATE_SIGNATURE"] = True
-    app.config["DONT_REGISTER_WITH_DISCORD"] = True
-
-    discord = DiscordInteractions(app)
-
+def test_register_options(discord: DiscordInteractions):
     @discord.command()
     def ping(ctx, option1: str, option2: float, option3: str = ""):
         return f"pong"
 
     discord.update_commands()
 
 
-def test_register_subcommand_options():
-    app = Flask(__name__)
-    app.config["DONT_VALIDATE_SIGNATURE"] = True
-    app.config["DONT_REGISTER_WITH_DISCORD"] = True
-
-    discord = DiscordInteractions(app)
-
+def test_register_subcommand_options(discord: DiscordInteractions):
     group = discord.command_group("group")
 
     @group.command()
     def subcommand(ctx, option1: str, option2: float, option3: str = ""):
         return "pong"
 
     discord.update_commands()
```

### Comparing `deta-discord-interactions-0.0.3/deta_discord_interactions/tests/test_response.py` & `deta-discord-interactions-0.1.0/deta_discord_interactions/tests/test_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,9 +90,9 @@
         "tts": False,
         "allowed_mentions": {"parse": ["roles", "users", "everyone"]},
         "components": None,
         "flags": 0,
     }
 
     result, mimetype = resp.encode(followup=True)
-    assert json.loads(result) == expected
+    assert json.loads(result.decode("UTF-8")) == expected
     assert mimetype == "application/json"
```

### Comparing `deta-discord-interactions-0.0.3/deta_discord_interactions/tests/test_subcommand.py` & `deta-discord-interactions-0.1.0/deta_discord_interactions/tests/test_subcommand.py`

 * *Files identical despite different names*

### Comparing `deta-discord-interactions-0.0.3/deta_discord_interactions/utils/database/_local_base.py` & `deta-discord-interactions-0.1.0/deta_discord_interactions/utils/database/_local_base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,16 @@
-from __future__ import annotations
-
 import functools
 import json
 import pathlib
 from typing import Callable, Optional
 
 from deta.base import Util
 
 from deta_discord_interactions.utils.database.bound_meta import BoundMeta
 
-# In the future: Perhaps get rid of this and use pytest fixtures instead?
-
 operations = {
     # no prefix = eq
     "ne": lambda key, value, record: record.get(key) != value,
 
     "lt": lambda key, value, record: record.get(key) < value,
     "lte": lambda key, value, record: record.get(key) <= value,
     "gt": lambda key, value, record: record.get(key) > value,
@@ -58,28 +54,33 @@
         self.count = count
         self.last = last
         self.items = items
 
 
 _memory_inventory = {}
 class Base:
-    def __init__(self, name: str, sync_disk: bool = False):
+    def __init__(self, name: str, sync_disk: bool = False, folder: Optional[str] = None):
         self.name = name
         if sync_disk:
-            self.inventory = DiskBaseBackend(name)
+            self.inventory = DiskBaseBackend(f'{name}.json', folder)
         else:
             self.inventory = _memory_inventory.setdefault(name, {})
 
     def get(self, key):
         obj = self.inventory.get(key)
         if obj:
             obj = json.loads(obj)
         return obj
 
-    def insert(self, data, key):
+    def insert(self, data, key, *, expire_in: None=None, expire_at: None=None):
+        if expire_in:
+            print(f"Ignoring parameter (not supported by local base): {expire_in=}")
+        if expire_at:
+            print(f"Ignoring parameter (not supported by local base): {expire_at=}")
+
         if key in self.inventory:
             raise Exception(f"Item with key '{key}' already exists")
         self.inventory[key] = json.dumps(data)
 
     def update(self, updates, key):
         if key not in self.inventory:
             raise Exception(f"Key '{key}' not found")
@@ -98,33 +99,40 @@
                     value.val + obj[attribute]
                 )
             else:
                 obj[attribute] = value
         
         self.inventory[key] = json.dumps(obj)
 
+    def delete(self, key):
+        del self.inventory[key]
+
     def put_many(self, items):
         items = {record.pop('key'): json.dumps(record) for record in (item.copy() for item in items)}
         self.inventory.update(items)
 
-    def put(self, item, key):
+    def put(self, item, key, *, expire_in: None=None, expire_at: None=None):
+        if expire_in:
+            print(f"Ignoring parameter (not supported by local base): {expire_in=}")
+        if expire_at:
+            print(f"Ignoring parameter (not supported by local base): {expire_at=}")
         self.inventory[key] = json.dumps(item)
 
     def fetch(self, query, limit, last):
         results = []
         match_condition = parse_filters(query)
         for key, value in self.inventory.items():
             obj = json.loads(value)
             obj["key"] = key
             if match_condition(obj):
                 results.append(obj)
         if isinstance(last, str):
             index = next((i for i, record in enumerate(results) if record['key'] == last), None)
             results = results[index:]
-        if limit and limit > 0:
+        if limit:
             results = results[:limit]
         return FetchResponse(items=results)
 
 
 
 
 bind_methods = [
@@ -133,30 +141,36 @@
 
 import pathlib
 import os
 
 
 class DiskBaseBackend(dict, metaclass=BoundMeta, bind_methods=bind_methods):
     """Database backend that saves to disk whenever it's modified."""
-    def __init__(self, database_name: str):
+    def __init__(self, database_name: str, folder: Optional[str]):
+        if folder:
+            self._path = pathlib.Path(folder) / database_name
+        elif (env_folder := os.getenv("DETA_ORM_FOLDER")):
+            self._path = pathlib.Path(env_folder) / database_name
+        else:
+            raise Exception("When using a Database on DISK mode, you must specify the path."\
+                "\nUsing the `disk_base_path` keyword argument or the `DETA_ORM_FOLDER` environment variable.")
         try:
-            with (pathlib.Path(os.getenv("DISCORD_INTERACTIONS_DATABASE_FOLDER")) / database_name).open('r') as file:
+            with self._path.open('r') as file:
                 super().__init__(json.load(file))
         except Exception:
             super().__init__()
-        self._file_name = database_name
-        if os.getenv("DISCORD_INTERACTIONS_DATABASE_FORMAT_NICELY", False):
+        if os.getenv("DETA_ORM_FORMAT_NICELY", False):
             self._options = {
                 "indent": 4,
                 "sort_keys": True,
             }
         else:
             self._options = {
                 "indent": None,
                 "separators": (',', ':'),
             }
 
 
     def _sync(self, method, value, *args, **kwargs):
-        with (pathlib.Path(os.getenv("DISCORD_INTERACTIONS_DATABASE_FOLDER")) / self._file_name).open('w') as file:
+        with self._path.open('w') as file:
             json.dump(dict(self), file, **self._options)
         return value
```

### Comparing `deta-discord-interactions-0.0.3/deta_discord_interactions/utils/database/bound_meta.py` & `deta-discord-interactions-0.1.0/deta_discord_interactions/utils/database/bound_meta.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     When any of the methods called to `bind_methods` are called, it will:
         - execute that method
         - call self._sync() with:
             the name of that method,
             the value returned by that method
             the arguments and keyword arguments passed to that method
         - return the value returned by _sync
-    Note: DO NOT overwrite these methods on your class
+    Note: The 'bound' methods are decorated. Do not further modify them. 
 
     Example Usage:
         class Test(list, metaclass=BoundMeta, bind_methods=['__iadd__', 'append', 'extend']):
             def _sync(self, method, value, *args, **kwargs):
                 print(self, method, value)
                 return value
     """
```

### Comparing `deta-discord-interactions-0.0.3/deta_discord_interactions/utils/database/query.py` & `deta-discord-interactions-0.1.0/deta_discord_interactions/utils/database/query.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,50 +5,48 @@
 query = Query(Field('name') == 'bob')
 
 query = Query('gaming' in Field('hobbies'))
 
 query = Query(Field('key').startswith('discord_interactions_user_'))
 
 # Combining multiple statements:
-query = Query(  # AND
+# AND
+query = Query(
   Field('name') == 'bob',
   Field('age').in_range(10, 18)
 )
-query = Query([  # AND
-  Field('name') == 'bob',
+# Alternatively for AND:
+query = Query(Field('person.name') == 'bob') & Query(Field('age') > 10)  # Combine as AND
+
+# OR
+q1 = Query(  
+  Field('name') == 'bob'
+) 
+q2 = Query(
   Field('age').in_range(10, 18)
-])
-query = Query(  # OR
-  [Field('name') == 'bob'],
-  [Field('age').in_range(10, 18)]
 )
-# query = Query(Field('name') == 'bob') | Query(Field('age') > 10)  # Combine as OR CURRENTLY NOT IMPLEMENTED
-query = Query(Field('person.name') == 'bob') & Query(Field('age') > 10)  # Combine as AND
-query = Query(Field('name') == 'bob') & Query(Field('age') > 10)
+query = q1 | q2
 
 # To evaluate a query
 results = database.fetch(query)
 """
 
 from typing import NoReturn
-from deta_discord_interactions.utils.database.adapters import transform_identifier
 
 class Field:
     "Proxy class for setting filters"
     def __init__(self, attribute: str):
         self.attribute = attribute
 
     def __eq__(self, other) -> dict:
-        other = transform_identifier(other, on_unknown='ignore')
         return {
             self.attribute: other
         }
 
     def __ne__(self, other) -> dict:
-        other = transform_identifier(other, on_unknown='ignore')
         return {
             f'{self.attribute}?ne': other
         }
 
     def __lt__(self, other) -> dict:
         return {
             f'{self.attribute}?lt': other
@@ -80,26 +78,23 @@
 
     def in_range(self, start: int, stop: int) -> dict:
         return {
             f'{self.attribute}?r': [start, stop]
         }
 
     def __contains__(self, other) -> dict:
-        other = transform_identifier(other, on_unknown='ignore')
         return {
             f'{self.attribute}?contains': other
         }
     def contains(self, other) -> dict:
-        other = transform_identifier(other, on_unknown='ignore')
         return {
             f'{self.attribute}?contains': other
         }
 
     def not_contains(self, other) -> dict:
-        other = transform_identifier(other, on_unknown='ignore')
         return {
             f'{self.attribute}?not_contains': other
         }
 
 
 class Query:
     """Query class for querying Deta Base.
```

### Comparing `deta-discord-interactions-0.0.3/deta_discord_interactions/utils/oauth/model.py` & `deta-discord-interactions-0.1.0/deta_discord_interactions/utils/oauth/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import os
-import importlib
 import datetime
-from typing import Optional
+from typing import Callable, Optional
 from dataclasses import dataclass
 
 import requests
 from deta_discord_interactions.models.user import User
 from deta_discord_interactions.models.message import Message
 
 from deta_discord_interactions.models.utils import LoadableDataclass
@@ -39,41 +38,58 @@
         if isinstance(self.expires, str):
             self.expires = datetime.datetime.fromisoformat(self.expires)
 
 
 @dataclass
 class OAuthToken(LoadableDataclass):
     access_token: str
-    refresh_token: str
     scope: str
     expires_in: int
+    refresh_token: str = None  # Not present in client credential grants
     webhook: 'Webhook' = None
     expire_date: datetime.datetime = None
 
+    @classmethod
+    def from_client_credentials(cls, scope: str = "identify connections"):
+        "Generate an OAuth Access Token from the environment variables client credentials"
+        # https://discord.com/developers/docs/topics/oauth2#client-credentials-grant
+        response = requests.post(
+            'https://discord.com/api/v10/oauth2/token',
+            data={
+                'grant_type': 'client_credentials',
+                'scope': scope,
+            },
+            headers={'Content-Type': 'application/x-www-form-urlencoded'},
+            auth=(os.getenv("DISCORD_CLIENT_ID"), os.getenv("DISCORD_CLIENT_SECRET"))
+        )
+        response.raise_for_status()
+        return cls.from_dict(response.json())
+
+
     def __post_init__(self):
         if isinstance(self.expires_in, int) and self.expire_date is None:
             self.expire_date = datetime.datetime.utcnow() + datetime.timedelta(seconds=self.expires_in)
         if isinstance(self.webhook, dict):
             self.webhook = Webhook.from_dict(self.webhook)
 
     def get_auth_data(self) -> OAuthInfo:
         "Returns information about the authentication, including information about the user"
         headers = {
             "Authorization": f"Bearer {self.access_token}"
         }
-        response = requests.get(f'https://discord.com/api/v10/oauth2/@me', headers=headers)
+        response = requests.get('https://discord.com/api/v10/oauth2/@me', headers=headers)
         response.raise_for_status()
         return OAuthInfo.from_dict(response.json())
 
     def get_user_data(self) -> User:
         "Returns detailed information about the user"
         headers = {
             "Authorization": f"Bearer {self.access_token}"
         }
-        response = requests.get(f'https://discord.com/api/v10/users/@me', headers=headers)
+        response = requests.get('https://discord.com/api/v10/users/@me', headers=headers)
         response.raise_for_status()
         return User.from_dict(response.json())
 
     def revoke(self) -> None:
         response = requests.post(
             "https://discord.com/api/oauth2/token/revoke",
             data={"token": self.access_token},
@@ -83,27 +99,20 @@
 
 
 
 @dataclass
 class PendingOAuth(LoadableDataclass):
     "A 'promise' of an OAuth process yet to be confirmed"
     ctx: Context
-    callback_module: str
-    callback_name: str
+    callback: Callable
     callback_args: list
     callback_kwargs: dict
 
-    @property
-    def callback(self):
-        module = importlib.import_module(self.callback_module)
-        function = getattr(module, self.callback_name)
-        return function
-
-    def execute_callback(self, oauth_token: OAuthToken):
-        "Executes the callback when the user finishes the OAuth process"
+    def execute_callback(self, oauth_token: Optional[OAuthToken]):
+        "Executes the callback when the user finishes or cancels the OAuth process"
         return self.callback(oauth_token, self.ctx, *self.callback_args, **self.callback_kwargs)
 
     def to_dict(self):
         _discord_interactions = self.ctx.discord
         try:
             self.ctx.discord = None
             return super().to_dict()
@@ -170,15 +179,15 @@
 
         wait_param = 'true' if wait_for_response else 'false'
 
         encoded, mimetype = message.encode(followup=True, **encode_kwargs)
 
         response = requests.post(
             self.url,
-            data=encoded.encode("UTF-8"),
+            data=encoded,
             headers={"Content-Type": mimetype},
             params={"wait": wait_param}
         )
         response.raise_for_status()
         if wait_for_response:
             return Message.from_dict(response.json())
```

### Comparing `deta-discord-interactions-0.0.3/deta_discord_interactions/utils/oauth/oauth.py` & `deta-discord-interactions-0.1.0/deta_discord_interactions/utils/oauth/oauth.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,57 @@
 "Deals with OAuth2, creating and saving Webhooks"
 import json
 import os
-from typing import Callable, NoReturn
+from typing import Callable, NoReturn, Optional, Protocol
 from urllib.parse import quote, unquote
+from dataclasses import dataclass
 
 import requests
 from deta_discord_interactions.models.component import ActionRow, Button, ButtonStyles
 
 from deta_discord_interactions.models.message import Message
 
 from deta_discord_interactions.discord import DiscordInteractions
 from deta_discord_interactions.context import Context
 
-from deta_discord_interactions.utils.database import Database
+from deta_discord_interactions.utils.database import Database, LoadableDataclass
 from deta_discord_interactions.utils.oauth.model import OAuthToken, PendingOAuth
 
 
 DISCORD_BASE_URL = 'https://discord.com/api/v10'
-DEFAULT_MICRO_PATH = "https://{MICRO}.deta.dev"
 
-pending_oauths = Database(name="_discord_interactions_pending_oauths")
+@dataclass
+class PendingRecord(LoadableDataclass):
+    redirect_uri: str
+    pending_oauth: PendingOAuth
 
 
+pending_oauths = Database(name="_discord_interactions_pending_oauths", record_type=PendingRecord)
+remember_callback = pending_oauths.remember_function
+
 def enable_oauth(app: DiscordInteractions, /, *, path: str = "/oauth") -> None:
     "Allows for the app to receive and process OAuth and create Webhooks"
     app.route(path)(_handle_oauth)
 
 
+class Callback(Protocol):
+    "Just to make it easier to identifity the signature the callback must have"
+    def __call__(self, token: Optional[OAuthToken], ctx: Context, *args, **kwargs) -> str: ...
+
+
 def request_oauth(
     ctx: Context,
     /,
     internal_id: str,
     *,
-    domain: str = DEFAULT_MICRO_PATH,
+    domain: Optional[str] = None,
     path: str = "/oauth",
     scope: str,
-    callback: Callable,
-    args: tuple = [],
+    callback: Callback,
+    args: list = [],
     kwargs: dict = {},
     message_content: str = "Use the button to register with OAuth",
     button_label: str = "Grant OAuth",
 ) -> Message:
     """Utility function to make OAuth creation and usage easier
     
     Returns a Message with a link the user must visit to grant an OAuth Token,
@@ -49,56 +60,54 @@
     See https://discord.com/developers/docs/topics/oauth2 for the list of available scopes and more information
 
     Parameters
     ----------
     ctx : Context
         The Context this function is being called from
     internal_id : str
-        ID to be used internally. Will be shown in the link.. Will be shown in the link.
-    domain : str, default https://{MICRO}.deta.dev
+        ID to be used internally. Will be shown in the link.
+    domain : str, automatically set
         Base URL for the Micro running the bot
-        {MICRO} is filled automatically from the environment variables
+        If not set, uses the `DETA_SPACE_APP_HOSTNAME` environment variable
     path : str, default '/oauth'
         Path that the user will be sent back to. 
-        Must match what has been passed to `enable_webhooks` and be set on the Developer Portal
+        Must match what has been passed to `enable_webhooks` and be set on the Discord Developer Portal
     scope : str
         OAuth scopes to request, separated by spaces.
     callback : Callable
-        Must be a normal function, not a lambda, partial nor a class method.
+        Must have been registered using the `remember_callback` decorator.
+        Args passed: (token or None, ctx, *args, **kwargs). 
+        If the user refuses the consent form, passes None instead of an OAuthToken
     args : tuple|list
     kwargs : dict
         Arguments and Keyword arguments to be passed onto callback
         The created newly created OAuthToken and Context passed to request_oauth are always passed first.
     message_content : str
         Message content, besides the button with the URL
     button_label : str
         The URL Button's label
 
-
     If the user never finishes the authorization process, the callback will not be called
     If they create one , it will be called with ctx, webhook, `args` and `kwargs`
     The link will only work for one authorization
     """
     promise = PendingOAuth(
         ctx,
-        callback.__module__,
-        callback.__name__,
+        callback,
         args,
         kwargs,
     )
-    redirect_uri = (
-        quote(
-            domain.format(MICRO = os.getenv("DETA_PATH")) + path,
-            safe=''
-        )
-    )
+    if domain is None:
+        if os.getenv("DETA_SPACE_APP"):
+            domain = f"""https://{os.getenv("DETA_SPACE_APP_HOSTNAME")}"""
+        else:
+            raise Exception("Cannot identify which domain to use for OAuth redirection")
+    redirect_uri = quote(domain + path, safe='')
 
-    with pending_oauths[internal_id] as record:
-        record["pending_oauth"] = promise
-        record["redirect_uri"] = redirect_uri
+    pending_oauths[internal_id] = PendingRecord(redirect_uri, promise)
 
     link = (
         f"{DISCORD_BASE_URL}/oauth2/authorize?"
         "response_type=code&"
         f"scope={quote(scope)}&"
         f"guild_id={ctx.guild_id}&"
         f"client_id={os.getenv('DISCORD_CLIENT_ID')}&"
@@ -120,19 +129,19 @@
 
 
 # Mostly for convenience and more... idk, semantic
 def create_webhook(
     ctx: Context,
     /,
     internal_id: str,
-    domain: str = DEFAULT_MICRO_PATH,
+    domain: Optional[str] = None,
     path: str = "/oauth",
     *,
-    callback: Callable,
-    args: tuple = (),
+    callback: Callback,
+    args: list = [],
     kwargs: dict = {},
     message_content: str = "Use the button to register the Webhook",
     button_label: str = "Create Webhook",
 ) -> Message:
     """Utility function to make Webhook creation and usage easier
     
     Returns a Message with a link the user must visit to create a webhook,
@@ -140,32 +149,34 @@
 
     Parameters
     ----------
     ctx : Context
         The Context this function is being called from
     internal_id : str
         ID to be used internally. Will be shown in the link.
-    domain : str, default https://{MICRO}.deta.dev
--        Base URL for the Micro running the bot
-        {MICRO} is filled automatically from the environment variables
+    domain : str, automatically set
+        Base URL for the Micro running the bot
+        If not set, uses the `DETA_SPACE_APP_HOSTNAME` environment variable
     path : str, default '/oauth'
         Path that the user will be sent back to. 
-        Must match what has been passed to `enable_webhooks` and be set on the Developer Portal
+        Must match what has been passed to `enable_webhooks` and be set on the Discord Developer Portal
     callback : Callable
         Must be a normal function, not a lambda, partial nor a class method.
+        You must use the `remember_callback` decorator when defining the function
+        Args passed: (token or None, ctx, *args, **kwargs). 
+        If the user refuses the consent form, passes None instead of an OAuthToken
     args : tuple|list
     kwargs : dict
         Arguments and Keyword arguments to be passed onto callback.
         The created newly created OAuthToken and Context passed to create_webhook are always passed first.
     message_content : str
         Message content, besides the button with the URL
     button_label : str
         The Label of the button
 
-
     If the user never finishes creating a webhook, the callback will not be called
     If they create one , it will be called with ctx, webhook, `args` and `kwargs`
     The link will only work for one webhook
     """
     return request_oauth(
         ctx,
         internal_id,
@@ -176,52 +187,57 @@
         args=args,
         kwargs=kwargs,
         message_content=message_content,
         button_label=button_label,
     )
 
 
-
 def _handle_oauth(
     request: dict,
     start_response: Callable[[str, list], None],
     abort: Callable[[int, str], NoReturn],
 ) -> list[str]:
-    try:
-        code = request["query_dict"]["code"]
-        state = request["query_dict"]["state"]
-        # guild_id = request["query_dict"]["guild_id"]
-    except KeyError:
+    state = request["query_dict"].get("state")  # Must always be present
+    code = request["query_dict"].get("code")  # Only on Success
+    error = request["query_dict"].get("error")  # Only on Cancelled
+    if state is None or (error is None and code is None):
         abort(400, 'Invalid URL')
 
     url = DISCORD_BASE_URL + "/oauth2/token"
 
     try:
+        record = pending_oauths.get(state)
+
+        if record is None:
+            abort(400, "State not found")
 
-        with pending_oauths[state] as record:
-            redirect_uri: str = record["redirect_uri"]
-            pending_oauth: PendingOAuth = record["pending_oauth"]
+        redirect_uri: str = record.redirect_uri
+        pending_oauth: PendingOAuth = record.pending_oauth
 
         del pending_oauths[state]
 
-        data = {
-            'client_id': os.getenv("DISCORD_CLIENT_ID"),
-            'client_secret': os.getenv("DISCORD_CLIENT_SECRET"),
-            'grant_type': 'authorization_code',
-            'code': code,
-            'redirect_uri': unquote(redirect_uri),
-        }
-        headers = {
-            'Content-Type': 'application/x-www-form-urlencoded'
-        }
-        response = requests.post(url, data=data, headers=headers)
-        response.raise_for_status()
-        result = response.json()
+        if error is not None:
+            oauth_token = None
+
+        else:  # if code is not None:
+            data = {
+                'client_id': os.getenv("DISCORD_CLIENT_ID"),
+                'client_secret': os.getenv("DISCORD_CLIENT_SECRET"),
+                'grant_type': 'authorization_code',
+                'code': code,
+                'redirect_uri': unquote(redirect_uri),
+            }
+            headers = {
+                'Content-Type': 'application/x-www-form-urlencoded'
+            }
+            response = requests.post(url, data=data, headers=headers)
+            response.raise_for_status()
+            result = response.json()
 
-        oauth_token = OAuthToken.from_dict(result)
+            oauth_token = OAuthToken.from_dict(result)
 
         callback_response = pending_oauth.execute_callback(oauth_token)
 
         if isinstance(callback_response, (dict, list, int, str)):
             callback_response = json.dumps(callback_response)
         if isinstance(callback_response, str):
             callback_response = callback_response.encode("UTF-8")
```

### Comparing `deta-discord-interactions-0.0.3/deta_discord_interactions.egg-info/PKG-INFO` & `deta-discord-interactions-0.1.0/deta_discord_interactions.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deta-discord-interactions
-Version: 0.0.3
+Version: 0.1.0
 Summary: A web framework for Discord interactions specialized for usage in https://deta.sh
 Home-page: https://github.com/etrotta/flask-discord-interactions/tree/deta
 Author: etrotta
 Author-email: etrotta <etrotta@duck.com>
 License: MIT
 Project-URL: Homepage, https://github.com/etrotta/flask-discord-interactions/tree/deta
 Project-URL: Bug Tracker, https://github.com/etrotta/flask-discord-interactions/issues
@@ -14,17 +14,17 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Deta-Discord-Interactions
 
-This is a small web framework that lets you write Discord Application Commands using a decorator syntax similar to Flask's `@app.route()` or Discord.py's `@bot.command()`, specialized for usage in https://deta.sh
+This is a small web framework that lets you write Discord Application Commands using a decorator syntax similar to Flask's `@app.route()` or Discord.py's `@bot.command()`, specialized for usage in https://deta.space
 
-It is a fork of [flask-discord-interactions](https://pypi.org/project/Flask-Discord-Interactions/), but without requiring Flask and with some added features to make the usage of the library simpler.
+It is a fork of [flask-discord-interactions](https://pypi.org/project/Flask-Discord-Interactions/), but without requiring Flask and with some added features to make the usage of the library better on deta.
 
 ```
 @app.command()
 def ping(ctx):
     "Respond with a friendly 'pong'!"
     return "Pong!"
 ```
```

### Comparing `deta-discord-interactions-0.0.3/deta_discord_interactions.egg-info/SOURCES.txt` & `deta-discord-interactions-0.1.0/deta_discord_interactions.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 pyproject.toml
 setup.py
 deta_discord_interactions/__init__.py
 deta_discord_interactions/client.py
 deta_discord_interactions/command.py
 deta_discord_interactions/context.py
 deta_discord_interactions/discord.py
+deta_discord_interactions/http.py
 deta_discord_interactions.egg-info/PKG-INFO
 deta_discord_interactions.egg-info/SOURCES.txt
 deta_discord_interactions.egg-info/dependency_links.txt
 deta_discord_interactions.egg-info/not-zip-safe
 deta_discord_interactions.egg-info/requires.txt
 deta_discord_interactions.egg-info/top_level.txt
 deta_discord_interactions/enums/__init__.py
@@ -32,30 +33,28 @@
 deta_discord_interactions/models/user.py
 deta_discord_interactions/models/utils.py
 deta_discord_interactions/tests/__init__.py
 deta_discord_interactions/tests/conftest.py
 deta_discord_interactions/tests/test_command.py
 deta_discord_interactions/tests/test_component.py
 deta_discord_interactions/tests/test_context.py
-deta_discord_interactions/tests/test_flask.py
-deta_discord_interactions/tests/test_full_quart.py
+deta_discord_interactions/tests/test_database.py
 deta_discord_interactions/tests/test_handler.py
+deta_discord_interactions/tests/test_http.py
+deta_discord_interactions/tests/test_oauth.py
 deta_discord_interactions/tests/test_options.py
 deta_discord_interactions/tests/test_ping.py
-deta_discord_interactions/tests/test_quart.py
 deta_discord_interactions/tests/test_register.py
 deta_discord_interactions/tests/test_response.py
 deta_discord_interactions/tests/test_subcommand.py
+deta_discord_interactions/tests/test_wsgi.py
 deta_discord_interactions/utils/__init__.py
+deta_discord_interactions/utils/cooldown/__init__.py
 deta_discord_interactions/utils/database/__init__.py
 deta_discord_interactions/utils/database/_local_base.py
-deta_discord_interactions/utils/database/adapters.py
-deta_discord_interactions/utils/database/bound_dict.py
-deta_discord_interactions/utils/database/bound_list.py
 deta_discord_interactions/utils/database/bound_meta.py
 deta_discord_interactions/utils/database/database.py
 deta_discord_interactions/utils/database/exceptions.py
 deta_discord_interactions/utils/database/query.py
-deta_discord_interactions/utils/database/record.py
 deta_discord_interactions/utils/oauth/__init__.py
 deta_discord_interactions/utils/oauth/model.py
 deta_discord_interactions/utils/oauth/oauth.py
```

### Comparing `deta-discord-interactions-0.0.3/pyproject.toml` & `deta-discord-interactions-0.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "deta-discord-interactions"
-version = "0.0.3"
+version = "0.1.0"
 authors = [
   { name="etrotta", email="etrotta@duck.com" },
 ]
 description = "A web framework for Discord interactions specialized for usage in https://deta.sh"
 readme = "README.md"
 license = { text = "MIT" }
 requires-python = ">=3.9"
+dependencies = ['requests', 'PyNaCl', 'requests-toolbelt', 'deta']
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `deta-discord-interactions-0.0.3/setup.py` & `deta-discord-interactions-0.1.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md") as file:
     readme = file.read()
 
 
 setup(
     name="Deta-Discord-Interactions",
-    version="0.0.3",
+    version="0.1.0",
     url="https://github.com/etrotta/flask-discord-interactions/tree/deta",
     author="etrotta",
     author_email="etrotta@duck.com",
     description="A web framework for Discord interactions specialized for deta.",
     long_description=readme,
     long_description_content_type="text/markdown",
     packages=find_packages(),
```

