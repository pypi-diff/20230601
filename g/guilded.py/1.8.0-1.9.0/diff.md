# Comparing `tmp/guilded.py-1.8.0.tar.gz` & `tmp/guilded.py-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\shay\Documents\GitHub\guilded.py\dist\.tmp-mvl_fg2u\guilded.py-1.8.0.tar", last modified: Tue May  2 00:02:33 2023, max compression
+gzip compressed data, was "C:\Users\shay\Documents\GitHub\guilded.py\dist\.tmp-cmatgno6\guilded.py-1.9.0.tar", last modified: Thu Jun  1 16:32:28 2023, max compression
```

## Comparing `guilded.py-1.8.0.tar` & `guilded.py-1.9.0.tar`

### file list

```diff
@@ -1,80 +1,82 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 00:02:33.159072 guilded.py-1.8.0/
--rw-rw-rw-   0        0        0     2402 2021-08-25 00:53:36.000000 guilded.py-1.8.0/LICENSE
--rw-rw-rw-   0        0        0     2101 2023-05-02 00:02:33.158071 guilded.py-1.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     1343 2022-12-18 15:12:28.000000 guilded.py-1.8.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 00:02:33.108071 guilded.py-1.8.0/guilded/
--rw-rw-rw-   0        0        0      756 2023-05-02 00:01:04.000000 guilded.py-1.8.0/guilded/__init__.py
--rw-rw-rw-   0        0        0    25648 2023-02-09 20:51:56.000000 guilded.py-1.8.0/guilded/abc.py
--rw-rw-rw-   0        0        0     2724 2022-10-15 20:18:59.000000 guilded.py-1.8.0/guilded/activity.py
--rw-rw-rw-   0        0        0    20033 2022-10-15 20:18:59.000000 guilded.py-1.8.0/guilded/asset.py
--rw-rw-rw-   0        0        0     3254 2022-10-15 20:18:59.000000 guilded.py-1.8.0/guilded/backoff.py
--rw-rw-rw-   0        0        0   126012 2023-04-30 21:55:55.000000 guilded.py-1.8.0/guilded/channel.py
--rw-rw-rw-   0        0        0    31299 2023-04-18 03:46:37.000000 guilded.py-1.8.0/guilded/client.py
--rw-rw-rw-   0        0        0    12981 2022-10-15 20:18:59.000000 guilded.py-1.8.0/guilded/colour.py
--rw-rw-rw-   0        0        0    19980 2023-04-05 23:14:18.000000 guilded.py-1.8.0/guilded/embed.py
--rw-rw-rw-   0        0        0     9002 2023-01-20 17:23:19.000000 guilded.py-1.8.0/guilded/emote.py
--rw-rw-rw-   0        0        0    13786 2023-02-07 18:15:39.000000 guilded.py-1.8.0/guilded/enums.py
--rw-rw-rw-   0        0        0     4836 2022-10-15 20:18:59.000000 guilded.py-1.8.0/guilded/errors.py
--rw-rw-rw-   0        0        0    85178 2023-04-18 04:05:51.000000 guilded.py-1.8.0/guilded/events.py
-drwxrwxrwx   0        0        0        0 2023-05-02 00:02:33.065070 guilded.py-1.8.0/guilded/ext/
-drwxrwxrwx   0        0        0        0 2023-05-02 00:02:33.135073 guilded.py-1.8.0/guilded/ext/commands/
--rw-rw-rw-   0        0        0      199 2022-10-16 15:08:32.000000 guilded.py-1.8.0/guilded/ext/commands/__init__.py
--rw-rw-rw-   0        0        0     1938 2022-10-15 20:19:00.000000 guilded.py-1.8.0/guilded/ext/commands/_types.py
--rw-rw-rw-   0        0        0    35354 2022-10-16 15:22:10.000000 guilded.py-1.8.0/guilded/ext/commands/bot.py
--rw-rw-rw-   0        0        0    18115 2022-10-15 20:19:00.000000 guilded.py-1.8.0/guilded/ext/commands/cog.py
--rw-rw-rw-   0        0        0     6658 2022-10-15 20:19:00.000000 guilded.py-1.8.0/guilded/ext/commands/context.py
--rw-rw-rw-   0        0        0    35791 2022-10-15 20:19:00.000000 guilded.py-1.8.0/guilded/ext/commands/converters.py
--rw-rw-rw-   0        0        0    15030 2022-10-16 15:09:19.000000 guilded.py-1.8.0/guilded/ext/commands/cooldowns.py
--rw-rw-rw-   0        0        0    60064 2022-10-16 17:11:48.000000 guilded.py-1.8.0/guilded/ext/commands/core.py
--rw-rw-rw-   0        0        0    30211 2022-10-16 17:27:04.000000 guilded.py-1.8.0/guilded/ext/commands/errors.py
--rw-rw-rw-   0        0        0    50177 2022-10-15 20:19:00.000000 guilded.py-1.8.0/guilded/ext/commands/help.py
--rw-rw-rw-   0        0        0     7466 2022-10-15 20:19:00.000000 guilded.py-1.8.0/guilded/ext/commands/view.py
-drwxrwxrwx   0        0        0        0 2023-05-02 00:02:33.136073 guilded.py-1.8.0/guilded/ext/tasks/
--rw-rw-rw-   0        0        0    18800 2022-10-15 20:19:00.000000 guilded.py-1.8.0/guilded/ext/tasks/__init__.py
--rw-rw-rw-   0        0        0    13190 2022-10-15 20:18:59.000000 guilded.py-1.8.0/guilded/file.py
--rw-rw-rw-   0        0        0     5232 2022-10-15 20:18:59.000000 guilded.py-1.8.0/guilded/flowbot.py
--rw-rw-rw-   0        0        0    57511 2023-04-17 23:12:58.000000 guilded.py-1.8.0/guilded/gateway.py
--rw-rw-rw-   0        0        0     8221 2022-10-15 20:18:59.000000 guilded.py-1.8.0/guilded/group.py
--rw-rw-rw-   0        0        0    45910 2023-04-30 21:58:18.000000 guilded.py-1.8.0/guilded/http.py
--rw-rw-rw-   0        0        0     3803 2022-10-15 20:18:59.000000 guilded.py-1.8.0/guilded/invite.py
--rw-rw-rw-   0        0        0    35256 2023-04-30 22:02:49.000000 guilded.py-1.8.0/guilded/message.py
--rw-rw-rw-   0        0        0     2873 2022-10-15 20:18:59.000000 guilded.py-1.8.0/guilded/mixins.py
--rw-rw-rw-   0        0        0    32359 2022-11-20 03:58:31.000000 guilded.py-1.8.0/guilded/permissions.py
--rw-rw-rw-   0        0        0     3224 2022-10-15 20:18:59.000000 guilded.py-1.8.0/guilded/presence.py
--rw-rw-rw-   0        0        0    10648 2022-11-21 13:58:08.000000 guilded.py-1.8.0/guilded/reaction.py
--rw-rw-rw-   0        0        0    16453 2023-04-30 21:56:02.000000 guilded.py-1.8.0/guilded/reply.py
--rw-rw-rw-   0        0        0     7459 2022-10-15 20:18:59.000000 guilded.py-1.8.0/guilded/role.py
--rw-rw-rw-   0        0        0    40337 2023-03-31 00:17:06.000000 guilded.py-1.8.0/guilded/server.py
--rw-rw-rw-   0        0        0     5309 2022-10-15 20:18:59.000000 guilded.py-1.8.0/guilded/status.py
-drwxrwxrwx   0        0        0        0 2023-05-02 00:02:33.154072 guilded.py-1.8.0/guilded/types/
--rw-rw-rw-   0        0        0     1600 2023-04-17 22:54:44.000000 guilded.py-1.8.0/guilded/types/announcement.py
--rw-rw-rw-   0        0        0     3011 2023-03-25 15:03:09.000000 guilded.py-1.8.0/guilded/types/calendar_event.py
--rw-rw-rw-   0        0        0     1967 2023-04-30 22:01:39.000000 guilded.py-1.8.0/guilded/types/channel.py
--rw-rw-rw-   0        0        0      225 2023-01-23 20:13:53.000000 guilded.py-1.8.0/guilded/types/comment.py
--rw-rw-rw-   0        0        0     1639 2023-02-09 20:44:26.000000 guilded.py-1.8.0/guilded/types/doc.py
--rw-rw-rw-   0        0        0     1995 2022-10-15 20:19:00.000000 guilded.py-1.8.0/guilded/types/embed.py
--rw-rw-rw-   0        0        0     1324 2023-01-20 17:10:42.000000 guilded.py-1.8.0/guilded/types/emote.py
--rw-rw-rw-   0        0        0     1774 2023-02-02 18:56:59.000000 guilded.py-1.8.0/guilded/types/forum_topic.py
--rw-rw-rw-   0        0        0     5515 2023-04-17 22:58:37.000000 guilded.py-1.8.0/guilded/types/gateway.py
--rw-rw-rw-   0        0        0     2027 2022-10-15 20:19:00.000000 guilded.py-1.8.0/guilded/types/list_item.py
--rw-rw-rw-   0        0        0     1958 2023-04-30 22:01:12.000000 guilded.py-1.8.0/guilded/types/message.py
--rw-rw-rw-   0        0        0     2050 2023-04-17 22:55:33.000000 guilded.py-1.8.0/guilded/types/reaction.py
--rw-rw-rw-   0        0        0     1799 2022-10-15 20:19:00.000000 guilded.py-1.8.0/guilded/types/role.py
--rw-rw-rw-   0        0        0     1689 2022-10-27 15:22:52.000000 guilded.py-1.8.0/guilded/types/server.py
--rw-rw-rw-   0        0        0     1508 2023-02-28 00:17:19.000000 guilded.py-1.8.0/guilded/types/social_link.py
--rw-rw-rw-   0        0        0     2604 2022-10-15 20:19:00.000000 guilded.py-1.8.0/guilded/types/user.py
--rw-rw-rw-   0        0        0     3029 2023-02-02 16:43:38.000000 guilded.py-1.8.0/guilded/types/webhook.py
--rw-rw-rw-   0        0        0    23674 2023-03-28 22:16:34.000000 guilded.py-1.8.0/guilded/user.py
--rw-rw-rw-   0        0        0    13639 2022-12-16 17:30:53.000000 guilded.py-1.8.0/guilded/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-02 00:02:33.157074 guilded.py-1.8.0/guilded/webhook/
--rw-rw-rw-   0        0        0       23 2022-10-15 20:19:00.000000 guilded.py-1.8.0/guilded/webhook/__init__.py
--rw-rw-rw-   0        0        0    37555 2022-10-15 20:19:00.000000 guilded.py-1.8.0/guilded/webhook/async_.py
--rw-rw-rw-   0        0        0        0 2022-08-13 03:46:11.000000 guilded.py-1.8.0/guilded/webhook/sync.py
-drwxrwxrwx   0        0        0        0 2023-05-02 00:02:33.122099 guilded.py-1.8.0/guilded.py.egg-info/
--rw-rw-rw-   0        0        0     2101 2023-05-02 00:02:33.000000 guilded.py-1.8.0/guilded.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1615 2023-05-02 00:02:33.000000 guilded.py-1.8.0/guilded.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 00:02:33.000000 guilded.py-1.8.0/guilded.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      107 2023-05-02 00:02:33.000000 guilded.py-1.8.0/guilded.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-02 00:02:33.000000 guilded.py-1.8.0/guilded.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 00:02:33.159072 guilded.py-1.8.0/setup.cfg
--rw-rw-rw-   0        0        0     1608 2022-09-23 00:42:16.000000 guilded.py-1.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 16:32:28.777519 guilded.py-1.9.0/
+-rw-rw-rw-   0        0        0     2402 2021-08-25 00:53:36.000000 guilded.py-1.9.0/LICENSE
+-rw-rw-rw-   0        0        0     2101 2023-06-01 16:32:28.776520 guilded.py-1.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1343 2022-12-18 15:12:28.000000 guilded.py-1.9.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 16:32:28.723568 guilded.py-1.9.0/guilded/
+-rw-rw-rw-   0        0        0      785 2023-06-01 16:31:47.000000 guilded.py-1.9.0/guilded/__init__.py
+-rw-rw-rw-   0        0        0    26852 2023-05-29 23:37:49.000000 guilded.py-1.9.0/guilded/abc.py
+-rw-rw-rw-   0        0        0    20033 2022-10-15 20:18:59.000000 guilded.py-1.9.0/guilded/asset.py
+-rw-rw-rw-   0        0        0     3254 2022-10-15 20:18:59.000000 guilded.py-1.9.0/guilded/backoff.py
+-rw-rw-rw-   0        0        0   126137 2023-05-29 23:17:33.000000 guilded.py-1.9.0/guilded/channel.py
+-rw-rw-rw-   0        0        0    32508 2023-05-16 23:19:50.000000 guilded.py-1.9.0/guilded/client.py
+-rw-rw-rw-   0        0        0    12981 2022-10-15 20:18:59.000000 guilded.py-1.9.0/guilded/colour.py
+-rw-rw-rw-   0        0        0    19980 2023-04-05 23:14:18.000000 guilded.py-1.9.0/guilded/embed.py
+-rw-rw-rw-   0        0        0     9002 2023-01-20 17:23:19.000000 guilded.py-1.9.0/guilded/emote.py
+-rw-rw-rw-   0        0        0    13931 2023-06-01 14:41:55.000000 guilded.py-1.9.0/guilded/enums.py
+-rw-rw-rw-   0        0        0     4836 2022-10-15 20:18:59.000000 guilded.py-1.9.0/guilded/errors.py
+-rw-rw-rw-   0        0        0    95325 2023-05-30 22:32:00.000000 guilded.py-1.9.0/guilded/events.py
+drwxrwxrwx   0        0        0        0 2023-06-01 16:32:28.674569 guilded.py-1.9.0/guilded/ext/
+drwxrwxrwx   0        0        0        0 2023-06-01 16:32:28.751520 guilded.py-1.9.0/guilded/ext/commands/
+-rw-rw-rw-   0        0        0      199 2022-10-16 15:08:32.000000 guilded.py-1.9.0/guilded/ext/commands/__init__.py
+-rw-rw-rw-   0        0        0     1938 2022-10-15 20:19:00.000000 guilded.py-1.9.0/guilded/ext/commands/_types.py
+-rw-rw-rw-   0        0        0    35283 2023-05-29 23:31:15.000000 guilded.py-1.9.0/guilded/ext/commands/bot.py
+-rw-rw-rw-   0        0        0    18115 2022-10-15 20:19:00.000000 guilded.py-1.9.0/guilded/ext/commands/cog.py
+-rw-rw-rw-   0        0        0     6658 2022-10-15 20:19:00.000000 guilded.py-1.9.0/guilded/ext/commands/context.py
+-rw-rw-rw-   0        0        0    35367 2023-05-29 21:04:13.000000 guilded.py-1.9.0/guilded/ext/commands/converters.py
+-rw-rw-rw-   0        0        0    15030 2022-10-16 15:09:19.000000 guilded.py-1.9.0/guilded/ext/commands/cooldowns.py
+-rw-rw-rw-   0        0        0    67778 2023-06-01 16:22:16.000000 guilded.py-1.9.0/guilded/ext/commands/core.py
+-rw-rw-rw-   0        0        0    30211 2022-10-16 17:27:04.000000 guilded.py-1.9.0/guilded/ext/commands/errors.py
+-rw-rw-rw-   0        0        0    50177 2022-10-15 20:19:00.000000 guilded.py-1.9.0/guilded/ext/commands/help.py
+-rw-rw-rw-   0        0        0     7466 2022-10-15 20:19:00.000000 guilded.py-1.9.0/guilded/ext/commands/view.py
+drwxrwxrwx   0        0        0        0 2023-06-01 16:32:28.752520 guilded.py-1.9.0/guilded/ext/tasks/
+-rw-rw-rw-   0        0        0    18800 2022-10-15 20:19:00.000000 guilded.py-1.9.0/guilded/ext/tasks/__init__.py
+-rw-rw-rw-   0        0        0    13190 2022-10-15 20:18:59.000000 guilded.py-1.9.0/guilded/file.py
+-rw-rw-rw-   0        0        0     5232 2022-10-15 20:18:59.000000 guilded.py-1.9.0/guilded/flowbot.py
+-rw-rw-rw-   0        0        0    61856 2023-05-25 18:32:35.000000 guilded.py-1.9.0/guilded/gateway.py
+-rw-rw-rw-   0        0        0     9890 2023-05-09 23:29:24.000000 guilded.py-1.9.0/guilded/group.py
+-rw-rw-rw-   0        0        0    49648 2023-06-01 14:40:24.000000 guilded.py-1.9.0/guilded/http.py
+-rw-rw-rw-   0        0        0     3803 2022-10-15 20:18:59.000000 guilded.py-1.9.0/guilded/invite.py
+-rw-rw-rw-   0        0        0    39544 2023-05-30 20:25:35.000000 guilded.py-1.9.0/guilded/message.py
+-rw-rw-rw-   0        0        0     2873 2022-10-15 20:18:59.000000 guilded.py-1.9.0/guilded/mixins.py
+-rw-rw-rw-   0        0        0    62638 2023-06-01 15:35:20.000000 guilded.py-1.9.0/guilded/permissions.py
+-rw-rw-rw-   0        0        0     3224 2022-10-15 20:18:59.000000 guilded.py-1.9.0/guilded/presence.py
+-rw-rw-rw-   0        0        0    10648 2022-11-21 13:58:08.000000 guilded.py-1.9.0/guilded/reaction.py
+-rw-rw-rw-   0        0        0    16453 2023-04-30 21:56:02.000000 guilded.py-1.9.0/guilded/reply.py
+-rw-rw-rw-   0        0        0    12620 2023-05-25 03:57:30.000000 guilded.py-1.9.0/guilded/role.py
+-rw-rw-rw-   0        0        0    50093 2023-06-01 15:09:46.000000 guilded.py-1.9.0/guilded/server.py
+-rw-rw-rw-   0        0        0     3200 2023-05-19 03:57:55.000000 guilded.py-1.9.0/guilded/status.py
+-rw-rw-rw-   0        0        0     3597 2023-06-01 03:01:11.000000 guilded.py-1.9.0/guilded/subscription.py
+drwxrwxrwx   0        0        0        0 2023-06-01 16:32:28.772520 guilded.py-1.9.0/guilded/types/
+-rw-rw-rw-   0        0        0     1600 2023-04-17 22:54:44.000000 guilded.py-1.9.0/guilded/types/announcement.py
+-rw-rw-rw-   0        0        0     3011 2023-03-25 15:03:09.000000 guilded.py-1.9.0/guilded/types/calendar_event.py
+-rw-rw-rw-   0        0        0     2100 2023-05-23 16:20:34.000000 guilded.py-1.9.0/guilded/types/channel.py
+-rw-rw-rw-   0        0        0      225 2023-01-23 20:13:53.000000 guilded.py-1.9.0/guilded/types/comment.py
+-rw-rw-rw-   0        0        0     1639 2023-02-09 20:44:26.000000 guilded.py-1.9.0/guilded/types/doc.py
+-rw-rw-rw-   0        0        0     1995 2022-10-15 20:19:00.000000 guilded.py-1.9.0/guilded/types/embed.py
+-rw-rw-rw-   0        0        0     1324 2023-01-20 17:10:42.000000 guilded.py-1.9.0/guilded/types/emote.py
+-rw-rw-rw-   0        0        0     1774 2023-02-02 18:56:59.000000 guilded.py-1.9.0/guilded/types/forum_topic.py
+-rw-rw-rw-   0        0        0     6220 2023-05-30 22:32:53.000000 guilded.py-1.9.0/guilded/types/gateway.py
+-rw-rw-rw-   0        0        0     1631 2023-05-09 01:29:48.000000 guilded.py-1.9.0/guilded/types/group.py
+-rw-rw-rw-   0        0        0     2027 2022-10-15 20:19:00.000000 guilded.py-1.9.0/guilded/types/list_item.py
+-rw-rw-rw-   0        0        0     1958 2023-04-30 22:01:12.000000 guilded.py-1.9.0/guilded/types/message.py
+-rw-rw-rw-   0        0        0     2050 2023-04-17 22:55:33.000000 guilded.py-1.9.0/guilded/types/reaction.py
+-rw-rw-rw-   0        0        0     1622 2023-05-18 21:03:59.000000 guilded.py-1.9.0/guilded/types/role.py
+-rw-rw-rw-   0        0        0     1689 2022-10-27 15:22:52.000000 guilded.py-1.9.0/guilded/types/server.py
+-rw-rw-rw-   0        0        0     1508 2023-02-28 00:17:19.000000 guilded.py-1.9.0/guilded/types/social_link.py
+-rw-rw-rw-   0        0        0     1442 2023-06-01 03:01:41.000000 guilded.py-1.9.0/guilded/types/subscription.py
+-rw-rw-rw-   0        0        0     2724 2023-05-19 03:27:49.000000 guilded.py-1.9.0/guilded/types/user.py
+-rw-rw-rw-   0        0        0     3029 2023-02-02 16:43:38.000000 guilded.py-1.9.0/guilded/types/webhook.py
+-rw-rw-rw-   0        0        0    24280 2023-06-01 15:32:28.000000 guilded.py-1.9.0/guilded/user.py
+-rw-rw-rw-   0        0        0    13639 2022-12-16 17:30:53.000000 guilded.py-1.9.0/guilded/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-01 16:32:28.775521 guilded.py-1.9.0/guilded/webhook/
+-rw-rw-rw-   0        0        0       23 2022-10-15 20:19:00.000000 guilded.py-1.9.0/guilded/webhook/__init__.py
+-rw-rw-rw-   0        0        0    37555 2022-10-15 20:19:00.000000 guilded.py-1.9.0/guilded/webhook/async_.py
+-rw-rw-rw-   0        0        0        0 2022-08-13 03:46:11.000000 guilded.py-1.9.0/guilded/webhook/sync.py
+drwxrwxrwx   0        0        0        0 2023-06-01 16:32:28.739567 guilded.py-1.9.0/guilded.py.egg-info/
+-rw-rw-rw-   0        0        0     2101 2023-06-01 16:32:28.000000 guilded.py-1.9.0/guilded.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1672 2023-06-01 16:32:28.000000 guilded.py-1.9.0/guilded.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 16:32:28.000000 guilded.py-1.9.0/guilded.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      107 2023-06-01 16:32:28.000000 guilded.py-1.9.0/guilded.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-01 16:32:28.000000 guilded.py-1.9.0/guilded.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 16:32:28.777519 guilded.py-1.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     1608 2022-09-23 00:42:16.000000 guilded.py-1.9.0/setup.py
```

### Comparing `guilded.py-1.8.0/LICENSE` & `guilded.py-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `guilded.py-1.8.0/PKG-INFO` & `guilded.py-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guilded.py
-Version: 1.8.0
+Version: 1.9.0
 Summary: An API wrapper in Python for Guilded's bot API
 Home-page: https://github.com/shayypy/guilded.py
 Author: shay (shayypy)
 License: MIT
 Project-URL: Documentation, https://guildedpy.readthedocs.io/en/latest/
 Project-URL: Issue tracker, https://github.com/shayypy/guilded.py/issues
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `guilded.py-1.8.0/README.md` & `guilded.py-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `guilded.py-1.8.0/guilded/__init__.py` & `guilded.py-1.9.0/guilded/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 __copyright__ = 'shay 2020-present'
-__version__ = '1.8.0'
+__version__ = '1.9.0'
 
 import logging
 
 from . import abc as abc, utils as utils
 from .utils import Object as Object
 from .asset import *
 from .channel import *
@@ -23,11 +23,12 @@
 from .reply import *
 from .role import *
 from .permissions import *
 from .presence import *
 from .reaction import *
 from .server import *
 from .status import *
+from .subscription import *
 from .user import *
 from .webhook import *
 
 logging.getLogger(__name__).addHandler(logging.NullHandler())
```

