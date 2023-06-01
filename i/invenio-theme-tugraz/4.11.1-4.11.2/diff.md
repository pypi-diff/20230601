# Comparing `tmp/invenio-theme-tugraz-4.11.1.tar.gz` & `tmp/invenio-theme-tugraz-4.11.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-theme-tugraz-4.11.1.tar", last modified: Thu Apr 20 21:29:39 2023, max compression
+gzip compressed data, was "dist/invenio-theme-tugraz-4.11.2.tar", last modified: Thu Jun  1 10:46:22 2023, max compression
```

## Comparing `invenio-theme-tugraz-4.11.1.tar` & `invenio-theme-tugraz-4.11.2.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:29:39.000000 invenio-theme-tugraz-4.11.1/
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:29:39.000000 invenio-theme-tugraz-4.11.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:29:39.000000 invenio-theme-tugraz-4.11.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/.github/workflows/tests.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:29:39.000000 invenio-theme-tugraz-4.11.1/.tx/
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/.tx/config
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-04-20 21:29:39.000000 invenio-theme-tugraz-4.11.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:29:39.000000 invenio-theme-tugraz-4.11.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:29:39.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:29:39.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:29:39.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/assets/scss/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:29:39.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/footer.scss
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/header.scss
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/overrides.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:29:39.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/search/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/search/footer.scss
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/search/theme.scss
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/search/variables.scss
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/theme.scss
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/variables.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:29:39.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/assets/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:29:39.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/assets/semantic-ui/js/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:29:39.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/assets/semantic-ui/js/invenio_theme_tugraz/
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/assets/semantic-ui/js/invenio_theme_tugraz/theme.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:29:39.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/assets/semantic-ui/less/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:29:39.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/accounts.less
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/communities.less
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/deposit.less
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:29:39.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:29:39.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/
--rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/OFL.txt
--rw-r--r--   0 runner    (1001) docker     (123)    94816 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/SourceSansPro-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   269108 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/SourceSansPro-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/footer.less
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/frontpage.less
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/header.less
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/login.less
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/macros.less
--rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/overrides.less
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/record.less
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/search.less
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/theme.less
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/variables.less
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:29:39.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:29:39.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/static/extra/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/static/extra/orcid.png
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:29:39.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)    18533 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/static/images/Fair_Data_Austria_orangerot.png
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/static/images/Icon_1_v2.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/static/images/TU_Austria_Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)   225210 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/static/images/footer.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/static/images/icon_use.png
--rw-r--r--   0 runner    (1001) docker     (123)    18643 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/static/images/inveniordm-tail.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/static/images/library_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    23820 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/static/images/login_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    97455 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/static/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    16480 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/static/images/oea.svg
--rw-r--r--   0 runner    (1001) docker     (123)    38212 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/static/images/re3data.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/static/images/tug_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:29:39.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:29:39.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/templates/invenio_theme_tugraz/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:29:39.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/
--rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/accounts_base.html
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/header_login.html
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/login_user.html
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/register_user.html
--rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/templates/invenio_theme_tugraz/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/templates/invenio_theme_tugraz/benefits.html
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/templates/invenio_theme_tugraz/comingsoon.html
--rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/templates/invenio_theme_tugraz/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/templates/invenio_theme_tugraz/header.html
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:29:39.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/templates/invenio_theme_tugraz/macros/
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/templates/invenio_theme_tugraz/macros/authors.html
--rw-r--r--   0 runner    (1001) docker     (123)     6530 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/templates/invenio_theme_tugraz/navbar.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:29:39.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/translations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/translations/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:29:39.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:29:39.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     6979 2023-04-20 21:29:39.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    15973 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/translations/de/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/translations/messages.pot
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/webpack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:29:39.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-04-20 21:29:39.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-04-20 21:29:39.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 21:29:39.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-20 21:29:39.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 21:29:39.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-20 21:29:39.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-20 21:29:39.000000 invenio-theme-tugraz-4.11.1/invenio_theme_tugraz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      660 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-04-20 21:29:39.000000 invenio-theme-tugraz-4.11.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:29:39.000000 invenio-theme-tugraz-4.11.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-20 21:29:30.000000 invenio-theme-tugraz-4.11.1/tests/test_invenio_theme_tugraz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/.github/workflows/tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/.tx/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7665 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/scss/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/footer.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/header.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/overrides.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/search/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/search/footer.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/search/theme.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/search/variables.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/theme.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/variables.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/js/invenio_theme_tugraz/
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/js/invenio_theme_tugraz/theme.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/accounts.less
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/communities.less
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/deposit.less
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/
+-rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    94816 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/SourceSansPro-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   269108 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/SourceSansPro-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/footer.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/frontpage.less
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/header.less
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/login.less
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/macros.less
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/overrides.less
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/record.less
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/search.less
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/theme.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/variables.less
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/extra/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/extra/orcid.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    18533 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/images/Fair_Data_Austria_orangerot.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/images/Icon_1_v2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/images/TU_Austria_Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)   225210 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/images/footer.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/images/icon_use.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18643 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/images/inveniordm-tail.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/images/library_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23820 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/images/login_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    97455 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    16480 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/images/oea.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    38212 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/images/re3data.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/images/tug_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/invenio_theme_tugraz/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/accounts_base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/header_login.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/login_user.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/register_user.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/invenio_theme_tugraz/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/invenio_theme_tugraz/benefits.html
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/invenio_theme_tugraz/comingsoon.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/invenio_theme_tugraz/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/invenio_theme_tugraz/header.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/invenio_theme_tugraz/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/invenio_theme_tugraz/macros/authors.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6530 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/invenio_theme_tugraz/navbar.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/translations/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-06-01 10:46:21.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    16921 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/translations/de/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)    12938 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/translations/messages.pot
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7665 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      660 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/tests/test_invenio_theme_tugraz.py
```

### Comparing `invenio-theme-tugraz-4.11.1/.editorconfig` & `invenio-theme-tugraz-4.11.2/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/.github/workflows/pypi-publish.yml` & `invenio-theme-tugraz-4.11.2/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/.github/workflows/tests.yml` & `invenio-theme-tugraz-4.11.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/.tx/config` & `invenio-theme-tugraz-4.11.2/.tx/config`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/CHANGES.rst` & `invenio-theme-tugraz-4.11.2/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,21 @@
     invenio-theme-tugraz is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
+Version v4.11.2 (release 2023-06-01)
+
+- frontpage: layout changes
+- translation: add oer frontpage translation
+- WIP: oer upload button on frontpage
+
+
 Version v4.11.1 (release 2023-04-20)
 
 - fix: increase invenio-config-tugraz
 
 
 Version v4.11.0 (release 2023-04-20)
```

