# Comparing `tmp/chatllm-2023.6.1.17.16.29.tar.gz` & `tmp/chatllm-2023.6.1.17.17.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatllm-2023.6.1.17.16.29.tar", last modified: Thu Jun  1 09:16:29 2023, max compression
+gzip compressed data, was "chatllm-2023.6.1.17.17.0.tar", last modified: Thu Jun  1 09:17:01 2023, max compression
```

## Comparing `chatllm-2023.6.1.17.16.29.tar` & `chatllm-2023.6.1.17.17.0.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 09:16:29.726451 chatllm-2023.6.1.17.16.29/
--rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 chatllm-2023.6.1.17.16.29/.editorconfig
--rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 chatllm-2023.6.1.17.16.29/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 chatllm-2023.6.1.17.16.29/.travis.yml
--rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 chatllm-2023.6.1.17.16.29/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      342 2023-05-31 08:06:48.000000 chatllm-2023.6.1.17.16.29/MANIFEST.in
--rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 chatllm-2023.6.1.17.16.29/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     6665 2023-06-01 09:16:29.726266 chatllm-2023.6.1.17.16.29/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     5935 2023-05-31 01:20:56.000000 chatllm-2023.6.1.17.16.29/README.md
--rw-r--r--   0 betterme   (501) staff       (20)     5851 2023-05-29 06:46:23.000000 chatllm-2023.6.1.17.16.29/README.md.bak
--rw-r--r--   0 betterme   (501) staff       (20)      898 2023-05-31 01:32:50.000000 chatllm-2023.6.1.17.16.29/TODO.md
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 09:16:29.677487 chatllm-2023.6.1.17.16.29/chatllm/
--rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 chatllm-2023.6.1.17.16.29/chatllm/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 09:16:29.679646 chatllm-2023.6.1.17.16.29/chatllm/_his/
--rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 chatllm-2023.6.1.17.16.29/chatllm/_his/FaissANN.py
--rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-27 10:06:48.000000 chatllm-2023.6.1.17.16.29/chatllm/_his/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1812 2023-04-25 08:31:06.000000 chatllm-2023.6.1.17.16.29/chatllm/_his/_chatllm.py
--rw-r--r--   0 betterme   (501) staff       (20)     2493 2023-04-27 10:06:48.000000 chatllm-2023.6.1.17.16.29/chatllm/_his/_qa.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 09:16:29.680139 chatllm-2023.6.1.17.16.29/chatllm/aigc/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-05-29 05:16:39.000000 chatllm-2023.6.1.17.16.29/chatllm/aigc/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      834 2023-05-29 05:17:00.000000 chatllm-2023.6.1.17.16.29/chatllm/aigc/common.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 09:16:29.682591 chatllm-2023.6.1.17.16.29/chatllm/api/
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-05-29 01:42:28.000000 chatllm-2023.6.1.17.16.29/chatllm/api/TODO.md
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-28 01:04:39.000000 chatllm-2023.6.1.17.16.29/chatllm/api/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      586 2023-06-01 01:41:38.000000 chatllm-2023.6.1.17.16.29/chatllm/api/app.py
--rw-r--r--   0 betterme   (501) staff       (20)     1529 2023-05-31 03:52:51.000000 chatllm-2023.6.1.17.16.29/chatllm/api/config.py
--rw-r--r--   0 betterme   (501) staff       (20)     1010 2023-05-31 00:47:03.000000 chatllm-2023.6.1.17.16.29/chatllm/api/datamodels.py
--rw-r--r--   0 betterme   (501) staff       (20)     1749 2023-05-31 00:30:21.000000 chatllm-2023.6.1.17.16.29/chatllm/api/openai_client.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 09:16:29.684019 chatllm-2023.6.1.17.16.29/chatllm/api/routes/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-05-25 10:51:34.000000 chatllm-2023.6.1.17.16.29/chatllm/api/routes/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      557 2023-05-29 01:39:47.000000 chatllm-2023.6.1.17.16.29/chatllm/api/routes/api.py
--rw-r--r--   0 betterme   (501) staff       (20)     2094 2023-05-26 02:43:34.000000 chatllm-2023.6.1.17.16.29/chatllm/api/routes/base.py
--rw-r--r--   0 betterme   (501) staff       (20)     4696 2023-06-01 04:39:18.000000 chatllm-2023.6.1.17.16.29/chatllm/api/routes/completions.py
--rw-r--r--   0 betterme   (501) staff       (20)     1904 2023-05-26 07:01:26.000000 chatllm-2023.6.1.17.16.29/chatllm/api/routes/embeddings.py
--rw-r--r--   0 betterme   (501) staff       (20)     3471 2023-05-31 08:27:43.000000 chatllm-2023.6.1.17.16.29/chatllm/api/routes/responses.py
--rw-r--r--   0 betterme   (501) staff       (20)    11497 2023-05-25 09:59:48.000000 chatllm-2023.6.1.17.16.29/chatllm/api/sse_api.py
--rw-r--r--   0 betterme   (501) staff       (20)      845 2023-05-26 07:01:26.000000 chatllm-2023.6.1.17.16.29/chatllm/api/test.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 09:16:29.687563 chatllm-2023.6.1.17.16.29/chatllm/applications/
--rw-r--r--   0 betterme   (501) staff       (20)     3532 2023-04-25 01:19:43.000000 chatllm-2023.6.1.17.16.29/chatllm/applications/Question2Answer.py
--rw-r--r--   0 betterme   (501) staff       (20)     3937 2023-05-29 07:27:53.000000 chatllm-2023.6.1.17.16.29/chatllm/applications/__chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)      294 2023-04-25 08:32:56.000000 chatllm-2023.6.1.17.16.29/chatllm/applications/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2414 2023-05-31 06:03:52.000000 chatllm-2023.6.1.17.16.29/chatllm/applications/chatann.py
--rw-r--r--   0 betterme   (501) staff       (20)      267 2023-05-04 01:43:23.000000 chatllm-2023.6.1.17.16.29/chatllm/applications/chataudio.py
--rw-r--r--   0 betterme   (501) staff       (20)     2395 2023-05-31 09:20:39.000000 chatllm-2023.6.1.17.16.29/chatllm/applications/chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)      944 2023-05-29 04:11:25.000000 chatllm-2023.6.1.17.16.29/chatllm/applications/chatcrawler.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 chatllm-2023.6.1.17.16.29/chatllm/applications/chatdoc.py
--rw-r--r--   0 betterme   (501) staff       (20)      316 2023-05-04 03:46:23.000000 chatllm-2023.6.1.17.16.29/chatllm/applications/chatmind.py
--rw-r--r--   0 betterme   (501) staff       (20)     1350 2023-05-29 07:27:53.000000 chatllm-2023.6.1.17.16.29/chatllm/applications/chatpdf.py
--rw-r--r--   0 betterme   (501) staff       (20)      269 2023-04-26 00:59:00.000000 chatllm-2023.6.1.17.16.29/chatllm/applications/chatsearch.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 chatllm-2023.6.1.17.16.29/chatllm/applications/chatweb.py
--rw-r--r--   0 betterme   (501) staff       (20)     1875 2023-05-25 06:54:08.000000 chatllm-2023.6.1.17.16.29/chatllm/applications/chatwhoosh.py
--rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 chatllm-2023.6.1.17.16.29/chatllm/applications/pipeline.py
--rw-r--r--   0 betterme   (501) staff       (20)     1964 2023-04-27 09:24:25.000000 chatllm-2023.6.1.17.16.29/chatllm/chatyuan.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 09:16:29.688120 chatllm-2023.6.1.17.16.29/chatllm/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 chatllm-2023.6.1.17.16.29/chatllm/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 chatllm-2023.6.1.17.16.29/chatllm/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1281 2023-06-01 09:05:12.000000 chatllm-2023.6.1.17.16.29/chatllm/clis/cli.py
--rw-r--r--   0 betterme   (501) staff       (20)      779 2023-05-25 08:42:08.000000 chatllm-2023.6.1.17.16.29/chatllm/closeai.py
--rw-r--r--   0 betterme   (501) staff       (20)     1439 2023-04-27 01:39:42.000000 chatllm-2023.6.1.17.16.29/chatllm/embedding.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 09:16:29.688975 chatllm-2023.6.1.17.16.29/chatllm/llms/
--rw-r--r--   0 betterme   (501) staff       (20)     1471 2023-05-31 06:17:06.000000 chatllm-2023.6.1.17.16.29/chatllm/llms/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2198 2023-05-31 09:13:06.000000 chatllm-2023.6.1.17.16.29/chatllm/llms/chatglm.py
--rw-r--r--   0 betterme   (501) staff       (20)     1559 2023-05-22 08:19:27.000000 chatllm-2023.6.1.17.16.29/chatllm/llms/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)     2083 2023-05-22 08:39:00.000000 chatllm-2023.6.1.17.16.29/chatllm/llms/llama.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 09:16:29.690710 chatllm-2023.6.1.17.16.29/chatllm/utils/
--rw-r--r--   0 betterme   (501) staff       (20)      278 2023-04-28 04:20:30.000000 chatllm-2023.6.1.17.16.29/chatllm/utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-28 04:37:16.000000 chatllm-2023.6.1.17.16.29/chatllm/utils/_textsplitter.py
--rw-r--r--   0 betterme   (501) staff       (20)     2336 2023-05-29 07:27:53.000000 chatllm-2023.6.1.17.16.29/chatllm/utils/common.py
--rw-r--r--   0 betterme   (501) staff       (20)     2430 2023-05-19 09:28:43.000000 chatllm-2023.6.1.17.16.29/chatllm/utils/gpu_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     6342 2023-05-30 08:31:55.000000 chatllm-2023.6.1.17.16.29/chatllm/utils/nbce.py
--rw-r--r--   0 betterme   (501) staff       (20)     5208 2023-05-30 08:22:36.000000 chatllm-2023.6.1.17.16.29/chatllm/utils/nbce_test.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 09:16:29.692972 chatllm-2023.6.1.17.16.29/chatllm/webui/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 chatllm-2023.6.1.17.16.29/chatllm/webui/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1457 2023-05-29 07:27:53.000000 chatllm-2023.6.1.17.16.29/chatllm/webui/chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)     3102 2023-06-01 03:54:54.000000 chatllm-2023.6.1.17.16.29/chatllm/webui/chatpdf.py
--rw-r--r--   0 betterme   (501) staff       (20)      144 2023-05-15 11:46:17.000000 chatllm-2023.6.1.17.16.29/chatllm/webui/conf.yaml
--rw-r--r--   0 betterme   (501) staff       (20)     4311 2023-04-26 01:00:01.000000 chatllm-2023.6.1.17.16.29/chatllm/webui/gradio_ui.py
--rw-r--r--   0 betterme   (501) staff       (20)     1819 2023-04-25 03:04:12.000000 chatllm-2023.6.1.17.16.29/chatllm/webui/nice_ui.py
--rw-r--r--   0 betterme   (501) staff       (20)      220 2023-04-26 07:34:11.000000 chatllm-2023.6.1.17.16.29/chatllm/webui/run.sh
--rw-r--r--   0 betterme   (501) staff       (20)     3506 2023-05-26 07:39:23.000000 chatllm-2023.6.1.17.16.29/chatllm/webui/visualglm_st.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 09:16:29.678496 chatllm-2023.6.1.17.16.29/chatllm.egg-info/
--rw-r--r--   0 betterme   (501) staff       (20)     6665 2023-06-01 09:16:29.000000 chatllm-2023.6.1.17.16.29/chatllm.egg-info/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     2640 2023-06-01 09:16:29.000000 chatllm-2023.6.1.17.16.29/chatllm.egg-info/SOURCES.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-06-01 09:16:29.000000 chatllm-2023.6.1.17.16.29/chatllm.egg-info/dependency_links.txt
--rw-r--r--   0 betterme   (501) staff       (20)       53 2023-06-01 09:16:29.000000 chatllm-2023.6.1.17.16.29/chatllm.egg-info/entry_points.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-06-01 09:16:29.000000 chatllm-2023.6.1.17.16.29/chatllm.egg-info/not-zip-safe
--rw-r--r--   0 betterme   (501) staff       (20)      334 2023-06-01 09:16:29.000000 chatllm-2023.6.1.17.16.29/chatllm.egg-info/requires.txt
--rw-r--r--   0 betterme   (501) staff       (20)        8 2023-06-01 09:16:29.000000 chatllm-2023.6.1.17.16.29/chatllm.egg-info/top_level.txt
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 09:16:29.697507 chatllm-2023.6.1.17.16.29/data/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 09:16:29.708301 chatllm-2023.6.1.17.16.29/data/imgs/
--rw-r--r--   0 betterme   (501) staff       (20)   206137 2023-04-26 05:39:20.000000 chatllm-2023.6.1.17.16.29/data/imgs/LLM.drawio.png
--rw-r--r--   0 betterme   (501) staff       (20)   206363 2023-04-26 05:33:47.000000 chatllm-2023.6.1.17.16.29/data/imgs/LLM.png
--rw-r--r--   0 betterme   (501) staff       (20)    80933 2023-05-31 01:13:52.000000 chatllm-2023.6.1.17.16.29/data/imgs/chatbox.png
--rw-r--r--   0 betterme   (501) staff       (20)  1230065 2023-04-26 08:27:23.000000 chatllm-2023.6.1.17.16.29/data/imgs/chatpdf.gif
--rw-r--r--   0 betterme   (501) staff       (20)    45633 2023-04-26 04:24:13.000000 chatllm-2023.6.1.17.16.29/data/imgs/chatpdf_ann_df.png
--rw-r--r--   0 betterme   (501) staff       (20)   477462 2023-05-08 01:03:47.000000 chatllm-2023.6.1.17.16.29/data/imgs/img.png
--rw-r--r--   0 betterme   (501) staff       (20)   333086 2023-05-08 01:03:52.000000 chatllm-2023.6.1.17.16.29/data/imgs/img_1.png
--rw-r--r--   0 betterme   (501) staff       (20)    29400 2023-04-27 10:24:48.000000 chatllm-2023.6.1.17.16.29/data/imgs/role.png
--rw-r--r--   0 betterme   (501) staff       (20)   443539 2023-05-26 00:55:04.000000 chatllm-2023.6.1.17.16.29/data/imgs/群.png
--rw-r--r--   0 betterme   (501) staff       (20)    31192 2023-05-29 00:57:03.000000 chatllm-2023.6.1.17.16.29/data/openai_keys.md
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 09:16:29.714494 chatllm-2023.6.1.17.16.29/data/医/
--rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 chatllm-2023.6.1.17.16.29/data/医/500种中药现代研究.txt
--rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 chatllm-2023.6.1.17.16.29/data/医/古今医统大全.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 chatllm-2023.6.1.17.16.29/data/姚明.txt
--rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 chatllm-2023.6.1.17.16.29/data/王治郅.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 chatllm-2023.6.1.17.16.29/data/科比.txt
--rw-r--r--   0 betterme   (501) staff       (20)  3051914 2023-04-25 02:58:13.000000 chatllm-2023.6.1.17.16.29/data/财报.pdf
--rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 chatllm-2023.6.1.17.16.29/data/马保国.txt
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 09:16:29.724068 chatllm-2023.6.1.17.16.29/docs/
--rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 chatllm-2023.6.1.17.16.29/docs/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 chatllm-2023.6.1.17.16.29/docs/authors.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 chatllm-2023.6.1.17.16.29/docs/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 chatllm-2023.6.1.17.16.29/docs/contributing.rst
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 chatllm-2023.6.1.17.16.29/docs/history.rst
--rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 chatllm-2023.6.1.17.16.29/docs/index.rst
--rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 chatllm-2023.6.1.17.16.29/docs/make.bat
--rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 chatllm-2023.6.1.17.16.29/docs/readme.rst
--rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 chatllm-2023.6.1.17.16.29/docs/usage.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)      332 2023-05-31 10:28:33.000000 chatllm-2023.6.1.17.16.29/git_init.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 chatllm-2023.6.1.17.16.29/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)       90 2023-05-26 09:35:58.000000 chatllm-2023.6.1.17.16.29/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)       14 2023-05-19 09:53:16.000000 chatllm-2023.6.1.17.16.29/requirements_ann.txt
--rw-r--r--   0 betterme   (501) staff       (20)       30 2023-05-31 02:41:18.000000 chatllm-2023.6.1.17.16.29/requirements_api.txt
--rw-r--r--   0 betterme   (501) staff       (20)       29 2023-05-26 08:03:09.000000 chatllm-2023.6.1.17.16.29/requirements_openai.txt
--rw-r--r--   0 betterme   (501) staff       (20)       33 2023-05-29 04:24:55.000000 chatllm-2023.6.1.17.16.29/requirements_pdf.txt
--rw-r--r--   0 betterme   (501) staff       (20)       25 2023-05-29 04:24:55.000000 chatllm-2023.6.1.17.16.29/requirements_streamlit.txt
--rw-r--r--   0 betterme   (501) staff       (20)       38 2023-06-01 09:16:29.726507 chatllm-2023.6.1.17.16.29/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     1700 2023-05-31 05:17:11.000000 chatllm-2023.6.1.17.16.29/setup.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 09:16:29.724680 chatllm-2023.6.1.17.16.29/tests/
--rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 chatllm-2023.6.1.17.16.29/tests/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 chatllm-2023.6.1.17.16.29/tests/test_llm4gpt.py
--rw-r--r--   0 betterme   (501) staff       (20)    51173 2023-04-21 11:31:44.000000 chatllm-2023.6.1.17.16.29/tests/内存型.ipynb
--rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 chatllm-2023.6.1.17.16.29/tox.ini
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 09:17:01.207807 chatllm-2023.6.1.17.17.0/
+-rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 chatllm-2023.6.1.17.17.0/.editorconfig
+-rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 chatllm-2023.6.1.17.17.0/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 chatllm-2023.6.1.17.17.0/.travis.yml
+-rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 chatllm-2023.6.1.17.17.0/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      342 2023-05-31 08:06:48.000000 chatllm-2023.6.1.17.17.0/MANIFEST.in
+-rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 chatllm-2023.6.1.17.17.0/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     6664 2023-06-01 09:17:01.207632 chatllm-2023.6.1.17.17.0/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     5935 2023-05-31 01:20:56.000000 chatllm-2023.6.1.17.17.0/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)     5851 2023-05-29 06:46:23.000000 chatllm-2023.6.1.17.17.0/README.md.bak
+-rw-r--r--   0 betterme   (501) staff       (20)      898 2023-05-31 01:32:50.000000 chatllm-2023.6.1.17.17.0/TODO.md
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 09:17:01.187421 chatllm-2023.6.1.17.17.0/chatllm/
+-rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 chatllm-2023.6.1.17.17.0/chatllm/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 09:17:01.188875 chatllm-2023.6.1.17.17.0/chatllm/_his/
+-rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 chatllm-2023.6.1.17.17.0/chatllm/_his/FaissANN.py
+-rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-27 10:06:48.000000 chatllm-2023.6.1.17.17.0/chatllm/_his/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1812 2023-04-25 08:31:06.000000 chatllm-2023.6.1.17.17.0/chatllm/_his/_chatllm.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2493 2023-04-27 10:06:48.000000 chatllm-2023.6.1.17.17.0/chatllm/_his/_qa.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 09:17:01.189124 chatllm-2023.6.1.17.17.0/chatllm/aigc/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-05-29 05:16:39.000000 chatllm-2023.6.1.17.17.0/chatllm/aigc/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      834 2023-05-29 05:17:00.000000 chatllm-2023.6.1.17.17.0/chatllm/aigc/common.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 09:17:01.190133 chatllm-2023.6.1.17.17.0/chatllm/api/
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-05-29 01:42:28.000000 chatllm-2023.6.1.17.17.0/chatllm/api/TODO.md
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-28 01:04:39.000000 chatllm-2023.6.1.17.17.0/chatllm/api/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      586 2023-06-01 01:41:38.000000 chatllm-2023.6.1.17.17.0/chatllm/api/app.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1529 2023-05-31 03:52:51.000000 chatllm-2023.6.1.17.17.0/chatllm/api/config.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1010 2023-05-31 00:47:03.000000 chatllm-2023.6.1.17.17.0/chatllm/api/datamodels.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1749 2023-05-31 00:30:21.000000 chatllm-2023.6.1.17.17.0/chatllm/api/openai_client.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 09:17:01.190868 chatllm-2023.6.1.17.17.0/chatllm/api/routes/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-05-25 10:51:34.000000 chatllm-2023.6.1.17.17.0/chatllm/api/routes/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      557 2023-05-29 01:39:47.000000 chatllm-2023.6.1.17.17.0/chatllm/api/routes/api.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2094 2023-05-26 02:43:34.000000 chatllm-2023.6.1.17.17.0/chatllm/api/routes/base.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4696 2023-06-01 04:39:18.000000 chatllm-2023.6.1.17.17.0/chatllm/api/routes/completions.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1904 2023-05-26 07:01:26.000000 chatllm-2023.6.1.17.17.0/chatllm/api/routes/embeddings.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3471 2023-05-31 08:27:43.000000 chatllm-2023.6.1.17.17.0/chatllm/api/routes/responses.py
+-rw-r--r--   0 betterme   (501) staff       (20)    11497 2023-05-25 09:59:48.000000 chatllm-2023.6.1.17.17.0/chatllm/api/sse_api.py
+-rw-r--r--   0 betterme   (501) staff       (20)      845 2023-05-26 07:01:26.000000 chatllm-2023.6.1.17.17.0/chatllm/api/test.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 09:17:01.193007 chatllm-2023.6.1.17.17.0/chatllm/applications/
+-rw-r--r--   0 betterme   (501) staff       (20)     3532 2023-04-25 01:19:43.000000 chatllm-2023.6.1.17.17.0/chatllm/applications/Question2Answer.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3937 2023-05-29 07:27:53.000000 chatllm-2023.6.1.17.17.0/chatllm/applications/__chatbase.py
+-rw-r--r--   0 betterme   (501) staff       (20)      294 2023-04-25 08:32:56.000000 chatllm-2023.6.1.17.17.0/chatllm/applications/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2414 2023-05-31 06:03:52.000000 chatllm-2023.6.1.17.17.0/chatllm/applications/chatann.py
+-rw-r--r--   0 betterme   (501) staff       (20)      267 2023-05-04 01:43:23.000000 chatllm-2023.6.1.17.17.0/chatllm/applications/chataudio.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2395 2023-05-31 09:20:39.000000 chatllm-2023.6.1.17.17.0/chatllm/applications/chatbase.py
+-rw-r--r--   0 betterme   (501) staff       (20)      944 2023-05-29 04:11:25.000000 chatllm-2023.6.1.17.17.0/chatllm/applications/chatcrawler.py
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 chatllm-2023.6.1.17.17.0/chatllm/applications/chatdoc.py
+-rw-r--r--   0 betterme   (501) staff       (20)      316 2023-05-04 03:46:23.000000 chatllm-2023.6.1.17.17.0/chatllm/applications/chatmind.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1350 2023-05-29 07:27:53.000000 chatllm-2023.6.1.17.17.0/chatllm/applications/chatpdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)      269 2023-04-26 00:59:00.000000 chatllm-2023.6.1.17.17.0/chatllm/applications/chatsearch.py
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 chatllm-2023.6.1.17.17.0/chatllm/applications/chatweb.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1875 2023-05-25 06:54:08.000000 chatllm-2023.6.1.17.17.0/chatllm/applications/chatwhoosh.py
+-rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 chatllm-2023.6.1.17.17.0/chatllm/applications/pipeline.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1964 2023-04-27 09:24:25.000000 chatllm-2023.6.1.17.17.0/chatllm/chatyuan.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 09:17:01.193533 chatllm-2023.6.1.17.17.0/chatllm/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 chatllm-2023.6.1.17.17.0/chatllm/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 chatllm-2023.6.1.17.17.0/chatllm/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1281 2023-06-01 09:05:12.000000 chatllm-2023.6.1.17.17.0/chatllm/clis/cli.py
+-rw-r--r--   0 betterme   (501) staff       (20)      779 2023-05-25 08:42:08.000000 chatllm-2023.6.1.17.17.0/chatllm/closeai.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1439 2023-04-27 01:39:42.000000 chatllm-2023.6.1.17.17.0/chatllm/embedding.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 09:17:01.194070 chatllm-2023.6.1.17.17.0/chatllm/llms/
+-rw-r--r--   0 betterme   (501) staff       (20)     1471 2023-05-31 06:17:06.000000 chatllm-2023.6.1.17.17.0/chatllm/llms/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2198 2023-05-31 09:13:06.000000 chatllm-2023.6.1.17.17.0/chatllm/llms/chatglm.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1559 2023-05-22 08:19:27.000000 chatllm-2023.6.1.17.17.0/chatllm/llms/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2083 2023-05-22 08:39:00.000000 chatllm-2023.6.1.17.17.0/chatllm/llms/llama.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 09:17:01.194877 chatllm-2023.6.1.17.17.0/chatllm/utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      278 2023-04-28 04:20:30.000000 chatllm-2023.6.1.17.17.0/chatllm/utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-28 04:37:16.000000 chatllm-2023.6.1.17.17.0/chatllm/utils/_textsplitter.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2336 2023-05-29 07:27:53.000000 chatllm-2023.6.1.17.17.0/chatllm/utils/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2430 2023-05-19 09:28:43.000000 chatllm-2023.6.1.17.17.0/chatllm/utils/gpu_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6342 2023-05-30 08:31:55.000000 chatllm-2023.6.1.17.17.0/chatllm/utils/nbce.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5208 2023-05-30 08:22:36.000000 chatllm-2023.6.1.17.17.0/chatllm/utils/nbce_test.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 09:17:01.195877 chatllm-2023.6.1.17.17.0/chatllm/webui/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 chatllm-2023.6.1.17.17.0/chatllm/webui/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1457 2023-05-29 07:27:53.000000 chatllm-2023.6.1.17.17.0/chatllm/webui/chatbase.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3102 2023-06-01 03:54:54.000000 chatllm-2023.6.1.17.17.0/chatllm/webui/chatpdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)      144 2023-05-15 11:46:17.000000 chatllm-2023.6.1.17.17.0/chatllm/webui/conf.yaml
+-rw-r--r--   0 betterme   (501) staff       (20)     4311 2023-04-26 01:00:01.000000 chatllm-2023.6.1.17.17.0/chatllm/webui/gradio_ui.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1819 2023-04-25 03:04:12.000000 chatllm-2023.6.1.17.17.0/chatllm/webui/nice_ui.py
+-rw-r--r--   0 betterme   (501) staff       (20)      220 2023-04-26 07:34:11.000000 chatllm-2023.6.1.17.17.0/chatllm/webui/run.sh
+-rw-r--r--   0 betterme   (501) staff       (20)     3506 2023-05-26 07:39:23.000000 chatllm-2023.6.1.17.17.0/chatllm/webui/visualglm_st.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 09:17:01.188354 chatllm-2023.6.1.17.17.0/chatllm.egg-info/
+-rw-r--r--   0 betterme   (501) staff       (20)     6664 2023-06-01 09:17:01.000000 chatllm-2023.6.1.17.17.0/chatllm.egg-info/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     2640 2023-06-01 09:17:01.000000 chatllm-2023.6.1.17.17.0/chatllm.egg-info/SOURCES.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-06-01 09:17:01.000000 chatllm-2023.6.1.17.17.0/chatllm.egg-info/dependency_links.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       53 2023-06-01 09:17:01.000000 chatllm-2023.6.1.17.17.0/chatllm.egg-info/entry_points.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-06-01 09:17:01.000000 chatllm-2023.6.1.17.17.0/chatllm.egg-info/not-zip-safe
+-rw-r--r--   0 betterme   (501) staff       (20)      334 2023-06-01 09:17:01.000000 chatllm-2023.6.1.17.17.0/chatllm.egg-info/requires.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        8 2023-06-01 09:17:01.000000 chatllm-2023.6.1.17.17.0/chatllm.egg-info/top_level.txt
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 09:17:01.198259 chatllm-2023.6.1.17.17.0/data/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 09:17:01.200765 chatllm-2023.6.1.17.17.0/data/imgs/
+-rw-r--r--   0 betterme   (501) staff       (20)   206137 2023-04-26 05:39:20.000000 chatllm-2023.6.1.17.17.0/data/imgs/LLM.drawio.png
+-rw-r--r--   0 betterme   (501) staff       (20)   206363 2023-04-26 05:33:47.000000 chatllm-2023.6.1.17.17.0/data/imgs/LLM.png
+-rw-r--r--   0 betterme   (501) staff       (20)    80933 2023-05-31 01:13:52.000000 chatllm-2023.6.1.17.17.0/data/imgs/chatbox.png
+-rw-r--r--   0 betterme   (501) staff       (20)  1230065 2023-04-26 08:27:23.000000 chatllm-2023.6.1.17.17.0/data/imgs/chatpdf.gif
+-rw-r--r--   0 betterme   (501) staff       (20)    45633 2023-04-26 04:24:13.000000 chatllm-2023.6.1.17.17.0/data/imgs/chatpdf_ann_df.png
+-rw-r--r--   0 betterme   (501) staff       (20)   477462 2023-05-08 01:03:47.000000 chatllm-2023.6.1.17.17.0/data/imgs/img.png
+-rw-r--r--   0 betterme   (501) staff       (20)   333086 2023-05-08 01:03:52.000000 chatllm-2023.6.1.17.17.0/data/imgs/img_1.png
+-rw-r--r--   0 betterme   (501) staff       (20)    29400 2023-04-27 10:24:48.000000 chatllm-2023.6.1.17.17.0/data/imgs/role.png
+-rw-r--r--   0 betterme   (501) staff       (20)   443539 2023-05-26 00:55:04.000000 chatllm-2023.6.1.17.17.0/data/imgs/群.png
+-rw-r--r--   0 betterme   (501) staff       (20)    31192 2023-05-29 00:57:03.000000 chatllm-2023.6.1.17.17.0/data/openai_keys.md
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 09:17:01.203339 chatllm-2023.6.1.17.17.0/data/医/
+-rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 chatllm-2023.6.1.17.17.0/data/医/500种中药现代研究.txt
+-rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 chatllm-2023.6.1.17.17.0/data/医/古今医统大全.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 chatllm-2023.6.1.17.17.0/data/姚明.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 chatllm-2023.6.1.17.17.0/data/王治郅.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 chatllm-2023.6.1.17.17.0/data/科比.txt
+-rw-r--r--   0 betterme   (501) staff       (20)  3051914 2023-04-25 02:58:13.000000 chatllm-2023.6.1.17.17.0/data/财报.pdf
+-rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 chatllm-2023.6.1.17.17.0/data/马保国.txt
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 09:17:01.206958 chatllm-2023.6.1.17.17.0/docs/
+-rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 chatllm-2023.6.1.17.17.0/docs/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 chatllm-2023.6.1.17.17.0/docs/authors.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 chatllm-2023.6.1.17.17.0/docs/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 chatllm-2023.6.1.17.17.0/docs/contributing.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 chatllm-2023.6.1.17.17.0/docs/history.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 chatllm-2023.6.1.17.17.0/docs/index.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 chatllm-2023.6.1.17.17.0/docs/make.bat
+-rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 chatllm-2023.6.1.17.17.0/docs/readme.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 chatllm-2023.6.1.17.17.0/docs/usage.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)      332 2023-05-31 10:28:33.000000 chatllm-2023.6.1.17.17.0/git_init.sh
+-rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 chatllm-2023.6.1.17.17.0/pypi.sh
+-rw-r--r--   0 betterme   (501) staff       (20)       90 2023-05-26 09:35:58.000000 chatllm-2023.6.1.17.17.0/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       14 2023-05-19 09:53:16.000000 chatllm-2023.6.1.17.17.0/requirements_ann.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       30 2023-05-31 02:41:18.000000 chatllm-2023.6.1.17.17.0/requirements_api.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       29 2023-05-26 08:03:09.000000 chatllm-2023.6.1.17.17.0/requirements_openai.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2023-05-29 04:24:55.000000 chatllm-2023.6.1.17.17.0/requirements_pdf.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       25 2023-05-29 04:24:55.000000 chatllm-2023.6.1.17.17.0/requirements_streamlit.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       38 2023-06-01 09:17:01.207864 chatllm-2023.6.1.17.17.0/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     1700 2023-05-31 05:17:11.000000 chatllm-2023.6.1.17.17.0/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 09:17:01.207336 chatllm-2023.6.1.17.17.0/tests/
+-rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 chatllm-2023.6.1.17.17.0/tests/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 chatllm-2023.6.1.17.17.0/tests/test_llm4gpt.py
+-rw-r--r--   0 betterme   (501) staff       (20)    51173 2023-04-21 11:31:44.000000 chatllm-2023.6.1.17.17.0/tests/内存型.ipynb
+-rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 chatllm-2023.6.1.17.17.0/tox.ini
```

### Comparing `chatllm-2023.6.1.17.16.29/.gitignore` & `chatllm-2023.6.1.17.17.0/.gitignore`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/.travis.yml` & `chatllm-2023.6.1.17.17.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/LICENSE` & `chatllm-2023.6.1.17.17.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/Makefile` & `chatllm-2023.6.1.17.17.0/Makefile`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/PKG-INFO` & `chatllm-2023.6.1.17.17.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatllm
-Version: 2023.6.1.17.16.29
+Version: 2023.6.1.17.17.0
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/ChatLLM
 Author: yuanjie
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: chatllm
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `chatllm-2023.6.1.17.16.29/README.md` & `chatllm-2023.6.1.17.17.0/README.md`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/README.md.bak` & `chatllm-2023.6.1.17.17.0/README.md.bak`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/TODO.md` & `chatllm-2023.6.1.17.17.0/TODO.md`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/chatllm/_his/FaissANN.py` & `chatllm-2023.6.1.17.17.0/chatllm/_his/FaissANN.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/chatllm/_his/_chatllm.py` & `chatllm-2023.6.1.17.17.0/chatllm/_his/_chatllm.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/chatllm/_his/_qa.py` & `chatllm-2023.6.1.17.17.0/chatllm/_his/_qa.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/chatllm/aigc/common.py` & `chatllm-2023.6.1.17.17.0/chatllm/aigc/common.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/chatllm/api/app.py` & `chatllm-2023.6.1.17.17.0/chatllm/api/app.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/chatllm/api/config.py` & `chatllm-2023.6.1.17.17.0/chatllm/api/config.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/chatllm/api/datamodels.py` & `chatllm-2023.6.1.17.17.0/chatllm/api/datamodels.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/chatllm/api/openai_client.py` & `chatllm-2023.6.1.17.17.0/chatllm/api/openai_client.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/chatllm/api/routes/api.py` & `chatllm-2023.6.1.17.17.0/chatllm/api/routes/api.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/chatllm/api/routes/base.py` & `chatllm-2023.6.1.17.17.0/chatllm/api/routes/base.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/chatllm/api/routes/completions.py` & `chatllm-2023.6.1.17.17.0/chatllm/api/routes/completions.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/chatllm/api/routes/embeddings.py` & `chatllm-2023.6.1.17.17.0/chatllm/api/routes/embeddings.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/chatllm/api/routes/responses.py` & `chatllm-2023.6.1.17.17.0/chatllm/api/routes/responses.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/chatllm/api/sse_api.py` & `chatllm-2023.6.1.17.17.0/chatllm/api/sse_api.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/chatllm/api/test.py` & `chatllm-2023.6.1.17.17.0/chatllm/api/test.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/chatllm/applications/Question2Answer.py` & `chatllm-2023.6.1.17.17.0/chatllm/applications/Question2Answer.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/chatllm/applications/__chatbase.py` & `chatllm-2023.6.1.17.17.0/chatllm/applications/__chatbase.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/chatllm/applications/chatann.py` & `chatllm-2023.6.1.17.17.0/chatllm/applications/chatann.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/chatllm/applications/chatbase.py` & `chatllm-2023.6.1.17.17.0/chatllm/applications/chatbase.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/chatllm/applications/chatcrawler.py` & `chatllm-2023.6.1.17.17.0/chatllm/applications/chatcrawler.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/chatllm/applications/chatpdf.py` & `chatllm-2023.6.1.17.17.0/chatllm/applications/chatpdf.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/chatllm/applications/chatwhoosh.py` & `chatllm-2023.6.1.17.17.0/chatllm/applications/chatwhoosh.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/chatllm/chatyuan.py` & `chatllm-2023.6.1.17.17.0/chatllm/chatyuan.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/chatllm/clis/cli.py` & `chatllm-2023.6.1.17.17.0/chatllm/clis/cli.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/chatllm/closeai.py` & `chatllm-2023.6.1.17.17.0/chatllm/closeai.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/chatllm/embedding.py` & `chatllm-2023.6.1.17.17.0/chatllm/embedding.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/chatllm/llms/__init__.py` & `chatllm-2023.6.1.17.17.0/chatllm/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/chatllm/llms/chatglm.py` & `chatllm-2023.6.1.17.17.0/chatllm/llms/chatglm.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/chatllm/llms/demo.py` & `chatllm-2023.6.1.17.17.0/chatllm/llms/demo.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/chatllm/llms/llama.py` & `chatllm-2023.6.1.17.17.0/chatllm/llms/llama.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/chatllm/utils/common.py` & `chatllm-2023.6.1.17.17.0/chatllm/utils/common.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/chatllm/utils/gpu_utils.py` & `chatllm-2023.6.1.17.17.0/chatllm/utils/gpu_utils.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/chatllm/utils/nbce.py` & `chatllm-2023.6.1.17.17.0/chatllm/utils/nbce.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/chatllm/utils/nbce_test.py` & `chatllm-2023.6.1.17.17.0/chatllm/utils/nbce_test.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/chatllm/webui/chatbase.py` & `chatllm-2023.6.1.17.17.0/chatllm/webui/chatbase.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/chatllm/webui/chatpdf.py` & `chatllm-2023.6.1.17.17.0/chatllm/webui/chatpdf.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/chatllm/webui/gradio_ui.py` & `chatllm-2023.6.1.17.17.0/chatllm/webui/gradio_ui.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/chatllm/webui/nice_ui.py` & `chatllm-2023.6.1.17.17.0/chatllm/webui/nice_ui.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/chatllm/webui/visualglm_st.py` & `chatllm-2023.6.1.17.17.0/chatllm/webui/visualglm_st.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/chatllm.egg-info/PKG-INFO` & `chatllm-2023.6.1.17.17.0/chatllm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatllm
-Version: 2023.6.1.17.16.29
+Version: 2023.6.1.17.17.0
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/ChatLLM
 Author: yuanjie
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: chatllm
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `chatllm-2023.6.1.17.16.29/chatllm.egg-info/SOURCES.txt` & `chatllm-2023.6.1.17.17.0/chatllm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/data/imgs/LLM.drawio.png` & `chatllm-2023.6.1.17.17.0/data/imgs/LLM.drawio.png`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/data/imgs/LLM.png` & `chatllm-2023.6.1.17.17.0/data/imgs/LLM.png`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/data/imgs/chatbox.png` & `chatllm-2023.6.1.17.17.0/data/imgs/chatbox.png`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/data/imgs/chatpdf.gif` & `chatllm-2023.6.1.17.17.0/data/imgs/chatpdf.gif`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/data/imgs/chatpdf_ann_df.png` & `chatllm-2023.6.1.17.17.0/data/imgs/chatpdf_ann_df.png`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/data/imgs/img.png` & `chatllm-2023.6.1.17.17.0/data/imgs/img.png`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/data/imgs/img_1.png` & `chatllm-2023.6.1.17.17.0/data/imgs/img_1.png`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/data/imgs/role.png` & `chatllm-2023.6.1.17.17.0/data/imgs/role.png`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/data/imgs/群.png` & `chatllm-2023.6.1.17.17.0/data/imgs/群.png`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/data/openai_keys.md` & `chatllm-2023.6.1.17.17.0/data/openai_keys.md`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/data/医/500种中药现代研究.txt` & `chatllm-2023.6.1.17.17.0/data/医/500种中药现代研究.txt`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/data/医/古今医统大全.txt` & `chatllm-2023.6.1.17.17.0/data/医/古今医统大全.txt`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/data/姚明.txt` & `chatllm-2023.6.1.17.17.0/data/姚明.txt`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/data/王治郅.txt` & `chatllm-2023.6.1.17.17.0/data/王治郅.txt`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/data/科比.txt` & `chatllm-2023.6.1.17.17.0/data/科比.txt`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/data/财报.pdf` & `chatllm-2023.6.1.17.17.0/data/财报.pdf`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/docs/Makefile` & `chatllm-2023.6.1.17.17.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/docs/conf.py` & `chatllm-2023.6.1.17.17.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/docs/make.bat` & `chatllm-2023.6.1.17.17.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/setup.py` & `chatllm-2023.6.1.17.17.0/setup.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/tests/test_llm4gpt.py` & `chatllm-2023.6.1.17.17.0/tests/test_llm4gpt.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.1.17.16.29/tests/内存型.ipynb` & `chatllm-2023.6.1.17.17.0/tests/内存型.ipynb`

 * *Files identical despite different names*

