# Comparing `tmp/ChatLLM-2023.5.4.12.7.23.tar.gz` & `tmp/chatllm-2023.6.1.12.39.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ChatLLM-2023.5.4.12.7.23.tar", last modified: Thu May  4 04:07:23 2023, max compression
+gzip compressed data, was "chatllm-2023.6.1.12.39.20.tar", last modified: Thu Jun  1 04:39:20 2023, max compression
```

## Comparing `ChatLLM-2023.5.4.12.7.23.tar` & `chatllm-2023.6.1.12.39.20.tar`

### file list

```diff
@@ -1,107 +1,133 @@
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 04:07:23.682687 ChatLLM-2023.5.4.12.7.23/
--rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.12.7.23/.editorconfig
--rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 ChatLLM-2023.5.4.12.7.23/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.12.7.23/.travis.yml
--rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.12.7.23/AUTHORS.rst
--rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.12.7.23/CONTRIBUTING.rst
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 04:07:23.643042 ChatLLM-2023.5.4.12.7.23/ChatLLM.egg-info/
--rw-r--r--   0 betterme   (501) staff       (20)     5808 2023-05-04 04:07:23.000000 ChatLLM-2023.5.4.12.7.23/ChatLLM.egg-info/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     2030 2023-05-04 04:07:23.000000 ChatLLM-2023.5.4.12.7.23/ChatLLM.egg-info/SOURCES.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-05-04 04:07:23.000000 ChatLLM-2023.5.4.12.7.23/ChatLLM.egg-info/dependency_links.txt
--rw-r--r--   0 betterme   (501) staff       (20)       53 2023-05-04 04:07:23.000000 ChatLLM-2023.5.4.12.7.23/ChatLLM.egg-info/entry_points.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-05-04 04:07:23.000000 ChatLLM-2023.5.4.12.7.23/ChatLLM.egg-info/not-zip-safe
--rw-r--r--   0 betterme   (501) staff       (20)      186 2023-05-04 04:07:23.000000 ChatLLM-2023.5.4.12.7.23/ChatLLM.egg-info/requires.txt
--rw-r--r--   0 betterme   (501) staff       (20)        8 2023-05-04 04:07:23.000000 ChatLLM-2023.5.4.12.7.23/ChatLLM.egg-info/top_level.txt
--rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.12.7.23/HISTORY.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.12.7.23/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.12.7.23/MANIFEST.in
--rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.12.7.23/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     5808 2023-05-04 04:07:23.682507 ChatLLM-2023.5.4.12.7.23/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-26 04:55:25.000000 ChatLLM-2023.5.4.12.7.23/README.bak.md
--rw-r--r--   0 betterme   (501) staff       (20)     4907 2023-04-28 07:55:35.000000 ChatLLM-2023.5.4.12.7.23/README.md
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 04:07:23.643805 ChatLLM-2023.5.4.12.7.23/chatllm/
--rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.12.7.23/chatllm/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 04:07:23.645074 ChatLLM-2023.5.4.12.7.23/chatllm/_his/
--rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 ChatLLM-2023.5.4.12.7.23/chatllm/_his/FaissANN.py
--rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-27 10:06:48.000000 ChatLLM-2023.5.4.12.7.23/chatllm/_his/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1812 2023-04-25 08:31:06.000000 ChatLLM-2023.5.4.12.7.23/chatllm/_his/_chatllm.py
--rw-r--r--   0 betterme   (501) staff       (20)     2493 2023-04-27 10:06:48.000000 ChatLLM-2023.5.4.12.7.23/chatllm/_his/_qa.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 04:07:23.645553 ChatLLM-2023.5.4.12.7.23/chatllm/api/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-28 01:04:39.000000 ChatLLM-2023.5.4.12.7.23/chatllm/api/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1827 2023-04-28 02:36:43.000000 ChatLLM-2023.5.4.12.7.23/chatllm/api/stream_api.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 04:07:23.649080 ChatLLM-2023.5.4.12.7.23/chatllm/applications/
--rw-r--r--   0 betterme   (501) staff       (20)     3532 2023-04-25 01:19:43.000000 ChatLLM-2023.5.4.12.7.23/chatllm/applications/Question2Answer.py
--rw-r--r--   0 betterme   (501) staff       (20)      294 2023-04-25 08:32:56.000000 ChatLLM-2023.5.4.12.7.23/chatllm/applications/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2805 2023-04-27 04:33:02.000000 ChatLLM-2023.5.4.12.7.23/chatllm/applications/chatann.py
--rw-r--r--   0 betterme   (501) staff       (20)      267 2023-05-04 01:43:23.000000 ChatLLM-2023.5.4.12.7.23/chatllm/applications/chataudio.py
--rw-r--r--   0 betterme   (501) staff       (20)     3587 2023-05-04 04:06:22.000000 ChatLLM-2023.5.4.12.7.23/chatllm/applications/chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)      949 2023-05-04 04:05:16.000000 ChatLLM-2023.5.4.12.7.23/chatllm/applications/chatcrawler.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.5.4.12.7.23/chatllm/applications/chatdoc.py
--rw-r--r--   0 betterme   (501) staff       (20)      316 2023-05-04 03:46:23.000000 ChatLLM-2023.5.4.12.7.23/chatllm/applications/chatmind.py
--rw-r--r--   0 betterme   (501) staff       (20)     1357 2023-04-28 07:16:03.000000 ChatLLM-2023.5.4.12.7.23/chatllm/applications/chatpdf.py
--rw-r--r--   0 betterme   (501) staff       (20)      269 2023-04-26 00:59:00.000000 ChatLLM-2023.5.4.12.7.23/chatllm/applications/chatsearch.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.5.4.12.7.23/chatllm/applications/chatweb.py
--rw-r--r--   0 betterme   (501) staff       (20)     1895 2023-04-27 02:58:56.000000 ChatLLM-2023.5.4.12.7.23/chatllm/applications/chatwhoosh.py
--rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 ChatLLM-2023.5.4.12.7.23/chatllm/applications/pipeline.py
--rw-r--r--   0 betterme   (501) staff       (20)     1964 2023-04-27 09:24:25.000000 ChatLLM-2023.5.4.12.7.23/chatllm/chatyuan.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 04:07:23.649745 ChatLLM-2023.5.4.12.7.23/chatllm/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.12.7.23/chatllm/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.12.7.23/chatllm/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1334 2023-04-28 07:03:35.000000 ChatLLM-2023.5.4.12.7.23/chatllm/clis/cli.py
--rw-r--r--   0 betterme   (501) staff       (20)     1439 2023-04-27 01:39:42.000000 ChatLLM-2023.5.4.12.7.23/chatllm/embedding.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 04:07:23.650233 ChatLLM-2023.5.4.12.7.23/chatllm/parse_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      302 2023-04-25 01:22:30.000000 ChatLLM-2023.5.4.12.7.23/chatllm/parse_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      273 2023-04-21 04:20:09.000000 ChatLLM-2023.5.4.12.7.23/chatllm/parse_utils/doc_parse.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 04:07:23.651054 ChatLLM-2023.5.4.12.7.23/chatllm/utils/
--rw-r--r--   0 betterme   (501) staff       (20)      278 2023-04-28 04:20:30.000000 ChatLLM-2023.5.4.12.7.23/chatllm/utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-28 04:37:16.000000 ChatLLM-2023.5.4.12.7.23/chatllm/utils/_textsplitter.py
--rw-r--r--   0 betterme   (501) staff       (20)     2218 2023-05-04 02:54:09.000000 ChatLLM-2023.5.4.12.7.23/chatllm/utils/common.py
--rw-r--r--   0 betterme   (501) staff       (20)     3208 2023-04-28 04:38:58.000000 ChatLLM-2023.5.4.12.7.23/chatllm/utils/gpu_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 04:07:23.652988 ChatLLM-2023.5.4.12.7.23/chatllm/webui/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 ChatLLM-2023.5.4.12.7.23/chatllm/webui/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1488 2023-04-26 01:00:01.000000 ChatLLM-2023.5.4.12.7.23/chatllm/webui/chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)     3017 2023-04-28 06:43:45.000000 ChatLLM-2023.5.4.12.7.23/chatllm/webui/chatpdf.py
--rw-r--r--   0 betterme   (501) staff       (20)     4311 2023-04-26 01:00:01.000000 ChatLLM-2023.5.4.12.7.23/chatllm/webui/gradio_ui.py
--rw-r--r--   0 betterme   (501) staff       (20)     1819 2023-04-25 03:04:12.000000 ChatLLM-2023.5.4.12.7.23/chatllm/webui/nice_ui.py
--rw-r--r--   0 betterme   (501) staff       (20)      220 2023-04-26 07:34:11.000000 ChatLLM-2023.5.4.12.7.23/chatllm/webui/run.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 04:07:23.656758 ChatLLM-2023.5.4.12.7.23/data/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 04:07:23.664233 ChatLLM-2023.5.4.12.7.23/data/imgs/
--rw-r--r--   0 betterme   (501) staff       (20)   206137 2023-04-26 05:39:20.000000 ChatLLM-2023.5.4.12.7.23/data/imgs/LLM.drawio.png
--rw-r--r--   0 betterme   (501) staff       (20)   206363 2023-04-26 05:33:47.000000 ChatLLM-2023.5.4.12.7.23/data/imgs/LLM.png
--rw-r--r--   0 betterme   (501) staff       (20)  1230065 2023-04-26 08:27:23.000000 ChatLLM-2023.5.4.12.7.23/data/imgs/chatpdf.gif
--rw-r--r--   0 betterme   (501) staff       (20)    45633 2023-04-26 04:24:13.000000 ChatLLM-2023.5.4.12.7.23/data/imgs/chatpdf_ann_df.png
--rw-r--r--   0 betterme   (501) staff       (20)    29400 2023-04-27 10:24:48.000000 ChatLLM-2023.5.4.12.7.23/data/imgs/role.png
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 04:07:23.668202 ChatLLM-2023.5.4.12.7.23/data/医/
--rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 ChatLLM-2023.5.4.12.7.23/data/医/500种中药现代研究.txt
--rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 ChatLLM-2023.5.4.12.7.23/data/医/古今医统大全.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 ChatLLM-2023.5.4.12.7.23/data/姚明.txt
--rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 ChatLLM-2023.5.4.12.7.23/data/王治郅.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 ChatLLM-2023.5.4.12.7.23/data/科比.txt
--rw-r--r--   0 betterme   (501) staff       (20)  3051914 2023-04-25 02:58:13.000000 ChatLLM-2023.5.4.12.7.23/data/财报.pdf
--rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 ChatLLM-2023.5.4.12.7.23/data/马保国.txt
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 04:07:23.681286 ChatLLM-2023.5.4.12.7.23/docs/
--rw-r--r--   0 betterme   (501) staff       (20)      564 2023-04-26 04:55:25.000000 ChatLLM-2023.5.4.12.7.23/docs/INSTALL.md
--rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.12.7.23/docs/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     4846 2023-04-27 11:05:23.000000 ChatLLM-2023.5.4.12.7.23/docs/README.md
--rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.12.7.23/docs/_config.yml
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.12.7.23/docs/authors.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.12.7.23/docs/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.12.7.23/docs/contributing.rst
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.12.7.23/docs/history.rst
--rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.12.7.23/docs/index.rst
--rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.12.7.23/docs/make.bat
--rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.12.7.23/docs/readme.rst
--rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.12.7.23/docs/usage.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)      269 2023-04-28 07:55:35.000000 ChatLLM-2023.5.4.12.7.23/git_init.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.12.7.23/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)       78 2023-04-28 08:43:50.000000 ChatLLM-2023.5.4.12.7.23/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)       14 2023-04-28 08:44:21.000000 ChatLLM-2023.5.4.12.7.23/requirements_api.txt
--rw-r--r--   0 betterme   (501) staff       (20)       25 2023-04-28 08:44:53.000000 ChatLLM-2023.5.4.12.7.23/requirements_pdf.txt
--rw-r--r--   0 betterme   (501) staff       (20)       10 2023-04-28 08:44:32.000000 ChatLLM-2023.5.4.12.7.23/requirements_streamlit.txt
--rw-r--r--   0 betterme   (501) staff       (20)       38 2023-05-04 04:07:23.682736 ChatLLM-2023.5.4.12.7.23/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     1897 2023-04-28 08:42:35.000000 ChatLLM-2023.5.4.12.7.23/setup.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 04:07:23.681735 ChatLLM-2023.5.4.12.7.23/tests/
--rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.12.7.23/tests/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.12.7.23/tests/test_llm4gpt.py
--rw-r--r--   0 betterme   (501) staff       (20)    51173 2023-04-21 11:31:44.000000 ChatLLM-2023.5.4.12.7.23/tests/内存型.ipynb
--rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.12.7.23/tox.ini
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:39:20.835052 chatllm-2023.6.1.12.39.20/
+-rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 chatllm-2023.6.1.12.39.20/.editorconfig
+-rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 chatllm-2023.6.1.12.39.20/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 chatllm-2023.6.1.12.39.20/.travis.yml
+-rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 chatllm-2023.6.1.12.39.20/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      342 2023-05-31 08:06:48.000000 chatllm-2023.6.1.12.39.20/MANIFEST.in
+-rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 chatllm-2023.6.1.12.39.20/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     6665 2023-06-01 04:39:20.834869 chatllm-2023.6.1.12.39.20/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     5935 2023-05-31 01:20:56.000000 chatllm-2023.6.1.12.39.20/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)     5851 2023-05-29 06:46:23.000000 chatllm-2023.6.1.12.39.20/README.md.bak
+-rw-r--r--   0 betterme   (501) staff       (20)      898 2023-05-31 01:32:50.000000 chatllm-2023.6.1.12.39.20/TODO.md
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:39:20.788515 chatllm-2023.6.1.12.39.20/chatllm/
+-rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 chatllm-2023.6.1.12.39.20/chatllm/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:39:20.790560 chatllm-2023.6.1.12.39.20/chatllm/_his/
+-rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 chatllm-2023.6.1.12.39.20/chatllm/_his/FaissANN.py
+-rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-27 10:06:48.000000 chatllm-2023.6.1.12.39.20/chatllm/_his/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1812 2023-04-25 08:31:06.000000 chatllm-2023.6.1.12.39.20/chatllm/_his/_chatllm.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2493 2023-04-27 10:06:48.000000 chatllm-2023.6.1.12.39.20/chatllm/_his/_qa.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:39:20.790974 chatllm-2023.6.1.12.39.20/chatllm/aigc/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-05-29 05:16:39.000000 chatllm-2023.6.1.12.39.20/chatllm/aigc/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      834 2023-05-29 05:17:00.000000 chatllm-2023.6.1.12.39.20/chatllm/aigc/common.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:39:20.793246 chatllm-2023.6.1.12.39.20/chatllm/api/
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-05-29 01:42:28.000000 chatllm-2023.6.1.12.39.20/chatllm/api/TODO.md
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-28 01:04:39.000000 chatllm-2023.6.1.12.39.20/chatllm/api/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      586 2023-06-01 01:41:38.000000 chatllm-2023.6.1.12.39.20/chatllm/api/app.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1529 2023-05-31 03:52:51.000000 chatllm-2023.6.1.12.39.20/chatllm/api/config.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1010 2023-05-31 00:47:03.000000 chatllm-2023.6.1.12.39.20/chatllm/api/datamodels.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1749 2023-05-31 00:30:21.000000 chatllm-2023.6.1.12.39.20/chatllm/api/openai_client.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:39:20.794371 chatllm-2023.6.1.12.39.20/chatllm/api/routes/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-05-25 10:51:34.000000 chatllm-2023.6.1.12.39.20/chatllm/api/routes/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      557 2023-05-29 01:39:47.000000 chatllm-2023.6.1.12.39.20/chatllm/api/routes/api.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2094 2023-05-26 02:43:34.000000 chatllm-2023.6.1.12.39.20/chatllm/api/routes/base.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4696 2023-06-01 04:39:18.000000 chatllm-2023.6.1.12.39.20/chatllm/api/routes/completions.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1904 2023-05-26 07:01:26.000000 chatllm-2023.6.1.12.39.20/chatllm/api/routes/embeddings.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3471 2023-05-31 08:27:43.000000 chatllm-2023.6.1.12.39.20/chatllm/api/routes/responses.py
+-rw-r--r--   0 betterme   (501) staff       (20)    11497 2023-05-25 09:59:48.000000 chatllm-2023.6.1.12.39.20/chatllm/api/sse_api.py
+-rw-r--r--   0 betterme   (501) staff       (20)      845 2023-05-26 07:01:26.000000 chatllm-2023.6.1.12.39.20/chatllm/api/test.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:39:20.797773 chatllm-2023.6.1.12.39.20/chatllm/applications/
+-rw-r--r--   0 betterme   (501) staff       (20)     3532 2023-04-25 01:19:43.000000 chatllm-2023.6.1.12.39.20/chatllm/applications/Question2Answer.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3937 2023-05-29 07:27:53.000000 chatllm-2023.6.1.12.39.20/chatllm/applications/__chatbase.py
+-rw-r--r--   0 betterme   (501) staff       (20)      294 2023-04-25 08:32:56.000000 chatllm-2023.6.1.12.39.20/chatllm/applications/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2414 2023-05-31 06:03:52.000000 chatllm-2023.6.1.12.39.20/chatllm/applications/chatann.py
+-rw-r--r--   0 betterme   (501) staff       (20)      267 2023-05-04 01:43:23.000000 chatllm-2023.6.1.12.39.20/chatllm/applications/chataudio.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2395 2023-05-31 09:20:39.000000 chatllm-2023.6.1.12.39.20/chatllm/applications/chatbase.py
+-rw-r--r--   0 betterme   (501) staff       (20)      944 2023-05-29 04:11:25.000000 chatllm-2023.6.1.12.39.20/chatllm/applications/chatcrawler.py
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 chatllm-2023.6.1.12.39.20/chatllm/applications/chatdoc.py
+-rw-r--r--   0 betterme   (501) staff       (20)      316 2023-05-04 03:46:23.000000 chatllm-2023.6.1.12.39.20/chatllm/applications/chatmind.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1350 2023-05-29 07:27:53.000000 chatllm-2023.6.1.12.39.20/chatllm/applications/chatpdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)      269 2023-04-26 00:59:00.000000 chatllm-2023.6.1.12.39.20/chatllm/applications/chatsearch.py
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 chatllm-2023.6.1.12.39.20/chatllm/applications/chatweb.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1875 2023-05-25 06:54:08.000000 chatllm-2023.6.1.12.39.20/chatllm/applications/chatwhoosh.py
+-rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 chatllm-2023.6.1.12.39.20/chatllm/applications/pipeline.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1964 2023-04-27 09:24:25.000000 chatllm-2023.6.1.12.39.20/chatllm/chatyuan.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:39:20.798333 chatllm-2023.6.1.12.39.20/chatllm/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 chatllm-2023.6.1.12.39.20/chatllm/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 chatllm-2023.6.1.12.39.20/chatllm/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1318 2023-05-30 11:36:20.000000 chatllm-2023.6.1.12.39.20/chatllm/clis/cli.py
+-rw-r--r--   0 betterme   (501) staff       (20)      779 2023-05-25 08:42:08.000000 chatllm-2023.6.1.12.39.20/chatllm/closeai.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1439 2023-04-27 01:39:42.000000 chatllm-2023.6.1.12.39.20/chatllm/embedding.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:39:20.799275 chatllm-2023.6.1.12.39.20/chatllm/llms/
+-rw-r--r--   0 betterme   (501) staff       (20)     1471 2023-05-31 06:17:06.000000 chatllm-2023.6.1.12.39.20/chatllm/llms/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2198 2023-05-31 09:13:06.000000 chatllm-2023.6.1.12.39.20/chatllm/llms/chatglm.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1559 2023-05-22 08:19:27.000000 chatllm-2023.6.1.12.39.20/chatllm/llms/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2083 2023-05-22 08:39:00.000000 chatllm-2023.6.1.12.39.20/chatllm/llms/llama.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:39:20.800746 chatllm-2023.6.1.12.39.20/chatllm/utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      278 2023-04-28 04:20:30.000000 chatllm-2023.6.1.12.39.20/chatllm/utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-28 04:37:16.000000 chatllm-2023.6.1.12.39.20/chatllm/utils/_textsplitter.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2336 2023-05-29 07:27:53.000000 chatllm-2023.6.1.12.39.20/chatllm/utils/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2430 2023-05-19 09:28:43.000000 chatllm-2023.6.1.12.39.20/chatllm/utils/gpu_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6342 2023-05-30 08:31:55.000000 chatllm-2023.6.1.12.39.20/chatllm/utils/nbce.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5208 2023-05-30 08:22:36.000000 chatllm-2023.6.1.12.39.20/chatllm/utils/nbce_test.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:39:20.802689 chatllm-2023.6.1.12.39.20/chatllm/webui/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 chatllm-2023.6.1.12.39.20/chatllm/webui/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1457 2023-05-29 07:27:53.000000 chatllm-2023.6.1.12.39.20/chatllm/webui/chatbase.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3102 2023-06-01 03:54:54.000000 chatllm-2023.6.1.12.39.20/chatllm/webui/chatpdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)      144 2023-05-15 11:46:17.000000 chatllm-2023.6.1.12.39.20/chatllm/webui/conf.yaml
+-rw-r--r--   0 betterme   (501) staff       (20)     4311 2023-04-26 01:00:01.000000 chatllm-2023.6.1.12.39.20/chatllm/webui/gradio_ui.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1819 2023-04-25 03:04:12.000000 chatllm-2023.6.1.12.39.20/chatllm/webui/nice_ui.py
+-rw-r--r--   0 betterme   (501) staff       (20)      220 2023-04-26 07:34:11.000000 chatllm-2023.6.1.12.39.20/chatllm/webui/run.sh
+-rw-r--r--   0 betterme   (501) staff       (20)     3506 2023-05-26 07:39:23.000000 chatllm-2023.6.1.12.39.20/chatllm/webui/visualglm_st.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:39:20.789535 chatllm-2023.6.1.12.39.20/chatllm.egg-info/
+-rw-r--r--   0 betterme   (501) staff       (20)     6665 2023-06-01 04:39:20.000000 chatllm-2023.6.1.12.39.20/chatllm.egg-info/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     2640 2023-06-01 04:39:20.000000 chatllm-2023.6.1.12.39.20/chatllm.egg-info/SOURCES.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-06-01 04:39:20.000000 chatllm-2023.6.1.12.39.20/chatllm.egg-info/dependency_links.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       53 2023-06-01 04:39:20.000000 chatllm-2023.6.1.12.39.20/chatllm.egg-info/entry_points.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-06-01 04:39:20.000000 chatllm-2023.6.1.12.39.20/chatllm.egg-info/not-zip-safe
+-rw-r--r--   0 betterme   (501) staff       (20)      334 2023-06-01 04:39:20.000000 chatllm-2023.6.1.12.39.20/chatllm.egg-info/requires.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        8 2023-06-01 04:39:20.000000 chatllm-2023.6.1.12.39.20/chatllm.egg-info/top_level.txt
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:39:20.806977 chatllm-2023.6.1.12.39.20/data/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:39:20.817053 chatllm-2023.6.1.12.39.20/data/imgs/
+-rw-r--r--   0 betterme   (501) staff       (20)   206137 2023-04-26 05:39:20.000000 chatllm-2023.6.1.12.39.20/data/imgs/LLM.drawio.png
+-rw-r--r--   0 betterme   (501) staff       (20)   206363 2023-04-26 05:33:47.000000 chatllm-2023.6.1.12.39.20/data/imgs/LLM.png
+-rw-r--r--   0 betterme   (501) staff       (20)    80933 2023-05-31 01:13:52.000000 chatllm-2023.6.1.12.39.20/data/imgs/chatbox.png
+-rw-r--r--   0 betterme   (501) staff       (20)  1230065 2023-04-26 08:27:23.000000 chatllm-2023.6.1.12.39.20/data/imgs/chatpdf.gif
+-rw-r--r--   0 betterme   (501) staff       (20)    45633 2023-04-26 04:24:13.000000 chatllm-2023.6.1.12.39.20/data/imgs/chatpdf_ann_df.png
+-rw-r--r--   0 betterme   (501) staff       (20)   477462 2023-05-08 01:03:47.000000 chatllm-2023.6.1.12.39.20/data/imgs/img.png
+-rw-r--r--   0 betterme   (501) staff       (20)   333086 2023-05-08 01:03:52.000000 chatllm-2023.6.1.12.39.20/data/imgs/img_1.png
+-rw-r--r--   0 betterme   (501) staff       (20)    29400 2023-04-27 10:24:48.000000 chatllm-2023.6.1.12.39.20/data/imgs/role.png
+-rw-r--r--   0 betterme   (501) staff       (20)   443539 2023-05-26 00:55:04.000000 chatllm-2023.6.1.12.39.20/data/imgs/群.png
+-rw-r--r--   0 betterme   (501) staff       (20)    31192 2023-05-29 00:57:03.000000 chatllm-2023.6.1.12.39.20/data/openai_keys.md
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:39:20.822571 chatllm-2023.6.1.12.39.20/data/医/
+-rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 chatllm-2023.6.1.12.39.20/data/医/500种中药现代研究.txt
+-rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 chatllm-2023.6.1.12.39.20/data/医/古今医统大全.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 chatllm-2023.6.1.12.39.20/data/姚明.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 chatllm-2023.6.1.12.39.20/data/王治郅.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 chatllm-2023.6.1.12.39.20/data/科比.txt
+-rw-r--r--   0 betterme   (501) staff       (20)  3051914 2023-04-25 02:58:13.000000 chatllm-2023.6.1.12.39.20/data/财报.pdf
+-rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 chatllm-2023.6.1.12.39.20/data/马保国.txt
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:39:20.832548 chatllm-2023.6.1.12.39.20/docs/
+-rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 chatllm-2023.6.1.12.39.20/docs/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 chatllm-2023.6.1.12.39.20/docs/authors.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 chatllm-2023.6.1.12.39.20/docs/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 chatllm-2023.6.1.12.39.20/docs/contributing.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 chatllm-2023.6.1.12.39.20/docs/history.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 chatllm-2023.6.1.12.39.20/docs/index.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 chatllm-2023.6.1.12.39.20/docs/make.bat
+-rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 chatllm-2023.6.1.12.39.20/docs/readme.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 chatllm-2023.6.1.12.39.20/docs/usage.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)      332 2023-05-31 10:28:33.000000 chatllm-2023.6.1.12.39.20/git_init.sh
+-rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 chatllm-2023.6.1.12.39.20/pypi.sh
+-rw-r--r--   0 betterme   (501) staff       (20)       90 2023-05-26 09:35:58.000000 chatllm-2023.6.1.12.39.20/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       14 2023-05-19 09:53:16.000000 chatllm-2023.6.1.12.39.20/requirements_ann.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       30 2023-05-31 02:41:18.000000 chatllm-2023.6.1.12.39.20/requirements_api.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       29 2023-05-26 08:03:09.000000 chatllm-2023.6.1.12.39.20/requirements_openai.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2023-05-29 04:24:55.000000 chatllm-2023.6.1.12.39.20/requirements_pdf.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       25 2023-05-29 04:24:55.000000 chatllm-2023.6.1.12.39.20/requirements_streamlit.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       38 2023-06-01 04:39:20.835102 chatllm-2023.6.1.12.39.20/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     1700 2023-05-31 05:17:11.000000 chatllm-2023.6.1.12.39.20/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-01 04:39:20.833117 chatllm-2023.6.1.12.39.20/tests/
+-rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 chatllm-2023.6.1.12.39.20/tests/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 chatllm-2023.6.1.12.39.20/tests/test_llm4gpt.py
+-rw-r--r--   0 betterme   (501) staff       (20)    51173 2023-04-21 11:31:44.000000 chatllm-2023.6.1.12.39.20/tests/内存型.ipynb
+-rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 chatllm-2023.6.1.12.39.20/tox.ini
```

### Comparing `ChatLLM-2023.5.4.12.7.23/.gitignore` & `chatllm-2023.6.1.12.39.20/.gitignore`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.12.7.23/.travis.yml` & `chatllm-2023.6.1.12.39.20/.travis.yml`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.12.7.23/ChatLLM.egg-info/PKG-INFO` & `chatllm-2023.6.1.12.39.20/README.md.bak`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,7 @@
-Metadata-Version: 2.1
-Name: ChatLLM
-Version: 2023.5.4.12.7.23
-Summary: Create a Python package.
-Home-page: https://github.com/yuanjie-ai/ChatLLM
-Author: yuanjie
-Author-email: 313303303@qq.com
-License: MIT license
-Keywords: chatllm
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: api
-Provides-Extra: pdf
-Provides-Extra: streamlit
-Provides-Extra: all
-License-File: LICENSE
-License-File: AUTHORS.rst
-
 ![image](https://img.shields.io/pypi/v/llm4gpt.svg) ![image](https://img.shields.io/travis/yuanjie-ai/llm4gpt.svg) ![image](https://readthedocs.org/projects/llm4gpt/badge/?version=latest)
 
 <h1 align = "center">🔥ChatLLM 基于知识库🔥</h1>
 
 <div align=center>
 <img src="data/imgs/LLM.drawio.png"/>
 </div>
@@ -42,127 +16,155 @@
 
 ## Usages
 
 ```python
 from chatllm.applications import ChatBase
 
 qa = ChatBase()
