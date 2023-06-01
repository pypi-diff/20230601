# Comparing `tmp/nester-struct-0.5.0.tar.gz` & `tmp/nester-struct-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nester-struct-0.5.0.tar", last modified: Thu Jun  1 20:23:19 2023, max compression
+gzip compressed data, was "nester-struct-0.5.1.tar", last modified: Thu Jun  1 20:28:17 2023, max compression
```

## Comparing `nester-struct-0.5.0.tar` & `nester-struct-0.5.1.tar`

### file list

```diff
@@ -1,163 +1,163 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:23:19.328689 nester-struct-0.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:23:19.308689 nester-struct-0.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:23:19.308689 nester-struct-0.5.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-01 20:23:02.000000 nester-struct-0.5.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-01 20:23:02.000000 nester-struct-0.5.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-01 20:23:02.000000 nester-struct-0.5.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-01 20:23:02.000000 nester-struct-0.5.0/.github/labeler.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:23:19.308689 nester-struct-0.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-01 20:23:02.000000 nester-struct-0.5.0/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-06-01 20:23:02.000000 nester-struct-0.5.0/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-06-01 20:23:02.000000 nester-struct-0.5.0/.github/workflows/increase_version.yml
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-01 20:23:02.000000 nester-struct-0.5.0/.github/workflows/label.yml
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-01 20:23:02.000000 nester-struct-0.5.0/.github/workflows/newsfragment_checker.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-01 20:23:02.000000 nester-struct-0.5.0/.github/workflows/packaging.yml
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-01 20:23:02.000000 nester-struct-0.5.0/.github/workflows/pylint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-01 20:23:02.000000 nester-struct-0.5.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-01 20:23:02.000000 nester-struct-0.5.0/.github/workflows/towncrier.yml
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-01 20:23:02.000000 nester-struct-0.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-01 20:23:02.000000 nester-struct-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-01 20:23:02.000000 nester-struct-0.5.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-01 20:23:02.000000 nester-struct-0.5.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-01 20:23:02.000000 nester-struct-0.5.0/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-06-01 20:23:02.000000 nester-struct-0.5.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-06-01 20:23:02.000000 nester-struct-0.5.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-01 20:23:02.000000 nester-struct-0.5.0/INSTALL.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-01 20:23:02.000000 nester-struct-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-06-01 20:23:19.328689 nester-struct-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6655 2023-06-01 20:23:02.000000 nester-struct-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-01 20:23:02.000000 nester-struct-0.5.0/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:23:19.308689 nester-struct-0.5.0/changelog/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:23:02.000000 nester-struct-0.5.0/changelog/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:23:19.312689 nester-struct-0.5.0/changelog.d/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-01 20:23:02.000000 nester-struct-0.5.0/changelog.d/30.added
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-01 20:23:02.000000 nester-struct-0.5.0/changelog.d/34.added
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-01 20:23:02.000000 nester-struct-0.5.0/changelog.d/changelog_template.jinja
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:23:19.312689 nester-struct-0.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:23:19.304689 nester-struct-0.5.0/docs/_build/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:23:19.312689 nester-struct-0.5.0/docs/_build/html/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/.buildinfo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:23:19.312689 nester-struct-0.5.0/docs/_build/html/.doctrees/
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/.doctrees/dev_docs.doctree
--rw-r--r--   0 runner    (1001) docker     (123)   116870 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/.doctrees/environment.pickle
--rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/.doctrees/index.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    10229 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/.doctrees/installation_guide.doctree
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:23:19.312689 nester-struct-0.5.0/docs/_build/html/.doctrees/source/
--rw-r--r--   0 runner    (1001) docker     (123)    28309 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/.doctrees/source/utils.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/.doctrees/supported_languages.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    23168 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/.doctrees/usage_guide.doctree
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:23:19.312689 nester-struct-0.5.0/docs/_build/html/_sources/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/_sources/dev_docs.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/_sources/index.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/_sources/installation_guide.rst.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:23:19.312689 nester-struct-0.5.0/docs/_build/html/_sources/source/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/_sources/source/utils.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/_sources/supported_languages.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/_sources/usage_guide.rst.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:23:19.316689 nester-struct-0.5.0/docs/_build/html/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    14813 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/_static/basic.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:23:19.316689 nester-struct-0.5.0/docs/_build/html/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/_static/css/badge_only.css
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:23:19.320689 nester-struct-0.5.0/docs/_build/html/_static/css/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    87624 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)    67312 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    86288 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    66444 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   165742 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (123)   444379 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (123)   165548 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    98024 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (123)    77160 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   323344 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/_static/css/fonts/lato-bold-italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)   193308 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   309728 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/_static/css/fonts/lato-bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)   184912 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/_static/css/fonts/lato-bold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   328412 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/_static/css/fonts/lato-normal-italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)   195704 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   309192 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/_static/css/fonts/lato-normal.woff
--rw-r--r--   0 runner    (1001) docker     (123)   182708 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/_static/css/fonts/lato-normal.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   135235 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/_static/css/theme.css
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/_static/doctools.js
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/_static/documentation_options.js
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/_static/file.png
--rw-r--r--   0 runner    (1001) docker     (123)    86196 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/_static/index_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:23:19.324689 nester-struct-0.5.0/docs/_build/html/_static/js/
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/_static/js/badge_only.js
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/_static/js/html5shiv-printshiv.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/_static/js/html5shiv.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/_static/js/theme.js
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/_static/language_data.js
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/_static/minus.png
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/_static/plus.png
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/_static/pygments.css
--rw-r--r--   0 runner    (1001) docker     (123)    18215 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/_static/searchtools.js
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/_static/sphinx_highlight.js
--rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/dev_docs.html
--rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/genindex.html
--rw-r--r--   0 runner    (1001) docker     (123)     7645 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     7665 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/installation_guide.html
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/objects.inv
--rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/py-modindex.html
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/search.html
--rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/searchindex.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:23:19.324689 nester-struct-0.5.0/docs/_build/html/source/
--rw-r--r--   0 runner    (1001) docker     (123)    13389 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/source/utils.html
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/supported_languages.html
--rw-r--r--   0 runner    (1001) docker     (123)    11300 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_build/html/usage_guide.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:23:19.324689 nester-struct-0.5.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:23:19.324689 nester-struct-0.5.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)    86196 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/_static/index_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/dev_docs.rst
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/installation_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:23:19.324689 nester-struct-0.5.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/source/utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/supported_languages.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-06-01 20:23:02.000000 nester-struct-0.5.0/docs/usage_guide.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:23:19.324689 nester-struct-0.5.0/img/
--rw-r--r--   0 runner    (1001) docker     (123)    70052 2023-06-01 20:23:02.000000 nester-struct-0.5.0/img/logo_social_preview.png
--rw-r--r--   0 runner    (1001) docker     (123)    62005 2023-06-01 20:23:02.000000 nester-struct-0.5.0/img/logo_thumbnail.png
--rw-r--r--   0 runner    (1001) docker     (123)    86196 2023-06-01 20:23:02.000000 nester-struct-0.5.0/index_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-01 20:23:02.000000 nester-struct-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-01 20:23:19.328689 nester-struct-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:23:19.308689 nester-struct-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:23:19.324689 nester-struct-0.5.0/src/nester/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-01 20:23:02.000000 nester-struct-0.5.0/src/nester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-06-01 20:23:02.000000 nester-struct-0.5.0/src/nester/nester_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     6065 2023-06-01 20:23:02.000000 nester-struct-0.5.0/src/nester/nester_log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:23:19.308689 nester-struct-0.5.0/src/nester/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:23:19.324689 nester-struct-0.5.0/src/nester/templates/c/
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-01 20:23:02.000000 nester-struct-0.5.0/src/nester/templates/c/c_layout.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:23:19.324689 nester-struct-0.5.0/src/nester/templates/cpp/
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-01 20:23:02.000000 nester-struct-0.5.0/src/nester/templates/cpp/cpp_layout.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:23:19.324689 nester-struct-0.5.0/src/nester/templates/cs/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-01 20:23:02.000000 nester-struct-0.5.0/src/nester/templates/cs/cs_layout.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:23:19.324689 nester-struct-0.5.0/src/nester/templates/java/
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-01 20:23:02.000000 nester-struct-0.5.0/src/nester/templates/java/java_layout.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:23:19.324689 nester-struct-0.5.0/src/nester/templates/py/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-01 20:23:02.000000 nester-struct-0.5.0/src/nester/templates/py/py_layout.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:23:19.324689 nester-struct-0.5.0/src/nester/templates/rb/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-01 20:23:02.000000 nester-struct-0.5.0/src/nester/templates/rb/rb_layout.json
--rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-06-01 20:23:02.000000 nester-struct-0.5.0/src/nester/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:23:19.324689 nester-struct-0.5.0/src/nester_struct.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-06-01 20:23:19.000000 nester-struct-0.5.0/src/nester_struct.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-06-01 20:23:19.000000 nester-struct-0.5.0/src/nester_struct.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 20:23:19.000000 nester-struct-0.5.0/src/nester_struct.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-01 20:23:19.000000 nester-struct-0.5.0/src/nester_struct.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-01 20:23:19.000000 nester-struct-0.5.0/src/nester_struct.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-01 20:23:19.000000 nester-struct-0.5.0/src/nester_struct.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 20:23:18.000000 nester-struct-0.5.0/src/nester_struct.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:23:19.324689 nester-struct-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:23:02.000000 nester-struct-0.5.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:23:19.324689 nester-struct-0.5.0/tests/interation_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:23:02.000000 nester-struct-0.5.0/tests/interation_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-06-01 20:23:02.000000 nester-struct-0.5.0/tests/interation_tests/test_util_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:23:19.328689 nester-struct-0.5.0/tests/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:23:02.000000 nester-struct-0.5.0/tests/unit_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-06-01 20:23:02.000000 nester-struct-0.5.0/tests/unit_tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-01 20:23:02.000000 nester-struct-0.5.0/tests/unit_tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.239712 nester-struct-0.5.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.227712 nester-struct-0.5.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.227712 nester-struct-0.5.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-01 20:27:59.000000 nester-struct-0.5.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-01 20:27:59.000000 nester-struct-0.5.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-01 20:27:59.000000 nester-struct-0.5.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-01 20:27:59.000000 nester-struct-0.5.1/.github/labeler.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.227712 nester-struct-0.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-01 20:27:59.000000 nester-struct-0.5.1/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-06-01 20:27:59.000000 nester-struct-0.5.1/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-06-01 20:27:59.000000 nester-struct-0.5.1/.github/workflows/increase_version.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-01 20:27:59.000000 nester-struct-0.5.1/.github/workflows/label.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-01 20:27:59.000000 nester-struct-0.5.1/.github/workflows/newsfragment_checker.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-01 20:27:59.000000 nester-struct-0.5.1/.github/workflows/packaging.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-01 20:27:59.000000 nester-struct-0.5.1/.github/workflows/pylint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-01 20:27:59.000000 nester-struct-0.5.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-01 20:27:59.000000 nester-struct-0.5.1/.github/workflows/towncrier.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-01 20:27:59.000000 nester-struct-0.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-01 20:27:59.000000 nester-struct-0.5.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-01 20:27:59.000000 nester-struct-0.5.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-01 20:27:59.000000 nester-struct-0.5.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-01 20:27:59.000000 nester-struct-0.5.1/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-06-01 20:27:59.000000 nester-struct-0.5.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-06-01 20:27:59.000000 nester-struct-0.5.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-01 20:27:59.000000 nester-struct-0.5.1/INSTALL.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-01 20:27:59.000000 nester-struct-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7205 2023-06-01 20:28:17.239712 nester-struct-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-06-01 20:27:59.000000 nester-struct-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-01 20:27:59.000000 nester-struct-0.5.1/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.227712 nester-struct-0.5.1/changelog/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:27:59.000000 nester-struct-0.5.1/changelog/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.227712 nester-struct-0.5.1/changelog.d/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-01 20:27:59.000000 nester-struct-0.5.1/changelog.d/30.added
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-01 20:27:59.000000 nester-struct-0.5.1/changelog.d/34.added
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-01 20:27:59.000000 nester-struct-0.5.1/changelog.d/changelog_template.jinja
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.227712 nester-struct-0.5.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-01 20:27:59.000000 nester-struct-0.5.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.223713 nester-struct-0.5.1/docs/_build/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.227712 nester-struct-0.5.1/docs/_build/html/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-01 20:27:59.000000 nester-struct-0.5.1/docs/_build/html/.buildinfo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.231712 nester-struct-0.5.1/docs/_build/html/.doctrees/
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-06-01 20:27:59.000000 nester-struct-0.5.1/docs/_build/html/.doctrees/dev_docs.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)   116870 2023-06-01 20:27:59.000000 nester-struct-0.5.1/docs/_build/html/.doctrees/environment.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-06-01 20:27:59.000000 nester-struct-0.5.1/docs/_build/html/.doctrees/index.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)    10229 2023-06-01 20:27:59.000000 nester-struct-0.5.1/docs/_build/html/.doctrees/installation_guide.doctree
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.231712 nester-struct-0.5.1/docs/_build/html/.doctrees/source/
+-rw-r--r--   0 runner    (1001) docker     (123)    28309 2023-06-01 20:27:59.000000 nester-struct-0.5.1/docs/_build/html/.doctrees/source/utils.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-06-01 20:27:59.000000 nester-struct-0.5.1/docs/_build/html/.doctrees/supported_languages.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)    23168 2023-06-01 20:27:59.000000 nester-struct-0.5.1/docs/_build/html/.doctrees/usage_guide.doctree
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.231712 nester-struct-0.5.1/docs/_build/html/_sources/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-01 20:27:59.000000 nester-struct-0.5.1/docs/_build/html/_sources/dev_docs.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-01 20:27:59.000000 nester-struct-0.5.1/docs/_build/html/_sources/index.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-01 20:27:59.000000 nester-struct-0.5.1/docs/_build/html/_sources/installation_guide.rst.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.231712 nester-struct-0.5.1/docs/_build/html/_sources/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-01 20:27:59.000000 nester-struct-0.5.1/docs/_build/html/_sources/source/utils.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-01 20:27:59.000000 nester-struct-0.5.1/docs/_build/html/_sources/supported_languages.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-06-01 20:27:59.000000 nester-struct-0.5.1/docs/_build/html/_sources/usage_guide.rst.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.231712 nester-struct-0.5.1/docs/_build/html/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    14813 2023-06-01 20:27:59.000000 nester-struct-0.5.1/docs/_build/html/_static/basic.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.231712 nester-struct-0.5.1/docs/_build/html/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-06-01 20:27:59.000000 nester-struct-0.5.1/docs/_build/html/_static/css/badge_only.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-06-01 20:27:59.000000 nester-struct-0.5.1/docs/_build/html/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.235712 nester-struct-0.5.1/docs/_build/html/_static/css/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    87624 2023-06-01 20:27:59.000000 nester-struct-0.5.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    67312 2023-06-01 20:27:59.000000 nester-struct-0.5.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    86288 2023-06-01 20:27:59.000000 nester-struct-0.5.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    66444 2023-06-01 20:27:59.000000 nester-struct-0.5.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   165742 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   444379 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   165548 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    98024 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    77160 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   323344 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   193308 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   309728 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/css/fonts/lato-bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   184912 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/css/fonts/lato-bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   328412 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   195704 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   309192 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/css/fonts/lato-normal.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   182708 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/css/fonts/lato-normal.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   135235 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/css/theme.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/doctools.js
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/documentation_options.js
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/file.png
+-rw-r--r--   0 runner    (1001) docker     (123)    86196 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/index_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.239712 nester-struct-0.5.1/docs/_build/html/_static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/js/badge_only.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/js/html5shiv.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/js/theme.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/language_data.js
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/minus.png
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/plus.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/pygments.css
+-rw-r--r--   0 runner    (1001) docker     (123)    18215 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/searchtools.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/_static/sphinx_highlight.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/dev_docs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/genindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7645 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7665 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/installation_guide.html
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/objects.inv
+-rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/py-modindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/searchindex.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.239712 nester-struct-0.5.1/docs/_build/html/source/
+-rw-r--r--   0 runner    (1001) docker     (123)    13389 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/source/utils.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/supported_languages.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11300 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_build/html/usage_guide.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.239712 nester-struct-0.5.1/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.239712 nester-struct-0.5.1/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)    86196 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/_static/index_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/dev_docs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/installation_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.239712 nester-struct-0.5.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/source/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/supported_languages.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-06-01 20:28:00.000000 nester-struct-0.5.1/docs/usage_guide.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.239712 nester-struct-0.5.1/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    70052 2023-06-01 20:28:00.000000 nester-struct-0.5.1/img/logo_social_preview.png
+-rw-r--r--   0 runner    (1001) docker     (123)    62005 2023-06-01 20:28:00.000000 nester-struct-0.5.1/img/logo_thumbnail.png
+-rw-r--r--   0 runner    (1001) docker     (123)    86196 2023-06-01 20:28:00.000000 nester-struct-0.5.1/index_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-01 20:28:00.000000 nester-struct-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-01 20:28:17.243713 nester-struct-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.223713 nester-struct-0.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.239712 nester-struct-0.5.1/src/nester/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-01 20:28:00.000000 nester-struct-0.5.1/src/nester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-06-01 20:28:00.000000 nester-struct-0.5.1/src/nester/nester_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6065 2023-06-01 20:28:00.000000 nester-struct-0.5.1/src/nester/nester_log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.223713 nester-struct-0.5.1/src/nester/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.239712 nester-struct-0.5.1/src/nester/templates/c/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-01 20:28:00.000000 nester-struct-0.5.1/src/nester/templates/c/c_layout.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.239712 nester-struct-0.5.1/src/nester/templates/cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-01 20:28:00.000000 nester-struct-0.5.1/src/nester/templates/cpp/cpp_layout.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.239712 nester-struct-0.5.1/src/nester/templates/cs/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-01 20:28:00.000000 nester-struct-0.5.1/src/nester/templates/cs/cs_layout.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.239712 nester-struct-0.5.1/src/nester/templates/java/
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-01 20:28:00.000000 nester-struct-0.5.1/src/nester/templates/java/java_layout.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.239712 nester-struct-0.5.1/src/nester/templates/py/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-01 20:28:00.000000 nester-struct-0.5.1/src/nester/templates/py/py_layout.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.239712 nester-struct-0.5.1/src/nester/templates/rb/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-01 20:28:00.000000 nester-struct-0.5.1/src/nester/templates/rb/rb_layout.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-06-01 20:28:00.000000 nester-struct-0.5.1/src/nester/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.239712 nester-struct-0.5.1/src/nester_struct.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7205 2023-06-01 20:28:17.000000 nester-struct-0.5.1/src/nester_struct.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-06-01 20:28:17.000000 nester-struct-0.5.1/src/nester_struct.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 20:28:17.000000 nester-struct-0.5.1/src/nester_struct.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-01 20:28:17.000000 nester-struct-0.5.1/src/nester_struct.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-01 20:28:17.000000 nester-struct-0.5.1/src/nester_struct.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-01 20:28:17.000000 nester-struct-0.5.1/src/nester_struct.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 20:28:16.000000 nester-struct-0.5.1/src/nester_struct.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.239712 nester-struct-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:00.000000 nester-struct-0.5.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.239712 nester-struct-0.5.1/tests/interation_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:00.000000 nester-struct-0.5.1/tests/interation_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-06-01 20:28:00.000000 nester-struct-0.5.1/tests/interation_tests/test_util_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:17.239712 nester-struct-0.5.1/tests/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:28:00.000000 nester-struct-0.5.1/tests/unit_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-06-01 20:28:00.000000 nester-struct-0.5.1/tests/unit_tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-01 20:28:00.000000 nester-struct-0.5.1/tests/unit_tests/test_utils.py
```

### Comparing `nester-struct-0.5.0/.github/ISSUE_TEMPLATE/bug_report.md` & `nester-struct-0.5.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/.github/ISSUE_TEMPLATE/feature_request.md` & `nester-struct-0.5.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/.github/PULL_REQUEST_TEMPLATE.md` & `nester-struct-0.5.1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/.github/workflows/codeql.yml` & `nester-struct-0.5.1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/.github/workflows/increase_version.yml` & `nester-struct-0.5.1/.github/workflows/increase_version.yml`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/.github/workflows/label.yml` & `nester-struct-0.5.1/.github/workflows/label.yml`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/.github/workflows/newsfragment_checker.yml` & `nester-struct-0.5.1/.github/workflows/newsfragment_checker.yml`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/.github/workflows/packaging.yml` & `nester-struct-0.5.1/.github/workflows/packaging.yml`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/.github/workflows/pylint.yml` & `nester-struct-0.5.1/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/.github/workflows/towncrier.yml` & `nester-struct-0.5.1/.github/workflows/towncrier.yml`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/.pre-commit-config.yaml` & `nester-struct-0.5.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/CODE_OF_CONDUCT.md` & `nester-struct-0.5.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/CONTRIBUTING.md` & `nester-struct-0.5.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/INSTALL.md` & `nester-struct-0.5.1/INSTALL.md`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/LICENSE` & `nester-struct-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/PKG-INFO` & `nester-struct-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nester-struct
-Version: 0.5.0
+Version: 0.5.1
 Summary: Automated creation of project structure
 Home-page: https://github.com/ByteOtter/nester
 Author: Christopher Hock
 Author-email: christopher-hock@protonmail.com
 License: GPLv3.0
 Keywords: automation,project_structure,python
 Classifier: Natural Language :: English