### Comparing `invenio-theme-tugraz-4.11.1/CONTRIBUTING.rst` & `invenio-theme-tugraz-4.11.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/LICENSE` & `invenio-theme-tugraz-4.11.2/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/MANIFEST.in` & `invenio-theme-tugraz-4.11.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/PKG-INFO` & `invenio-theme-tugraz-4.11.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-theme-tugraz
-Version: 4.11.1
+Version: 4.11.2
 Summary: "Invenio module for TUGRAZ theme."
 Home-page: https://github.com/tu-graz-library/invenio-theme-tugraz
 Author: "Graz University of Technology"
 Author-email: mojib.wali@tugraz.at
 License: MIT
 Description: ..
             Copyright (C) 2020-2021 Graz University of Technology.
@@ -58,14 +58,21 @@
             invenio-theme-tugraz is free software; you can redistribute it and/or
             modify it under the terms of the MIT License; see LICENSE file for more
             details.
         
         Changes
         =======
         
+        Version v4.11.2 (release 2023-06-01)
+        
+        - frontpage: layout changes
+        - translation: add oer frontpage translation
+        - WIP: oer upload button on frontpage
+        
+        
         Version v4.11.1 (release 2023-04-20)
         
         - fix: increase invenio-config-tugraz
         
         
         Version v4.11.0 (release 2023-04-20)