### Comparing `guilded.py-1.8.0/guilded/abc.py` & `guilded.py-1.9.0/guilded/abc.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,30 +50,33 @@
 """
 
 from __future__ import annotations
 
 import abc
 import datetime
 import re
-from typing import TYPE_CHECKING, List, Optional, Sequence, Union
+from typing import TYPE_CHECKING, List, Optional, Sequence
+from typing_extensions import Self
 
-from .activity import Activity
 from .asset import Asset
 from .colour import Colour
 from .enums import ChannelType, try_enum, UserType
+from .errors import InvalidArgument
 from .message import HasContentMixin, ChatMessage
 from .mixins import Hashable
 from .presence import Presence
+from .status import Status
 from .utils import ISO8601, MISSING
 
 if TYPE_CHECKING:
     from .types.user import User as UserPayload
     from .types.channel import ServerChannel as ServerChannelPayload
     from .types.comment import ContentComment
 
+    from .channel import Thread
     from .embed import Embed
     from .group import Group
     from .server import Server
     from .user import Member
 
 
 __all__ = (
@@ -187,21 +190,14 @@
         )
 
         if delete_after is not None:
             await message.delete(delay=delete_after)
 
         return message
 
-    async def trigger_typing(self) -> None:
-        """|coro|
-
-        Begin your typing indicator in this channel.
-        """
-        await self._state.trigger_typing(self._channel_id)
-
     async def history(self,
         *,
         before: datetime.datetime = None,
         after: datetime.datetime = None,
         limit: int = 50,
         include_private: bool = False,
     ) -> List[ChatMessage]:
@@ -256,46 +252,87 @@
         :class:`.ChatMessage`
             The message from the ID.
         """
         data = await self._state.get_channel_message(self._channel_id, message_id)
         message = self._state.create_message(data=data['message'], channel=self._channel)
         return message
 
-    #async def create_thread(self, *content, **kwargs) -> Thread:
-    #    """|coro|
+    async def create_thread(
+        self,
+        name: str,
+        *,
+        message: Optional[ChatMessage] = None,
+    ) -> Thread:
+        """|coro|
 
-    #    Create a new thread in this channel.
+        Create a new thread in the channel.
 
-    #    Parameters
-    #    -----------
-    #    \*content: Any
-    #        The content of the message that should be created as the initial
-    #        message of the newly-created thread. Passing either this or
-    #        ``message`` is required.
-    #    name: :class:`str`
-    #        The name to create the thread with.
-    #    message: Optional[:class:`.ChatMessage`]
-    #        The message to create the thread from. Passing either this or
-    #        values for ``content`` is required.
+        .. warning::
 
-    #    Returns
-    #    --------
-    #    :class:`.Thread`
-    #        The thread that was created.
-    #    """
-    #    name = kwargs.get('name')
-    #    message = kwargs.get('message')
-    #    if not name:
-    #        raise TypeError('name is a required argument that is missing.')
-    #    if not message and not content:
-    #        raise TypeError('Must include message, an argument list of content, or both.')
-
-    #    data = await self._state.create_thread(self._channel_id, content, name=name, initial_message=message)
-    #    thread = self._state.create_channel(data=data.get('thread', data), group=self.group, server=self.server)
-    #    return thread
+            Be careful with this method!
+            It is very easy to accidentally cause a loop if you create a
+            thread on a message that caused the creation of its thread.
+
+        Depending on the type of the parent channel, this method requires
+        different permissions:
+
+        +------------------------------+-----------------------------------+
+        |         Parent Type          |             Permission            |
+        +------------------------------+-----------------------------------+
+        | :attr:`~.ChannelType.chat`   | :attr:`Permissions.read_messages` |
+        +------------------------------+-----------------------------------+
+        | :attr:`~.ChannelType.voice`  | :attr:`Permissions.hear_voice`    |
+        +------------------------------+-----------------------------------+
+        | :attr:`~.ChannelType.stream` | :attr:`Permissions.view_streams`  |
+        +------------------------------+-----------------------------------+
+
+        .. versionadded:: 1.9
+
+        Parameters
+        -----------
+        name: :class:`str`
+            The thread's name. Can include spaces.
+        message: Optional[:class:`.ChatMessage`]
+            The message to create the thread with.
+            If a private message is passed (i.e. :attr:`.ChatMessage.private`
+            is ``True``), then the thread is private too.
+            Otherwise, the thread is always public.
+
+        Returns
+        --------
+        :class:`.Thread`
+            The created thread.
+
+        Raises
+        -------
+        NotFound
+            The server, channel, or message provided does not exist.
+        Forbidden
+            You are not allowed to create a thread in this channel.
+        HTTPException
+            Failed to create a thread.
+        """
+
+        server_id = getattr(self._channel, 'server_id', None)
+        if not server_id:
+            raise InvalidArgument('Threads can only be created in a server context.')
+
+        data = await self._state.create_server_channel(
+            server_id,
+            'chat',
+            name=name,
+            parent_id=self._channel_id,
+            message_id=message.id if message else None,
+        )
+        channel = self._state.create_channel(
+            data=data['channel'],
+            group=message.group if message else None,
+            server=message.server if message else None,
+        )
+        return channel
 
     #async def pins(self) -> List[ChatMessage]:
     #    """|coro|
 
     #    Fetch the list of pinned messages in this channel.
 
     #    Returns
@@ -332,14 +369,16 @@
         This will likely only be available for the connected :class:`.ClientUser`.
     avatar: Optional[:class:`.Asset`]
         The user's set avatar, if any.
     banner: Optional[:class:`.Asset`]
         The user's profile banner, if any.
     created_at: :class:`datetime.datetime`
         When the user's account was created.
+    status: Optional[:class:`.Status`]
+        The custom status set by the user.
     """
 
     __slots__ = (
         'type',
         '_user_type',
         'id',
         'bot_id',
@@ -377,19 +416,15 @@
         self.nick: Optional[str] = None
         self.colour: Colour = Colour(0)
         self.slug: Optional[str] = data.get('subdomain')
         self.games: List = data.get('aliases', [])
         self.bio: str = (data.get('aboutInfo') or {}).get('bio') or ''
         self.tagline: str = (data.get('aboutInfo') or {}).get('tagLine') or ''
         self.presence: Presence = Presence.from_value(data.get('userPresenceStatus')) or None
-        status = data.get('userStatus') or {}
-        if status.get('content'):
-            self.status: Optional[Activity] = Activity.build(status['content'])
-        else:
-            self.status: Optional[Activity] = None
+        self.status = Status(data=data.get('status')) if data.get('status') else None
 
         self.blocked_at: Optional[datetime.datetime] = ISO8601(data.get('blockedDate'))
         self.online_at: Optional[datetime.datetime] = ISO8601(data.get('lastOnline'))
         self.created_at: datetime.datetime = ISO8601(data.get('createdAt') or data.get('joinDate'))
         # in profilev3, createdAt is returned instead of joinDate
 
         self.default_avatar: Asset = Asset._from_default_user_avatar(self._state, 1)
@@ -477,21 +512,20 @@
         * :class:`.ListChannel`
         * :class:`.MediaChannel`
         * :class:`.Thread`
         * :class:`.SchedulingChannel`
         * :class:`.VoiceChannel`
     """
 
-    def __init__(self, *, state, data: ServerChannelPayload, group: Group, **extra):
+    def __init__(self, *, state, data: ServerChannelPayload, group: Optional[Group] = None, **extra):
         self._state = state
         self._group = group
 
         self.group_id: str = data.get('groupId')
         self.server_id: str = data.get('serverId')
-        self.parent_id: Optional[str] = data.get('parentId')
         self.category_id: Optional[int] = data.get('categoryId')
 
         self.id: str = data['id']
         self.type: ChannelType = try_enum(ChannelType, data.get('type'))
         self.name: str = data.get('name') or ''
         self.topic: str = data.get('topic') or ''
         self.public: bool = data.get('isPublic', False)
@@ -531,16 +565,16 @@
     jump_url = share_url
 
     @property
     def mention(self) -> str:
         return f'<#{self.id}>'
 
     @property
-    def group(self) -> Group:
-        """:class:`~guilded.Group`: The group that this channel is in."""
+    def group(self) -> Optional[Group]:
+        """Optional[:class:`~guilded.Group`]: The group that this channel is in."""
         group = self._group
         if not group and self.server:
             group = self.server.get_group(self.group_id)
 
         return group
 
     @property
@@ -578,30 +612,30 @@
 
     async def edit(
         self,
         *,
         name: str = MISSING,
         topic: str = MISSING,
         public: bool = None,
-    ) -> ServerChannel:
+    ) -> Self:
         """|coro|
 
         Edit this channel.
 
         All parameters are optional.
 
         Parameters
         -----------
         name: :class:`str`
             The channel's name.
         topic: :class:`str`
             The channel's topic. Not applicable to threads.
         public: :class:`bool`
             Whether the channel should be public, i.e., visible to users who
-            are not a member of the server.
+            are not a member of the server. Not applicable to threads.
 
         Returns
         --------
         :class:`.ServerChannel`
             The newly edited channel.
         """
```

### Comparing `guilded.py-1.8.0/guilded/activity.py` & `guilded.py-1.9.0/guilded/mixins.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,16 +45,32 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
-class Activity:
-    '''Represents a user or member's activity in Guilded. Referred to as "Status" in the user popout.'''
-    def __init__(self, *, details: str):
-        self.details = details
-
-    @classmethod
-    def build(cls, data):
-        pl = data
-        return cls(details=pl.get('content'))
+from typing import Union
+
+
+__all__ = (
+    'EqualityComparable',
+    'Hashable',
+)
+
+
+class EqualityComparable:
+    __slots__ = ()
+
+    id: Union[str, int]
+
+    def __eq__(self, other: object) -> bool:
+        if isinstance(other, self.__class__):
+            return other.id == self.id
+        return NotImplemented
+
+
+class Hashable(EqualityComparable):
+    __slots__ = ()
+
+    def __hash__(self) -> int:
+        return hash(self.id)
```

### Comparing `guilded.py-1.8.0/guilded/asset.py` & `guilded.py-1.9.0/guilded/asset.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.8.0/guilded/backoff.py` & `guilded.py-1.9.0/guilded/backoff.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.8.0/guilded/channel.py` & `guilded.py-1.9.0/guilded/channel.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,31 +62,32 @@
 from .enums import ChannelType, CustomRepeatInterval, DeleteSeriesType, FileType, RSVPStatus, RepeatInterval, Weekday, try_enum
 from .group import Group
 from .message import HasContentMixin
 from .mixins import Hashable
 from .reply import AnnouncementReply, CalendarEventReply, DocReply, ForumTopicReply
 from .user import Member
 from .utils import GUILDED_EPOCH_DATETIME, MISSING, ISO8601, Object
-from .status import Game
 
 if TYPE_CHECKING:
     from .types.announcement import Announcement as AnnouncementPayload
     from .types.calendar_event import (
         CalendarEvent as CalendarEventPayload,
         CalendarEventRsvp as CalendarEventRsvpPayload,
         RepeatInfo as RepeatInfoPayload,
     )
+    from .types.channel import Thread as ThreadPayload
     from .types.doc import Doc as DocPayload
     from .types.list_item import (
         ListItem as ListItemPayload,
         ListItemNote as ListItemNotePayload,
     )
     from .types.forum_topic import ForumTopic as ForumTopicPayload
 
     from .emote import Emote
+    from .message import ChatMessage
     from .role import Role
     from .server import Server
     from .user import User
     from .webhook import Webhook
 
 
 __all__ = (
@@ -106,14 +107,16 @@
     'MediaChannel',
     'ListChannel',
     'ListItem',
     'ListItemNote',
     'PartialMessageable',
     'RepeatInfo',
     'SchedulingChannel',
+    'StreamChannel',
+    'StreamingChannel',
     'TextChannel',
     'Thread',
     'VoiceChannel',
 )
 
 
 class CalendarChannel(guilded.abc.ServerChannel):
@@ -2247,102 +2250,100 @@
     #        transport_id=lobby_connection_data['sendTransportOptions']['id'],
     #        dtls_parameters=dtls_parameters
     #    )
 
 
 class Thread(guilded.abc.ServerChannel, guilded.abc.Messageable):
     """Represents a thread in a :class:`.Server`.
-    """
-    def __init__(self, **fields):
-        super().__init__(**fields)
-        self.type = ChannelType.thread
-    #    data = fields.get('data') or fields.get('channel', {})
-
-    #    self._message_count = data.get('messageCount') or 0
-    #    self.initial_message_id = data.get('threadMessageId')
-    #    self._initial_message = self._state._get_message(self.initial_message_id)
-    #    # This is unlikely to not be None given the temporal nature of message cache
-
-    #    self._participant_ids = []
 
-    #    for user_id in data.get('userIds') or []:
-    #        self._participant_ids.append(user_id)
-
-    #    for member_data in data.get('participants') or []:
-    #        if member_data.get('id'):
-    #            self._participant_ids.append(member_data['id'])
+    Attributes
+    -----------
+    parent_id: :class:`str`
+        The ID of the immediately next higher channel or thread in the thread chain.
+    root_id: :class:`str`
+        The ID of the topmost channel in the thread chain.
+
+        .. versionadded:: 1.9
+    starter_message_id: Optional[:class:`str`]
+        The ID of the message that the thread was created from, if any.
 
-    #@property
-    #def message_count(self) -> int:
-    #    """:class:`int`: The number of messages in the thread.
+        .. versionadded:: 1.9
+    """
 
-    #    This may be inaccurate if this object has existed for an extended
-    #    period of time since it does not get updated by the library when new
-    #    messages are sent within the thread.
-    #    """
-    #    return int(self._message_count)
+    __slots__: Tuple[str, ...] = (
+        'type',
+        'root_id',
+        'parent_id',
+        'starter_message_id',
+    )
 
-    #@property
-    #def initial_message(self) -> Optional[ChatMessage]:
-    #    """Optional[:class:`.ChatMessage`]: The initial message in this thread.
+    def __init__(self, *, data: ThreadPayload, **fields):
+        super().__init__(data=data, **fields)
+        self.type = ChannelType.thread
+        self._channel_id = self.id
 
-    #    This may be ``None`` if the message was not cached when this object was
-    #    created. In this case, you may fetch the message with :meth:`.fetch_initial_message`.
-    #    """
-    #    return self._initial_message
+        self.root_id: str = data.get('rootId')
+        self.parent_id: str = data.get('parentId')
+        self.starter_message_id: Optional[str] = data.get('messageId')
 
