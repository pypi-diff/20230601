# Comparing `tmp/unstructured-0.7.0.tar.gz` & `tmp/unstructured-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unstructured-0.7.0.tar", last modified: Wed May 31 20:15:02 2023, max compression
+gzip compressed data, was "unstructured-0.7.1.tar", last modified: Thu Jun  1 20:53:22 2023, max compression
```

## Comparing `unstructured-0.7.0.tar` & `unstructured-0.7.1.tar`

### file list

```diff
@@ -1,127 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:15:02.575583 unstructured-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-05-31 20:14:52.000000 unstructured-0.7.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-31 20:14:52.000000 unstructured-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17916 2023-05-31 20:15:02.575583 unstructured-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14528 2023-05-31 20:14:52.000000 unstructured-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:15:02.563583 unstructured-0.7.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-31 20:14:52.000000 unstructured-0.7.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-31 20:14:52.000000 unstructured-0.7.0/requirements/huggingface.in
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-31 20:14:52.000000 unstructured-0.7.0/requirements/ingest-azure.in
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-31 20:14:52.000000 unstructured-0.7.0/requirements/ingest-discord.in
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-31 20:14:52.000000 unstructured-0.7.0/requirements/ingest-github.in
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-31 20:14:52.000000 unstructured-0.7.0/requirements/ingest-gitlab.in
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-31 20:14:52.000000 unstructured-0.7.0/requirements/ingest-google-drive.in
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-31 20:14:52.000000 unstructured-0.7.0/requirements/ingest-reddit.in
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-31 20:14:52.000000 unstructured-0.7.0/requirements/ingest-s3.in
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-31 20:14:52.000000 unstructured-0.7.0/requirements/ingest-slack.in
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-31 20:14:52.000000 unstructured-0.7.0/requirements/ingest-wikipedia.in
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-31 20:14:52.000000 unstructured-0.7.0/requirements/local-inference.in
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-31 20:15:02.575583 unstructured-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-31 20:14:52.000000 unstructured-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:15:02.563583 unstructured-0.7.0/test_unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 20:14:52.000000 unstructured-0.7.0/test_unstructured/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:15:02.563583 unstructured-0.7.0/test_unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 20:14:52.000000 unstructured-0.7.0/test_unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-31 20:14:52.000000 unstructured-0.7.0/test_unstructured/nlp/mock_nltk.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-31 20:14:52.000000 unstructured-0.7.0/test_unstructured/nlp/test_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-31 20:14:52.000000 unstructured-0.7.0/test_unstructured/nlp/test_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-05-31 20:14:52.000000 unstructured-0.7.0/test_unstructured/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:15:02.563583 unstructured-0.7.0/unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:15:02.563583 unstructured-0.7.0/unstructured/cleaners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/cleaners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/cleaners/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/cleaners/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/cleaners/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:15:02.563583 unstructured-0.7.0/unstructured/documents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/documents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/documents/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/documents/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/documents/email_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    15004 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/documents/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/documents/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:15:02.563583 unstructured-0.7.0/unstructured/file_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/file_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/file_utils/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/file_utils/exploration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/file_utils/file_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    12533 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/file_utils/filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/file_utils/google_filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/file_utils/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:15:02.563583 unstructured-0.7.0/unstructured/ingest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/ingest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:15:02.567583 unstructured-0.7.0/unstructured/ingest/connector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/ingest/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/ingest/connector/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/ingest/connector/biomed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/ingest/connector/discord.py
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/ingest/connector/fsspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/ingest/connector/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/ingest/connector/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/ingest/connector/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/ingest/connector/google_drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/ingest/connector/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/ingest/connector/reddit.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/ingest/connector/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/ingest/connector/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/ingest/connector/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:15:02.567583 unstructured-0.7.0/unstructured/ingest/doc_processor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/ingest/doc_processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/ingest/doc_processor/generalized.py
--rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/ingest/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/ingest/logger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24164 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/ingest/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:15:02.567583 unstructured-0.7.0/unstructured/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:15:02.571583 unstructured-0.7.0/unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/nlp/english-words.txt
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/nlp/english_words.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/nlp/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/nlp/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/nlp/tokenize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:15:02.571583 unstructured-0.7.0/unstructured/partition/
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/partition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/partition/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8925 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/partition/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/partition/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/partition/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/partition/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/partition/docx.py
--rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/partition/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/partition/epub.py
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/partition/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/partition/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/partition/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/partition/md.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/partition/msg.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/partition/odt.py
--rw-r--r--   0 runner    (1001) docker     (123)    13004 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/partition/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/partition/ppt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/partition/pptx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/partition/rtf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/partition/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/partition/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/partition/text_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/partition/xlsx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/partition/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:15:02.575583 unstructured-0.7.0/unstructured/staging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/staging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/staging/argilla.py
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/staging/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/staging/baseplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/staging/datasaur.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/staging/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/staging/label_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/staging/label_studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/staging/prodigy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-31 20:14:52.000000 unstructured-0.7.0/unstructured/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:15:02.563583 unstructured-0.7.0/unstructured.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17916 2023-05-31 20:15:02.000000 unstructured-0.7.0/unstructured.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-05-31 20:15:02.000000 unstructured-0.7.0/unstructured.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 20:15:02.000000 unstructured-0.7.0/unstructured.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-31 20:15:02.000000 unstructured-0.7.0/unstructured.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-31 20:15:02.000000 unstructured-0.7.0/unstructured.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-31 20:15:02.000000 unstructured-0.7.0/unstructured.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:22.964075 unstructured-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-06-01 20:53:14.000000 unstructured-0.7.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-01 20:53:14.000000 unstructured-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17917 2023-06-01 20:53:22.964075 unstructured-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14529 2023-06-01 20:53:14.000000 unstructured-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:22.952075 unstructured-0.7.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-01 20:53:14.000000 unstructured-0.7.1/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-01 20:53:14.000000 unstructured-0.7.1/requirements/huggingface.in
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-01 20:53:14.000000 unstructured-0.7.1/requirements/ingest-azure.in
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-01 20:53:14.000000 unstructured-0.7.1/requirements/ingest-discord.in
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-01 20:53:14.000000 unstructured-0.7.1/requirements/ingest-github.in
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-01 20:53:14.000000 unstructured-0.7.1/requirements/ingest-gitlab.in
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-01 20:53:14.000000 unstructured-0.7.1/requirements/ingest-google-drive.in
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-01 20:53:14.000000 unstructured-0.7.1/requirements/ingest-reddit.in
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-01 20:53:14.000000 unstructured-0.7.1/requirements/ingest-s3.in
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-01 20:53:14.000000 unstructured-0.7.1/requirements/ingest-slack.in
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-01 20:53:14.000000 unstructured-0.7.1/requirements/ingest-wikipedia.in
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-01 20:53:14.000000 unstructured-0.7.1/requirements/local-inference.in
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-01 20:53:22.968075 unstructured-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-06-01 20:53:14.000000 unstructured-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:22.952075 unstructured-0.7.1/test_unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:14.000000 unstructured-0.7.1/test_unstructured/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:22.952075 unstructured-0.7.1/test_unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:14.000000 unstructured-0.7.1/test_unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-01 20:53:14.000000 unstructured-0.7.1/test_unstructured/nlp/mock_nltk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-01 20:53:14.000000 unstructured-0.7.1/test_unstructured/nlp/test_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-06-01 20:53:14.000000 unstructured-0.7.1/test_unstructured/nlp/test_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-01 20:53:14.000000 unstructured-0.7.1/test_unstructured/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:22.952075 unstructured-0.7.1/unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:22.956075 unstructured-0.7.1/unstructured/cleaners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/cleaners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/cleaners/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/cleaners/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/cleaners/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:22.956075 unstructured-0.7.1/unstructured/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/documents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/documents/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/documents/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/documents/email_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15004 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/documents/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/documents/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:22.956075 unstructured-0.7.1/unstructured/file_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/file_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/file_utils/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/file_utils/exploration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/file_utils/file_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12533 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/file_utils/filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/file_utils/google_filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/file_utils/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:22.956075 unstructured-0.7.1/unstructured/ingest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/ingest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:22.956075 unstructured-0.7.1/unstructured/ingest/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/ingest/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/ingest/connector/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/ingest/connector/biomed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/ingest/connector/discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/ingest/connector/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/ingest/connector/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/ingest/connector/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/ingest/connector/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/ingest/connector/google_drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/ingest/connector/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/ingest/connector/reddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/ingest/connector/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/ingest/connector/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/ingest/connector/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:22.956075 unstructured-0.7.1/unstructured/ingest/doc_processor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/ingest/doc_processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/ingest/doc_processor/generalized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/ingest/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/ingest/logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24164 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/ingest/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:22.956075 unstructured-0.7.1/unstructured/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:22.964075 unstructured-0.7.1/unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/nlp/english-words.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/nlp/english_words.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/nlp/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/nlp/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/nlp/tokenize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:22.964075 unstructured-0.7.1/unstructured/partition/
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/partition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/partition/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8925 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/partition/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/partition/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/partition/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/partition/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/partition/docx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/partition/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/partition/epub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/partition/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/partition/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/partition/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/partition/md.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/partition/msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/partition/odt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13004 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/partition/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/partition/ppt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/partition/pptx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/partition/rtf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/partition/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/partition/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/partition/text_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/partition/xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/partition/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:22.964075 unstructured-0.7.1/unstructured/staging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/staging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/staging/argilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/staging/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/staging/baseplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/staging/datasaur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/staging/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/staging/label_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/staging/label_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/staging/prodigy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/staging/weaviate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-01 20:53:14.000000 unstructured-0.7.1/unstructured/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:53:22.952075 unstructured-0.7.1/unstructured.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17917 2023-06-01 20:53:22.000000 unstructured-0.7.1/unstructured.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-06-01 20:53:22.000000 unstructured-0.7.1/unstructured.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 20:53:22.000000 unstructured-0.7.1/unstructured.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-01 20:53:22.000000 unstructured-0.7.1/unstructured.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-01 20:53:22.000000 unstructured-0.7.1/unstructured.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-01 20:53:22.000000 unstructured-0.7.1/unstructured.egg-info/top_level.txt
```

### Comparing `unstructured-0.7.0/LICENSE.md` & `unstructured-0.7.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/PKG-INFO` & `unstructured-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.7.0
+Version: 0.7.1
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
@@ -102,15 +102,15 @@
         | Excel Documents (`.xlsx`/`.xls`) | `partition_xlsx` | N/A | Yes | None |
         | HTML Pages (`.html`) | `partition_html` | N/A | No | Encoding; Include Page Breaks |
         | Images (`.png`/`.jpg`) | `partition_image` | `"auto"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy |
         | Markdown (`.md`) | `partitin_md` | N/A | No | Include Page Breaks |
         | Open Office Documents (`.odt`) | `partition_odt` | N/A | Yes | None |
         | PDFs (`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy |
         | Plain Text (`.txt`) | `partition_text` | N/A | No | Encoding, Paragraph Grouper |
