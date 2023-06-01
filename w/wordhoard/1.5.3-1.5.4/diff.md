# Comparing `tmp/wordhoard-1.5.3.tar.gz` & `tmp/wordhoard-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wordhoard-1.5.3.tar", last modified: Tue Mar 21 15:37:05 2023, max compression
+gzip compressed data, was "wordhoard-1.5.4.tar", last modified: Thu Jun  1 14:22:53 2023, max compression
```

## Comparing `wordhoard-1.5.3.tar` & `wordhoard-1.5.4.tar`

### file list

```diff
@@ -1,69 +1,70 @@
-drwxr-xr-x   0 bumgarner   (501) staff       (20)        0 2023-03-21 15:37:05.484107 wordhoard-1.5.3/
--rw-r--r--   0 bumgarner   (501) staff       (20)     1071 2020-10-20 22:26:04.000000 wordhoard-1.5.3/LICENSE
--rw-r--r--   0 bumgarner   (501) staff       (20)       73 2020-10-23 19:09:16.000000 wordhoard-1.5.3/MANIFEST.in
--rw-r--r--   0 bumgarner   (501) staff       (20)     5231 2023-03-21 15:37:05.483866 wordhoard-1.5.3/PKG-INFO
--rw-r--r--   0 bumgarner   (501) staff       (20)       38 2023-03-21 15:37:05.484179 wordhoard-1.5.3/setup.cfg
--rw-r--r--   0 bumgarner   (501) staff       (20)     2522 2023-03-21 15:23:59.000000 wordhoard-1.5.3/setup.py
-drwxr-xr-x   0 bumgarner   (501) staff       (20)        0 2023-03-21 15:37:05.469274 wordhoard-1.5.3/wordhoard/
--rw-r--r--   0 bumgarner   (501) staff       (20)      828 2023-03-21 14:56:48.000000 wordhoard-1.5.3/wordhoard/__init__.py
-drwxr-xr-x   0 bumgarner   (501) staff       (20)        0 2023-03-21 15:37:05.472872 wordhoard-1.5.3/wordhoard/__pycache__/
--rw-r--r--   0 bumgarner   (501) staff       (20)     1106 2023-03-21 14:37:01.000000 wordhoard-1.5.3/wordhoard/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 bumgarner   (501) staff       (20)    13558 2023-03-20 19:33:37.000000 wordhoard-1.5.3/wordhoard/__pycache__/antonyms.cpython-39.pyc
--rw-r--r--   0 bumgarner   (501) staff       (20)    18393 2023-03-20 19:33:37.000000 wordhoard-1.5.3/wordhoard/__pycache__/dictionary.cpython-39.pyc
--rw-r--r--   0 bumgarner   (501) staff       (20)     5301 2023-03-21 14:37:01.000000 wordhoard-1.5.3/wordhoard/__pycache__/homophones.cpython-39.pyc
--rw-r--r--   0 bumgarner   (501) staff       (20)    10659 2023-03-20 19:33:37.000000 wordhoard-1.5.3/wordhoard/__pycache__/hypernyms.cpython-39.pyc
--rw-r--r--   0 bumgarner   (501) staff       (20)    11292 2023-03-20 19:33:37.000000 wordhoard-1.5.3/wordhoard/__pycache__/hyponyms.cpython-39.pyc
--rw-r--r--   0 bumgarner   (501) staff       (20)    21711 2023-03-20 19:33:37.000000 wordhoard-1.5.3/wordhoard/__pycache__/synonyms.cpython-39.pyc
--rw-r--r--   0 bumgarner   (501) staff       (20)    19770 2023-03-21 14:56:48.000000 wordhoard-1.5.3/wordhoard/antonyms.py
--rw-r--r--   0 bumgarner   (501) staff       (20)    29639 2023-03-21 14:56:48.000000 wordhoard-1.5.3/wordhoard/dictionary.py
-drwxr-xr-x   0 bumgarner   (501) staff       (20)        0 2023-03-21 15:37:05.474140 wordhoard-1.5.3/wordhoard/files/
--rw-r--r--   0 bumgarner   (501) staff       (20)        1 2020-10-24 00:22:43.000000 wordhoard-1.5.3/wordhoard/files/__init__.py
--rw-r--r--   0 bumgarner   (501) staff       (20)    29162 2021-06-09 14:56:46.000000 wordhoard-1.5.3/wordhoard/files/common_english_homophones.pkl
--rw-r--r--   0 bumgarner   (501) staff       (20)    35141 2021-09-12 12:42:32.000000 wordhoard-1.5.3/wordhoard/files/common_user_agents.pkl
--rw-r--r--   0 bumgarner   (501) staff       (20)   636545 2021-06-10 00:27:56.000000 wordhoard-1.5.3/wordhoard/files/no_homophones_english.pkl
--rw-r--r--   0 bumgarner   (501) staff       (20)     6443 2023-03-21 14:56:48.000000 wordhoard-1.5.3/wordhoard/homophones.py
--rw-r--r--   0 bumgarner   (501) staff       (20)    16961 2023-03-21 14:56:48.000000 wordhoard-1.5.3/wordhoard/hypernyms.py
--rw-r--r--   0 bumgarner   (501) staff       (20)    17245 2023-03-21 14:56:48.000000 wordhoard-1.5.3/wordhoard/hyponyms.py
--rw-r--r--   0 bumgarner   (501) staff       (20)    33916 2023-03-21 14:56:48.000000 wordhoard-1.5.3/wordhoard/synonyms.py
-drwxr-xr-x   0 bumgarner   (501) staff       (20)        0 2023-03-21 15:37:05.479233 wordhoard-1.5.3/wordhoard/utilities/
--rw-r--r--   0 bumgarner   (501) staff       (20)        1 2020-10-24 00:22:43.000000 wordhoard-1.5.3/wordhoard/utilities/__init__.py
-drwxr-xr-x   0 bumgarner   (501) staff       (20)        0 2023-03-21 15:37:05.483560 wordhoard-1.5.3/wordhoard/utilities/__pycache__/
--rw-r--r--   0 bumgarner   (501) staff       (20)      177 2021-06-12 12:23:57.000000 wordhoard-1.5.3/wordhoard/utilities/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 bumgarner   (501) staff       (20)     3198 2023-03-19 14:46:10.000000 wordhoard-1.5.3/wordhoard/utilities/__pycache__/caching.cpython-39.pyc
--rw-r--r--   0 bumgarner   (501) staff       (20)     3143 2022-03-05 18:28:10.000000 wordhoard-1.5.3/wordhoard/utilities/__pycache__/captcha_checker.cpython-39.pyc
--rw-r--r--   0 bumgarner   (501) staff       (20)     2122 2023-03-04 14:25:28.000000 wordhoard-1.5.3/wordhoard/utilities/__pycache__/cleansing.cpython-39.pyc
--rw-r--r--   0 bumgarner   (501) staff       (20)     2242 2023-02-25 19:31:27.000000 wordhoard-1.5.3/wordhoard/utilities/__pycache__/cloudflare_bypass.cpython-39.pyc
--rw-r--r--   0 bumgarner   (501) staff       (20)     3435 2023-03-08 15:41:26.000000 wordhoard-1.5.3/wordhoard/utilities/__pycache__/cloudflare_checker.cpython-39.pyc
--rw-r--r--   0 bumgarner   (501) staff       (20)     1024 2023-02-18 18:50:54.000000 wordhoard-1.5.3/wordhoard/utilities/__pycache__/colorized_text.cpython-39.pyc
--rw-r--r--   0 bumgarner   (501) staff       (20)     7860 2023-03-02 15:25:13.000000 wordhoard-1.5.3/wordhoard/utilities/__pycache__/deep_translator.cpython-39.pyc
--rw-r--r--   0 bumgarner   (501) staff       (20)      879 2023-02-10 15:52:21.000000 wordhoard-1.5.3/wordhoard/utilities/__pycache__/email_address_verification.cpython-39.pyc
--rw-r--r--   0 bumgarner   (501) staff       (20)     2519 2023-03-02 15:16:31.000000 wordhoard-1.5.3/wordhoard/utilities/__pycache__/exceptions.cpython-39.pyc
--rw-r--r--   0 bumgarner   (501) staff       (20)     7783 2023-02-12 13:42:58.000000 wordhoard-1.5.3/wordhoard/utilities/__pycache__/google_translator.cpython-39.pyc
--rw-r--r--   0 bumgarner   (501) staff       (20)    11237 2023-02-11 15:17:46.000000 wordhoard-1.5.3/wordhoard/utilities/__pycache__/mymemory_translator.cpython-39.pyc
--rw-r--r--   0 bumgarner   (501) staff       (20)     7425 2023-03-18 14:29:02.000000 wordhoard-1.5.3/wordhoard/utilities/__pycache__/request_html.cpython-39.pyc
--rw-r--r--   0 bumgarner   (501) staff       (20)     7081 2023-03-02 15:16:31.000000 wordhoard-1.5.3/wordhoard/utilities/__pycache__/translator_languages.cpython-39.pyc
--rw-r--r--   0 bumgarner   (501) staff       (20)     3088 2023-03-04 14:25:28.000000 wordhoard-1.5.3/wordhoard/utilities/__pycache__/user_agents.cpython-39.pyc
--rw-r--r--   0 bumgarner   (501) staff       (20)     1037 2023-03-04 15:22:37.000000 wordhoard-1.5.3/wordhoard/utilities/__pycache__/word_verification.cpython-39.pyc
--rw-r--r--   0 bumgarner   (501) staff       (20)      812 2023-02-28 16:23:56.000000 wordhoard-1.5.3/wordhoard/utilities/__pycache__/wordhoard_logger.cpython-39.pyc
--rw-r--r--   0 bumgarner   (501) staff       (20)     5462 2023-03-21 14:56:48.000000 wordhoard-1.5.3/wordhoard/utilities/caching.py
--rw-r--r--   0 bumgarner   (501) staff       (20)     4169 2023-03-21 14:56:48.000000 wordhoard-1.5.3/wordhoard/utilities/captcha_checker.py
--rw-r--r--   0 bumgarner   (501) staff       (20)     2226 2023-03-21 14:56:48.000000 wordhoard-1.5.3/wordhoard/utilities/cleansing.py
--rw-r--r--   0 bumgarner   (501) staff       (20)     3044 2023-03-21 14:56:48.000000 wordhoard-1.5.3/wordhoard/utilities/cloudflare_bypass.py
--rw-r--r--   0 bumgarner   (501) staff       (20)     4244 2023-03-21 14:56:48.000000 wordhoard-1.5.3/wordhoard/utilities/cloudflare_checker.py
--rw-r--r--   0 bumgarner   (501) staff       (20)     1537 2023-03-21 14:56:48.000000 wordhoard-1.5.3/wordhoard/utilities/colorized_text.py
--rw-r--r--   0 bumgarner   (501) staff       (20)    14340 2023-03-21 14:56:48.000000 wordhoard-1.5.3/wordhoard/utilities/deep_translator.py
--rw-r--r--   0 bumgarner   (501) staff       (20)     1712 2023-03-21 14:56:48.000000 wordhoard-1.5.3/wordhoard/utilities/email_address_verification.py
--rw-r--r--   0 bumgarner   (501) staff       (20)     2507 2023-02-13 14:13:15.000000 wordhoard-1.5.3/wordhoard/utilities/exceptions.py
--rw-r--r--   0 bumgarner   (501) staff       (20)    15158 2023-03-21 14:56:48.000000 wordhoard-1.5.3/wordhoard/utilities/google_translator.py
--rw-r--r--   0 bumgarner   (501) staff       (20)    18208 2023-03-21 14:56:48.000000 wordhoard-1.5.3/wordhoard/utilities/mymemory_translator.py
--rw-r--r--   0 bumgarner   (501) staff       (20)    14077 2023-03-21 14:56:48.000000 wordhoard-1.5.3/wordhoard/utilities/request_html.py
--rw-r--r--   0 bumgarner   (501) staff       (20)    18164 2023-03-21 14:56:48.000000 wordhoard-1.5.3/wordhoard/utilities/translator_languages.py
--rw-r--r--   0 bumgarner   (501) staff       (20)     4297 2023-03-21 14:56:48.000000 wordhoard-1.5.3/wordhoard/utilities/user_agents.py
--rw-r--r--   0 bumgarner   (501) staff       (20)     1873 2023-03-21 14:56:48.000000 wordhoard-1.5.3/wordhoard/utilities/word_verification.py
--rw-r--r--   0 bumgarner   (501) staff       (20)     1623 2023-03-21 14:56:48.000000 wordhoard-1.5.3/wordhoard/utilities/wordhoard_logger.py
-drwxr-xr-x   0 bumgarner   (501) staff       (20)        0 2023-03-21 15:37:05.470851 wordhoard-1.5.3/wordhoard.egg-info/
--rw-r--r--   0 bumgarner   (501) staff       (20)     5231 2023-03-21 15:37:05.000000 wordhoard-1.5.3/wordhoard.egg-info/PKG-INFO
--rw-r--r--   0 bumgarner   (501) staff       (20)     2559 2023-03-21 15:37:05.000000 wordhoard-1.5.3/wordhoard.egg-info/SOURCES.txt
--rw-r--r--   0 bumgarner   (501) staff       (20)        1 2023-03-21 15:37:05.000000 wordhoard-1.5.3/wordhoard.egg-info/dependency_links.txt
--rw-r--r--   0 bumgarner   (501) staff       (20)      258 2023-03-21 15:37:05.000000 wordhoard-1.5.3/wordhoard.egg-info/requires.txt
--rw-r--r--   0 bumgarner   (501) staff       (20)       10 2023-03-21 15:37:05.000000 wordhoard-1.5.3/wordhoard.egg-info/top_level.txt
+drwxr-xr-x   0 bumgarner   (501) staff       (20)        0 2023-06-01 14:22:53.567582 wordhoard-1.5.4/
+-rw-r--r--   0 bumgarner   (501) staff       (20)     1071 2020-10-20 22:26:04.000000 wordhoard-1.5.4/LICENSE
+-rw-r--r--   0 bumgarner   (501) staff       (20)       73 2020-10-23 19:09:16.000000 wordhoard-1.5.4/MANIFEST.in
+-rw-r--r--   0 bumgarner   (501) staff       (20)     5282 2023-06-01 14:22:53.567229 wordhoard-1.5.4/PKG-INFO
+-rw-r--r--   0 bumgarner   (501) staff       (20)       38 2023-06-01 14:22:53.567684 wordhoard-1.5.4/setup.cfg
+-rw-r--r--   0 bumgarner   (501) staff       (20)     2580 2023-06-01 14:21:27.000000 wordhoard-1.5.4/setup.py
+drwxr-xr-x   0 bumgarner   (501) staff       (20)        0 2023-06-01 14:22:53.543229 wordhoard-1.5.4/wordhoard/
+-rw-r--r--   0 bumgarner   (501) staff       (20)    10244 2023-06-01 14:09:29.000000 wordhoard-1.5.4/wordhoard/.DS_Store
+-rw-r--r--   0 bumgarner   (501) staff       (20)      828 2023-05-31 17:55:08.000000 wordhoard-1.5.4/wordhoard/__init__.py
+drwxr-xr-x   0 bumgarner   (501) staff       (20)        0 2023-06-01 14:22:53.548631 wordhoard-1.5.4/wordhoard/__pycache__/
+-rw-r--r--   0 bumgarner   (501) staff       (20)     1106 2023-03-21 14:37:01.000000 wordhoard-1.5.4/wordhoard/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 bumgarner   (501) staff       (20)    13558 2023-03-20 19:33:37.000000 wordhoard-1.5.4/wordhoard/__pycache__/antonyms.cpython-39.pyc
+-rw-r--r--   0 bumgarner   (501) staff       (20)    18393 2023-03-20 19:33:37.000000 wordhoard-1.5.4/wordhoard/__pycache__/dictionary.cpython-39.pyc
+-rw-r--r--   0 bumgarner   (501) staff       (20)     5301 2023-03-21 14:37:01.000000 wordhoard-1.5.4/wordhoard/__pycache__/homophones.cpython-39.pyc
+-rw-r--r--   0 bumgarner   (501) staff       (20)    10659 2023-03-20 19:33:37.000000 wordhoard-1.5.4/wordhoard/__pycache__/hypernyms.cpython-39.pyc
+-rw-r--r--   0 bumgarner   (501) staff       (20)    11292 2023-03-20 19:33:37.000000 wordhoard-1.5.4/wordhoard/__pycache__/hyponyms.cpython-39.pyc
+-rw-r--r--   0 bumgarner   (501) staff       (20)    21711 2023-03-20 19:33:37.000000 wordhoard-1.5.4/wordhoard/__pycache__/synonyms.cpython-39.pyc
+-rw-r--r--   0 bumgarner   (501) staff       (20)    19670 2023-05-31 19:42:24.000000 wordhoard-1.5.4/wordhoard/antonyms.py
+-rw-r--r--   0 bumgarner   (501) staff       (20)    29507 2023-05-31 19:42:24.000000 wordhoard-1.5.4/wordhoard/dictionary.py
+drwxr-xr-x   0 bumgarner   (501) staff       (20)        0 2023-06-01 14:22:53.550023 wordhoard-1.5.4/wordhoard/files/
+-rw-r--r--   0 bumgarner   (501) staff       (20)        1 2020-10-24 00:22:43.000000 wordhoard-1.5.4/wordhoard/files/__init__.py
+-rw-r--r--   0 bumgarner   (501) staff       (20)    29162 2021-06-09 14:56:46.000000 wordhoard-1.5.4/wordhoard/files/common_english_homophones.pkl
+-rw-r--r--   0 bumgarner   (501) staff       (20)    35141 2021-09-12 12:42:32.000000 wordhoard-1.5.4/wordhoard/files/common_user_agents.pkl
+-rw-r--r--   0 bumgarner   (501) staff       (20)   636545 2021-06-10 00:27:56.000000 wordhoard-1.5.4/wordhoard/files/no_homophones_english.pkl
+-rw-r--r--   0 bumgarner   (501) staff       (20)     6478 2023-05-31 14:55:32.000000 wordhoard-1.5.4/wordhoard/homophones.py
+-rw-r--r--   0 bumgarner   (501) staff       (20)    16773 2023-05-31 18:07:54.000000 wordhoard-1.5.4/wordhoard/hypernyms.py
+-rw-r--r--   0 bumgarner   (501) staff       (20)    17057 2023-05-31 18:07:54.000000 wordhoard-1.5.4/wordhoard/hyponyms.py
+-rw-r--r--   0 bumgarner   (501) staff       (20)    33769 2023-06-01 13:11:41.000000 wordhoard-1.5.4/wordhoard/synonyms.py
+drwxr-xr-x   0 bumgarner   (501) staff       (20)        0 2023-06-01 14:22:53.554828 wordhoard-1.5.4/wordhoard/utilities/
+-rw-r--r--   0 bumgarner   (501) staff       (20)        1 2020-10-24 00:22:43.000000 wordhoard-1.5.4/wordhoard/utilities/__init__.py
+drwxr-xr-x   0 bumgarner   (501) staff       (20)        0 2023-06-01 14:22:53.566415 wordhoard-1.5.4/wordhoard/utilities/__pycache__/
+-rw-r--r--   0 bumgarner   (501) staff       (20)      177 2021-06-12 12:23:57.000000 wordhoard-1.5.4/wordhoard/utilities/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 bumgarner   (501) staff       (20)     3198 2023-03-19 14:46:10.000000 wordhoard-1.5.4/wordhoard/utilities/__pycache__/caching.cpython-39.pyc
+-rw-r--r--   0 bumgarner   (501) staff       (20)     3143 2022-03-05 18:28:10.000000 wordhoard-1.5.4/wordhoard/utilities/__pycache__/captcha_checker.cpython-39.pyc
+-rw-r--r--   0 bumgarner   (501) staff       (20)     2122 2023-03-04 14:25:28.000000 wordhoard-1.5.4/wordhoard/utilities/__pycache__/cleansing.cpython-39.pyc
+-rw-r--r--   0 bumgarner   (501) staff       (20)     2242 2023-02-25 19:31:27.000000 wordhoard-1.5.4/wordhoard/utilities/__pycache__/cloudflare_bypass.cpython-39.pyc
+-rw-r--r--   0 bumgarner   (501) staff       (20)     3435 2023-03-08 15:41:26.000000 wordhoard-1.5.4/wordhoard/utilities/__pycache__/cloudflare_checker.cpython-39.pyc
+-rw-r--r--   0 bumgarner   (501) staff       (20)     1024 2023-02-18 18:50:54.000000 wordhoard-1.5.4/wordhoard/utilities/__pycache__/colorized_text.cpython-39.pyc
+-rw-r--r--   0 bumgarner   (501) staff       (20)     7860 2023-03-02 15:25:13.000000 wordhoard-1.5.4/wordhoard/utilities/__pycache__/deep_translator.cpython-39.pyc
+-rw-r--r--   0 bumgarner   (501) staff       (20)      879 2023-02-10 15:52:21.000000 wordhoard-1.5.4/wordhoard/utilities/__pycache__/email_address_verification.cpython-39.pyc
+-rw-r--r--   0 bumgarner   (501) staff       (20)     2519 2023-03-02 15:16:31.000000 wordhoard-1.5.4/wordhoard/utilities/__pycache__/exceptions.cpython-39.pyc
+-rw-r--r--   0 bumgarner   (501) staff       (20)     7783 2023-02-12 13:42:58.000000 wordhoard-1.5.4/wordhoard/utilities/__pycache__/google_translator.cpython-39.pyc
+-rw-r--r--   0 bumgarner   (501) staff       (20)    11237 2023-02-11 15:17:46.000000 wordhoard-1.5.4/wordhoard/utilities/__pycache__/mymemory_translator.cpython-39.pyc
+-rw-r--r--   0 bumgarner   (501) staff       (20)     7425 2023-03-18 14:29:02.000000 wordhoard-1.5.4/wordhoard/utilities/__pycache__/request_html.cpython-39.pyc
+-rw-r--r--   0 bumgarner   (501) staff       (20)     7081 2023-03-02 15:16:31.000000 wordhoard-1.5.4/wordhoard/utilities/__pycache__/translator_languages.cpython-39.pyc
+-rw-r--r--   0 bumgarner   (501) staff       (20)     3088 2023-03-04 14:25:28.000000 wordhoard-1.5.4/wordhoard/utilities/__pycache__/user_agents.cpython-39.pyc
+-rw-r--r--   0 bumgarner   (501) staff       (20)     1037 2023-03-04 15:22:37.000000 wordhoard-1.5.4/wordhoard/utilities/__pycache__/word_verification.cpython-39.pyc
+-rw-r--r--   0 bumgarner   (501) staff       (20)      812 2023-02-28 16:23:56.000000 wordhoard-1.5.4/wordhoard/utilities/__pycache__/wordhoard_logger.cpython-39.pyc
+-rw-r--r--   0 bumgarner   (501) staff       (20)     5455 2023-04-14 14:54:35.000000 wordhoard-1.5.4/wordhoard/utilities/caching.py
+-rw-r--r--   0 bumgarner   (501) staff       (20)     4169 2023-03-21 14:56:48.000000 wordhoard-1.5.4/wordhoard/utilities/captcha_checker.py
+-rw-r--r--   0 bumgarner   (501) staff       (20)     2226 2023-03-21 14:56:48.000000 wordhoard-1.5.4/wordhoard/utilities/cleansing.py
+-rw-r--r--   0 bumgarner   (501) staff       (20)     3044 2023-04-10 13:56:10.000000 wordhoard-1.5.4/wordhoard/utilities/cloudflare_bypass.py
+-rw-r--r--   0 bumgarner   (501) staff       (20)     4244 2023-03-21 14:56:48.000000 wordhoard-1.5.4/wordhoard/utilities/cloudflare_checker.py
+-rw-r--r--   0 bumgarner   (501) staff       (20)     1632 2023-05-29 16:46:14.000000 wordhoard-1.5.4/wordhoard/utilities/colorized_text.py
+-rw-r--r--   0 bumgarner   (501) staff       (20)    13901 2023-05-31 14:04:31.000000 wordhoard-1.5.4/wordhoard/utilities/deep_translator.py
+-rw-r--r--   0 bumgarner   (501) staff       (20)     1712 2023-03-21 14:56:48.000000 wordhoard-1.5.4/wordhoard/utilities/email_address_verification.py
+-rw-r--r--   0 bumgarner   (501) staff       (20)     2507 2023-02-13 14:13:15.000000 wordhoard-1.5.4/wordhoard/utilities/exceptions.py
+-rw-r--r--   0 bumgarner   (501) staff       (20)    14793 2023-05-31 14:04:31.000000 wordhoard-1.5.4/wordhoard/utilities/google_translator.py
+-rw-r--r--   0 bumgarner   (501) staff       (20)    17428 2023-05-31 14:04:31.000000 wordhoard-1.5.4/wordhoard/utilities/mymemory_translator.py
+-rw-r--r--   0 bumgarner   (501) staff       (20)    13501 2023-05-31 14:55:32.000000 wordhoard-1.5.4/wordhoard/utilities/request_html.py
+-rw-r--r--   0 bumgarner   (501) staff       (20)    18164 2023-03-21 14:56:48.000000 wordhoard-1.5.4/wordhoard/utilities/translator_languages.py
+-rw-r--r--   0 bumgarner   (501) staff       (20)     4297 2023-03-21 14:56:48.000000 wordhoard-1.5.4/wordhoard/utilities/user_agents.py
+-rw-r--r--   0 bumgarner   (501) staff       (20)     1873 2023-03-21 14:56:48.000000 wordhoard-1.5.4/wordhoard/utilities/word_verification.py
+-rw-r--r--   0 bumgarner   (501) staff       (20)     1623 2023-03-21 14:56:48.000000 wordhoard-1.5.4/wordhoard/utilities/wordhoard_logger.py
+drwxr-xr-x   0 bumgarner   (501) staff       (20)        0 2023-06-01 14:22:53.544772 wordhoard-1.5.4/wordhoard.egg-info/
+-rw-r--r--   0 bumgarner   (501) staff       (20)     5282 2023-06-01 14:22:53.000000 wordhoard-1.5.4/wordhoard.egg-info/PKG-INFO
+-rw-r--r--   0 bumgarner   (501) staff       (20)     2579 2023-06-01 14:22:53.000000 wordhoard-1.5.4/wordhoard.egg-info/SOURCES.txt
+-rw-r--r--   0 bumgarner   (501) staff       (20)        1 2023-06-01 14:22:53.000000 wordhoard-1.5.4/wordhoard.egg-info/dependency_links.txt
+-rw-r--r--   0 bumgarner   (501) staff       (20)      258 2023-06-01 14:22:53.000000 wordhoard-1.5.4/wordhoard.egg-info/requires.txt
+-rw-r--r--   0 bumgarner   (501) staff       (20)       10 2023-06-01 14:22:53.000000 wordhoard-1.5.4/wordhoard.egg-info/top_level.txt
```

### Comparing `wordhoard-1.5.3/LICENSE` & `wordhoard-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wordhoard-1.5.3/PKG-INFO` & `wordhoard-1.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wordhoard
-Version: 1.5.3
+Version: 1.5.4
 Summary: A comprehensive lexical discovery application that is useful for finding semantic relationships such as, the antonyms, synonyms, hypernyms, hyponyms, homophones and definitions for a specific word.
 Home-page: https://github.com/johnbumgarner/wordhoard
 Author: John Bumgarner
 Author-email: wordhoardproject@gmail.com
 License: LICENSE.txt
 Keywords: antonyms,bag of words,definitions,hypernyms,hyponyms,homophones,information retrieval,lexicon,semantic relationships,synonyms,natural language processing
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,14 +12,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: General
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,25 +1,26 @@
-Metadata-Version: 2.1 Name: wordhoard Version: 1.5.3 Summary: A comprehensive
+Metadata-Version: 2.1 Name: wordhoard Version: 1.5.4 Summary: A comprehensive
 lexical discovery application that is useful for finding semantic relationships
 such as, the antonyms, synonyms, hypernyms, hyponyms, homophones and
 definitions for a specific word. Home-page: https://github.com/johnbumgarner/
 wordhoard Author: John Bumgarner Author-email: wordhoardproject@gmail.com
 License: LICENSE.txt Keywords: antonyms,bag of
 words,definitions,hypernyms,hyponyms,homophones,information
 retrieval,lexicon,semantic relationships,synonyms,natural language processing
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3.6 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Topic :: Software Development :: Libraries :: Python Modules Classifier: Topic
-:: Text Processing :: General Classifier: Topic :: Text Processing ::
-Linguistic Classifier: Topic :: Utilities Requires-Python: >=3.6 Description-
-Content-Type: text/markdown License-File: LICENSE # Primary Use Case
+Programming Language :: Python :: 3.10 Classifier: Topic :: Software
+Development :: Libraries :: Python Modules Classifier: Topic :: Text Processing
+:: General Classifier: Topic :: Text Processing :: Linguistic Classifier: Topic
+:: Utilities Requires-Python: >=3.6 Description-Content-Type: text/markdown
+License-File: LICENSE # Primary Use Case
 Textual analysis is a broad term for various research methodologies used to
 qualitatively describe, interpret and understand text data. These methodologies
 are mainly used in academic research to analyze content related to media and
 communication studies, popular culture, sociology, and philosophy. Textual
 analysis allows these researchers to quickly obtain relevant insights from
 unstructured data. All types of information can be gleaned from textual data,
 especially from social media posts or news articles. Some of this information