-    #@property
-    #def participants(self) -> List[Member]:
-    #    """List[:class:`.Member`]: The cached list of participants in this thread."""
-    #    return [self.server.get_member(member_id) for member_id in self._participant_ids]
+    @property
+    def root(self) -> Optional[ChatChannel | VoiceChannel | StreamChannel]:
+        """Optional[:class:`.ChatChannel` | :class:`.VoiceChannel` | :class:`.StreamChannel`]:
+        The topmost channel in the thread chain
 
-    #async def archive(self) -> None:
-    #    """|coro|
+        .. versionadded:: 1.9
+        """
+        if self.root_id:
+            return self.server.get_channel_or_thread(self.root_id)
 
-    #    Archive this thread.
-    #    """
-    #    request = self._state.archive_thread(self.server_id, self.group_id, self.id)
-    #    await request
+    @property
+    def parent(self) -> Optional[ChatChannel | VoiceChannel | StreamChannel | Thread]:
+        """Optional[:class:`.ChatChannel` | :class:`.VoiceChannel` | :class:`.StreamChannel` | :class:`.Thread`]:
+        The parent channel or thread that the thread belongs to"""
+        if self.parent_id:
+            return self.server.get_channel_or_thread(self.parent_id)
 
-    #async def restore(self) -> None:
-    #    """|coro|
+    @property
+    def starter_message(self) -> Optional[ChatMessage]:
+        """Optional[:class:`.ChatMessage`]: The starter message in the thread,
+        if it exists and is cached.
 
-    #    Restore this thread.
-    #    """
-    #    request = self._state.restore_thread(self.server_id, self.group_id, self.id)
-    #    await request
+        .. versionadded:: 1.9
+        """
+        if self.starter_message_id:
+            return self._state._get_message(self.starter_message_id)
 
-    #async def leave(self) -> None:
-    #    """|coro|
+    async def fetch_starter_message(self) -> Optional[ChatMessage]:
+        """|coro|
 
-    #    Leave this thread.
-    #    """
-    #    request = self._state.leave_thread(self.id)
-    #    await request
+        Fetch the starter message in this thread. Sometimes this may be
+        available via :attr:`.starter_message`, but it is unlikely when
+        dealing with existing threads because it relies on message cache.
 
-    #async def fetch_initial_message(self) -> ChatMessage:
-    #    """|coro|
+        This is roughly equivalent to:
 
-    #    Fetch the initial message in this thread. Sometimes this may be
-    #    available via :attr:`.initial_message`, but it is unlikely when
-    #    dealing with existing threads because it relies on message cache.
+        .. code-block:: python3
 
-    #    This is equivalent to:
+            initial_message = await thread.fetch_message(thread.starter_message_id)
 
-    #    .. code-block:: python3
+        .. versionadded:: 1.9
 
-    #        initial_message = await thread.fetch_message(thread.initial_message_id)
+        Returns
+        --------
+        Optional[:class:`.ChatMessage`]
+            The initial message in the thread, if any.
 
-    #    Returns
-    #    --------
-    #    :class:`.ChatMessage`
-    #        The initial message in the thread.
-    #    """
-    #    message = await self.fetch_message(self.initial_message_id)
-    #    return message
+        Raises
+        -------
+        NotFound
+            The starter message was deleted.
+        """
+        if self.starter_message_id:
+            message = await self.fetch_message(self.starter_message_id)
+            return message
 
 
 class DMChannel(Hashable, guilded.abc.Messageable):
     """Represents a private channel between users.
 
     .. container:: operations
 
@@ -2833,18 +2834,14 @@
             self.url = data['src']
         except KeyError:
             pass
         try:
             self.type = getattr(FileType, data['type'])
         except (KeyError, AttributeError):
             pass
-        try:
-            self.game = Game(game_id=data['gameId'])
-        except KeyError:
-            pass
 
     @property
     def server(self) -> Server:
         """:class:`.Server`: The server that the media is in."""
         return self.channel.server
 
     @property
@@ -3911,14 +3908,24 @@
     #    data = await self._state.create_availability(self.id, start=start, end=end)
     #    for availability_data in data['availabilities']:
     #        availability = Availability(data=availability_data, channel=self, state=self._state)
     #        if availability.id == data['id']:
     #            return availability
 
 
+class StreamChannel(guilded.abc.ServerChannel, guilded.abc.Messageable):
+    """Represents a stream channel in a :class:`.Server`."""
+    def __init__(self, **fields):
+        super().__init__(**fields)
+        self.type = ChannelType.stream
+        self._channel_id = self.id
+
+StreamingChannel = StreamChannel
+
+
 class PartialMessageable(guilded.abc.Messageable, Hashable):
     """Represents a partial messageable to aid with working messageable channels when
     only a channel ID is present.
 
     The only way to construct this class is through :meth:`Client.get_partial_messageable`.
 
     Note that this class is trimmed down and has no rich attributes.
```

### Comparing `guilded.py-1.8.0/guilded/client.py` & `guilded.py-1.9.0/guilded/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -661,15 +661,15 @@
 
         Fetch your list of servers from the API.
 
         .. versionadded:: 1.8
 
         Returns
         --------
-        List[:class:`.Servers`]
+        List[:class:`.Server`]
             The servers you are a member of.
         """
 
         data = await self.http.get_my_servers()
         return [Server(state=self.http, data=server_data) for server_data in data['servers']]
 
     async def fetch_channel(self, channel_id: str) -> ServerChannel:
@@ -717,14 +717,58 @@
         invite = Invite(
             data=data['metadata']['inviteInfo'],
             canonical=data['metadata'].get('canonicalUrl'),
             state=self.http,
         )
         return invite
 
+    async def set_status(self, emote: Emote, *, content: Optional[str] = MISSING) -> None:
+        """|coro|
+
+        Update your custom status.
+
+        This method cannot be used to remove your status.
+        Instead, use :meth:`.remove_status`.
+
+        .. versionadded: 1.9
+
+        Parameters
+        -----------
+        emote: :class:`Emote`
+            The emote displayed to the left of the content.
+
+            .. note::
+
+                Perhaps unexpectedly, this parameter is required by Guilded.
+                If you do not wish to provide it, ``90002547`` is the default
+                emote ID used by the desktop client.
+
+        content: Optional[:class:`str`]
+            The text content of the status.
+        """
+
+        emote_id: int = getattr(emote, 'id', emote)
+        payload = {
+            'emoteId': emote_id,
+        }
+
+        if content is not MISSING:
+            payload['content'] = content
+
+        await self.http.update_my_status(payload)
+
+    async def remove_status(self) -> None:
+        """|coro|
+
+        Remove your custom status.
+
+        .. versionadded: 1.9
+        """
+        await self.http.delete_my_status()
+
     async def on_error(self, event_method, *args, **kwargs) -> None:
         print(f'Ignoring exception in {event_method}:', file=sys.stderr)
         traceback.print_exc()
 
     async def start(self, token: str = None, *, reconnect: bool = True) -> None:
         self.http.token = token or self.http.token
         if not self.http.token:
```

### Comparing `guilded.py-1.8.0/guilded/colour.py` & `guilded.py-1.9.0/guilded/colour.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.8.0/guilded/embed.py` & `guilded.py-1.9.0/guilded/embed.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.8.0/guilded/emote.py` & `guilded.py-1.9.0/guilded/emote.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.8.0/guilded/enums.py` & `guilded.py-1.9.0/guilded/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,15 @@
     'UserType',
     'SocialLinkType',
     'RSVPStatus',
     'RepeatInterval',
     'CustomRepeatInterval',
     'Weekday',
     'DeleteSeriesType',
+    'ServerSubscriptionTierType',
 )
 
 
 def _create_value_cls(name, comparable):
     cls = namedtuple('_EnumValue_' + name, 'name value')
     cls.__repr__ = lambda self: f'<{name}.{self.name}: {self.value!r}>'
     cls.__str__ = lambda self: f'{name}.{self.name}'
@@ -394,14 +395,20 @@
 
 
 class DeleteSeriesType(Enum):
     all = 'all'
     forward = 'fromEventForward'
 
 
+class ServerSubscriptionTierType(Enum):
+    gold = 'Gold'
+    silver = 'Silver'
+    copper = 'Copper'
+
+
 T = TypeVar('T')
 
 
 def create_unknown_value(cls: Type[T], val: Any) -> T:
     value_cls = cls._enum_value_cls_  # type: ignore
     name = f'unknown_{val}'
     return value_cls(name=name, value=val)
```

### Comparing `guilded.py-1.8.0/guilded/errors.py` & `guilded.py-1.9.0/guilded/errors.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.8.0/guilded/events.py` & `guilded.py-1.9.0/guilded/events.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,16 +39,19 @@
     DMChannel,
     ForumTopic,
     ListItem,
     Thread,
     VoiceChannel,
 )
 from .emote import Emote
+from .group import Group
 from .message import ChatMessage
+from .status import Status
 from .reply import AnnouncementReply, CalendarEventReply, DocReply, ForumTopicReply
+from .role import Role
 from .user import Member, MemberBan, SocialLink
 from .utils import ISO8601
 from .webhook.async_ import Webhook
 
 if TYPE_CHECKING:
     from .types import gateway as gw
 
@@ -127,21 +130,30 @@
     'ForumTopicReactionAddEvent',
     'ForumTopicReactionRemoveEvent',
     'ForumTopicReplyCreateEvent',
     'ForumTopicReplyUpdateEvent',
     'ForumTopicReplyDeleteEvent',
     'ForumTopicReplyReactionAddEvent',
     'ForumTopicReplyReactionRemoveEvent',
+    'GroupCreateEvent',
+    'GroupUpdateEvent',
+    'GroupDeleteEvent',
     'ListItemCreateEvent',
     'ListItemUpdateEvent',
     'ListItemDeleteEvent',
     'ListItemCompleteEvent',
     'ListItemUncompleteEvent',
     'MessageReactionAddEvent',
     'MessageReactionRemoveEvent',
+    'BulkMessageReactionRemoveEvent',
+    'UserStatusCreateEvent',
+    'UserStatusDeleteEvent',
+    'RoleCreateEvent',
+    'RoleUpdateEvent',
+    'RoleDeleteEvent',
 )
 
 
 class BaseEvent:
     """Represents a Gateway event for dispatching to event handlers.
 
     All events inherit from this class, and thus have the following attributes:
@@ -799,33 +811,38 @@
         The ID of the server that the channel is in.
     server: :class:`Server`
         The server that the channel is in.
     before: Optional[:class:`.abc.ServerChannel`]
         The channel before modification, if it was cached.
     after: :class:`.abc.ServerChannel`
         The channel after modification.
+
+        .. deprecated:: 1.9
+            The ``channel`` alias.
     """
 
     __gateway_event__ = 'ServerChannelUpdated'
     __dispatch_event__ = 'server_channel_update'
     __slots__: Tuple[str, ...] = (
         'before',
         'after',
+        'channel',
     )
 
     def __init__(
         self,
         state,
         data: gw.ServerChannelEvent,
         /,
     ) -> None:
         super().__init__(state, data)
 
         self.before = self.server.get_channel_or_thread(data['channel']['id'])
-        self.channel: ServerChannel = state.create_channel(data=data['channel'], server=self.server)
+        self.after: ServerChannel = state.create_channel(data=data['channel'], server=self.server)
+        self.channel = self.after
 
 
 class ServerChannelDeleteEvent(_ServerChannelEvent):
     """Represents a :gdocs:`ServerChannelDeleted <websockets/ServerChannelDeleted>` event for dispatching to event handlers.
 
     Attributes
     -----------
@@ -2443,14 +2460,81 @@
         The emote that the reaction shows.
     """
 
     __gateway_event__ = 'ForumTopicCommentReactionDeleted'
     __dispatch_event__ = 'forum_topic_reply_reaction_remove'
 
 
