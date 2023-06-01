# Comparing `tmp/MeUtils-2023.5.9.15.50.17.tar.gz` & `tmp/MeUtils-2023.6.1.12.25.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MeUtils-2023.5.9.15.50.17.tar", last modified: Tue May  9 07:50:17 2023, max compression
+gzip compressed data, was "MeUtils-2023.6.1.12.25.13.tar", last modified: Thu Jun  1 04:25:13 2023, max compression
```

## Comparing `MeUtils-2023.5.9.15.50.17.tar` & `MeUtils-2023.6.1.12.25.13.tar`

### file list

```diff
@@ -1,688 +1,532 @@
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.947408 MeUtils-2023.5.9.15.50.17/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.837857 MeUtils-2023.5.9.15.50.17/.idea/
--rw-r--r--   0 betterme   (501) staff       (20)      182 2023-04-14 01:04:23.000000 MeUtils-2023.5.9.15.50.17/.idea/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)      742 2023-04-14 01:04:23.000000 MeUtils-2023.5.9.15.50.17/.idea/MeUtils.iml
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.838118 MeUtils-2023.5.9.15.50.17/.idea/inspectionProfiles/
--rw-r--r--   0 betterme   (501) staff       (20)     3037 2023-04-14 01:04:23.000000 MeUtils-2023.5.9.15.50.17/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 betterme   (501) staff       (20)      174 2023-04-14 01:04:23.000000 MeUtils-2023.5.9.15.50.17/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 betterme   (501) staff       (20)      195 2023-04-14 01:05:27.000000 MeUtils-2023.5.9.15.50.17/.idea/misc.xml
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-14 01:04:23.000000 MeUtils-2023.5.9.15.50.17/.idea/modules.xml
--rw-r--r--   0 betterme   (501) staff       (20)      167 2023-04-14 01:04:23.000000 MeUtils-2023.5.9.15.50.17/.idea/vcs.xml
--rw-r--r--   0 betterme   (501) staff       (20)    11357 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      249 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/MANIFEST.in
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.838902 MeUtils-2023.5.9.15.50.17/MeUtils.egg-info/
--rw-r--r--   0 betterme   (501) staff       (20)     1867 2023-05-09 07:50:17.000000 MeUtils-2023.5.9.15.50.17/MeUtils.egg-info/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)    24178 2023-05-09 07:50:17.000000 MeUtils-2023.5.9.15.50.17/MeUtils.egg-info/SOURCES.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-05-09 07:50:17.000000 MeUtils-2023.5.9.15.50.17/MeUtils.egg-info/dependency_links.txt
--rw-r--r--   0 betterme   (501) staff       (20)      193 2023-05-09 07:50:17.000000 MeUtils-2023.5.9.15.50.17/MeUtils.egg-info/entry_points.txt
--rw-r--r--   0 betterme   (501) staff       (20)      949 2023-05-09 07:50:17.000000 MeUtils-2023.5.9.15.50.17/MeUtils.egg-info/requires.txt
--rw-r--r--   0 betterme   (501) staff       (20)       17 2023-05-09 07:50:17.000000 MeUtils-2023.5.9.15.50.17/MeUtils.egg-info/top_level.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1867 2023-05-09 07:50:17.947150 MeUtils-2023.5.9.15.50.17/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     1067 2023-05-04 03:00:27.000000 MeUtils-2023.5.9.15.50.17/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      684 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/clear_git_history.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      196 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/git_init.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.843819 MeUtils-2023.5.9.15.50.17/meutils/
--rw-r--r--   0 betterme   (501) staff       (20)      348 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1850 2023-04-11 05:47:45.000000 MeUtils-2023.5.9.15.50.17/meutils/_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.845586 MeUtils-2023.5.9.15.50.17/meutils/annzoo/
--rw-r--r--   0 betterme   (501) staff       (20)      781 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/annzoo/README.md
--rw-r--r--   0 betterme   (501) staff       (20)     1389 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/annzoo/README_gensim.md
--rw-r--r--   0 betterme   (501) staff       (20)      240 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/annzoo/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     9161 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/annzoo/ann.py
--rw-r--r--   0 betterme   (501) staff       (20)     5662 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/annzoo/ann_faiss.py
--rw-r--r--   0 betterme   (501) staff       (20)      965 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/annzoo/ann_gensim.py
--rw-r--r--   0 betterme   (501) staff       (20)     1171 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/annzoo/ann_service.py
--rw-r--r--   0 betterme   (501) staff       (20)     4743 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/annzoo/ann_v1.py
--rw-r--r--   0 betterme   (501) staff       (20)     1927 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/annzoo/cli.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.845888 MeUtils-2023.5.9.15.50.17/meutils/annzoo/examples/
--rw-r--r--   0 betterme   (501) staff       (20)     1476 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/annzoo/examples/client.py
--rw-r--r--   0 betterme   (501) staff       (20)      463 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/annzoo/examples/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)      238 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/annzoo/milvus.py
--rw-r--r--   0 betterme   (501) staff       (20)     1076 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/annzoo/shake_demo.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.846035 MeUtils-2023.5.9.15.50.17/meutils/asyncio_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      243 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/asyncio_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     6034 2023-05-05 05:00:40.000000 MeUtils-2023.5.9.15.50.17/meutils/cache_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.847354 MeUtils-2023.5.9.15.50.17/meutils/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2828 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/clis/cli.py
--rw-r--r--   0 betterme   (501) staff       (20)      738 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/clis/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)     2234 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/clis/cron.py
--rw-r--r--   0 betterme   (501) staff       (20)      595 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/clis/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)     1517 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/clis/gunicorn.conf.py
--rw-r--r--   0 betterme   (501) staff       (20)      619 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/clis/monitor.py
--rw-r--r--   0 betterme   (501) staff       (20)     1018 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/clis/nesc.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.848086 MeUtils-2023.5.9.15.50.17/meutils/cmds/
--rw-r--r--   0 betterme   (501) staff       (20)     1185 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/cmds/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      293 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/cmds/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      458 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/cmds/cmd.py
--rw-r--r--   0 betterme   (501) staff       (20)     1734 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/cmds/hdfs_cmd.py
--rw-r--r--   0 betterme   (501) staff       (20)      629 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/cmds/subprocess_demo.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.848370 MeUtils-2023.5.9.15.50.17/meutils/coding/
--rw-r--r--   0 betterme   (501) staff       (20)      244 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/coding/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      942 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/coding/find132.py
--rw-r--r--   0 betterme   (501) staff       (20)     8275 2023-04-27 09:03:26.000000 MeUtils-2023.5.9.15.50.17/meutils/common.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.848668 MeUtils-2023.5.9.15.50.17/meutils/comp_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      361 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/comp_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1705 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/comp_utils/reverse_metric.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.854469 MeUtils-2023.5.9.15.50.17/meutils/data/
--rw-r--r--   0 betterme   (501) staff       (20) 10062565 2022-11-07 06:01:38.000000 MeUtils-2023.5.9.15.50.17/meutils/data/SimHei.ttf
--rw-r--r--   0 betterme   (501) staff       (20)       19 2023-05-09 07:50:17.000000 MeUtils-2023.5.9.15.50.17/meutils/data/VERSION
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/data/_FLAG
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/data/_SUCCESS
--rw-r--r--   0 betterme   (501) staff       (20)      243 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/data/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      600 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/data/coordinate.py
--rw-r--r--   0 betterme   (501) staff       (20)     2514 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/date_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.859963 MeUtils-2023.5.9.15.50.17/meutils/db/
--rw-r--r--   0 betterme   (501) staff       (20)     1507 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/db/README.md
--rw-r--r--   0 betterme   (501) staff       (20)     4817 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/db/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2337 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/db/mongo.py
--rw-r--r--   0 betterme   (501) staff       (20)     2168 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/db/neo4j.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.862671 MeUtils-2023.5.9.15.50.17/meutils/decorators/
--rw-r--r--   0 betterme   (501) staff       (20)      238 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/decorators/README.md
--rw-r--r--   0 betterme   (501) staff       (20)     3284 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/decorators/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1679 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/decorators/ai.py
--rw-r--r--   0 betterme   (501) staff       (20)     1837 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/decorators/catch.py
--rw-r--r--   0 betterme   (501) staff       (20)     6730 2023-05-04 01:22:21.000000 MeUtils-2023.5.9.15.50.17/meutils/decorators/common.py
--rw-r--r--   0 betterme   (501) staff       (20)    15570 2023-04-06 06:24:58.000000 MeUtils-2023.5.9.15.50.17/meutils/decorators/decorator.py
--rw-r--r--   0 betterme   (501) staff       (20)      754 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/decorators/decorator_demo.py
--rw-r--r--   0 betterme   (501) staff       (20)      527 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/decorators/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)     2115 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/decorators/feishu.py
--rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/decorators/retry.py
--rw-r--r--   0 betterme   (501) staff       (20)     1678 2023-04-04 15:22:58.000000 MeUtils-2023.5.9.15.50.17/meutils/decorators/scheduler.py
--rw-r--r--   0 betterme   (501) staff       (20)     3536 2023-03-31 02:35:37.000000 MeUtils-2023.5.9.15.50.17/meutils/dist_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.863053 MeUtils-2023.5.9.15.50.17/meutils/docarray_/
--rw-r--r--   0 betterme   (501) staff       (20)      334 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.865060 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/
--rw-r--r--   0 betterme   (501) staff       (20)       59 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1561 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/annlite.py
--rw-r--r--   0 betterme   (501) staff       (20)      581 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/base.py
--rw-r--r--   0 betterme   (501) staff       (20)     2088 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/chunk.py
--rw-r--r--   0 betterme   (501) staff       (20)     8448 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/document.py
--rw-r--r--   0 betterme   (501) staff       (20)      715 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/elastic.py
--rw-r--r--   0 betterme   (501) staff       (20)     1736 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/match.py
--rw-r--r--   0 betterme   (501) staff       (20)     1111 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/memory.py
--rw-r--r--   0 betterme   (501) staff       (20)     1486 2023-04-21 00:49:09.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/milvus.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.869083 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/
--rw-r--r--   0 betterme   (501) staff       (20)     2465 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     5114 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/content.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.869371 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/dataloader/
--rw-r--r--   0 betterme   (501) staff       (20)     2939 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/dataloader/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2419 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/dataloader/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)     2966 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/delitem.py
--rw-r--r--   0 betterme   (501) staff       (20)     7175 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/embed.py
--rw-r--r--   0 betterme   (501) staff       (20)      649 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/empty.py
--rw-r--r--   0 betterme   (501) staff       (20)    21535 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/evaluation.py
--rw-r--r--   0 betterme   (501) staff       (20)    13576 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     1845 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/getattr.py
--rw-r--r--   0 betterme   (501) staff       (20)     4237 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/getitem.py
--rw-r--r--   0 betterme   (501) staff       (20)     3803 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/group.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.870699 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/io/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/io/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)    14676 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/io/binary.py
--rw-r--r--   0 betterme   (501) staff       (20)     2588 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/io/common.py
--rw-r--r--   0 betterme   (501) staff       (20)     4181 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/io/csv.py
--rw-r--r--   0 betterme   (501) staff       (20)     1317 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/io/dataframe.py
--rw-r--r--   0 betterme   (501) staff       (20)     9193 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/io/from_gen.py
--rw-r--r--   0 betterme   (501) staff       (20)     3223 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/io/json.py
--rw-r--r--   0 betterme   (501) staff       (20)     1348 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/io/pbar.py
--rw-r--r--   0 betterme   (501) staff       (20)    10591 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/io/pushpull.py
--rw-r--r--   0 betterme   (501) staff       (20)     4762 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/match.py
--rw-r--r--   0 betterme   (501) staff       (20)    15464 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/parallel.py
--rw-r--r--   0 betterme   (501) staff       (20)    20479 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/plot.py
--rw-r--r--   0 betterme   (501) staff       (20)     3910 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/post.py
--rw-r--r--   0 betterme   (501) staff       (20)     1243 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/pydantic.py
--rw-r--r--   0 betterme   (501) staff       (20)     4129 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/reduce.py
--rw-r--r--   0 betterme   (501) staff       (20)     1612 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/sample.py
--rw-r--r--   0 betterme   (501) staff       (20)     8834 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/setitem.py
--rw-r--r--   0 betterme   (501) staff       (20)      833 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/strawberry.py
--rw-r--r--   0 betterme   (501) staff       (20)     1086 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/text.py
--rw-r--r--   0 betterme   (501) staff       (20)     9638 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/traverse.py
--rw-r--r--   0 betterme   (501) staff       (20)      733 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/opensearch.py
--rw-r--r--   0 betterme   (501) staff       (20)     1806 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/qdrant.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.871178 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/queryset/
--rw-r--r--   0 betterme   (501) staff       (20)       64 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/queryset/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     8771 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/queryset/lookup.py
--rw-r--r--   0 betterme   (501) staff       (20)     3680 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/queryset/parser.py
--rw-r--r--   0 betterme   (501) staff       (20)      647 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/redis.py
--rw-r--r--   0 betterme   (501) staff       (20)     1232 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/sqlite.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.871447 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.872328 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/annlite/
--rw-r--r--   0 betterme   (501) staff       (20)      473 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/annlite/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     4062 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/annlite/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     2078 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/annlite/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     2365 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/annlite/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     4541 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/annlite/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)     1424 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/annlite/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.873031 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/base/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/base/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     3861 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/base/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)    12782 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/base/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     2078 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/base/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)     2680 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/base/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.873710 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/elastic/
--rw-r--r--   0 betterme   (501) staff       (20)      473 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/elastic/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     9847 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/elastic/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     5811 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/elastic/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     4746 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/elastic/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     3838 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/elastic/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.874368 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/memory/
--rw-r--r--   0 betterme   (501) staff       (20)      437 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/memory/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2751 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/memory/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     8505 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/memory/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     2453 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/memory/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     2046 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/memory/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.875095 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/milvus/
--rw-r--r--   0 betterme   (501) staff       (20)      315 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/milvus/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)    12584 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/milvus/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     1897 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/milvus/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     4492 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/milvus/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     2772 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/milvus/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.875868 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/opensearch/
--rw-r--r--   0 betterme   (501) staff       (20)      491 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/opensearch/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)    10803 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/opensearch/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     6436 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/opensearch/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     4491 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/opensearch/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     3913 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/opensearch/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.876805 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/qdrant/
--rw-r--r--   0 betterme   (501) staff       (20)     1492 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/qdrant/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     9051 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/qdrant/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     4457 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/qdrant/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     4441 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/qdrant/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)      161 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/qdrant/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)     2085 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/qdrant/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.877743 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/redis/
--rw-r--r--   0 betterme   (501) staff       (20)      313 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/redis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     7368 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/redis/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     6653 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/redis/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     4303 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/redis/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     2662 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/redis/seqlike.py
--rw-r--r--   0 betterme   (501) staff       (20)       88 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/registry.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.879017 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/sqlite/
--rw-r--r--   0 betterme   (501) staff       (20)      520 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/sqlite/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     4894 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/sqlite/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     2783 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/sqlite/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     2279 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/sqlite/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)     2735 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/sqlite/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.879964 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/weaviate/
--rw-r--r--   0 betterme   (501) staff       (20)      479 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/weaviate/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)    14786 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/weaviate/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     7830 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/weaviate/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     3285 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/weaviate/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     2834 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/weaviate/seqlike.py
--rw-r--r--   0 betterme   (501) staff       (20)     1689 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/weaviate.py
--rw-r--r--   0 betterme   (501) staff       (20)     4806 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/base.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.880771 MeUtils-2023.5.9.15.50.17/meutils/docarray_/dataclasses/
--rw-r--r--   0 betterme   (501) staff       (20)       80 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/dataclasses/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      633 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/dataclasses/enums.py
--rw-r--r--   0 betterme   (501) staff       (20)     1063 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/dataclasses/getter.py
--rw-r--r--   0 betterme   (501) staff       (20)     2920 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/dataclasses/setter.py
--rw-r--r--   0 betterme   (501) staff       (20)     9205 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/dataclasses/types.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.881475 MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/
--rw-r--r--   0 betterme   (501) staff       (20)     4881 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     5422 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/data.py
--rw-r--r--   0 betterme   (501) staff       (20)    12146 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/generators.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.884986 MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/mixins/
--rw-r--r--   0 betterme   (501) staff       (20)     1779 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/mixins/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     5775 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/mixins/_property.py
--rw-r--r--   0 betterme   (501) staff       (20)      856 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/mixins/attribute.py
--rw-r--r--   0 betterme   (501) staff       (20)     2987 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/mixins/audio.py
--rw-r--r--   0 betterme   (501) staff       (20)     1988 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/mixins/blob.py
--rw-r--r--   0 betterme   (501) staff       (20)      866 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/mixins/content.py
--rw-r--r--   0 betterme   (501) staff       (20)     2034 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/mixins/convert.py
--rw-r--r--   0 betterme   (501) staff       (20)      701 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/mixins/dump.py
--rw-r--r--   0 betterme   (501) staff       (20)     2942 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/mixins/featurehash.py
--rw-r--r--   0 betterme   (501) staff       (20)     2749 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/mixins/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)    19532 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/mixins/image.py
--rw-r--r--   0 betterme   (501) staff       (20)     5080 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/mixins/mesh.py
--rw-r--r--   0 betterme   (501) staff       (20)     8677 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/mixins/multimodal.py
--rw-r--r--   0 betterme   (501) staff       (20)    14400 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/mixins/plot.py
--rw-r--r--   0 betterme   (501) staff       (20)     6281 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/mixins/porting.py
--rw-r--r--   0 betterme   (501) staff       (20)     2930 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/mixins/property.py
--rw-r--r--   0 betterme   (501) staff       (20)      839 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/mixins/protobuf.py
--rw-r--r--   0 betterme   (501) staff       (20)     2891 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/mixins/pydantic.py
--rw-r--r--   0 betterme   (501) staff       (20)     1120 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/mixins/rich_embedding.py
--rw-r--r--   0 betterme   (501) staff       (20)     2601 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/mixins/strawberry.py
--rw-r--r--   0 betterme   (501) staff       (20)     6782 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/mixins/sugar.py
--rw-r--r--   0 betterme   (501) staff       (20)     4811 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/mixins/text.py
--rw-r--r--   0 betterme   (501) staff       (20)     5987 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/mixins/video.py
--rw-r--r--   0 betterme   (501) staff       (20)     2277 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/pydantic_model.py
--rw-r--r--   0 betterme   (501) staff       (20)     2691 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/strawberry_type.py
--rw-r--r--   0 betterme   (501) staff       (20)    15985 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/helper.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.885473 MeUtils-2023.5.9.15.50.17/meutils/docarray_/math/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/math/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.886111 MeUtils-2023.5.9.15.50.17/meutils/docarray_/math/distance/
--rw-r--r--   0 betterme   (501) staff       (20)     4465 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/math/distance/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2990 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/math/distance/numpy.py
--rw-r--r--   0 betterme   (501) staff       (20)     2107 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/math/distance/paddle.py
--rw-r--r--   0 betterme   (501) staff       (20)     2287 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/math/distance/tensorflow.py
--rw-r--r--   0 betterme   (501) staff       (20)     1950 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/math/distance/torch.py
--rw-r--r--   0 betterme   (501) staff       (20)     6289 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/math/evaluation.py
--rw-r--r--   0 betterme   (501) staff       (20)     3205 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/math/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)     9093 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/math/ndarray.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.886349 MeUtils-2023.5.9.15.50.17/meutils/docarray_/proto/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/proto/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      173 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/proto/docarray_pb2.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.886610 MeUtils-2023.5.9.15.50.17/meutils/docarray_/proto/io/
--rw-r--r--   0 betterme   (501) staff       (20)     3132 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/proto/io/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     5231 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/proto/io/ndarray.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.886848 MeUtils-2023.5.9.15.50.17/meutils/docarray_/proto/pb/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/proto/pb/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     4228 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/proto/pb/docarray_pb2.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.887073 MeUtils-2023.5.9.15.50.17/meutils/docarray_/proto/pb2/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/proto/pb2/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     7490 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/proto/pb2/docarray_pb2.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.887203 MeUtils-2023.5.9.15.50.17/meutils/docarray_/resources/
--rw-r--r--   0 betterme   (501) staff       (20)     4404 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/resources/ci-vendors.json
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.887328 MeUtils-2023.5.9.15.50.17/meutils/docarray_/resources/embedding-projector/
--rw-r--r--   0 betterme   (501) staff       (20)   494360 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/resources/embedding-projector/index.html.gz
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.888569 MeUtils-2023.5.9.15.50.17/meutils/docarray_/score/
--rw-r--r--   0 betterme   (501) staff       (20)      258 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/score/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      977 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/score/data.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.889068 MeUtils-2023.5.9.15.50.17/meutils/docarray_/score/mixins/
--rw-r--r--   0 betterme   (501) staff       (20)      194 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/score/mixins/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1097 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/score/mixins/property.py
--rw-r--r--   0 betterme   (501) staff       (20)      174 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/score/mixins/representer.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.889199 MeUtils-2023.5.9.15.50.17/meutils/docarray_/typing/
--rw-r--r--   0 betterme   (501) staff       (20)     2187 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_/typing/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.890327 MeUtils-2023.5.9.15.50.17/meutils/docarray_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-18 06:24:19.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      977 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_utils/demo_es.py
--rw-r--r--   0 betterme   (501) staff       (20)     1341 2023-04-26 13:37:46.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_utils/demo_hnsw.py
--rw-r--r--   0 betterme   (501) staff       (20)      985 2023-04-27 02:39:23.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_utils/in_memory.py
--rw-r--r--   0 betterme   (501) staff       (20)     1058 2023-04-27 01:04:00.000000 MeUtils-2023.5.9.15.50.17/meutils/docarray_utils/改造下hnsw.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.890822 MeUtils-2023.5.9.15.50.17/meutils/easy_search/
--rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/easy_search/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2171 2023-04-26 12:04:06.000000 MeUtils-2023.5.9.15.50.17/meutils/easy_search/es.py
--rw-r--r--   0 betterme   (501) staff       (20)     2393 2023-04-04 15:30:40.000000 MeUtils-2023.5.9.15.50.17/meutils/hash_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)      969 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/import_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.891641 MeUtils-2023.5.9.15.50.17/meutils/init/
--rw-r--r--   0 betterme   (501) staff       (20)      242 2023-04-27 08:58:17.000000 MeUtils-2023.5.9.15.50.17/meutils/init/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      933 2023-05-08 05:45:58.000000 MeUtils-2023.5.9.15.50.17/meutils/init/evn.py
--rw-r--r--   0 betterme   (501) staff       (20)    12882 2023-05-05 10:52:25.000000 MeUtils-2023.5.9.15.50.17/meutils/init/oo.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.892680 MeUtils-2023.5.9.15.50.17/meutils/io/
--rw-r--r--   0 betterme   (501) staff       (20)     2107 2023-04-13 02:51:32.000000 MeUtils-2023.5.9.15.50.17/meutils/io/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      409 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/io/file.py
--rw-r--r--   0 betterme   (501) staff       (20)     2290 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/io/image.py
--rw-r--r--   0 betterme   (501) staff       (20)     8580 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/io/tf_io.py
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/io/x.yml
--rw-r--r--   0 betterme   (501) staff       (20)      708 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/jinja_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     2512 2023-04-02 12:55:05.000000 MeUtils-2023.5.9.15.50.17/meutils/log_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.893677 MeUtils-2023.5.9.15.50.17/meutils/nlp_utils/
--rw-r--r--   0 betterme   (501) staff       (20)     6921 2023-04-25 07:32:56.000000 MeUtils-2023.5.9.15.50.17/meutils/nlp_utils/SplitSentence.py
--rw-r--r--   0 betterme   (501) staff       (20)      244 2023-04-25 06:23:09.000000 MeUtils-2023.5.9.15.50.17/meutils/nlp_utils/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.894176 MeUtils-2023.5.9.15.50.17/meutils/nlp_utils/_textsplitter/
--rw-r--r--   0 betterme   (501) staff       (20)      291 2023-04-25 03:45:09.000000 MeUtils-2023.5.9.15.50.17/meutils/nlp_utils/_textsplitter/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     6673 2023-04-25 06:23:09.000000 MeUtils-2023.5.9.15.50.17/meutils/nlp_utils/_textsplitter/chinese_text_splitter.py
--rw-r--r--   0 betterme   (501) staff       (20)     2300 2023-04-25 07:48:57.000000 MeUtils-2023.5.9.15.50.17/meutils/nlp_utils/_textsplitter/text_split.py
--rw-r--r--   0 betterme   (501) staff       (20)     1972 2023-04-24 02:28:40.000000 MeUtils-2023.5.9.15.50.17/meutils/nlp_utils/ner.py
--rw-r--r--   0 betterme   (501) staff       (20)     1997 2023-04-25 07:39:01.000000 MeUtils-2023.5.9.15.50.17/meutils/nlp_utils/textsplitter.py
--rw-r--r--   0 betterme   (501) staff       (20)     3206 2023-04-24 02:28:40.000000 MeUtils-2023.5.9.15.50.17/meutils/nlp_utils/word_segmentation.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.895609 MeUtils-2023.5.9.15.50.17/meutils/notice/
--rw-r--r--   0 betterme   (501) staff       (20)      837 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/notice/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2403 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/notice/emails.py
--rw-r--r--   0 betterme   (501) staff       (20)      703 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/notice/feishu.py
--rw-r--r--   0 betterme   (501) staff       (20)      953 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/notice/file_post.py
--rw-r--r--   0 betterme   (501) staff       (20)     2229 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/notice/wechat.py
--rw-r--r--   0 betterme   (501) staff       (20)     3215 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/notice/wechat_.py
--rw-r--r--   0 betterme   (501) staff       (20)     6983 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/notice/wecom.py
--rw-r--r--   0 betterme   (501) staff       (20)     1102 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/notice/weekmeet.py
--rw-r--r--   0 betterme   (501) staff       (20)     3181 2023-03-31 02:35:37.000000 MeUtils-2023.5.9.15.50.17/meutils/np_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.897041 MeUtils-2023.5.9.15.50.17/meutils/office_automation/
--rw-r--r--   0 betterme   (501) staff       (20)      241 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/office_automation/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      508 2023-03-27 04:08:21.000000 MeUtils-2023.5.9.15.50.17/meutils/office_automation/doc.py
--rw-r--r--   0 betterme   (501) staff       (20)     1538 2023-04-28 07:14:17.000000 MeUtils-2023.5.9.15.50.17/meutils/office_automation/pdf.py
--rw-r--r--   0 betterme   (501) staff       (20)    11894 2023-03-20 03:17:38.000000 MeUtils-2023.5.9.15.50.17/meutils/office_automation/pdm.py
--rw-r--r--   0 betterme   (501) staff       (20)    13502 2023-03-21 06:30:39.000000 MeUtils-2023.5.9.15.50.17/meutils/office_automation/pdm_run.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.898056 MeUtils-2023.5.9.15.50.17/meutils/office_automation/report/
--rw-r--r--   0 betterme   (501) staff       (20)      244 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/office_automation/report/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)   736444 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/office_automation/投资管理系统O3.2_交易组.pdm
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.898865 MeUtils-2023.5.9.15.50.17/meutils/other/
--rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/other/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)    23121 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/other/besttable.py
--rw-r--r--   0 betterme   (501) staff       (20)    44366 2023-03-21 05:16:40.000000 MeUtils-2023.5.9.15.50.17/meutils/other/crontab.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.899560 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/
--rw-r--r--   0 betterme   (501) staff       (20)      334 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.901595 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/
--rw-r--r--   0 betterme   (501) staff       (20)       59 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1561 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/annlite.py
--rw-r--r--   0 betterme   (501) staff       (20)      581 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/base.py
--rw-r--r--   0 betterme   (501) staff       (20)     2088 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/chunk.py
--rw-r--r--   0 betterme   (501) staff       (20)     8448 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/document.py
--rw-r--r--   0 betterme   (501) staff       (20)      715 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/elastic.py
--rw-r--r--   0 betterme   (501) staff       (20)     1736 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/match.py
--rw-r--r--   0 betterme   (501) staff       (20)     1111 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/memory.py
--rw-r--r--   0 betterme   (501) staff       (20)     1486 2023-04-21 00:49:09.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/milvus.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.904742 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/mixins/
--rw-r--r--   0 betterme   (501) staff       (20)     2465 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/mixins/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     5114 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/mixins/content.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.904997 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/mixins/dataloader/
--rw-r--r--   0 betterme   (501) staff       (20)     2939 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/mixins/dataloader/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2419 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/mixins/dataloader/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)     2966 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/mixins/delitem.py
--rw-r--r--   0 betterme   (501) staff       (20)     7175 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/mixins/embed.py
--rw-r--r--   0 betterme   (501) staff       (20)      649 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/mixins/empty.py
--rw-r--r--   0 betterme   (501) staff       (20)    21535 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/mixins/evaluation.py
--rw-r--r--   0 betterme   (501) staff       (20)    13576 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/mixins/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     1845 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/mixins/getattr.py
--rw-r--r--   0 betterme   (501) staff       (20)     4237 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/mixins/getitem.py
--rw-r--r--   0 betterme   (501) staff       (20)     3803 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/mixins/group.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.906255 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/mixins/io/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/mixins/io/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)    14676 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/mixins/io/binary.py
--rw-r--r--   0 betterme   (501) staff       (20)     2588 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/mixins/io/common.py
--rw-r--r--   0 betterme   (501) staff       (20)     4181 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/mixins/io/csv.py
--rw-r--r--   0 betterme   (501) staff       (20)     1317 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/mixins/io/dataframe.py
--rw-r--r--   0 betterme   (501) staff       (20)     9193 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/mixins/io/from_gen.py
--rw-r--r--   0 betterme   (501) staff       (20)     3223 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/mixins/io/json.py
--rw-r--r--   0 betterme   (501) staff       (20)     1348 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/mixins/io/pbar.py
--rw-r--r--   0 betterme   (501) staff       (20)    10591 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/mixins/io/pushpull.py
--rw-r--r--   0 betterme   (501) staff       (20)     4762 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/mixins/match.py
--rw-r--r--   0 betterme   (501) staff       (20)    15464 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/mixins/parallel.py
--rw-r--r--   0 betterme   (501) staff       (20)    20479 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/mixins/plot.py
--rw-r--r--   0 betterme   (501) staff       (20)     3910 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/mixins/post.py
--rw-r--r--   0 betterme   (501) staff       (20)     1243 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/mixins/pydantic.py
--rw-r--r--   0 betterme   (501) staff       (20)     4129 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/mixins/reduce.py
--rw-r--r--   0 betterme   (501) staff       (20)     1612 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/mixins/sample.py
--rw-r--r--   0 betterme   (501) staff       (20)     8834 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/mixins/setitem.py
--rw-r--r--   0 betterme   (501) staff       (20)      833 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/mixins/strawberry.py
--rw-r--r--   0 betterme   (501) staff       (20)     1086 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/mixins/text.py
--rw-r--r--   0 betterme   (501) staff       (20)     9638 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/mixins/traverse.py
--rw-r--r--   0 betterme   (501) staff       (20)      733 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/opensearch.py
--rw-r--r--   0 betterme   (501) staff       (20)     1806 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/qdrant.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.906629 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/queryset/
--rw-r--r--   0 betterme   (501) staff       (20)       64 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/queryset/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     8771 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/queryset/lookup.py
--rw-r--r--   0 betterme   (501) staff       (20)     3680 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/queryset/parser.py
--rw-r--r--   0 betterme   (501) staff       (20)      647 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/redis.py
--rw-r--r--   0 betterme   (501) staff       (20)     1232 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/sqlite.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.906862 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.907621 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/annlite/
--rw-r--r--   0 betterme   (501) staff       (20)      473 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/annlite/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     4062 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/annlite/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     2078 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/annlite/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     2365 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/annlite/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     4541 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/annlite/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)     1424 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/annlite/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.908215 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/base/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/base/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     3861 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/base/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)    12782 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/base/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     2078 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/base/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)     2680 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/base/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.908916 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/elastic/
--rw-r--r--   0 betterme   (501) staff       (20)      473 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/elastic/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     9847 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/elastic/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     5811 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/elastic/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     4746 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/elastic/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     3838 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/elastic/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.909666 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/memory/
--rw-r--r--   0 betterme   (501) staff       (20)      437 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/memory/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2751 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/memory/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     8505 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/memory/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     2453 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/memory/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     2046 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/memory/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.910400 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/milvus/
--rw-r--r--   0 betterme   (501) staff       (20)      315 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/milvus/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)    12584 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/milvus/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     1897 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/milvus/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     4492 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/milvus/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     2772 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/milvus/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.911076 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/opensearch/
--rw-r--r--   0 betterme   (501) staff       (20)      491 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/opensearch/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)    10803 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/opensearch/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     6436 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/opensearch/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     4491 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/opensearch/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     3913 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/opensearch/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.911968 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/qdrant/
--rw-r--r--   0 betterme   (501) staff       (20)     1492 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/qdrant/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     9051 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/qdrant/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     4457 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/qdrant/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     4441 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/qdrant/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)      161 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/qdrant/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)     2085 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/qdrant/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.912706 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/redis/
--rw-r--r--   0 betterme   (501) staff       (20)      313 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/redis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     7368 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/redis/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     6653 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/redis/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     4303 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/redis/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     2662 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/redis/seqlike.py
--rw-r--r--   0 betterme   (501) staff       (20)       88 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/registry.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.913393 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/sqlite/
--rw-r--r--   0 betterme   (501) staff       (20)      520 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/sqlite/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     4894 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/sqlite/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     2783 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/sqlite/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     2279 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/sqlite/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)     2735 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/sqlite/seqlike.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.914368 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/weaviate/
--rw-r--r--   0 betterme   (501) staff       (20)      479 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/weaviate/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)    14786 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/weaviate/backend.py
--rw-r--r--   0 betterme   (501) staff       (20)     7830 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/weaviate/find.py
--rw-r--r--   0 betterme   (501) staff       (20)     3285 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/weaviate/getsetdel.py
--rw-r--r--   0 betterme   (501) staff       (20)     2834 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/storage/weaviate/seqlike.py
--rw-r--r--   0 betterme   (501) staff       (20)     1689 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/array/weaviate.py
--rw-r--r--   0 betterme   (501) staff       (20)     4806 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/base.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.915005 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/dataclasses/
--rw-r--r--   0 betterme   (501) staff       (20)       80 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/dataclasses/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      633 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/dataclasses/enums.py
--rw-r--r--   0 betterme   (501) staff       (20)     1063 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/dataclasses/getter.py
--rw-r--r--   0 betterme   (501) staff       (20)     2920 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/dataclasses/setter.py
--rw-r--r--   0 betterme   (501) staff       (20)     9205 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/dataclasses/types.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.915697 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/document/
--rw-r--r--   0 betterme   (501) staff       (20)     4881 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/document/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     5422 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/document/data.py
--rw-r--r--   0 betterme   (501) staff       (20)    12146 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/document/generators.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.919708 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/document/mixins/
--rw-r--r--   0 betterme   (501) staff       (20)     1779 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/document/mixins/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     5775 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/document/mixins/_property.py
--rw-r--r--   0 betterme   (501) staff       (20)      856 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/document/mixins/attribute.py
--rw-r--r--   0 betterme   (501) staff       (20)     2987 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/document/mixins/audio.py
--rw-r--r--   0 betterme   (501) staff       (20)     1988 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/document/mixins/blob.py
--rw-r--r--   0 betterme   (501) staff       (20)      866 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/document/mixins/content.py
--rw-r--r--   0 betterme   (501) staff       (20)     2034 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/document/mixins/convert.py
--rw-r--r--   0 betterme   (501) staff       (20)      701 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/document/mixins/dump.py
--rw-r--r--   0 betterme   (501) staff       (20)     2942 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/document/mixins/featurehash.py
--rw-r--r--   0 betterme   (501) staff       (20)     2749 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/document/mixins/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)    19532 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/document/mixins/image.py
--rw-r--r--   0 betterme   (501) staff       (20)     5080 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/document/mixins/mesh.py
--rw-r--r--   0 betterme   (501) staff       (20)     8677 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/document/mixins/multimodal.py
--rw-r--r--   0 betterme   (501) staff       (20)    14400 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/document/mixins/plot.py
--rw-r--r--   0 betterme   (501) staff       (20)     6281 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/document/mixins/porting.py
--rw-r--r--   0 betterme   (501) staff       (20)     2930 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/document/mixins/property.py
--rw-r--r--   0 betterme   (501) staff       (20)      839 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/document/mixins/protobuf.py
--rw-r--r--   0 betterme   (501) staff       (20)     2891 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/document/mixins/pydantic.py
--rw-r--r--   0 betterme   (501) staff       (20)     1120 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/document/mixins/rich_embedding.py
--rw-r--r--   0 betterme   (501) staff       (20)     2601 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/document/mixins/strawberry.py
--rw-r--r--   0 betterme   (501) staff       (20)     6782 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/document/mixins/sugar.py
--rw-r--r--   0 betterme   (501) staff       (20)     4811 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/document/mixins/text.py
--rw-r--r--   0 betterme   (501) staff       (20)     5987 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/document/mixins/video.py
--rw-r--r--   0 betterme   (501) staff       (20)     2277 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/document/pydantic_model.py
--rw-r--r--   0 betterme   (501) staff       (20)     2691 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/document/strawberry_type.py
--rw-r--r--   0 betterme   (501) staff       (20)    15985 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/helper.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.920202 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/math/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/math/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.920866 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/math/distance/
--rw-r--r--   0 betterme   (501) staff       (20)     4465 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/math/distance/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2990 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/math/distance/numpy.py
--rw-r--r--   0 betterme   (501) staff       (20)     2107 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/math/distance/paddle.py
--rw-r--r--   0 betterme   (501) staff       (20)     2287 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/math/distance/tensorflow.py
--rw-r--r--   0 betterme   (501) staff       (20)     1950 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/math/distance/torch.py
--rw-r--r--   0 betterme   (501) staff       (20)     6289 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/math/evaluation.py
--rw-r--r--   0 betterme   (501) staff       (20)     3205 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/math/helper.py
--rw-r--r--   0 betterme   (501) staff       (20)     9093 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/math/ndarray.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.921113 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/proto/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/proto/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      173 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/proto/docarray_pb2.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.921368 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/proto/io/
--rw-r--r--   0 betterme   (501) staff       (20)     3132 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/proto/io/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     5231 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/proto/io/ndarray.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.921601 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/proto/pb/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/proto/pb/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     4228 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/proto/pb/docarray_pb2.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.921825 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/proto/pb2/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/proto/pb2/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     7490 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/proto/pb2/docarray_pb2.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.921954 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/resources/
--rw-r--r--   0 betterme   (501) staff       (20)     4404 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/resources/ci-vendors.json
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.922084 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/resources/embedding-projector/
--rw-r--r--   0 betterme   (501) staff       (20)   494360 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/resources/embedding-projector/index.html.gz
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.923190 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/score/
--rw-r--r--   0 betterme   (501) staff       (20)      258 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/score/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      977 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/score/data.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.923625 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/score/mixins/
--rw-r--r--   0 betterme   (501) staff       (20)      194 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/score/mixins/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1097 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/score/mixins/property.py
--rw-r--r--   0 betterme   (501) staff       (20)      174 2023-04-18 09:06:43.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/score/mixins/representer.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.923766 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/typing/
--rw-r--r--   0 betterme   (501) staff       (20)     2187 2023-04-21 04:31:21.000000 MeUtils-2023.5.9.15.50.17/meutils/other/docarray/typing/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.924243 MeUtils-2023.5.9.15.50.17/meutils/pandas_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/pandas_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1228 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/pandas_utils/opt.py
--rw-r--r--   0 betterme   (501) staff       (20)     6300 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/pandas_utils/pd_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     2846 2023-04-13 02:51:32.000000 MeUtils-2023.5.9.15.50.17/meutils/path_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     6084 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/pd_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     8419 2023-04-27 08:56:11.000000 MeUtils-2023.5.9.15.50.17/meutils/pipe.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.925463 MeUtils-2023.5.9.15.50.17/meutils/plot_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      241 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/plot_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      265 2023-05-09 07:50:11.000000 MeUtils-2023.5.9.15.50.17/meutils/plot_utils/common.py
--rw-r--r--   0 betterme   (501) staff       (20)      732 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/plot_utils/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)     2611 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/plot_utils/echarts.py
--rw-r--r--   0 betterme   (501) staff       (20)    11980 2023-05-09 07:49:05.000000 MeUtils-2023.5.9.15.50.17/meutils/plot_utils/embedding_plot.py
--rw-r--r--   0 betterme   (501) staff       (20)     3610 2023-04-24 07:54:55.000000 MeUtils-2023.5.9.15.50.17/meutils/plot_utils/mecharts.py
--rw-r--r--   0 betterme   (501) staff       (20)    19326 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/plot_utils/metrics.py
--rw-r--r--   0 betterme   (501) staff       (20)     2449 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/plot_utils/plot_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.926774 MeUtils-2023.5.9.15.50.17/meutils/request_utils/
--rw-r--r--   0 betterme   (501) staff       (20)     2461 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/request_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1503 2023-04-21 05:45:54.000000 MeUtils-2023.5.9.15.50.17/meutils/request_utils/crawler.py
--rw-r--r--   0 betterme   (501) staff       (20)     1767 2023-03-30 02:00:48.000000 MeUtils-2023.5.9.15.50.17/meutils/request_utils/download.py
--rw-r--r--   0 betterme   (501) staff       (20)     1334 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/request_utils/results.py
--rw-r--r--   0 betterme   (501) staff       (20)      417 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/request_utils/wechat.py
--rw-r--r--   0 betterme   (501) staff       (20)      644 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/request_utils/公网ip.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.927422 MeUtils-2023.5.9.15.50.17/meutils/serving/
--rw-r--r--   0 betterme   (501) staff       (20)       22 2023-04-28 03:00:12.000000 MeUtils-2023.5.9.15.50.17/meutils/serving/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-28 02:50:45.000000 MeUtils-2023.5.9.15.50.17/meutils/serving/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2397 2023-04-28 05:43:39.000000 MeUtils-2023.5.9.15.50.17/meutils/serving/_fastapi.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.928419 MeUtils-2023.5.9.15.50.17/meutils/serving/gui/
--rw-r--r--   0 betterme   (501) staff       (20)       10 2023-04-18 07:29:22.000000 MeUtils-2023.5.9.15.50.17/meutils/serving/gui/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1658 2023-03-21 01:20:09.000000 MeUtils-2023.5.9.15.50.17/meutils/serving/gui/bar.py
--rw-r--r--   0 betterme   (501) staff       (20)     1273 2023-04-18 07:21:04.000000 MeUtils-2023.5.9.15.50.17/meutils/serving/gui/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)      210 2023-03-21 01:26:30.000000 MeUtils-2023.5.9.15.50.17/meutils/serving/gui/run.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.929825 MeUtils-2023.5.9.15.50.17/meutils/serving/st_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      290 2023-04-28 10:26:48.000000 MeUtils-2023.5.9.15.50.17/meutils/serving/st_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      898 2023-04-28 10:41:27.000000 MeUtils-2023.5.9.15.50.17/meutils/serving/st_utils/_test.py
--rw-r--r--   0 betterme   (501) staff       (20)     6995 2023-04-28 10:39:20.000000 MeUtils-2023.5.9.15.50.17/meutils/serving/st_utils/common.py
--rw-r--r--   0 betterme   (501) staff       (20)      131 2023-04-28 10:38:41.000000 MeUtils-2023.5.9.15.50.17/meutils/serving/st_utils/conf.yaml
--rw-r--r--   0 betterme   (501) staff       (20)      218 2023-04-28 10:38:28.000000 MeUtils-2023.5.9.15.50.17/meutils/serving/st_utils/run.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.930102 MeUtils-2023.5.9.15.50.17/meutils/serving/webui/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-28 02:48:41.000000 MeUtils-2023.5.9.15.50.17/meutils/serving/webui/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      956 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/sftp.py
--rw-r--r--   0 betterme   (501) staff       (20)      796 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/sk_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     1398 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/smooth_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.930235 MeUtils-2023.5.9.15.50.17/meutils/spark/
--rw-r--r--   0 betterme   (501) staff       (20)      576 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/spark/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.930966 MeUtils-2023.5.9.15.50.17/meutils/str_utils/
--rw-r--r--   0 betterme   (501) staff       (20)     1258 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/str_utils/Translator.py
--rw-r--r--   0 betterme   (501) staff       (20)     6417 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/str_utils/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.931798 MeUtils-2023.5.9.15.50.17/meutils/str_utils/__translater/
--rw-r--r--   0 betterme   (501) staff       (20)      277 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/str_utils/__translater/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1408 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/str_utils/__translater/tencent.py
--rw-r--r--   0 betterme   (501) staff       (20)     1238 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/str_utils/__translater/translater.py
--rw-r--r--   0 betterme   (501) staff       (20)     1168 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/str_utils/__translater/youdao.py
--rw-r--r--   0 betterme   (501) staff       (20)     1002 2023-04-07 09:07:13.000000 MeUtils-2023.5.9.15.50.17/meutils/str_utils/json_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)      926 2023-04-09 12:05:21.000000 MeUtils-2023.5.9.15.50.17/meutils/str_utils/regular_expression.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.933591 MeUtils-2023.5.9.15.50.17/meutils/templates/
--rw-r--r--   0 betterme   (501) staff       (20)      349 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      291 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      224 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/demo.conf
--rw-r--r--   0 betterme   (501) staff       (20)      578 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/demo.j2
--rw-r--r--   0 betterme   (501) staff       (20)      808 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)      536 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/demox.py
--rw-r--r--   0 betterme   (501) staff       (20)     2416 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/df_html.j2
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.937850 MeUtils-2023.5.9.15.50.17/meutils/templates/dockerfiles/
--rw-r--r--   0 betterme   (501) staff       (20)      112 2023-03-21 05:16:40.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/dockerfiles/Dockerfile
--rw-r--r--   0 betterme   (501) staff       (20)      170 2023-03-21 05:16:40.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/dockerfiles/Dockerfile_me
--rw-r--r--   0 betterme   (501) staff       (20)      217 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/dockerfiles/Dockerfile_milvus
--rw-r--r--   0 betterme   (501) staff       (20)      245 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/dockerfiles/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      712 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/dockerfiles/docker_build_push.py
--rwxr-xr-x   0 betterme   (501) staff       (20)      386 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/dockerfiles/docker_push.sh
--rw-r--r--   0 betterme   (501) staff       (20)     2266 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/hegui.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.938006 MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/
--rw-r--r--   0 betterme   (501) staff       (20)      831 2022-05-05 05:21:39.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/cookiecutter.json
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.941252 MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/
--rw-r--r--   0 betterme   (501) staff       (20)      292 2021-09-03 02:19:39.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.editorconfig
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.941403 MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.github/
--rw-r--r--   0 betterme   (501) staff       (20)      342 2021-09-03 02:19:39.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 betterme   (501) staff       (20)     1207 2023-04-18 10:18:45.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)      842 2021-09-03 02:19:39.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.travis.yml
--rw-r--r--   0 betterme   (501) staff       (20)      178 2021-09-03 02:19:39.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/AUTHORS.rst
--rw-r--r--   0 betterme   (501) staff       (20)     4010 2021-09-03 02:19:39.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/CONTRIBUTING.rst
--rw-r--r--   0 betterme   (501) staff       (20)      117 2021-09-03 02:19:39.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/HISTORY.rst
--rw-r--r--   0 betterme   (501) staff       (20)     5987 2021-09-03 02:19:39.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      351 2021-09-04 06:53:23.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/MANIFEST.in
--rw-r--r--   0 betterme   (501) staff       (20)     2516 2021-09-03 02:19:39.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)      704 2023-04-18 10:20:21.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.md
--rw-r--r--   0 betterme   (501) staff       (20)     1738 2021-09-03 02:19:39.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.rst
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.943566 MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/
--rw-r--r--   0 betterme   (501) staff       (20)      632 2021-09-03 02:19:39.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)      702 2021-09-14 08:44:31.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/README.md
--rw-r--r--   0 betterme   (501) staff       (20)       26 2022-04-18 06:25:28.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/_config.yml
--rw-r--r--   0 betterme   (501) staff       (20)       28 2021-09-03 02:19:39.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/authors.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)     5157 2021-09-03 02:19:39.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)       33 2021-09-03 02:19:39.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/contributing.rst
--rw-r--r--   0 betterme   (501) staff       (20)       28 2021-09-03 02:19:39.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/history.rst
--rw-r--r--   0 betterme   (501) staff       (20)      388 2021-09-03 02:19:39.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/index.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1410 2021-09-03 02:19:39.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/installation.rst
--rw-r--r--   0 betterme   (501) staff       (20)      829 2021-09-03 02:19:39.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/make.bat
--rw-r--r--   0 betterme   (501) staff       (20)       27 2021-09-03 02:19:39.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/readme.rst
--rw-r--r--   0 betterme   (501) staff       (20)      117 2021-09-03 02:19:39.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/usage.rst
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.943750 MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/examples/
--rw-r--r--   0 betterme   (501) staff       (20)      234 2021-09-04 07:26:59.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/examples/demo.py
--rwxr--r--   0 betterme   (501) staff       (20)      244 2022-05-05 05:24:52.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/git_init.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      152 2021-09-01 08:44:34.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)        8 2021-09-03 02:19:39.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)      302 2021-09-03 02:19:39.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/requirements_dev.txt
--rw-r--r--   0 betterme   (501) staff       (20)      549 2021-09-03 02:19:39.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     2532 2022-04-19 09:34:52.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.944070 MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/
--rw-r--r--   0 betterme   (501) staff       (20)       61 2021-09-03 02:19:39.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2315 2021-09-03 02:32:04.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/test_{{cookiecutter.project_slug}}.py
--rw-r--r--   0 betterme   (501) staff       (20)      678 2021-09-03 02:19:39.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tox.ini
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.944407 MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/
--rw-r--r--   0 betterme   (501) staff       (20)      273 2022-04-18 06:39:54.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.944947 MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2021-08-31 05:12:27.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2022-04-27 09:56:07.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      591 2022-04-27 09:56:07.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/cli.py
--rw-r--r--   0 betterme   (501) staff       (20)       19 2021-09-03 02:19:39.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}.py
--rw-r--r--   0 betterme   (501) staff       (20)    11496 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/tpl.docx
--rw-r--r--   0 betterme   (501) staff       (20)   172819 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/templates/合规日报模板.docx
--rw-r--r--   0 betterme   (501) staff       (20)      590 2023-05-08 05:49:55.000000 MeUtils-2023.5.9.15.50.17/meutils/todo.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.946314 MeUtils-2023.5.9.15.50.17/meutils/tools/
--rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/tools/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1383 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/tools/cprint.py
--rw-r--r--   0 betterme   (501) staff       (20)     2392 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/tools/machine_monitor.py
--rw-r--r--   0 betterme   (501) staff       (20)      929 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/tools/monitor.yml
--rw-r--r--   0 betterme   (501) staff       (20)     1064 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/tools/seize.py
--rw-r--r--   0 betterme   (501) staff       (20)     1255 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/tools/service_monitor.py
--rw-r--r--   0 betterme   (501) staff       (20)      429 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/tools/sys_monitor.py
--rw-r--r--   0 betterme   (501) staff       (20)      360 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/typings.py
--rw-r--r--   0 betterme   (501) staff       (20)     2438 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/meutils/zk_utils.py
--rwxr-xr-x   0 betterme   (501) staff       (20)      529 2023-04-11 09:18:47.000000 MeUtils-2023.5.9.15.50.17/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)      324 2023-04-04 15:18:39.000000 MeUtils-2023.5.9.15.50.17/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)       21 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/requirements_ai.txt
--rw-r--r--   0 betterme   (501) staff       (20)       20 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/requirements_ann.txt
--rw-r--r--   0 betterme   (501) staff       (20)       46 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/requirements_app.txt
--rw-r--r--   0 betterme   (501) staff       (20)       32 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/requirements_db.txt
--rw-r--r--   0 betterme   (501) staff       (20)        6 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/requirements_office.txt
--rw-r--r--   0 betterme   (501) staff       (20)       65 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/requirements_pd.txt
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/requirements_plot.txt
--rw-r--r--   0 betterme   (501) staff       (20)      241 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/requirements_plus.txt
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-09 07:50:17.946860 MeUtils-2023.5.9.15.50.17/scripts/
--rwxr-xr-x   0 betterme   (501) staff       (20)      251 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/scripts/demo.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      274 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/scripts/killall.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      233 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/scripts/py_sh.sh
--rw-r--r--   0 betterme   (501) staff       (20)       53 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/scripts/yum.sh
--rw-r--r--   0 betterme   (501) staff       (20)       38 2023-05-09 07:50:17.947484 MeUtils-2023.5.9.15.50.17/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     2307 2023-03-20 02:44:39.000000 MeUtils-2023.5.9.15.50.17/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.994912 MeUtils-2023.6.1.12.25.13/
+-rw-r--r--   0 betterme   (501) staff       (20)     1204 2023-05-22 06:35:12.000000 MeUtils-2023.6.1.12.25.13/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)    11357 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      249 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/MANIFEST.in
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.886467 MeUtils-2023.6.1.12.25.13/MeUtils.egg-info/
+-rw-r--r--   0 betterme   (501) staff       (20)     1894 2023-06-01 04:25:13.000000 MeUtils-2023.6.1.12.25.13/MeUtils.egg-info/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)    18041 2023-06-01 04:25:13.000000 MeUtils-2023.6.1.12.25.13/MeUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-06-01 04:25:13.000000 MeUtils-2023.6.1.12.25.13/MeUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      193 2023-06-01 04:25:13.000000 MeUtils-2023.6.1.12.25.13/MeUtils.egg-info/entry_points.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      976 2023-06-01 04:25:13.000000 MeUtils-2023.6.1.12.25.13/MeUtils.egg-info/requires.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       17 2023-06-01 04:25:13.000000 MeUtils-2023.6.1.12.25.13/MeUtils.egg-info/top_level.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1894 2023-06-01 04:25:13.994742 MeUtils-2023.6.1.12.25.13/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     1067 2023-05-04 03:00:27.000000 MeUtils-2023.6.1.12.25.13/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      684 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/clear_git_history.sh
+-rwxr-xr-x   0 betterme   (501) staff       (20)      289 2023-05-26 11:03:24.000000 MeUtils-2023.6.1.12.25.13/git_init.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.891050 MeUtils-2023.6.1.12.25.13/meutils/
+-rw-r--r--   0 betterme   (501) staff       (20)      348 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1850 2023-04-11 05:47:45.000000 MeUtils-2023.6.1.12.25.13/meutils/_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.891477 MeUtils-2023.6.1.12.25.13/meutils/ai_audio/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-17 05:51:24.000000 MeUtils-2023.6.1.12.25.13/meutils/ai_audio/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      637 2023-05-17 05:56:24.000000 MeUtils-2023.6.1.12.25.13/meutils/ai_audio/asr.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.892003 MeUtils-2023.6.1.12.25.13/meutils/ai_cv/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-18 08:11:56.000000 MeUtils-2023.6.1.12.25.13/meutils/ai_cv/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      263 2023-05-18 08:11:56.000000 MeUtils-2023.6.1.12.25.13/meutils/ai_cv/ocr.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.894481 MeUtils-2023.6.1.12.25.13/meutils/ai_nlp/
+-rw-r--r--   0 betterme   (501) staff       (20)     6921 2023-04-25 07:32:56.000000 MeUtils-2023.6.1.12.25.13/meutils/ai_nlp/SplitSentence.py
+-rw-r--r--   0 betterme   (501) staff       (20)    13489 2023-05-21 05:19:20.000000 MeUtils-2023.6.1.12.25.13/meutils/ai_nlp/Untitled-1(1).py
+-rw-r--r--   0 betterme   (501) staff       (20)      244 2023-04-25 06:23:09.000000 MeUtils-2023.6.1.12.25.13/meutils/ai_nlp/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.895202 MeUtils-2023.6.1.12.25.13/meutils/ai_nlp/_textsplitter/
+-rw-r--r--   0 betterme   (501) staff       (20)      287 2023-05-22 01:52:50.000000 MeUtils-2023.6.1.12.25.13/meutils/ai_nlp/_textsplitter/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6673 2023-05-21 05:10:54.000000 MeUtils-2023.6.1.12.25.13/meutils/ai_nlp/_textsplitter/chinese_text_splitter.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2282 2023-05-21 05:27:40.000000 MeUtils-2023.6.1.12.25.13/meutils/ai_nlp/_textsplitter/text_split.py
+-rw-r--r--   0 betterme   (501) staff       (20)   176179 2023-05-21 05:08:52.000000 MeUtils-2023.6.1.12.25.13/meutils/ai_nlp/img.png
+-rw-r--r--   0 betterme   (501) staff       (20)     2261 2023-05-19 10:20:12.000000 MeUtils-2023.6.1.12.25.13/meutils/ai_nlp/ner.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1994 2023-05-17 05:51:24.000000 MeUtils-2023.6.1.12.25.13/meutils/ai_nlp/textsplitter.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3430 2023-05-19 08:11:11.000000 MeUtils-2023.6.1.12.25.13/meutils/ai_nlp/word_segmentation.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.897891 MeUtils-2023.6.1.12.25.13/meutils/ann/
+-rw-r--r--   0 betterme   (501) staff       (20)      781 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/ann/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)     1389 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/ann/README_gensim.md
+-rw-r--r--   0 betterme   (501) staff       (20)      240 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/ann/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9161 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/ann/ann.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5662 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/ann/ann_faiss.py
+-rw-r--r--   0 betterme   (501) staff       (20)      965 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/ann/ann_gensim.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1002 2023-05-16 06:47:06.000000 MeUtils-2023.6.1.12.25.13/meutils/ann/ann_inmemory.py
+-rw-r--r--   0 betterme   (501) staff       (20)      458 2023-05-19 06:06:57.000000 MeUtils-2023.6.1.12.25.13/meutils/ann/ann_qdrant.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1171 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/ann/ann_service.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4743 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/ann/ann_v1.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1927 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/ann/cli.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.898254 MeUtils-2023.6.1.12.25.13/meutils/ann/examples/
+-rw-r--r--   0 betterme   (501) staff       (20)     1476 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/ann/examples/client.py
+-rw-r--r--   0 betterme   (501) staff       (20)      463 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/ann/examples/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)      238 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/ann/milvus.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1076 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/ann/shake_demo.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.898411 MeUtils-2023.6.1.12.25.13/meutils/asyncio_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      243 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/asyncio_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6015 2023-05-30 11:54:16.000000 MeUtils-2023.6.1.12.25.13/meutils/cache_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.899914 MeUtils-2023.6.1.12.25.13/meutils/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2828 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/clis/cli.py
+-rw-r--r--   0 betterme   (501) staff       (20)      738 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/clis/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2234 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/clis/cron.py
+-rw-r--r--   0 betterme   (501) staff       (20)      595 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/clis/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1517 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/clis/gunicorn.conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)      619 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/clis/monitor.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1018 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/clis/nesc.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.900740 MeUtils-2023.6.1.12.25.13/meutils/cmds/
+-rw-r--r--   0 betterme   (501) staff       (20)     1185 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/cmds/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      293 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/cmds/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      458 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/cmds/cmd.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1734 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/cmds/hdfs_cmd.py
+-rw-r--r--   0 betterme   (501) staff       (20)      629 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/cmds/subprocess_demo.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.901152 MeUtils-2023.6.1.12.25.13/meutils/coding/
+-rw-r--r--   0 betterme   (501) staff       (20)      244 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/coding/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      942 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/coding/find132.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8749 2023-06-01 04:25:11.000000 MeUtils-2023.6.1.12.25.13/meutils/common.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.901470 MeUtils-2023.6.1.12.25.13/meutils/comp_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      361 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/comp_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1705 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/comp_utils/reverse_metric.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.909900 MeUtils-2023.6.1.12.25.13/meutils/data/
+-rw-r--r--   0 betterme   (501) staff       (20) 10062565 2022-11-07 06:01:38.000000 MeUtils-2023.6.1.12.25.13/meutils/data/SimHei.ttf
+-rw-r--r--   0 betterme   (501) staff       (20)       19 2023-06-01 04:25:13.000000 MeUtils-2023.6.1.12.25.13/meutils/data/VERSION
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/data/_FLAG
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/data/_SUCCESS
+-rw-r--r--   0 betterme   (501) staff       (20)      243 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/data/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      600 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/data/coordinate.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2514 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/date_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.913956 MeUtils-2023.6.1.12.25.13/meutils/db/
+-rw-r--r--   0 betterme   (501) staff       (20)     1507 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/db/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)     4817 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/db/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2337 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/db/mongo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2168 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/db/neo4j.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.917071 MeUtils-2023.6.1.12.25.13/meutils/decorators/
+-rw-r--r--   0 betterme   (501) staff       (20)      238 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/decorators/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)     1681 2023-05-25 09:49:50.000000 MeUtils-2023.6.1.12.25.13/meutils/decorators/__ai.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3284 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/decorators/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1837 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/decorators/catch.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6968 2023-05-30 11:54:16.000000 MeUtils-2023.6.1.12.25.13/meutils/decorators/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)    15570 2023-04-06 06:24:58.000000 MeUtils-2023.6.1.12.25.13/meutils/decorators/decorator.py
+-rw-r--r--   0 betterme   (501) staff       (20)      754 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/decorators/decorator_demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)      527 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/decorators/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2115 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/decorators/feishu.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/decorators/retry.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1678 2023-04-04 15:22:58.000000 MeUtils-2023.6.1.12.25.13/meutils/decorators/scheduler.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3640 2023-05-15 10:32:24.000000 MeUtils-2023.6.1.12.25.13/meutils/dist_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.918712 MeUtils-2023.6.1.12.25.13/meutils/docarray_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-18 06:24:19.000000 MeUtils-2023.6.1.12.25.13/meutils/docarray_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      977 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/docarray_utils/demo_es.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1341 2023-04-26 13:37:46.000000 MeUtils-2023.6.1.12.25.13/meutils/docarray_utils/demo_hnsw.py
+-rw-r--r--   0 betterme   (501) staff       (20)      985 2023-04-27 02:39:23.000000 MeUtils-2023.6.1.12.25.13/meutils/docarray_utils/in_memory.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1058 2023-04-27 01:04:00.000000 MeUtils-2023.6.1.12.25.13/meutils/docarray_utils/改造下hnsw.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.919128 MeUtils-2023.6.1.12.25.13/meutils/easy_search/
+-rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/easy_search/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2217 2023-05-25 08:27:44.000000 MeUtils-2023.6.1.12.25.13/meutils/easy_search/es.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.920385 MeUtils-2023.6.1.12.25.13/meutils/fileparser/
+-rw-r--r--   0 betterme   (501) staff       (20)     1975 2023-05-30 05:34:49.000000 MeUtils-2023.6.1.12.25.13/meutils/fileparser/PDF抽取.py
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-05-18 08:38:53.000000 MeUtils-2023.6.1.12.25.13/meutils/fileparser/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-18 08:32:11.000000 MeUtils-2023.6.1.12.25.13/meutils/fileparser/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-05-18 08:39:22.000000 MeUtils-2023.6.1.12.25.13/meutils/fileparser/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)      263 2023-05-18 08:39:36.000000 MeUtils-2023.6.1.12.25.13/meutils/fileparser/pdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2393 2023-04-04 15:30:40.000000 MeUtils-2023.6.1.12.25.13/meutils/hash_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)      969 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/import_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.921284 MeUtils-2023.6.1.12.25.13/meutils/init/
+-rw-r--r--   0 betterme   (501) staff       (20)      242 2023-04-27 08:58:17.000000 MeUtils-2023.6.1.12.25.13/meutils/init/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1278 2023-05-29 03:58:41.000000 MeUtils-2023.6.1.12.25.13/meutils/init/evn.py
+-rw-r--r--   0 betterme   (501) staff       (20)    12882 2023-05-05 10:52:25.000000 MeUtils-2023.6.1.12.25.13/meutils/init/oo.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.923283 MeUtils-2023.6.1.12.25.13/meutils/io/
+-rw-r--r--   0 betterme   (501) staff       (20)     2107 2023-04-13 02:51:32.000000 MeUtils-2023.6.1.12.25.13/meutils/io/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      409 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/io/file.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2319 2023-05-30 01:57:16.000000 MeUtils-2023.6.1.12.25.13/meutils/io/image.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8580 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/io/tf_io.py
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/io/x.yml
+-rw-r--r--   0 betterme   (501) staff       (20)      708 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/jinja_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2512 2023-04-02 12:55:05.000000 MeUtils-2023.6.1.12.25.13/meutils/log_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.924815 MeUtils-2023.6.1.12.25.13/meutils/notice/
+-rw-r--r--   0 betterme   (501) staff       (20)      837 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/notice/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2403 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/notice/emails.py
+-rw-r--r--   0 betterme   (501) staff       (20)      703 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/notice/feishu.py
+-rw-r--r--   0 betterme   (501) staff       (20)      953 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/notice/file_post.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2229 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/notice/wechat.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3215 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/notice/wechat_.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6983 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/notice/wecom.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1102 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/notice/weekmeet.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2962 2023-05-16 06:23:15.000000 MeUtils-2023.6.1.12.25.13/meutils/np_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.927031 MeUtils-2023.6.1.12.25.13/meutils/office_automation/
+-rw-r--r--   0 betterme   (501) staff       (20)      241 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/office_automation/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      508 2023-03-27 04:08:21.000000 MeUtils-2023.6.1.12.25.13/meutils/office_automation/doc.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1538 2023-04-28 07:14:17.000000 MeUtils-2023.6.1.12.25.13/meutils/office_automation/pdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)    11894 2023-03-20 03:17:38.000000 MeUtils-2023.6.1.12.25.13/meutils/office_automation/pdm.py
+-rw-r--r--   0 betterme   (501) staff       (20)    13502 2023-03-21 06:30:39.000000 MeUtils-2023.6.1.12.25.13/meutils/office_automation/pdm_run.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.927995 MeUtils-2023.6.1.12.25.13/meutils/office_automation/report/
+-rw-r--r--   0 betterme   (501) staff       (20)      244 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/office_automation/report/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)   736444 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/office_automation/投资管理系统O3.2_交易组.pdm
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.929059 MeUtils-2023.6.1.12.25.13/meutils/other/
+-rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/other/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)    23121 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/other/besttable.py
+-rw-r--r--   0 betterme   (501) staff       (20)    44366 2023-03-21 05:16:40.000000 MeUtils-2023.6.1.12.25.13/meutils/other/crontab.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.930092 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/
+-rw-r--r--   0 betterme   (501) staff       (20)      334 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.933396 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/
+-rw-r--r--   0 betterme   (501) staff       (20)       59 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1561 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/annlite.py
+-rw-r--r--   0 betterme   (501) staff       (20)      581 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/base.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2088 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/chunk.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8448 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/document.py
+-rw-r--r--   0 betterme   (501) staff       (20)      715 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/elastic.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1736 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/match.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1111 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/memory.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1486 2023-04-21 00:49:09.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/milvus.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.937831 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/
+-rw-r--r--   0 betterme   (501) staff       (20)     2465 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5114 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/content.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.938274 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/dataloader/
+-rw-r--r--   0 betterme   (501) staff       (20)     2939 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/dataloader/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2419 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/dataloader/helper.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2966 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/delitem.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7175 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/embed.py
+-rw-r--r--   0 betterme   (501) staff       (20)      649 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/empty.py
+-rw-r--r--   0 betterme   (501) staff       (20)    21535 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/evaluation.py
+-rw-r--r--   0 betterme   (501) staff       (20)    13576 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1845 2023-04-18 09:06:43.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/getattr.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4237 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/getitem.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3803 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/group.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.939821 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/io/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/io/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)    14676 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/io/binary.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2588 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/io/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4181 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/io/csv.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1317 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/io/dataframe.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9193 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/io/from_gen.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3223 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/io/json.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1348 2023-04-18 09:06:43.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/io/pbar.py
+-rw-r--r--   0 betterme   (501) staff       (20)    10591 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/io/pushpull.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4762 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/match.py
+-rw-r--r--   0 betterme   (501) staff       (20)    15464 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/parallel.py
+-rw-r--r--   0 betterme   (501) staff       (20)    20479 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/plot.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3910 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/post.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1243 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/pydantic.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4129 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/reduce.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1612 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/sample.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8834 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/setitem.py
+-rw-r--r--   0 betterme   (501) staff       (20)      833 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/strawberry.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1086 2023-04-18 09:06:43.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/text.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9638 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/traverse.py
+-rw-r--r--   0 betterme   (501) staff       (20)      733 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/opensearch.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1806 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/qdrant.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.940734 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/queryset/
+-rw-r--r--   0 betterme   (501) staff       (20)       64 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/queryset/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8771 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/queryset/lookup.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3680 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/queryset/parser.py
+-rw-r--r--   0 betterme   (501) staff       (20)      647 2023-04-18 09:06:43.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/redis.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1232 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/sqlite.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.941048 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.942067 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/annlite/
+-rw-r--r--   0 betterme   (501) staff       (20)      473 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/annlite/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4062 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/annlite/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2078 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/annlite/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2365 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/annlite/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4541 2023-04-18 09:06:43.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/annlite/helper.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1424 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/annlite/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.943083 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/base/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/base/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3861 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/base/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)    12782 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/base/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2078 2023-04-18 09:06:43.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/base/helper.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2680 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/base/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.944076 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/elastic/
+-rw-r--r--   0 betterme   (501) staff       (20)      473 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/elastic/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9847 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/elastic/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5811 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/elastic/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4746 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/elastic/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3838 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/elastic/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.945272 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/memory/
+-rw-r--r--   0 betterme   (501) staff       (20)      437 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/memory/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2751 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/memory/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8505 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/memory/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2453 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/memory/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2046 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/memory/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.946180 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/milvus/
+-rw-r--r--   0 betterme   (501) staff       (20)      315 2023-04-18 09:06:43.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/milvus/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)    12584 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/milvus/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1897 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/milvus/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4492 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/milvus/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2772 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/milvus/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.947046 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/opensearch/
+-rw-r--r--   0 betterme   (501) staff       (20)      491 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/opensearch/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)    10803 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/opensearch/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6436 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/opensearch/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4491 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/opensearch/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3913 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/opensearch/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.948090 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/qdrant/
+-rw-r--r--   0 betterme   (501) staff       (20)     1492 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/qdrant/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9051 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/qdrant/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4457 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/qdrant/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4441 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/qdrant/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)      161 2023-04-18 09:06:43.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/qdrant/helper.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2085 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/qdrant/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.948830 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/redis/
+-rw-r--r--   0 betterme   (501) staff       (20)      313 2023-04-18 09:06:43.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/redis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7368 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/redis/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6653 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/redis/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4303 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/redis/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2662 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/redis/seqlike.py
+-rw-r--r--   0 betterme   (501) staff       (20)       88 2023-04-18 09:06:43.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/registry.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.949547 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/sqlite/
+-rw-r--r--   0 betterme   (501) staff       (20)      520 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/sqlite/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4894 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/sqlite/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2783 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/sqlite/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2279 2023-04-18 09:06:43.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/sqlite/helper.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2735 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/sqlite/seqlike.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.950479 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/weaviate/
+-rw-r--r--   0 betterme   (501) staff       (20)      479 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/weaviate/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)    14786 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/weaviate/backend.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7830 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/weaviate/find.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3285 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/weaviate/getsetdel.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2834 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/weaviate/seqlike.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1689 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/weaviate.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4806 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/base.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.951505 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/dataclasses/
+-rw-r--r--   0 betterme   (501) staff       (20)       80 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/dataclasses/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      633 2023-04-18 09:06:43.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/dataclasses/enums.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1063 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/dataclasses/getter.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2920 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/dataclasses/setter.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9205 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/dataclasses/types.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.952711 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/
+-rw-r--r--   0 betterme   (501) staff       (20)     4881 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5422 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/data.py
+-rw-r--r--   0 betterme   (501) staff       (20)    12146 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/generators.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.956974 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/mixins/
+-rw-r--r--   0 betterme   (501) staff       (20)     1779 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/mixins/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5775 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/mixins/_property.py
+-rw-r--r--   0 betterme   (501) staff       (20)      856 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/mixins/attribute.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2987 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/mixins/audio.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1988 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/mixins/blob.py
+-rw-r--r--   0 betterme   (501) staff       (20)      866 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/mixins/content.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2034 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/mixins/convert.py
+-rw-r--r--   0 betterme   (501) staff       (20)      701 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/mixins/dump.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2942 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/mixins/featurehash.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2749 2023-04-18 09:06:43.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/mixins/helper.py
+-rw-r--r--   0 betterme   (501) staff       (20)    19532 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/mixins/image.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5080 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/mixins/mesh.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8677 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/mixins/multimodal.py
+-rw-r--r--   0 betterme   (501) staff       (20)    14400 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/mixins/plot.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6281 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/mixins/porting.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2930 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/mixins/property.py
+-rw-r--r--   0 betterme   (501) staff       (20)      839 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/mixins/protobuf.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2891 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/mixins/pydantic.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1120 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/mixins/rich_embedding.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2601 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/mixins/strawberry.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6782 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/mixins/sugar.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4811 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/mixins/text.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5987 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/mixins/video.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2277 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/pydantic_model.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2691 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/strawberry_type.py
+-rw-r--r--   0 betterme   (501) staff       (20)    15985 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/helper.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.959859 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/math/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/math/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.960830 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/math/distance/
+-rw-r--r--   0 betterme   (501) staff       (20)     4465 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/math/distance/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2990 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/math/distance/numpy.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2107 2023-04-18 09:06:43.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/math/distance/paddle.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2287 2023-04-18 09:06:43.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/math/distance/tensorflow.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1950 2023-04-18 09:06:43.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/math/distance/torch.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6289 2023-04-18 09:06:43.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/math/evaluation.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3205 2023-04-18 09:06:43.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/math/helper.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9093 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/math/ndarray.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.961150 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/proto/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/proto/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      173 2023-04-18 09:06:43.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/proto/docarray_pb2.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.961515 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/proto/io/
+-rw-r--r--   0 betterme   (501) staff       (20)     3132 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/proto/io/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5231 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/proto/io/ndarray.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.961807 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/proto/pb/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/proto/pb/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4228 2023-04-18 09:06:43.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/proto/pb/docarray_pb2.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.962124 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/proto/pb2/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-18 09:06:43.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/proto/pb2/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7490 2023-04-18 09:06:43.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/proto/pb2/docarray_pb2.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.962291 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/resources/
+-rw-r--r--   0 betterme   (501) staff       (20)     4404 2023-04-18 09:06:43.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/resources/ci-vendors.json
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.962472 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/resources/embedding-projector/
+-rw-r--r--   0 betterme   (501) staff       (20)   494360 2023-04-18 09:06:43.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/resources/embedding-projector/index.html.gz
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.963312 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/score/
+-rw-r--r--   0 betterme   (501) staff       (20)      258 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/score/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      977 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/score/data.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.963898 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/score/mixins/
+-rw-r--r--   0 betterme   (501) staff       (20)      194 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/score/mixins/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1097 2023-04-18 09:06:43.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/score/mixins/property.py
+-rw-r--r--   0 betterme   (501) staff       (20)      174 2023-04-18 09:06:43.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/score/mixins/representer.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.964061 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/typing/
+-rw-r--r--   0 betterme   (501) staff       (20)     2187 2023-04-21 04:31:21.000000 MeUtils-2023.6.1.12.25.13/meutils/other/docarray/typing/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.964897 MeUtils-2023.6.1.12.25.13/meutils/pandas_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/pandas_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1228 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/pandas_utils/opt.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6300 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/pandas_utils/pd_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2846 2023-04-13 02:51:32.000000 MeUtils-2023.6.1.12.25.13/meutils/path_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6084 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/pd_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8388 2023-06-01 04:25:11.000000 MeUtils-2023.6.1.12.25.13/meutils/pipe.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.966856 MeUtils-2023.6.1.12.25.13/meutils/plot_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      241 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/plot_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      265 2023-05-09 07:50:11.000000 MeUtils-2023.6.1.12.25.13/meutils/plot_utils/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)      732 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/plot_utils/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2611 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/plot_utils/echarts.py
+-rw-r--r--   0 betterme   (501) staff       (20)    11980 2023-05-09 07:49:05.000000 MeUtils-2023.6.1.12.25.13/meutils/plot_utils/embedding_plot.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3610 2023-04-24 07:54:55.000000 MeUtils-2023.6.1.12.25.13/meutils/plot_utils/mecharts.py
+-rw-r--r--   0 betterme   (501) staff       (20)    19326 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/plot_utils/metrics.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2449 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/plot_utils/plot_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.968191 MeUtils-2023.6.1.12.25.13/meutils/request_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)     2461 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/request_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1503 2023-04-21 05:45:54.000000 MeUtils-2023.6.1.12.25.13/meutils/request_utils/crawler.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1767 2023-03-30 02:00:48.000000 MeUtils-2023.6.1.12.25.13/meutils/request_utils/download.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1334 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/request_utils/results.py
+-rw-r--r--   0 betterme   (501) staff       (20)      417 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/request_utils/wechat.py
+-rw-r--r--   0 betterme   (501) staff       (20)      644 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/request_utils/公网ip.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.968838 MeUtils-2023.6.1.12.25.13/meutils/serving/
+-rw-r--r--   0 betterme   (501) staff       (20)       22 2023-04-28 03:00:12.000000 MeUtils-2023.6.1.12.25.13/meutils/serving/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-28 02:50:45.000000 MeUtils-2023.6.1.12.25.13/meutils/serving/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2478 2023-05-11 08:02:45.000000 MeUtils-2023.6.1.12.25.13/meutils/serving/_fastapi.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.969376 MeUtils-2023.6.1.12.25.13/meutils/serving/fastapi/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.969892 MeUtils-2023.6.1.12.25.13/meutils/serving/fastapi/__demo/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-29 01:58:15.000000 MeUtils-2023.6.1.12.25.13/meutils/serving/fastapi/__demo/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1444 2023-06-01 01:17:23.000000 MeUtils-2023.6.1.12.25.13/meutils/serving/fastapi/__demo/异步任务.py
+-rw-r--r--   0 betterme   (501) staff       (20)      290 2023-05-26 07:01:26.000000 MeUtils-2023.6.1.12.25.13/meutils/serving/fastapi/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2110 2023-05-31 05:48:53.000000 MeUtils-2023.6.1.12.25.13/meutils/serving/fastapi/common.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.970504 MeUtils-2023.6.1.12.25.13/meutils/serving/fastapi/errors/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-05-25 10:51:34.000000 MeUtils-2023.6.1.12.25.13/meutils/serving/fastapi/errors/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      277 2023-05-25 10:51:34.000000 MeUtils-2023.6.1.12.25.13/meutils/serving/fastapi/errors/http_error.py
+-rw-r--r--   0 betterme   (501) staff       (20)      825 2023-05-25 10:51:34.000000 MeUtils-2023.6.1.12.25.13/meutils/serving/fastapi/errors/validation_error.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.971838 MeUtils-2023.6.1.12.25.13/meutils/serving/gui/
+-rw-r--r--   0 betterme   (501) staff       (20)       10 2023-04-18 07:29:22.000000 MeUtils-2023.6.1.12.25.13/meutils/serving/gui/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1658 2023-03-21 01:20:09.000000 MeUtils-2023.6.1.12.25.13/meutils/serving/gui/bar.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1273 2023-04-18 07:21:04.000000 MeUtils-2023.6.1.12.25.13/meutils/serving/gui/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)      210 2023-03-21 01:26:30.000000 MeUtils-2023.6.1.12.25.13/meutils/serving/gui/run.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.972230 MeUtils-2023.6.1.12.25.13/meutils/serving/jina/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.973541 MeUtils-2023.6.1.12.25.13/meutils/serving/jina/__demo/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-16 11:10:26.000000 MeUtils-2023.6.1.12.25.13/meutils/serving/jina/__demo/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      781 2023-05-16 12:04:33.000000 MeUtils-2023.6.1.12.25.13/meutils/serving/jina/__demo/client.py
+-rw-r--r--   0 betterme   (501) staff       (20)    13659 2023-05-18 02:37:48.000000 MeUtils-2023.6.1.12.25.13/meutils/serving/jina/__demo/flow.svg
+-rw-r--r--   0 betterme   (501) staff       (20)     2011 2023-05-18 02:37:46.000000 MeUtils-2023.6.1.12.25.13/meutils/serving/jina/__demo/server.py
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-16 11:10:26.000000 MeUtils-2023.6.1.12.25.13/meutils/serving/jina/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.974096 MeUtils-2023.6.1.12.25.13/meutils/serving/jina/nlp_serving/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-17 01:14:50.000000 MeUtils-2023.6.1.12.25.13/meutils/serving/jina/nlp_serving/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1078 2023-05-18 03:03:19.000000 MeUtils-2023.6.1.12.25.13/meutils/serving/jina/nlp_serving/word_segmentation.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.975544 MeUtils-2023.6.1.12.25.13/meutils/serving/st_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      290 2023-04-28 10:26:48.000000 MeUtils-2023.6.1.12.25.13/meutils/serving/st_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      826 2023-05-15 04:13:53.000000 MeUtils-2023.6.1.12.25.13/meutils/serving/st_utils/_test.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7163 2023-05-30 01:47:36.000000 MeUtils-2023.6.1.12.25.13/meutils/serving/st_utils/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)      149 2023-05-15 03:46:21.000000 MeUtils-2023.6.1.12.25.13/meutils/serving/st_utils/conf.yaml
+-rw-r--r--   0 betterme   (501) staff       (20)      218 2023-04-28 10:38:28.000000 MeUtils-2023.6.1.12.25.13/meutils/serving/st_utils/run.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.976964 MeUtils-2023.6.1.12.25.13/meutils/serving/webui/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.977554 MeUtils-2023.6.1.12.25.13/meutils/serving/webui/.streamlit/
+-rw-r--r--   0 betterme   (501) staff       (20)     7586 2023-03-24 08:27:34.000000 MeUtils-2023.6.1.12.25.13/meutils/serving/webui/.streamlit/_config.toml
+-rw-r--r--   0 betterme   (501) staff       (20)      511 2023-03-24 08:27:34.000000 MeUtils-2023.6.1.12.25.13/meutils/serving/webui/.streamlit/config.toml
+-rw-r--r--   0 betterme   (501) staff       (20)     1756 2023-05-22 09:24:56.000000 MeUtils-2023.6.1.12.25.13/meutils/serving/webui/_2_词性标注与实体识别.py
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-21 09:09:55.000000 MeUtils-2023.6.1.12.25.13/meutils/serving/webui/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      508 2023-05-22 10:05:43.000000 MeUtils-2023.6.1.12.25.13/meutils/serving/webui/_🏆_主页.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.978436 MeUtils-2023.6.1.12.25.13/meutils/serving/webui/pages/
+-rw-r--r--   0 betterme   (501) staff       (20)     1943 2023-05-22 10:51:26.000000 MeUtils-2023.6.1.12.25.13/meutils/serving/webui/pages/_1_分词.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1714 2023-05-22 10:56:06.000000 MeUtils-2023.6.1.12.25.13/meutils/serving/webui/pages/_2_词性标注与实体识别.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2424 2023-05-22 10:48:03.000000 MeUtils-2023.6.1.12.25.13/meutils/serving/webui/pages/_3_文本匹配.py
+-rwxr--r--   0 betterme   (501) staff       (20)      252 2023-05-22 10:17:52.000000 MeUtils-2023.6.1.12.25.13/meutils/serving/webui/run.sh
+-rw-r--r--   0 betterme   (501) staff       (20)      956 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/sftp.py
+-rw-r--r--   0 betterme   (501) staff       (20)      796 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/sk_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1398 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/smooth_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.978792 MeUtils-2023.6.1.12.25.13/meutils/spark/
+-rw-r--r--   0 betterme   (501) staff       (20)      576 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/spark/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.979740 MeUtils-2023.6.1.12.25.13/meutils/str_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)     1258 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/str_utils/Translator.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6655 2023-05-17 05:26:27.000000 MeUtils-2023.6.1.12.25.13/meutils/str_utils/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.980568 MeUtils-2023.6.1.12.25.13/meutils/str_utils/__translater/
+-rw-r--r--   0 betterme   (501) staff       (20)      277 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/str_utils/__translater/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1408 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/str_utils/__translater/tencent.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1238 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/str_utils/__translater/translater.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1168 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/str_utils/__translater/youdao.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1002 2023-04-07 09:07:13.000000 MeUtils-2023.6.1.12.25.13/meutils/str_utils/json_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)      926 2023-04-09 12:05:21.000000 MeUtils-2023.6.1.12.25.13/meutils/str_utils/regular_expression.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.982276 MeUtils-2023.6.1.12.25.13/meutils/templates/
+-rw-r--r--   0 betterme   (501) staff       (20)      349 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      291 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      224 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/demo.conf
+-rw-r--r--   0 betterme   (501) staff       (20)      578 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/demo.j2
+-rw-r--r--   0 betterme   (501) staff       (20)      808 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)      536 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/demox.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2416 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/df_html.j2
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.983667 MeUtils-2023.6.1.12.25.13/meutils/templates/dockerfiles/
+-rw-r--r--   0 betterme   (501) staff       (20)      112 2023-03-21 05:16:40.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/dockerfiles/Dockerfile
+-rw-r--r--   0 betterme   (501) staff       (20)      170 2023-03-21 05:16:40.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/dockerfiles/Dockerfile_me
+-rw-r--r--   0 betterme   (501) staff       (20)      217 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/dockerfiles/Dockerfile_milvus
+-rw-r--r--   0 betterme   (501) staff       (20)      245 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/dockerfiles/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      712 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/dockerfiles/docker_build_push.py
+-rwxr-xr-x   0 betterme   (501) staff       (20)      386 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/dockerfiles/docker_push.sh
+-rw-r--r--   0 betterme   (501) staff       (20)     2266 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/hegui.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.983867 MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/
+-rw-r--r--   0 betterme   (501) staff       (20)      831 2022-05-05 05:21:39.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/cookiecutter.json
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.987760 MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 betterme   (501) staff       (20)      292 2021-09-03 02:19:39.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.editorconfig
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.987982 MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.github/
+-rw-r--r--   0 betterme   (501) staff       (20)      342 2021-09-03 02:19:39.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 betterme   (501) staff       (20)     1198 2023-05-31 00:59:56.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)      842 2021-09-03 02:19:39.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.travis.yml
+-rw-r--r--   0 betterme   (501) staff       (20)      178 2021-09-03 02:19:39.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/AUTHORS.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     4010 2021-09-03 02:19:39.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/CONTRIBUTING.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      117 2021-09-03 02:19:39.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/HISTORY.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     5987 2021-09-03 02:19:39.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      351 2021-09-04 06:53:23.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/MANIFEST.in
+-rw-r--r--   0 betterme   (501) staff       (20)     2516 2021-09-03 02:19:39.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)      704 2023-04-18 10:20:21.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)     1738 2021-09-03 02:19:39.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.rst
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.990760 MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/
+-rw-r--r--   0 betterme   (501) staff       (20)      632 2021-09-03 02:19:39.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)      702 2021-09-14 08:44:31.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)       26 2022-04-18 06:25:28.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/_config.yml
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2021-09-03 02:19:39.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/authors.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)     5157 2021-09-03 02:19:39.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2021-09-03 02:19:39.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/contributing.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2021-09-03 02:19:39.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/history.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      388 2021-09-03 02:19:39.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/index.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1410 2021-09-03 02:19:39.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/installation.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      829 2021-09-03 02:19:39.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/make.bat
+-rw-r--r--   0 betterme   (501) staff       (20)       27 2021-09-03 02:19:39.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/readme.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      117 2021-09-03 02:19:39.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/usage.rst
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.990991 MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/examples/
+-rw-r--r--   0 betterme   (501) staff       (20)      234 2021-09-04 07:26:59.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/examples/demo.py
+-rwxr--r--   0 betterme   (501) staff       (20)      244 2022-05-05 05:24:52.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/git_init.sh
+-rwxr-xr-x   0 betterme   (501) staff       (20)      152 2021-09-01 08:44:34.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/pypi.sh
+-rw-r--r--   0 betterme   (501) staff       (20)        8 2021-09-03 02:19:39.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      302 2021-09-03 02:19:39.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/requirements_dev.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      549 2021-09-03 02:19:39.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     2532 2022-04-19 09:34:52.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.991338 MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/
+-rw-r--r--   0 betterme   (501) staff       (20)       61 2021-09-03 02:19:39.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2315 2021-09-03 02:32:04.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/test_{{cookiecutter.project_slug}}.py
+-rw-r--r--   0 betterme   (501) staff       (20)      678 2021-09-03 02:19:39.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tox.ini
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.991750 MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 betterme   (501) staff       (20)      273 2022-04-18 06:39:54.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.992279 MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2021-08-31 05:12:27.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2022-04-27 09:56:07.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      591 2022-04-27 09:56:07.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/cli.py
+-rw-r--r--   0 betterme   (501) staff       (20)       19 2021-09-03 02:19:39.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}.py
+-rw-r--r--   0 betterme   (501) staff       (20)    11496 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/tpl.docx
+-rw-r--r--   0 betterme   (501) staff       (20)   172819 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/templates/合规日报模板.docx
+-rw-r--r--   0 betterme   (501) staff       (20)      590 2023-05-08 05:49:55.000000 MeUtils-2023.6.1.12.25.13/meutils/todo.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.993735 MeUtils-2023.6.1.12.25.13/meutils/tools/
+-rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/tools/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1383 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/tools/cprint.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2392 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/tools/machine_monitor.py
+-rw-r--r--   0 betterme   (501) staff       (20)      929 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/tools/monitor.yml
+-rw-r--r--   0 betterme   (501) staff       (20)     1064 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/tools/seize.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1255 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/tools/service_monitor.py
+-rw-r--r--   0 betterme   (501) staff       (20)      429 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/tools/sys_monitor.py
+-rw-r--r--   0 betterme   (501) staff       (20)      360 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/typings.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2438 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/meutils/zk_utils.py
+-rwxr-xr-x   0 betterme   (501) staff       (20)      526 2023-05-15 03:11:01.000000 MeUtils-2023.6.1.12.25.13/pypi.sh
+-rw-r--r--   0 betterme   (501) staff       (20)      326 2023-05-19 04:31:42.000000 MeUtils-2023.6.1.12.25.13/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       21 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/requirements_ai.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       20 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/requirements_ann.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       46 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/requirements_app.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       32 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/requirements_db.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        8 2023-05-18 08:43:00.000000 MeUtils-2023.6.1.12.25.13/requirements_fileparser.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        6 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/requirements_office.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       65 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/requirements_pd.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/requirements_plot.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      241 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/requirements_plus.txt
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:25:13.994426 MeUtils-2023.6.1.12.25.13/scripts/
+-rwxr-xr-x   0 betterme   (501) staff       (20)      251 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/scripts/demo.sh
+-rwxr-xr-x   0 betterme   (501) staff       (20)      274 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/scripts/killall.sh
+-rwxr-xr-x   0 betterme   (501) staff       (20)      233 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/scripts/py_sh.sh
+-rw-r--r--   0 betterme   (501) staff       (20)       53 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/scripts/yum.sh
+-rw-r--r--   0 betterme   (501) staff       (20)       38 2023-06-01 04:25:13.994967 MeUtils-2023.6.1.12.25.13/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     2307 2023-03-20 02:44:39.000000 MeUtils-2023.6.1.12.25.13/setup.py
```

### Comparing `MeUtils-2023.5.9.15.50.17/LICENSE` & `MeUtils-2023.6.1.12.25.13/LICENSE`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/MeUtils.egg-info/PKG-INFO` & `MeUtils-2023.6.1.12.25.13/MeUtils.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MeUtils
-Version: 2023.5.9.15.50.17
+Version: 2023.6.1.12.25.13
 Summary: description
 Home-page: https://github.com/yuanjie-ai/MeUtils
 Author: yuanjie
 Author-email: 313303303@qq.com
 Maintainer: yuanjie
 Maintainer-email: 313303303@qq.com
 License: MIT License
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: ann
 Provides-Extra: plus
 Provides-Extra: plot
+Provides-Extra: fileparser
 Provides-Extra: ai
 Provides-Extra: app
 Provides-Extra: office
 Provides-Extra: db
 Provides-Extra: pd
 Provides-Extra: all
 License-File: LICENSE
```