```

### Comparing `invenio-theme-tugraz-4.11.1/README.rst` & `invenio-theme-tugraz-4.11.2/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/docs/Makefile` & `invenio-theme-tugraz-4.11.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/docs/conf.py` & `invenio-theme-tugraz-4.11.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/docs/index.rst` & `invenio-theme-tugraz-4.11.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/docs/make.bat` & `invenio-theme-tugraz-4.11.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/footer.scss` & `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/footer.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/header.scss` & `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/header.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/overrides.scss` & `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/overrides.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/search/footer.scss` & `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/search/footer.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/assets/semantic-ui/js/invenio_theme_tugraz/theme.js` & `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/js/invenio_theme_tugraz/theme.js`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/accounts.less` & `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/accounts.less`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/OFL.txt` & `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/OFL.txt`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/SourceSansPro-Italic.ttf` & `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/SourceSansPro-Italic.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/SourceSansPro-Regular.ttf` & `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/SourceSansPro-Regular.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/footer.less` & `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/footer.less`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/frontpage.less` & `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/frontpage.less`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/header.less` & `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/header.less`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/overrides.less` & `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/overrides.less`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/search.less` & `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/search.less`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/theme.less` & `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/theme.less`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/variables.less` & `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/variables.less`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/config.py` & `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/config.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/ext.py` & `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/search.py` & `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/search.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/static/extra/orcid.png` & `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/extra/orcid.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/static/favicon.ico` & `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/static/images/Fair_Data_Austria_orangerot.png` & `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/images/Fair_Data_Austria_orangerot.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/static/images/Icon_1_v2.svg` & `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/images/Icon_1_v2.svg`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/static/images/TU_Austria_Logo.png` & `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/images/TU_Austria_Logo.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/static/images/footer.jpg` & `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/images/footer.jpg`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/static/images/icon_use.png` & `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/images/icon_use.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/static/images/inveniordm-tail.svg` & `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/images/inveniordm-tail.svg`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/static/images/library_logo.png` & `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/images/library_logo.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/static/images/login_logo.png` & `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/images/login_logo.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/static/images/logo.svg` & `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/static/images/oea.svg` & `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/images/oea.svg`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/static/images/re3data.svg` & `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/images/re3data.svg`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/static/images/tug_logo.png` & `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/images/tug_logo.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/accounts_base.html` & `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/accounts_base.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/header_login.html` & `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/header_login.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/login_user.html` & `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/login_user.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/register_user.html` & `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/register_user.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/templates/invenio_theme_tugraz/base.html` & `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/invenio_theme_tugraz/base.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/templates/invenio_theme_tugraz/benefits.html` & `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/invenio_theme_tugraz/benefits.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/templates/invenio_theme_tugraz/footer.html` & `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/invenio_theme_tugraz/footer.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/templates/invenio_theme_tugraz/header.html` & `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/invenio_theme_tugraz/header.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html` & `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 {#
-  Copyright (C) 2020-2021 Graz University of Technology.
+  Copyright (C) 2020-2023 Graz University of Technology.
 
   invenio-theme-tugraz is free software; you can redistribute it and/or
   modify it under the terms of the MIT License; see LICENSE file for more
   details.
 #}
 
 {%- extends config.INVENIO_THEME_TUGRAZ_BASE_TEMPLATE %}
@@ -19,38 +19,38 @@
 <div class="ui container">
   <div class="ui divider hidden"></div>
 
   <div class="ui stackable grid">
 
     <!---Recent uploads-->
     <div class="ten wide column random-records-frontpage">
-      <h2>{{_('Recent uploads')}}</h2>
+      <h2>{{ _('Recent uploads') }}</h2>
 
       {% if not records %}
       <div class="ui centered grid">
-        <p style="font-size: medium;">{{_('There are no public records to show.')}}</p>
+        <p style="font-size: medium;">{{ _('There are no public records to show.') }}</p>
       </div>
       {% endif %}
 
       {%- for r in records %}
       {%- set creation_date = r.created|from_isodatetime -%}
       {%- set record_url = url_for('invenio_app_rdm_records.record_detail', pid_value=r.id) %}
 
       <article>
         <!--TODO:
         something with doi
         -->
         <div class="badges">
           <!--Publication date/Version badge-->
-          <span class="ui label blue" data-tooltip="{{_('Publication date')}}" data-inverted="">
+          <span class="ui label blue" data-tooltip="{{ _('Publication date') }}" data-inverted="">
             {{ r.metadata.publication_date }} {{ '(' ~ r.metadata.version ~ ')' if r.metadata.version }}
           </span>
 
           <!--Resource type badge-->
-          <span class="ui label grey" data-tooltip="{{_('Resource type')}}" data-inverted>
+          <span class="ui label grey" data-tooltip="{{ _('Resource type') }}" data-inverted>
             {{ r.ui.resource_type.title_l10n }}
           </span>
 
           <span class="ui label access-status {{ r.ui.access_status.id }}" data-tooltip="{{ r.ui.access_status.description_l10n }}" data-inverted="">
             {% if r.ui.access_status.icon %}<i class="icon {{ r.ui.access_status.icon }}"></i>{% endif %}
             {{ r.ui.access_status.title_l10n }}
           </span>
@@ -58,15 +58,15 @@
           <span class="label record-version">
             <!--TODO: add subtype--->
           </span>
         </div>
 
         <h4>
           <a href="{{ record_url }}" class="no-decoration">
-            {{r.metadata.title}}
+            {{ r.metadata.title }}
           </a>
         </h4>
 
         <p>
           {{ creators(r.metadata.creators) }}
         </p>
 
@@ -76,15 +76,15 @@
           </a>
         </p>
 
         <div class="ui grid">
           <div class="two column row">
             <div class="left floated column">
               {%- for s in r.metadata.subjects %}
-              <div class="ui tiny label">{{s.subject}}</div>
+              <div class="ui tiny label">{{ s.subject }}</div>
               {%- endfor %}
               <div>
                 <small>
                   {% trans user=userprofile, date=creation_date | dateformat('long')%}
                   Uploaded on {{date}}
                   {% endtrans %}
                 </small>
@@ -94,50 +94,73 @@
           </div>
         </div>
       </article>
 
       {%- endfor %}
       {% if records %}
       <div class="ui centered grid">
-        <a class="ui button more" href="{{url_for('invenio_search_ui.search')}}">{{_('More')}}</a>
+        <a class="ui button more" href="{{ url_for('invenio_search_ui.search') }}">{{ _('More') }}</a>
       </div>
       {%- endif %}
     </div>
 
 
     <!---segments-->
     <div class="six wide column">
-      <!--contact us-->
       <div class="ui segment" style="padding-bottom: 10px;">
-        <h4>{{_ ("Need help?")}}</h4>
+        <h4>{{ _("You can upload different types of records:") }}</h4>
+
+        <p style="margin: 14px">
+          <span class="ui left floated" style="text-align: justify; width:260px; display:inline-block;">
+            {{ _("Visibility of uploaded content is maximized through synchronization with data hubs (DataCite).") }}
+          </span>
+          <a class="ui positive right floated button" style="width:250px; display:inline-block;" href="me/uploads" title="Research Data">
+            <i aria-hidden="true" class="upload icon"></i>
+            {{ _("Upload Research Output") }}
+          </a>
+        </p>
+        <p style="margin: 14px;">
+          <span class="ui left floated" style="text-align: justify; width:260px; display:inline-block;">
+            {{ _("Open Educational Resources (OER) will be visible on various discovery tools like the OERhub.") }}
+          </span>
+
+          <a class="ui positive right floated button" style="width:250px; display:inline-block;" href="lom/uploads" title="Open Educational Resources">
+            <i aria-hidden="true" class="upload icon"></i>
+            {{ _("Upload OER") }}
+          </a>
+        </p>
+      </div>
+
+      <!--contact us-->
+      <div class="ui segment">
+        <h4>{{ _("Need help?") }}</h4>
         {%- if config.THEME_TUGRAZ_CONTACT_FORM %}
         <div style="padding-bottom: 10px;">
           <a id="feedback-form" class="fluid ui button">
-            {{_ ("Contact us")}} 
+            {{ _("Contact us") }}
           </a>
         </div>
         {%- endif %}
         <p>
-          {{config.THEME_SITENAME}} {{_ ("prioritizes all Recent uploads.")}}
+          {{ config.THEME_SITENAME }} {{ _("prioritizes all Recent uploads.") }}
         </p>
         <p>
-          {{_ ("We can help with:")}} 
-          
+          {{ _("We can help with:") }}
         </p>
 
         <ul>
-          <li>{{_ ("Uploading your research data, software, preprints, etc.")}}</li>
-          <li>{{_ ("One-on-one with")}} {{config.THEME_SITENAME}} {{_ ("supporters.")}}</li>
-          <li>{{_ ("Quota increases beyond our default policy.")}}</li>
-          <li>{{_ ("Scripts for automated uploading of larger datasets.")}}</li>
+          <li>{{ _("Uploading your research data, software, preprints, etc.") }}</li>
+          <li>{{ _("One-on-one with") }} {{ config.THEME_SITENAME }} {{ _("supporters.") }}</li>
+          <li>{{ _("Quota increases beyond our default policy.") }}</li>
+          <li>{{ _("Scripts for automated uploading of larger datasets.") }}</li>
         </ul>
       </div>
 
       <div class="ui segment" style="padding-bottom: 10px;">
-        <h4>{{_ ("Why use")}} {{config.THEME_SITENAME}}?</h4>
+        <h4>{{ _("Why use") }} {{ config.THEME_SITENAME }}?</h4>
 
         {% include "invenio_theme_tugraz/benefits.html" %}
       </div>
     </div>
   </div>
 </div>
```