+class _GroupEvent(ServerEvent):
+    __slots__: Tuple[str, ...] = (
+        'group',
+    )
+
+    def __init__(
+        self,
+        state,
+        data: gw.GroupEvent,
+        /,
+    ) -> None:
+        super().__init__(state, data)
+
+        self.group = Group(state=state, data=data['group'], server=self.server)
+
+
+class GroupCreateEvent(_GroupEvent):
+    """Represents a :gdocs:`GroupCreated <websockets/GroupCreated>` event for dispatching to event handlers.
+
+    Attributes
+    -----------
+    server_id: :class:`str`
+        The ID of the server that the group is in.
+    server: :class:`Server`
+        The server that the group is in.
+    group: :class:`Group`
+        The group that was created.
+    """
+
+    __gateway_event__ = 'GroupCreated'
+    __dispatch_event__ = 'group_create'
+
+
+class GroupUpdateEvent(_GroupEvent):
+    """Represents a :gdocs:`GroupUpdated <websockets/GroupUpdated>` event for dispatching to event handlers.
+
+    Attributes
+    -----------
+    server_id: :class:`str`
+        The ID of the server that the group is in.
+    server: :class:`Server`
+        The server that the group is in.
+    group: :class:`Group`
+        The group after modification.
+    """
+
+    __gateway_event__ = 'GroupUpdated'
+    __dispatch_event__ = 'group_update'
+
+
+class GroupDeleteEvent(_GroupEvent):
+    """Represents a :gdocs:`GroupDeleted <websockets/GroupDeleted>` event for dispatching to event handlers.
+
+    Attributes
+    -----------
+    server_id: :class:`str`
+        The ID of the server that the group was in.
+    server: :class:`Server`
+        The server that the group was in.
+    group: :class:`Group`
+        The group that was deleted.
+    """
+
+    __gateway_event__ = 'GroupDeleted'
+    __dispatch_event__ = 'group_delete'
+
+
 class _ListItemEvent(ServerEvent):
     __slots__: Tuple[str, ...] = (
         'channel',
         'item',
     )
 
     def __init__(
@@ -2557,29 +2641,55 @@
         The list item that was uncompleted.
     """
 
     __gateway_event__ = 'ListItemUncompleted'
     __dispatch_event__ = 'list_item_uncomplete'
 
 
-class _MessageReactionEvent(ServerEvent):
+class MessageReactionAddEvent(ServerEvent):
+    """Represents a :gdocs:`ChannelMessageReactionCreated <websockets/ChannelMessageReactionCreated>` event for dispatching to event handlers.
+
+    Attributes
+    -----------
+    server_id: :class:`str`
+        The ID of the server that the reaction is in.
+    server: :class:`Server`
+        The server that the reaction is in.
+    channel: Union[:class:`ChatChannel`, :class:`VoiceChannel`, :class:`Thread`, :class:`DMChannel`]
+        The channel that the reaction is in.
+    message: Optional[:class:`ChatMessage`]
+        The message that the reaction is on, if it is cached.
+    member: Optional[:class:`Member`]
+        The member that added the reaction, if they are cached.
+    channel_id: :class:`str`
+        The ID of the channel that the reaction is in.
+    message_id: :class:`str`
+        The ID of the message that the reaction is on.
+    user_id: :class:`str`
+        The ID of the user that added the reaction.
+    emote: :class:`Emote`
+        The emote that the reaction shows.
+    """
+
+    __gateway_event__ = 'ChannelMessageReactionCreated'
+    __dispatch_event__ = 'message_reaction_add'
     __slots__: Tuple[str, ...] = (
         'channel_id',
         'message_id',
         'user_id',
         'emote',
         'channel',
         'message',
         'member',
     )
 
     def __init__(
         self,
         state,
-        data: gw.ChannelMessageReactionEvent,
+        data: gw.ChannelMessageReactionCreatedEvent,
         /,
         channel: Union[ChatChannel, VoiceChannel, Thread, DMChannel],
     ) -> None:
         super().__init__(state, data)
 
         self.channel_id = data['reaction']['channelId']
         self.message_id = data['reaction']['messageId']
@@ -2587,63 +2697,292 @@
         self.emote = Emote(state=state, data=data['reaction']['emote'])
 
         self.channel = channel
         self.message: Optional[ChatMessage] = state._get_message(self.message_id)
         self.member = self.server.get_member(self.user_id)
 
 
-class MessageReactionAddEvent(_MessageReactionEvent):
-    """Represents a :gdocs:`ChannelMessageReactionCreated <websockets/ChannelMessageReactionCreated>` event for dispatching to event handlers.
+class MessageReactionRemoveEvent(ServerEvent):
+    """Represents a :gdocs:`ChannelMessageReactionDeleted <websockets/ChannelMessageReactionDeleted>` event for dispatching to event handlers.
 
     Attributes
     -----------
     server_id: :class:`str`
-        The ID of the server that the reaction is in.
+        The ID of the server that the reaction was in.
     server: :class:`Server`
-        The server that the reaction is in.
+        The server that the reaction was in.
     channel: Union[:class:`ChatChannel`, :class:`VoiceChannel`, :class:`Thread`, :class:`DMChannel`]
-        The channel that the reaction is in.
+        The channel that the reaction was in.
     message: Optional[:class:`ChatMessage`]
-        The message that the reaction is on, if it is cached.
+        The message that the reaction was on, if it is cached.
     member: Optional[:class:`Member`]
         The member that added the reaction, if they are cached.
+    deleted_by: Optional[:class:`Member`]
+        The member that removed the reaction, if they are cached.
     channel_id: :class:`str`
-        The ID of the channel that the reaction is in.
+        The ID of the channel that the reaction was in.
     message_id: :class:`str`
-        The ID of the message that the reaction is on.
+        The ID of the message that the reaction was on.
     user_id: :class:`str`
         The ID of the user that added the reaction.
+    deleted_by_id: :class:`str`
+        The ID of the user that removed the reaction.
     emote: :class:`Emote`
-        The emote that the reaction shows.
+        The emote that the reaction showed.
     """
 
-    __gateway_event__ = 'ChannelMessageReactionCreated'
-    __dispatch_event__ = 'message_reaction_add'
+    __gateway_event__ = 'ChannelMessageReactionDeleted'
+    __dispatch_event__ = 'message_reaction_remove'
+    __slots__: Tuple[str, ...] = (
+        'channel_id',
+        'message_id',
+        'user_id',
+        'deleted_by_id',
+        'emote',
+        'channel',
+        'message',
+        'member',
+        'deleted_by',
+    )
 
+    def __init__(
+        self,
+        state,
+        data: gw.ChannelMessageReactionDeletedEvent,
+        /,
+        channel: Union[ChatChannel, VoiceChannel, Thread, DMChannel],
+    ) -> None:
+        super().__init__(state, data)
 
-class MessageReactionRemoveEvent(_MessageReactionEvent):
-    """Represents a :gdocs:`ChannelMessageReactionDeleted <websockets/ChannelMessageReactionDeleted>` event for dispatching to event handlers.
+        self.channel_id = data['reaction']['channelId']
+        self.message_id = data['reaction']['messageId']
+        self.user_id = data['reaction']['createdBy']
+        self.deleted_by_id = data['deletedBy']
+        self.emote = Emote(state=state, data=data['reaction']['emote'])
+
+        self.channel = channel
+        self.message: Optional[ChatMessage] = state._get_message(self.message_id)
+        self.member = self.server.get_member(self.user_id)
+        self.deleted_by = self.server.get_member(self.deleted_by_id)
+
+
+class BulkMessageReactionRemoveEvent(ServerEvent):
+    """Represents a :gdocs:`ChannelMessageReactionManyDeleted <websockets/ChannelMessageReactionManyDeleted>` event for dispatching to event handlers.
+
+    .. versionadded: 1.9
 
     Attributes
     -----------
     server_id: :class:`str`
-        The ID of the server that the reaction is in.
+        The ID of the server that the reactions were in.
     server: :class:`Server`
-        The server that the reaction is in.
+        The server that the reactions were in.
     channel: Union[:class:`ChatChannel`, :class:`VoiceChannel`, :class:`Thread`, :class:`DMChannel`]
-        The channel that the reaction is in.
+        The channel that the reactions were in.
     message: Optional[:class:`ChatMessage`]
-        The message that the reaction is on, if it is cached.
-    member: Optional[:class:`Member`]
-        The member that added the reaction, if they are cached.
+        The message that the reactions were on, if it is cached.
     channel_id: :class:`str`
-        The ID of the channel that the reaction is in.
+        The ID of the channel that the reactions were in.
     message_id: :class:`str`
-        The ID of the message that the reaction is on.
+        The ID of the message that the reactions were on.
     user_id: :class:`str`
         The ID of the user that added the reaction.
-    emote: :class:`Emote`
-        The emote that the reaction shows.
+    deleted_by_id: :class:`str`
+        The ID of the user that removed the reactions.
+    deleted_by: Optional[:class:`Member`]
+        The member that removed the reactions, if they are cached.
+    count: :class:`int`
+        The number of reactions that were removed.
+    emote: Optional[:class:`Emote`]
+        The emote that the reactions showed, if applicable.
     """
 
-    __gateway_event__ = 'ChannelMessageReactionDeleted'
-    __dispatch_event__ = 'message_reaction_remove'
+    __gateway_event__ = 'ChannelMessageReactionManyDeleted'
+    __dispatch_event__ = 'bulk_message_reaction_remove'
+
+    __slots__: Tuple[str, ...] = (
+        'channel_id',
+        'message_id',
+        'user_id',
+        'deleted_by_id',
+        'count',
+        'emote',
+        'channel',
+        'message',
+        'deleted_by',
+    )
+
+    def __init__(
+        self,
+        state,
+        data: gw.ChannelMessageReactionManyDeletedEvent,
+        /,
+        channel: Union[ChatChannel, VoiceChannel, Thread, DMChannel],
+    ) -> None:
+        super().__init__(state, data)
+
+        self.channel_id = data['channelId']
+        self.message_id = data['messageId']
+        self.deleted_by_id = data['deletedBy']
+        self.count = data['count']
+        self.emote = Emote(state=state, data=data.get('emote')) if data.get('emote') else None
+
+        self.channel = channel
+        self.message: Optional[ChatMessage] = state._get_message(self.message_id)
+        self.deleted_by = self.server.get_member(self.deleted_by_id)
+
+
+class UserStatusCreateEvent(BaseEvent):
+    """Represents a :gdocs:`UserStatusCreated <websockets/UserStatusCreated>` event for dispatching to event handlers.
+
+    Attributes
+    -----------
+    user_id: :class:`str`
+        The ID of the user that updated their status.
+    user: Optional[:class:`~guilded.User`]
+        The user that updated their status.
+    status: :class:`.Status`
+        The new status.
+    expires_at: Optional[:class:`datetime.datetime`]
+        When the status will expire, if applicable.
+    """
+
+    __gateway_event__ = 'UserStatusCreated'
+    __dispatch_event__ = 'user_status_create'
+    __slots__: Tuple[str, ...] = (
+        'user_id',
+        'user',
+        'status',
+        'expires_at',
+    )
+
+    def __init__(
+        self,
+        state,
+        data: gw.UserStatusCreatedEvent,
+        /,
+    ) -> None:
+        super().__init__(state, data)
+
+        self.user_id = data['userId']
+        self.user: Optional[User] = state._get_user(self.user_id)
+
+        self.status = Status(data=data['userStatus'])
+        self.expires_at = ISO8601(data.get('expiresAt'))
+
+
+class UserStatusDeleteEvent(BaseEvent):
+    """Represents a :gdocs:`UserStatusDeleted <websockets/UserStatusDeleted>` event for dispatching to event handlers.
+
+    Attributes
+    -----------
+    user_id: :class:`str`
+        The ID of the user that deleted their status.
+    user: Optional[:class:`~guilded.User`]
+        The user that deleted their status.
+    status: :class:`.Status`
+        The status that was deleted.
+    """
+
+    __gateway_event__ = 'UserStatusDeleted'
+    __dispatch_event__ = 'user_status_delete'
+    __slots__: Tuple[str, ...] = (
+        'user_id',
+        'user',
+        'status',
+    )
+
+    def __init__(
+        self,
+        state,
+        data: gw.UserStatusDeletedEvent,
+        /,
+    ) -> None:
+        super().__init__(state, data)
+
+        self.user_id = data['userId']
+        self.user: Optional[User] = state._get_user(self.user_id)
+
+        self.status = Status(data=data['userStatus'])
+
+
+class _RoleEvent(ServerEvent):
+    __slots__: Tuple[str, ...] = (
+        'role',
+    )
+
+    def __init__(
+        self,
+        state,
+        data: gw.RoleEvent,
+        /,
+    ) -> None:
+        super().__init__(state, data)
+        self.role = Role(state=state, data=data['role'])
+
+
+class RoleCreateEvent(_RoleEvent):
+    """Represents a :gdocs:`RoleCreated <websockets/RoleCreated>` event for dispatching to event handlers.
+
+    Attributes
+    -----------
+    server_id: :class:`str`
+        The ID of the server that the role is in.
+    server: :class:`Server`
+        The server that the role is in.
+    role: :class:`.Role`
+        The role that was created.
+    """
+
+    __gateway_event__ = 'RoleCreated'
+    __dispatch_event__ = 'role_create'
+
+
+class RoleUpdateEvent(ServerEvent):
+    """Represents a :gdocs:`RoleUpdated <websockets/RoleUpdated>` event for dispatching to event handlers.
+
+    Attributes
+    -----------
+    server_id: :class:`str`
+        The ID of the server that the role is in.
+    server: :class:`Server`
+        The server that the role is in.
+    before: Optional[:class:`.Role`]
+        The role before modification, if it was cached.
+    after: :class:`.Role`
+        The role after modification.
+    """
+
+    __gateway_event__ = 'RoleUpdated'
+    __dispatch_event__ = 'role_update'
+    __slots__: Tuple[str, ...] = (
+        'before',
+        'after',
+    )
+
+    def __init__(
+        self,
+        state,
+        data: gw.RoleEvent,
+        /,
+    ) -> None:
+        super().__init__(state, data)
+
+        self.before = self.server.get_role(data['role']['id'])
+        self.after = Role(state=state, data=data['role'])
+
+
+class RoleDeleteEvent(_RoleEvent):
+    """Represents a :gdocs:`RoleDeleted <websockets/RoleDeleted>` event for dispatching to event handlers.
+
+    Attributes
+    -----------
+    server_id: :class:`str`
+        The ID of the server that the role was in.
+    server: :class:`Server`
+        The server that the role was in.
+    role: :class:`.Role`
+        The role that was deleted.
+    """
+
+    __gateway_event__ = 'RoleDeleted'
+    __dispatch_event__ = 'role_delete'
```

### Comparing `guilded.py-1.8.0/guilded/ext/commands/_types.py` & `guilded.py-1.9.0/guilded/ext/commands/_types.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.8.0/guilded/ext/commands/bot.py` & `guilded.py-1.9.0/guilded/ext/commands/bot.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,16 +83,15 @@
 
 
 def when_mentioned(bot: BotBase, message: guilded.Message, /) -> List[str]:
     """A callable that implements a command prefix equivalent to being mentioned.
 
     These are meant to be passed into the :attr:`.Bot.command_prefix` attribute.
     """
-    # bot.user will never be None when this is called
-    return [f'<@{bot.user.id}> ']  # type: ignore
+    return [f'<@{bot.user_id}> ']
 
 
 def when_mentioned_or(*prefixes: str) -> Callable[[BotBase, guilded.Message], List[str]]:
     """A callable that implements when mentioned or other prefixes provided.
 
     These are meant to be passed into the :attr:`.Bot.command_prefix` attribute.
 
@@ -421,15 +420,15 @@
             Whether the user is the owner.
         """
         if self.owner_id:
             return user.id == self.owner_id
         elif self.owner_ids:
             return user.id in self.owner_ids
         else:
-            return user.id == self.user.id
+            return user.id == self.user_id
 
     async def get_prefix(self, message: guilded.ChatMessage, /) -> Union[List[str], str]:
         """|coro|
 
         Retrieves the prefix the bot is listening to with the message as a context.
 
         Parameters
@@ -463,15 +462,15 @@
 
         return ret
 
     async def get_context(self, message: guilded.ChatMessage, /, *, cls = Context) -> Context:
         view = StringView(str(message.content))
         ctx = cls(prefix=None, view=view, bot=self, message=message)
 
-        if self._skip_check(message.author.id, self.user.id):
+        if self._skip_check(message.author.id, self.user_id):
             return ctx
 
         prefix = await self.get_prefix(message)
         invoked_prefix = prefix
 
         if isinstance(prefix, str):
             if not view.skip_string(prefix):
```

### Comparing `guilded.py-1.8.0/guilded/ext/commands/cog.py` & `guilded.py-1.9.0/guilded/ext/commands/cog.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.8.0/guilded/ext/commands/context.py` & `guilded.py-1.9.0/guilded/ext/commands/context.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.8.0/guilded/ext/commands/converters.py` & `guilded.py-1.9.0/guilded/ext/commands/converters.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,15 +104,14 @@
     'ServerConverter',
     'ChatMessageConverter',
     'MessageConverter',
     'ColourConverter',
     'ColorConverter',
     'EmoteConverter',
     'EmojiConverter',
-    'GameConverter',
     'RoleConverter',
     'Greedy',
     'clean_content',
     'run_converters',
 )
 
 
@@ -257,30 +256,35 @@
     async def convert(self, ctx: Context, argument: str) -> guilded.Member:
         bot = ctx.bot
         match = self._get_id_match(argument)
         server = ctx.server
         result = None
         user_id = None
         if match is None:
-            # not a mention
+            # not an ID
             result = self.find_member_named(server, argument)
         else:
             user_id = match.group(1)
             if server:
                 result = server.get_member(user_id) or _utils_get(ctx.message.mentions, id=user_id)
             else:
                 result = _get_from_servers(bot, 'get_member', user_id)
 
         if result is None:
             if server is None:
                 raise MemberNotFound(argument)
 
             if user_id is not None:
-                result = await server.getch_member(user_id)
-            else:
+                try:
+                    result = await server.getch_member(user_id)
+                except:
+                    pass
+
+            if not result:
+                # At this point, the argument is definitely not an ID
                 result = self.find_member_named(server, argument)
 
             if not result:
                 raise MemberNotFound(argument)
 
         return result
 
@@ -367,18 +371,18 @@
 
     1. Lookup by ID
     2. Lookup by mention
     3. Lookup by name.
     """
 
     async def convert(self, ctx: Context, argument: str) -> guilded.abc.GuildChannel:
-        return self._resolve_channel(ctx, argument, 'channels', guilded.abc.GuildChannel)
+        return await self._resolve_channel(ctx, argument, 'channels', guilded.abc.GuildChannel)
 
     @staticmethod
-    def _resolve_channel(ctx: Context, argument: str, attribute: str, type: Type[CT]) -> CT:
+    async def _resolve_channel(ctx: Context, argument: str, attribute: str, type: Type[CT]) -> CT:
         bot = ctx.bot
 
         match = UUIDConverter._get_id_match(argument) or re.match(r'<#(\b[0-9a-f]{8}\b-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-\b[0-9a-f]{12}\b)>$', argument)
         result = None
         server = ctx.server
 
         if match is None:
@@ -390,42 +394,47 @@
 
                 def check(c):
                     return isinstance(c, type) and c.name == argument
 
                 result = _utils_find(check, bot.get_all_channels())  # type: ignore
         else:
             channel_id = match.group(1)
-            if server:
-                # server.get_channel returns an explicit union instead of the base class
-                result = server.get_channel(channel_id)  # type: ignore
-            else:
-                result = _get_from_servers(bot, 'get_channel', channel_id)
+            try:
+                result = await ctx.bot.getch_channel(channel_id)
+            except:
+                pass
+
+            if server and result and result.server_id != server.id:
+                raise ChannelNotFound(argument)
 
         if not isinstance(result, type):
             raise ChannelNotFound(argument)
 
         return result
 
     @staticmethod
-    def _resolve_thread(ctx: Context, argument: str, attribute: str, type: Type[TT]) -> TT:
+    async def _resolve_thread(ctx: Context, argument: str, attribute: str, type: Type[TT]) -> TT:
         match = UUIDConverter._get_id_match(argument) or re.match(r'<#(\b[0-9a-f]{8}\b-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-\b[0-9a-f]{12}\b)>$', argument)
         result = None
         server = ctx.server
 
         if match is None:
             # not a mention
             if server:
                 iterable: Iterable[TT] = getattr(server, attribute)
                 result: Optional[TT] = _utils_get(iterable, name=argument)
         else:
             thread_id = match.group(1)
             if server:
-                result = server.get_thread(thread_id)  # type: ignore
+                try:
+                    result = server.get_thread(thread_id) or await ctx.bot.fetch_channel(thread_id)
+                except:
+                    pass
 
-        if not result or not isinstance(result, type):
+        if not result or not isinstance(result, type) or (server and result.server_id != server.id):
             raise ThreadNotFound(argument)
 
         return result
 
 GuildChannelConverter = ServerChannelConverter  # discord.py
 
 
@@ -438,15 +447,15 @@
     The lookup strategy is as follows (in order):
 
     1. Lookup by ID
     2. Lookup by mention
     3. Lookup by name
     """
 
-    async def convert(self, ctx: Context, argument: str) -> guilded.AnnouncementChannel:
+    def convert(self, ctx: Context, argument: str) -> guilded.AnnouncementChannel:
         return ServerChannelConverter._resolve_channel(ctx, argument, 'announcement_channels', guilded.AnnouncementChannel)
 
 
 class ChatChannelConverter(UUIDConverter[guilded.ChatChannel]):
     """Converts to a :class:`~guilded.ChatChannel`.
 
     All lookups are via the local server. If in a DM context, then the lookup
@@ -455,15 +464,15 @@
     The lookup strategy is as follows (in order):
 
     1. Lookup by ID
     2. Lookup by mention
     3. Lookup by name
     """
 
-    async def convert(self, ctx: Context, argument: str) -> guilded.ChatChannel:
+    def convert(self, ctx: Context, argument: str) -> guilded.ChatChannel:
         return ServerChannelConverter._resolve_channel(ctx, argument, 'chat_channels', guilded.ChatChannel)
 
 TextChannelConverter = ChatChannelConverter  # discord.py
 
 
 class DocsChannelConverter(UUIDConverter[guilded.DocsChannel]):
     """Converts to a :class:`~guilded.DocsChannel`.
@@ -474,15 +483,15 @@
     The lookup strategy is as follows (in order):
 
     1. Lookup by ID
     2. Lookup by mention
     3. Lookup by name
     """
 
-    async def convert(self, ctx: Context, argument: str) -> guilded.DocsChannel:
+    def convert(self, ctx: Context, argument: str) -> guilded.DocsChannel:
         return ServerChannelConverter._resolve_channel(ctx, argument, 'docs_channels', guilded.DocsChannel)
 
 
 class ForumChannelConverter(UUIDConverter[guilded.ForumChannel]):
     """Converts to a :class:`~guilded.ForumChannel`.
 
     All lookups are via the local server. If in a DM context, then the lookup
@@ -491,15 +500,15 @@
     The lookup strategy is as follows (in order):
 
     1. Lookup by ID
     2. Lookup by mention
     3. Lookup by name
     """
 
-    async def convert(self, ctx: Context, argument: str) -> guilded.ForumChannel:
+    def convert(self, ctx: Context, argument: str) -> guilded.ForumChannel:
         return ServerChannelConverter._resolve_channel(ctx, argument, 'forum_channels', guilded.ForumChannel)
 
 
 class ListChannelConverter(UUIDConverter[guilded.ListChannel]):
     """Converts to a :class:`~guilded.ListChannel`.
 
     All lookups are via the local server. If in a DM context, then the lookup
@@ -508,15 +517,15 @@
     The lookup strategy is as follows (in order):
 
     1. Lookup by ID
     2. Lookup by mention
     3. Lookup by name
     """
 
-    async def convert(self, ctx: Context, argument: str) -> guilded.ListChannel:
+    def convert(self, ctx: Context, argument: str) -> guilded.ListChannel:
         return ServerChannelConverter._resolve_channel(ctx, argument, 'list_channels', guilded.ListChannel)
 
 
 class MediaChannelConverter(UUIDConverter[guilded.MediaChannel]):
     """Converts to a :class:`~guilded.MediaChannel`.
 
     All lookups are via the local server. If in a DM context, then the lookup
@@ -525,15 +534,15 @@
     The lookup strategy is as follows (in order):
 
     1. Lookup by ID
     2. Lookup by mention
     3. Lookup by name
     """
 
-    async def convert(self, ctx: Context, argument: str) -> guilded.MediaChannel:
+    def convert(self, ctx: Context, argument: str) -> guilded.MediaChannel:
         return ServerChannelConverter._resolve_channel(ctx, argument, 'media_channels', guilded.MediaChannel)
 
 
 class SchedulingChannelConverter(UUIDConverter[guilded.SchedulingChannel]):
     """Converts to a :class:`~guilded.SchedulingChannel`.
 
     All lookups are via the local server. If in a DM context, then the lookup
@@ -542,15 +551,15 @@
     The lookup strategy is as follows (in order):
 
     1. Lookup by ID
     2. Lookup by mention
     3. Lookup by name
     """
 
-    async def convert(self, ctx: Context, argument: str) -> guilded.SchedulingChannel:
+    def convert(self, ctx: Context, argument: str) -> guilded.SchedulingChannel:
         return ServerChannelConverter._resolve_channel(ctx, argument, 'scheduling_channels', guilded.SchedulingChannel)
 
 
 class ThreadConverter(UUIDConverter[guilded.Thread]):
     """Converts to a :class:`~guilded.Thread`.
 
     All lookups are via the local server. If in a DM context, then the lookup
@@ -559,15 +568,15 @@
     The lookup strategy is as follows (in order):
 
     1. Lookup by ID
     2. Lookup by mention
     3. Lookup by name
     """
 
-    async def convert(self, ctx: Context, argument: str) -> guilded.Thread:
+    def convert(self, ctx: Context, argument: str) -> guilded.Thread:
         return ServerChannelConverter._resolve_thread(ctx, argument, 'threads', guilded.Thread)
 
 
 class VoiceChannelConverter(UUIDConverter[guilded.VoiceChannel]):
     """Converts to a :class:`~guilded.VoiceChannel`.
 
     All lookups are via the local server. If in a DM context, then the lookup
@@ -576,15 +585,15 @@
     The lookup strategy is as follows (in order):
 
     1. Lookup by ID
     2. Lookup by mention
     3. Lookup by name
     """
 