### Comparing `MeUtils-2023.5.9.15.50.17/MeUtils.egg-info/requires.txt` & `MeUtils-2023.6.1.12.25.13/MeUtils.egg-info/requires.txt`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 matplotlib
 cachetools
 scikit-learn
 Pillow-PIL
 faker
 wrapt
 loguru
-fire
 typer
 kazoo
 pyyaml
 wget
 requests
 tenacity
 lxml
@@ -21,44 +20,45 @@
 schedule
 
 [ai]
 faiss-gpu
 gensim
 
 [all]
-reportlab
-gensim
+jieba
+pymongo
+fastapi[all]
+pandas-profiling[notebook]
+filetype
 streamlit
 seaborn
-simplejson
-geopy
 missingno
-redis-py-cluster
+faiss-gpu
+pretty_errors
+pyarrow
+uvicorn
 iteration_utilities
-faiss-cpu
 schedule
-pymysql
-uvicorn
+pandas_summary
+faiss-cpu
 pymilvus
-dataframe_image
-jmespath
-cachetools
-pymongo
 thefuck
-jinja2
-jieba
-fastapi[all]
-pyarrow
-pandas-profiling[notebook]
+pymysql
+cachetools
+redis-py-cluster
 pymupd
+geopy
 polars
-faiss-gpu
-pretty_errors
-pandas_summary
+reportlab
+simplejson
+jmespath
 thriftpy2