#### html2text {}

```diff
@@ -1,40 +1,48 @@
-{# Copyright (C) 2020-2021 Graz University of Technology. invenio-theme-tugraz
+{# Copyright (C) 2020-2023 Graz University of Technology. invenio-theme-tugraz
 is free software; you can redistribute it and/or modify it under the terms of
 the MIT License; see LICENSE file for more details. #} {%- extends
 config.INVENIO_THEME_TUGRAZ_BASE_TEMPLATE %} {%- block javascript %} {{ webpack
 ['invenio-theme-tugraz-js.js'] }} {%- endblock javascript %} {%- from
 "invenio_theme_tugraz/macros/authors.html" import creators -%} {%- block
 page_body %}
-***** {{_('Recent uploads')}} *****
+***** {{ _('Recent uploads') }} *****
 {% if not records %}
-{{_('There are no public records to show.')}}
+{{ _('There are no public records to show.') }}
 {% endif %} {%- for r in records %} {%- set creation_date =
 r.created|from_isodatetime -%} {%- set record_url = url_for
 ('invenio_app_rdm_records.record_detail', pid_value=r.id) %}
   {{ r.metadata.publication_date }} {{ '(' ~ r.metadata.version ~ ')' if
 r.metadata.version }}    {{ r.ui.resource_type.title_l10n }}   {% if
 r.ui.access_status.icon %}{% endif %} {{ r.ui.access_status.title_l10n }}
-*** {{r.metadata.title}} ***
+*** {{_r.metadata.title_}} ***
 {{ creators(r.metadata.creators) }}
 {{_r.metadata.description_|_striptags_|_truncate(300)_}}
 {%- for s in r.metadata.subjects %}
-{{s.subject}}
+{{ s.subject }}
 {%- endfor %}
 {% trans user=userprofile, date=creation_date | dateformat('long')%} Uploaded
 on {{date}} {% endtrans %}
  {%- endfor %} {% if records %}
-{{_('More')}}
+{{__('More')_}}
 {%- endif %}
-*** {{_ ("Need help?")}} ***
+*** {{ _("You can upload different types of records:") }} ***
+ {{ _("Visibility of uploaded content is maximized through synchronization with
+data hubs (DataCite).") }}
+ {{__("Upload_Research_Output")_}}
+ {{ _("Open Educational Resources (OER) will be visible on various discovery
+tools like the OERhub.") }}
+ {{__("Upload_OER")_}}
+*** {{ _("Need help?") }} ***
 {%- if config.THEME_TUGRAZ_CONTACT_FORM %}
-{{_ ("Contact us")}}
+{{ _("Contact us") }}
 {%- endif %}
-{{config.THEME_SITENAME}} {{_ ("prioritizes all Recent uploads.")}}
-{{_ ("We can help with:")}}
-    * {{_ ("Uploading your research data, software, preprints, etc.")}}
-    * {{_ ("One-on-one with")}} {{config.THEME_SITENAME}} {{_ ("supporters.")}}
-    * {{_ ("Quota increases beyond our default policy.")}}
-    * {{_ ("Scripts for automated uploading of larger datasets.")}}
-*** {{_ ("Why use")}} {{config.THEME_SITENAME}}? ***
+{{ config.THEME_SITENAME }} {{ _("prioritizes all Recent uploads.") }}
+{{ _("We can help with:") }}
+    * {{ _("Uploading your research data, software, preprints, etc.") }}
+    * {{ _("One-on-one with") }} {{ config.THEME_SITENAME }} {{ _
+      ("supporters.") }}
+    * {{ _("Quota increases beyond our default policy.") }}
+    * {{ _("Scripts for automated uploading of larger datasets.") }}
+*** {{ _("Why use") }} {{ config.THEME_SITENAME }}? ***
 {% include "invenio_theme_tugraz/benefits.html" %}
 {%- endblock %}
```