-    async def convert(self, ctx: Context, argument: str) -> guilded.VoiceChannel:
+    def convert(self, ctx: Context, argument: str) -> guilded.VoiceChannel:
         return ServerChannelConverter._resolve_channel(ctx, argument, 'voice_channels', guilded.VoiceChannel)
 
 
 class ServerConverter(GenericIDConverter[guilded.Server]):
     """Converts to a :class:`~guilded.Server`.
 
     The lookup strategy is as follows (in order):
@@ -679,42 +688,14 @@
             if arg.startswith('from_') or method is None or not inspect.ismethod(method):
                 raise BadColourArgument(arg)
             return method()
 
 ColorConverter = ColourConverter
 
 
-class GameConverter(Converter[guilded.Game]):
-    """Converts to a :class:`~guilded.Game`.
-
-    :attr:`~guilded.Game.MAPPING` must be populated for this converter to work
-    as expected. Call :meth:`~guilded.Client.fill_game_list` at least
-    once in your process's lifetime to ensure this.
-
-    The lookup strategy is as follows (in order):
-
-    1. Lookup by ID
-    2. Lookup by name
-    """
-
-    async def convert(self, ctx: Context, argument: str):
-        if not guilded.Game.MAPPING:
-            raise BadGameArgument(argument)
-
-        result = None
-        if argument in guilded.Game.MAPPING.keys():
-            result = guilded.Game(game_id=argument)
-        elif argument in guilded.Game.MAPPING.values():
-            result = guilded.Game(name=argument)
-        else:
-            raise GameNotFound(argument)
-
-        return result
-
-
 class RoleConverter(IntIDConverter[guilded.Role]):
     """Converts to a :class:`~guilded.Role`.
 
     All lookups are via the local server. If in a DM context, the converter raises
     the :exc:`.NoPrivateMessage` exception.
 
     The lookup strategy is as follows (in order):
@@ -725,21 +706,30 @@
     """
 
     async def convert(self, ctx: Context, argument: str):
         server = ctx.server
         if not server:
             raise NoPrivateMessage()
 
+        if len(server.roles) == 0:
+            # Every server has at least the base role,
+            # so we know our cache is improperly filled
+            await server.fill_roles()
+
         result = None
         match = self._get_id_match(argument)
 
         if match is not None:
             role_id = int(match.group(1))
-            result = server.get_role(role_id)
-        else:
+            try:
+                result = await server.getch_role(role_id)
+            except:
+                pass
+
+        if not result:
             result = _utils_get(server.roles, name=argument)
 
         if not result:
             raise RoleNotFound(argument)
 
         return result
 
@@ -911,15 +901,14 @@
     guilded.AnnouncementChannel: AnnouncementChannelConverter,
     guilded.ChatChannel: ChatChannelConverter,
     guilded.ChatMessage: ChatMessageConverter,
     guilded.Colour: ColourConverter,
     guilded.DocsChannel: DocsChannelConverter,
     guilded.Emote: EmoteConverter,
     guilded.ForumChannel: ForumChannelConverter,
-    guilded.Game: GameConverter,
     guilded.ListChannel: ListChannelConverter,
     guilded.MediaChannel: MediaChannelConverter,
     guilded.Member: MemberConverter,
     guilded.Object: ObjectConverter,
     guilded.Role: RoleConverter,
     guilded.SchedulingChannel: SchedulingChannelConverter,
     guilded.Server: ServerConverter,
```

### Comparing `guilded.py-1.8.0/guilded/ext/commands/cooldowns.py` & `guilded.py-1.9.0/guilded/ext/commands/cooldowns.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.8.0/guilded/ext/commands/core.py` & `guilded.py-1.9.0/guilded/ext/commands/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -73,34 +73,36 @@
 
 
 __all__ = (
     'Command',
     'Group',
     'command',
     'group',
-    # 'has_role',
+    'has_role',
     # 'has_permissions',
-    # 'has_any_role',
+    'has_any_role',
     'check',
     'check_any',
     'before_invoke',
     'after_invoke',
-    # 'bot_has_role',
+    'bot_has_role',
     # 'bot_has_permissions',
-    # 'bot_has_any_role',
+    'bot_has_any_role',
     'cooldown',
     'dynamic_cooldown',
     'max_concurrency',
     'dm_only',
     'server_only',
     'guild_only',
     'is_owner',
     'is_nsfw',
-    # 'has_server_permissions',
-    # 'bot_has_server_permissions',
+    'has_server_permissions',
+    'has_guild_permissions',
+    'bot_has_server_permissions',
+    'bot_has_guild_permissions',
 )
 
 
 T = TypeVar('T')
 
 
 def hooked_wrapped_callback(command, ctx, coro):
@@ -1666,7 +1668,243 @@
         if isinstance(func, Command):
             func._max_concurrency = value
         else:
             func.__commands_max_concurrency__ = value
         return func
 
     return decorator  # type: ignore
+
+
+def has_role(item: Union[int, str], /) -> Check[Any]:
+    """A :func:`.check` that is added that checks if the member invoking the
+    command has the role specified via the name or ID specified.
+
+    If a string is specified, you must give the exact name of the role, including
+    caps and spelling.
+
+    If an integer is specified, you must give the ID of the role.
+
+    This check raises one of two special exceptions, :exc:`.MissingRole` if the user
+    is missing a role, or :exc:`.NoPrivateMessage` if it is used in a private message.
+    Both inherit from :exc:`.CheckFailure`.
+
+    .. versionadded:: 1.9
+
+    Parameters
+    -----------
+    item: Union[:class:`int`, :class:`str`]
+        The name or ID of the role to check.
+    """
+
+    def predicate(ctx: Context) -> bool:
+        if ctx.server is None:
+            raise NoPrivateMessage()
+
+        # ctx.server is None doesn't narrow ctx.author to Member
+        if isinstance(item, int):
+            # This is more reliable since server roles are often unfilled,
+            # but member instances should usually have role IDs
+            role = item in ctx.author._role_ids  # type: ignore
+        else:
+            role = guilded.utils.get(ctx.author.roles, name=item) is not None  # type: ignore
+
+        if not role:
+            raise MissingRole(item)
+
+        return True
+
+    return check(predicate)
+
+
+def has_any_role(*items: Union[int, str]) -> Callable[[T], T]:
+    r"""A :func:`.check` that is added that checks if the member invoking the
+    command has **any** of the roles specified. This means that if they have
+    one out of the three roles specified, then this check will return ``True``.
+
+    Similar to :func:`.has_role`\, the names or IDs passed in must be exact.
+
+    This check raises one of two special exceptions, :exc:`.MissingAnyRole` if the user
+    is missing all roles, or :exc:`.NoPrivateMessage` if it is used in a private message.
+    Both inherit from :exc:`.CheckFailure`.
+
+    .. versionadded:: 1.9
+
+    Parameters
+    -----------
+    items: List[Union[:class:`str`, :class:`int`]]
+        An argument list of names or IDs to check for roles that the member has.
+
+    Example
+    --------
+
+    .. code-block:: python3
+
+        @bot.command()
+        @commands.has_any_role('Library Developer', 'Moderator', 23218717)
+        async def cool(ctx):
+            await ctx.send('You are cool indeed')
+    """
+
+    def predicate(ctx: Context):
+        if ctx.server is None:
+            raise NoPrivateMessage()
+
+        # ctx.server is None doesn't narrow ctx.author to Member
+        if any(
+            item in ctx.author._role_ids
+            if isinstance(item, int)
+            else guilded.utils.get(ctx.author.roles, name=item) is not None
+            for item in items
+        ):
+            return True
+
+        raise MissingAnyRole(list(items))
+
+    return check(predicate)
+
+
+def bot_has_role(item: int, /) -> Callable[[T], T]:
+    """Similar to :func:`.has_role` except checks if the bot itself has the
+    role.
+
+    This check raises one of two special exceptions, :exc:`.BotMissingRole` if the bot
+    is missing the role, or :exc:`.NoPrivateMessage` if it is used in a private message.
+    Both inherit from :exc:`.CheckFailure`.
+
+    .. versionadded:: 1.9
+    """
+
+    def predicate(ctx: Context):
+        if ctx.server is None:
+            raise NoPrivateMessage()
+
+        if isinstance(item, int):
+            role = item in ctx.me._role_ids
+        else:
+            role = guilded.utils.get(ctx.me.roles, name=item) is not None
+
+        if not role:
+            raise BotMissingRole(item)
+
+        return True
+
+    return check(predicate)
+
+
+def bot_has_any_role(*items: int) -> Callable[[T], T]:
+    """Similar to :func:`.has_any_role` except checks if the bot itself has
+    any of the roles listed.
+
+    This check raises one of two special exceptions, :exc:`.BotMissingAnyRole` if the bot
+    is missing all roles, or :exc:`.NoPrivateMessage` if it is used in a private message.
+    Both inherit from :exc:`.CheckFailure`.
+
+    .. versionadded:: 1.9
+    """
+
+    def predicate(ctx: Context):
+        if ctx.server is None:
+            raise NoPrivateMessage()
+
+        me = ctx.me
+        if any(
+            item in me._role_ids
+            if isinstance(item, int)
+            else guilded.utils.get(me.roles, name=item) is not None
+            for item in items
+        ):
+            return True
+
+        raise BotMissingAnyRole(list(items))
+
+    return check(predicate)
+
+
+def has_server_permissions(**perms: bool) -> Check[Any]:
+    """A :func:`.check` that is added that checks if the member has all of
+    the permissions necessary at the server level.
+
+    The permissions passed in must be exactly like the properties shown under
+    :class:`~guilded.Permissions`.
+
+    This check raises a special exception, :exc:`.MissingPermissions`
+    that is inherited from :exc:`.CheckFailure`.
+
+    If this check is called in a DM context, it will raise an
+    exception, :exc:`.NoPrivateMessage`.
+
+    .. versionadded:: 1.9
+
+    Parameters
+    -----------
+    perms
+        An argument list of permissions to check for.
+
+    Example
+    --------
+
+    .. code-block:: python3
+
+        @bot.command()
+        @commands.has_server_permissions(manage_messages=True)
+        async def test(ctx):
+            await ctx.send('You can manage messages in this server.')
+
+    """
+
+    # I'm aware that this is open to false positives
+    # e.g. if the user passes `values=True`.
+    # But since Guilded permissions are not flag-based I'll have to develop
+    # another solution sometime later. Preferably not just an enormous list
+    # of valid permission names.
+    invalid = [perm for perm in perms.keys() if not getattr(guilded.Permissions, perm, None)]
+    if invalid:
+        raise TypeError(f"Invalid permission(s): {', '.join(invalid)}")
+
+    def predicate(ctx: Context) -> bool:
+        if not ctx.server:
+            raise NoPrivateMessage
+
+        permissions = ctx.author.server_permissions  # type: ignore
+        missing = [perm for perm, value in perms.items() if getattr(permissions, perm) != value]
+
+        if not missing:
+            return True
+
+        raise MissingPermissions(missing)
+
+    return check(predicate)
+
+has_guild_permissions = has_server_permissions  # discord.py
+
+
+def bot_has_server_permissions(**perms: bool) -> Check[Any]:
+    """Identical to :func:`.has_server_permissions` but for the bot
+    member's permissions.
+
+    .. versionadded:: 1.9
+    """
+
+    # I'm aware that this is open to false positives
+    # e.g. if the user passes `values=True`.
+    # But since Guilded permissions are not flag-based I'll have to develop
+    # another solution sometime later. Preferably not just an enormous list
+    # of valid permission names.
+    invalid = [perm for perm in perms.keys() if not getattr(guilded.Permissions, perm, None)]
+    if invalid:
+        raise TypeError(f"Invalid permission(s): {', '.join(invalid)}")
+
+    def predicate(ctx: Context) -> bool:
+        if not ctx.server:
+            raise NoPrivateMessage
+
+        permissions = ctx.me.server_permissions  # type: ignore
+        missing = [perm for perm, value in perms.items() if getattr(permissions, perm) != value]
+
+        if not missing:
+            return True
+
+        raise MissingPermissions(missing)
+
+    return check(predicate)
+
+bot_has_guild_permissions = bot_has_server_permissions  # discord.py
```

### Comparing `guilded.py-1.8.0/guilded/ext/commands/errors.py` & `guilded.py-1.9.0/guilded/ext/commands/errors.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.8.0/guilded/ext/commands/help.py` & `guilded.py-1.9.0/guilded/ext/commands/help.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.8.0/guilded/ext/commands/view.py` & `guilded.py-1.9.0/guilded/ext/commands/view.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.8.0/guilded/ext/tasks/__init__.py` & `guilded.py-1.9.0/guilded/ext/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.8.0/guilded/file.py` & `guilded.py-1.9.0/guilded/file.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.8.0/guilded/flowbot.py` & `guilded.py-1.9.0/guilded/flowbot.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.8.0/guilded/gateway.py` & `guilded.py-1.9.0/guilded/gateway.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,16 +63,18 @@
 import traceback
 from typing import TYPE_CHECKING, Dict, Optional
 
 from .errors import GuildedException, HTTPException
 from .enums import ChannelType
 from . import events as ev
 from .channel import *
+from .group import Group
 from .reaction import RawReactionActionEvent, Reaction
 from .role import Role
+from .status import Status
 from .user import ClientUser, Member
 from .utils import ISO8601
 from .webhook import Webhook
 
 if TYPE_CHECKING:
     from typing_extensions import Self
 
@@ -574,15 +576,15 @@
                 # with this data since it will undoubtably be the newest available
                 server._roles.clear()
 
                 for role_id, updated in data['rolesById'].items():
                     if role_id.isdigit():
                         # "baseRole" is included in rolesById, resulting in a
                         # duplicate entry for the base role.
-                        role = Role(state=self._state, data=updated, server=server)
+                        role = Role(state=self._state, data=updated)
                         server._roles[role.id] = role
 
     async def parse_server_member_social_link_created(self, data: gw.ServerMemberSocialLinkEvent):
         if self._exp_style:
             event = ev.MemberSocialLinkCreateEvent(self._state, data)
             self.client.dispatch(event)
 
@@ -796,15 +798,15 @@
             channel = self._state.create_channel(data=data['channel'], server=server)
             self._state.add_to_server_channel_cache(channel)
             self.client.dispatch('server_channel_create', channel)
 
     async def parse_server_channel_updated(self, data: gw.ServerChannelEvent):
         if self._exp_style:
             event = ev.ServerChannelUpdateEvent(self._state, data)
-            self._state.add_to_server_channel_cache(event.channel)
+            self._state.add_to_server_channel_cache(event.after)
             self.client.dispatch(event)
 
         else:
             server = self.client.get_server(data['serverId'])
             before = server.get_channel(data['channel']['id'])
             if not before:
                 return
@@ -821,15 +823,15 @@
 
         else:
             server = self.client.get_server(data['serverId'])
             channel = self._state.create_channel(data=data['channel'], server=server)
             channel.server._channels.pop(channel.id, None)
             self.client.dispatch('server_channel_delete', channel)
 
-    async def parse_channel_message_reaction_created(self, data: gw.ChannelMessageReactionEvent):
+    async def parse_channel_message_reaction_created(self, data: gw.ChannelMessageReactionCreatedEvent):
         if self._exp_style:
             channel = await self._force_resolve_channel(data['serverId'], data['reaction']['channelId'])
             event = ev.MessageReactionAddEvent(self._state, data, channel)
             self.client.dispatch(event)
 
         else:
             server = self.client.get_server(data['serverId'])
@@ -838,15 +840,15 @@
             self.client.dispatch('raw_message_reaction_add', payload)
 
             message = self._state._get_message(data['reaction']['messageId'])
             if message:
                 reaction = Reaction(data=data['reaction'], parent=message)
                 self.client.dispatch('message_reaction_add', reaction)
 
-    async def parse_channel_message_reaction_deleted(self, data: gw.ChannelMessageReactionEvent):
+    async def parse_channel_message_reaction_deleted(self, data: gw.ChannelMessageReactionDeletedEvent):
         if self._exp_style:
             channel = await self._force_resolve_channel(data['serverId'], data['reaction']['channelId'])
             event = ev.MessageReactionRemoveEvent(self._state, data, channel)
             self.client.dispatch(event)
 
         else:
             server = self.client.get_server(data['serverId'])
@@ -855,14 +857,20 @@
             self.client.dispatch('raw_message_reaction_remove', payload)
 
             message = self._state._get_message(data['reaction']['messageId'])
             if message:
                 reaction = Reaction(data=data['reaction'], parent=message)
                 self.client.dispatch('message_reaction_remove', reaction)
 
+    async def parse_channel_message_reaction_many_deleted(self, data: gw.ChannelMessageReactionManyDeletedEvent):
+        if self._exp_style:
+            channel = await self._force_resolve_channel(data['serverId'], data['channelId'])
+            event = ev.BulkMessageReactionRemoveEvent(self._state, data, channel)
+            self.client.dispatch(event)
+
     async def parse_calendar_event_created(self, data: gw.CalendarEventEvent):
         if self._exp_style:
             channel = await self._force_resolve_channel(data['serverId'], data['calendarEvent']['channelId'], ChannelType.calendar)
             event = ev.CalendarEventCreateEvent(self._state, data, channel)
             self.client.dispatch(event)
 
         else:
@@ -1107,14 +1115,53 @@
 
     async def parse_forum_topic_comment_reaction_deleted(self, data: gw.ForumTopicCommentReactionEvent):
         if self._exp_style:
             channel = await self._force_resolve_channel(data['serverId'], data['reaction']['channelId'], ChannelType.forums)
             event = ev.ForumTopicReplyReactionRemoveEvent(self._state, data, channel)
             self.client.dispatch(event)
 
+    async def parse_group_created(self, data: gw.GroupEvent):
+        if self._exp_style:
+            event = ev.GroupCreateEvent(self._state, data)
+            self.client.dispatch(event)
+
+        else:
+            server = self.client.get_server(data['serverId'])
+            if not server:
+                return
+
+            group = Group(state=self._state, data=data['group'], server=server)
+            self.client.dispatch('group_create', group)
+
+    async def parse_group_updated(self, data: gw.GroupEvent):
+        if self._exp_style:
+            event = ev.GroupUpdateEvent(self._state, data)
+            self.client.dispatch(event)
+
+        else:
+            server = self.client.get_server(data['serverId'])
+            if not server:
+                return
+
+            group = Group(state=self._state, data=data['group'], server=server)
+            self.client.dispatch('raw_group_update', group)
+
+    async def parse_group_deleted(self, data: gw.GroupEvent):
+        if self._exp_style:
+            event = ev.GroupDeleteEvent(self._state, data)
+            self.client.dispatch(event)
+
+        else:
+            server = self.client.get_server(data['serverId'])
+            if not server:
+                return
+
+            group = Group(state=self._state, data=data['group'], server=server)
+            self.client.dispatch('group_delete', group)
+
     async def parse_list_item_created(self, data: gw.ListItemEvent):
         if self._exp_style:
             channel = await self._force_resolve_channel(data['serverId'], data['listItem']['channelId'], ChannelType.list)
             event = ev.ListItemCreateEvent(self._state, data, channel)
             self.client.dispatch(event)
 
     async def parse_list_item_updated(self, data: gw.ListItemEvent):
@@ -1215,14 +1262,77 @@
                 event = await channel.fetch_event(data['calendarEventRsvp']['calendarEventId'])
             except HTTPException:
                 return
 
             rsvp = CalendarEventRSVP(data=data['calendarEventRsvp'], event=event)
             self.client.dispatch('calendar_event_rsvp_delete', rsvp)
 
+    async def parse_user_status_created(self, data: gw.UserStatusCreatedEvent):
+        if self._exp_style:
+            event = ev.UserStatusCreateEvent(self._state, data)
+            self.client.dispatch(event)
+
+        else:
+            user = self._state._get_user(data['userId'])
+            status = Status(state=self._state, data=data['userStatus'])
+            expires_at = ISO8601(data.get('expiresAt'))
+
+            if user:
+                self.client.dispatch('user_status_create', user, status, expires_at)
+
+    async def parse_user_status_deleted(self, data: gw.UserStatusDeletedEvent):
+        if self._exp_style:
+            event = ev.UserStatusDeleteEvent(self._state, data)
+            self.client.dispatch(event)
+
+        else:
+            user = self._state._get_user(data['userId'])
+            status = Status(state=self._state, data=data['userStatus'])
+
+            if user:
+                self.client.dispatch('user_status_delete', user, status)
+
+    async def parse_role_created(self, data: gw.RoleEvent):
+        if self._exp_style:
+            event = ev.RoleCreateEvent(self._state, data)
+            self._state.add_to_role_cache(event.role)
+            self.client.dispatch(event)
+
+        else:
+            role = Role(state=self._state, data=data['role'])
+            self._state.add_to_role_cache(role)
+            self.client.dispatch('role_create', role)
+
+    async def parse_role_updated(self, data: gw.RoleEvent):
+        if self._exp_style:
+            event = ev.RoleUpdateEvent(self._state, data)
+            self._state.add_to_role_cache(event.after)
+            self.client.dispatch(event)
+
+        else:
+            server = self.client.get_server(data['serverId'])
+            before = server.get_role(data['role']['id'])
+            if not before:
+                return
+
+            role = Role(state=self._state, data=data['role'])
+            self._state.add_to_role_cache(role)
+            self.client.dispatch('role_update', before, role)
+
+    async def parse_role_deleted(self, data: gw.RoleEvent):
+        if self._exp_style:
+            event = ev.RoleDeleteEvent(self._state, data)
+            self._state.remove_from_role_cache(event.server_id, event.role.id)
+            self.client.dispatch(event)
+
+        else:
+            role = Role(state=self._state, data=data['role'])
+            self._state.remove_from_role_cache(data['serverId'], role.id)
+            self.client.dispatch('role_delete', role)
+
 
 class Heartbeater(threading.Thread):
     def __init__(self, ws: GuildedWebSocket, *, interval: float):
         self.ws = ws
         self.interval = interval
         #self.heartbeat_timeout = timeout
         super().__init__()
```

### Comparing `guilded.py-1.8.0/guilded/group.py` & `guilded.py-1.9.0/guilded/group.py`

 * *Files 12% similar despite different names*

```diff
@@ -48,25 +48,27 @@
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
 from __future__ import annotations
 
 import datetime
-from typing import TYPE_CHECKING, Optional
+from typing import TYPE_CHECKING, Optional, Tuple
 
 from .asset import Asset
 from .mixins import Hashable
-from .status import Game
-from .utils import ISO8601
+from .utils import ISO8601, MISSING
 
 if TYPE_CHECKING:
+    from .emote import Emote
     from .server import Server
     from .user import Member
 
+    from .types.group import Group as GroupPayload
+
 
 __all__ = (
     'Group',
 )
 
 
 class Group(Hashable):
@@ -96,94 +98,93 @@
         The server that the group is in.
     id: :class:`str`
         The group's id.
     name: :class:`str`
         The group's name.
     description: Optional[:class:`str`]
         The group's description.
-    position: Optional[:class:`int`]
-        The group's position on the sidebar. Will be ``None`` if :attr:`.base`
-        is ``True``\.
+    home: :class:`bool`
+        Whether the group is the home group of its server.
     public: :class:`bool`
-        Whether the group is public.
+        Whether the group is able to be joined by anyone.
+    emote_id: Optional[:class:`int`]
+        The ID of the emote associated with the group, if any.
+    created_at: :class:`datetime.datetime`
+        When the group was created.
+    updated_at: Optional[:class:`datetime.datetime`]
+        When the group was last updated.
+    archived_at: Optional[:class:`datetime.datetime`]
+        When the group was archived, if applicable.
     """
 