-qa.load_llm4chat(model_name_or_path="THUDM/chatglm-6b")
-
-_ = list(qa(query='周杰伦是谁', knowledge_base='周杰伦是傻子', role=' '))
+qa.load_llm(model_name_or_path="THUDM/chatglm-6b")
+for i in qa(query='周杰伦是谁', knowledge_base='周杰伦是傻子'):
+    print(i, end='')
 # 根据已知信息无法回答该问题，因为周杰伦是中国内地流行歌手、演员、音乐制作人、导演，
 # 是具有一定的知名度和专业能力的人物，没有提供足够的信息无法判断他是傻子。
 ```
+
 - 支持角色扮演
-![img.png](data/imgs/role.png)
+  ![img.png](data/imgs/role.png)
+
+## OpenaiEcosystem
+<details markdown="1">
+  <summary>Click to 无缝对接openai生态</summary>
+
+```shell
+# 服务端
+pip install "chatllm[openai]" && chatllm-run openai <本地模型地址>
+```
+```python
+# 客户端
+import openai
+
+openai.api_base = 'http://0.0.0.0:8000/v1'
+openai.api_key = 'chatllm'
+prompt = "你好"
+completion = openai.Completion.create(prompt=prompt, stream=True, model="text-davinci-003")
+for c in completion:
+    print(c.choices[0].text, end='')
+# 你好👋!我是人工智能助手 ChatGLM-6B,很高兴见到你，欢迎问我任何问题。
+```
+### [openai_keys](./data/openai_keys.md): `不定期更新免费keys`
+</details>
 
 ## ChatPDF
+
 <details markdown="1">
   <summary>Click to ChatPDF</summary>
 
-一键启动UI `chatllm-run webui --name chatpdf`
+
+```shell
+pip install "chatllm[pdf]" && chatllm-run webui --name chatpdf
+```
+
+- python交互
 
 ```python
 from chatllm.applications.chatpdf import ChatPDF
 
 qa = ChatPDF(encode_model='nghuyong/ernie-3.0-nano-zh')