-        | Power Points (`.ppt`) | `partition_ppt` | N/A | No | Include Page Breaks |
+        | Power Points (`.ppt`) | `partition_ppt` | N/A | Yes | Include Page Breaks |
         | Power Points (`.pptx`) | `partition_pptx` | N/A | Yes | Include Page Breaks |
         | Rich Text Files (`.rtf`) | `partition_rtf` | N/A | No | Include Page Breaks |
         | Word Documents (`.doc`) | `partition_doc` | N/A | Yes | None |
         | Word Documents (`.docx`) | `partition_docx` | N/A | Yes | None |
         | XML Documents (`.xml`) | `partition_xml` | N/A | No | Encoding; XML Keep Tags |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.7.0 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.7.1 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
@@ -65,15 +65,15 @@
 `partition_image` | `"auto"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding;
 Include Page Breaks; Infer Table Structure; OCR Languages, Strategy | |
 Markdown (`.md`) | `partitin_md` | N/A | No | Include Page Breaks | | Open
 Office Documents (`.odt`) | `partition_odt` | N/A | Yes | None | | PDFs
 (`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes
 | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy
 | | Plain Text (`.txt`) | `partition_text` | N/A | No | Encoding, Paragraph
-Grouper | | Power Points (`.ppt`) | `partition_ppt` | N/A | No | Include Page
+Grouper | | Power Points (`.ppt`) | `partition_ppt` | N/A | Yes | Include Page
 Breaks | | Power Points (`.pptx`) | `partition_pptx` | N/A | Yes | Include Page
 Breaks | | Rich Text Files (`.rtf`) | `partition_rtf` | N/A | No | Include Page
 Breaks | | Word Documents (`.doc`) | `partition_doc` | N/A | Yes | None | |
 Word Documents (`.docx`) | `partition_docx` | N/A | Yes | None | | XML
 Documents (`.xml`) | `partition_xml` | N/A | No | Encoding; XML Keep Tags | ##
 :dizzy: Instructions for using the docker image The following instructions are
 intended to help you get up and running using Docker to interact with