+dataframe_image
+jinja2
+gensim
 
 [ann]
 pymilvus
 faiss-cpu
 
 [app]
 fastapi[all]
@@ -67,14 +67,17 @@
 streamlit
 
 [db]
 pymysql
 pymongo
 redis-py-cluster
 
+[fileparser]
+filetype
+
 [office]
 pymupd
 
 [pd]
 dataframe_image
 pandas-profiling[notebook]
 pandas_summary
```

### Comparing `MeUtils-2023.5.9.15.50.17/PKG-INFO` & `MeUtils-2023.6.1.12.25.13/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MeUtils
-Version: 2023.5.9.15.50.17
+Version: 2023.6.1.12.25.13
 Summary: description
 Home-page: https://github.com/yuanjie-ai/MeUtils
 Author: yuanjie
 Author-email: 313303303@qq.com
 Maintainer: yuanjie
 Maintainer-email: 313303303@qq.com
 License: MIT License
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: ann
 Provides-Extra: plus
 Provides-Extra: plot
+Provides-Extra: fileparser
 Provides-Extra: ai
 Provides-Extra: app
 Provides-Extra: office
 Provides-Extra: db
 Provides-Extra: pd
 Provides-Extra: all
 License-File: LICENSE
```

### Comparing `MeUtils-2023.5.9.15.50.17/README.md` & `MeUtils-2023.6.1.12.25.13/README.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/clear_git_history.sh` & `MeUtils-2023.6.1.12.25.13/clear_git_history.sh`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/_utils.py` & `MeUtils-2023.6.1.12.25.13/meutils/_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/annzoo/README.md` & `MeUtils-2023.6.1.12.25.13/meutils/ann/README.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/annzoo/README_gensim.md` & `MeUtils-2023.6.1.12.25.13/meutils/ann/README_gensim.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/annzoo/ann.py` & `MeUtils-2023.6.1.12.25.13/meutils/ann/ann.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/annzoo/ann_faiss.py` & `MeUtils-2023.6.1.12.25.13/meutils/ann/ann_faiss.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/annzoo/ann_gensim.py` & `MeUtils-2023.6.1.12.25.13/meutils/ann/ann_gensim.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/annzoo/ann_service.py` & `MeUtils-2023.6.1.12.25.13/meutils/ann/ann_service.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/annzoo/ann_v1.py` & `MeUtils-2023.6.1.12.25.13/meutils/ann/ann_v1.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/annzoo/cli.py` & `MeUtils-2023.6.1.12.25.13/meutils/ann/cli.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/annzoo/examples/client.py` & `MeUtils-2023.6.1.12.25.13/meutils/ann/examples/client.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/annzoo/shake_demo.py` & `MeUtils-2023.6.1.12.25.13/meutils/ann/shake_demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/cache_utils.py` & `MeUtils-2023.6.1.12.25.13/meutils/cache_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,26 +17,28 @@
 MRU：Most Recently Used，与 LRU 相反，淘汰最近用的。
 
 RR：Random Replacement，就是随机替换。
 
 TTL：time-to-live 的简称，也就是说，Cache 中的每个元素都是有过期时间的，如果超过了这个时间，那这个元素就会被自动销毁。
 如果都没过期并且 Cache 已经满了的话，那就会采用 LRU 置换算法来替换掉最久不用的，以此来保证数量。
 """
+import sys
 import math
 import pickle
 import hashlib
 import numpy as np
 import pandas as pd
 import joblib
 
 from typing import Iterable
 from functools import lru_cache
 from pathlib import Path
 from joblib import Memory
 from loguru import logger
+
 from tqdm.auto import tqdm
 from cachetools import cached, cachedmethod, LRUCache, RRCache, TTLCache as _TTLCache, keys
 
 # ME
 from meutils.decorators import decorator, singleton
 from meutils.hash_utils import md5
 
@@ -191,18 +193,14 @@
                 batch = tqdm(batch, desc='miss')
             return list(map(wrap, batch))  # 递归
         return func(batch)  # 需支持单条输入
 
     return wrap(args[0])
 
 
-# todo
-"""
-缓存 docarray
-"""
 if __name__ == '__main__':
     from meutils.pipe import *
 
 
     @timer()
     @pickle_cache(location='demo')
     def func(x):
```

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/clis/cli.py` & `MeUtils-2023.6.1.12.25.13/meutils/clis/cli.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/clis/conf.py` & `MeUtils-2023.6.1.12.25.13/meutils/clis/conf.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/clis/cron.py` & `MeUtils-2023.6.1.12.25.13/meutils/clis/cron.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/clis/demo.py` & `MeUtils-2023.6.1.12.25.13/meutils/clis/demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/clis/gunicorn.conf.py` & `MeUtils-2023.6.1.12.25.13/meutils/clis/gunicorn.conf.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/clis/monitor.py` & `MeUtils-2023.6.1.12.25.13/meutils/clis/monitor.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/clis/nesc.py` & `MeUtils-2023.6.1.12.25.13/meutils/clis/nesc.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/cmds/README.md` & `MeUtils-2023.6.1.12.25.13/meutils/cmds/README.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/cmds/hdfs_cmd.py` & `MeUtils-2023.6.1.12.25.13/meutils/cmds/hdfs_cmd.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/cmds/subprocess_demo.py` & `MeUtils-2023.6.1.12.25.13/meutils/cmds/subprocess_demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/coding/find132.py` & `MeUtils-2023.6.1.12.25.13/meutils/coding/find132.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/common.py` & `MeUtils-2023.6.1.12.25.13/meutils/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,62 +11,71 @@
 import io
 import os
 import gc
 import re
 import sys
 import time
 import types
