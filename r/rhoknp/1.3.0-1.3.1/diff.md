# Comparing `tmp/rhoknp-1.3.0.tar.gz` & `tmp/rhoknp-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rhoknp-1.3.0.tar", max compression
+gzip compressed data, was "rhoknp-1.3.1.tar", max compression
```

## Comparing `rhoknp-1.3.0.tar` & `rhoknp-1.3.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0     1073 2022-07-07 05:13:45.612050 rhoknp-1.3.0/LICENSE
--rw-r--r--   0        0        0     6528 2023-05-01 10:39:22.233408 rhoknp-1.3.0/README.md
--rw-r--r--   0        0        0     1609 2023-05-01 10:39:22.239539 rhoknp-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      474 2023-01-23 11:06:01.235960 rhoknp-1.3.0/src/rhoknp/__init__.py
--rw-r--r--   0        0        0      293 2023-01-25 04:22:29.044533 rhoknp-1.3.0/src/rhoknp/cli/__init__.py
--rw-r--r--   0        0        0     3334 2023-05-01 10:39:22.239944 rhoknp-1.3.0/src/rhoknp/cli/cli.py
--rw-r--r--   0        0        0     6802 2023-05-01 10:39:22.240180 rhoknp-1.3.0/src/rhoknp/cli/serve.py
--rw-r--r--   0        0        0     5782 2023-05-01 10:39:22.240529 rhoknp-1.3.0/src/rhoknp/cli/show.py
--rw-r--r--   0        0        0      823 2023-05-01 10:39:22.240711 rhoknp-1.3.0/src/rhoknp/cli/static/css/style.css
--rw-r--r--   0        0        0     9898 2023-05-01 10:39:22.241416 rhoknp-1.3.0/src/rhoknp/cli/static/images/apple-touch-icon.png
--rw-r--r--   0        0        0    15086 2023-05-01 10:39:22.242054 rhoknp-1.3.0/src/rhoknp/cli/static/images/favicon.ico
--rw-r--r--   0        0        0     1960 2023-05-01 10:39:22.242198 rhoknp-1.3.0/src/rhoknp/cli/static/js/script.js
--rw-r--r--   0        0        0     1779 2023-01-23 11:06:01.236808 rhoknp-1.3.0/src/rhoknp/cli/stats.py
--rw-r--r--   0        0        0     1705 2023-05-01 10:39:22.242748 rhoknp-1.3.0/src/rhoknp/cli/templates/base.jinja2
--rw-r--r--   0        0        0      724 2023-05-01 10:39:22.242904 rhoknp-1.3.0/src/rhoknp/cli/templates/components/dependency_parsing.jinja2
--rw-r--r--   0        0        0     1840 2023-05-01 10:39:22.243108 rhoknp-1.3.0/src/rhoknp/cli/templates/components/discourse_parsing.jinja2
--rw-r--r--   0        0        0      276 2023-05-01 10:39:22.243247 rhoknp-1.3.0/src/rhoknp/cli/templates/components/error.jinja2
--rw-r--r--   0        0        0      344 2023-05-01 10:39:22.243341 rhoknp-1.3.0/src/rhoknp/cli/templates/components/form.jinja2
--rw-r--r--   0        0        0      136 2023-05-01 10:39:22.243485 rhoknp-1.3.0/src/rhoknp/cli/templates/components/hide_all_button.jinja2
--rw-r--r--   0        0        0     1987 2023-05-01 10:39:22.243568 rhoknp-1.3.0/src/rhoknp/cli/templates/components/morphological_analysis.jinja2
--rw-r--r--   0        0        0     1063 2023-05-01 10:39:22.243719 rhoknp-1.3.0/src/rhoknp/cli/templates/components/named_entity_recognition.jinja2
--rw-r--r--   0        0        0      163 2023-05-01 10:39:22.243791 rhoknp-1.3.0/src/rhoknp/cli/templates/components/navbar.jinja2
--rw-r--r--   0        0        0       63 2023-05-01 10:39:22.244032 rhoknp-1.3.0/src/rhoknp/cli/templates/components/raw_input.jinja2
--rw-r--r--   0        0        0      636 2023-05-01 10:39:22.244218 rhoknp-1.3.0/src/rhoknp/cli/templates/components/raw_output.jinja2
--rw-r--r--   0        0        0      131 2023-05-01 10:39:22.244412 rhoknp-1.3.0/src/rhoknp/cli/templates/components/show_all_button.jinja2
--rw-r--r--   0        0        0     1034 2023-05-01 10:39:22.244575 rhoknp-1.3.0/src/rhoknp/cli/templates/components/typo_correction.jinja2
--rw-r--r--   0        0        0      722 2023-05-01 10:39:22.244665 rhoknp-1.3.0/src/rhoknp/cli/templates/components/word_splitting.jinja2
--rw-r--r--   0        0        0      333 2023-05-01 10:39:22.244808 rhoknp-1.3.0/src/rhoknp/cli/templates/jumanpp.jinja2
--rw-r--r--   0        0        0      526 2023-05-01 10:39:22.244946 rhoknp-1.3.0/src/rhoknp/cli/templates/knp.jinja2
--rw-r--r--   0        0        0      643 2023-05-01 10:39:22.245089 rhoknp-1.3.0/src/rhoknp/cli/templates/kwja.jinja2
--rw-r--r--   0        0        0      826 2023-01-23 11:06:01.237203 rhoknp-1.3.0/src/rhoknp/cohesion/__init__.py
--rw-r--r--   0        0        0     6744 2023-02-07 06:49:22.772304 rhoknp-1.3.0/src/rhoknp/cohesion/argument.py
--rw-r--r--   0        0        0     9899 2023-02-07 06:49:22.772615 rhoknp-1.3.0/src/rhoknp/cohesion/coreference.py
--rw-r--r--   0        0        0     9566 2023-01-23 11:06:01.238718 rhoknp-1.3.0/src/rhoknp/cohesion/discourse.py
--rw-r--r--   0        0        0     2427 2023-01-23 11:06:01.239467 rhoknp-1.3.0/src/rhoknp/cohesion/exophora.py
--rw-r--r--   0        0        0    10329 2023-02-07 06:49:22.772957 rhoknp-1.3.0/src/rhoknp/cohesion/pas.py
--rw-r--r--   0        0        0     2595 2023-01-23 11:06:01.239969 rhoknp-1.3.0/src/rhoknp/cohesion/predicate.py
--rw-r--r--   0        0        0     4716 2023-01-23 11:06:01.240472 rhoknp-1.3.0/src/rhoknp/cohesion/rel.py
--rw-r--r--   0        0        0      226 2023-01-23 11:06:01.240680 rhoknp-1.3.0/src/rhoknp/processors/__init__.py
--rw-r--r--   0        0        0     5264 2023-05-01 10:39:22.245299 rhoknp-1.3.0/src/rhoknp/processors/jumanpp.py
--rw-r--r--   0        0        0     7027 2023-05-01 10:39:22.245466 rhoknp-1.3.0/src/rhoknp/processors/knp.py
--rw-r--r--   0        0        0     5617 2023-05-01 10:39:22.245819 rhoknp-1.3.0/src/rhoknp/processors/kwja.py
--rw-r--r--   0        0        0     2984 2022-10-29 15:30:49.159597 rhoknp-1.3.0/src/rhoknp/processors/processor.py
--rw-r--r--   0        0        0     3070 2023-05-01 10:39:22.245994 rhoknp-1.3.0/src/rhoknp/processors/senter.py
--rw-r--r--   0        0        0      378 2023-01-23 11:06:01.241792 rhoknp-1.3.0/src/rhoknp/props/__init__.py
--rw-r--r--   0        0        0      210 2022-10-24 08:19:10.843963 rhoknp-1.3.0/src/rhoknp/props/dependency.py
--rw-r--r--   0        0        0     1996 2023-01-23 11:06:01.242202 rhoknp-1.3.0/src/rhoknp/props/feature.py
--rw-r--r--   0        0        0      863 2023-01-23 11:06:01.242583 rhoknp-1.3.0/src/rhoknp/props/memo.py
--rw-r--r--   0        0        0     2917 2023-02-07 06:49:22.773596 rhoknp-1.3.0/src/rhoknp/props/named_entity.py
--rw-r--r--   0        0        0     1633 2023-01-23 11:06:01.243129 rhoknp-1.3.0/src/rhoknp/props/semantics.py
--rw-r--r--   0        0        0        0 2022-07-07 07:10:30.837345 rhoknp-1.3.0/src/rhoknp/py.typed
--rw-r--r--   0        0        0      337 2023-01-23 11:06:01.243840 rhoknp-1.3.0/src/rhoknp/units/__init__.py
--rw-r--r--   0        0        0    14479 2023-03-03 06:23:17.602965 rhoknp-1.3.0/src/rhoknp/units/base_phrase.py
--rw-r--r--   0        0        0     7740 2023-02-07 06:49:22.774401 rhoknp-1.3.0/src/rhoknp/units/clause.py
--rw-r--r--   0        0        0    15809 2023-02-07 06:49:22.774863 rhoknp-1.3.0/src/rhoknp/units/document.py
--rw-r--r--   0        0        0    11875 2023-02-07 06:49:22.775146 rhoknp-1.3.0/src/rhoknp/units/morpheme.py
--rw-r--r--   0        0        0     7202 2023-02-07 06:49:22.775468 rhoknp-1.3.0/src/rhoknp/units/phrase.py
--rw-r--r--   0        0        0    18039 2023-05-01 10:39:22.246566 rhoknp-1.3.0/src/rhoknp/units/sentence.py
--rw-r--r--   0        0        0     1521 2023-01-23 11:06:01.246571 rhoknp-1.3.0/src/rhoknp/units/unit.py
--rw-r--r--   0        0        0        0 2023-01-23 11:06:01.246629 rhoknp-1.3.0/src/rhoknp/utils/__init__.py
--rw-r--r--   0        0        0     3783 2023-05-01 10:39:22.247129 rhoknp-1.3.0/src/rhoknp/utils/reader.py
--rw-r--r--   0        0        0     1112 2023-05-01 10:39:22.247398 rhoknp-1.3.0/src/rhoknp/utils/util.py
--rw-r--r--   0        0        0     7785 1970-01-01 00:00:00.000000 rhoknp-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2022-07-07 05:13:45.612050 rhoknp-1.3.1/LICENSE
+-rw-r--r--   0        0        0     6528 2023-06-01 10:08:32.507270 rhoknp-1.3.1/README.md
+-rw-r--r--   0        0        0     1849 2023-06-01 10:08:39.510243 rhoknp-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0      474 2023-01-23 11:06:01.235960 rhoknp-1.3.1/src/rhoknp/__init__.py
+-rw-r--r--   0        0        0      293 2023-01-25 04:22:29.044533 rhoknp-1.3.1/src/rhoknp/cli/__init__.py
+-rw-r--r--   0        0        0     3334 2023-05-01 10:39:22.239944 rhoknp-1.3.1/src/rhoknp/cli/cli.py
+-rw-r--r--   0        0        0     6802 2023-05-01 10:39:22.240180 rhoknp-1.3.1/src/rhoknp/cli/serve.py
+-rw-r--r--   0        0        0     5782 2023-05-01 10:39:22.240529 rhoknp-1.3.1/src/rhoknp/cli/show.py
+-rw-r--r--   0        0        0      823 2023-05-01 10:39:22.240711 rhoknp-1.3.1/src/rhoknp/cli/static/css/style.css
+-rw-r--r--   0        0        0     9898 2023-05-01 10:39:22.241416 rhoknp-1.3.1/src/rhoknp/cli/static/images/apple-touch-icon.png
+-rw-r--r--   0        0        0    15086 2023-05-01 10:39:22.242054 rhoknp-1.3.1/src/rhoknp/cli/static/images/favicon.ico
+-rw-r--r--   0        0        0     1960 2023-05-01 10:39:22.242198 rhoknp-1.3.1/src/rhoknp/cli/static/js/script.js
+-rw-r--r--   0        0        0     1779 2023-01-23 11:06:01.236808 rhoknp-1.3.1/src/rhoknp/cli/stats.py
+-rw-r--r--   0        0        0     1705 2023-05-01 10:39:22.242748 rhoknp-1.3.1/src/rhoknp/cli/templates/base.jinja2
+-rw-r--r--   0        0        0      724 2023-05-01 10:39:22.242904 rhoknp-1.3.1/src/rhoknp/cli/templates/components/dependency_parsing.jinja2
+-rw-r--r--   0        0        0     1840 2023-05-01 10:39:22.243108 rhoknp-1.3.1/src/rhoknp/cli/templates/components/discourse_parsing.jinja2
+-rw-r--r--   0        0        0      276 2023-05-01 10:39:22.243247 rhoknp-1.3.1/src/rhoknp/cli/templates/components/error.jinja2
+-rw-r--r--   0        0        0      344 2023-05-01 10:39:22.243341 rhoknp-1.3.1/src/rhoknp/cli/templates/components/form.jinja2
+-rw-r--r--   0        0        0      136 2023-05-01 10:39:22.243485 rhoknp-1.3.1/src/rhoknp/cli/templates/components/hide_all_button.jinja2
+-rw-r--r--   0        0        0     1987 2023-05-01 10:39:22.243568 rhoknp-1.3.1/src/rhoknp/cli/templates/components/morphological_analysis.jinja2
+-rw-r--r--   0        0        0     1063 2023-05-01 10:39:22.243719 rhoknp-1.3.1/src/rhoknp/cli/templates/components/named_entity_recognition.jinja2
+-rw-r--r--   0        0        0      163 2023-05-01 10:39:22.243791 rhoknp-1.3.1/src/rhoknp/cli/templates/components/navbar.jinja2
+-rw-r--r--   0        0        0       63 2023-05-01 10:39:22.244032 rhoknp-1.3.1/src/rhoknp/cli/templates/components/raw_input.jinja2
+-rw-r--r--   0        0        0      636 2023-05-01 10:39:22.244218 rhoknp-1.3.1/src/rhoknp/cli/templates/components/raw_output.jinja2
+-rw-r--r--   0        0        0      131 2023-05-01 10:39:22.244412 rhoknp-1.3.1/src/rhoknp/cli/templates/components/show_all_button.jinja2
+-rw-r--r--   0        0        0     1034 2023-05-01 10:39:22.244575 rhoknp-1.3.1/src/rhoknp/cli/templates/components/typo_correction.jinja2
+-rw-r--r--   0        0        0      722 2023-05-01 10:39:22.244665 rhoknp-1.3.1/src/rhoknp/cli/templates/components/word_splitting.jinja2
+-rw-r--r--   0        0        0      333 2023-05-01 10:39:22.244808 rhoknp-1.3.1/src/rhoknp/cli/templates/jumanpp.jinja2
+-rw-r--r--   0        0        0      526 2023-05-01 10:39:22.244946 rhoknp-1.3.1/src/rhoknp/cli/templates/knp.jinja2
+-rw-r--r--   0        0        0      643 2023-05-01 10:39:22.245089 rhoknp-1.3.1/src/rhoknp/cli/templates/kwja.jinja2
+-rw-r--r--   0        0        0      826 2023-01-23 11:06:01.237203 rhoknp-1.3.1/src/rhoknp/cohesion/__init__.py
+-rw-r--r--   0        0        0     6744 2023-02-07 06:49:22.772304 rhoknp-1.3.1/src/rhoknp/cohesion/argument.py
+-rw-r--r--   0        0        0     9899 2023-02-07 06:49:22.772615 rhoknp-1.3.1/src/rhoknp/cohesion/coreference.py
+-rw-r--r--   0        0        0     9566 2023-01-23 11:06:01.238718 rhoknp-1.3.1/src/rhoknp/cohesion/discourse.py
+-rw-r--r--   0        0        0     2427 2023-01-23 11:06:01.239467 rhoknp-1.3.1/src/rhoknp/cohesion/exophora.py
+-rw-r--r--   0        0        0    10329 2023-02-07 06:49:22.772957 rhoknp-1.3.1/src/rhoknp/cohesion/pas.py
+-rw-r--r--   0        0        0     2595 2023-01-23 11:06:01.239969 rhoknp-1.3.1/src/rhoknp/cohesion/predicate.py
+-rw-r--r--   0        0        0     4716 2023-01-23 11:06:01.240472 rhoknp-1.3.1/src/rhoknp/cohesion/rel.py
+-rw-r--r--   0        0        0      226 2023-01-23 11:06:01.240680 rhoknp-1.3.1/src/rhoknp/processors/__init__.py
+-rw-r--r--   0        0        0     5264 2023-05-01 10:39:22.245299 rhoknp-1.3.1/src/rhoknp/processors/jumanpp.py
+-rw-r--r--   0        0        0     7027 2023-05-01 10:39:22.245466 rhoknp-1.3.1/src/rhoknp/processors/knp.py
+-rw-r--r--   0        0        0     5617 2023-05-01 10:39:22.245819 rhoknp-1.3.1/src/rhoknp/processors/kwja.py
+-rw-r--r--   0        0        0     2984 2022-10-29 15:30:49.159597 rhoknp-1.3.1/src/rhoknp/processors/processor.py
+-rw-r--r--   0        0        0     3070 2023-05-01 10:39:22.245994 rhoknp-1.3.1/src/rhoknp/processors/senter.py
+-rw-r--r--   0        0        0      378 2023-01-23 11:06:01.241792 rhoknp-1.3.1/src/rhoknp/props/__init__.py
+-rw-r--r--   0        0        0      210 2022-10-24 08:19:10.843963 rhoknp-1.3.1/src/rhoknp/props/dependency.py
+-rw-r--r--   0        0        0     1996 2023-01-23 11:06:01.242202 rhoknp-1.3.1/src/rhoknp/props/feature.py
+-rw-r--r--   0        0        0      863 2023-01-23 11:06:01.242583 rhoknp-1.3.1/src/rhoknp/props/memo.py
+-rw-r--r--   0        0        0     2917 2023-02-07 06:49:22.773596 rhoknp-1.3.1/src/rhoknp/props/named_entity.py
+-rw-r--r--   0        0        0     1633 2023-01-23 11:06:01.243129 rhoknp-1.3.1/src/rhoknp/props/semantics.py
+-rw-r--r--   0        0        0        0 2022-07-07 07:10:30.837345 rhoknp-1.3.1/src/rhoknp/py.typed
+-rw-r--r--   0        0        0      337 2023-01-23 11:06:01.243840 rhoknp-1.3.1/src/rhoknp/units/__init__.py
+-rw-r--r--   0        0        0    14479 2023-03-03 06:23:17.602965 rhoknp-1.3.1/src/rhoknp/units/base_phrase.py
+-rw-r--r--   0        0        0     7740 2023-02-07 06:49:22.774401 rhoknp-1.3.1/src/rhoknp/units/clause.py
+-rw-r--r--   0        0        0    15809 2023-02-07 06:49:22.774863 rhoknp-1.3.1/src/rhoknp/units/document.py
+-rw-r--r--   0        0        0    12324 2023-06-01 10:08:39.510621 rhoknp-1.3.1/src/rhoknp/units/morpheme.py
+-rw-r--r--   0        0        0     7202 2023-02-07 06:49:22.775468 rhoknp-1.3.1/src/rhoknp/units/phrase.py
+-rw-r--r--   0        0        0    18039 2023-05-01 10:39:22.246566 rhoknp-1.3.1/src/rhoknp/units/sentence.py
+-rw-r--r--   0        0        0     1521 2023-01-23 11:06:01.246571 rhoknp-1.3.1/src/rhoknp/units/unit.py
+-rw-r--r--   0        0        0        0 2023-01-23 11:06:01.246629 rhoknp-1.3.1/src/rhoknp/utils/__init__.py
+-rw-r--r--   0        0        0     3783 2023-05-01 10:39:22.247129 rhoknp-1.3.1/src/rhoknp/utils/reader.py
+-rw-r--r--   0        0        0     1112 2023-05-01 10:39:22.247398 rhoknp-1.3.1/src/rhoknp/utils/util.py
+-rw-r--r--   0        0        0     7888 1970-01-01 00:00:00.000000 rhoknp-1.3.1/PKG-INFO
```

### Comparing `rhoknp-1.3.0/LICENSE` & `rhoknp-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.0/README.md` & `rhoknp-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.0/pyproject.toml` & `rhoknp-1.3.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rhoknp"
-version = "1.3.0"
+version = "1.3.1"
 description = "Yet another Python binding for Juman++/KNP/KWJA"
 license = "MIT"
 authors = [
     "Hirokazu Kiyomaru <h.kiyomaru@gmail.com>",
     "Nobuhiro Ueda <ueda@nlp.ist.i.kyoto-u.ac.jp>",
 ]
 readme = "README.md"