### Comparing `invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/templates/invenio_theme_tugraz/macros/authors.html` & `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/invenio_theme_tugraz/macros/authors.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/templates/invenio_theme_tugraz/navbar.html` & `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/invenio_theme_tugraz/navbar.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/translations/de/LC_MESSAGES/messages.mo` & `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/translations/de/LC_MESSAGES/messages.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,13 +1,13 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-theme-tugraz 1.0.4\n"
 "Report-Msgid-Bugs-To: mojib.wali@tugraz.at\n"
-"POT-Creation-Date: 2022-08-05 10:15+0200\n"
-"PO-Revision-Date: 2022-08-05 10:21+0200\n"
+"POT-Creation-Date: 2023-05-26 09:37+0200\n"
+"PO-Revision-Date: 2023-05-31 15:27+0200\n"
 "Last-Translator: \n"
 "Language: de\n"
 "Language-Team: de <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -142,14 +142,21 @@
 
 msgid "One-on-one with"
 msgstr "One-on-one mit"
 
 msgid "Open Educational Resources"
 msgstr "Open Educational Resources"
 
+msgid ""
+"Open Educational Resources (OER) will be visible on various discovery tools "
+"like the OERhub."
+msgstr ""
+"Open Educational Resources (OER) werden auf Suchmaschinen wie OERhub "
+"sichtbar sein."
+
 msgid "Open or closed"
 msgstr "Offen oder geschlossen"
 
 msgid "Or"
 msgstr "Oder"
 
 msgid "PASSION"