-from abc import abstractmethod
-
-import wget
+import uuid
 import zipfile
-import joblib
 import datetime
 import operator
 import inspect
 import textwrap
-import requests
 import socket
 import warnings
 import argparse
-import yaml
-import fire
-import itertools
-import subprocess
-import wrapt
 import traceback
 import multiprocessing
 import base64
-import typer
 import shutil
+import random
 import asyncio
 import importlib
-import random
-import numpy as np
-import pandas as pd
+import itertools
+import pickle
 import textwrap
+import subprocess
+
+import wget
+import yaml
+import fire
+import typer
+import joblib
+import requests
+import wrapt
 import sklearn
+import numpy as np
+import pandas as pd
+
+from typing import *
+from pathlib import Path
+from pprint import pprint
+from abc import abstractmethod
+from functools import reduce, lru_cache, partial
+from collections import Counter, OrderedDict
+from concurrent.futures import ThreadPoolExecutor, ProcessPoolExecutor
+
 import matplotlib.pyplot as plt
 from matplotlib.font_manager import FontProperties
 
 plt.rcParams['axes.unicode_minus'] = False
-from typing import *
+
 # from PIL import Image, ImageGrab
 
-from pathlib import Path
 from loguru import logger
+# logger.remove()
+# logger.add(sys.stderr,
+#            format='<green>{time:YYYY-MM-DD HH:mm:ss.SSS}</green> | <level>{level: <4}</level> - <level>{message}</level>')
+
 from tqdm.auto import tqdm
 
 tqdm.pandas()