-qa.load_llm4chat(model_name_or_path="THUDM/chatglm-6b")
+qa.load_llm(model_name_or_path="THUDM/chatglm-6b")
 qa.create_index('财报.pdf')  # 构建知识库
 
-list(qa(query='东北证券主营业务'))
+for i in qa(query='东北证券主营业务'):
+    print(i, end='')
 # 根据已知信息，东北证券的主营业务为证券业务。公司作为证券公司，主要从事证券经纪、证券投资咨询、与证券交易、
 # 证券投资活动有关的财务顾问、证券承销与保荐、证券自营、融资融券、证券投资基金代销和代销金融产品待业务。
 ```
-- 支持查看召回结果
-![向量召回结果](data/imgs/chatpdf.gif)
+
+- 支持召回结果查看
+  ![向量召回结果](data/imgs/chatpdf.gif)
 
 </details>
 
 ## Deploy
 
 <details markdown="1">
   <summary>Click to Deploy</summary>
 
 - ChatGLM-6B 模型硬件需求
 
-    | **量化等级**   | **最低 GPU 显存**（推理） | **最低 GPU 显存**（高效参数微调） |
-    | -------------- | ------------------------- | --------------------------------- |
-    | FP16（无量化） | 13 GB                     | 14 GB                             |
-    | INT8           | 8 GB                     | 9 GB                             |
-    | INT4           | 6 GB                      | 7 GB                              |
+  | **量化等级**   | **最低 GPU 显存**（推理） | **最低 GPU 显存**（高效参数微调） |
+      | -------------- | ------------------------- | --------------------------------- |
+  | FP16（无量化） | 13 GB                     | 14 GB                             |
+  | INT8           | 8 GB                     | 9 GB                             |
+  | INT4           | 6 GB                      | 7 GB                              |
 
 
 - 从本地加载模型
-  - [安装指南](docs/INSTALL.md)
-  - [ChatGLM-6B Mac 本地部署实操记录](https://www.yuque.com/arvinxx/llm/chatglm-6b-deployment-on-mac)
-  - [THUDM/ChatGLM-6B#从本地加载模型](https://github.com/THUDM/ChatGLM-6B#从本地加载模型)
+    - [安装指南](docs/INSTALL.md)
+    - [ChatGLM-6B Mac 本地部署实操记录](https://www.yuque.com/arvinxx/llm/chatglm-6b-deployment-on-mac)
+    - [THUDM/ChatGLM-6B#从本地加载模型](https://github.com/THUDM/ChatGLM-6B#从本地加载模型)
 
 </details>
 
 ## TODO
+
 <details markdown="1">
   <summary>Click to TODO</summary>
 
 - [ ] ChatLLM 应用
-  - [x] 接入非结构化文档（已支持 md、pdf、docx、txt 文件格式）
-  - [ ] 搜索引擎与本地网页接入
-  - [ ] 结构化数据接入（如 csv、Excel、SQL 等）
-  - [ ] 知识图谱/图数据库接入
-  - [ ] 增加 ANN 后端，ES/RedisSearch【确保生产高可用】
-  - [ ] 增加多级缓存缓存
+    - [x] 接入非结构化文档（已支持 md、pdf、docx、txt 文件格式）
+    - [ ] 搜索引擎与本地网页接入
+    - [ ] 结构化数据接入（如 csv、Excel、SQL 等）
+    - [ ] 知识图谱/图数据库接入
+    - [ ] 增加 ANN 后端，ES/RedisSearch【确保生产高可用】
+    - [ ] 增加多级缓存缓存
 
 - [ ] 多路召回
-  - [ ] 问
-    - [ ] 标量匹配
-    - [x] 多种向量化，向量匹配
-    - [ ] 增加相似问，换几个问法
-    - [ ] 高置信度直接返回答案【匹配标准问】
-  - [ ] 答
-    - [ ] 高置信度篇章
-    - [ ] 增加上下文信息
-    - [ ] 增加夸篇章信息
-    - [ ] 增加召回信息的相似信息
-    - [ ] 提前生成标准问，匹配问
-    - [ ] 拒绝推断
+    - [ ] 问
+        - [ ] 标量匹配
+        - [x] 多种向量化，向量匹配
+        - [ ] 增加相似问，换几个问法
+        - [ ] 高置信度直接返回答案【匹配标准问】
+    - [ ] 答
+        - [ ] 高置信度篇章
+        - [ ] 增加上下文信息
+        - [ ] 增加夸篇章信息
+        - [ ] 增加召回信息的相似信息
+        - [ ] 提前生成标准问，匹配问
+        - [ ] 拒绝推断
 
 
 - [ ] 增加更多 LLM 模型支持
-  - [x] [THUDM/chatglm-6b](https://huggingface.co/THUDM/chatglm-6b)
-  - [ ] [THUDM/chatglm-6b-int8](https://huggingface.co/THUDM/chatglm-6b-int8)
-  - [ ] [THUDM/chatglm-6b-int4](https://huggingface.co/THUDM/chatglm-6b-int4)
-  - [ ] [THUDM/chatglm-6b-int4-qe](https://huggingface.co/THUDM/chatglm-6b-int4-qe)
-  - [ ] [ClueAI/ChatYuan-large-v2](https://huggingface.co/ClueAI/ChatYuan-large-v2)
+    - [x] [THUDM/chatglm-6b](https://huggingface.co/THUDM/chatglm-6b)
+    - [ ] [THUDM/chatglm-6b-int8](https://huggingface.co/THUDM/chatglm-6b-int8)
+    - [ ] [THUDM/chatglm-6b-int4](https://huggingface.co/THUDM/chatglm-6b-int4)
+    - [ ] [THUDM/chatglm-6b-int4-qe](https://huggingface.co/THUDM/chatglm-6b-int4-qe)
+    - [ ] [ClueAI/ChatYuan-large-v2](https://huggingface.co/ClueAI/ChatYuan-large-v2)
 - [ ] 增加更多 Embedding 模型支持
-  - [x] [nghuyong/ernie-3.0-nano-zh](https://huggingface.co/nghuyong/ernie-3.0-nano-zh)
-  - [x] [nghuyong/ernie-3.0-base-zh](https://huggingface.co/nghuyong/ernie-3.0-base-zh)
-  - [x] [shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese)
-  - [x] [GanymedeNil/text2vec-large-chinese](https://huggingface.co/GanymedeNil/text2vec-large-chinese)
+    - [x] [nghuyong/ernie-3.0-nano-zh](https://huggingface.co/nghuyong/ernie-3.0-nano-zh)
+    - [x] [nghuyong/ernie-3.0-base-zh](https://huggingface.co/nghuyong/ernie-3.0-base-zh)
+    - [x] [shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese)
+    - [x] [GanymedeNil/text2vec-large-chinese](https://huggingface.co/GanymedeNil/text2vec-large-chinese)
 - [x] 增加一键启动 webui
-  - [x] 利用 streamlit 实现 ChatPDF，一键启动 `chatllm-run webui --name chatpdf`
-  - [ ] 利用 gradio 实现 Web UI DEMO
-  - [ ] 添加输出内容及错误提示
-  - [ ] 引用标注
-  - [ ] 增加知识库管理
-    - [ ] 选择知识库开始问答
-    - [ ] 上传文件/文件夹至知识库
-    - [ ] 删除知识库中文件
+    - [x] 利用 streamlit 实现 ChatPDF，一键启动 `chatllm-run webui --name chatpdf`
+    - [ ] 利用 gradio 实现 Web UI DEMO
+    - [ ] 添加输出内容及错误提示
+    - [ ] 引用标注
+    - [ ] 增加知识库管理
+        - [ ] 选择知识库开始问答
+        - [ ] 上传文件/文件夹至知识库
+        - [ ] 删除知识库中文件
 - [ ] 增加 API 支持
-  - [x] 利用 Fastapi/Flask/Grpc 实现流式接口 `chatllm-run flask-api --model_name_or_path <MODEL_PATH> --host 127.0.0.1 --port 8000`
-  - [ ] 前后端分离，实现调用 API 的 Web UI Demo
-
-## 交流群
-![二维码]()
+    - [x] 利用 Fastapi/Flask/Grpc
+      实现流式接口 `chatllm-run openai <本地模型地址> --host 127.0.0.1 --port 8000`
+    - [ ] 前后端分离，实现调用 API 的 Web UI Demo
 
 </details>
 
+## 交流群
+<div align=center>
+<img src="data/imgs/群.png" alt="群" width="250" height="400">
+</div>
 
+> 若二维码失效加微信拉群 313303303
 
 
 
-=======
-History
-=======
-
-0.0.0 (2023-04-11)
-------------------
-
-* First release on PyPI.
```