@@ -113,15 +113,15 @@
 nester <OPERATION> <OPTIONAL -git FLAG> <LANGUAGE> <PROJECT_NAME>
 ```
 The following operations will be available:
 |`Operation`|Flags|Argument|Argument|Effect|
 |-|-|-|-|-|
 |`create`|`-g/--git`, `--no-log`|`Language`|`Projectname`|Creates the project structure for the selected lanugage in *the current directory*. IF `-git` is set it will also call `git init` in this directory. `--no-log` Will prevent Nester from creating a log entry for this project. You can find the log in your home directory at `~/nester.log`|
 |`validate`|n/A|`Language`|`Projectname`|Checks the current directory and its sub-directories if it corresponds to the schema provided for the language|
-|`list`|n/A|n/A|n/A|Prints out all *logged* projects that have been created previously|
+|`log`|n/A|n/A|n/A|Prints out all *logged* projects that have been created previously|
 |`clean`|`-y/--yes`|`Projectname`|n/A|Deletes the content of the specified project|
 
 ### Interactive / GUI - Mode (coming soon)
 
 This is considered to be the fallback mode. If **Nester** is called without any arguments you will be asked to enter all parameters manually.
 
 The parameters themselves will stay the same though.
```

### Comparing `nester-struct-0.5.0/README.md` & `nester-struct-0.5.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 nester <OPERATION> <OPTIONAL -git FLAG> <LANGUAGE> <PROJECT_NAME>
 ```
 The following operations will be available:
 |`Operation`|Flags|Argument|Argument|Effect|
 |-|-|-|-|-|
 |`create`|`-g/--git`, `--no-log`|`Language`|`Projectname`|Creates the project structure for the selected lanugage in *the current directory*. IF `-git` is set it will also call `git init` in this directory. `--no-log` Will prevent Nester from creating a log entry for this project. You can find the log in your home directory at `~/nester.log`|
 |`validate`|n/A|`Language`|`Projectname`|Checks the current directory and its sub-directories if it corresponds to the schema provided for the language|
-|`list`|n/A|n/A|n/A|Prints out all *logged* projects that have been created previously|
+|`log`|n/A|n/A|n/A|Prints out all *logged* projects that have been created previously|
 |`clean`|`-y/--yes`|`Projectname`|n/A|Deletes the content of the specified project|
 
 ### Interactive / GUI - Mode (coming soon)
 
 This is considered to be the fallback mode. If **Nester** is called without any arguments you will be asked to enter all parameters manually.
 
 The parameters themselves will stay the same though.
```