-from functools import reduce, lru_cache, partial
-from collections import Counter, OrderedDict
-from concurrent.futures import ThreadPoolExecutor, ProcessPoolExecutor
-from pydantic import BaseModel, Field
-from pprint import pprint
 
+from pydantic import BaseModel, Field
 from faker import Faker  # https://www.cnblogs.com/aichixigua12/p/13236092.html
 
 fake_zh = Faker(locale='zh_CN')
 
 # 第三方
 from meutils.other.crontab import CronTab
 from meutils.other.besttable import Besttable
@@ -77,18 +86,18 @@
 from meutils.init.oo import O000OO0O0000OO00O
 from meutils.decorators import decorator, args, singleton, timer
 from meutils.hash_utils import murmurhash
 from meutils.path_utils import get_module_path, get_resolve_path, sys_path_append, path2list, get_config
 from meutils.cache_utils import ttl_cache, disk_cache
 
 O000OO0O0000OO00O()
-try:
-    import dill as pickle
-except ImportError:
-    import pickle
+# try:
+#     import dill as pickle
+# except ImportError:
+#     import pickle
 
 try:
     import orjson as json  # dumps 结果是字节型
 
     json.dumps = partial(json.dumps, option=json.OPT_NON_STR_KEYS)
 
 except ImportError:
@@ -102,18 +111,19 @@
     pass
 
 cli = typer.Typer(name="MeUtils CLI")
 warnings.filterwarnings("ignore")
 
 # 常量
 CPU_NUM = os.cpu_count()
-HOST_NAME = socket.getfqdn(socket.gethostname())
 FONT = FontProperties(fname=get_resolve_path('./data/SimHei.ttf', __file__))
 
 try:
+    HOST_NAME = socket.getfqdn(socket.gethostname())
+
     with socket.socket(socket.AF_INET, socket.SOCK_DGRAM) as _st:
         _st.connect(('10.255.255.255', 1))
         HOST, PORT = _st.getsockname()
         LOCAL_HOST = HOST
 except:
     LOCAL_HOST = HOST = '127.0.0.1'
     PORT = None
@@ -231,17 +241,17 @@
 
     if print_output:
         logger.info(f"CMD Output: {output}")
 
     return status, parse_fn(output)
 
 
-def is_open(ip='88.01.012.01'[::-1], port=7000, timeout=1):
+def is_open(ip='88.01.012.01'[::-1], port=7000, timeout=0.5):
     """
-        os.system(f"ping {'88.01.012.01'[::-1]} -c 1 -W 1 > IS_PRODUCT") == 0
+        互联网 is_open('baidu.com:80')
 
     @param ip:
     @param port:
     @param timeout:
     @return:
     """
     if ':' in ip:
@@ -331,14 +341,27 @@
     """
     namespace = namespace or {}
     exec(source, namespace)
     namespace.pop('__builtins__')
     return namespace  # output
 
 
+def pkl_dump(obj, file):
+    with open(file, 'wb') as f:
+        pickle.dump(obj, f)
+
+
+def pkl_load(file):
+    with open(file, 'rb') as f:
+        pickle.load(f)
+
+
+# import uuid
+# uuid.uuid4().hex
+# attrs = [attr for attr in dir(i) if not callable(getattr(i, attr)) and not attr.startswith("__")]
 if __name__ == '__main__':
     s = "import pandas as pd; output = pd.__version__"
     s = "import os; output = os.popen(cmd).read().split()"
     print(exec_callback(s, cmd='ls'))
     # with timer() as t:
     #     time.sleep(3)
     #
```

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/comp_utils/reverse_metric.py` & `MeUtils-2023.6.1.12.25.13/meutils/comp_utils/reverse_metric.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/data/SimHei.ttf` & `MeUtils-2023.6.1.12.25.13/meutils/data/SimHei.ttf`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/data/coordinate.py` & `MeUtils-2023.6.1.12.25.13/meutils/data/coordinate.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/date_utils.py` & `MeUtils-2023.6.1.12.25.13/meutils/date_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/db/README.md` & `MeUtils-2023.6.1.12.25.13/meutils/db/README.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/db/__init__.py` & `MeUtils-2023.6.1.12.25.13/meutils/db/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/db/mongo.py` & `MeUtils-2023.6.1.12.25.13/meutils/db/mongo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/db/neo4j.py` & `MeUtils-2023.6.1.12.25.13/meutils/db/neo4j.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/decorators/__init__.py` & `MeUtils-2023.6.1.12.25.13/meutils/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/decorators/ai.py` & `MeUtils-2023.6.1.12.25.13/meutils/decorators/__ai.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,17 +37,19 @@
     return wrapper
 
 
 if __name__ == '__main__':
     from tensorflow.keras.layers import Dense
     from tensorflow.keras.models import Sequential
 
+
     @compile(loss="binary_crossentropy", optimizer="adam", metrics=["accuracy"])
     def create_model():
         """from tensorflow.python.keras.models import clone_and_build_model"""
         model = Sequential()
         model.add(Dense(12, input_dim=20, kernel_initializer="uniform", activation="relu"))
         model.add(Dense(8, kernel_initializer="uniform", activation="relu"))
         model.add(Dense(1, kernel_initializer="uniform", activation="sigmoid"))
         return model
 
+
     print(create_model().summary())
```

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/decorators/catch.py` & `MeUtils-2023.6.1.12.25.13/meutils/decorators/catch.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/decorators/common.py` & `MeUtils-2023.6.1.12.25.13/meutils/decorators/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import sys
 import time
 import schedule
 import threading
 import traceback
 
 from loguru import logger
+
 from concurrent.futures import ThreadPoolExecutor, ProcessPoolExecutor
 from contextlib import contextmanager
 
 # ME
 from meutils.decorators.decorator import decorator
 
 
@@ -32,15 +33,15 @@
     :param args:
     :param kwargs:
     :return:
     """
     if int(time.time()) % bins == 0:
         import torch
         if torch.cuda.is_available():
-            with torch.cuda.device(device):
+            with torch.cuda.device(device):  # torch.cuda.current_device()
                 torch.cuda.empty_cache()
                 torch.cuda.ipc_collect()
 
         elif torch.backends.mps.is_available():
             try:
                 from torch.mps import empty_cache
                 empty_cache()
@@ -236,14 +237,22 @@
         schedule.run_pending()
 
         if stop_func():
             logger.info(f"{func.__name__} 调度终止")
             break
 
 
+def add_start_docstrings(*docstr):
+    def docstring_decorator(fn):
+        fn.__doc__ = "".join(docstr) + (fn.__doc__ if fn.__doc__ is not None else "")
+        return fn
+
+    return docstring_decorator
+
+
 if __name__ == '__main__':
     import time
 
 
     # @timeout()
     # def ff():
     #     import time
```

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/decorators/decorator.py` & `MeUtils-2023.6.1.12.25.13/meutils/decorators/decorator.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/decorators/decorator_demo.py` & `MeUtils-2023.6.1.12.25.13/meutils/decorators/decorator_demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/decorators/demo.py` & `MeUtils-2023.6.1.12.25.13/meutils/decorators/demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/decorators/feishu.py` & `MeUtils-2023.6.1.12.25.13/meutils/decorators/feishu.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/decorators/retry.py` & `MeUtils-2023.6.1.12.25.13/meutils/decorators/retry.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/decorators/scheduler.py` & `MeUtils-2023.6.1.12.25.13/meutils/decorators/scheduler.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/dist_utils.py` & `MeUtils-2023.6.1.12.25.13/meutils/dist_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 
 def jaccard(a, b):
     a, b = map(set, (a, b))
     return 1 - len(a & b) / len(a | b)
 
 
-def get_sorted_top_k(array, top_k=1, axis=-1, reverse=False):
+def get_sorted_top_k(array, top_k=1, axis=-1, reverse=False):  # 不准
     """https://blog.csdn.net/danengbinggan33/article/details/112525700
     多维数组排序
     Args:
         array: 多维数组
         top_k: 取数
         axis: 轴维度
         reverse: 是否倒序
@@ -67,18 +67,20 @@
 
 if __name__ == "__main__":
     import time
     from sklearn.metrics.pairwise import cosine_similarity
 
     x = np.random.rand(10, 128)
     y = np.random.rand(1000000, 128)
-    z = cosine_similarity(x, y)
 
     start_time = time.time()
+    z = cosine_similarity(x, y)
     sorted_index_1 = get_sorted_top_k(z, top_k=3, axis=1, reverse=True)[1]
     print(time.time() - start_time)
 
     start_time = time.time()
+    z = cosine_similarity(x, y)
     sorted_index_2 = np.flip(np.argsort(z, axis=1)[:, -3:], axis=1)
     print(time.time() - start_time)
 
     print((sorted_index_1 == sorted_index_2).all())
+    print(get_sorted_top_k(z, top_k=3, axis=1, reverse=True))
```

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/annlite.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/annlite.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/base.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/base.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/chunk.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/chunk.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/document.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/document.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/elastic.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/elastic.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/match.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/match.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/memory.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/memory.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/milvus.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/milvus.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/__init__.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/content.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/content.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/dataloader/__init__.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/dataloader/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/dataloader/helper.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/dataloader/helper.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/delitem.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/delitem.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/embed.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/embed.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/empty.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/empty.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/evaluation.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/evaluation.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/find.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/getattr.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/getattr.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/getitem.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/getitem.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/group.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/group.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/io/binary.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/io/binary.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/io/common.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/io/common.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/io/csv.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/io/csv.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/io/dataframe.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/io/dataframe.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/io/from_gen.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/io/from_gen.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/io/json.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/io/json.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/io/pbar.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/io/pbar.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/io/pushpull.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/io/pushpull.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/match.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/match.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/parallel.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/parallel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/plot.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/plot.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/post.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/post.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/pydantic.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/pydantic.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/reduce.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/reduce.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/sample.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/sample.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/setitem.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/setitem.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/strawberry.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/strawberry.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/text.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/text.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/mixins/traverse.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/mixins/traverse.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/opensearch.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/opensearch.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/qdrant.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/qdrant.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/queryset/lookup.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/queryset/lookup.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/queryset/parser.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/queryset/parser.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/redis.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/redis.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/sqlite.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/sqlite.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/annlite/backend.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/annlite/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/annlite/find.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/annlite/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/annlite/getsetdel.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/annlite/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/annlite/helper.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/annlite/helper.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/annlite/seqlike.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/annlite/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/base/backend.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/base/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/base/getsetdel.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/base/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/base/helper.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/base/helper.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/base/seqlike.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/base/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/elastic/backend.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/elastic/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/elastic/find.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/elastic/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/elastic/getsetdel.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/elastic/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/elastic/seqlike.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/elastic/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/memory/backend.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/memory/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/memory/find.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/memory/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/memory/getsetdel.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/memory/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/memory/seqlike.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/memory/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/milvus/backend.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/milvus/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/milvus/find.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/milvus/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/milvus/getsetdel.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/milvus/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/milvus/seqlike.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/milvus/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/opensearch/backend.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/opensearch/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/opensearch/find.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/opensearch/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/opensearch/getsetdel.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/opensearch/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/opensearch/seqlike.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/opensearch/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/qdrant/__init__.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/qdrant/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/qdrant/backend.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/qdrant/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/qdrant/find.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/qdrant/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/qdrant/getsetdel.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/qdrant/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/qdrant/seqlike.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/qdrant/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/redis/backend.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/redis/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/redis/find.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/redis/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/redis/getsetdel.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/redis/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/redis/seqlike.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/redis/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/sqlite/__init__.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/sqlite/backend.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/sqlite/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/sqlite/getsetdel.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/sqlite/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/sqlite/helper.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/sqlite/helper.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/sqlite/seqlike.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/sqlite/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/weaviate/backend.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/weaviate/backend.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/weaviate/find.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/weaviate/find.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/weaviate/getsetdel.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/weaviate/getsetdel.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/storage/weaviate/seqlike.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/storage/weaviate/seqlike.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/array/weaviate.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/array/weaviate.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/base.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/base.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/dataclasses/enums.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/dataclasses/enums.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/dataclasses/getter.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/dataclasses/getter.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/dataclasses/setter.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/dataclasses/setter.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/dataclasses/types.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/dataclasses/types.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/__init__.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/data.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/data.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/generators.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/generators.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/mixins/__init__.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/mixins/_property.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/mixins/_property.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/mixins/attribute.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/mixins/attribute.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/mixins/audio.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/mixins/audio.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/mixins/blob.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/mixins/blob.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/mixins/content.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/mixins/content.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/mixins/convert.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/mixins/convert.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/mixins/dump.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/mixins/dump.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/mixins/featurehash.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/mixins/featurehash.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/mixins/helper.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/mixins/helper.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/mixins/image.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/mixins/image.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/mixins/mesh.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/mixins/mesh.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/mixins/multimodal.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/mixins/multimodal.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/mixins/plot.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/mixins/plot.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/mixins/porting.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/mixins/porting.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/mixins/property.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/mixins/property.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/mixins/protobuf.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/mixins/protobuf.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/mixins/pydantic.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/mixins/pydantic.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/mixins/rich_embedding.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/mixins/rich_embedding.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/mixins/strawberry.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/mixins/strawberry.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/mixins/sugar.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/mixins/sugar.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/mixins/text.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/mixins/text.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/mixins/video.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/mixins/video.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/pydantic_model.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/pydantic_model.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/document/strawberry_type.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/document/strawberry_type.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/helper.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/helper.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/math/distance/__init__.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/math/distance/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/math/distance/numpy.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/math/distance/numpy.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/math/distance/paddle.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/math/distance/paddle.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/math/distance/tensorflow.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/math/distance/tensorflow.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/math/distance/torch.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/math/distance/torch.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/math/evaluation.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/math/evaluation.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/math/helper.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/math/helper.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/math/ndarray.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/math/ndarray.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/proto/io/__init__.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/proto/io/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/proto/io/ndarray.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/proto/io/ndarray.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/proto/pb/docarray_pb2.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/proto/pb/docarray_pb2.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/proto/pb2/docarray_pb2.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/proto/pb2/docarray_pb2.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/resources/ci-vendors.json` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/resources/ci-vendors.json`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/resources/embedding-projector/index.html.gz` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/resources/embedding-projector/index.html.gz`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/score/data.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/score/data.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/score/mixins/property.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/score/mixins/property.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_/typing/__init__.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/docarray/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_utils/demo_es.py` & `MeUtils-2023.6.1.12.25.13/meutils/docarray_utils/demo_es.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_utils/demo_hnsw.py` & `MeUtils-2023.6.1.12.25.13/meutils/docarray_utils/demo_hnsw.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_utils/in_memory.py` & `MeUtils-2023.6.1.12.25.13/meutils/docarray_utils/in_memory.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/docarray_utils/改造下hnsw.py` & `MeUtils-2023.6.1.12.25.13/meutils/docarray_utils/改造下hnsw.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/easy_search/es.py` & `MeUtils-2023.6.1.12.25.13/meutils/easy_search/es.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # @Project      : MeUtils.
 # @File         : es
 # @Time         : 2023/3/14 上午10:38
 # @Author       : yuanjie
 # @WeChat       : meutils
 # @Software     : PyCharm
 # @Description  :