-    def __init__(self, *, state, data, server: Server):
+    __slots__: Tuple[str, ...] = (
+        '_state',
+        'server',
+        'server_id',
+        'id',
+        'name',
+        'description',
+        'home',
+        'public',
+        'emote_id',
+        'author_id',
+        'updated_by_id',
+        'archived_by_id',
+        'created_at',
+        'updated_at',
+        'archived_at',
+        '_avatar',
+    )
+
+    def __init__(self, *, state, data: GroupPayload, server: Server):
         self._state = state
         self.server = server
-        data = data.get('group', data)
+        self.server_id: str = data.get('serverId')
 
-        self.id: str = data.get('id')
+        self.id: str = data['id']
         self.name: str = data.get('name')
-        self.type: str = data.get('type', 'team')
         self.description: str = data.get('description') or ''
-        self.position: Optional[int] = data.get('priority')
-        self.server_id: str = data.get('teamId')
 
-        self.game_id: Optional[int] = data.get('gameId')
-        self._base: bool = data.get('isBase')
-        self.public: bool = data.get('isPublic')
+        self.home: bool = data.get('isHome') or False
+        self.public: bool = data.get('isPublic') or False
 
+        self.emote_id: Optional[int] = data.get('emoteId')
         self.author_id: Optional[str] = data.get('createdBy')
         self.updated_by_id: Optional[str] = data.get('updatedBy')
         self.archived_by_id: Optional[str] =  data.get('archivedBy')
 
         self.created_at: datetime.datetime = ISO8601(data.get('createdAt'))
         self.updated_at: Optional[datetime.datetime] = ISO8601(data.get('updatedAt'))
-        self.deleted_at: Optional[datetime.datetime] = ISO8601(data.get('deletedAt'))
         self.archived_at: Optional[datetime.datetime] = ISO8601(data.get('archivedAt'))
 
         avatar = None
         if data.get('avatar'):
             avatar = Asset._from_group_avatar(state, data.get('avatar'))
         self._avatar: Optional[Asset] = avatar
 
-        banner = None
-        if data.get('banner'):
-            banner = Asset._from_group_banner(state, data.get('banner'))
-        self._banner: Optional[Asset] = banner
-
     def __str__(self):
         return self.name
 
     def __repr__(self):
         return f'<Group id={self.id!r} name={self.name!r} server_id={self.server_id!r}>'
 
     @property
-    def game(self) -> Game:
-        """Optional[:class:`Game`]: The game that the group is for."""
-        if self.game_id:
-            return Game(game_id=self.game_id)
-        return None
-
-    @property
     def archived(self) -> bool:
         """:class:`bool`: Whether this group is archived."""
-        return self.archived_at is not None or self.archived_by is not None
+        return self.archived_at is not None
 
     @property
-    def base(self) -> bool:
-        """:class:`bool`: Whether the group is the base or "home" group of its server."""
-        return self._base or self.server.base_group == self
+    def display_avatar(self) -> Optional[Asset]:
+        """Optional[:class:`.Asset`]: The group's displayed avatar.
+        If :attr:`.home` is ``True``, this will be the :attr:`.server`\'s avatar instead."""
 
-    @property
-    def avatar(self) -> Optional[Asset]:
-        """Optional[:class:`.Asset`]: The group's avatar, if any.
-        If :attr:`.base` is ``True``, this will be the :attr:`.server`\'s avatar instead."""
-        if self.base:
+        if self.home:
             return self._avatar or self.server.avatar
-        return self._avatar
 
-    @property
-    def banner(self) -> Optional[Asset]:
-        """Optional[:class:`.Asset`]: The group's banner, if any.
-        If :attr:`.base` is ``True``, this will be the :attr:`.server`\'s banner instead."""
-        if self.base:
-            return self._banner or self.server.banner
-        return self._banner
+        return self._avatar
 
     @property
     def author(self) -> Optional[Member]:
         """Optional[:class:`.Member`]: The member who created the group."""
         return self.server.get_member(self.author_id)
 
     @property
@@ -192,14 +193,94 @@
         return self.server.get_member(self.updated_by_id)
 
     @property
     def archived_by(self) -> Optional[Member]:
         """Optional[:class:`.Member`]: The member who archived the group, if any."""
         return self.server.get_member(self.archived_by_id)
 
+    async def edit(
+        self,
+        *,
+        name: Optional[str] = MISSING,
+        description: Optional[str] = MISSING,
+        emote: Optional[Emote] = MISSING,
+        public: bool = MISSING,
+    ) -> Group:
+        """|coro|
+
+        Edit the group.
+
+        All parameters are optional.
+
+        .. versionadded:: 1.9
+
+        Parameters
+        -----------
+        name: :class:`str`
+            The name of the group.
+        description: :class:`str`
+            The description of the group.
+        emote: :class:`.Emote`
+            The emote associated with the group.
+        public: :class:`bool`
+            Whether the group is public.
+
+        Raises
+        -------
+        HTTPException
+            Editing the group failed.
+        Forbidden
+            You do not have permissions to edit the group.
+
+        Returns
+        --------
+        :class:`Group`
+            The newly edited group.
+        """
+
+        payload = {}
+
+        if name is not MISSING:
+            payload['name'] = name
+
+        if description is not MISSING:
+            payload['description'] = description
+
+        if emote is not MISSING:
+            emote_id: int = getattr(emote, 'id', emote)
+            payload['emoteId'] = emote_id
+
+        if public is not MISSING:
+            payload['isPublic'] = public
+
+        data = await self._state.update_group(
+            self.server_id,
+            self.id,
+            payload=payload
+        )
+
+        group = Group(state=self._state, data=data['group'], server=self.server)
+        return group
+
+    async def delete(self) -> None:
+        """|coro|
+
+        Delete the group.
+
+        .. versionadded:: 1.9
+
+        Raises
+        -------
+        HTTPException
+            Deleting the group failed.
+        Forbidden
+            You do not have permissions to delete the group.
+        """
+        await self._state.delete_group(self.server_id, self.id)
+
     async def add_member(self, member: Member, /) -> None:
         """|coro|
 
         Add a member to this group.
 
         Raises
         -------
```

### Comparing `guilded.py-1.8.0/guilded/http.py` & `guilded.py-1.9.0/guilded/http.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 """
 
 from __future__ import annotations
 import sys
 
 import aiohttp
 import asyncio
+from collections.abc import Iterable
 import datetime
 import json
 import logging
 from typing import TYPE_CHECKING, Any, Dict, List, NamedTuple, Optional, Sequence, Type, TypeVar, Union
 
 from . import __version__, channel
 from .abc import ServerChannel
@@ -71,19 +72,22 @@
 log = logging.getLogger(__name__)
 
 
 if TYPE_CHECKING:
     from typing_extensions import Self
     from types import TracebackType
 
+    from .types.channel import ServerChannel as ServerChannelPayload
+
     from .asset import Asset
     from .channel import DMChannel, Thread
     from .emote import Emote
     from .file import Attachment, File
     from .gateway import GuildedWebSocket
+    from .role import Role
     from .server import Server
     from .user import ClientUser
 
     T = TypeVar('T')
     BE = TypeVar('BE', bound=BaseException)
 
 
@@ -271,14 +275,18 @@
         if self._get_server(server_id):
             return self._get_server(server_id).get_thread(thread_id)
 
     def _get_server_member(self, server_id: str, user_id: str) -> Optional[Member]:
         if self._get_server(server_id):
             return self._get_server(server_id).get_member(user_id)
 
+    def _get_server_role(self, server_id: str, role_id: int) -> Optional[Role]:
+        if self._get_server(server_id):
+            return self._get_server(server_id).get_role(role_id)
+
     @property
     def _emotes(self) -> Dict[int, Emote]:
         emotes = {}
         for server in self._servers.values():
             emotes = {**emotes, **server._emotes}
 
         return emotes
@@ -289,29 +297,38 @@
     def add_to_message_cache(self, message: ChatMessage) -> None:
         if self._max_messages is None:
             return
         self._messages[message.id] = message
         while len(self._messages) > self._max_messages:
             del self._messages[list(self._messages.keys())[0]]
 
-    def add_to_server_cache(self, server):
+    def add_to_server_cache(self, server: Server):
         self._servers[server.id] = server
 
     def remove_from_server_cache(self, server_id: str):
         self._servers.pop(server_id, None)
 
-    def add_to_member_cache(self, member):
+    def add_to_member_cache(self, member: Member):
         server = member.server or self._get_server(member.server_id)
         if server:
             server._members[member.id] = member
 
-    def remove_from_member_cache(self, server_id, member_id):
+    def remove_from_member_cache(self, server_id: str, member_id: str):
         if self._get_server(server_id):
             self._get_server(server_id)._members.pop(member_id, None)
 
+    def add_to_role_cache(self, role: Role):
+        server = role.server
+        if server:
+            server._roles[role.id] = role
+
+    def remove_from_role_cache(self, server_id: str, role_id: int):
+        if self._get_server(server_id):
+            self._get_server(server_id)._roles.pop(role_id, None)
+
     def add_to_server_channel_cache(self, channel):
         server = channel.server or self._get_server(channel.server_id)
         if server:
             server._channels[channel.id] = channel
 
     def remove_from_server_channel_cache(self, server_id, channel_id):
         if self._get_server(server_id):
@@ -390,14 +407,20 @@
 
     def get_my_user(self):
         return self.request(Route('GET', '/users/@me'))
 
     def get_my_servers(self):
         return self.request(Route('GET', '/users/@me/servers'))
 
+    def update_my_status(self, payload: Dict[str, Any]):
+        return self.request(Route('PUT', '/users/@me/status'), json=payload)
+
+    def delete_my_status(self):
+        return self.request(Route('DELETE', '/users/@me/status'))
+
     # /content
 
     def get_metadata(self, route: str):
         params = {
             'route': route,
         }
         return self.request(Route('GET', '/content/route/metadata', override_base=Route.USER_BASE), params=params)
@@ -454,15 +477,18 @@
             kwargs['data'] = json.dumps(kwargs.pop('json'))
 
         kwargs['headers'] = headers
 
         # route.url doesn't include params since we don't pass them to the Route
         log_url = url
         if kwargs.get('params'):
-            log_url = '?' + '&'.join([f'{key}={val}' for key, val in kwargs['params'].items()])
+            if isinstance(kwargs['params'], dict):
+                log_url += '?' + '&'.join([f'{key}={val}' for key, val in kwargs['params'].items()])
+            elif isinstance(kwargs['params'], Iterable):
+                log_url += '?' + '&'.join([f'{param[0]}={param[1]}' for param in kwargs['params']])
 
         log_headers = headers.copy()
         if 'Authorization' in log_headers:
             log_headers['Authorization'] = 'Bearer [removed]'
 
         response: Optional[aiohttp.ClientResponse] = None
         data: Optional[Union[Dict[str, Any], str]] = None
@@ -560,14 +586,16 @@
         content_type: str,
         *,
         name: str,
         topic: Optional[str] = None,
         public: Optional[bool] = None,
         category_id: Optional[int] = None,
         group_id: Optional[str] = None,
+        parent_id: Optional[str] = None,
+        message_id: Optional[str] = None,
     ):
         payload = {
             'serverId': server_id,
             'type': content_type,
             'name': name,
         }
 
@@ -579,14 +607,20 @@
 
         if category_id is not None:
             payload['categoryId'] = category_id
 
         if group_id is not None:
             payload['groupId'] = group_id
 