@@ -248,14 +255,20 @@
 
 msgid "Trusted"
 msgstr "Vertrauenswürdig"
 
 msgid "Trusted Research Data Management"
 msgstr "Vertrauenswürdiges Forschungsdatenmanagement"
 
+msgid "Upload OER"
+msgstr "Upload OER"
+
+msgid "Upload Research Output"
+msgstr "Upload Forschungsergebnisse"
+
 msgid "Uploading your research data, software, preprints, etc."
 msgstr "Hochladen Ihrer Forschungsdaten, Software, Preprints usw."
 
 msgid ""
 "Uploads are made available online as soon as you hit publish, and your DOI "
 "is registered within seconds."
 msgstr ""
@@ -273,20 +286,30 @@
 
 msgid "Use Ctrl + and Crtl -"
 msgstr "Verwenden Sie Strg+ und Strg-"
 
 msgid "Versioning"
 msgstr "Versionierung"
 
+msgid ""
+"Visibility of uploaded content is maximized through synchronization with "
+"data hubs (DataCite)."
+msgstr ""
+"Steigerung der Sichtbarkeit der Datensätze durch Synchronisation mit "
+"Harvestern (DataCite)."
+
 msgid "We can help with:"
 msgstr "Dabei können wir helfen:"
 
 msgid "Why use"
 msgstr "Warum"
 
+msgid "You can upload different types of records:"
+msgstr "Upload verschiedener Arten von Datensätzen:"
+
 msgid ""
 "built and operated by CERN and OpenAIRE to ensure that everyone can join in "
 "Open Science."
 msgstr ""
 "Aufgebaut und betrieben von CERN und OpenAIRE, um sicherzustellen, dass "
 "jeder an Open Science teilnehmen kann."
```

### Comparing `invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/translations/de/LC_MESSAGES/messages.po` & `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/translations/de/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 # invenio-theme-tugraz project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2020.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-theme-tugraz 1.0.4\n"
 "Report-Msgid-Bugs-To: mojib.wali@tugraz.at\n"
-"POT-Creation-Date: 2022-08-05 10:15+0200\n"
-"PO-Revision-Date: 2022-08-05 10:21+0200\n"
+"POT-Creation-Date: 2023-05-26 09:37+0200\n"
+"PO-Revision-Date: 2023-05-31 15:27+0200\n"
 "Last-Translator: \n"
 "Language-Team: de <LL@li.org>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
@@ -194,16 +194,16 @@
 msgid "to change the font size."
 msgstr "Um die Schriftgröße zu ändern."
 
 #: invenio_theme_tugraz/templates/invenio_theme_tugraz/footer.html:117
 #, fuzzy, python-format
 msgid ""
 "<strong>Powered by</strong>\n"