-
+import pandas as pd
 from whoosh import scoring
 from whoosh.fields import *
 from whoosh.filedb.filestore import FileStorage
 
 from jieba.analyse import ChineseAnalyzer
 
 # ME
@@ -26,18 +26,18 @@
         self.storage = FileStorage(indexdir)
         self.indexname = indexname
 
         self.ix = None
         if self.storage.index_exists(indexname=indexname):
             self.ix = self.storage.open_index(indexname)
 
-    def create_index(self, df, schema, procs=4, limitmb=1024 * 2):
+    def create_index(self, df: pd.DataFrame, schema, procs=4, limitmb=1024 * 2):
         self.ix = self.storage.create_index(schema, indexname=self.indexname)
         writer = self.ix.writer(procs=procs, multisegment=True, limitmb=limitmb)
-        for fields in tqdm(df.to_dict('r'), 'Create Index'):
+        for fields in tqdm(df.to_dict(orient='records'), 'Create Index'):
             writer.add_document(**fields)
         writer.commit()
 
     def find(self, defaultfield, querystring, limit=5, weighting=scoring.BM25F, **kwargs):
         """
 
         @param defaultfield:
```

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/hash_utils.py` & `MeUtils-2023.6.1.12.25.13/meutils/hash_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/import_utils.py` & `MeUtils-2023.6.1.12.25.13/meutils/import_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/init/evn.py` & `MeUtils-2023.6.1.12.25.13/meutils/init/evn.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,29 +7,34 @@
 # @WeChat       : meutils
 # @Software     : PyCharm
 # @Description  : 
 
 import os
 
 # 环境变量配置
-os.environ['JINA_HIDE_SURVEY'] = '0'
+os.environ['JINA_HIDE_SURVEY'] = '1'
 os.environ["TOKENIZERS_PARALLELISM"] = "true"
+os.environ['OPEN_API_BASE'] = 'https://api.openai-proxy.com/v1'
 
 # LLM
-os.environ['LLM_ROLE'] = '你扮演的角色是ChatLLM灵知大语言模型，是由Betterme开发'
+os.environ['LLM_ROLE'] = '你扮演的角色是ChatLLM灵知大语言模型，是由Betterme开发。'
 os.environ['PROMPT_TEMPLATE'] = """
 {role}
-请根据以下<>中的信息简洁、专业地回答问题。
-信息：<{context}>
-问题：{question}
-如果无法从中得到答案，请回答“根据已知信息无法回答该问题”或“没有提供足够的信息”。请使用中文回答，不允许添加编造内容。
+根据以下信息，简洁、专业地回答用户的问题。如果无法得到答案，请回复：“根据已知信息无法回答该问题”或“没有提供足够的信息”。请勿编造信息，答案必须使用中文。
+已知信息：
+{context}
+问题：
+{question}
 """.strip()
+# """
+# {role}
+# 请根据以下<>中的信息简洁、专业地回答问题。
+# 信息：<{context}>
+# 问题：{question}
+# 如果无法从中得到答案，请回答“根据已知信息无法回答该问题”或“没有提供足够的信息”。请使用中文回答，不允许添加编造内容。
+# """
+
 
 if __name__ == '__main__':
     from pprint import pprint
 
     pprint(os.environ['PROMPT_TEMPLATE'])
-
-
-import baidubce
-
-import chromadb
```

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/init/oo.py` & `MeUtils-2023.6.1.12.25.13/meutils/init/oo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/io/__init__.py` & `MeUtils-2023.6.1.12.25.13/meutils/io/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/io/image.py` & `MeUtils-2023.6.1.12.25.13/meutils/io/image.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     np_arr = np.frombuffer(_bytes, dtype=np.uint8)
     # np.asarray(bytearray(bs), dtype=np.uint8)
     img = cv2.imdecode(np_arr, cv2.IMREAD_COLOR)
     return img
 
 
 def image_read(filename):
+    filename = str(filename)
     _bytes = b''
     if filename.startswith('http'):
         _bytes = requests.get(url, stream=True).content
 
     elif Path(filename).exists():
         _bytes = Path(filename).read_bytes()
```

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/io/tf_io.py` & `MeUtils-2023.6.1.12.25.13/meutils/io/tf_io.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/jinja_utils.py` & `MeUtils-2023.6.1.12.25.13/meutils/jinja_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/log_utils.py` & `MeUtils-2023.6.1.12.25.13/meutils/log_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/nlp_utils/SplitSentence.py` & `MeUtils-2023.6.1.12.25.13/meutils/ai_nlp/SplitSentence.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/nlp_utils/_textsplitter/chinese_text_splitter.py` & `MeUtils-2023.6.1.12.25.13/meutils/ai_nlp/_textsplitter/chinese_text_splitter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 import re
 
 
 class SplitSentence(object):
     """ 分句，将文本切分为若干句子，其中处理引号的部分逻辑情况较多
 
     Args:
@@ -135,8 +134,8 @@
 
 
 split_sentence = SplitSentence()
 
 if __name__ == '__main__':
     text = '央视新闻消息，近日，特朗普老友皮尔斯·摩根喊话特朗普：“美国人的生命比你的选举更重要。如果你继续以自己为中心，继续玩弄愚蠢的政治……如果你意识不到自己>的错误，你就做不对”。目前，特朗普已“取关”了这位老友。'
     res = split_sentence(text, criterion='coarse')
-    print(res)
+    print(res)
```

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/nlp_utils/_textsplitter/text_split.py` & `MeUtils-2023.6.1.12.25.13/meutils/ai_nlp/_textsplitter/text_split.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 # @Software     : PyCharm
 # @Description  : 
 
 from meutils.pipe import *
 
 
 # 分句，句子长度累加到 512 组合到一起，重叠n个句子或者size，
-def text_split(text, window_size=512, overlap_rate=0):  # 简单粗暴
+def text_split(text, window_size=512, overlap_rate=0.):  # 简单粗暴
     return str(text.strip()).lower() | xgroup(window_size, overlap_rate)
 
 
 if __name__ == '__main__':
     text = """
     姚明（Yao Ming），男，汉族，无党派人士，1980年9月12日出生于上海市徐汇区，祖籍江苏省苏州市吴江区震泽镇，前中国职业篮球运动员，司职中锋，现任亚洲篮球联合会主席、中国篮球协会主席、中职联公司董事长兼总经理， [1-3]   十三届全国青联副主席， [4]  改革先锋奖章获得者。 [5]  第十四届全国人大代表 [108]  。
 1998年4月，姚明入选王非执教的国家队，开始篮球生涯。2001夺得CBA常规赛MVP，2002年夺得CBA总冠军以及总决赛MVP，分别3次当选CBA篮板王以及盖帽王，2次当选CBA扣篮王。在2002年NBA选秀中，他以状元秀身份被NBA的休斯敦火箭队选中，2003-09年连续6个赛季（生涯共8次）入选NBA全明星赛阵容，2次入选NBA最佳阵容二阵，3次入选NBA最佳阵容三阵。2009年，姚明收购上海男篮，成为上海久事大鲨鱼俱乐部老板。2011年7月20日，姚明宣布退役。
 2013年，姚明当选为第十二届全国政协委员。2015年2月10日，姚明正式成为北京申办冬季奥林匹克运动会形象大使之一。2016年4月4日，姚明正式入选2016年奈史密斯篮球名人纪念堂，成为首位获此殊荣的中国人；10月，姚明成为中国“火星大使”；11月，当选CBA公司副董事长。 [6]
 2017年10月20日，姚明已将上海哔哩哔哩俱乐部全部股权转让。 [7]  2018年9月，荣获第十届“中华慈善奖”慈善楷模奖项。 [8]  2019年10月28日，胡润研究院发布《2019胡润80后白手起家富豪榜》，姚明以22亿元排名第48。
     """.strip()
-    # pprint(text_split(text))
-    pprint(str(text.strip()).lower())
 
-    pprint(text | xgroup(200))
+    for i in text_split(text, 200, 0.1):
+        print('='*100)
+        print(i)
```

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/nlp_utils/ner.py` & `MeUtils-2023.6.1.12.25.13/meutils/ai_nlp/ner.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,51 +11,61 @@
 from meutils.pipe import *
 from paddlenlp import Taskflow
 
 
 @lru_cache()
 class Ner(object):
 
-    def __init__(self, mode='fast', batch_size=8, entity_only=False, device=None, filter_func=None):
+    def __init__(self, mode='fast', batch_size=8, entity_only=False, device=None, filter_func=None, model=None):
         """
 
         :param mode:
             fast lac
-            accurate 解语
+            accurate wordtag 解语
         :param filter_func: lambda w2t: w2t[1].startswith(('n', 'PER')) # word2tag
         :param batch_size:
         :param entity_only:
         :param device:
+        :param model:
+        ---
+        pip install 'protobuf<4,>=3.20.2' -U
+
+
         """
         self.batch_size = max(batch_size, 2)
         self.filter_func = filter_func
 
         self.task_flow = Taskflow(
             task='ner',
+            model=model,
             mode=mode,
             device=device,
             batch_size=batch_size,
             entity_only=entity_only
         )
 
     def __call__(self, texts):
-        if isinstance(texts, str):
-            texts = [texts]
-
-        results = texts | xbar4iter(self.task_flow, self.batch_size)
+        results = texts | xbar4iter(self._task_flow, self.batch_size)
         if self.filter_func:  # 每一条都过滤
             results = results | xmap_(lambda w2ts: w2ts | xfilter_(self.filter_func))
 
-        return results if len(texts) > 1 else [results]
+        return results
 
+    def _task_flow(self, texts):
+        _ = self.task_flow(texts)
+        if isinstance(texts, str) or len(texts) == 1:
+            return [_]
+        return _
     # 名词标注 https://github.com/PaddlePaddle/PaddleNLP/blob/develop/docs/model_zoo/taskflow.md#%E8%A7%A3%E8%AF%AD%E7%9F%A5%E8%AF%86%E6%A0%87%E6%B3%A8
     # >>> from paddlenlp import Taskflow
     # >>> nptag = Taskflow("knowledge_mining", model="nptag")
     # >>> nptag("糖醋排骨")
     # [{'text': '糖醋排骨', 'label': '菜品'}]
 
 
 if __name__ == '__main__':
     # print(Ner('accurate')(['周杰伦是个音乐家'] * 10))
     filter_func = lambda w2t: w2t[1].startswith(('n', 'PER'))
-    print(Ner('fast', filter_func=filter_func)(['周杰伦是个音乐家'] * 2))  # 1 有bug
+    print(Ner('fast', filter_func=filter_func)(['周杰伦是个音乐家'] * 2))
     print(Ner('fast')('周杰伦是个音乐家'))
+    print(Ner('fast')(['周杰伦是个音乐家']))
+    print(Ner('accurate')(['周杰伦是个音乐家']))
```

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/nlp_utils/textsplitter.py` & `MeUtils-2023.6.1.12.25.13/meutils/ai_nlp/textsplitter.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # @Time         : 2023/4/25 15:33
 # @Author       : betterme
 # @WeChat       : meutils
 # @Software     : PyCharm
 # @Description  : 
 
 from meutils.pipe import *
-from meutils.nlp_utils.SplitSentence import split_sentence
+from meutils.ai_nlp.SplitSentence import split_sentence
 
 
 def merge_short_sentences(sentences, chunk_size):
     short_sentences = []
     for i, sentence in enumerate(sentences):  # 句子太长 需要再切
         short_sentences.append(sentence)
         if len(''.join(short_sentences)) > chunk_size:
```

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/nlp_utils/word_segmentation.py` & `MeUtils-2023.6.1.12.25.13/meutils/ai_nlp/word_segmentation.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 
     def __init__(self, mode='fast', user_dict=None, batch_size=32, device='cpu', filter_func=None):
         """https://github.com/PaddlePaddle/PaddleNLP/blob/develop/docs/model_zoo/taskflow.md#%E4%B8%AD%E6%96%87%E5%88%86%E8%AF%8D
 
         :param mode:
             base 实体粒度分词，在精度和速度上的权衡，基于百度LAC
             fast 最快：实现文本快速切分，基于jieba中文分词工具
-            accurate 精确模式————最准：实体粒度切分准确度最高，基于百度解语, 精确模式基于预训练模型，更适合实体粒度分词需求，适用于知识图谱构建、企业搜索Query分析等场景中
+            accurate wordtag
+            精确模式————最准：实体粒度切分准确度最高，基于百度解语, 精确模式基于预训练模型，更适合实体粒度分词需求，适用于知识图谱构建、企业搜索Query分析等场景中
 
         :param user_dict:
             在快速模式下，词典文件每一行为一个自定义item+"\t"+词频（词频可省略，词频省略则自动计算能保证分出该词的词频），暂时不支持黑名单词典（即通过设置”年“、”末“，以达到切分”年末“的目的）。
                 平原上的火焰  10
 
             在base模式和精确模式下，词典文件每一行由一个或多个自定义item组成。
                 平原上的火焰
@@ -52,22 +53,27 @@
             mode=mode,
             batch_size=batch_size,
             user_dict=user_dict,
             device=device
         )
 
     def __call__(self, texts):
-        if isinstance(texts, str):
-            texts = [texts]
-
-        results = texts | xbar4iter(self.task_flow, self.batch_size)
+        results = texts | xbar4iter(self._task_flow, self.batch_size)
 
         if self.filter_func:  # 每一条都过滤
             results = results | xmap_(lambda ws: ws | xfilter_(self.filter_func))  # 重写过滤逻辑
-        return results if len(texts) > 1 else [results]
+        return results
+
+    def _task_flow(self, texts):
+        _ = self.task_flow(texts)
+        if isinstance(texts, str) or len(texts) == 1:
+            return [_]
+        return _
 
 
 if __name__ == '__main__':