```

### Comparing `wordhoard-1.5.3/setup.py` & `wordhoard-1.5.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import setuptools
 
 
-
 with open("PYPI_description.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="wordhoard",
-    version="1.5.3",
+    version="1.5.4",
     author="John Bumgarner",
     author_email="wordhoardproject@gmail.com",
     description="A comprehensive lexical discovery application that is useful for finding semantic relationships "
                 "such as, the antonyms, synonyms, hypernyms, hyponyms, homophones and definitions for a specific word.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/johnbumgarner/wordhoard",
@@ -26,14 +25,15 @@
                  "License :: OSI Approved :: MIT License",
                  "Natural Language :: English",
                  "Operating System :: OS Independent",
                  "Programming Language :: Python :: 3.6",
                  "Programming Language :: Python :: 3.7",
                  "Programming Language :: Python :: 3.8",
                  "Programming Language :: Python :: 3.9",
+                 "Programming Language :: Python :: 3.10",
                  "Topic :: Software Development :: Libraries :: Python Modules",
                  "Topic :: Text Processing :: General",
                  "Topic :: Text Processing :: Linguistic",
                  "Topic :: Utilities"],
    keywords=['antonyms', 'bag of words', 'definitions', 'hypernyms', 'hyponyms', 'homophones',
               'information retrieval', 'lexicon', 'semantic relationships', 'synonyms',
               'natural language processing'],