-"            <a href=\"%(invenio_rdm)s\" target=\"_blank\" title=\"invenioRDM"
-"\">"
+"            <a href=\"%(invenio_rdm)s\" target=\"_blank\" "
+"title=\"invenioRDM\">"
 msgstr ""
 "<strong>Powered by</strong> <a href=\"%(invenio_rdm)s\" target=\"_blank\">"
 
 #: invenio_theme_tugraz/templates/invenio_theme_tugraz/footer.html:126
 #, fuzzy, python-format
 msgid ""
 "<strong>Enabled by</strong>\n"
@@ -268,51 +268,79 @@
 "\n"
 "\t\tHochgeladen am %(date)s"
 
 #: invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html:101
 msgid "More"
 msgstr "Mehr"
 
-#: invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html:111
+#: invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html:110
+msgid "You can upload different types of records:"
+msgstr "Upload verschiedener Arten von Datensätzen:"
+
+#: invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html:114
+msgid ""
+"Visibility of uploaded content is maximized through synchronization with "
+"data hubs (DataCite)."
+msgstr ""
+"Steigerung der Sichtbarkeit der Datensätze durch Synchronisation mit "
+"Harvestern (DataCite)."
+
+#: invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html:118
+msgid "Upload Research Output"
+msgstr "Upload Forschungsergebnisse"
+
+#: invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html:123
+msgid ""
+"Open Educational Resources (OER) will be visible on various discovery tools "
+"like the OERhub."
+msgstr ""
+"Open Educational Resources (OER) werden auf Suchmaschinen wie OERhub "
+"sichtbar sein."
+
+#: invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html:128
+msgid "Upload OER"
+msgstr "Upload OER"
+
+#: invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html:135
 msgid "Need help?"
 msgstr "Brauchen Sie Hilfe?"
 
-#: invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html:115
+#: invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html:139
 msgid "Contact us"
 msgstr "Kontaktiere uns"
 
-#: invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html:120
+#: invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html:144
 msgid "prioritizes all Recent uploads."
 msgstr "reiht die neuesten Uploads vor."
 
-#: invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html:123
+#: invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html:147
 msgid "We can help with:"
 msgstr "Dabei können wir helfen:"
 
-#: invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html:128
+#: invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html:151
 msgid "Uploading your research data, software, preprints, etc."
 msgstr "Hochladen Ihrer Forschungsdaten, Software, Preprints usw."
 
-#: invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html:129
+#: invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html:152
 msgid "One-on-one with"
 msgstr "One-on-one mit"
 
-#: invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html:129
+#: invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html:152
 msgid "supporters."
 msgstr "Unterstützern"
 
-#: invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html:130
+#: invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html:153
 msgid "Quota increases beyond our default policy."
 msgstr "Quota Erhöhungen über unsere Standard Policy hinaus."
 
-#: invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html:131
+#: invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html:154
 msgid "Scripts for automated uploading of larger datasets."
 msgstr "Skripte zum automatisierten Hochladen größerer Datensätze."
 
-#: invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html:136
+#: invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html:159
 msgid "Why use"
 msgstr "Warum"
 
 #: invenio_theme_tugraz/templates/invenio_theme_tugraz/navbar.html:12
 msgid "All"
 msgstr "Alle"
 
@@ -454,17 +482,14 @@
 
 #~ msgid "RDM DOI Badge"
 #~ msgstr "RDM DOI Abzeichen"
 
 #~ msgid "DOI"
 #~ msgstr "DOI"
 
-#~ msgid "Uploads"
-#~ msgstr "Hochladen"
-
 #~ msgid "German"
 #~ msgstr "Deutsche"
 
 #~ msgid "New version"
 #~ msgstr "neue Version"
 
 #~ msgid "New upload"