+        if parent_id is not None:
+            payload['parentId'] = parent_id
+
+        if message_id is not None:
+            payload['messageId'] = message_id
+
         return self.request(Route('POST', f'/channels'), json=payload)
 
     def update_channel(
         self,
         channel_id: str,
         *,
         payload: Dict[str, Any],
@@ -632,16 +666,27 @@
             params['limit'] = limit
 
         return self.request(Route('GET', f'/channels/{channel_id}/messages'), params=params)
 
     def add_channel_message_reaction(self, channel_id: str, message_id: str, emote_id: int):
         return self.request(Route('PUT', f'/channels/{channel_id}/messages/{message_id}/emotes/{emote_id}'))
 
-    def remove_channel_message_reaction(self, channel_id: str, message_id: str, emote_id: int):
-        return self.request(Route('DELETE', f'/channels/{channel_id}/messages/{message_id}/emotes/{emote_id}'))
+    def remove_channel_message_reaction(self, channel_id: str, message_id: str, emote_id: int, user_id: Optional[str] = None):
+        params = {}
+        if user_id:
+            params['userId'] = user_id
+
+        return self.request(Route('DELETE', f'/channels/{channel_id}/messages/{message_id}/emotes/{emote_id}'), params=params)
+
+    def remove_channel_message_reactions(self, channel_id: str, message_id: str, emote_id: int = None):
+        params = {}
+        if emote_id is not None:
+            params['emoteId'] = emote_id
+
+        return self.request(Route('DELETE', f'/channels/{channel_id}/messages/{message_id}/emotes'), params=params)
 
     def create_forum_topic(self, channel_id: str, *, title: str, content: str):
         payload = {
             'title': title,
             'content': content,
         }
 
@@ -998,14 +1043,29 @@
 
     def award_role_xp(self, server_id: str, role_id: int, amount: int):
         payload = {
             'amount': amount,
         }
         return self.request(Route('POST', f'/servers/{server_id}/roles/{role_id}/xp'), json=payload)
 
+    def create_role(self, server_id: str, *, payload: Dict[str, Any]):
+        return self.request(Route('POST', f'/servers/{server_id}/roles'), json=payload)
+
+    def get_role(self, server_id: str, role_id: int):
+        return self.request(Route('GET', f'/servers/{server_id}/roles/{role_id}'))
+
+    def get_roles(self, server_id: str):
+        return self.request(Route('GET', f'/servers/{server_id}/roles'))
+
+    def update_role(self, server_id: str, role_id: int, *, payload: Dict[str, Any]):
+        return self.request(Route('PATCH', f'/servers/{server_id}/roles/{role_id}'), json=payload)
+
+    def delete_role(self, server_id: str, role_id: int):
+        return self.request(Route('DELETE', f'/servers/{server_id}/roles/{role_id}'))
+
     def ban_server_member(self, server_id: str, user_id: str, *, reason: str = None):
         payload = {}
         if reason is not None:
             payload['reason'] = reason
 
         return self.request(Route('POST', f'/servers/{server_id}/bans/{user_id}'), json=payload)
 
@@ -1034,54 +1094,77 @@
 
     def update_webhook(self, server_id: str, webhook_id: str, *, payload: Dict[str, Any]):
         return self.request(Route('PUT', f'/servers/{server_id}/webhooks/{webhook_id}'), json=payload)
 
     def delete_webhook(self, server_id: str, webhook_id: str):
         return self.request(Route('DELETE', f'/servers/{server_id}/webhooks/{webhook_id}'))
 
-    # /groups
+    # groups
+
+    def create_group(self, server_id: str, *, payload: Dict[str, Any]):
+        return self.request(Route('POST', f'/servers/{server_id}/groups'), json=payload)
+
+    def get_group(self, server_id: str, group_id: str):
+        return self.request(Route('GET', f'/servers/{server_id}/groups/{group_id}'))
+
+    def get_groups(self, server_id: str):
+        return self.request(Route('GET', f'/servers/{server_id}/groups'))
+
+    def update_group(self, server_id: str, group_id: str, *, payload: Dict[str, Any]):
+        return self.request(Route('PATCH', f'/servers/{server_id}/groups/{group_id}'), json=payload)
+
+    def delete_group(self, server_id: str, group_id: str):
+        return self.request(Route('DELETE', f'/servers/{server_id}/groups/{group_id}'))
 
     def add_group_member(self, group_id: str, user_id: str):
         return self.request(Route('PUT', f'/groups/{group_id}/members/{user_id}'))
 
     def remove_group_member(self, group_id: str, user_id: str):
         return self.request(Route('DELETE', f'/groups/{group_id}/members/{user_id}'))
 
+    # subscriptions
+
+    def get_subscription_tier(self, server_id: str, tier_type: str):
+        return self.request(Route('GET', f'/servers/{server_id}/subscriptions/tiers/{tier_type}'))
+
+    def get_subscription_tiers(self, server_id: str):
+        return self.request(Route('GET', f'/servers/{server_id}/subscriptions/tiers'))
+
     # create objects from data
 
     def create_user(self, **data) -> User:
         return User(state=self, **data)
 
     def create_member(self, **data) -> Member:
         return Member(state=self, **data)
 
-    def create_channel(self, **data) -> ServerChannel:
-        channel_data = data.get('data', data)
-        if channel_data.get('serverId') is None:
-            return channel.DMChannel(state=self, **data)
+    def create_channel(self, *, data: ServerChannelPayload, **extra) -> ServerChannel:
+        if data.get('serverId') is None:
+            return channel.DMChannel(state=self, **extra)
 
         data['group'] = data.get('group')
-        if 'parentId' in channel_data:
+        if 'parentId' in data:
             # Only threads have parent channels or parent threads.
             # Their type is still 'chat' so this is the only way we can differentiate them.
             cls = channel.Thread
         else:
             types = {
                 ChannelType.announcements: channel.AnnouncementChannel,
                 ChannelType.calendar: channel.CalendarChannel,
                 ChannelType.chat: channel.ChatChannel,
                 ChannelType.docs: channel.DocsChannel,
                 ChannelType.forums: channel.ForumChannel,
                 ChannelType.list: channel.ListChannel,
                 ChannelType.media: channel.MediaChannel,
                 ChannelType.scheduling: channel.SchedulingChannel,
+                ChannelType.stream: channel.StreamChannel,
                 ChannelType.voice: channel.VoiceChannel,
             }
-            cls = types.get(try_enum(ChannelType, channel_data['type']))
+            cls = types.get(try_enum(ChannelType, data['type']))
             if cls is None:
                 cls = ServerChannel
 
-        return cls(state=self, **data)
+        return cls(state=self, data=data, **extra)
 
     def create_message(self, **data) -> ChatMessage:
         data['channel'] = data.get('channel')
         return ChatMessage(state=self, **data)
```

### Comparing `guilded.py-1.8.0/guilded/invite.py` & `guilded.py-1.9.0/guilded/invite.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.8.0/guilded/message.py` & `guilded.py-1.9.0/guilded/message.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,15 +64,16 @@
 from .file import Attachment
 from .mixins import Hashable
 from .utils import ISO8601, MISSING, valid_video_extensions
 
 if TYPE_CHECKING:
     from .types.channel import Mentions as MentionsPayload
 
-    from .abc import Messageable, ServerChannel
+    from .abc import Messageable, ServerChannel, User as abc_User
+    from .channel import Thread
     from .emote import Emote
     from .group import Group
     from .role import Role
     from .server import Server
     from .user import Member, User
 
 log = logging.getLogger(__name__)
@@ -162,18 +163,14 @@
         ignore_cache: bool = False,
         ignore_errors: bool = False,
     ) -> None:
         """|coro|
 
         Fetch & fill the internal cache with the targets referenced.
 
-        .. note::
-
-            Due to Guilded limitations, this will not fill role information.
-
         Parameters
         -----------
         ignore_cache: :class:`bool`
             Whether to fetch objects even if they are already cached.
             Defaults to ``False`` if not specified.
         ignore_errors: :class:`bool`
             Whether to ignore :exc:`HTTPException`\s that occur while fetching.
@@ -221,14 +218,42 @@
                             user = await self._state.get_user(user_data['id'])
                         except HTTPException:
                             if not ignore_errors:
                                 raise
                         else:
                             self._state.add_to_user_cache(user)
 
+        # Just fetch the whole role list instead of fetching >=5 roles individually.
+        uncached_role_count = len(self._roles) - len(self.roles)
+        if (
+            self._server and (
+                uncached_role_count >= 5
+                or (len(self._roles) >= 5 and ignore_cache)
+            )
+        ):
+            # `fill_roles` here would cause potentially unwanted/unexpected
+            # cache usage, especially in large servers.
+            roles = await self._server.fetch_roles()
+            role_ids = [role['id'] for role in self._roles]
+            for role in roles:
+                if role.id in role_ids:
+                    self._state.add_to_role_cache(role)
+
+        else:
+            for role_data in self._roles:
+                cached_role = self._state._get_server_role(self._server.id, role_data['id'])
+                if self._server and (ignore_cache or not cached_role):
+                    try:
+                        role = await self._server.fetch_role(role_data['id'])
+                    except HTTPException:
+                        if not ignore_errors:
+                            raise
+                    else:
+                        self._state.add_to_role_cache(role)
+
         for channel_data in self._channels:
             if not self._server:
                 # This should never happen
                 break
 
             cached_channel = self._state._get_server_channel_or_thread(self._server.id, channel_data['id'])
             if ignore_cache or not cached_channel:
@@ -830,26 +855,74 @@
         -----------
         emote: :class:`.Emote`
             The emote to add.
         """
         emote_id: int = getattr(emote, 'id', emote)
         await self._state.add_channel_message_reaction(self.channel_id, self.id, emote_id)
 
+    async def remove_reaction(self, emote: Emote, member: Optional[abc_User] = None) -> None:
+        """|coro|
+
+        Remove a reaction from this message.
+
+        If the reaction is not your own then :attr:`~Permissions.manage_messages` is required.
+
+        .. versionadded:: 1.9
+
+        Parameters
+        -----------
+        emote: :class:`.Emote`
+            The emote to remove.
+        member: Optional[:class:`~.abc.User`]
+            The member whose reaction to remove.
+            If this is not specified, the client's reaction will be removed instead.
+        """
+        emote_id: int = getattr(emote, 'id', emote)
+        await self._state.remove_channel_message_reaction(self.channel.id, self.id, emote_id, member.id if member else None)
+
     async def remove_self_reaction(self, emote: Emote, /) -> None:
         """|coro|
 
         Remove one of your reactions from this message.
 
+        .. deprecated:: 1.9
+            Use :meth:`.remove_reaction` instead.
+
+        Parameters
+        -----------
+        emote: :class:`.Emote`
+            The emote to remove.
+        """
+        await self.remove_reaction(emote)
+
+    async def clear_reaction(self, emote: Emote, /) -> None:
+        """|coro|
+
+        Bulk remove reactions from this message based on their emote.
+
+        To remove individual reactions from specific users, see :meth:`.remove_reaction`.
+
+        .. versionadded:: 1.9
+
         Parameters
         -----------
         emote: :class:`.Emote`
             The emote to remove.
         """
         emote_id: int = getattr(emote, 'id', emote)
-        await self._state.remove_channel_message_reaction(self.channel.id, self.id, emote_id)
+        await self._state.remove_channel_message_reactions(self.channel.id, self.id, emote_id)
+
+    async def clear_reactions(self) -> None:
+        """|coro|
+
+        Bulk remove all the reactions from this message.
+
+        .. versionadded:: 1.9
+        """
+        await self._state.remove_channel_message_reactions(self.channel.id, self.id)
 
     async def reply(
         self,
         content: Optional[str] = MISSING,
         *,
         embed: Optional[Embed] = MISSING,
         embeds: Optional[Sequence[Embed]] = MISSING,
@@ -881,21 +954,60 @@
             reply_to=reply_to,
             mention_author=mention_author,
             silent=silent,
             private=private,
             delete_after=delete_after,
         )
 
-    #async def create_thread(self, *content, **kwargs):
-    #    """|coro|
+    async def create_thread(self, name: str) -> Thread:
+        """|coro|
 
-    #    Create a thread on this message.
-    #    """
-    #    kwargs['message'] = self
-    #    return await self.channel.create_thread(*content, **kwargs)
+        Create a new thread under the message.
+
+        .. warning::
+
+            Be careful with this method!
+            It is very easy to accidentally cause a loop if you create a
+            thread on a message that caused the creation of its thread.
+
+        Depending on the type of the parent channel, this method requires
+        different permissions:
+
+        +------------------------------+-----------------------------------+
+        |         Parent Type          |             Permission            |
+        +------------------------------+-----------------------------------+
+        | :attr:`~.ChannelType.chat`   | :attr:`Permissions.read_messages` |
+        +------------------------------+-----------------------------------+
+        | :attr:`~.ChannelType.voice`  | :attr:`Permissions.hear_voice`    |
+        +------------------------------+-----------------------------------+
+        | :attr:`~.ChannelType.stream` | :attr:`Permissions.view_streams`  |
+        +------------------------------+-----------------------------------+
+
+        .. versionadded:: 1.9
+
+        Parameters
+        -----------
+        name: :class:`str`
+            The thread's name. Can include spaces.
+
+        Returns
+        --------
+        :class:`.Thread`
+            The created thread.
+
+        Raises
+        -------
+        NotFound
+            The server, channel, or message does not exist.
+        Forbidden
+            You are not allowed to create a thread in this channel.
+        HTTPException
+            Failed to create a thread.
+        """
+        return await self.channel.create_thread(name=name, message=self)
 
     #async def pin(self):
     #    """|coro|
 
     #    Pin this message.
     #    """
     #    await self._state.pin_message(self.channel.id, self.id)
```

### Comparing `guilded.py-1.8.0/guilded/mixins.py` & `guilded.py-1.9.0/guilded/types/webhook.py`

 * *Files 17% similar despite different names*

```diff
@@ -45,32 +45,35 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
-from typing import Union
+from __future__ import annotations
 
+from typing import Optional, TypedDict
+from typing_extensions import NotRequired
 
-__all__ = (
-    'EqualityComparable',
-    'Hashable',
-)
 
+class PartialWebhook(TypedDict):
+    id: str
+    name: str
+    token: NotRequired[Optional[str]]
+    channelId: NotRequired[str]
+    deletedAt: NotRequired[str]
+    createdAt: NotRequired[str]
 
-class EqualityComparable:
-    __slots__ = ()
 
-    id: Union[str, int]
+class _UserWebhook(TypedDict, total=False):
+    teamId: str
+    iconUrl: Optional[str]
+    createdBy: NotRequired[str]
 
-    def __eq__(self, other: object) -> bool:
-        if isinstance(other, self.__class__):
-            return other.id == self.id
-        return NotImplemented
 
+class _Webhook(TypedDict, total=False):
+    avatar: NotRequired[str]
+    serverId: str
 
-class Hashable(EqualityComparable):
-    __slots__ = ()
 
-    def __hash__(self) -> int:
-        return hash(self.id)
+class Webhook(PartialWebhook, _UserWebhook, _Webhook):
+    ...
```

### Comparing `guilded.py-1.8.0/guilded/presence.py` & `guilded.py-1.9.0/guilded/presence.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.8.0/guilded/reaction.py` & `guilded.py-1.9.0/guilded/reaction.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.8.0/guilded/reply.py` & `guilded.py-1.9.0/guilded/reply.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.8.0/guilded/server.py` & `guilded.py-1.9.0/guilded/server.py`

 * *Files 13% similar despite different names*

```diff
@@ -52,30 +52,32 @@
 from __future__ import annotations
 
 import datetime
 import re
 from typing import TYPE_CHECKING, Dict, Optional, List, Union
 
 from .abc import ServerChannel, User
-
 from .asset import Asset
 from .channel import AnnouncementChannel, ChatChannel, DocsChannel, ForumChannel, ListChannel, MediaChannel, SchedulingChannel, Thread, VoiceChannel
+from .colour import Colour
 from .errors import InvalidData
-from .enums import ServerType, try_enum, ChannelType
+from .enums import ServerSubscriptionTierType, ServerType, try_enum, ChannelType
 from .group import Group
 from .mixins import Hashable
 from .role import Role
+from .subscription import ServerSubscriptionTier
 from .user import Member, MemberBan
-from .utils import ISO8601, get, find
+from .utils import ISO8601, MISSING, get
 
 if TYPE_CHECKING:
     from .types.server import Server as ServerPayload
 
     from .emote import Emote
     from .flowbot import FlowBot
+    from .permissions import Permissions
     from .webhook import Webhook
 
 # ZoneInfo is in the stdlib in Python 3.9+
 try:
     from zoneinfo import ZoneInfo  # type: ignore
 except ImportError:
     # Fall back to pytz, if installed
@@ -155,15 +157,14 @@
         self._groups: Dict[str, Group] = {}
         self._emotes: Dict[int, Emote] = {}
         self._members: Dict[str, Member] = {}
         self._roles: Dict[int, Role] = {}
         self._flowbots: Dict[str, FlowBot] = {}
 
         self._base_role: Optional[Role] = None
-        self._bot_role: Optional[Role] = None
 
         self.owner_id: str = data.get('ownerId')
         self.name: str = data.get('name')
         self.slug: str = data.get('url')
         self.created_at: datetime.datetime = ISO8601(data.get('createdAt'))
         self.about: str = data.get('about') or ''
         self.default_channel_id: Optional[str] = data.get('defaultChannelId')
@@ -174,20 +175,18 @@
             member['serverId'] = self.id
             self._members[member['id']] = self._state.create_member(data=member, server=self)
 
         for role_id, role in data.get('rolesById', {}).items():
             if role_id.isdigit():
                 # "baseRole" is included in rolesById, resulting in a
                 # duplicate entry for the base role.
-                role: Role = Role(state=self._state, data=role, server=self)
+                role: Role = Role(state=self._state, data=role)
                 self._roles[role.id] = role
                 if role.base:
                     self._base_role: Optional[Role] = role
-                if role.is_bot():
-                    self._bot_role: Optional[Role] = role
 
         avatar = None
         avatar_url = data.get('profilePicture') or data.get('avatar')
         if avatar_url:
             avatar = Asset._from_team_avatar(state, avatar_url)
         self.avatar: Optional[Asset] = avatar
 
@@ -389,19 +388,14 @@
 
     @property
     def base_role(self) -> Optional[Role]:
         """Optional[:class:`.Role`]: The base ``Member`` role for the server."""
         return self._base_role or get(self.roles, base=True)
 
     @property
-    def bot_role(self) -> Optional[Role]:
-        """Optional[:class:`.Role`]: The ``Bot`` role for the server."""
-        return self._bot_role or find(lambda role: role.is_bot(), self.roles)
-
-    @property
     def icon(self) -> Optional[Asset]:
         """Optional[:class:`.Asset`]: |dpyattr|
 
         This is an alias of :attr:`.avatar`.
 
         The server's set avatar, if any.
         """
@@ -1023,14 +1017,177 @@
             try:
                 member = self._state.create_member(server=self, data=member_data)
             except:
                 continue
             else:
                 self._members[member.id] = member
 
+    async def create_role(
+        self,
+        *,
+        name: str = MISSING,
+        permissions: Permissions = MISSING,
+        colours: List[Union[Colour, int]] = MISSING,
+        colors: List[Union[Colour, int]] = MISSING,
+        colour: Union[Colour, int] = MISSING,
+        color: Union[Colour, int] = MISSING,
+        displayed_separately: bool = MISSING,
+        hoist: bool = MISSING,
+        self_assignable: bool = MISSING,
+        mentionable: bool = MISSING,
+    ) -> Group:
+        """|coro|
+
+        Create a role in the server.
+
+        All parameters are optional.
+
+        .. versionadded:: 1.9
+
+        Parameters
+        -----------
+        name: :class:`str`
+            The name of the role. Defaults to 'New role'.
+        permissions: :class:`Permissions`
+            The permissions for the role.
+        colours: List[Union[:class:`Colour`, :class:`int`]]
+            The colour(s) of the role. If there are two values, the
+            second indicates the end of the gradient.
+            This is also aliased to ``colors``.
+            This cannot be used with ``colour``.
+        colour: Union[:class:`Colour`, :class:`int`]
+            The primary colour of the role.
+            This is also aliased to ``color``.
+            This cannot be used with ``colours``.
+        displayed_separately: :class:`bool`
+            Whether the role should be separated in the member list.
+            Defaults to ``False``.
+            This is also aliased to ``hoist``.
+        self_assignable: :class:`bool`
+            Whether members should be allowed to assign the role to themselves.
+            Defaults to ``False``.
+        mentionable: :class:`bool`
+            Whether all members should be able to mention the role.
+            Defaults to ``False``.
+
+        Raises
+        -------
+        Forbidden
+            You do not have permissions to create a role.
+        HTTPException
+            Creating the role failed.
+        TypeError
+            Cannot provide both ``colours`` and ``colour``
+            or ``displayed_separately`` and ``hoist``.
+
+        Returns
+        --------
+        :class:`Role`
+            The created role.
+        """
+
+        if (
+            (colours is not MISSING or colors is not MISSING) and
+            (colour is not MISSING or color is not MISSING)
+        ):
+            raise TypeError('Cannot mix colour/color and colours/colors keyword arguments.')
+        if displayed_separately is not MISSING and hoist is not MISSING:
+            raise TypeError('Cannot mix displayed_separately and hoist keyword arguments.')
+
+        payload = {
+            # This is for discord.py compatibility.
+            # `name` is not actually optional but 'New role' is the
+            # default name that the client uses.
+            'name': name if name is not MISSING else 'New role',
+            'permissions': permissions.values if permissions is not MISSING else [],
+        }
+
+        if colours is not MISSING:
+            payload['colors'] = [c.value if isinstance(c, Colour) else c for c in colours]
+        elif colors is not MISSING:
+            payload['colors'] = [c.value if isinstance(c, Colour) else c for c in colors]
+        elif colour is not MISSING:
+            payload['colors'] = [colour.value if isinstance(colour, Colour) else colour]
+        elif color is not MISSING:
+            payload['colors'] = [color.value if isinstance(color, Colour) else color]
+
+        if displayed_separately is not MISSING:
+            payload['isDisplayedSeparately'] = displayed_separately
+        elif hoist is not MISSING:
+            payload['isDisplayedSeparately'] = hoist
+
+        if self_assignable is not MISSING:
+            payload['isSelfAssignable'] = self_assignable
+
+        if mentionable is not MISSING:
+            payload['isMentionable'] = mentionable
+
+        data = await self._state.create_role(
+            self.id,
+            payload=payload
+        )
+
+        role = Role(state=self._state, data=data['role'])
+        return role
+
+    async def fetch_roles(self) -> List[Role]:
+        """|coro|
+
+        Fetch the list of :class:`Role`\s in the server.
+
+        .. versionadded:: 1.9
+
+        Returns
+        --------
+        List[:class:`.Role`]
+            The roles in the server.
+        """
+        data = await self._state.get_roles(self.id)
+        return [Role(state=self._state, data=role_data) for role_data in data['roles']]
+
+    async def fetch_role(self, role_id: int, /) -> Role:
+        """|coro|
+
+        Fetch a specific :class:`Role` in this server.
+
+        .. versionadded:: 1.9
+
+        Parameters
+        -----------
+        id: :class:`int`
+            The role's ID to fetch.
+
+        Returns
+        --------
+        :class:`Role`
+            The role from the ID.
+
+        Raises
+        -------
+        :class:`NotFound`
+            A role with that ID does not exist in this server.
+        """
+
+        data = await self._state.get_role(self.id, role_id)
+        return Role(state=self._state, data=data['role'])
+
+    async def getch_role(self, role_id: int, /) -> Role:
+        return self.get_role(role_id) or await self.fetch_role(role_id)
+
+    async def fill_roles(self) -> None:
+        """Fill the role cache for this server.
+
+        .. versionadded:: 1.9
+        """
+
+        data = await self._state.get_roles(self.id)
+        self._roles.clear()
+        for role_data in data['roles']:
+            self._roles[role_data['id']] = Role(state=self._state, data=role_data)
+
     async def ban(
         self,
         user: User,
         *,
         reason: str = None,
     ) -> MemberBan:
         """|coro|
@@ -1222,8 +1379,162 @@
         """
 
         if not self.default_channel_id:
             raise ValueError('This server has no default channel.')
 
         return await self.fetch_channel(self.default_channel_id)
 