### Comparing `nester-struct-0.5.0/docs/Makefile` & `nester-struct-0.5.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_build/html/.doctrees/dev_docs.doctree` & `nester-struct-0.5.1/docs/_build/html/.doctrees/dev_docs.doctree`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_build/html/.doctrees/environment.pickle` & `nester-struct-0.5.1/docs/_build/html/.doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_build/html/.doctrees/index.doctree` & `nester-struct-0.5.1/docs/_build/html/.doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_build/html/.doctrees/installation_guide.doctree` & `nester-struct-0.5.1/docs/_build/html/.doctrees/installation_guide.doctree`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_build/html/.doctrees/source/utils.doctree` & `nester-struct-0.5.1/docs/_build/html/.doctrees/source/utils.doctree`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_build/html/.doctrees/supported_languages.doctree` & `nester-struct-0.5.1/docs/_build/html/.doctrees/supported_languages.doctree`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_build/html/.doctrees/usage_guide.doctree` & `nester-struct-0.5.1/docs/_build/html/.doctrees/usage_guide.doctree`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_build/html/_sources/index.rst.txt` & `nester-struct-0.5.1/docs/_build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_build/html/_sources/installation_guide.rst.txt` & `nester-struct-0.5.1/docs/_build/html/_sources/installation_guide.rst.txt`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_build/html/_sources/supported_languages.rst.txt` & `nester-struct-0.5.1/docs/_build/html/_sources/supported_languages.rst.txt`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_build/html/_sources/usage_guide.rst.txt` & `nester-struct-0.5.1/docs/_build/html/_sources/usage_guide.rst.txt`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_build/html/_static/basic.css` & `nester-struct-0.5.1/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_build/html/_static/css/badge_only.css` & `nester-struct-0.5.1/docs/_build/html/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_build/html/_static/css/custom.css` & `nester-struct-0.5.1/docs/_build/html/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff` & `nester-struct-0.5.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2` & `nester-struct-0.5.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff` & `nester-struct-0.5.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2` & `nester-struct-0.5.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot` & `nester-struct-0.5.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg` & `nester-struct-0.5.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf` & `nester-struct-0.5.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff` & `nester-struct-0.5.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2` & `nester-struct-0.5.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_build/html/_static/css/fonts/lato-bold-italic.woff` & `nester-struct-0.5.1/docs/_build/html/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2` & `nester-struct-0.5.1/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_build/html/_static/css/fonts/lato-bold.woff` & `nester-struct-0.5.1/docs/_build/html/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_build/html/_static/css/fonts/lato-bold.woff2` & `nester-struct-0.5.1/docs/_build/html/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_build/html/_static/css/fonts/lato-normal-italic.woff` & `nester-struct-0.5.1/docs/_build/html/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2` & `nester-struct-0.5.1/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_build/html/_static/css/fonts/lato-normal.woff` & `nester-struct-0.5.1/docs/_build/html/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_build/html/_static/css/fonts/lato-normal.woff2` & `nester-struct-0.5.1/docs/_build/html/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_build/html/_static/css/theme.css` & `nester-struct-0.5.1/docs/_build/html/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_build/html/_static/doctools.js` & `nester-struct-0.5.1/docs/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_build/html/_static/index_logo.png` & `nester-struct-0.5.1/docs/_build/html/_static/index_logo.png`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_build/html/_static/js/badge_only.js` & `nester-struct-0.5.1/docs/_build/html/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_build/html/_static/js/html5shiv-printshiv.min.js` & `nester-struct-0.5.1/docs/_build/html/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_build/html/_static/js/html5shiv.min.js` & `nester-struct-0.5.1/docs/_build/html/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_build/html/_static/js/theme.js` & `nester-struct-0.5.1/docs/_build/html/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_build/html/_static/language_data.js` & `nester-struct-0.5.1/docs/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_build/html/_static/pygments.css` & `nester-struct-0.5.1/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_build/html/_static/searchtools.js` & `nester-struct-0.5.1/docs/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_build/html/_static/sphinx_highlight.js` & `nester-struct-0.5.1/docs/_build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_build/html/dev_docs.html` & `nester-struct-0.5.1/docs/_build/html/dev_docs.html`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_build/html/genindex.html` & `nester-struct-0.5.1/docs/_build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_build/html/index.html` & `nester-struct-0.5.1/docs/_build/html/index.html`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_build/html/installation_guide.html` & `nester-struct-0.5.1/docs/_build/html/installation_guide.html`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_build/html/py-modindex.html` & `nester-struct-0.5.1/docs/_build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_build/html/search.html` & `nester-struct-0.5.1/docs/_build/html/search.html`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_build/html/searchindex.js` & `nester-struct-0.5.1/docs/_build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_build/html/source/utils.html` & `nester-struct-0.5.1/docs/_build/html/source/utils.html`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_build/html/supported_languages.html` & `nester-struct-0.5.1/docs/_build/html/supported_languages.html`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_build/html/usage_guide.html` & `nester-struct-0.5.1/docs/_build/html/usage_guide.html`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_static/css/custom.css` & `nester-struct-0.5.1/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/_static/index_logo.png` & `nester-struct-0.5.1/docs/_static/index_logo.png`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/conf.py` & `nester-struct-0.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/index.rst` & `nester-struct-0.5.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/installation_guide.rst` & `nester-struct-0.5.1/docs/installation_guide.rst`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/supported_languages.rst` & `nester-struct-0.5.1/docs/supported_languages.rst`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/docs/usage_guide.rst` & `nester-struct-0.5.1/docs/usage_guide.rst`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/img/logo_social_preview.png` & `nester-struct-0.5.1/img/logo_social_preview.png`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/img/logo_thumbnail.png` & `nester-struct-0.5.1/img/logo_thumbnail.png`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/index_logo.png` & `nester-struct-0.5.1/index_logo.png`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/pyproject.toml` & `nester-struct-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/setup.cfg` & `nester-struct-0.5.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/src/nester/nester_commands.py` & `nester-struct-0.5.1/src/nester/nester_commands.py`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/src/nester/nester_log.py` & `nester-struct-0.5.1/src/nester/nester_log.py`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/src/nester/templates/c/c_layout.json` & `nester-struct-0.5.1/src/nester/templates/c/c_layout.json`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/src/nester/templates/cpp/cpp_layout.json` & `nester-struct-0.5.1/src/nester/templates/cpp/cpp_layout.json`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/src/nester/templates/java/java_layout.json` & `nester-struct-0.5.1/src/nester/templates/java/java_layout.json`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/src/nester/utils.py` & `nester-struct-0.5.1/src/nester/utils.py`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/src/nester_struct.egg-info/PKG-INFO` & `nester-struct-0.5.1/src/nester_struct.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nester-struct
-Version: 0.5.0
+Version: 0.5.1
 Summary: Automated creation of project structure
 Home-page: https://github.com/ByteOtter/nester
 Author: Christopher Hock
 Author-email: christopher-hock@protonmail.com
 License: GPLv3.0
 Keywords: automation,project_structure,python
 Classifier: Natural Language :: English