@@ -12,37 +12,42 @@
 documentation = "https://rhoknp.readthedocs.io/en/latest"
 keywords = ["NLP"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 cached-property = { version = "^1.5", python = "<3.8" }
 importlib-metadata = { version = ">=5.2", python = "<3.8" }
-typer = { version = ">=0.6.1,<0.8", optional = true }
+typer = [
+    { version = ">=0.7,<0.9", python = "<3.8", optional = true },
+    { version = ">=0.7", python = ">=3.8", optional = true },
+]
 PyYAML = { version = "^6.0", optional = true }
 rich = { version = ">=12.6", optional = true }
 uvicorn = { version = ">=0.21.0,<1", optional = true }
 fastapi = { version = ">=0.92.0,<1", optional = true }
-jinja2 = { version = "^3.1.2", optional = true }
-
-[tool.poetry.group.dev]
+jinja2 = { version = "^3.1", optional = true }
 
 [tool.poetry.group.dev.dependencies]
-ipdb = "^0.13.9"
-
-[tool.poetry.group.test]
+ipython = [
+    { version = "^7.34", python = "<3.8" },
+    { version = "~8.12.1", python = "3.8" },
+    { version = "^8.13", python = ">=3.9" },
+]
+ipdb = "^0.13.13"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2"
 pytest-cov = "^4.0"
 httpx = "^0.24.0"
 
-[tool.poetry.group.docs]
-
 [tool.poetry.group.docs.dependencies]
-Sphinx = "^5.3"
+Sphinx = [
+    { version = "^5.3", python = "<3.8" },
+    { version = "^6.2", python = ">=3.8" },
+]
 sphinx-prompt = "^1.5"
 sphinx-copybutton = "^0.5.0"
 myst-parser = "^1.0"
 furo = "^2023.3"
 
 [tool.poetry.extras]
 cli = ["typer", "PyYAML", "rich", "uvicorn", "fastapi", "jinja2"]
```

### Comparing `rhoknp-1.3.0/src/rhoknp/cli/cli.py` & `rhoknp-1.3.1/src/rhoknp/cli/cli.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.0/src/rhoknp/cli/serve.py` & `rhoknp-1.3.1/src/rhoknp/cli/serve.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.0/src/rhoknp/cli/show.py` & `rhoknp-1.3.1/src/rhoknp/cli/show.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.0/src/rhoknp/cli/static/css/style.css` & `rhoknp-1.3.1/src/rhoknp/cli/static/css/style.css`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.0/src/rhoknp/cli/static/images/apple-touch-icon.png` & `rhoknp-1.3.1/src/rhoknp/cli/static/images/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.0/src/rhoknp/cli/static/images/favicon.ico` & `rhoknp-1.3.1/src/rhoknp/cli/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.0/src/rhoknp/cli/static/js/script.js` & `rhoknp-1.3.1/src/rhoknp/cli/static/js/script.js`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.0/src/rhoknp/cli/stats.py` & `rhoknp-1.3.1/src/rhoknp/cli/stats.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.0/src/rhoknp/cli/templates/base.jinja2` & `rhoknp-1.3.1/src/rhoknp/cli/templates/base.jinja2`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.0/src/rhoknp/cli/templates/components/dependency_parsing.jinja2` & `rhoknp-1.3.1/src/rhoknp/cli/templates/components/dependency_parsing.jinja2`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.0/src/rhoknp/cli/templates/components/discourse_parsing.jinja2` & `rhoknp-1.3.1/src/rhoknp/cli/templates/components/discourse_parsing.jinja2`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.0/src/rhoknp/cli/templates/components/morphological_analysis.jinja2` & `rhoknp-1.3.1/src/rhoknp/cli/templates/components/morphological_analysis.jinja2`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.0/src/rhoknp/cli/templates/components/named_entity_recognition.jinja2` & `rhoknp-1.3.1/src/rhoknp/cli/templates/components/named_entity_recognition.jinja2`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.0/src/rhoknp/cli/templates/components/raw_output.jinja2` & `rhoknp-1.3.1/src/rhoknp/cli/templates/components/raw_output.jinja2`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.0/src/rhoknp/cli/templates/components/typo_correction.jinja2` & `rhoknp-1.3.1/src/rhoknp/cli/templates/components/typo_correction.jinja2`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.0/src/rhoknp/cli/templates/components/word_splitting.jinja2` & `rhoknp-1.3.1/src/rhoknp/cli/templates/components/word_splitting.jinja2`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.0/src/rhoknp/cli/templates/knp.jinja2` & `rhoknp-1.3.1/src/rhoknp/cli/templates/knp.jinja2`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.0/src/rhoknp/cli/templates/kwja.jinja2` & `rhoknp-1.3.1/src/rhoknp/cli/templates/kwja.jinja2`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.0/src/rhoknp/cohesion/__init__.py` & `rhoknp-1.3.1/src/rhoknp/cohesion/__init__.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.0/src/rhoknp/cohesion/argument.py` & `rhoknp-1.3.1/src/rhoknp/cohesion/argument.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.0/src/rhoknp/cohesion/coreference.py` & `rhoknp-1.3.1/src/rhoknp/cohesion/coreference.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.0/src/rhoknp/cohesion/discourse.py` & `rhoknp-1.3.1/src/rhoknp/cohesion/discourse.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.0/src/rhoknp/cohesion/exophora.py` & `rhoknp-1.3.1/src/rhoknp/cohesion/exophora.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.0/src/rhoknp/cohesion/pas.py` & `rhoknp-1.3.1/src/rhoknp/cohesion/pas.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.0/src/rhoknp/cohesion/predicate.py` & `rhoknp-1.3.1/src/rhoknp/cohesion/predicate.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.0/src/rhoknp/cohesion/rel.py` & `rhoknp-1.3.1/src/rhoknp/cohesion/rel.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.0/src/rhoknp/processors/jumanpp.py` & `rhoknp-1.3.1/src/rhoknp/processors/jumanpp.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.0/src/rhoknp/processors/knp.py` & `rhoknp-1.3.1/src/rhoknp/processors/knp.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.0/src/rhoknp/processors/kwja.py` & `rhoknp-1.3.1/src/rhoknp/processors/kwja.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.0/src/rhoknp/processors/processor.py` & `rhoknp-1.3.1/src/rhoknp/processors/processor.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.0/src/rhoknp/processors/senter.py` & `rhoknp-1.3.1/src/rhoknp/processors/senter.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.0/src/rhoknp/props/feature.py` & `rhoknp-1.3.1/src/rhoknp/props/feature.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.0/src/rhoknp/props/memo.py` & `rhoknp-1.3.1/src/rhoknp/props/memo.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.0/src/rhoknp/props/named_entity.py` & `rhoknp-1.3.1/src/rhoknp/props/named_entity.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.0/src/rhoknp/props/semantics.py` & `rhoknp-1.3.1/src/rhoknp/props/semantics.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.0/src/rhoknp/units/base_phrase.py` & `rhoknp-1.3.1/src/rhoknp/units/base_phrase.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.0/src/rhoknp/units/clause.py` & `rhoknp-1.3.1/src/rhoknp/units/clause.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.0/src/rhoknp/units/document.py` & `rhoknp-1.3.1/src/rhoknp/units/document.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.0/src/rhoknp/units/morpheme.py` & `rhoknp-1.3.1/src/rhoknp/units/morpheme.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     from rhoknp.units.sentence import Sentence
 
 
 class Morpheme(Unit):
     """形態素クラス．"""
 
     _ATTRIBUTES = (
-        "surf",
+        "_surf",
         "reading",
         "lemma",
         "pos",
         "pos_id",
         "subpos",
         "subpos_id",
         "conjtype",
@@ -51,14 +51,17 @@
 
     PAT_REPEATED: ClassVar[re.Pattern] = re.compile(
         r"(?P<surf>.+) (?P<attrs>(?P=surf) (?P=surf) [^ ]+ \d+ [^ ]+ \d+ [^ ]+ \d+ [^ ]+ \d+)"
         + rf"( {SemanticsDict.PAT.pattern})?"
         + rf"( {FeatureDict.PAT.pattern})?$"
     )
 
+    _ESCAPE_MAP = {" ": "　", '"': "”"}
+    _UNESCAPE_MAP = {v: k for k, v in _ESCAPE_MAP.items()}
+
     count = 0
 
     def __init__(
         self,
         text: str,
         reading: str,
         lemma: str,
@@ -72,14 +75,15 @@
         conjform_id: int,
         semantics: Optional[SemanticsDict] = None,
         features: Optional[FeatureDict] = None,
         homograph: bool = False,
     ) -> None:
         super().__init__()
         self.text = text
+        self._text_escaped = text
         self.reading = reading  #: 読み．
         self.lemma = lemma  #: 原形．
         self.pos = pos  #: 品詞．
         self.pos_id = pos_id  #: 品詞ID．
         self.subpos = subpos  #: 品詞細分類．
         self.subpos_id = subpos_id  #: 品詞細分類ID．
         self.conjtype = conjtype  #: 活用型．
@@ -95,14 +99,18 @@
         self.features: FeatureDict = features if features is not None else FeatureDict()  #: 素性．
         self.homographs: List["Morpheme"] = []  #: 同形の形態素のリスト．
 
         self.index = self.count  #: 文内におけるインデックス．
         if homograph is False:
             Morpheme.count += 1
 
+        # Resume text if it is escaped
+        if self.semantics.get("元半角") is True:
+            self.text = self._UNESCAPE_MAP.get(self.text, self.text)
+
     def __eq__(self, other: Any) -> bool:
         if isinstance(other, type(self)) is False:
             return False
         if self.parent_unit != other.parent_unit:
             return False
         return self.index == other.index
 
@@ -198,14 +206,19 @@
 
     @property
     def surf(self) -> str:
         """表層表現．"""
         return self.text
 
     @property
+    def _surf(self) -> str:
+        """表層表現（Juman/KNP フォーマット出力用）．"""
+        return self._text_escaped
+
+    @property
     def canon(self) -> Optional[str]:
         """代表表記．"""
         canon = self.semantics.get("代表表記")
         assert canon is None or isinstance(canon, str)
         return canon
 
     @property
```

### Comparing `rhoknp-1.3.0/src/rhoknp/units/phrase.py` & `rhoknp-1.3.1/src/rhoknp/units/phrase.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.0/src/rhoknp/units/sentence.py` & `rhoknp-1.3.1/src/rhoknp/units/sentence.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.0/src/rhoknp/units/unit.py` & `rhoknp-1.3.1/src/rhoknp/units/unit.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.0/src/rhoknp/utils/reader.py` & `rhoknp-1.3.1/src/rhoknp/utils/reader.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.0/src/rhoknp/utils/util.py` & `rhoknp-1.3.1/src/rhoknp/utils/util.py`

 * *Files identical despite different names*

### Comparing `rhoknp-1.3.0/PKG-INFO` & `rhoknp-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rhoknp
-Version: 1.3.0
+Version: 1.3.1
 Summary: Yet another Python binding for Juman++/KNP/KWJA
 Home-page: https://github.com/ku-nlp/rhoknp
 License: MIT
 Keywords: NLP
 Author: Hirokazu Kiyomaru
 Author-email: h.kiyomaru@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -16,17 +16,18 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: cli
 Requires-Dist: PyYAML (>=6.0,<7.0) ; extra == "cli"
 Requires-Dist: cached-property (>=1.5,<2.0) ; python_version < "3.8"
 Requires-Dist: fastapi (>=0.92.0,<1) ; extra == "cli"
 Requires-Dist: importlib-metadata (>=5.2) ; python_version < "3.8"
-Requires-Dist: jinja2 (>=3.1.2,<4.0.0) ; extra == "cli"
+Requires-Dist: jinja2 (>=3.1,<4.0) ; extra == "cli"
 Requires-Dist: rich (>=12.6) ; extra == "cli"
-Requires-Dist: typer (>=0.6.1,<0.8) ; extra == "cli"
+Requires-Dist: typer (>=0.7) ; (python_version >= "3.8") and (extra == "cli")
+Requires-Dist: typer (>=0.7,<0.9) ; (python_version < "3.8") and (extra == "cli")
 Requires-Dist: uvicorn (>=0.21.0,<1) ; extra == "cli"
 Project-URL: Documentation, https://rhoknp.readthedocs.io/en/latest
 Project-URL: Repository, https://github.com/ku-nlp/rhoknp
 Description-Content-Type: text/markdown
 
 <p align="center">
 <a href="https://rhoknp.readthedocs.io/en/latest/" rel="noopener" target="_blank">
```

#### html2text {}

```diff
@@ -1,24 +1,25 @@
-Metadata-Version: 2.1 Name: rhoknp Version: 1.3.0 Summary: Yet another Python
+Metadata-Version: 2.1 Name: rhoknp Version: 1.3.1 Summary: Yet another Python
 binding for Juman++/KNP/KWJA Home-page: https://github.com/ku-nlp/rhoknp
 License: MIT Keywords: NLP Author: Hirokazu Kiyomaru Author-email:
 h.kiyomaru@gmail.com Requires-Python: >=3.7,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Provides-Extra: cli Requires-Dist: PyYAML
 (>=6.0,<7.0) ; extra == "cli" Requires-Dist: cached-property (>=1.5,<2.0) ;
 python_version < "3.8" Requires-Dist: fastapi (>=0.92.0,<1) ; extra == "cli"
 Requires-Dist: importlib-metadata (>=5.2) ; python_version < "3.8" Requires-
-Dist: jinja2 (>=3.1.2,<4.0.0) ; extra == "cli" Requires-Dist: rich (>=12.6) ;
-extra == "cli" Requires-Dist: typer (>=0.6.1,<0.8) ; extra == "cli" Requires-
-Dist: uvicorn (>=0.21.0,<1) ; extra == "cli" Project-URL: Documentation, https:
-//rhoknp.readthedocs.io/en/latest Project-URL: Repository, https://github.com/
-ku-nlp/rhoknp Description-Content-Type: text/markdown
+Dist: jinja2 (>=3.1,<4.0) ; extra == "cli" Requires-Dist: rich (>=12.6) ; extra
+== "cli" Requires-Dist: typer (>=0.7) ; (python_version >= "3.8") and (extra ==
+"cli") Requires-Dist: typer (>=0.7,<0.9) ; (python_version < "3.8") and (extra
+== "cli") Requires-Dist: uvicorn (>=0.21.0,<1) ; extra == "cli" Project-URL:
+Documentation, https://rhoknp.readthedocs.io/en/latest Project-URL: Repository,
+https://github.com/ku-nlp/rhoknp Description-Content-Type: text/markdown
                                  [rhoknp_logo]
      ****** rhoknp: Yet another Python binding for Juman++/KNP/KWJA ******
  [Test] [Codecov] [CodeFactor] [PyPI] [PyPI_-_Python_Version]_[Documentation]_
                              [Code_style_-_black]
 _rhoknp_ is a Python binding for [Juman++](https://github.com/ku-nlp/jumanpp),
 [KNP](https://github.com/ku-nlp/knp), and [KWJA](https://github.com/ku-nlp/
 kwja).[^1] [^1]: The logo was originally generated using OpenAI DALLÂ·E 2
```