```

### Comparing `wordhoard-1.5.3/wordhoard/__init__.py` & `wordhoard-1.5.4/wordhoard/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ = 'John Bumgarner'
-__date__ = 'July 5, 2021'
+__date__ = 'May 31, 2023'
 __module_name__ = 'wordhoard'
-__version__ = '1.5.3'
+__version__ = '1.5.4'
 __status__ = 'Production'
 __license__ = 'MIT'
 __copyright__ = "Copyright (C) 2021 John Bumgarner"
 __url__ = 'https://pypi.org/project/wordhoard/'
 __url_bug_tracker__ = 'https://github.com/johnbumgarner/wordhoard/issues'
 __url_documentation__ = 'https://wordhoard.readthedocs.io/en/latest/'
 __url_source_code__ = 'https://github.com/johnbumgarner/wordhoard'
```

### Comparing `wordhoard-1.5.3/wordhoard/__pycache__/__init__.cpython-39.pyc` & `wordhoard-1.5.4/wordhoard/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wordhoard-1.5.3/wordhoard/__pycache__/antonyms.cpython-39.pyc` & `wordhoard-1.5.4/wordhoard/__pycache__/antonyms.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wordhoard-1.5.3/wordhoard/__pycache__/dictionary.cpython-39.pyc` & `wordhoard-1.5.4/wordhoard/__pycache__/dictionary.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wordhoard-1.5.3/wordhoard/__pycache__/homophones.cpython-39.pyc` & `wordhoard-1.5.4/wordhoard/__pycache__/homophones.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wordhoard-1.5.3/wordhoard/__pycache__/hypernyms.cpython-39.pyc` & `wordhoard-1.5.4/wordhoard/__pycache__/hypernyms.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wordhoard-1.5.3/wordhoard/__pycache__/hyponyms.cpython-39.pyc` & `wordhoard-1.5.4/wordhoard/__pycache__/hyponyms.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wordhoard-1.5.3/wordhoard/__pycache__/synonyms.cpython-39.pyc` & `wordhoard-1.5.4/wordhoard/__pycache__/synonyms.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wordhoard-1.5.3/wordhoard/antonyms.py` & `wordhoard-1.5.4/wordhoard/antonyms.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 __license__ = 'MIT'
 __copyright__ = "Copyright (C) 2020 John Bumgarner"
 
 ##################################################################################
 # Date Completed: October 15, 2020
 # Author: John Bumgarner
 #
-# Date Last Revised: March 19, 2023
+# Date Last Revised: May 31, 2023
 # Revised by: John Bumgarner
 ##################################################################################
 
 ##################################################################################
 # “AS-IS” Clause
 #
 # Except as represented in this agreement, all work produced by Developer is
@@ -28,14 +28,15 @@
 # purpose.
 ##################################################################################
 
 ##################################################################################
 # Python imports required for basic operations
 ##################################################################################
 import bs4
+import sys
 import json
 import logging
 import requests
 import traceback
 import re as regex
 from bs4 import BeautifulSoup
 from backoff import on_exception, expo
@@ -43,15 +44,14 @@
 from wordhoard.utilities.request_html import Query
 from wordhoard.utilities.colorized_text import colorized_text
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from typing import Dict, List, Optional, Set, Sized, Tuple, Union
 from wordhoard.utilities import caching, cleansing, word_verification
 from wordhoard.utilities.cloudflare_checker import CloudflareVerification
 