@@ -113,15 +113,15 @@
 nester <OPERATION> <OPTIONAL -git FLAG> <LANGUAGE> <PROJECT_NAME>
 ```
 The following operations will be available:
 |`Operation`|Flags|Argument|Argument|Effect|
 |-|-|-|-|-|
 |`create`|`-g/--git`, `--no-log`|`Language`|`Projectname`|Creates the project structure for the selected lanugage in *the current directory*. IF `-git` is set it will also call `git init` in this directory. `--no-log` Will prevent Nester from creating a log entry for this project. You can find the log in your home directory at `~/nester.log`|
 |`validate`|n/A|`Language`|`Projectname`|Checks the current directory and its sub-directories if it corresponds to the schema provided for the language|
-|`list`|n/A|n/A|n/A|Prints out all *logged* projects that have been created previously|
+|`log`|n/A|n/A|n/A|Prints out all *logged* projects that have been created previously|
 |`clean`|`-y/--yes`|`Projectname`|n/A|Deletes the content of the specified project|
 
 ### Interactive / GUI - Mode (coming soon)
 
 This is considered to be the fallback mode. If **Nester** is called without any arguments you will be asked to enter all parameters manually.
 
 The parameters themselves will stay the same though.
```

### Comparing `nester-struct-0.5.0/src/nester_struct.egg-info/SOURCES.txt` & `nester-struct-0.5.1/src/nester_struct.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/tests/interation_tests/test_util_integration.py` & `nester-struct-0.5.1/tests/interation_tests/test_util_integration.py`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/tests/unit_tests/test_logging.py` & `nester-struct-0.5.1/tests/unit_tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `nester-struct-0.5.0/tests/unit_tests/test_utils.py` & `nester-struct-0.5.1/tests/unit_tests/test_utils.py`

 * *Files identical despite different names*