### Comparing `ChatLLM-2023.5.4.12.7.23/ChatLLM.egg-info/SOURCES.txt` & `chatllm-2023.6.1.12.39.20/chatllm.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,59 @@
 .editorconfig
 .gitignore
 .travis.yml
-AUTHORS.rst
-CONTRIBUTING.rst
-HISTORY.rst
 LICENSE
 MANIFEST.in
 Makefile
-README.bak.md
 README.md
+README.md.bak
+TODO.md
 git_init.sh
 pypi.sh
 requirements.txt
+requirements_ann.txt
 requirements_api.txt
+requirements_openai.txt
 requirements_pdf.txt
 requirements_streamlit.txt
 setup.py
 tox.ini
-ChatLLM.egg-info/PKG-INFO
-ChatLLM.egg-info/SOURCES.txt
-ChatLLM.egg-info/dependency_links.txt
-ChatLLM.egg-info/entry_points.txt
-ChatLLM.egg-info/not-zip-safe
-ChatLLM.egg-info/requires.txt
-ChatLLM.egg-info/top_level.txt
 chatllm/__init__.py
 chatllm/chatyuan.py
+chatllm/closeai.py
 chatllm/embedding.py
+chatllm.egg-info/PKG-INFO
+chatllm.egg-info/SOURCES.txt
+chatllm.egg-info/dependency_links.txt
+chatllm.egg-info/entry_points.txt
+chatllm.egg-info/not-zip-safe
+chatllm.egg-info/requires.txt
+chatllm.egg-info/top_level.txt
 chatllm/_his/FaissANN.py
 chatllm/_his/__init__.py
 chatllm/_his/_chatllm.py
 chatllm/_his/_qa.py
+chatllm/aigc/__init__.py
+chatllm/aigc/common.py
+chatllm/api/TODO.md
 chatllm/api/__init__.py
-chatllm/api/stream_api.py
+chatllm/api/app.py
+chatllm/api/config.py
+chatllm/api/datamodels.py
+chatllm/api/openai_client.py
+chatllm/api/sse_api.py
+chatllm/api/test.py
+chatllm/api/routes/__init__.py
+chatllm/api/routes/api.py
+chatllm/api/routes/base.py
+chatllm/api/routes/completions.py
+chatllm/api/routes/embeddings.py
+chatllm/api/routes/responses.py
 chatllm/applications/Question2Answer.py
+chatllm/applications/__chatbase.py
 chatllm/applications/__init__.py
 chatllm/applications/chatann.py
 chatllm/applications/chataudio.py
 chatllm/applications/chatbase.py
 chatllm/applications/chatcrawler.py
 chatllm/applications/chatdoc.py
 chatllm/applications/chatmind.py
@@ -45,42 +61,50 @@
 chatllm/applications/chatsearch.py
 chatllm/applications/chatweb.py
 chatllm/applications/chatwhoosh.py
 chatllm/applications/pipeline.py
 chatllm/clis/README.md
 chatllm/clis/__init__.py
 chatllm/clis/cli.py
-chatllm/parse_utils/__init__.py
-chatllm/parse_utils/doc_parse.py
+chatllm/llms/__init__.py
+chatllm/llms/chatglm.py
+chatllm/llms/demo.py
+chatllm/llms/llama.py
 chatllm/utils/__init__.py
 chatllm/utils/_textsplitter.py
 chatllm/utils/common.py
 chatllm/utils/gpu_utils.py
+chatllm/utils/nbce.py
+chatllm/utils/nbce_test.py
 chatllm/webui/__init__.py
 chatllm/webui/chatbase.py
 chatllm/webui/chatpdf.py
+chatllm/webui/conf.yaml
 chatllm/webui/gradio_ui.py
 chatllm/webui/nice_ui.py
 chatllm/webui/run.sh
+chatllm/webui/visualglm_st.py
+data/openai_keys.md
 data/姚明.txt
 data/王治郅.txt
 data/科比.txt
 data/财报.pdf
 data/马保国.txt
 data/imgs/LLM.drawio.png
 data/imgs/LLM.png
+data/imgs/chatbox.png
 data/imgs/chatpdf.gif
 data/imgs/chatpdf_ann_df.png
+data/imgs/img.png
+data/imgs/img_1.png
 data/imgs/role.png
+data/imgs/群.png
 data/医/500种中药现代研究.txt
 data/医/古今医统大全.txt
-docs/INSTALL.md
 docs/Makefile
-docs/README.md
-docs/_config.yml
 docs/authors.rst
 docs/conf.py
 docs/contributing.rst
 docs/history.rst
 docs/index.rst
 docs/make.bat
 docs/readme.rst