+    async def create_group(
+        self,
+        name: str,
+        *,
+        description: Optional[str] = MISSING,
+        emote: Optional[Emote] = MISSING,
+        public: bool = MISSING,
+    ) -> Group:
+        """|coro|
+
+        Create a group in the server.
+
+        Parameters
+        -----------
+        name: :class:`str`
+            The name of the group.
+        description: Optional[:class:`str`]
+            The description of the group.
+        emote: Optional[:class:`.Emote`]
+            The emote associated with the group.
+        public: Optional[:class:`bool`]
+            Whether the group is public.
+
+        Raises
+        -------
+        HTTPException
+            Creating the group failed.
+        Forbidden
+            You do not have permissions to create a group.
+
+        Returns
+        --------
+        :class:`Group`
+            The created group.
+        """
+
+        payload = {
+            'name': name,
+        }
+
+        if description is not MISSING:
+            payload['description'] = description
+
+        if emote is not MISSING:
+            emote_id: int = getattr(emote, 'id', emote)
+            payload['emoteId'] = emote_id
+
+        if public is not MISSING:
+            payload['isPublic'] = public
+
+        data = await self._state.create_group(
+            self.id,
+            payload=payload
+        )
+
+        group = Group(state=self._state, data=data['group'], server=self)
+        return group
+
+    async def fetch_group(self, group_id: str, /) -> Group:
+        """|coro|
+
+        Fetch a group in the server.
+
+        Raises
+        -------
+        HTTPException
+            Fetching the group failed.
+        Forbidden
+            You do not have permissions to fetch the group.
+
+        Returns
+        --------
+        :class:`Group`
+            The group by the ID.
+        """
+
+        data = await self._state.get_group(self.id, group_id)
+        group = Group(state=self._state, data=data['group'], server=self)
+        return group
+
+    async def getch_group(self, group_id: str, /) -> Group:
+        return self.get_group(group_id) or await self.fetch_group(group_id)
+
+    async def fetch_groups(self) -> List[Group]:
+        """|coro|
+
+        Fetch all groups in the server.
+
+        Raises
+        -------
+        HTTPException
+            Fetching the groups failed.
+        Forbidden
+            You do not have permissions to fetch the groups.
+
+        Returns
+        --------
+        List[:class:`Group`]
+            The groups in the server.
+        """
+
+        data = await self._state.get_groups(self.id)
+        groups = [Group(state=self._state, data=group_data, server=self) for group_data in data['groups']]
+        return groups
+
+    async def fetch_subscription_tier(self, tier_type: ServerSubscriptionTierType, /) -> ServerSubscriptionTier:
+        """|coro|
+
+        Fetch a subscription tier in the server.
+
+        .. versionadded:: 1.9
+
+        Parameters
+        -----------
+        tier_type: :class:`.ServerSubscriptionTierType`
+            The type of the tier to fetch.
+
+        Raises
+        -------
+        NotFound
+            The server has no tier with the provided type.
+        HTTPException
+            Fetching the tier failed.
+
+        Returns
+        --------
+        :class:`.ServerSubscriptionTier`
+            The subscription tier by the type.
+        """
+
+        data = await self._state.get_subscription_tier(self.id, tier_type.value)
+        return ServerSubscriptionTier(state=self._state, data=data['serverSubscriptionTier'])
+
+    async def fetch_subscription_tiers(self) -> List[ServerSubscriptionTier]:
+        """|coro|
+
+        Fetch all subscription tiers in the server.
+
+        .. versionadded:: 1.9
+
+        Raises
+        -------
+        HTTPException
+            Fetching the tiers failed.
+
+        Returns
+        --------
+        List[:class:`.ServerSubscriptionTier`]
+            The subscription tiers in the server.
+        """
+
+        data = await self._state.get_subscription_tiers(self.id)
+        return [ServerSubscriptionTier(state=self._state, data=tier_data) for tier_data in data['serverSubscriptionTiers']]
+
 Guild = Server  # discord.py
```

### Comparing `guilded.py-1.8.0/guilded/types/announcement.py` & `guilded.py-1.9.0/guilded/types/announcement.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.8.0/guilded/types/calendar_event.py` & `guilded.py-1.9.0/guilded/types/calendar_event.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.8.0/guilded/types/channel.py` & `guilded.py-1.9.0/guilded/types/channel.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,21 +35,28 @@
     type: Literal['announcements', 'chat', 'calendar', 'forums', 'media', 'docs', 'voice', 'list', 'scheduling', 'stream']
     name: str
     topic: Optional[str]
     createdAt: str
     createdBy: str
     updatedAt: NotRequired[str]
     serverId: str
+    rootId: NotRequired[str]
     parentId: NotRequired[str]
+    messageId: NotRequired[str]
     categoryId: NotRequired[int]
     groupId: str
     isPublic: NotRequired[bool]
     archivedBy: NotRequired[str]
     archivedAt: NotRequired[str]
 
 
+class Thread(ServerChannel):
+    rootId: str
+    parentId: str
+
+
 class Mentions(TypedDict):
     users: Optional[List[User]]
     channels: Optional[List[ServerChannel]]
     roles: Optional[List[Role]]
     everyone: bool
     here: bool
```

### Comparing `guilded.py-1.8.0/guilded/types/doc.py` & `guilded.py-1.9.0/guilded/types/doc.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.8.0/guilded/types/embed.py` & `guilded.py-1.9.0/guilded/types/embed.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.8.0/guilded/types/emote.py` & `guilded.py-1.9.0/guilded/types/emote.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.8.0/guilded/types/forum_topic.py` & `guilded.py-1.9.0/guilded/types/forum_topic.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.8.0/guilded/types/gateway.py` & `guilded.py-1.9.0/guilded/types/gateway.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,21 +26,24 @@
 from typing import Any, Dict, List, Literal, Optional, TypedDict
 from typing_extensions import NotRequired
 
 from .announcement import Announcement, AnnouncementComment
 from .calendar_event import CalendarEvent, CalendarEventComment, CalendarEventRsvp
 from .channel import ServerChannel
 from .doc import Doc, DocComment
+from .emote import Emote
 from .forum_topic import ForumTopic, ForumTopicComment
+from .group import Group
 from .list_item import ListItem
 from .message import ChatMessage, DeletedChatMessage
 from .reaction import AnnouncementCommentReaction, AnnouncementReaction, CalendarEventCommentReaction, ChannelMessageReaction, CalendarEventReaction, DocCommentReaction, DocReaction, ForumTopicCommentReaction, ForumTopicReaction
+from .role import Role
 from .server import Server
 from .social_link import SocialLink
-from .user import ServerMember, ServerMemberBan, User
+from .user import ServerMember, ServerMemberBan, User, UserStatus
 from .webhook import Webhook
 
 
 class EventSkeleton(TypedDict):
     op: Literal[0, 1, 2, 8, 9]
     d: NotRequired[Dict[str, Any]]
     s: NotRequired[str]
@@ -196,21 +199,53 @@
     forumTopicComment: ForumTopicComment
 
 
 class ForumTopicCommentReactionEvent(_ServerEvent):
     reaction: ForumTopicCommentReaction
 
 
+class GroupEvent(_ServerEvent):
+    group: Group
+
+
 class CalendarEventRsvpEvent(_ServerEvent):
     calendarEventRsvp: CalendarEventRsvp
 
 
 class CalendarEventRsvpManyUpdatedEvent(_ServerEvent):
     calendarEventRsvps: List[CalendarEventRsvp]
 
 
 class ListItemEvent(_ServerEvent):
     listItem: ListItem
 
 
-class ChannelMessageReactionEvent(_ServerEvent):
+class ChannelMessageReactionCreatedEvent(_ServerEvent):
     reaction: ChannelMessageReaction
+
+
+class ChannelMessageReactionDeletedEvent(_ServerEvent):
+    deletedBy: str
+    reaction: ChannelMessageReaction
+
+
+class ChannelMessageReactionManyDeletedEvent(_ServerEvent):
+    channelId: str
+    messageId: str
+    deletedBy: str
+    count: int
+    emote: NotRequired[Emote]
+
+
+class UserStatusCreatedEvent(TypedDict):
+    userId: str
+    expiresAt: NotRequired[str]
+    userStatus: UserStatus
+
+
+class UserStatusDeletedEvent(TypedDict):
+    userId: str
+    userStatus: UserStatus
+
+
+class RoleEvent(TypedDict):
+    role: Role
```

### Comparing `guilded.py-1.8.0/guilded/types/list_item.py` & `guilded.py-1.9.0/guilded/types/list_item.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.8.0/guilded/types/message.py` & `guilded.py-1.9.0/guilded/types/message.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.8.0/guilded/types/reaction.py` & `guilded.py-1.9.0/guilded/types/reaction.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.8.0/guilded/types/role.py` & `guilded.py-1.9.0/guilded/types/group.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,27 +19,26 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 from __future__ import annotations
-from typing import Any, Dict, List, Literal, Optional, TypedDict, Union
+from typing import TypedDict
 from typing_extensions import NotRequired
 
 
-class Role(TypedDict):
-    id: int
+class Group(TypedDict):
+    id: str
+    serverId: str
     name: str
-    color: Optional[str]
-    permissions: NotRequired[Dict[str, int]]
-    priority: NotRequired[int]
-    teamId: str
+    description: NotRequired[str]
+    avatar: NotRequired[str]
+    isHome: NotRequired[bool]
+    emoteId: NotRequired[int]
+    isPublic: NotRequired[bool]
     createdAt: str
+    createdBy: str
     updatedAt: NotRequired[str]
-    isBase: NotRequired[bool]
-    discordRoleId: NotRequired[Optional[str]]
-    discordSyncedAt: NotRequired[Optional[str]]
-    isMentionable: NotRequired[bool]
-    isSelfAssignable: NotRequired[bool]
-    isDisplayedSeparately: NotRequired[bool]
-    botScope: NotRequired[Optional[Dict[str, str]]]
+    updatedBy: NotRequired[str]
+    archivedAt: NotRequired[str]
+    archivedBy: NotRequired[str]
```

### Comparing `guilded.py-1.8.0/guilded/types/server.py` & `guilded.py-1.9.0/guilded/types/server.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.8.0/guilded/types/social_link.py` & `guilded.py-1.9.0/guilded/types/social_link.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.8.0/guilded/types/user.py` & `guilded.py-1.9.0/guilded/types/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,19 @@
 """
 
 from __future__ import annotations
 from typing import Any, Dict, List, Literal, Optional, TypedDict, Union
 from typing_extensions import NotRequired
 
 
+class UserStatus(TypedDict):
+    content: NotRequired[str]
+    emoteId: int
+
+
 class UserSummary(TypedDict):
     id: str
     type: NotRequired[Literal['user', 'bot']]
     name: str
     avatar: NotRequired[Optional[str]]
 
 
@@ -52,14 +57,15 @@
     joinDate: NotRequired[str]
     lastOnline: NotRequired[str]
     steamId: NotRequired[str]
     stonks: NotRequired[int]
     badges: NotRequired[List[str]]
     flairInfos: NotRequired[Dict[str, Any]]
     teams: NotRequired[Union[Literal[False], List[Dict[str, Any]]]]
+    status: NotRequired[UserStatus]
 
 
 class ServerMemberSummary(TypedDict):
     user: UserSummary
     roleIds: List[int]
```

### Comparing `guilded.py-1.8.0/guilded/types/webhook.py` & `guilded.py-1.9.0/guilded/status.py`

 * *Files 13% similar despite different names*

```diff
@@ -47,33 +47,40 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
 from __future__ import annotations
 
-from typing import Optional, TypedDict
-from typing_extensions import NotRequired
+from typing import TYPE_CHECKING, Tuple
 
+if TYPE_CHECKING:
+    from .types.user import UserStatus as UserStatusPayload
 
-class PartialWebhook(TypedDict):
-    id: str
-    name: str
-    token: NotRequired[Optional[str]]
-    channelId: NotRequired[str]
-    deletedAt: NotRequired[str]
-    createdAt: NotRequired[str]
 
+__all__ = (
+    'Status',
+)
 
-class _UserWebhook(TypedDict, total=False):
-    teamId: str
-    iconUrl: Optional[str]
-    createdBy: NotRequired[str]
 
+class Status:
+    """Represents a user's status.
 
-class _Webhook(TypedDict, total=False):
-    avatar: NotRequired[str]
-    serverId: str
+    This is displayed under the user's name in the sidebar, analogous to an
+    "activity" on Discord.
 
+    Attributes
+    -----------
+    content: Optional[:class:`str`]
+        The content of the status.
+    emote_id: :class:`int`
+        The ID of the emote associated with the status.
+    """
 
-class Webhook(PartialWebhook, _UserWebhook, _Webhook):
-    ...
+    __slots__: Tuple[str, ...] = (
+        'content',
+        'emote_id',
+    )
+
+    def __init__(self, *, data: UserStatusPayload):
+        self.content = data.get('content')
+        self.emote_id = data['emoteId']
```

### Comparing `guilded.py-1.8.0/guilded/user.py` & `guilded.py-1.9.0/guilded/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,20 +51,21 @@
 
 from __future__ import annotations
 
 import datetime
 import inspect
 import itertools
 from operator import attrgetter
-from typing import TYPE_CHECKING, List, Optional, Tuple, TypeVar, Union
+from typing import TYPE_CHECKING, List, Optional, Set, Tuple, TypeVar, Union
 
 import guilded.abc
 
 from .asset import Asset
 from .enums import SocialLinkType, try_enum
+from .permissions import Permissions
 from .role import Role
 from .utils import MISSING, Object, copy_doc, ISO8601
 
 if TYPE_CHECKING:
     from .types.user import (
         User as UserPayload,
         ServerMember as ServerMemberPayload,
@@ -226,15 +227,14 @@
     """
 
     __slots__ = (
         '_state',
         '_role_ids',
         '_user'
         '_server',
-        'bot_id',
         'nick',
         'xp',
         'joined_at',
         'colour',
     )
 
     if TYPE_CHECKING:
@@ -286,21 +286,41 @@
             self.server.get_role(int(role_id))
             for role_id in self._role_ids
             if self.server.get_role(int(role_id)) is not None
         ]
         return roles
 
     @property
-    def bot(self) -> bool:
-        """:class:`bool`: Whether the member is a bot or webhook."""
-        return self._user.bot or (
-            self.server is not None
-            and self.server.bot_role is not None
-            and self.server.bot_role.id in self._role_ids
-        )
+    def server_permissions(self) -> Permissions:
+        """:class:`.Permissions`: The server-level permissions that this
+        member has.
+
+        This only considers the permissions immediately granted by the
+        member's roles and not any channel permission overwrites.
+
+        This does take into consideration server ownership.
+
+        .. versionadded:: 1.9
+        """
+        if self.is_owner():
+            return Permissions.all()
+
+        values: List[str] = []
+        for role in self.roles:
+            values += role.permissions.values
+
+        return Permissions(*set(values))
+
+    @property
+    def guild_permissions(self) -> Permissions:
+        """:class:`.Permissions`: |dpyattr|
+
+        This is an alias of :attr:`.server_permissions`.
+        """
+        return self.server_permissions
 
     @classmethod
     def _copy(cls, member: Member):
         self = cls.__new__(cls)
 
         self._user = member._user
         self._role_ids = member._role_ids.copy()
@@ -528,21 +548,21 @@
         return data['roleIds']
 
     async def fetch_social_link(self, social_link_type: SocialLinkType, /) -> SocialLink:
         """|coro|
 
         Fetch one of this member's social links.
 
+        .. versionadded:: 1.3
+
         Parameters
         -----------
         social_link_type: :class:`SocialLinkType`
             The type of social link to get.
 
-        .. versionadded:: 1.3
-
         Returns
         --------
         :class:`SocialLink`
             The member's social link on the external service.
 
         Raises
         -------
@@ -699,14 +719,16 @@
 
             Checks if two social links are equal.
 
         .. describe:: x != y
 
             Checks if two social links are not equal.
 
+    .. versionadded:: 1.3
+
     Attributes
     -----------
     user: Union[:class:`Member`, :class:`~guilded.User`]
         The social link's parent member or user.
     user_id: :class:`str`
         The ID of the social link's parent user.
     type: :class:`SocialLinkType`
```

### Comparing `guilded.py-1.8.0/guilded/utils.py` & `guilded.py-1.9.0/guilded/utils.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.8.0/guilded/webhook/async_.py` & `guilded.py-1.9.0/guilded/webhook/async_.py`

 * *Files identical despite different names*

### Comparing `guilded.py-1.8.0/guilded.py.egg-info/PKG-INFO` & `guilded.py-1.9.0/guilded.py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guilded.py
-Version: 1.8.0
+Version: 1.9.0
 Summary: An API wrapper in Python for Guilded's bot API
 Home-page: https://github.com/shayypy/guilded.py
 Author: shay (shayypy)
 License: MIT
 Project-URL: Documentation, https://guildedpy.readthedocs.io/en/latest/
 Project-URL: Issue tracker, https://github.com/shayypy/guilded.py/issues
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `guilded.py-1.8.0/guilded.py.egg-info/SOURCES.txt` & `guilded.py-1.9.0/guilded.py.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 LICENSE
 README.md
 setup.py
 guilded/__init__.py
 guilded/abc.py
-guilded/activity.py
 guilded/asset.py
 guilded/backoff.py
 guilded/channel.py
 guilded/client.py
 guilded/colour.py
 guilded/embed.py
 guilded/emote.py
@@ -25,14 +24,15 @@
 guilded/permissions.py
 guilded/presence.py
 guilded/reaction.py
 guilded/reply.py
 guilded/role.py
 guilded/server.py
 guilded/status.py
+guilded/subscription.py
 guilded/user.py
 guilded/utils.py
 guilded.py.egg-info/PKG-INFO
 guilded.py.egg-info/SOURCES.txt
 guilded.py.egg-info/dependency_links.txt
 guilded.py.egg-info/requires.txt
 guilded.py.egg-info/top_level.txt
@@ -53,18 +53,20 @@
 guilded/types/channel.py
 guilded/types/comment.py
 guilded/types/doc.py
 guilded/types/embed.py
 guilded/types/emote.py
 guilded/types/forum_topic.py
 guilded/types/gateway.py
+guilded/types/group.py
 guilded/types/list_item.py
 guilded/types/message.py
 guilded/types/reaction.py
 guilded/types/role.py
 guilded/types/server.py
 guilded/types/social_link.py
+guilded/types/subscription.py
 guilded/types/user.py
 guilded/types/webhook.py
 guilded/webhook/__init__.py
 guilded/webhook/async_.py
 guilded/webhook/sync.py
```

### Comparing `guilded.py-1.8.0/setup.py` & `guilded.py-1.9.0/setup.py`

 * *Files identical despite different names*