-    # print(WordSegmentation('fast', filter_func=lambda w: w not in ('的'))(['我是中国人'] * 2))  # 1 有 bug
-    print(WordSegmentation('fast')(['我是中国人'] * 2))  # 1 有 bug
-    print(WordSegmentation('fast')(['我是中国人']))  # 1 有 bug
-    print(WordSegmentation('fast')('我是中国人'))  # 1 有 bug
+    print(WordSegmentation('fast', filter_func=lambda w: w not in ('的'))('我的中国人'))
+    print(WordSegmentation('fast', filter_func=lambda w: w not in ('的'))(['我的中国人']))
+    print(WordSegmentation('fast', filter_func=lambda w: w not in ('的'))(['我的中国人'] * 2))
+    print(WordSegmentation('fast')(['我的中国人'] * 2))
+    print(WordSegmentation('fast')(['我的中国人']))
+    print(WordSegmentation('fast')('我的中国人'))
```

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/notice/__init__.py` & `MeUtils-2023.6.1.12.25.13/meutils/notice/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/notice/emails.py` & `MeUtils-2023.6.1.12.25.13/meutils/notice/emails.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/notice/feishu.py` & `MeUtils-2023.6.1.12.25.13/meutils/notice/feishu.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/notice/file_post.py` & `MeUtils-2023.6.1.12.25.13/meutils/notice/file_post.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/notice/wechat.py` & `MeUtils-2023.6.1.12.25.13/meutils/notice/wechat.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/notice/wechat_.py` & `MeUtils-2023.6.1.12.25.13/meutils/notice/wechat_.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/notice/wecom.py` & `MeUtils-2023.6.1.12.25.13/meutils/notice/wecom.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/notice/weekmeet.py` & `MeUtils-2023.6.1.12.25.13/meutils/notice/weekmeet.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/np_utils.py` & `MeUtils-2023.6.1.12.25.13/meutils/np_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -40,22 +40,24 @@
     v1 = np.array([[1, 2], [3, 4]])
     v2 = np.array([[5, 6], [7, 8], [5, 6]])
     cosine_dist(v1, v2)
     """
     assert v1.ndim == v2.ndim
     if v1.ndim == 1:
         v1, v2 = v1.reshape(1, -1), v2.reshape(1, -1)
+
+    from sklearn.metrics.pairwise import cosine_similarity
     return cosine_similarity(v1, v2).clip(0, 1)
 
 
 def cosine_topk(v1, v2, topk=10):  # 相似度不是距离
     dist = - cosine(v1, v2)
     idxs = np.argsort(dist)[:, :topk]
     scores = - np.take_along_axis(dist, idxs, -1)  # 取出得分
-    return idxs, scores
+    return idxs[0], scores[0]
 
 
 def cooccurrence_matrix(texts, window_size=2):
     """
     构建共现矩阵
     :param texts: 文本列表
     :param window_size: 单词之间的最大距离
@@ -95,18 +97,9 @@
 
 if __name__ == "__main__":
     import time
     from sklearn.metrics.pairwise import cosine_similarity
 
     x = np.random.rand(10, 128)
     y = np.random.rand(1000000, 128)
-    z = cosine_similarity(x, y)
-
-    start_time = time.time()
-    sorted_index_1 = get_sorted_top_k(z, topk=3, axis=1)[1]
-    print(time.time() - start_time)
-
-    start_time = time.time()
-    sorted_index_2 = np.flip(np.argsort(z, axis=1)[:, -3:], axis=1)
-    print(time.time() - start_time)
-
-    print((sorted_index_1 == sorted_index_2).all())
+    idxs, scores = cosine_topk(x[:1], x)
+    print(idxs[0])
```

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/office_automation/pdf.py` & `MeUtils-2023.6.1.12.25.13/meutils/office_automation/pdf.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/office_automation/pdm.py` & `MeUtils-2023.6.1.12.25.13/meutils/office_automation/pdm.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/office_automation/pdm_run.py` & `MeUtils-2023.6.1.12.25.13/meutils/office_automation/pdm_run.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/office_automation/投资管理系统O3.2_交易组.pdm` & `MeUtils-2023.6.1.12.25.13/meutils/office_automation/投资管理系统O3.2_交易组.pdm`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/other/besttable.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/besttable.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/other/crontab.py` & `MeUtils-2023.6.1.12.25.13/meutils/other/crontab.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/pandas_utils/opt.py` & `MeUtils-2023.6.1.12.25.13/meutils/pandas_utils/opt.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/pandas_utils/pd_utils.py` & `MeUtils-2023.6.1.12.25.13/meutils/pandas_utils/pd_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/path_utils.py` & `MeUtils-2023.6.1.12.25.13/meutils/path_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/pd_utils.py` & `MeUtils-2023.6.1.12.25.13/meutils/pd_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/pipe.py` & `MeUtils-2023.6.1.12.25.13/meutils/pipe.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 # itertools: https://blog.csdn.net/weixin_43193719/article/details/87536371
 xchain = Pipe(lambda iterable: itertools.chain(*iterable))
 xchain_ = Pipe(lambda iterable: list(itertools.chain(*iterable)))
 
 xenumerate = Pipe(lambda iterable, start=0: enumerate(iterable, start))
 xenumerate_ = Pipe(lambda iterable, start=0: enumerate(iterable, start))
 
-xshuffle = Pipe(lambda l: sklearn.utils.shuffle(l, random_state=None, n_samples=None))
+xshuffle = Pipe(lambda l, n_samples=None: sklearn.utils.shuffle(l, n_samples=n_samples))
 
 # dateframe dfs
 """多个df: 
 dfs = (
     Path('.').glob('demo*.txt') | xmap(lambda p: pd.read_csv(p, chunksize=2, names=['id'])) | xchain
 )
 """
@@ -87,16 +87,15 @@
 # 统计词频
 xCounter = Pipe(lambda iterable: Counter(iterable))
 
 
 @Pipe
 def xCounterUpdate(iterable, counter: Counter = None):
     """[['w1', 'w2'], ...]"""
-    if counter is None:
-        counter = Counter()
+    counter = counter or Counter()
     for i in iterable:
         counter.update(i)
     return counter
 
 
 # operator: 排序、取多个值     https://blog.csdn.net/u010339879/article/details/98304292
 # operator.itemgetter(*keys)(dic)
@@ -114,25 +113,18 @@
         yield operator.getitem(i, index)
 
 
 # np
 xstack = Pipe(lambda iterable, axis=0: np.stack(iterable, axis=axis))
 xrow_stack = Pipe(lambda iterable, axis=0: np.row_stack(iterable))
 
-# group
-xgroup = Pipe(lambda ls, step=3, overlap_rate=0: [ls[max(idx - int(step * overlap_rate), 0): idx + step] for idx in
-                                                  range(0, len(ls), step)])
-# xgroups = Pipe(lambda ls, step=3: np.array_split(ls, step))
-
 # 调试用
 xnext = Pipe(lambda ls: iter(ls).__next__())
 
 
-# todo；map filter
-
 @Pipe
 def xwrite(iterable, filename):
     with open(filename, mode='a') as f:
         for line in iterable:
             f.write(f"{line}\n")
 
 
@@ -141,23 +133,36 @@
     if keep_order:
         return list(OrderedDict.fromkeys(iterable))  # 移除列表中的重复元素(保持有序)
     else:
         return list(set(iterable))
 
 
 @Pipe
-def xbar4iter(iterable, func, batch_size=1):
+def xbar4iter(iterable: list, func, batch_size=1) -> list:
     """func 入参出参都是 list"""
     l = []
     for i in iterable | xgroup(batch_size) | xtqdm:
         l += func(i)
     return l
 
 
 @Pipe
+def xgroup(iterable, step=3, bins=None):
+    n = len(iterable)
+    if bins:
+        step = max(n // bins, 1)
+
+    _ = [iterable[idx: idx + step] for idx in range(0, n, step)]
+
+    # if len(bins) > bins:  # todo: 确保正确的bins
+
+    return _
+
+
+@Pipe
 def xsections(iterable, batch_size=3):
     def generator():
         yield from iterable
 
     g = generator()
 
     while True:
```

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/plot_utils/demo.py` & `MeUtils-2023.6.1.12.25.13/meutils/plot_utils/demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/plot_utils/echarts.py` & `MeUtils-2023.6.1.12.25.13/meutils/plot_utils/echarts.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/plot_utils/embedding_plot.py` & `MeUtils-2023.6.1.12.25.13/meutils/plot_utils/embedding_plot.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/plot_utils/mecharts.py` & `MeUtils-2023.6.1.12.25.13/meutils/plot_utils/mecharts.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/plot_utils/metrics.py` & `MeUtils-2023.6.1.12.25.13/meutils/plot_utils/metrics.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/plot_utils/plot_utils.py` & `MeUtils-2023.6.1.12.25.13/meutils/plot_utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/request_utils/__init__.py` & `MeUtils-2023.6.1.12.25.13/meutils/request_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/request_utils/crawler.py` & `MeUtils-2023.6.1.12.25.13/meutils/request_utils/crawler.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/request_utils/download.py` & `MeUtils-2023.6.1.12.25.13/meutils/request_utils/download.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/request_utils/results.py` & `MeUtils-2023.6.1.12.25.13/meutils/request_utils/results.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/request_utils/公网ip.py` & `MeUtils-2023.6.1.12.25.13/meutils/request_utils/公网ip.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/serving/_fastapi.py` & `MeUtils-2023.6.1.12.25.13/meutils/serving/_fastapi.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,43 +16,43 @@
 
 
 class App(FastAPI):
 
     def __init__(self, title: str = "Meutils API", **kwargs):
         super().__init__(title=title, **kwargs)
 
-    def run(self, app=None, host="0.0.0.0", port=8000, workers=1, access_log=True, debug=False, **kwargs):
+    def run(self, app=None, host="0.0.0.0", port=8000, workers=1, access_log=True, reload=False, app_dir=None, **kwargs):
         """
         :param app:   app字符串可开启热更新 debug/reload
         """
         import uvicorn
 
         uvicorn.config.LOGGING_CONFIG['formatters']['access']['fmt'] = f"""
               🔥 %(asctime)s - %(levelprefix)s %(client_addr)s - "%(request_line)s" %(status_code)s
               """.strip()
         uvicorn.run(
             app or self,
-            host=host, port=port, workers=workers, access_log=access_log, debug=debug, **kwargs
+            host=host, port=port, workers=workers, access_log=access_log, reload=reload, app_dir=app_dir, **kwargs
         )
 
-    def register(self, handler_func, path=None, methods=None, prefix='', **api_route_kwargs):
+    def register(self, handler_func, path=None, methods=None, prefix='', **api_route_kwargs):  # add_route注册服务
         """
 
         :param handler_func: 自定义 handler_func
         :param path:
         :param methods:
         :return:
         """
         path = path or f"{handler_func.__name__.replace('_', '-')}"
         path = (Path('/') / Path(prefix) / Path(path)).as_posix()
 
         self.handler_func = handler_func
         self.api_route(path=path, methods=methods, **api_route_kwargs)(self.handler)
 
-    async def handler(self, request: Request):
+    async def handler(self, request: Request):  # 处理一切入参
         """可重写"""
         input = request.query_params._dict
         body = await request.body()
 
         if body.startswith(b'{'):  # 主要分支 # json={}
             input.update(json_loads(body))  # json_loads
```

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/serving/gui/bar.py` & `MeUtils-2023.6.1.12.25.13/meutils/serving/gui/bar.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/serving/gui/demo.py` & `MeUtils-2023.6.1.12.25.13/meutils/serving/gui/demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/serving/st_utils/_test.py` & `MeUtils-2023.6.1.12.25.13/meutils/serving/st_utils/_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,10 +23,9 @@
     topk: int = 3
     threshold: float = 0.66
 
 
 conf = Conf()
 conf = set_config(conf)
 
-################################################################################################################
-
-st.json(conf.dict())
+if st.session_state.get('init'):
+    st.json(st.session_state)
```

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/serving/st_utils/common.py` & `MeUtils-2023.6.1.12.25.13/meutils/serving/st_utils/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,35 +5,30 @@
 # @Time         : 2022/10/18 下午1:29
 # @Author       : yuanjie
 # @WeChat       : meutils
 # @Software     : PyCharm
 # @Description  :
 
 import streamlit as st
-from meutils.pipe import *
 from streamlit.components.v1 import html
 from streamlit.elements.image import image_to_url
 
+from meutils.pipe import *
+
 
 def hide_st_style(footer_content='🔥'):
-    _ = """
-    <style>
-    #MainMenu {visibility: hidden;}
-    footer {visibility: hidden;}
-    header {visibility: hidden;}
-    </style>
-    """
     _ = f"""
         <style>.css-18e3th9 {{padding-top: 2rem;}}
         #MainMenu {{visibility: hidden;}}
         header {{visibility: hidden;}}
-        footer {{visibility: hidden;}}
-        footer:after {{content:"{footer_content}";visibility: visible;display: block;position: 'fixed';}}
+        footer {{visibility: hidden;}}        
+        footer:after {{content:"{footer_content}";visibility: visible;display: block;position: absolute;left: 50%;transform: translate(-50%, -100%);}}
         </style>
         """
+
     st.markdown(_, unsafe_allow_html=True)
 
 
 def set_footer(prefix="Made with 🔥 by ", author='Betterme', url=None):  # 链接门户、微信
     _ = f"""
     <style>
     .footer {{
@@ -50,15 +45,15 @@
         padding: 8px;
         }}
     </style>
     <div class="footer">
     <p>{prefix}<a href="{url}" target="_blank">{author}</a></p> 
     </div>
     """
-    st.markdown(_, unsafe_allow_html=True)
+    st.sidebar.markdown(_, unsafe_allow_html=True)
 
 
 # 设置文本字体
 def set_font():
     _ = f"""
     <style>
     h1,h2,h3,h4,h5,h6 {{
@@ -208,15 +203,15 @@
         color:#ff0000;
        }
     </style>
     """
     html(css)  # st.markdown
 
 
-def set_config(conf: BaseConfig, conf_path='conf.yaml'):
+def set_config(conf: BaseConfig, conf_path='conf.yaml'):  # todo: 数值改为 slider
     """
     :param conf:
     :param conf_path:
     :return:
     """
     if Path(conf_path).is_file():
         conf = conf.parse_yaml(conf_path)
@@ -229,8 +224,16 @@
 
         if form.checkbox("是否保存配置"):
             yaml.safe_dump(conf.dict(), open(conf_path, 'w'))  # 固化
 
         if form.form_submit_button('刷新配置'):
             # form.balloons()
             form.json(conf.dict())
+
+            st.session_state.init = True  # 初始化标识
+
         return conf
+
+
+def text_align(text, position='center'):
+    """中显示标题"""
+    st.markdown(f"<h1 style='text-align: {position};'>{text}</h1>", unsafe_allow_html=True)
```

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/sftp.py` & `MeUtils-2023.6.1.12.25.13/meutils/sftp.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/sk_utils.py` & `MeUtils-2023.6.1.12.25.13/meutils/sk_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/smooth_utils.py` & `MeUtils-2023.6.1.12.25.13/meutils/smooth_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/spark/__init__.py` & `MeUtils-2023.6.1.12.25.13/meutils/spark/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/str_utils/Translator.py` & `MeUtils-2023.6.1.12.25.13/meutils/str_utils/Translator.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/str_utils/__init__.py` & `MeUtils-2023.6.1.12.25.13/meutils/str_utils/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,18 +10,26 @@
 
 
 from meutils.pipe import *
 # from meutils.str_utils.translater import translater
 from meutils.request_utils.crawler import Crawler
 from urllib.parse import urlencode, parse_qs, parse_qsl, quote_plus, unquote_plus, urljoin
 
-json2query_params = lambda js: unquote_plus(urlencode(js))
 query_params2json = lambda q: dict(parse_qsl(q))
 
 
+def json2query_params(js: dict = None, url='') -> str:
+    js = js or {}
+    js = {k: v for k, v in js.items() if v}
+    query_params = unquote_plus(urlencode(js))
+    if query_params and url:
+        url = f'{url}?{query_params}'
+    return url
+
+
 def remove_punctuation(sentence: str, punctuation='!"#$%&\'()*+,-./:;<=>?@[\\]^_`{|}~'):
     dic = str.maketrans('', '', punctuation)
     return sentence.translate(dic)
 
 
 def chinese_convert(s, config='t2s'):
     """https://github.com/BYVoid/OpenCC
@@ -37,15 +45,15 @@
     hk2t.json Traditional Chinese (Hong Kong variant) to Traditional Chinese 香港繁體到繁體（OpenCC 標準）
     t2hk.json Traditional Chinese (OpenCC Standard) to Hong Kong variant 繁體（OpenCC 標準）到香港繁體
     t2jp.json Traditional Chinese Characters (Kyūjitai) to New Japanese Kanji (Shinjitai) 繁體（OpenCC 標準，舊字體）到日文新字體
     jp2t.json New Japanese Kanji (Shinjitai) to Traditional Chinese Characters (Kyūjitai) 日文新字體到繁體（OpenCC 標準，舊字體）
     tw2t.json Traditional Chinese (Taiwan standard) to Traditional Chinese 臺灣正體到繁體（OpenCC 標準）
     @return:
     """
-    import opencc
+    import opencc # pip install opencc opencc-python-reimplemented
     converter = opencc.OpenCC(config)
     return converter.convert(s)
 
 
 def sentence_cut(sentence, pattern='[，。！?\n]'):
     """'([，。！?\n])'可保留分隔符"""
     regexp = re.compile(pattern)
```

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/str_utils/__translater/tencent.py` & `MeUtils-2023.6.1.12.25.13/meutils/str_utils/__translater/tencent.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/str_utils/__translater/translater.py` & `MeUtils-2023.6.1.12.25.13/meutils/str_utils/__translater/translater.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/str_utils/__translater/youdao.py` & `MeUtils-2023.6.1.12.25.13/meutils/str_utils/__translater/youdao.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/str_utils/json_utils.py` & `MeUtils-2023.6.1.12.25.13/meutils/str_utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/str_utils/regular_expression.py` & `MeUtils-2023.6.1.12.25.13/meutils/str_utils/regular_expression.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/templates/demo.j2` & `MeUtils-2023.6.1.12.25.13/meutils/templates/demo.j2`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/templates/demo.py` & `MeUtils-2023.6.1.12.25.13/meutils/templates/demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/templates/demox.py` & `MeUtils-2023.6.1.12.25.13/meutils/templates/demox.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/templates/df_html.j2` & `MeUtils-2023.6.1.12.25.13/meutils/templates/df_html.j2`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/templates/dockerfiles/docker_build_push.py` & `MeUtils-2023.6.1.12.25.13/meutils/templates/dockerfiles/docker_build_push.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/templates/hegui.py` & `MeUtils-2023.6.1.12.25.13/meutils/templates/hegui.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/cookiecutter.json` & `MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.gitignore` & `MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -100,8 +100,7 @@
 
 # mypy
 .mypy_cache/
 
 # IDE settings
 .vscode/
 
-.github/
```

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.travis.yml` & `MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.travis.yml`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/CONTRIBUTING.rst` & `MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/LICENSE` & `MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/LICENSE`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/Makefile` & `MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/Makefile`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.md` & `MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.rst` & `MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.rst`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/Makefile` & `MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/Makefile`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/README.md` & `MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/README.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/conf.py` & `MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/conf.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/installation.rst` & `MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/make.bat` & `MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/make.bat`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.cfg` & `MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.cfg`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.py` & `MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/test_{{cookiecutter.project_slug}}.py` & `MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/test_{{cookiecutter.project_slug}}.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tox.ini` & `MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tox.ini`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/cli.py` & `MeUtils-2023.6.1.12.25.13/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/cli.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/templates/tpl.docx` & `MeUtils-2023.6.1.12.25.13/meutils/templates/tpl.docx`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/templates/合规日报模板.docx` & `MeUtils-2023.6.1.12.25.13/meutils/templates/合规日报模板.docx`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/todo.py` & `MeUtils-2023.6.1.12.25.13/meutils/todo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/tools/cprint.py` & `MeUtils-2023.6.1.12.25.13/meutils/tools/cprint.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/tools/machine_monitor.py` & `MeUtils-2023.6.1.12.25.13/meutils/tools/machine_monitor.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/tools/monitor.yml` & `MeUtils-2023.6.1.12.25.13/meutils/tools/monitor.yml`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/tools/seize.py` & `MeUtils-2023.6.1.12.25.13/meutils/tools/seize.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/tools/service_monitor.py` & `MeUtils-2023.6.1.12.25.13/meutils/tools/service_monitor.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/meutils/zk_utils.py` & `MeUtils-2023.6.1.12.25.13/meutils/zk_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2023.5.9.15.50.17/pypi.sh` & `MeUtils-2023.6.1.12.25.13/pypi.sh`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 pip install ./dist/*.whl -U
 rm -rf ./build ./dist ./*.egg* ./.eggs
 exit
 
 # twine upload -r pypi dist/*
 # twine upload -r pypitest dist/*
 
-# vim ~/.pypirc​
+# vim ~/.pypirc
 #[distutils] # this tells distutils what package indexes you can push to
 #index-servers =
 #  pypi
 #  pypitest
 #
 #[pypi]
 #repository: https://pypi.python.org/pypi
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `MeUtils-2023.5.9.15.50.17/setup.py` & `MeUtils-2023.6.1.12.25.13/setup.py`

 * *Files identical despite different names*