```

### Comparing `ChatLLM-2023.5.4.12.7.23/LICENSE` & `chatllm-2023.6.1.12.39.20/LICENSE`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.12.7.23/Makefile` & `chatllm-2023.6.1.12.39.20/Makefile`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.12.7.23/PKG-INFO` & `chatllm-2023.6.1.12.39.20/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,7 @@
-Metadata-Version: 2.1
-Name: ChatLLM
-Version: 2023.5.4.12.7.23
-Summary: Create a Python package.
-Home-page: https://github.com/yuanjie-ai/ChatLLM
-Author: yuanjie
-Author-email: 313303303@qq.com
-License: MIT license
-Keywords: chatllm
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: api
-Provides-Extra: pdf
-Provides-Extra: streamlit
-Provides-Extra: all
-License-File: LICENSE
-License-File: AUTHORS.rst
-
 ![image](https://img.shields.io/pypi/v/llm4gpt.svg) ![image](https://img.shields.io/travis/yuanjie-ai/llm4gpt.svg) ![image](https://readthedocs.org/projects/llm4gpt/badge/?version=latest)
 
 <h1 align = "center">🔥ChatLLM 基于知识库🔥</h1>
 
 <div align=center>
 <img src="data/imgs/LLM.drawio.png"/>
 </div>
@@ -42,127 +16,155 @@
 
 ## Usages
 
 ```python
 from chatllm.applications import ChatBase
 
 qa = ChatBase()
-qa.load_llm4chat(model_name_or_path="THUDM/chatglm-6b")
-
-_ = list(qa(query='周杰伦是谁', knowledge_base='周杰伦是傻子', role=' '))
+qa.load_llm(model_name_or_path="THUDM/chatglm-6b")
+for i in qa(query='周杰伦是谁', knowledge_base='周杰伦是傻子'):
+    print(i, end='')
 # 根据已知信息无法回答该问题，因为周杰伦是中国内地流行歌手、演员、音乐制作人、导演，
 # 是具有一定的知名度和专业能力的人物，没有提供足够的信息无法判断他是傻子。
 ```
-- 支持角色扮演
-![img.png](data/imgs/role.png)
+
+## OpenaiEcosystem
+<details markdown="1">
+  <summary>Click to 无缝对接openai生态</summary>
+
+```shell
+# 服务端
+pip install "chatllm[openai]" && chatllm-run openai <本地模型地址>
+```
+- SDK：`pip install openai`
+```python
+import openai
+
+openai.api_base = 'http://0.0.0.0:8000/v1'
+openai.api_key = 'chatllm'
+prompt = "你好"
+completion = openai.Completion.create(prompt=prompt, stream=True, model="text-davinci-003")
+for c in completion:
+    print(c.choices[0].text, end='')
+# 你好👋!我是人工智能助手 ChatGLM-6B,很高兴见到你，欢迎问我任何问题。
+```
+- 客户端：[点击下载chatbox](https://chatboxapp.xyz/)，也可接入客户端
+![客户端](data/imgs/chatbox.png)
+
+### [openai_keys](./data/openai_keys.md): `不定期更新免费keys`
+</details>
 
 ## ChatPDF
+
 <details markdown="1">
   <summary>Click to ChatPDF</summary>
 
-一键启动UI `chatllm-run webui --name chatpdf`
+
+```shell
+pip install "chatllm[pdf]" && chatllm-run webui --name chatpdf
+```
+
+- python交互
 
 ```python
 from chatllm.applications.chatpdf import ChatPDF
 
 qa = ChatPDF(encode_model='nghuyong/ernie-3.0-nano-zh')
-qa.load_llm4chat(model_name_or_path="THUDM/chatglm-6b")
+qa.load_llm(model_name_or_path="THUDM/chatglm-6b")
 qa.create_index('财报.pdf')  # 构建知识库
 
-list(qa(query='东北证券主营业务'))
+for i in qa(query='东北证券主营业务'):
+    print(i, end='')
 # 根据已知信息，东北证券的主营业务为证券业务。公司作为证券公司，主要从事证券经纪、证券投资咨询、与证券交易、
 # 证券投资活动有关的财务顾问、证券承销与保荐、证券自营、融资融券、证券投资基金代销和代销金融产品待业务。
 ```
-- 支持查看召回结果
-![向量召回结果](data/imgs/chatpdf.gif)
+
+- 支持召回结果查看
+  ![向量召回结果](data/imgs/chatpdf.gif)
 
 </details>
 
 ## Deploy
 
 <details markdown="1">
   <summary>Click to Deploy</summary>
 
 - ChatGLM-6B 模型硬件需求
 
-    | **量化等级**   | **最低 GPU 显存**（推理） | **最低 GPU 显存**（高效参数微调） |
-    | -------------- | ------------------------- | --------------------------------- |
-    | FP16（无量化） | 13 GB                     | 14 GB                             |
-    | INT8           | 8 GB                     | 9 GB                             |
-    | INT4           | 6 GB                      | 7 GB                              |
+  | **量化等级**   | **最低 GPU 显存**（推理） | **最低 GPU 显存**（高效参数微调） |
+      | -------------- | ------------------------- | --------------------------------- |
+  | FP16（无量化） | 13 GB                     | 14 GB                             |
+  | INT8           | 8 GB                     | 9 GB                             |
+  | INT4           | 6 GB                      | 7 GB                              |
 
 
 - 从本地加载模型
-  - [安装指南](docs/INSTALL.md)
-  - [ChatGLM-6B Mac 本地部署实操记录](https://www.yuque.com/arvinxx/llm/chatglm-6b-deployment-on-mac)
-  - [THUDM/ChatGLM-6B#从本地加载模型](https://github.com/THUDM/ChatGLM-6B#从本地加载模型)
+    - [安装指南](docs/INSTALL.md)
+    - [ChatGLM-6B Mac 本地部署实操记录](https://www.yuque.com/arvinxx/llm/chatglm-6b-deployment-on-mac)
+    - [THUDM/ChatGLM-6B#从本地加载模型](https://github.com/THUDM/ChatGLM-6B#从本地加载模型)
 
 </details>
 
 ## TODO
+
 <details markdown="1">
   <summary>Click to TODO</summary>
 
 - [ ] ChatLLM 应用
-  - [x] 接入非结构化文档（已支持 md、pdf、docx、txt 文件格式）
-  - [ ] 搜索引擎与本地网页接入
-  - [ ] 结构化数据接入（如 csv、Excel、SQL 等）
-  - [ ] 知识图谱/图数据库接入
-  - [ ] 增加 ANN 后端，ES/RedisSearch【确保生产高可用】
-  - [ ] 增加多级缓存缓存
+    - [x] 接入非结构化文档（已支持 md、pdf、docx、txt 文件格式）
+    - [ ] 搜索引擎与本地网页接入
+    - [ ] 结构化数据接入（如 csv、Excel、SQL 等）
+    - [ ] 知识图谱/图数据库接入
+    - [ ] 增加 ANN 后端，ES/RedisSearch【确保生产高可用】
+    - [ ] 增加多级缓存缓存
 
 - [ ] 多路召回
-  - [ ] 问
-    - [ ] 标量匹配
-    - [x] 多种向量化，向量匹配
-    - [ ] 增加相似问，换几个问法
-    - [ ] 高置信度直接返回答案【匹配标准问】
-  - [ ] 答
-    - [ ] 高置信度篇章
-    - [ ] 增加上下文信息
-    - [ ] 增加夸篇章信息
-    - [ ] 增加召回信息的相似信息
-    - [ ] 提前生成标准问，匹配问
-    - [ ] 拒绝推断
+    - [ ] 问
+        - [ ] 标量匹配
+        - [x] 多种向量化，向量匹配
+        - [ ] 增加相似问，换几个问法
+        - [ ] 高置信度直接返回答案【匹配标准问】
+    - [ ] 答
+        - [ ] 高置信度篇章
+        - [ ] 增加上下文信息
+        - [ ] 增加夸篇章信息
+        - [ ] 增加召回信息的相似信息
+        - [ ] 提前生成标准问，匹配问
+        - [ ] 拒绝推断
 
 
 - [ ] 增加更多 LLM 模型支持
-  - [x] [THUDM/chatglm-6b](https://huggingface.co/THUDM/chatglm-6b)
-  - [ ] [THUDM/chatglm-6b-int8](https://huggingface.co/THUDM/chatglm-6b-int8)
-  - [ ] [THUDM/chatglm-6b-int4](https://huggingface.co/THUDM/chatglm-6b-int4)
-  - [ ] [THUDM/chatglm-6b-int4-qe](https://huggingface.co/THUDM/chatglm-6b-int4-qe)
-  - [ ] [ClueAI/ChatYuan-large-v2](https://huggingface.co/ClueAI/ChatYuan-large-v2)
+    - [x] [THUDM/chatglm-6b](https://huggingface.co/THUDM/chatglm-6b)
+    - [ ] [THUDM/chatglm-6b-int8](https://huggingface.co/THUDM/chatglm-6b-int8)
+    - [ ] [THUDM/chatglm-6b-int4](https://huggingface.co/THUDM/chatglm-6b-int4)
+    - [ ] [THUDM/chatglm-6b-int4-qe](https://huggingface.co/THUDM/chatglm-6b-int4-qe)
+    - [ ] [ClueAI/ChatYuan-large-v2](https://huggingface.co/ClueAI/ChatYuan-large-v2)
 - [ ] 增加更多 Embedding 模型支持
-  - [x] [nghuyong/ernie-3.0-nano-zh](https://huggingface.co/nghuyong/ernie-3.0-nano-zh)
-  - [x] [nghuyong/ernie-3.0-base-zh](https://huggingface.co/nghuyong/ernie-3.0-base-zh)
-  - [x] [shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese)
-  - [x] [GanymedeNil/text2vec-large-chinese](https://huggingface.co/GanymedeNil/text2vec-large-chinese)
+    - [x] [nghuyong/ernie-3.0-nano-zh](https://huggingface.co/nghuyong/ernie-3.0-nano-zh)
+    - [x] [nghuyong/ernie-3.0-base-zh](https://huggingface.co/nghuyong/ernie-3.0-base-zh)
+    - [x] [shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese)
+    - [x] [GanymedeNil/text2vec-large-chinese](https://huggingface.co/GanymedeNil/text2vec-large-chinese)
 - [x] 增加一键启动 webui
-  - [x] 利用 streamlit 实现 ChatPDF，一键启动 `chatllm-run webui --name chatpdf`
-  - [ ] 利用 gradio 实现 Web UI DEMO
-  - [ ] 添加输出内容及错误提示
-  - [ ] 引用标注
-  - [ ] 增加知识库管理
-    - [ ] 选择知识库开始问答
-    - [ ] 上传文件/文件夹至知识库
-    - [ ] 删除知识库中文件
+    - [x] 利用 streamlit 实现 ChatPDF，一键启动 `chatllm-run webui --name chatpdf`
+    - [ ] 利用 gradio 实现 Web UI DEMO
+    - [ ] 添加输出内容及错误提示
+    - [ ] 引用标注
+    - [ ] 增加知识库管理
+        - [ ] 选择知识库开始问答
+        - [ ] 上传文件/文件夹至知识库
+        - [ ] 删除知识库中文件
 - [ ] 增加 API 支持
-  - [x] 利用 Fastapi/Flask/Grpc 实现流式接口 `chatllm-run flask-api --model_name_or_path <MODEL_PATH> --host 127.0.0.1 --port 8000`
-  - [ ] 前后端分离，实现调用 API 的 Web UI Demo
-
-## 交流群
-![二维码]()
+    - [x] 利用 Fastapi/Flask/Grpc
+      实现流式接口 `chatllm-run openai <本地模型地址> --host 127.0.0.1 --port 8000`
+    - [ ] 前后端分离，实现调用 API 的 Web UI Demo
 
 </details>
 
+## 交流群
+<div align=center>
+<img src="data/imgs/群.png" alt="群" width="250" height="400">
+</div>
 
+> 若二维码失效加微信拉群 313303303
 
 
 
-=======
-History
-=======
-
-0.0.0 (2023-04-11)
-------------------
-
-* First release on PyPI.
```

### Comparing `ChatLLM-2023.5.4.12.7.23/README.md` & `chatllm-2023.6.1.12.39.20/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+Metadata-Version: 2.1
+Name: chatllm
+Version: 2023.6.1.12.39.20
+Summary: Create a Python package.
+Home-page: https://github.com/yuanjie-ai/ChatLLM
+Author: yuanjie
+Author-email: 313303303@qq.com
+License: MIT license
+Keywords: chatllm
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: ann
+Provides-Extra: api
+Provides-Extra: pdf
+Provides-Extra: openai
+Provides-Extra: streamlit
+Provides-Extra: all
+License-File: LICENSE
+
 ![image](https://img.shields.io/pypi/v/llm4gpt.svg) ![image](https://img.shields.io/travis/yuanjie-ai/llm4gpt.svg) ![image](https://readthedocs.org/projects/llm4gpt/badge/?version=latest)
 
 <h1 align = "center">🔥ChatLLM 基于知识库🔥</h1>
 
 <div align=center>
 <img src="data/imgs/LLM.drawio.png"/>
 </div>
@@ -16,117 +41,155 @@
 
 ## Usages
 
 ```python
 from chatllm.applications import ChatBase
 
 qa = ChatBase()
-qa.load_llm4chat(model_name_or_path="THUDM/chatglm-6b")
-
-_ = list(qa(query='周杰伦是谁', knowledge_base='周杰伦是傻子', role=' '))
+qa.load_llm(model_name_or_path="THUDM/chatglm-6b")
+for i in qa(query='周杰伦是谁', knowledge_base='周杰伦是傻子'):
+    print(i, end='')
 # 根据已知信息无法回答该问题，因为周杰伦是中国内地流行歌手、演员、音乐制作人、导演，
 # 是具有一定的知名度和专业能力的人物，没有提供足够的信息无法判断他是傻子。
 ```
-- 支持角色扮演
-![img.png](data/imgs/role.png)
+
+## OpenaiEcosystem
+<details markdown="1">
+  <summary>Click to 无缝对接openai生态</summary>
+
+```shell
+# 服务端
+pip install "chatllm[openai]" && chatllm-run openai <本地模型地址>
+```
+- SDK：`pip install openai`
+```python
+import openai
+
+openai.api_base = 'http://0.0.0.0:8000/v1'
+openai.api_key = 'chatllm'
+prompt = "你好"
+completion = openai.Completion.create(prompt=prompt, stream=True, model="text-davinci-003")
+for c in completion:
+    print(c.choices[0].text, end='')
+# 你好👋!我是人工智能助手 ChatGLM-6B,很高兴见到你，欢迎问我任何问题。
+```
+- 客户端：[点击下载chatbox](https://chatboxapp.xyz/)，也可接入客户端
+![客户端](data/imgs/chatbox.png)
+
+### [openai_keys](./data/openai_keys.md): `不定期更新免费keys`
+</details>
 
 ## ChatPDF
+
 <details markdown="1">
   <summary>Click to ChatPDF</summary>
 
-一键启动UI `chatllm-run webui --name chatpdf`
+
+```shell
+pip install "chatllm[pdf]" && chatllm-run webui --name chatpdf
+```
+
+- python交互
 
 ```python
 from chatllm.applications.chatpdf import ChatPDF
 
 qa = ChatPDF(encode_model='nghuyong/ernie-3.0-nano-zh')
-qa.load_llm4chat(model_name_or_path="THUDM/chatglm-6b")
+qa.load_llm(model_name_or_path="THUDM/chatglm-6b")
 qa.create_index('财报.pdf')  # 构建知识库
 
-list(qa(query='东北证券主营业务'))
+for i in qa(query='东北证券主营业务'):
+    print(i, end='')
 # 根据已知信息，东北证券的主营业务为证券业务。公司作为证券公司，主要从事证券经纪、证券投资咨询、与证券交易、
 # 证券投资活动有关的财务顾问、证券承销与保荐、证券自营、融资融券、证券投资基金代销和代销金融产品待业务。
 ```
-- 支持查看召回结果
-![向量召回结果](data/imgs/chatpdf.gif)
+
+- 支持召回结果查看
+  ![向量召回结果](data/imgs/chatpdf.gif)
 
 </details>
 
 ## Deploy
 
 <details markdown="1">
   <summary>Click to Deploy</summary>
 
 - ChatGLM-6B 模型硬件需求
 
-    | **量化等级**   | **最低 GPU 显存**（推理） | **最低 GPU 显存**（高效参数微调） |
-    | -------------- | ------------------------- | --------------------------------- |
-    | FP16（无量化） | 13 GB                     | 14 GB                             |
-    | INT8           | 8 GB                     | 9 GB                             |
-    | INT4           | 6 GB                      | 7 GB                              |
+  | **量化等级**   | **最低 GPU 显存**（推理） | **最低 GPU 显存**（高效参数微调） |
+      | -------------- | ------------------------- | --------------------------------- |
+  | FP16（无量化） | 13 GB                     | 14 GB                             |
+  | INT8           | 8 GB                     | 9 GB                             |
+  | INT4           | 6 GB                      | 7 GB                              |
 
 
 - 从本地加载模型
-  - [安装指南](docs/INSTALL.md)
-  - [ChatGLM-6B Mac 本地部署实操记录](https://www.yuque.com/arvinxx/llm/chatglm-6b-deployment-on-mac)
-  - [THUDM/ChatGLM-6B#从本地加载模型](https://github.com/THUDM/ChatGLM-6B#从本地加载模型)
+    - [安装指南](docs/INSTALL.md)
+    - [ChatGLM-6B Mac 本地部署实操记录](https://www.yuque.com/arvinxx/llm/chatglm-6b-deployment-on-mac)
+    - [THUDM/ChatGLM-6B#从本地加载模型](https://github.com/THUDM/ChatGLM-6B#从本地加载模型)
 
 </details>
 
 ## TODO
+
 <details markdown="1">
   <summary>Click to TODO</summary>
 
 - [ ] ChatLLM 应用
-  - [x] 接入非结构化文档（已支持 md、pdf、docx、txt 文件格式）
-  - [ ] 搜索引擎与本地网页接入
-  - [ ] 结构化数据接入（如 csv、Excel、SQL 等）
-  - [ ] 知识图谱/图数据库接入
-  - [ ] 增加 ANN 后端，ES/RedisSearch【确保生产高可用】
-  - [ ] 增加多级缓存缓存
+    - [x] 接入非结构化文档（已支持 md、pdf、docx、txt 文件格式）
+    - [ ] 搜索引擎与本地网页接入
+    - [ ] 结构化数据接入（如 csv、Excel、SQL 等）
+    - [ ] 知识图谱/图数据库接入
+    - [ ] 增加 ANN 后端，ES/RedisSearch【确保生产高可用】
+    - [ ] 增加多级缓存缓存
 
 - [ ] 多路召回
-  - [ ] 问
-    - [ ] 标量匹配
-    - [x] 多种向量化，向量匹配
-    - [ ] 增加相似问，换几个问法
-    - [ ] 高置信度直接返回答案【匹配标准问】
-  - [ ] 答
-    - [ ] 高置信度篇章
-    - [ ] 增加上下文信息
-    - [ ] 增加夸篇章信息
-    - [ ] 增加召回信息的相似信息
-    - [ ] 提前生成标准问，匹配问
-    - [ ] 拒绝推断
+    - [ ] 问
+        - [ ] 标量匹配
+        - [x] 多种向量化，向量匹配
+        - [ ] 增加相似问，换几个问法
+        - [ ] 高置信度直接返回答案【匹配标准问】
+    - [ ] 答
+        - [ ] 高置信度篇章
+        - [ ] 增加上下文信息
+        - [ ] 增加夸篇章信息
+        - [ ] 增加召回信息的相似信息
+        - [ ] 提前生成标准问，匹配问
+        - [ ] 拒绝推断
 
 
 - [ ] 增加更多 LLM 模型支持
-  - [x] [THUDM/chatglm-6b](https://huggingface.co/THUDM/chatglm-6b)
-  - [ ] [THUDM/chatglm-6b-int8](https://huggingface.co/THUDM/chatglm-6b-int8)
-  - [ ] [THUDM/chatglm-6b-int4](https://huggingface.co/THUDM/chatglm-6b-int4)
-  - [ ] [THUDM/chatglm-6b-int4-qe](https://huggingface.co/THUDM/chatglm-6b-int4-qe)
-  - [ ] [ClueAI/ChatYuan-large-v2](https://huggingface.co/ClueAI/ChatYuan-large-v2)
+    - [x] [THUDM/chatglm-6b](https://huggingface.co/THUDM/chatglm-6b)
+    - [ ] [THUDM/chatglm-6b-int8](https://huggingface.co/THUDM/chatglm-6b-int8)
+    - [ ] [THUDM/chatglm-6b-int4](https://huggingface.co/THUDM/chatglm-6b-int4)
+    - [ ] [THUDM/chatglm-6b-int4-qe](https://huggingface.co/THUDM/chatglm-6b-int4-qe)
+    - [ ] [ClueAI/ChatYuan-large-v2](https://huggingface.co/ClueAI/ChatYuan-large-v2)
 - [ ] 增加更多 Embedding 模型支持
-  - [x] [nghuyong/ernie-3.0-nano-zh](https://huggingface.co/nghuyong/ernie-3.0-nano-zh)
-  - [x] [nghuyong/ernie-3.0-base-zh](https://huggingface.co/nghuyong/ernie-3.0-base-zh)
-  - [x] [shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese)
-  - [x] [GanymedeNil/text2vec-large-chinese](https://huggingface.co/GanymedeNil/text2vec-large-chinese)
+    - [x] [nghuyong/ernie-3.0-nano-zh](https://huggingface.co/nghuyong/ernie-3.0-nano-zh)
+    - [x] [nghuyong/ernie-3.0-base-zh](https://huggingface.co/nghuyong/ernie-3.0-base-zh)
+    - [x] [shibing624/text2vec-base-chinese](https://huggingface.co/shibing624/text2vec-base-chinese)
+    - [x] [GanymedeNil/text2vec-large-chinese](https://huggingface.co/GanymedeNil/text2vec-large-chinese)
 - [x] 增加一键启动 webui
-  - [x] 利用 streamlit 实现 ChatPDF，一键启动 `chatllm-run webui --name chatpdf`
-  - [ ] 利用 gradio 实现 Web UI DEMO
-  - [ ] 添加输出内容及错误提示
-  - [ ] 引用标注
-  - [ ] 增加知识库管理
-    - [ ] 选择知识库开始问答
-    - [ ] 上传文件/文件夹至知识库
-    - [ ] 删除知识库中文件
+    - [x] 利用 streamlit 实现 ChatPDF，一键启动 `chatllm-run webui --name chatpdf`
+    - [ ] 利用 gradio 实现 Web UI DEMO
+    - [ ] 添加输出内容及错误提示
+    - [ ] 引用标注
+    - [ ] 增加知识库管理
+        - [ ] 选择知识库开始问答
+        - [ ] 上传文件/文件夹至知识库
+        - [ ] 删除知识库中文件
 - [ ] 增加 API 支持
-  - [x] 利用 Fastapi/Flask/Grpc 实现流式接口 `chatllm-run flask-api --model_name_or_path <MODEL_PATH> --host 127.0.0.1 --port 8000`
-  - [ ] 前后端分离，实现调用 API 的 Web UI Demo
+    - [x] 利用 Fastapi/Flask/Grpc
+      实现流式接口 `chatllm-run openai <本地模型地址> --host 127.0.0.1 --port 8000`
+    - [ ] 前后端分离，实现调用 API 的 Web UI Demo
+
+</details>
 
 ## 交流群
-![二维码]()
+<div align=center>
+<img src="data/imgs/群.png" alt="群" width="250" height="400">
+</div>
 
-</details>
+> 若二维码失效加微信拉群 313303303
```

### Comparing `ChatLLM-2023.5.4.12.7.23/chatllm/_his/FaissANN.py` & `chatllm-2023.6.1.12.39.20/chatllm/_his/FaissANN.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.12.7.23/chatllm/_his/_chatllm.py` & `chatllm-2023.6.1.12.39.20/chatllm/_his/_chatllm.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.12.7.23/chatllm/_his/_qa.py` & `chatllm-2023.6.1.12.39.20/chatllm/_his/_qa.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.12.7.23/chatllm/applications/Question2Answer.py` & `chatllm-2023.6.1.12.39.20/chatllm/applications/Question2Answer.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.12.7.23/chatllm/applications/chatann.py` & `chatllm-2023.6.1.12.39.20/chatllm/applications/chatann.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,21 +4,19 @@
 # @File         : ann4qa
 # @Time         : 2023/4/24 18:10
 # @Author       : betterme
 # @WeChat       : meutils
 # @Software     : PyCharm
 # @Description  :
 
+
 from meutils.pipe import *
+from meutils.np_utils import cosine_topk
 from chatllm.applications import ChatBase
 
-from docarray import DocList, BaseDoc
-from docarray.typing import TorchTensor
-from docarray.utils.find import find
-from docarray.utils.filter import filter_docs
 from sentence_transformers import SentenceTransformer
 
 
 class ChatANN(ChatBase):
 
     def __init__(self, backend='in_memory', encode_model="nghuyong/ernie-3.0-nano-zh", **kwargs):
         """
@@ -28,61 +26,53 @@
             "nghuyong/ernie-3.0-nano-zh"
             "shibing624/text2vec-base-chinese"
             "GanymedeNil/text2vec-large-chinese"
         :param kwargs:
         """
         super().__init__(**kwargs)
         self.backend = backend
-
         self.encode = SentenceTransformer(encode_model).encode  # 加缓存，可重新set
 
         # create index
         self.index = None
 
         # 召回结果df
         self.recall = pd.DataFrame({'id': [], 'text': [], 'score': []})
 
     def qa(self, query, topk=3, threshold=0.66, **kwargs):
         df = self.find(query, topk, threshold)
-        if len(df) == 0:
-            logger.warning('召回内容为空!!!')
-
-        knowledge_base = '\n'.join(df.text)
-        return self._qa(query, knowledge_base, **kwargs)
+        if len(df):
+            knowledge_base = '\n'.join(df.text)
+            return self._qa(query, knowledge_base, **kwargs)
+        logger.error('召回内容为空!!!')
 
     def find(self, query, topk=5, threshold=0.66):  # 返回df
-        v = self.encode(query)  # np
+        v = self.encode([query])  # ndim=2
 
         if self.backend == 'in_memory':
-            r = self.index.find(TorchTensor(v), topk)
+            idxs, scores = cosine_topk(v, np.array(self.index.embedding.tolist()), topk)
+
             self.recall = (
-                # r.documents.to_dataframe() # bug
-                pd.DataFrame(json.loads(r.documents.to_json()))
-                .assign(score=r.scores)
+                self.index.iloc[idxs, :]
+                .assign(score=scores)
                 .query(f'score > {threshold}')
             )
 
         return self.recall
 
-    def create_index(self, texts):
-        tensors = self.encode(texts, show_progress_bar=True, convert_to_numpy=False)
-
-        class Document(BaseDoc):
-            text: str
-            embedding: TorchTensor
-
-        self.index = DocList[Document]()
-        self.index.extend([Document(text=text, embedding=tensor) for text, tensor in zip(texts, tensors)])
-        self.index.find = lambda query, topk=3: find(self.index, query, limit=topk, search_field='embedding')
+    def create_index(self, texts):  # todo：增加 encode_model参数
+        embeddings = self.encode(texts, show_progress_bar=True)
+        if self.backend == 'in_memory':
+            self.index = pd.DataFrame({'text': texts, 'embedding': embeddings.tolist()})
 
         return self.index
 
 
 if __name__ == '__main__':
 
     qa = ChatANN(encode_model="nghuyong/ernie-3.0-nano-zh")
-    qa.load_llm4chat(model_name_or_path="/Users/betterme/PycharmProjects/AI/CHAT_MODEL/chatglm")
+    qa.load_llm(model_name_or_path="/CHAT_MODEL/chatglm-6b")
     qa.create_index(['周杰伦'] * 10)
 
-    for i, _ in qa(query='有几个周杰伦'):
-        pass
+    for i in qa(query='有几个周杰伦'):
+        print(i, end='')
     print(qa.recall)
```

### Comparing `ChatLLM-2023.5.4.12.7.23/chatllm/applications/chatbase.py` & `chatllm-2023.6.1.12.39.20/chatllm/applications/__chatbase.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,22 +32,24 @@
     def qa(self, query, knowledge_base='', **kwargs):
         """重写"""
         return self._qa(query, knowledge_base, **kwargs)
 
     def set_chat_kwargs(self, **kwargs):
         self.chat_func = partial(self.chat_func, **kwargs)
 
-    @clear_cuda_cache
+    @clear_cuda_cache(bins=3)
     def _qa(self, query, knowledge_base='', role='', max_turns=1):
         self.role = role or os.environ.get('LLM_ROLE', '')
         self.knowledge_base = str(knowledge_base).strip()
         if self.knowledge_base:
-            query = self.prompt_template.format(context=self.knowledge_base, question=query, role=self.role).strip()
+            query = self.prompt_template.format(context=self.knowledge_base, question=query, role=' ').strip()  # 无角色扮演
         else:
-            query = """{role}\n{question}""".format(question=query, role=self.role).strip()  # 简化模版
+            query = """{role}\n{question}""".format(question=query, role=self.role).strip()  # 知识库为空则转通用回答
+
+        self.query = query
 
         _history = self.history[-(max_turns - 1):] if max_turns > 1 else []
         result = self.chat_func(query=query, history=_history)
 
         if isinstance(result, types.GeneratorType):
             return self._stream(result)
         else:
@@ -61,16 +63,21 @@
         bar = tqdm(result, ascii=True)  # ncols
         for response, history in bar:
             bar.set_description(response)
             yield response, history
         # self.history_ = history  # 历史所有
         self.history += [[None, response]]  # 置空知识
 
-    def load_llm4chat(self, model_name_or_path="THUDM/chatglm-6b", device=DEVICE, stream=True, **kwargs):
-        self.chat_func = load_llm4chat(model_name_or_path, device, stream, **kwargs)
+    def load_llm4chat(self, model_name_or_path="THUDM/chatglm-6b", device=DEVICE, **kwargs):  # 废弃
+        self.chat_func = load_llm4chat(model_name_or_path, device, **kwargs)
+
+    def load_llm(self, model_name_or_path="THUDM/chatglm-6b", device=DEVICE, return_history=False, **kwargs):
+        from chatllm.llms import load_llm4chat
+        self.chat_func = load_llm4chat(model_name_or_path, device=device, **kwargs)
+        self.chat_func = partial(self.chat_func, return_history=return_history)
 
     def run_serving(self, host='127.0.0.1', port=8000, path='/'):
         from flask import Flask, Response, jsonify, request
 
         app = Flask(__name__)
 
         def gen(**input):
@@ -89,13 +96,13 @@
         app.run(host=host, port=port, debug=False)
 
 
 if __name__ == '__main__':
     from chatllm.applications import ChatBase
 
     qa = ChatBase()
-    qa.load_llm4chat(model_name_or_path="/Users/betterme/PycharmProjects/AI/CHAT_MODEL/chatglm")
+    qa.load_llm4chat(model_name_or_path="/CHAT_MODEL/chatglm-6b")
 
     # list(qa(query='你是谁', knowledge_base=''))
     # list(qa(query='你是谁', knowledge_base='周杰伦是傻子', role=' '))
 
     qa.run_serving()
```

### Comparing `ChatLLM-2023.5.4.12.7.23/chatllm/applications/chatcrawler.py` & `chatllm-2023.6.1.12.39.20/chatllm/applications/chatcrawler.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,11 +29,11 @@
 
 
 if __name__ == '__main__':
     from chatllm.utils import MODEL_PATH
 
 
     qa = Crawler4QA()
-    qa.load_llm4chat(MODEL_PATH)
+    qa.load_llm(MODEL_PATH)
 
     list(qa(query='提取人名'))
```

### Comparing `ChatLLM-2023.5.4.12.7.23/chatllm/applications/chatpdf.py` & `chatllm-2023.6.1.12.39.20/chatllm/applications/chatpdf.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     # bytes_array = Path(filename).read_bytes()
     # texts = extract_text(bytes_array)
     # texts = textsplitter(texts)
     # print(texts)
     from chatllm.applications.chatpdf import ChatPDF
 
     qa = ChatPDF(encode_model='nghuyong/ernie-3.0-nano-zh')  # 自动建索引
+    qa.load_llm(model_name_or_path='/CHAT_MODEL/chatglm-6b', device='cpu')
     qa.create_index('../../data/财报.pdf')
-    qa.load_llm4chat(model_name_or_path='/Users/betterme/PycharmProjects/AI/CHAT_MODEL/chatglm', device='cpu')
 
-    list(qa(query='东北证券主营业务', topk=1, threshold=0.8))
+    for i in qa(query='东北证券主营业务', topk=1, threshold=0.8):
+        print(i, end='')
 
     # 召回结果
     print(qa.recall)
```

### Comparing `ChatLLM-2023.5.4.12.7.23/chatllm/applications/chatwhoosh.py` & `chatllm-2023.6.1.12.39.20/chatllm/applications/chatwhoosh.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # @Project      : AI.  @by PyCharm
 # @File         : chatwhoosh
 # @Time         : 2023/4/26 19:04
 # @Author       : betterme
 # @WeChat       : meutils
 # @Software     : PyCharm
 # @Description  :
-import pandas as pd
 
 from meutils.pipe import *
 from meutils.hash_utils import md5
 from meutils.easy_search.es import EasySearch
 
 from chatllm.applications import ChatBase
```

### Comparing `ChatLLM-2023.5.4.12.7.23/chatllm/chatyuan.py` & `chatllm-2023.6.1.12.39.20/chatllm/chatyuan.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.12.7.23/chatllm/clis/cli.py` & `chatllm-2023.6.1.12.39.20/chatllm/clis/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,51 +2,55 @@
 # -*- coding: utf-8 -*-
 # @Project      : MeUtils.
 # @File         : __init__.py
 # @Time         : 2021/1/31 10:20 下午
 # @Author       : yuanjie
 # @Email        : meutils@qq.com
 # @Software     : PyCharm
-# @Description  : python meutils/clis/__init__.py
-import os
+# @Description  :
 
 from meutils.pipe import *
 
 cli = typer.Typer(name="ChatLLM CLI")
 
 if LOCAL_HOST.startswith('10.219'):
-    MODEL_PATH = "/Users/betterme/PycharmProjects/AI/CHAT_MODEL/chatglm"
+    MODEL_PATH = "/CHAT_MODEL/chatglm-6b"
 
 
 def f(a=1, **kw):
     print(a)
     print(kw)
 
 
 @cli.command(help="help")  # help会覆盖docstring
-def clitest(**kwargs): # 不支持 **kwargs
+def clitest(**kwargs):  # 不支持 **kwargs
     f(**kwargs)
 
 
 @cli.command()  # help会覆盖docstring
 def webui(name: str = 'chatpdf', port=8501):
     """
         chatllm-run webui --name chatpdf --port 8501
     """
     main = get_resolve_path(f'../webui/{name}.py', __file__)
     os.system(f'streamlit run {main} --server.port {port}')
 
 
 @cli.command()  # help会覆盖docstring
-def flask_api(model_name_or_path=None, host='127.0.0.1', port=8000, path='/'):
+def openapi(llm_model, host='127.0.0.1', port: int = 8000, debug='1'):
     """
-        chatllm-run flask-api --model_name_or_path <MODEL_PATH> --host 127.0.0.1 --port 8000
+        chatllm-run openapi <MODEL_PATH> --host 127.0.0.1 --port 8000
     """
-    from chatllm.applications import ChatBase
 
-    qa = ChatBase()
-    qa.load_llm4chat(model_name_or_path or MODEL_PATH)
-    qa.run_serving(host, port, path)
+    os.environ['LLM_MODEL'] = llm_model
+    os.environ['DEBUG'] = debug
+
+    from meutils.serving.fastapi import App
+    from chatllm.api.routes.api import router
+
+    app = App()
+    app.include_router(router)
+    app.run(host=host, port=port)
 
 
 if __name__ == '__main__':
     cli()
```

### Comparing `ChatLLM-2023.5.4.12.7.23/chatllm/embedding.py` & `chatllm-2023.6.1.12.39.20/chatllm/embedding.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.12.7.23/chatllm/utils/common.py` & `chatllm-2023.6.1.12.39.20/chatllm/utils/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,58 +3,62 @@
 # @Project      : AI.  @by PyCharm
 # @File         : utils
 # @Time         : 2023/4/20 12:50
 # @Author       : betterme
 # @WeChat       : meutils
 # @Software     : PyCharm
 # @Description  :
+
 import torch
 from transformers import AutoTokenizer, AutoModel
 
 from meutils.pipe import *
 from chatllm.utils.gpu_utils import load_chatglm_on_gpus
 
 DEVICE = (
-    os.environ['DEVICE'] if 'DEVICE' in os.environ
+    os.getenv('DEVICE') if 'DEVICE' in os.environ
     else "cuda" if torch.cuda.is_available()
     else "mps" if torch.backends.mps.is_available()
     else "cpu"
 )
+
 if LOCAL_HOST.startswith('10.219'):
-    MODEL_PATH = "/Users/betterme/PycharmProjects/AI/CHAT_MODEL/chatglm"
+    MODEL_PATH = "/CHAT_MODEL/chatglm-6b"
 else:
     MODEL_PATH = "THUDM/chatglm-6b"
 
+xgroup = Pipe(lambda ls, step=3, overlap_rate=0: [ls[max(idx - int(step * overlap_rate), 0): idx + step] for idx in
+                                                  range(0, len(ls), step)])
 
-# todo 多卡 https://github.com/THUDM/ChatGLM-6B#%E5%A4%9A%E5%8D%A1%E9%83%A8%E7%BD%B2
 
 def textsplitter(text, chunk_size=512, overlap_rate=0.2, sep=''):  # 简单粗暴
     return text.lower().split() | xjoin(sep) | xgroup(chunk_size, overlap_rate)
 
 
 def load_llm(model_name_or_path="THUDM/chatglm-6b", device=DEVICE, num_gpus=2, **kwargs):
     model = AutoModel.from_pretrained(model_name_or_path, trust_remote_code=True)
     tokenizer = AutoTokenizer.from_pretrained(model_name_or_path, trust_remote_code=True)
 
     if torch.cuda.is_available() and device.lower().startswith("cuda"):
-        num_gpus = min(1, num_gpus, torch.cuda.device_count())
+        num_gpus = min(num_gpus, torch.cuda.device_count())
 
         if num_gpus == 1:  # 单卡
             model = model.half().cuda()
             # model.transformer.prefix_encoder.float()
         elif 'chatglm' in model_name_or_path:  # chatglm多卡
             model = load_chatglm_on_gpus(model_name_or_path, num_gpus)
+            logger.info('多卡加载模型')
 
     else:
         model = model.float().to(device)
 
     return model.eval(), tokenizer
 
 
-def load_llm4chat(model_name_or_path="THUDM/chatglm-6b", device=DEVICE, num_gpus=1, stream=True, **kwargs):
+def load_llm4chat(model_name_or_path="THUDM/chatglm-6b", device=DEVICE, num_gpus=2, stream=True, **kwargs):
     model, tokenizer = load_llm(model_name_or_path, device, num_gpus, **kwargs)
     if stream and hasattr(model, 'stream_chat'):
         return partial(model.stream_chat, tokenizer=tokenizer)  # 可以在每一次生成清GPU
     else:
         return partial(model.chat, tokenizer=tokenizer)
```

### Comparing `ChatLLM-2023.5.4.12.7.23/chatllm/utils/gpu_utils.py` & `chatllm-2023.6.1.12.39.20/chatllm/utils/gpu_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 import os
 from typing import Dict, Tuple, Union, Optional
 
 from torch.nn import Module
 from transformers import AutoModel
 
+
 # os.environ["CUDA_VISIBLE_DEVICES"] = "0,1,2"
 
 def auto_configure_device_map(num_gpus: int) -> Dict[str, int]:
     # transformer.word_embeddings 占用1层
     # transformer.final_layernorm 和 lm_head 占用1层
     # transformer.layers 占用 28 层
     # 总共30层分配到num_gpus张卡上
@@ -44,37 +45,21 @@
         used += 1
 
     return device_map
 
 
 def load_chatglm_on_gpus(checkpoint_path: Union[str, os.PathLike], num_gpus: int = 2,
                          device_map: Optional[Dict[str, int]] = None, **kwargs) -> Module:
+    """https://github.com/THUDM/ChatGLM-6B#%E5%A4%9A%E5%8D%A1%E9%83%A8%E7%BD%B2"""
     if num_gpus < 2 and device_map is None:
         model = AutoModel.from_pretrained(checkpoint_path, trust_remote_code=True, **kwargs).half().cuda()
     else:
         from accelerate import dispatch_model
 
         model = AutoModel.from_pretrained(checkpoint_path, trust_remote_code=True, **kwargs).half()
 
         if device_map is None:
             device_map = auto_configure_device_map(num_gpus)
 
         model = dispatch_model(model, device_map=device_map)
 
     return model
-
-
-# def load_chatglm_on_gpus(model, model_name_or_path, num_gpus=2, checkpoint="chatglm_checkpoint"):
-#     """https://github.com/THUDM/ChatGLM-6B/issues/200"""
-#     from accelerate import load_checkpoint_and_dispatch
-#
-#     device_map = auto_configure_device_map(num_gpus)
-#     try:
-#         model = load_checkpoint_and_dispatch(model, model_name_or_path, device_map=device_map, offload_folder="offload",
-#                                              offload_state_dict=True).half()
-#     except ValueError:
-#         logger.info('多卡加载，第一次需要缓存模型')
-#         model.save_pretrained(checkpoint, max_shard_size='2GB')
-#         model = load_checkpoint_and_dispatch(model, checkpoint, device_map=device_map,
-#                                              offload_folder="offload", offload_state_dict=True).half()
-#     return model
-
```

### Comparing `ChatLLM-2023.5.4.12.7.23/chatllm/webui/chatbase.py` & `chatllm-2023.6.1.12.39.20/chatllm/webui/chatbase.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 st.set_page_config('🔥ChatLLM', layout='centered', initial_sidebar_state='collapsed')
 
 
 @st.cache_resource
 def get_chat_func():
     chat_func = load_llm4chat(
-        model_name_or_path="/Users/betterme/PycharmProjects/AI/CHAT_MODEL/chatglm"
+        model_name_or_path="/CHAT_MODEL/chatglm-6b"
     )
     return chat_func
 
 
 chat_func = get_chat_func()
 
 qa = ChatBase(chat_func=chat_func)
```

### Comparing `ChatLLM-2023.5.4.12.7.23/chatllm/webui/chatpdf.py` & `chatllm-2023.6.1.12.39.20/chatllm/webui/chatpdf.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,85 +6,89 @@
 # @Author       : betterme
 # @WeChat       : meutils
 # @Software     : PyCharm
 # @Description  :
 
 import streamlit as st
 from meutils.pipe import *
-from appzoo.streamlit_app.utils import display_pdf, reply4input
+from meutils.serving.st_utils import display_pdf, st_chat, set_config
 
 from chatllm.applications.chatpdf import ChatPDF
 
 st.set_page_config(page_title='🔥ChatPDF', layout='wide', initial_sidebar_state='collapsed')
 
 
 ################################################################################################################
 class Conf(BaseConfig):
     encode_model = 'nghuyong/ernie-3.0-nano-zh'
-    llm = "THUDM/chatglm-6b"  # /Users/betterme/PycharmProjects/AI/CHAT_MODEL/chatglm
+    llm = "THUDM/chatglm-6b"  # /Users/betterme/PycharmProjects/AI/CHAT_MODEL/chatglm-6b
     cachedir = 'pdf_cache'
 
     topk: int = 3
     threshold: float = 0.66
 
 
 conf = Conf()
+conf = set_config(conf)
 
-for k, v in conf:  # 更新配置
-    v = type(v)(st.sidebar.text_input(label=k.upper(), value=v))
-    setattr(conf, k, v)
+
+################################################################################################################
 
 
 @st.cache_resource()
-def qa4pdf(encode_model, model_name_or_path):
+def qa4pdf(encode_model, model_name_or_path, cachedir):
     qa = ChatPDF(encode_model=encode_model)
-    qa.load_llm4chat(model_name_or_path=model_name_or_path)
+    # qa.encode = disk_cache(qa.encode, location=cachedir)  # 缓存
+    qa.load_llm(model_name_or_path=model_name_or_path, num_gpus=2)
+    qa.create_index = lru_cache()(qa.create_index)
+
     return qa
 
 
-################################################################################################################
+def reply_func(query):
+    response = ''
+    for _ in qa(query=query, topk=conf.topk, threshold=conf.threshold):
+        response += _
+        yield response
+
 
-tabs = st.tabs(['ChatPDF', 'PDF文件预览'])
+if st.session_state.get('init'):
 
-file = st.sidebar.file_uploader("上传PDF", type=['pdf'])
-bytes_array = ''
-if file:
-    bytes_array = file.read()
-    base64_pdf = base64.b64encode(bytes_array).decode('utf-8')
+    tabs = st.tabs(['ChatPDF', 'PDF文件预览'])
+
+    with tabs[0]:
+        file = st.file_uploader("上传PDF", type=['pdf'])
+        bytes_array = ''
+        try:
+            qa = qa4pdf(conf.encode_model, conf.llm, conf.cachedir)
+        except Exception as e:
+            st.warning('启动前选择正确的参数进行初始化')
+            st.error(e)
+
+        if file:
+            bytes_array = file.read()
+            with st.spinner("构建知识库：文本向量化"):
+                qa.create_index(bytes_array)
+
+            base64_pdf = base64.b64encode(bytes_array).decode('utf-8')
+
+            container = st.container()  # 占位符
+            text = st.text_area(label="用户输入", height=100, placeholder="请在这儿输入您的问题")
+
+            if st.button("发送", key="predict"):
+                with st.spinner("🤔 AI 正在思考，请稍等..."):
+                    history = st.session_state.get('state')
+                    st.session_state["state"] = st_chat(
+                        text, history, container=container,
+                        previous_messages=['请上传需要分析的PDF，我将为你解答'],
+                        reply_func=reply_func,
+                    )
+
+            with st.expander('点击可查看被召回的知识'):
+                st.dataframe(qa.recall.drop(labels='embedding', axis=1, errors='ignore'))
+                # st.dataframe(qa.recall)
 
     with tabs[1]:
         if bytes_array:
             display_pdf(base64_pdf)
         else:
             st.warning('### 请先上传PDF')
-################################################################################################################
-try:
-    qa = qa4pdf(conf.encode_model, conf.llm)
-    with st.spinner("构建知识库：文本向量化"):
-        disk_cache(location=conf.cachedir)(qa.create_index)(bytes_array)
-except Exception as e:
-    st.warning('启动前选择正确的参数进行初始化')
-    st.error(e)
-
-
-################################################################################################################
-def reply_func(query):
-    for response, _ in qa(query=query, topk=conf.topk, threshold=conf.threshold):
-        yield response
-
-
-with tabs[0]:
-    if file:
-        container = st.container()  # 占位符
-        text = st.text_area(label="用户输入", height=100, placeholder="请在这儿输入您的问题")
-
-        if st.button("发送", key="predict"):
-            with st.spinner("🤔 AI 正在思考，请稍等..."):
-                history = st.session_state.get('state')
-                st.session_state["state"] = reply4input(
-                    text, history, container=container,
-                    previous_messages=['请上传需要分析的PDF，我将为你解答'],
-                    reply_func=reply_func,
-                )
-
-        with st.expander('点击可查看被召回的知识'):
-            st.dataframe(qa.recall)
```

### Comparing `ChatLLM-2023.5.4.12.7.23/chatllm/webui/gradio_ui.py` & `chatllm-2023.6.1.12.39.20/chatllm/webui/gradio_ui.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.12.7.23/chatllm/webui/nice_ui.py` & `chatllm-2023.6.1.12.39.20/chatllm/webui/nice_ui.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.12.7.23/data/imgs/LLM.drawio.png` & `chatllm-2023.6.1.12.39.20/data/imgs/LLM.drawio.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.12.7.23/data/imgs/LLM.png` & `chatllm-2023.6.1.12.39.20/data/imgs/LLM.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.12.7.23/data/imgs/chatpdf.gif` & `chatllm-2023.6.1.12.39.20/data/imgs/chatpdf.gif`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.12.7.23/data/imgs/chatpdf_ann_df.png` & `chatllm-2023.6.1.12.39.20/data/imgs/chatpdf_ann_df.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.12.7.23/data/imgs/role.png` & `chatllm-2023.6.1.12.39.20/data/imgs/role.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.12.7.23/data/医/500种中药现代研究.txt` & `chatllm-2023.6.1.12.39.20/data/医/500种中药现代研究.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.12.7.23/data/医/古今医统大全.txt` & `chatllm-2023.6.1.12.39.20/data/医/古今医统大全.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.12.7.23/data/姚明.txt` & `chatllm-2023.6.1.12.39.20/data/姚明.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.12.7.23/data/王治郅.txt` & `chatllm-2023.6.1.12.39.20/data/王治郅.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.12.7.23/data/科比.txt` & `chatllm-2023.6.1.12.39.20/data/科比.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.12.7.23/data/财报.pdf` & `chatllm-2023.6.1.12.39.20/data/财报.pdf`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.12.7.23/docs/Makefile` & `chatllm-2023.6.1.12.39.20/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.12.7.23/docs/conf.py` & `chatllm-2023.6.1.12.39.20/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.12.7.23/docs/make.bat` & `chatllm-2023.6.1.12.39.20/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.12.7.23/setup.py` & `chatllm-2023.6.1.12.39.20/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,51 +8,47 @@
 
 DIR = Path(__file__).resolve().parent
 version = time.strftime("%Y.%m.%d.%H.%M.%S", time.localtime())
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
-with open('HISTORY.rst') as history_file:
-    history = history_file.read()
 
 get_requirements = lambda p='requirements.txt': pd.read_csv(p, comment='#', names=['name']).name.tolist()
 extras_require = {v.name.split('_')[1][:-4]: get_requirements(v) for v in DIR.glob('requirements_*')}
 extras_require['all'] = list(set(sum(extras_require.values(), [])))
 
 setup(
     author="yuanjie",
     author_email='313303303@qq.com',
     python_requires='>=3.7',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
     ],
     description="Create a Python package.",
     entry_points={
         'console_scripts': [
             'chatllm-run=chatllm.clis.cli:cli'
         ],
     },
     setup_requires=["pandas"],
     install_requires=get_requirements(),
     extras_require=extras_require,  # pip install -U meutils\[all\]
     license="MIT license",
-    long_description=readme + '\n\n' + history,
+    long_description=readme,
     long_description_content_type="text/markdown",
     include_package_data=True,
     keywords='chatllm',
-    name='ChatLLM',
-    # name='ChatSearch', # 抢占包
+    name='chatllm',
+    # name='llms', # 抢占包
 
     packages=find_packages(include=['chatllm', 'chatllm.*']),
 
     test_suite='tests',
     url='https://github.com/yuanjie-ai/ChatLLM',
     version=version,  # '0.0.0',
     zip_safe=False,
```

### Comparing `ChatLLM-2023.5.4.12.7.23/tests/test_llm4gpt.py` & `chatllm-2023.6.1.12.39.20/tests/test_llm4gpt.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.12.7.23/tests/内存型.ipynb` & `chatllm-2023.6.1.12.39.20/tests/内存型.ipynb`

 * *Files identical despite different names*