-
 logger = logging.getLogger(__name__)
 
 
 class Antonyms(object):
 
     def __init__(self,
                  search_string: str = '',
@@ -105,17 +105,16 @@
         handler = on_exception(expo, RateLimitException, max_time=60, on_backoff=self._backoff_handler)
         # Establishes a rate limit for making requests to the antonyms repositories
         limiter = limits(calls=max_number_of_requests, period=rate_limit_timeout_period)
         self.find_antonyms = handler(limiter(self.find_antonyms))
 
     def _backoff_handler(self):
         if self._rate_limit_status is False:
-            print(colorized_text(255, 0, 0,
-                                 'The antonyms query rate limit was reached. The querying process is entering a '
-                                 'temporary hibernation mode.'))
+            colorized_text('The antonyms query rate limit was reached. The querying process is entering '
+                           'a temporary hibernation mode.', 'red')
             logger.info('The antonyms query rate limit was reached.')
             self._rate_limit_status = True
 
     def _validate_word(self) -> bool:
         """
         This function is designed to validate that the syntax for a string variable is in an acceptable format.
 
@@ -156,15 +155,15 @@
         elif self._proxies is not None and self._user_agent is None:
             response = Query(url, user_agent=None, proxies=self._proxies).get_website_html()
             return response
         elif self._proxies is not None and self._user_agent is not None:
             response = Query(url, user_agent=self._user_agent, proxies=self._proxies).get_website_html()
             return response
 
-    def _run_query_tasks_in_parallel(self) -> List[str]:
+    def _run_query_tasks_in_parallel(self) -> List[tuple[List[str], str]]:
         """
         Runs the query tasks in parallel using a ThreadPool.
 
         :return: list
         :rtype: nested list
         """
         tasks = [self._query_thesaurus_com, self._query_wordhippo]
@@ -195,43 +194,41 @@
         ----------
         :returns:
             antonyms: list of antonyms
 
         :rtype: list
         """
         if self._output_format not in self._valid_output_formats:
-            print(colorized_text(255, 0, 0,
-                                 f'The provided output type --> {self._output_format} <-- is not one of the '
-                                 f'acceptable types: dictionary, list or json.'))
+            colorized_text(f'The provided output type --> {self._output_format} <-- is not one of the '
+                           f'acceptable types: dictionary, list or json.', 'red')
+            sys.exit(1)
         else:
             valid_word = self._validate_word()
             if valid_word is False:
-                print(colorized_text(255, 0, 255, f'Please verify that the word {self._word} is spelled correctly.'))
+                colorized_text(f'Please verify that the word --> {self._word} <-- is spelled correctly.', 'magenta')
             elif valid_word is True:
                 check_cache = self._check_cache()
                 if check_cache[0] is True:
                     part_of_speech = list(check_cache[1].keys())[0]
                     antonyms = cleansing.flatten_multidimensional_list(list(check_cache[1].values()))
                     if self._output_format == 'list':
-                        return antonyms
+                        return sorted(set(antonyms))
                     elif self._output_format == 'dictionary':
                         output_dict = {self._word: {'part_of_speech': part_of_speech,
                                                     'antonyms': sorted(set(antonyms), key=len)}}
                         return output_dict
                     elif self._output_format == 'json':
                         json_object = json.dumps({self._word: {'part_of_speech': part_of_speech,
                                                                'antonyms': sorted(set(antonyms), key=len)}},
                                                  indent=4, ensure_ascii=False)
                         return json_object
 
                 elif check_cache[0] is False:
                     query_results = self._run_query_tasks_in_parallel()
-
                     part_of_speech = ''.join(set([x[1] for x in query_results if x and x is not None]))
-
                     antonyms = ([x[0] for x in query_results if x and x is not None])
                     # flatten antonyms list
                     antonyms_results = cleansing.flatten_multidimensional_list(antonyms)
                     # remove excess white spaces from the strings in the list
                     antonyms_results = cleansing.normalize_space(antonyms_results)
 
                     if len(antonyms_results) != 0:
@@ -244,17 +241,16 @@
                         elif self._output_format == 'json':
                             json_object = json.dumps({self._word: {'part_of_speech': part_of_speech,
                                                                    'antonyms': sorted(set(antonyms_results), key=len)}},
                                                      indent=4, ensure_ascii=False)
 
                             return json_object
                     else:
-                        print(colorized_text(255, 0, 255,
-                                             f'antonyms were found for the word: {self._word} \n'
-                                             f'Please verify that the word is spelled correctly.'))
+                        colorized_text(f'No antonyms were found for the word: {self._word} \n'
+                                       f'Please verify that the word is spelled correctly.', 'blue')
 
     def _query_thesaurus_com(self) -> Union[Tuple[List[str], str], None]:
         """
         This function queries thesaurus.com for antonyms associated
         with the specific word provided to the Class Antonyms.
 
         :returns:
```

### Comparing `wordhoard-1.5.3/wordhoard/dictionary.py` & `wordhoard-1.5.4/wordhoard/dictionary.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 __license__ = 'MIT'
 __copyright__ = "Copyright (C) 2021 John Bumgarner"
 
 ##################################################################################
 # Date Completed: October 15, 2020
 # Author: John Bumgarner
 #
-# Date Last Revised: March 19, 2023
+# Date Last Revised: May 31, 2023
 # Revised by: John Bumgarner
 ##################################################################################
 
 ##################################################################################
 # “AS-IS” Clause
 #
 # Except as represented in this agreement, all work produced by Developer is
@@ -28,14 +28,15 @@
 # purpose.
 ##################################################################################
 
 ##################################################################################
 # Python imports required for basic operations
 ##################################################################################
 import bs4
+import sys
 import json
 import logging
 import requests
 import traceback
 import re as regex
 from bs4 import BeautifulSoup
 from backoff import on_exception, expo
@@ -104,17 +105,16 @@
         handler = on_exception(expo, RateLimitException, max_time=60, on_backoff=self._backoff_handler)
         # Establishes a rate limit for making requests to the definition repositories
         limiter = limits(calls=max_number_of_requests, period=rate_limit_timeout_period)
         self.find_definitions = handler(limiter(self.find_definitions))
 
     def _backoff_handler(self):
         if self._rate_limit_status is False:
-            print(colorized_text(255, 0, 0,
-                                 'The definition query rate limit was reached. The querying process is entering '
-                                 'a temporary hibernation mode.'))
+            colorized_text('The definition query rate limit was reached. The querying process is entering '
+                           'a temporary hibernation mode.', 'red')
             logger.info('The definition query rate limit was reached.')
             self._rate_limit_status = True
 
     def _validate_word(self) -> bool:
         """
         This function is designed to validate that the syntax for a string variable is in an acceptable format.
 
@@ -155,15 +155,15 @@
         elif self._proxies is not None and self._user_agent is None:
             response = Query(url, user_agent=None, proxies=self._proxies).get_website_html()
             return response
         elif self._proxies is not None and self._user_agent is not None:
             response = Query(url, user_agent=self._user_agent, proxies=self._proxies).get_website_html()
             return response
 
-    def _run_query_tasks_in_parallel(self) -> List[str]:
+    def _run_query_tasks_in_parallel(self) -> List[tuple[List[str], str]]:
         """
         Runs the query tasks in parallel using a ThreadPool.
 
         :return: list
         :rtype: nested list
         """
         tasks = [self._query_collins_dictionary, self._query_merriam_webster,
@@ -194,55 +194,52 @@
         Returns
         ----------
         :return: list of definitions
 
         :rtype: list
         """
         if self._output_format not in self._valid_output_formats:
-            print(colorized_text(255, 0, 0,
-                                 f'The provided output type --> {self._output_format} <-- is not one of the '
-                                 f'acceptable types: dictionary, list or json.'))
+            colorized_text(f'The provided output type --> {self._output_format} <-- is not one of the '
+                           f'acceptable types: dictionary, list or json.', 'red')
+            sys.exit(1)
         else:
             valid_word = self._validate_word()
             if valid_word is False:
-                print(colorized_text(255, 0, 255,
-                                     f'Please verify that the word {self._word} is spelled correctly.'))
+                colorized_text(f'Please verify that the word {self._word} is spelled correctly.', 'magenta')
             elif valid_word is True:
                 check_cache = self._check_cache()
                 if check_cache[0] is True:
                     part_of_speech = list(check_cache[1].keys())[0]
                     definitions = cleansing.flatten_multidimensional_list(list(check_cache[1].values()))
                     if self._output_format == 'list':
-                        return sorted(set(definitions), key=len)
+                        return sorted(set(definitions))
                     elif self._output_format == 'dictionary':
                         output_dict = {self._word: {'part_of_speech': part_of_speech,
                                                     'definitions': sorted(set(definitions), key=len)}}
                         return output_dict
                     elif self._output_format == 'json':
                         json_object = json.dumps({self._word: {'part_of_speech': part_of_speech,
                                                                'definitions': sorted(set(definitions), key=len)}},
                                                  indent=4, ensure_ascii=False)
                         return json_object
 
                 elif check_cache[0] is False:
                     query_results = self._run_query_tasks_in_parallel()
-
                     part_of_speech = ''.join(set([x[1] for x in query_results if x and x is not None]))
-
                     definitions = ([x[0] for x in query_results if x and x is not None])
+                    # flatten definitions list
                     definitions = cleansing.flatten_multidimensional_list(definitions)
                     # remove excess white spaces from the strings in the list
                     definitions = [regex.sub(' +', " ", x) for x in definitions]
                     if not definitions:
-                        print(colorized_text(255, 0, 255,
-                                             f'No definitions were found for the word: {self._word} \n'
-                                             f'Please verify that the word is spelled correctly.'))
+                        colorized_text(f'No definitions were found for the word: {self._word} \n'
+                                       f'Please verify that the word is spelled correctly.', 'blue')
                     else:
                         if self._output_format == 'list':
-                            return sorted(set(definitions), key=len)
+                            return sorted(set(definitions))
                         elif self._output_format == 'dictionary':
                             output_dict = {self._word: {'part_of_speech': part_of_speech, 'definitions': sorted(set(
                                 definitions), key=len)}}
                             return output_dict
                         elif self._output_format == 'json':
                             json_object = json.dumps({self._word: {'part_of_speech': part_of_speech,
                                                                    'definitions': sorted(set(definitions), key=len)}},
@@ -383,15 +380,14 @@
                         return None
                     elif soup.find('h1', {'class': 'mispelled-word'}):
                         logger.info(f'Merriam-webster.com has no definition reference for the word {self._word}')
                         return None
                     else:
                         definition_list = []
                         part_of_speech_category = ''
-
                         # obtain the part of speech category for the specific word
                         if soup.select(
                             '#dictionary-entry-1 > div.row.entry-header > div > '
                             'div.entry-header-content.d-flex.flex-wrap.align-items-baseline.flex-row.mb-0 > h2 > a'):
                             css_part_of_speech = soup.select(
                                 '#dictionary-entry-1 > div.row.entry-header > div > div.entry-header-content.d-flex.flex-wrap.align-items-baseline.flex-row.mb-0 > h2 > a')
                             if len(css_part_of_speech[0].text) != 0:
```

### Comparing `wordhoard-1.5.3/wordhoard/files/common_english_homophones.pkl` & `wordhoard-1.5.4/wordhoard/files/common_english_homophones.pkl`

 * *Files identical despite different names*

### Comparing `wordhoard-1.5.3/wordhoard/files/common_user_agents.pkl` & `wordhoard-1.5.4/wordhoard/files/common_user_agents.pkl`

 * *Files identical despite different names*

### Comparing `wordhoard-1.5.3/wordhoard/files/no_homophones_english.pkl` & `wordhoard-1.5.4/wordhoard/files/no_homophones_english.pkl`

 * *Files identical despite different names*

### Comparing `wordhoard-1.5.3/wordhoard/homophones.py` & `wordhoard-1.5.4/wordhoard/homophones.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 __license__ = 'MIT'
 __copyright__ = "Copyright (C) 2021 John Bumgarner"
 
 ##################################################################################
 # Date Completed: June 11, 2021
 # Author: John Bumgarner
 #
-# Date Last Revised: February 27, 2023
+# Date Last Revised: May 31, 2023
 # Revised by: John Bumgarner
 ##################################################################################
 
 ##################################################################################
 # “AS-IS” Clause
 #
 # Except as represented in this agreement, all work produced by Developer is
@@ -135,29 +135,28 @@
             if match:
                 for word in homophones:
                     if word != self._word:
                         rtn_list.append(f'{self._word} is a homophone of {word}')
         if len(rtn_list) > 0:
             return list(set(rtn_list))
 
-    def _english_words_without_homophones(self) -> str:
+    def _english_words_without_homophones(self) -> None:
         """
         This function iterates through a list of English
         language words with no known homophones.
 
         :return: no homophones for word
         :rtype: str
         """
         global _no_homophones_list
         match = bool(self._word in _no_homophones_list)
         if match:
-            return colorized_text(255, 0, 255,
-                                  f'No homophones for {self._word}')
+            return None
 
-    def find_homophones(self) -> Union[List[str], str]:
+    def find_homophones(self) -> Union[List[str], None]:
         """
         Purpose
         ----------
         This function queries multiple lists to find
         English language homophones associated with the
         specific word provided to the Class Homophones.
 
@@ -172,8 +171,11 @@
         """
         valid_word = self._validate_word()
         if valid_word:
             known_english_homophones = self._common_english_homophones()
             if known_english_homophones:
                 return known_english_homophones
             elif not known_english_homophones:
-                return self._english_words_without_homophones()
+                if self._english_words_without_homophones() is None:
+                    colorized_text(f'No homophones for the word - {self._word}', 'magenta')
+                    return None
+
```

### Comparing `wordhoard-1.5.3/wordhoard/hypernyms.py` & `wordhoard-1.5.4/wordhoard/hypernyms.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 __license__ = 'MIT'
 __copyright__ = "Copyright (C) 2021 John Bumgarner"
 
 ##################################################################################
 # Date Initially Completed: June 12, 2021
 # Author: John Bumgarner
 #
-# Date Last Revised: March 19, 2023
+# Date Last Revised: May 31, 2023
 # Revised by: John Bumgarner
 ##################################################################################
 
 ##################################################################################
 # “AS-IS” Clause
 #
 # Except as represented in this agreement, all work produced by Developer is
@@ -28,14 +28,15 @@
 # purpose.
 ##################################################################################
 
 ##################################################################################
 # Python imports required for basic operations
 ##################################################################################
 import bs4
+import sys
 import json
 import logging
 import traceback
 from bs4 import BeautifulSoup
 from backoff import on_exception, expo
 from ratelimit import limits, RateLimitException
 from wordhoard.utilities.request_html import Query
@@ -175,17 +176,16 @@
         handler = on_exception(expo, RateLimitException, max_time=60, on_backoff=self._backoff_handler)
         # Establishes a rate limit for making requests to the hypernyms repositories
         limiter = limits(calls=max_number_of_requests, period=rate_limit_timeout_period)
         self.find_hypernyms = handler(limiter(self.find_hypernyms))
 
     def _backoff_handler(self):
         if self._rate_limit_status is False:
-            print(colorized_text(255, 0, 0,
-                                 'The hypernym query rate limit was reached. The querying process is entering '
-                                 'a temporary hibernation mode.'))
+            colorized_text('The hypernym query rate limit was reached. The querying process is entering '
+                           'a temporary hibernation mode.', 'red')
             logger.info('The hypernym query rate limit was reached.')
             self._rate_limit_status = True
 
     def _validate_word(self) -> bool:
         """
         This function is designed to validate that the syntax for a string variable is in an acceptable format.
 
@@ -233,22 +233,21 @@
 
             TypeError: Raised when an operation or function is applied to an object of inappropriate type
 
             bs4.FeatureNotFound: raised by the BeautifulSoup constructor if no parser with the requested features
             is found
         """
         if self._output_format not in self._valid_output_formats:
-            print(colorized_text(255, 0, 0,
-                                 f'The provided output type --> {self._output_format} <-- is not one of the '
-                                 f'acceptable types: dictionary, list or json.'))
+            colorized_text(f'The provided output type --> {self._output_format} <-- is not one of the '
+                           f'acceptable types: dictionary, list or json.', 'red')
+            sys.exit(1)
         else:
             valid_word = self._validate_word()
             if valid_word is False:
-                print(colorized_text(255, 0, 255,
-                                     f'Please verify that the word {self._word} is spelled correctly.'))
+                colorized_text(f'Please verify that the word {self._word} is spelled correctly.', 'magenta')
             elif valid_word is True:
                 check_cache = self._check_cache()
                 if check_cache[0] is True:
                     hypernym = cleansing.flatten_multidimensional_list(list(check_cache[1]))
                     if self._output_format == 'list':
                         return hypernym
                     elif self._output_format == 'dictionary':
@@ -281,17 +280,16 @@
                         else:
                             soup = BeautifulSoup(response.text, "lxml")
                             cloudflare_protection = CloudflareVerification('https://www.classicthesaurus.com',
                                                                            soup).cloudflare_protected_url()
                             if cloudflare_protection is False:
                                 hypernym = _get_hypernyms(soup)
                                 if 'no hypernyms found' in hypernym:
-                                    print(colorized_text(255, 0, 255,
-                                                         f'No hypernyms were found for the word: {self._word} \n'
-                                                         f'Please verify that the word is spelled correctly.'))
+                                    colorized_text(f'No hypernyms were found for the word: {self._word} \n'
+                                                   f'Please verify that the word is spelled correctly.', 'blue')
                                 else:
                                     number_of_pages = _get_number_of_pages(soup)
                                     if number_of_pages >= 2:
                                         for page in range(2, number_of_pages):
                                             sub_html = ''
                                             if self._proxies is None and self._user_agent is None:
                                                     sub_html = Query(
```

### Comparing `wordhoard-1.5.3/wordhoard/hyponyms.py` & `wordhoard-1.5.4/wordhoard/hyponyms.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 __license__ = 'MIT'
 __copyright__ = "Copyright (C) 2021 John Bumgarner"
 
 ##################################################################################
 # Date Initially Completed: June 12, 2021
 # Author: John Bumgarner
 #
-# Date Last Revised: March 19, 2023
+# Date Last Revised: May 31, 2023
 # Revised by: John Bumgarner
 ###################################################################################
 
 ##################################################################################
 # “AS-IS” Clause
 #
 # Except as represented in this agreement, all work produced by Developer is
@@ -28,14 +28,15 @@
 # purpose.
 ##################################################################################
 
 ##################################################################################
 # Python imports required for basic operations
 ##################################################################################
 import bs4
+import sys
 import json
 import logging
 import traceback
 from bs4 import BeautifulSoup
 from backoff import on_exception, expo
 from ratelimit import limits, RateLimitException
 from wordhoard.utilities.request_html import Query
@@ -179,17 +180,16 @@
         handler = on_exception(expo, RateLimitException, max_time=60, on_backoff=self._backoff_handler)
         # Establishes a rate limit for making requests to the hyponyms repositories
         limiter = limits(calls=max_number_of_requests, period=rate_limit_timeout_period)
         self.find_hyponyms = handler(limiter(self.find_hyponyms))
 
     def _backoff_handler(self):
         if self._rate_limit_status is False:
-            print(colorized_text(255, 0, 0,
-                                 'The hyponyms query rate limit was reached. The querying process is entering '
-                                 'a temporary hibernation mode.'))
+            colorized_text('The hyponyms query rate limit was reached. The querying process is entering '
+                           'a temporary hibernation mode.', 'red')
             logger.info('The hyponyms query rate limit was reached.')
             self._rate_limit_status = True
 
     def _validate_word(self) -> bool:
         """
         This function is designed to validate that the syntax for a string variable is in an acceptable format.
 
@@ -237,22 +237,21 @@
 
             TypeError: Raised when an operation or function is applied to an object of inappropriate type
 
             bs4.FeatureNotFound: raised by the BeautifulSoup constructor if no parser with the requested features
             is found
         """
         if self._output_format not in self._valid_output_formats:
-            print(colorized_text(255, 0, 0,
-                                 f'The provided output type --> {self._output_format} <-- is not one of the '
-                                 f'acceptable types: dictionary, list or json.'))
+            colorized_text(f'The provided output type --> {self._output_format} <-- is not one of the '
+                           f'acceptable types: dictionary, list or json.', 'red')
+            sys.exit(1)
         else:
             valid_word = self._validate_word()
             if valid_word is False:
-                print(colorized_text(255, 0, 255,
-                                     f'Please verify that the word {self._word} is spelled correctly.'))
+                colorized_text(f'Please verify that the word {self._word} is spelled correctly.', 'magenta')
             elif valid_word is True:
                 check_cache = self._check_cache()
                 if check_cache[0] is True:
                     hyponym = cleansing.flatten_multidimensional_list(check_cache[1])
                     if self._output_format == 'list':
                         return [word.lower() for word in hyponym]
                     elif self._output_format == 'dictionary':
@@ -287,17 +286,16 @@
                         else:
                             soup = BeautifulSoup(response.text, "lxml")
                             cloudflare_protection = CloudflareVerification('https://www.classicthesaurus.com',
                                                                            soup).cloudflare_protected_url()
                             if cloudflare_protection is False:
                                 hyponym = _get_hyponyms(soup)
                                 if 'no hyponyms found' in hyponym:
-                                    print(colorized_text(255, 0, 255,
-                                                         f'No hyponyms were found for the word: {self._word} \n'
-                                                         f'Please verify that the word is spelled correctly.'))
+                                    colorized_text(f'No hyponyms were found for the word: {self._word} \n'
+                                                   f'Please verify that the word is spelled correctly.', 'blue')
                                     return None
                                 else:
                                     number_of_pages = _get_number_of_pages(soup)
                                     if number_of_pages >= 2:
                                         for page in range(2, number_of_pages):
                                             sub_html = ''
                                             if self._proxies is None and self._user_agent is None:
```

### Comparing `wordhoard-1.5.3/wordhoard/synonyms.py` & `wordhoard-1.5.4/wordhoard/synonyms.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 __license__ = 'MIT'
 __copyright__ = "Copyright (C) 2020 John Bumgarner"
 
 ##################################################################################
 # Date Completed: October 15, 2020
 # Author: John Bumgarner
 #
-# Date Last Revised: March 20, 2023
+# Date Last Revised: May 31, 2023
 # Revised by: John Bumgarner
 ##################################################################################
 
 ##################################################################################
 # “AS-IS” Clause
 #
 # Except as represented in this agreement, all work produced by Developer is
@@ -28,14 +28,15 @@
 # purpose.
 ##################################################################################
 
 ##################################################################################
 # Python imports required for basic operations
 ##################################################################################
 import bs4
+import sys
 import json
 import logging
 import requests
 import traceback
 import re as regex
 from bs4 import BeautifulSoup
 from backoff import on_exception, expo
@@ -44,14 +45,15 @@
 from wordhoard.utilities.cloudflare_bypass import Cloudflare
 from wordhoard.utilities.colorized_text import colorized_text
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from typing import Dict, List, Optional, Set, Sized, Tuple, Union
 from wordhoard.utilities import caching, cleansing, word_verification
 from wordhoard.utilities.cloudflare_checker import CloudflareVerification
 
+
 logger = logging.getLogger(__name__)
 
 class Synonyms(object):
 
     def __init__(self,
                  search_string: str = '',
                  output_format: str = 'list',
@@ -100,17 +102,16 @@
         handler = on_exception(expo, RateLimitException, max_time=60, on_backoff=self._backoff_handler)
         # Establishes a rate limit for making requests to the synonyms repositories
         limiter = limits(calls=max_number_of_requests, period=rate_limit_timeout_period)
         self.find_synonyms = handler(limiter(self.find_synonyms))
 
     def _backoff_handler(self):
         if self._rate_limit_status is False:
-            print(colorized_text(255, 0, 0,
-                                 'The synonyms query rate limit was reached. The querying process is '
-                                 'entering a temporary hibernation mode.'))
+            colorized_text('The synonyms query rate limit was reached. The querying process is '
+                                 'entering a temporary hibernation mode.', 'red')
             logger.info('The synonyms query rate limit was reached.')
             self._rate_limit_status = True
 
     def _validate_word(self) -> bool:
         """
         This function is designed to validate that the syntax for
         a string variable is in an acceptable format.
@@ -152,15 +153,15 @@
         elif self._proxies is not None and self._user_agent is None:
             response = Query(url, user_agent=None, proxies=self._proxies).get_website_html()
             return response
         elif self._proxies is not None and self._user_agent is not None:
             response = Query(url, user_agent=self._user_agent, proxies=self._proxies).get_website_html()
             return response
 
-    def _run_query_tasks_in_parallel(self) -> List[str]:
+    def _run_query_tasks_in_parallel(self) -> List[tuple[List[str], str]]:
         """
         Runs the query tasks in parallel using a ThreadPool.
 
         :return: list
         :rtype: nested list
         """
         tasks = [self._query_collins_dictionary, self._query_merriam_webster, self._query_synonym_com,
@@ -192,55 +193,52 @@
         ----------
         :returns:
             synonyms: list of synonyms
 
         :rtype: list
         """
         if self._output_format not in self._valid_output_formats:
-            print(colorized_text(255, 0, 0,
-                                 f'The provided output type --> {self._output_format} <-- is not one of the '
-                                 f'acceptable types: dictionary, list or json.'))
+            colorized_text(f'The provided output type --> {self._output_format} <-- is not one of the '
+                           f'acceptable types: dictionary, list or json.', 'red')
+            sys.exit(1)
         else:
             valid_word = self._validate_word()
             if valid_word is False:
-                print(colorized_text(255, 0, 255,
-                                  f'Please verify that the word {self._word} is spelled correctly.'))
+                colorized_text(f'Please verify that the word {self._word} is spelled correctly.', 'magenta')
             elif valid_word is True:
                 check_cache = self._check_cache()
                 if check_cache[0] is True:
                     part_of_speech = list(check_cache[1].keys())[0]
                     synonyms = cleansing.flatten_multidimensional_list(list(check_cache[1].values()))
                     if self._output_format == 'list':
-                        return sorted(set([word.lower() for word in check_cache[1]]))
+                        return sorted(set(synonyms))
                     elif self._output_format == 'dictionary':
                         output_dict = {self._word: {'part_of_speech': part_of_speech, 'synonyms': sorted(set(
                             synonyms), key=len)}}
                         return output_dict
                     elif self._output_format == 'json':
                         json_object = json.dumps({self._word: {'part_of_speech': part_of_speech,
                                                                'synonyms': sorted(set(synonyms), key=len)}},
                                                  indent=4, ensure_ascii=False)
                         return json_object
 
                 elif check_cache[0] is False:
                     query_results = self._run_query_tasks_in_parallel()
-
                     part_of_speech = ''.join(set([x[1] for x in query_results if x and x is not None]))
-
                     synonyms = ([x[0] for x in query_results if x and x is not None])
+                    # flatten synonyms list
                     synonyms_results =  cleansing.flatten_multidimensional_list(synonyms)
                     # remove excess white spaces from the strings in the list
                     synonyms_results = cleansing.normalize_space(synonyms_results)
                     if not synonyms_results:
-                        print(colorized_text(255, 0, 255,
-                                             f'No synonyms were found for the word: {self._word} \n'
-                                             f'Please verify that the word is spelled correctly.'))
+                        colorized_text(f'No synonyms were found for the word: {self._word} \n'
+                                       f'Please verify that the word is spelled correctly.', 'blue')
                     else:
                         if self._output_format == 'list':
-                            return sorted(set([word.lower() for word in synonyms_results]), key=len)
+                            return sorted(set([word.lower() for word in synonyms_results]))
                         elif self._output_format == 'dictionary':
                             output_dict = {self._word: {'part_of_speech': part_of_speech, 'synonyms': sorted(set(
                                 synonyms_results), key=len)}}
                             return output_dict
                         elif self._output_format == 'json':
                             json_object = json.dumps({self._word: {'part_of_speech': part_of_speech,
                                                                    'synonyms': sorted(set(synonyms_results), key=len)}},
@@ -653,7 +651,8 @@
             logger.error(''.join(traceback.format_tb(error.__traceback__)))
         except KeyError as error:
             logger.error('A KeyError occurred in the following code segment:')
             logger.error(''.join(traceback.format_tb(error.__traceback__)))
         except TypeError as error:
             logger.error('A TypeError occurred in the following code segment:')
             logger.error(''.join(traceback.format_tb(error.__traceback__)))
+
```

### Comparing `wordhoard-1.5.3/wordhoard/utilities/__pycache__/caching.cpython-39.pyc` & `wordhoard-1.5.4/wordhoard/utilities/__pycache__/caching.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wordhoard-1.5.3/wordhoard/utilities/__pycache__/captcha_checker.cpython-39.pyc` & `wordhoard-1.5.4/wordhoard/utilities/__pycache__/captcha_checker.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wordhoard-1.5.3/wordhoard/utilities/__pycache__/cleansing.cpython-39.pyc` & `wordhoard-1.5.4/wordhoard/utilities/__pycache__/cleansing.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wordhoard-1.5.3/wordhoard/utilities/__pycache__/cloudflare_bypass.cpython-39.pyc` & `wordhoard-1.5.4/wordhoard/utilities/__pycache__/cloudflare_bypass.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wordhoard-1.5.3/wordhoard/utilities/__pycache__/cloudflare_checker.cpython-39.pyc` & `wordhoard-1.5.4/wordhoard/utilities/__pycache__/cloudflare_checker.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wordhoard-1.5.3/wordhoard/utilities/__pycache__/colorized_text.cpython-39.pyc` & `wordhoard-1.5.4/wordhoard/utilities/__pycache__/colorized_text.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wordhoard-1.5.3/wordhoard/utilities/__pycache__/deep_translator.cpython-39.pyc` & `wordhoard-1.5.4/wordhoard/utilities/__pycache__/deep_translator.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wordhoard-1.5.3/wordhoard/utilities/__pycache__/email_address_verification.cpython-39.pyc` & `wordhoard-1.5.4/wordhoard/utilities/__pycache__/email_address_verification.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wordhoard-1.5.3/wordhoard/utilities/__pycache__/exceptions.cpython-39.pyc` & `wordhoard-1.5.4/wordhoard/utilities/__pycache__/exceptions.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wordhoard-1.5.3/wordhoard/utilities/__pycache__/google_translator.cpython-39.pyc` & `wordhoard-1.5.4/wordhoard/utilities/__pycache__/google_translator.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wordhoard-1.5.3/wordhoard/utilities/__pycache__/mymemory_translator.cpython-39.pyc` & `wordhoard-1.5.4/wordhoard/utilities/__pycache__/mymemory_translator.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wordhoard-1.5.3/wordhoard/utilities/__pycache__/request_html.cpython-39.pyc` & `wordhoard-1.5.4/wordhoard/utilities/__pycache__/request_html.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wordhoard-1.5.3/wordhoard/utilities/__pycache__/translator_languages.cpython-39.pyc` & `wordhoard-1.5.4/wordhoard/utilities/__pycache__/translator_languages.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wordhoard-1.5.3/wordhoard/utilities/__pycache__/user_agents.cpython-39.pyc` & `wordhoard-1.5.4/wordhoard/utilities/__pycache__/user_agents.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wordhoard-1.5.3/wordhoard/utilities/__pycache__/word_verification.cpython-39.pyc` & `wordhoard-1.5.4/wordhoard/utilities/__pycache__/word_verification.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wordhoard-1.5.3/wordhoard/utilities/__pycache__/wordhoard_logger.cpython-39.pyc` & `wordhoard-1.5.4/wordhoard/utilities/__pycache__/wordhoard_logger.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wordhoard-1.5.3/wordhoard/utilities/caching.py` & `wordhoard-1.5.4/wordhoard/utilities/caching.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,22 +20,22 @@
 # purpose.
 ##################################################################################
 
 ##################################################################################
 # Date Completed: October 15, 2020
 # Author: John Bumgarner
 #
-# Date Last Revised: March 18, 2023
+# Date Last Revised: April 14, 2023
 # Revised by: John Bumgarner
 ##################################################################################
 
 ##################################################################################
 # Python imports required for basic operations
 ##################################################################################
-from typing import List, Dict, Optional, Tuple, Union, Set
+from typing import List, Dict, Optional, Tuple, Set
 
 ##################################################################################
 # in memory temporary cache for antonyms
 ##################################################################################
 temporary_dict_antonyms: Dict[str, Dict[str, Set[str]]] = {}
 
 def cache_antonyms(word:  str) -> Tuple[bool, Optional[str]]:
```

### Comparing `wordhoard-1.5.3/wordhoard/utilities/captcha_checker.py` & `wordhoard-1.5.4/wordhoard/utilities/captcha_checker.py`

 * *Files identical despite different names*

### Comparing `wordhoard-1.5.3/wordhoard/utilities/cleansing.py` & `wordhoard-1.5.4/wordhoard/utilities/cleansing.py`

 * *Files identical despite different names*

### Comparing `wordhoard-1.5.3/wordhoard/utilities/cloudflare_bypass.py` & `wordhoard-1.5.4/wordhoard/utilities/cloudflare_bypass.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,16 +51,17 @@
     def bypass(self) -> BeautifulSoup:
         """
         This function attempts to bypass the Cloudflare's DDoS mitigation protection
         for a specific website.
 
         :return: BeautifulSoup object
         """
-        scraper = cloudscraper.create_scraper(delay=10,  browser={'custom': 'ScraperBot/1.0', })
+        scraper = cloudscraper.create_scraper(delay=10, browser={'custom': 'ScraperBot/1.0', })
         response = scraper.get(self._url)
+
         if response.status_code == 502 or response.status_code == 520 or response.status_code == 521:
             logger.info('-' * 80)
             logger.info(f'Cloudflare DDoS mitigation service protection bypass started.')
             logger.info(f'Requested URL: {self._url}')
             logger.info(f'Status Code: {response.status_code}')
             logger.info('-' * 80)
             scraper.close()
```

### Comparing `wordhoard-1.5.3/wordhoard/utilities/cloudflare_checker.py` & `wordhoard-1.5.4/wordhoard/utilities/cloudflare_checker.py`

 * *Files identical despite different names*

### Comparing `wordhoard-1.5.3/wordhoard/utilities/colorized_text.py` & `wordhoard-1.5.4/wordhoard/utilities/colorized_text.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 
 """
 This Python script provide colorized text in the error messages thrown by WordHoard.
 """
 __author__ = 'John Bumgarner'
-__date__ = 'February 04, 2023'
+__date__ = 'May 28, 2023'
 __status__ = 'Production'
 __license__ = 'MIT'
 __copyright__ = "Copyright (C) 2023 John Bumgarner"
 
 ##################################################################################
 # “AS-IS” Clause
 #
@@ -16,28 +16,32 @@
 # provided “AS IS”. Other than as provided in this agreement, Developer makes no
 # other warranties, express or implied, and hereby disclaims all implied warranties,
 # including any warranty of merchantability and warranty of fitness for a particular
 # purpose.
 ##################################################################################
 
 ##################################################################################
-# Date Completed: February 04, 2023
+# Date Completed: May 28, 2023
 # Author: John Bumgarner
 #
 # Date Last Revised:
 # Revised by:
 ##################################################################################
 
-
-def colorized_text(r: int, g: int, b: int, text: str) -> str:
+def colorized_text(text: str, color: str) -> None:
     """
-    This function provides error messages color.
-    For example:
-    rgb(255, 0, 0) is displayed as the color red
-    rgb(0, 255, 0) is displayed as the color green
-    :param r: red color value
-    :param g: green color value
-    :param b: below color value
+    This function provides terminal error messages in color.
     :param text: text to colorized
-    :return: string of colorized text
+    :param color: color value
+    :return: print error in color
     """
-    return f"\033[38;2;{r};{g};{b}m{text}\033[0m"
+    RESET = "\033[0m" # resets the terminal color to its default
+    if color == 'red':
+        print(f'\033[1;31m{text}{RESET}')
+    elif color == 'blue':
+        print(f'\033[1;34m{text}{RESET}')
+    elif color == 'green':
+        print(f'\033[1;32m{text}{RESET}')
+    elif color == 'magenta':
+        print(f'\033[1;35m{text}{RESET}')
+
+
```

### Comparing `wordhoard-1.5.3/wordhoard/utilities/deep_translator.py` & `wordhoard-1.5.4/wordhoard/utilities/deep_translator.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 # purpose.
 ##################################################################################
 
 ##################################################################################
 # Date Completed: September 24, 2021
 # Author: John Bumgarner
 #
-# Date Last Revised: March 02, 2023
+# Date Last Revised: May 31, 2023
 # Revised by: John Bumgarner
 ##################################################################################
 
 ##################################################################################
 # Python imports required for basic operations
 ##################################################################################
 import deepl
@@ -67,17 +67,16 @@
         # Establishes a rate limit for making requests to the Deep translation service
         limiter = limits(calls=60, period=60)
         self.translate_word = handler(limiter(self.translate_word))
         self.reverse_translate = handler(limiter(self.reverse_translate))
 
     def _backoff_handler(self):
         if self._rate_limit_status is False:
-            print(colorized_text(255, 0, 0,
-                                 'The Deep translation service query rate Limit was reached. The querying '
-                                 'process is entering a temporary hibernation mode.'))
+            colorized_text('The Deep translation service query rate Limit was reached. The querying '
+                           'process is entering a temporary hibernation mode.', 'red')
             logger.info('The Deep translation service query rate limit was reached.')
             self._rate_limit_status = True
 
     def _deep_supported_languages(self) -> Union[str, None]:
         """
         This function determines if the requested source language is
         one of the supported languages for the Deep translation service.
@@ -123,37 +122,36 @@
             translated_text = result.text
             return translated_text
 
         except AuthorizationException as error:
             """
             The exception is thrown when the authentication key is not valid for the Deep Translation service.
             """
-            print(colorized_text(255, 0, 0, 'The authentication key used for Deep Translation service is '
-                                            'invalid.\nPlease verify that the authentication key used is valid.'))
+            colorized_text('The authentication key used for Deep Translation service is invalid.\nPlease verify '
+                           'that the authentication key used is valid.', 'red')
             logger.error('Authorization Error:')
             logger.error('An authorization error has occurred when using the Deep Translation service.')
             logger.error('Please verify that the authentication key used is valid.')
             logger.error(''.join(traceback.format_tb(error.__traceback__)))
 
         except QuotaExceededException as error:
             """
             The exception is thrown when the translation quota for this billing period has been exceeded.
             """
-            print(colorized_text(255, 0, 0, 'The quota for the Deep Translation service for this billing '
-                                            'period has been exceeded.'))
+            colorized_text('The quota for the Deep Translation service for this billing period has '
+                           'been exceeded.', 'red')
             logger.error('The quota for the the Deep Translation service for this billing period has been exceeded.')
             logger.error(''.join(traceback.format_tb(error.__traceback__)))
 
         except TooManyRequestsException as error:
             """
             This exception is thrown when the maximum number of connection requests have been exceeded for a 
             specific time for the Deep Translation service.
             """
-            print(colorized_text(255, 0, 0, 'There has been too many connection requests to the Deep '
-                                            'Translation service.'))
+            colorized_text('There has been too many connection requests to the Deep Translation service.', 'red')
             logger.error('Connection Request Error:')
             logger.error('There has been too many connection requests to the Deep Translation service.')
             logger.error(''.join(traceback.format_tb(error.__traceback__)))
 
         except TypeError as error:
             """
             The exception is thrown when an operation or function is applied to an object of inappropriate type.
@@ -163,20 +161,20 @@
 
         except ValueError as error:
             """
             The exception is thrown when an operation or function receives an argument that 
             has the right type but an inappropriate value.
             """
             if str(error) == "auth_key must not be empty":
-                print(colorized_text(255, 0, 0, 'An Authorization failure has occurred when using the Deep '
-                                                'translation service.  Please verify your authentication key'))
+                colorized_text('An Authorization failure has occurred when using the Deep translation service.  '
+                               'Please verify your authentication key', 'red')
                 logger.error('An Authorization key cannot be empty when using the Deep translation service.')
                 logger.error(''.join(traceback.format_tb(error.__traceback__)))
             elif str(error) == 'text must not be empty':
-                print(colorized_text(255, 0, 0, 'An empty string was passed to the Deep translation service.'))
+                colorized_text('An empty string was passed to the Deep translation service.', 'red')
                 logger.error('An empty string was passed to the Deep translation service.')
                 logger.error(''.join(traceback.format_tb(error.__traceback__)))
             else:
                 logger.error(f'An unknown ValueError occurred when attempting to translate the word'
                              f' {self._str_to_translate}')
                 logger.error(''.join(traceback.format_tb(error.__traceback__)))
 
@@ -195,38 +193,36 @@
             translated_text = result.text
             return translated_text
 
         except AuthorizationException as error:
             """
             The exception is thrown when the authentication key is not valid for the Deep Translation service.
             """
-            print(colorized_text(255, 0, 0, 'The authentication key used for Deep Translation service is '
-                                            'invalid.\nPlease verify that the authentication key used is '
-                                            'valid.'))
+            colorized_text('The authentication key used for Deep Translation service is invalid.\nPlease verify '
+                           'that the authentication key used is valid.', 'red')
             logger.error('Authorization Error:')
             logger.error('An authorization error has occurred when using the Deep Translation service.')
             logger.error('Please verify that the authentication key used is valid.')
             logger.error(''.join(traceback.format_tb(error.__traceback__)))
 
         except QuotaExceededException as error:
             """
             The exception is thrown when the translation quota for this billing period has been exceeded.
             """
-            print(colorized_text(255, 0, 0, 'The quota for the Deep Translation service for this billing '
-                                            'period has been exceeded.'))
+            colorized_text('The quota for the Deep Translation service for this billing period has '
+                           'been exceeded.', 'red')
             logger.error('The quota for the Deep Translation service for this billing period has been exceeded.')
             logger.error(''.join(traceback.format_tb(error.__traceback__)))
 
         except TooManyRequestsException as error:
             """
             This exception is thrown when the maximum number of connection requests have been exceeded for a 
             specific time for the Deep Translation service.
             """
-            print(colorized_text(255, 0, 0, 'There has been too many connection requests to the Deep '
-                                            'Translation service.'))
+            colorized_text('There has been too many connection requests to the Deep Translation service.', 'red')
             logger.error('Connection Request Error:')
             logger.error('There has been too many connection requests to the Deep Translation service.')
             logger.error(''.join(traceback.format_tb(error.__traceback__)))
 
         except TypeError as error:
             """
             The exception is thrown when an operation or function is applied to an object of inappropriate type.
@@ -236,20 +232,20 @@
 
         except ValueError as error:
             """
             The exception is thrown when an operation or function receives an argument that 
             has the right type but an inappropriate value.
             """
             if str(error) == "auth_key must not be empty":
-                print(colorized_text(255, 0, 0, 'An Authorization failure has occurred when using the Deep '
-                                                'Translation service.  Please verify your authentication key'))
+                colorized_text('An Authorization failure has occurred when using the Deep Translation service.\n'
+                               'Please verify your authentication key', 'red')
                 logger.error('An Authorization key cannot be empty when using the Deep Translation service.')
                 logger.error(''.join(traceback.format_tb(error.__traceback__)))
             elif str(error) == 'text must not be empty':
-                print(colorized_text(255, 0, 0, 'An empty string was passed to the Deep Translation service.'))
+                colorized_text('An empty string was passed to the Deep Translation service.', 'red')
                 logger.error('An empty string was passed to the Deep translation service.')
                 logger.error(''.join(traceback.format_tb(error.__traceback__)))
             else:
                 logger.error(f'An unknown ValueError occurred when attempting to translate the word'
                              f' {self._str_to_translate}')
                 logger.error(''.join(traceback.format_tb(error.__traceback__)))
 
@@ -260,19 +256,20 @@
         :return: translated word
         :rtype: string
         """
         supported_language = self._deep_supported_languages()
         if supported_language:
             return self._deep_translate(supported_language)
         elif not supported_language:
-            print(colorized_text(255, 0, 0, f'The language provided is not one of the supported languages '
-                                            f'for the Deep Translation service.'))
-            print(colorized_text(255, 0, 0, f'Requested language: {self._source_language}'))
-            print(colorized_text(255, 0, 0, f'Please review the languages supported by the Deep Translate service\n'
-                                            f'https://wordhoard.readthedocs.io/en/latest/translations/deepl_supported_translation_languages/'))
+            colorized_text(f'The language provided is not one of the supported languages for the '
+                           f'Deep Translation service.', 'red')
+            colorized_text(f'Requested language: {self._source_language}', 'red')
+            colorized_text(f'Please review the languages supported by the Deep Translate service\n'
+                           f'https://wordhoard.readthedocs.io/en/latest/translations'
+                           f'/deepl_supported_translation_languages/', 'green')
             return None
 
     def reverse_translate(self) -> str:
         """
         This function is used to translate a word from American English into another language, such as Spanish.
 
         :return: translated word
```

### Comparing `wordhoard-1.5.3/wordhoard/utilities/email_address_verification.py` & `wordhoard-1.5.4/wordhoard/utilities/email_address_verification.py`

 * *Files identical despite different names*

### Comparing `wordhoard-1.5.3/wordhoard/utilities/exceptions.py` & `wordhoard-1.5.4/wordhoard/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `wordhoard-1.5.3/wordhoard/utilities/google_translator.py` & `wordhoard-1.5.4/wordhoard/utilities/google_translator.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 # purpose.
 ##################################################################################
 
 ##################################################################################
 # Date Completed: September 24, 2021
 # Author: John Bumgarner
 #
-# Date Last Revised: March 04, 2023
+# Date Last Revised: May 31, 2023
 # Revised by: John Bumgarner
 ##################################################################################
 
 ##################################################################################
 # Python imports required for basic operations
 ##################################################################################
 import logging
@@ -76,17 +76,16 @@
         # Establishes a rate limit for making requests to the Google translation service
         limiter = limits(calls=60, period=60)
         self.translate_word = handler(limiter(self.translate_word))
         self.reverse_translate = handler(limiter(self.reverse_translate))
 
     def _backoff_handler(self):
         if self._rate_limit_status is False:
-            print(colorized_text(255, 0, 0,
-                                 'The Google Translation service query rate Limit was reached. The querying '
-                                 'process is entering a temporary hibernation mode.'))
+            colorized_text('The Google Translation service query rate Limit was reached. The querying '
+                           'process is entering a temporary hibernation mode.', 'red')
             logger.info('The Google Translation service query rate limit was reached.')
             self._rate_limit_status = True
 
     def _google_supported_languages(self) -> Union[str, None]:
         """
         This function determines if the requested source language is
         one supported languages for the Google Translator.
@@ -159,15 +158,15 @@
                 raise RequestException()
             else:
                 soup = BeautifulSoup(response.text, 'html.parser')
                 if soup.find('div', {"class": "result-container"}):
                     translated_word = soup.find('div', {"class": "result-container"})
                     return translated_word.text
                 else:
-                    print(colorized_text(255, 0, 0, f'Google could not translate the word {self._str_to_translate}'))
+                    colorized_text(f'Google could not translate the word {self._str_to_translate}', 'magenta')
                     return None
 
         except ElementNotFoundException as error:
             """
             The exception is thrown if the requested HTML element was not found in the body element being 
             parsed by BeautifulSoup.
             """
@@ -183,28 +182,26 @@
             logger.error(''.join(traceback.format_tb(error.__traceback__)))
 
         except TooManyRequestsException as error:
             """
             This exception is thrown when the maximum number of connection requests have been exceeded for a 
             specific time for the Google Translation service.
             """
-            print(colorized_text(255, 0, 0, 'There has been too many connection requests to the Google '
-                                            'Translation service.'))
+            colorized_text('There has been too many connection requests to the Google Translation service.', 'red')
             logger.error('Connection Request Error:')
             logger.error('There has been too many connection requests to the Google Translation service.')
             logger.error(''.join(traceback.format_tb(error.__traceback__)))
 
         except RequestException as error:
             """
             This exception is thrown when an ambiguous exception occurs during a connection to the 
             Google Translation service.
             """
-            print(colorized_text(255, 0, 0, 'An ambiguous connection exception has occurred when contacting the'
-                                            'Google Translation service.  Please check the WordHoard log file '
-                                            'for additional information.'))
+            colorized_text('An ambiguous connection exception has occurred when contacting theGoogle Translation '
+                           'service.  Please check the WordHoard log file for additional information.', 'red')
             logger.error('Connection Exception:')
             logger.error('An ambiguous connection exception has occurred when communicating with the '
                          'Google Translation service.')
             logger.error(''.join(traceback.format_tb(error.__traceback__)))
 
     def _google_translate_reverse(self) -> Union[str, None]:
         """
@@ -230,15 +227,15 @@
                 raise RequestException()
             else:
                 soup = BeautifulSoup(response.text, 'html.parser')
                 if soup.find('div', {"class": "result-container"}):
                     translated_word = soup.find('div', {"class": "result-container"})
                     return translated_word.text
                 else:
-                    print(colorized_text(255, 0, 0, f'Google could not translate the word {self._str_to_translate}'))
+                    colorized_text(f'Google could not translate the word {self._str_to_translate}', 'magenta')
                     return None
 
         except ElementNotFoundException as error:
             """
             This exception is thrown if the requested HTML element was not found in the body element being 
             parsed by BeautifulSoup.
             """
@@ -254,28 +251,26 @@
             logger.error(''.join(traceback.format_tb(error.__traceback__)))
 
         except TooManyRequestsException as error:
             """
             This exception is thrown when the maximum number of connection requests have been exceeded for a 
             specific time for the Google Translation service.
             """
-            print(colorized_text(255, 0, 0, 'There has been too many connection requests to the Google '
-                                            'Translation service.'))
+            colorized_text('There has been too many connection requests to the Google Translation service.', 'red')
             logger.error('Connection Request Error:')
             logger.error('There has been too many connection requests to the Google Translation service.')
             logger.error(''.join(traceback.format_tb(error.__traceback__)))
 
         except RequestException as error:
             """
             This exception is thrown when an ambiguous exception occurs during a connection to the 
             Google Translation service.
             """
-            print(colorized_text(255, 0, 0, 'An ambiguous connection exception has occurred when contacting the'
-                                            'Google Translation service.  Please check the WordHoard log file '
-                                            'for additional information.'))
+            colorized_text('An ambiguous connection exception has occurred when contacting the Google Translation '
+                           'service.  Please check the WordHoard log file for additional information.', 'red')
             logger.error('Connection Exception:')
             logger.error('An ambiguous connection exception has occurred when communicating with the '
                          'Google Translation service.')
             logger.error(''.join(traceback.format_tb(error.__traceback__)))
 
     def translate_word(self) -> Union[str, None]:
         """
@@ -285,19 +280,20 @@
         :return: translated word
         :rtype: string
         """
         supported_language = self._google_supported_languages()
         if supported_language:
             return self._google_translate(supported_language)
         elif not supported_language:
-            print(colorized_text(255, 0, 0, f'The language provided is not one of the supported languages '
-                                            f'for the Google Translation service.'))
-            print(colorized_text(255, 0, 0, f'Requested language: {self._source_language}'))
-            print(colorized_text(255, 0, 0, f'Please review the languages supported by the Google Translation service\n'
-                                            f'https://wordhoard.readthedocs.io/en/latest/translations/google_supported_translation_languages/'))
+            colorized_text(f'The language provided is not one of the supported languages for the '
+                           f'Google Translation service.', 'red')
+            colorized_text(f'Requested language: {self._source_language}', 'red')
+            colorized_text(f'Please review the languages supported by the Google Translation service\n'
+                           f'https://wordhoard.readthedocs.io/en/latest/translations'
+                           f'/google_supported_translation_languages/', 'green')
             return None
 
     def reverse_translate(self) -> str:
         """
         This function is used to translate a word from American English into
         another language, such as Spanish.
```

### Comparing `wordhoard-1.5.3/wordhoard/utilities/mymemory_translator.py` & `wordhoard-1.5.4/wordhoard/utilities/mymemory_translator.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 # purpose.
 ##################################################################################
 
 ##################################################################################
 # Date Completed: September 24, 2021
 # Author: John Bumgarner
 #
-# Date Last Revised: February 12, 2023
+# Date Last Revised: May 31, 2023
 # Revised by: John Bumgarner
 ##################################################################################
 
 ##################################################################################
 # Python imports required for basic operations
 ##################################################################################
 import sys
@@ -82,17 +82,16 @@
         # Establishes a rate limit for making requests to the MyMemory translation service
         limiter = limits(calls=30, period=60)
         self.translate_word = handler(limiter(self.translate_word))
         self.reverse_translate = handler(limiter(self.reverse_translate))
 
     def _backoff_handler(self):
         if self._rate_limit_status is False:
-            print(colorized_text(255, 0, 0,
-                                 'The MyMemory translation service query rate Limit was reached. The querying '
-                                 'process is entering a temporary hibernation mode.'))
+            colorized_text('The MyMemory translation service query rate Limit was reached. The querying '
+                           'process is entering a temporary hibernation mode.', 'red')
             logger.info('The MyMemory translation service query rate limit was reached.')
             self._rate_limit_status = True
 
     def _mymemory_supported_languages(self) -> Union[str, None]:
         """
         This function determines if the requested source language is
         one supported languages for the MyMemory Translator.
@@ -146,17 +145,15 @@
 
         :param original_language: language to translated from
         :return: translated word
         :rtype: string or None
         """
         try:
             if validate_address(self._email_address) is False:
-                print(colorized_text(255, 0, 0,
-                                     'A valid email address is required to use the MyMemory Translation '
-                                     'service.'))
+                colorized_text('A valid email address is required to use the MyMemory Translation service.', 'red')
                 sys.exit(1)
             elif validate_address(self._email_address) is True:
                 response = self._requests_retry_session().get(self._url_to_query,
                                                               params={'langpair': f'{original_language}|en-us',
                                                                       'q': self._str_to_translate,
                                                                       'de': self._email_address},
                                                               headers=self._headers,
@@ -168,16 +165,15 @@
                     # sent too many requests in a given amount of time ("rate limiting")
                     raise TooManyRequestsException()
                 elif response.status_code != 200:
                     raise RequestException()
                 else:
                     data = response.json()
                     if not data:
-                        print(colorized_text(255, 0, 0,f'MyMemory could not translate the word '
-                                                       f'{self._str_to_translate}.'))
+                        colorized_text(f'MyMemory could not translate the word {self._str_to_translate}.', 'magenta')
                         return None
 
                     else:
                         translation = data.get('responseData').get('translatedText')
                         if translation == 'INVALID EMAIL PROVIDED':
                             raise InvalidEmailAddressException()
                         elif translation:
@@ -187,67 +183,63 @@
             """
             This exception is thrown when the email address provided for authentication to the MyMemory Translation 
             service is invalid. 
             
             Please note that the MyMemory Translation service only validates the format of the email address and 
             not the validity of the address provided.
             """
-            print(colorized_text(255, 0, 0, 'The email address provided for authentication to the MyMemory '
-                                            'Translation service is invalid.'))
+            colorized_text('The email address provided for authentication to the MyMemory Translation service '
+                           'is invalid.', 'red')
             logger.error('Invalid Email Address Error:')
             logger.error('The email address provided for authentication to the MyMemory Translation service '
                          'is invalid.')
             logger.error(''.join(traceback.format_tb(error.__traceback__)))
 
         except InvalidLengthException as error:
             """
             This exception is thrown if the provided text exceed the length limit of the MyMemory Translator service.
             """
-            print(colorized_text(255, 0, 0, f'The text length for the word: {self._str_to_translate} '
-                                            f'exceed the length limit of MyMemory translation service.'))
+            colorized_text(f'The text length for the word: {self._str_to_translate} exceed the length limit '
+                           f'of MyMemory translation service.', 'red')
             logger.error(f'The text length for the word: {self._str_to_translate} exceed the length limit of '
                          f'MyMemory Translation service.')
             logger.error(''.join(traceback.format_tb(error.__traceback__)))
 
         except TooManyRequestsException as error:
             """
             This exception is thrown when the maximum number of connection requests have been exceeded for a 
             specific time for the MyMemory Translation service.
             """
-            print(colorized_text(255, 0, 0, 'There has been too many connection requests to the MyMemory '
-                                            'Translation service.'))
+            colorized_text('There has been too many connection requests to the MyMemory Translation service.', 'red')
             logger.error('Connection Request Error:')
             logger.error('There has been too many connection requests to the MyMemory Translation service.')
             logger.error(''.join(traceback.format_tb(error.__traceback__)))
 
         except RequestException as error:
             """
             This exception is thrown when an ambiguous exception occurs during a connection to the 
             MyMemory Translation service.
             """
-            print(colorized_text(255, 0, 0, 'An ambiguous connection exception has occurred when contacting the'
-                                            'MyMemory Translation service.  Please check the WordHoard log file '
-                                            'for additional information.'))
+            colorized_text('An ambiguous connection exception has occurred when contacting the MyMemory Translation '
+                           'service.  Please check the WordHoard log file for additional information.', 'red')
             logger.error('Connection Exception:')
             logger.error('An ambiguous connection exception has occurred when communicating with the '
                          'MyMemory Translation service.')
             logger.error(''.join(traceback.format_tb(error.__traceback__)))
 
     def _mymemory_translate_reverse(self) -> Union[str, None]:
         """
         This function is used to translate a word from it source language, such as Spanish into American English.
 
         :return: translated word
         :rtype: string or None
         """
         try:
             if validate_address(self._email_address) is False:
-                print(colorized_text(255, 0, 0,
-                                     'A valid email address is required to use the MyMemory Translation '
-                                     'service.'))
+                colorized_text('A valid email address is required to use the MyMemory Translation service.', 'red')
                 sys.exit(1)
             elif validate_address(self._email_address) is True:
                 response = self._requests_retry_session().get(self._url_to_query,
                                                               params={'langpair': f'en-us|{self._source_language}',
                                                                       'q': self._str_to_translate,
                                                                       'de': self._email_address},
                                                               headers=self._headers,
@@ -259,16 +251,15 @@
                     # sent too many requests in a given amount of time ("rate limiting")
                     raise TooManyRequestsException()
                 elif response.status_code != 200:
                     raise RequestException()
                 else:
                     data = response.json()
                     if not data:
-                        print(colorized_text(255, 0, 0, f'MyMemory could not translate the word '
-                                                        f'{self._str_to_translate}.'))
+                        colorized_text(f'MyMemory could not translate the word {self._str_to_translate}.', 'red')
                         return None
 
                     else:
                         translation = data.get('responseData').get('translatedText')
                         if translation == 'INVALID EMAIL PROVIDED':
                             raise InvalidEmailAddressException()
                         elif translation:
@@ -278,51 +269,49 @@
             """
             This exception is thrown when the email address provided for authentication to the MyMemory Translation 
             service is invalid. 
             
             Please note that the MyMemory Translation service only validates the format of the email address and 
             not the validity of the address provided.
             """
-            print(colorized_text(255, 0, 0, 'The email address provided for authentication to the MyMemory '
-                                            'Translation is invalid.'))
+            colorized_text('The email address provided for authentication to the MyMemory Translation is invalid.',
+                           'red')
             logger.error('Invalid Email Address Error:')
             logger.error('The email address provided for authentication to the MyMemory Translation '
                          'is invalid.')
             logger.error(''.join(traceback.format_tb(error.__traceback__)))
             sys.exit(1)
 
         except InvalidLengthException as error:
             """
             This exception is thrown if the provided text exceed the length limit of the MyMemory Translator service.
             """
-            print(colorized_text(255, 0, 0, f'The text length for the word: {self._str_to_translate} '
-                                            f'exceed the length limit of MyMemory translation service.'))
+            colorized_text(f'The text length for the word: {self._str_to_translate} exceed the length limit '
+                           f'of MyMemory translation service.', 'red')
             logger.error(f'The text length for the word: {self._str_to_translate} exceed the length limit of '
                          f'MyMemory translation service.')
             logger.error(''.join(traceback.format_tb(error.__traceback__)))
 
         except TooManyRequestsException as error:
             """
             This exception is thrown when the maximum number of connection requests have been exceeded for a 
             specific time for the MyMemory Translation service.
             """
-            print(colorized_text(255, 0, 0, 'There has been too many connection requests to the MyMemory '
-                                            'Translation service.'))
+            colorized_text('There has been too many connection requests to the MyMemory Translation service.', 'red')
             logger.error('Connection Request Error:')
             logger.error('There has been too many connection requests to the MyMemory Translation service.')
             logger.error(''.join(traceback.format_tb(error.__traceback__)))
 
         except RequestException as error:
             """
             This exception is thrown when an ambiguous exception occurs during a connection to the 
             MyMemory Translation service.
             """
-            print(colorized_text(255, 0, 0, 'An ambiguous connection exception has occurred when contacting the'
-                                            'MyMemory Translation service.  Please check the WordHoard log file '
-                                            'for additional information.'))
+            colorized_text('An ambiguous connection exception has occurred when contacting the MyMemory Translation '
+                           'service.  Please check the WordHoard log file for additional information.', 'red')
             logger.error('Connection Exception:')
             logger.error('An ambiguous connection exception has occurred when communicating with the '
                          'MyMemory Translation service.')
             logger.error(''.join(traceback.format_tb(error.__traceback__)))
 
     def translate_word(self) -> Union[str, None]:
         """
@@ -331,19 +320,20 @@
         :return: translated word
         :rtype: string
         """
         supported_language = self._mymemory_supported_languages()
         if supported_language:
             return self._mymemory_translate(supported_language)
         elif not supported_language:
-            print(colorized_text(255, 0, 0, f'The language provided is not one of the supported languages '
-                                            f'for the MyMemory Translation service.'))
-            print(colorized_text(255, 0, 0, f'Requested language: {self._source_language}'))
-            print(colorized_text(255, 0, 0, f'Please review the languages supported by the MyMemory Translate service\n'
-                                            f'https://wordhoard.readthedocs.io/en/latest/translations/mymemory_supported_translation_languages/'))
+            colorized_text(f'The language provided is not one of the supported languages for the MyMemory '
+                           f'Translation service.', 'red')
+            colorized_text(f'Requested language: {self._source_language}', 'red')
+            colorized_text(f'Please review the languages supported by the MyMemory Translate service\n'
+                           f'https://wordhoard.readthedocs.io/en/latest/translations'
+                           f'/mymemory_supported_translation_languages/', 'green')
 
             return None
 
     def reverse_translate(self) -> Union[str, None]:
         """
         This function is used to translate a word from American English into another language, such as Spanish.
```

### Comparing `wordhoard-1.5.3/wordhoard/utilities/request_html.py` & `wordhoard-1.5.4/wordhoard/utilities/request_html.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # purpose.
 ##################################################################################
 
 ##################################################################################
 # Date Completed: October 15, 2020
 # Author: John Bumgarner
 #
-# Date Last Revised: March 18, 2023
+# Date Last Revised: May 31, 2023
 # Revised by: John Bumgarner
 ##################################################################################
 
 ##################################################################################
 # Python imports required for basic operations
 ##################################################################################
 import sys
@@ -150,106 +150,95 @@
                 logger.error(f'Response Status Code: {response.status_code}')
                 logger.info(
                     'The HTTP 404 Not Found status code means that the file or page that the was requested '
                     'was not found on the server')
                 logger.info(f'Requested URL: {self._url_to_scrape}')
                 logger.info('-' * 80)
             elif response.status_code == 500:
-                print(colorized_text(255, 0, 0,
-                                     'An HTTP 500 Internal Server Error has occurred.'
-                                     '\nPlease review the WordHoard logs for additional information.'))
+                colorized_text('An HTTP 500 Internal Server Error has occurred.'
+                               '\nPlease review the WordHoard logs for additional information.', 'red')
                 logger.info('-' * 80)
                 logger.error(f'Response Status Code: {response.status_code}')
                 logger.info(
                     "The HTTP 500 Internal Server Error status code indicates that the server encountered "
                     "an unexpected condition that prevented it from fulfilling the request.")
                 logger.info(f'Requested URL: {self._url_to_scrape}')
                 logger.info('-' * 80)
             elif response.status_code == 503:
-                print(colorized_text(255, 0, 0,
-                                     'A 503 Service Unavailable status code has been detected.'
-                                     '\nPlease review the WordHoard logs for additional information.'))
+                colorized_text('A 503 Service Unavailable status code has been detected.'
+                               '\nPlease review the WordHoard logs for additional information.', 'red')
                 logger.info('-' * 80)
                 logger.error(f'Response Status Code: {response.status_code}')
                 logger.info(
                     "The 503 Service Unavailable status code indicates that the server is temporarily unable "
                     "to handle the request")
                 logger.error(f'Requested URL: {self._url_to_scrape}')
                 logger.info('-' * 80)
             elif response.status_code == 504:
-                print(colorized_text(255, 0, 0,
-                                     'An HTTP 504 Gateway Timeout Error status code has been detected.'
-                                     '\nPlease review the WordHoard logs for additional information.'))
+                colorized_text('An HTTP 504 Gateway Timeout Error status code has been detected.'
+                               '\nPlease review the WordHoard logs for additional information.', 'red')
                 logger.info('-' * 80)
                 logger.error(f'Response Status Code: {response.status_code}')
                 logger.info(
                     "The HTTP 504 Gateway Timeout Error status code indicating that a server, which is "
                     "currently acting as a gateway or proxy, did not receive a timely response "
                     "from another server")
                 logger.error(f'Requested URL: {self._url_to_scrape}')
                 logger.info('-' * 80)
             elif response.status_code == 521:
-                print(colorized_text(255, 0, 0,
-                                     'A 521 status code has been detected. This code is often used by CloudFlare.'
-                                     '\nPlease review the WordHoard logs for additional information.'))
+                colorized_text('A 521 status code has been detected. This code is often used by CloudFlare.'
+                               '\nPlease review the WordHoard logs for additional information.', 'red')
                 logger.info('-' * 80)
                 logger.error(f'Response Status Code: {response.status_code}')
                 logger.info("This status code is not specified in any RFCs, but is used by CloudFlare's"
                             "reverse proxies to indicate that the origin webserver refused the connection")
                 logger.info(f'Requested URL: {self._url_to_scrape}')
                 logger.info('-' * 80)
             else:
                 if response.status_code != 200:
-                    print(colorized_text(255, 0, 0,
-                                         f'The Status Code: {response.status_code} has been detected.'
-                                         '\nPlease review the WordHoard logs for additional information.'))
+                    colorized_text(f'The Status Code: {response.status_code} has been detected.'
+                                   '\nPlease review the WordHoard logs for additional information.', 'red')
                     logger.error(f'Response Status Code: {response.status_code}')
                     logger.info(f'Requested URL: {self._url_to_scrape}')
                     logger.info('-' * 80)
 
         except requests.HTTPError as error:
-            print(colorized_text(255, 0, 0,
-                                 'A HTTPError has occurred.'
-                                 '\nPlease review the WordHoard logs for additional information.'))
+            colorized_text('A HTTPError has occurred.'
+                           '\nPlease review the WordHoard logs for additional information.', 'red')
             logger.error(f'A HTTPError has occurred when requesting {self._url_to_scrape}')
             logger.error(''.join(traceback.format_tb(error.__traceback__)))
             sys.exit(1)
         except requests.URLRequired as error:
             logger.error(f'A URLRequired has occurred when requesting {self._url_to_scrape}')
             logger.error(''.join(traceback.format_tb(error.__traceback__)))
             sys.exit(1)
         except requests.exceptions.ProxyError as error:
-            print(colorized_text(255, 0, 0,
-                                 'A unknown type of Proxy Error has occurred.'
-                                 '\nPlease verify that your proxies are working.'))
+            colorized_text('A unknown type of Proxy Error has occurred.'
+                           '\nPlease verify that your proxies are working.', 'red')
             logger.error(f'A ProxyError has occurred when requesting {self._url_to_scrape}')
             logger.error(''.join(traceback.format_tb(error.__traceback__)))
             sys.exit(1)
         except MaxRetryError as error:
-            print(colorized_text(255, 0, 0,
-                                 'The max number of connection retries was exceeded.'
-                                 '\nPlease review the WordHoard logs for additional information.'))
+            colorized_text('The max number of connection retries was exceeded.'
+                           '\nPlease review the WordHoard logs for additional information.', 'red')
             logger.error(f'A MaxRetryError has occurred when requesting {self._url_to_scrape}')
             logger.error(''.join(traceback.format_tb(error.__traceback__)))
             sys.exit(1)
         except requests.ConnectionError as error:
-            print(colorized_text(255, 0, 0,
-                                 'A ConnectionError has occurred.'
-                                 '\nPlease review the WordHoard logs for additional information.'))
+            colorized_text('A ConnectionError has occurred.'
+                           '\nPlease review the WordHoard logs for additional information.', 'red')
             logger.error(f'A ConnectionError has occurred when requesting {self._url_to_scrape}')
             logger.error(''.join(traceback.format_tb(error.__traceback__)))
             sys.exit(1)
         except requests.Timeout as error:
-            print(colorized_text(255, 0, 0,
-                                 'A connection timeout has occurred.'
-                                 '\nPlease review the WordHoard logs for additional information.'))
+            colorized_text('A connection timeout has occurred.'
+                           '\nPlease review the WordHoard logs for additional information.', 'red')
             logger.error(f'A Timeout has occurred when requesting {self._url_to_scrape}')
             logger.error(''.join(traceback.format_tb(error.__traceback__)))
             sys.exit(1)
         except requests.RequestException as error:
-            print(colorized_text(255, 0, 0,
-                                 'A RequestException has occurred.'
-                                 '\nPlease review the WordHoard logs for additional information.'))
+            colorized_text('A RequestException has occurred.'
+                           '\nPlease review the WordHoard logs for additional information.', 'red')
             logger.error(f'A RequestException has occurred when requesting {self._url_to_scrape}')
             logger.error(''.join(traceback.format_tb(error.__traceback__)))
             sys.exit(1)
         return response
```

### Comparing `wordhoard-1.5.3/wordhoard/utilities/translator_languages.py` & `wordhoard-1.5.4/wordhoard/utilities/translator_languages.py`

 * *Files identical despite different names*

### Comparing `wordhoard-1.5.3/wordhoard/utilities/user_agents.py` & `wordhoard-1.5.4/wordhoard/utilities/user_agents.py`

 * *Files identical despite different names*

### Comparing `wordhoard-1.5.3/wordhoard/utilities/word_verification.py` & `wordhoard-1.5.4/wordhoard/utilities/word_verification.py`

 * *Files identical despite different names*

### Comparing `wordhoard-1.5.3/wordhoard/utilities/wordhoard_logger.py` & `wordhoard-1.5.4/wordhoard/utilities/wordhoard_logger.py`

 * *Files identical despite different names*

### Comparing `wordhoard-1.5.3/wordhoard.egg-info/PKG-INFO` & `wordhoard-1.5.4/wordhoard.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wordhoard
-Version: 1.5.3
+Version: 1.5.4
 Summary: A comprehensive lexical discovery application that is useful for finding semantic relationships such as, the antonyms, synonyms, hypernyms, hyponyms, homophones and definitions for a specific word.
 Home-page: https://github.com/johnbumgarner/wordhoard
 Author: John Bumgarner
 Author-email: wordhoardproject@gmail.com
 License: LICENSE.txt
 Keywords: antonyms,bag of words,definitions,hypernyms,hyponyms,homophones,information retrieval,lexicon,semantic relationships,synonyms,natural language processing
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,14 +12,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: General
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,25 +1,26 @@
-Metadata-Version: 2.1 Name: wordhoard Version: 1.5.3 Summary: A comprehensive
+Metadata-Version: 2.1 Name: wordhoard Version: 1.5.4 Summary: A comprehensive
 lexical discovery application that is useful for finding semantic relationships
 such as, the antonyms, synonyms, hypernyms, hyponyms, homophones and
 definitions for a specific word. Home-page: https://github.com/johnbumgarner/
 wordhoard Author: John Bumgarner Author-email: wordhoardproject@gmail.com
 License: LICENSE.txt Keywords: antonyms,bag of
 words,definitions,hypernyms,hyponyms,homophones,information
 retrieval,lexicon,semantic relationships,synonyms,natural language processing
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3.6 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Topic :: Software Development :: Libraries :: Python Modules Classifier: Topic
-:: Text Processing :: General Classifier: Topic :: Text Processing ::
-Linguistic Classifier: Topic :: Utilities Requires-Python: >=3.6 Description-
-Content-Type: text/markdown License-File: LICENSE # Primary Use Case
+Programming Language :: Python :: 3.10 Classifier: Topic :: Software
+Development :: Libraries :: Python Modules Classifier: Topic :: Text Processing
+:: General Classifier: Topic :: Text Processing :: Linguistic Classifier: Topic
+:: Utilities Requires-Python: >=3.6 Description-Content-Type: text/markdown
+License-File: LICENSE # Primary Use Case
 Textual analysis is a broad term for various research methodologies used to
 qualitatively describe, interpret and understand text data. These methodologies
 are mainly used in academic research to analyze content related to media and
 communication studies, popular culture, sociology, and philosophy. Textual
 analysis allows these researchers to quickly obtain relevant insights from
 unstructured data. All types of information can be gleaned from textual data,
 especially from social media posts or news articles. Some of this information
```

### Comparing `wordhoard-1.5.3/wordhoard.egg-info/SOURCES.txt` & `wordhoard-1.5.4/wordhoard.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 setup.py
+wordhoard/.DS_Store
 wordhoard/__init__.py
 wordhoard/antonyms.py
 wordhoard/dictionary.py
 wordhoard/homophones.py
 wordhoard/hypernyms.py
 wordhoard/hyponyms.py
 wordhoard/synonyms.py
```