```

### Comparing `unstructured-0.7.0/README.md` & `unstructured-0.7.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 | Excel Documents (`.xlsx`/`.xls`) | `partition_xlsx` | N/A | Yes | None |
 | HTML Pages (`.html`) | `partition_html` | N/A | No | Encoding; Include Page Breaks |
 | Images (`.png`/`.jpg`) | `partition_image` | `"auto"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy |
 | Markdown (`.md`) | `partitin_md` | N/A | No | Include Page Breaks |
 | Open Office Documents (`.odt`) | `partition_odt` | N/A | Yes | None |
 | PDFs (`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy |
 | Plain Text (`.txt`) | `partition_text` | N/A | No | Encoding, Paragraph Grouper |
-| Power Points (`.ppt`) | `partition_ppt` | N/A | No | Include Page Breaks |
+| Power Points (`.ppt`) | `partition_ppt` | N/A | Yes | Include Page Breaks |
 | Power Points (`.pptx`) | `partition_pptx` | N/A | Yes | Include Page Breaks |
 | Rich Text Files (`.rtf`) | `partition_rtf` | N/A | No | Include Page Breaks |
 | Word Documents (`.doc`) | `partition_doc` | N/A | Yes | None |
 | Word Documents (`.docx`) | `partition_docx` | N/A | Yes | None |
 | XML Documents (`.xml`) | `partition_xml` | N/A | No | Encoding; XML Keep Tags |