```

### Comparing `invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/translations/messages.pot` & `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/translations/messages.pot`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # Translations template for invenio-theme-tugraz.
-# Copyright (C) 2022 Graz University of Technology
+# Copyright (C) 2023 Graz University of Technology
 # This file is distributed under the same license as the
 # invenio-theme-tugraz project.
-# FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
+# FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 #
 #, fuzzy
 msgid ""
 msgstr ""
-"Project-Id-Version: invenio-theme-tugraz 4.0.0\n"
+"Project-Id-Version: invenio-theme-tugraz 4.11.1\n"
 "Report-Msgid-Bugs-To: mojib.wali@tugraz.at\n"
-"POT-Creation-Date: 2022-08-05 10:15+0200\n"
+"POT-Creation-Date: 2023-05-26 09:37+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.10.1\n"
 
 #: invenio_theme_tugraz/config.py:13 invenio_theme_tugraz/config.py:60
 msgid "TU Graz Repository"
 msgstr ""
 
 #: invenio_theme_tugraz/config.py:63
 #: invenio_theme_tugraz/templates/invenio_theme_tugraz/footer.html:30
@@ -252,51 +252,75 @@
 "                  "
 msgstr ""
 
 #: invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html:101
 msgid "More"
 msgstr ""
 
-#: invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html:111
+#: invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html:110
+msgid "You can upload different types of records:"
+msgstr ""
+
+#: invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html:114
+msgid ""
+"Visibility of uploaded content is maximized through synchronization with "
+"data hubs (DataCite)."
+msgstr ""
+
+#: invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html:118
+msgid "Upload Research Output"
+msgstr ""
+
+#: invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html:123
+msgid ""
+"Open Educational Resources (OER) will be visible on various discovery "
+"tools like the OERhub."
+msgstr ""
+
+#: invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html:128
+msgid "Upload OER"
+msgstr ""
+
+#: invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html:135
 msgid "Need help?"
 msgstr ""
 
-#: invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html:115
+#: invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html:139
 msgid "Contact us"
 msgstr ""
 
-#: invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html:120
+#: invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html:144
 msgid "prioritizes all Recent uploads."
 msgstr ""
 
-#: invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html:123
+#: invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html:147
 msgid "We can help with:"
 msgstr ""
 
-#: invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html:128
+#: invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html:151
 msgid "Uploading your research data, software, preprints, etc."
 msgstr ""
 
-#: invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html:129
+#: invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html:152
 msgid "One-on-one with"
 msgstr ""
 
-#: invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html:129
+#: invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html:152
 msgid "supporters."
 msgstr ""
 
-#: invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html:130
+#: invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html:153
 msgid "Quota increases beyond our default policy."
 msgstr ""
 
-#: invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html:131
+#: invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html:154
 msgid "Scripts for automated uploading of larger datasets."
 msgstr ""
 
-#: invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html:136
+#: invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html:159
 msgid "Why use"
 msgstr ""
 
 #: invenio_theme_tugraz/templates/invenio_theme_tugraz/navbar.html:12
 msgid "All"
 msgstr ""
```

### Comparing `invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/views.py` & `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/views.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/invenio_theme_tugraz/webpack.py` & `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/webpack.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/invenio_theme_tugraz.egg-info/PKG-INFO` & `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-theme-tugraz
-Version: 4.11.1
+Version: 4.11.2
 Summary: "Invenio module for TUGRAZ theme."
 Home-page: https://github.com/tu-graz-library/invenio-theme-tugraz
 Author: "Graz University of Technology"
 Author-email: mojib.wali@tugraz.at
 License: MIT
 Description: ..
             Copyright (C) 2020-2021 Graz University of Technology.
@@ -58,14 +58,21 @@
             invenio-theme-tugraz is free software; you can redistribute it and/or
             modify it under the terms of the MIT License; see LICENSE file for more
             details.
         
         Changes
         =======
         
+        Version v4.11.2 (release 2023-06-01)
+        
+        - frontpage: layout changes
+        - translation: add oer frontpage translation
+        - WIP: oer upload button on frontpage
+        
+        
         Version v4.11.1 (release 2023-04-20)
         
         - fix: increase invenio-config-tugraz
         
         
         Version v4.11.0 (release 2023-04-20)
```

### Comparing `invenio-theme-tugraz-4.11.1/invenio_theme_tugraz.egg-info/SOURCES.txt` & `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/requirements-devel.txt` & `invenio-theme-tugraz-4.11.2/requirements-devel.txt`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/run-tests.sh` & `invenio-theme-tugraz-4.11.2/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/setup.cfg` & `invenio-theme-tugraz-4.11.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/tests/conftest.py` & `invenio-theme-tugraz-4.11.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.1/tests/test_invenio_theme_tugraz.py` & `invenio-theme-tugraz-4.11.2/tests/test_invenio_theme_tugraz.py`

 * *Files identical despite different names*