```

#### html2text {}

```diff
@@ -61,15 +61,15 @@
 `partition_image` | `"auto"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding;
 Include Page Breaks; Infer Table Structure; OCR Languages, Strategy | |
 Markdown (`.md`) | `partitin_md` | N/A | No | Include Page Breaks | | Open
 Office Documents (`.odt`) | `partition_odt` | N/A | Yes | None | | PDFs
 (`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes
 | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy
 | | Plain Text (`.txt`) | `partition_text` | N/A | No | Encoding, Paragraph
-Grouper | | Power Points (`.ppt`) | `partition_ppt` | N/A | No | Include Page
+Grouper | | Power Points (`.ppt`) | `partition_ppt` | N/A | Yes | Include Page
 Breaks | | Power Points (`.pptx`) | `partition_pptx` | N/A | Yes | Include Page
 Breaks | | Rich Text Files (`.rtf`) | `partition_rtf` | N/A | No | Include Page
 Breaks | | Word Documents (`.doc`) | `partition_doc` | N/A | Yes | None | |
 Word Documents (`.docx`) | `partition_docx` | N/A | Yes | None | | XML
 Documents (`.xml`) | `partition_xml` | N/A | No | Encoding; XML Keep Tags | ##
 :dizzy: Instructions for using the docker image The following instructions are
 intended to help you get up and running using Docker to interact with
```

### Comparing `unstructured-0.7.0/setup.py` & `unstructured-0.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/test_unstructured/nlp/mock_nltk.py` & `unstructured-0.7.1/test_unstructured/nlp/mock_nltk.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/test_unstructured/nlp/test_tokenize.py` & `unstructured-0.7.1/test_unstructured/nlp/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/test_unstructured/test_utils.py` & `unstructured-0.7.1/test_unstructured/test_utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/cleaners/core.py` & `unstructured-0.7.1/unstructured/cleaners/core.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/cleaners/extract.py` & `unstructured-0.7.1/unstructured/cleaners/extract.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/cleaners/translate.py` & `unstructured-0.7.1/unstructured/cleaners/translate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/documents/base.py` & `unstructured-0.7.1/unstructured/documents/base.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/documents/elements.py` & `unstructured-0.7.1/unstructured/documents/elements.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/documents/email_elements.py` & `unstructured-0.7.1/unstructured/documents/email_elements.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/documents/html.py` & `unstructured-0.7.1/unstructured/documents/html.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/documents/xml.py` & `unstructured-0.7.1/unstructured/documents/xml.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/file_utils/encoding.py` & `unstructured-0.7.1/unstructured/file_utils/encoding.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/file_utils/exploration.py` & `unstructured-0.7.1/unstructured/file_utils/exploration.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/file_utils/file_conversion.py` & `unstructured-0.7.1/unstructured/file_utils/file_conversion.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/file_utils/filetype.py` & `unstructured-0.7.1/unstructured/file_utils/filetype.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/file_utils/metadata.py` & `unstructured-0.7.1/unstructured/file_utils/metadata.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/ingest/connector/azure.py` & `unstructured-0.7.1/unstructured/ingest/connector/azure.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/ingest/connector/biomed.py` & `unstructured-0.7.1/unstructured/ingest/connector/biomed.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/ingest/connector/discord.py` & `unstructured-0.7.1/unstructured/ingest/connector/discord.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/ingest/connector/fsspec.py` & `unstructured-0.7.1/unstructured/ingest/connector/fsspec.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/ingest/connector/git.py` & `unstructured-0.7.1/unstructured/ingest/connector/git.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/ingest/connector/github.py` & `unstructured-0.7.1/unstructured/ingest/connector/github.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/ingest/connector/gitlab.py` & `unstructured-0.7.1/unstructured/ingest/connector/gitlab.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/ingest/connector/google_drive.py` & `unstructured-0.7.1/unstructured/ingest/connector/google_drive.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/ingest/connector/local.py` & `unstructured-0.7.1/unstructured/ingest/connector/local.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/ingest/connector/reddit.py` & `unstructured-0.7.1/unstructured/ingest/connector/reddit.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/ingest/connector/s3.py` & `unstructured-0.7.1/unstructured/ingest/connector/s3.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/ingest/connector/slack.py` & `unstructured-0.7.1/unstructured/ingest/connector/slack.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/ingest/connector/wikipedia.py` & `unstructured-0.7.1/unstructured/ingest/connector/wikipedia.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/ingest/doc_processor/generalized.py` & `unstructured-0.7.1/unstructured/ingest/doc_processor/generalized.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/ingest/interfaces.py` & `unstructured-0.7.1/unstructured/ingest/interfaces.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/ingest/main.py` & `unstructured-0.7.1/unstructured/ingest/main.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/nlp/english-words.txt` & `unstructured-0.7.1/unstructured/nlp/english-words.txt`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/nlp/english_words.py` & `unstructured-0.7.1/unstructured/nlp/english_words.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/nlp/patterns.py` & `unstructured-0.7.1/unstructured/nlp/patterns.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/nlp/tokenize.py` & `unstructured-0.7.1/unstructured/nlp/tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/partition/__init__.py` & `unstructured-0.7.1/unstructured/partition/__init__.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/partition/api.py` & `unstructured-0.7.1/unstructured/partition/api.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/partition/auto.py` & `unstructured-0.7.1/unstructured/partition/auto.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/partition/common.py` & `unstructured-0.7.1/unstructured/partition/common.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/partition/csv.py` & `unstructured-0.7.1/unstructured/partition/csv.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/partition/doc.py` & `unstructured-0.7.1/unstructured/partition/doc.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/partition/docx.py` & `unstructured-0.7.1/unstructured/partition/docx.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/partition/email.py` & `unstructured-0.7.1/unstructured/partition/email.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/partition/epub.py` & `unstructured-0.7.1/unstructured/partition/epub.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/partition/html.py` & `unstructured-0.7.1/unstructured/partition/html.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/partition/image.py` & `unstructured-0.7.1/unstructured/partition/image.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/partition/json.py` & `unstructured-0.7.1/unstructured/partition/json.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/partition/md.py` & `unstructured-0.7.1/unstructured/partition/md.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/partition/msg.py` & `unstructured-0.7.1/unstructured/partition/msg.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/partition/odt.py` & `unstructured-0.7.1/unstructured/partition/odt.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/partition/pdf.py` & `unstructured-0.7.1/unstructured/partition/pdf.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/partition/ppt.py` & `unstructured-0.7.1/unstructured/partition/ppt.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/partition/pptx.py` & `unstructured-0.7.1/unstructured/partition/pptx.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/partition/rtf.py` & `unstructured-0.7.1/unstructured/partition/rtf.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/partition/strategies.py` & `unstructured-0.7.1/unstructured/partition/strategies.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/partition/text.py` & `unstructured-0.7.1/unstructured/partition/text.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/partition/text_type.py` & `unstructured-0.7.1/unstructured/partition/text_type.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/partition/xlsx.py` & `unstructured-0.7.1/unstructured/partition/xlsx.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/partition/xml.py` & `unstructured-0.7.1/unstructured/partition/xml.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/staging/argilla.py` & `unstructured-0.7.1/unstructured/staging/argilla.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/staging/base.py` & `unstructured-0.7.1/unstructured/staging/base.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/staging/baseplate.py` & `unstructured-0.7.1/unstructured/staging/baseplate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/staging/datasaur.py` & `unstructured-0.7.1/unstructured/staging/datasaur.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/staging/huggingface.py` & `unstructured-0.7.1/unstructured/staging/huggingface.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/staging/label_box.py` & `unstructured-0.7.1/unstructured/staging/label_box.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/staging/label_studio.py` & `unstructured-0.7.1/unstructured/staging/label_studio.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/staging/prodigy.py` & `unstructured-0.7.1/unstructured/staging/prodigy.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured/utils.py` & `unstructured-0.7.1/unstructured/utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.0/unstructured.egg-info/PKG-INFO` & `unstructured-0.7.1/unstructured.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.7.0
+Version: 0.7.1
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
@@ -102,15 +102,15 @@
         | Excel Documents (`.xlsx`/`.xls`) | `partition_xlsx` | N/A | Yes | None |
         | HTML Pages (`.html`) | `partition_html` | N/A | No | Encoding; Include Page Breaks |
         | Images (`.png`/`.jpg`) | `partition_image` | `"auto"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy |
         | Markdown (`.md`) | `partitin_md` | N/A | No | Include Page Breaks |
         | Open Office Documents (`.odt`) | `partition_odt` | N/A | Yes | None |
         | PDFs (`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy |
         | Plain Text (`.txt`) | `partition_text` | N/A | No | Encoding, Paragraph Grouper |
-        | Power Points (`.ppt`) | `partition_ppt` | N/A | No | Include Page Breaks |
+        | Power Points (`.ppt`) | `partition_ppt` | N/A | Yes | Include Page Breaks |
         | Power Points (`.pptx`) | `partition_pptx` | N/A | Yes | Include Page Breaks |
         | Rich Text Files (`.rtf`) | `partition_rtf` | N/A | No | Include Page Breaks |
         | Word Documents (`.doc`) | `partition_doc` | N/A | Yes | None |
         | Word Documents (`.docx`) | `partition_docx` | N/A | Yes | None |
         | XML Documents (`.xml`) | `partition_xml` | N/A | No | Encoding; XML Keep Tags |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.7.0 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.7.1 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
@@ -65,15 +65,15 @@
 `partition_image` | `"auto"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding;
 Include Page Breaks; Infer Table Structure; OCR Languages, Strategy | |
 Markdown (`.md`) | `partitin_md` | N/A | No | Include Page Breaks | | Open
 Office Documents (`.odt`) | `partition_odt` | N/A | Yes | None | | PDFs
 (`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes
 | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy
 | | Plain Text (`.txt`) | `partition_text` | N/A | No | Encoding, Paragraph
-Grouper | | Power Points (`.ppt`) | `partition_ppt` | N/A | No | Include Page
+Grouper | | Power Points (`.ppt`) | `partition_ppt` | N/A | Yes | Include Page
 Breaks | | Power Points (`.pptx`) | `partition_pptx` | N/A | Yes | Include Page
 Breaks | | Rich Text Files (`.rtf`) | `partition_rtf` | N/A | No | Include Page
 Breaks | | Word Documents (`.doc`) | `partition_doc` | N/A | Yes | None | |
 Word Documents (`.docx`) | `partition_docx` | N/A | Yes | None | | XML
 Documents (`.xml`) | `partition_xml` | N/A | No | Encoding; XML Keep Tags | ##
 :dizzy: Instructions for using the docker image The following instructions are
 intended to help you get up and running using Docker to interact with
```

### Comparing `unstructured-0.7.0/unstructured.egg-info/SOURCES.txt` & `unstructured-0.7.1/unstructured.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -103,8 +103,9 @@
 unstructured/staging/argilla.py
 unstructured/staging/base.py
 unstructured/staging/baseplate.py
 unstructured/staging/datasaur.py
 unstructured/staging/huggingface.py
 unstructured/staging/label_box.py
 unstructured/staging/label_studio.py
-unstructured/staging/prodigy.py
+unstructured/staging/prodigy.py
+unstructured/staging/weaviate.py
```

