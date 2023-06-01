# Comparing `tmp/hxl-proxy-2.0.tar.gz` & `tmp/hxl_proxy-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hxl-proxy-2.0.tar", last modified: Tue May 23 20:32:22 2023, max compression
+gzip compressed data, was "hxl_proxy-2.0.1.tar", last modified: Thu Jun  1 16:49:14 2023, max compression
```

## Comparing `hxl-proxy-2.0.tar` & `hxl_proxy-2.0.1.tar`

### file list

```diff
@@ -1,157 +1,157 @@
-drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-05-23 20:32:22.019588 hxl-proxy-2.0/
--rw-rw-r--   0 david     (1001) david     (1001)     1210 2022-10-28 23:21:23.000000 hxl-proxy-2.0/LICENSE.md
--rw-rw-r--   0 david     (1001) david     (1001)       77 2022-10-28 23:21:23.000000 hxl-proxy-2.0/MANIFEST.in
--rw-rw-r--   0 david     (1001) david     (1001)     3514 2023-05-23 20:32:22.019588 hxl-proxy-2.0/PKG-INFO
--rw-rw-r--   0 david     (1001) david     (1001)     3209 2022-10-28 23:21:23.000000 hxl-proxy-2.0/README.md
-drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-05-23 20:32:22.003588 hxl-proxy-2.0/hxl_proxy/
--rw-rw-r--   0 david     (1001) david     (1001)     4356 2023-05-23 20:30:05.000000 hxl-proxy-2.0/hxl_proxy/__init__.py
--rw-rw-r--   0 david     (1001) david     (1001)     3194 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/admin.py
--rw-rw-r--   0 david     (1001) david     (1001)     1925 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/auth.py
--rw-rw-r--   0 david     (1001) david     (1001)     1660 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/caching.py
--rw-rw-r--   0 david     (1001) david     (1001)    51713 2023-05-23 20:28:31.000000 hxl-proxy-2.0/hxl_proxy/controllers.py
--rw-rw-r--   0 david     (1001) david     (1001)    12898 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/dao.py
--rw-rw-r--   0 david     (1001) david     (1001)      352 2022-11-25 16:22:47.000000 hxl-proxy-2.0/hxl_proxy/default_config.py
--rw-rw-r--   0 david     (1001) david     (1001)     1878 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/exceptions.py
--rw-rw-r--   0 david     (1001) david     (1001)    14423 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/filters.py
--rw-rw-r--   0 david     (1001) david     (1001)     4223 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/pcodes.py
--rw-rw-r--   0 david     (1001) david     (1001)      929 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/preview.py
--rw-rw-r--   0 david     (1001) david     (1001)     5398 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/recipes.py
--rw-rw-r--   0 david     (1001) david     (1001)     1465 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/reverse_proxied.py
--rw-rw-r--   0 david     (1001) david     (1001)      929 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/schema-mysql.sql
--rw-rw-r--   0 david     (1001) david     (1001)      650 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/schema-sqlite3.sql
-drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-05-23 20:32:21.999588 hxl-proxy-2.0/hxl_proxy/static/
-drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-05-23 20:32:21.999588 hxl-proxy-2.0/hxl_proxy/static/bootstrap/
-drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-05-23 20:32:22.003588 hxl-proxy-2.0/hxl_proxy/static/bootstrap/css/
--rw-rw-r--   0 david     (1001) david     (1001)    22608 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/bootstrap/css/bootstrap-theme.css
--rw-rw-r--   0 david     (1001) david     (1001)    43339 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/bootstrap/css/bootstrap-theme.css.map
--rw-rw-r--   0 david     (1001) david     (1001)    19963 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/bootstrap/css/bootstrap-theme.min.css
--rw-rw-r--   0 david     (1001) david     (1001)   141414 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/bootstrap/css/bootstrap.css
--rw-rw-r--   0 david     (1001) david     (1001)   379710 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/bootstrap/css/bootstrap.css.map
--rw-rw-r--   0 david     (1001) david     (1001)   117150 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/bootstrap/css/bootstrap.min.css
-drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-05-23 20:32:22.007588 hxl-proxy-2.0/hxl_proxy/static/bootstrap/fonts/
--rw-rw-r--   0 david     (1001) david     (1001)    20127 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/bootstrap/fonts/glyphicons-halflings-regular.eot
--rw-rw-r--   0 david     (1001) david     (1001)   108738 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/bootstrap/fonts/glyphicons-halflings-regular.svg
--rw-rw-r--   0 david     (1001) david     (1001)    45404 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/bootstrap/fonts/glyphicons-halflings-regular.ttf
--rw-rw-r--   0 david     (1001) david     (1001)    23424 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/bootstrap/fonts/glyphicons-halflings-regular.woff
--rw-rw-r--   0 david     (1001) david     (1001)    18028 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/bootstrap/fonts/glyphicons-halflings-regular.woff2
-drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-05-23 20:32:22.007588 hxl-proxy-2.0/hxl_proxy/static/bootstrap/js/
--rw-rw-r--   0 david     (1001) david     (1001)    66732 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/bootstrap/js/bootstrap.js
--rw-rw-r--   0 david     (1001) david     (1001)    35452 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/bootstrap/js/bootstrap.min.js
--rw-rw-r--   0 david     (1001) david     (1001)      484 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/bootstrap/js/npm.js
-drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-05-23 20:32:22.007588 hxl-proxy-2.0/hxl_proxy/static/compat/
--rw-rw-r--   0 david     (1001) david     (1001)     2636 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/compat/html5shiv.min.js
--rw-rw-r--   0 david     (1001) david     (1001)      694 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/compat/ie10-viewport-bug-workaround.js
--rw-rw-r--   0 david     (1001) david     (1001)     4377 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/compat/respond.min.js
-drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-05-23 20:32:22.007588 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/
--rw-rw-r--   0 david     (1001) david     (1001)     3470 2023-04-04 17:11:40.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/hxl-proxy.css
--rw-rw-r--   0 david     (1001) david     (1001)    15879 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/hxl-proxy.js
-drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-05-23 20:32:22.011588 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/
--rw-rw-r--   0 david     (1001) david     (1001)     9448 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/android-icon-144x144.png
--rw-rw-r--   0 david     (1001) david     (1001)    11645 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/android-icon-192x192.png
--rw-rw-r--   0 david     (1001) david     (1001)     1960 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/android-icon-36x36.png
--rw-rw-r--   0 david     (1001) david     (1001)     3057 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/android-icon-48x48.png
--rw-rw-r--   0 david     (1001) david     (1001)     4171 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/android-icon-72x72.png
--rw-rw-r--   0 david     (1001) david     (1001)     5857 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/android-icon-96x96.png
--rw-rw-r--   0 david     (1001) david     (1001)     7317 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/apple-icon-114x114.png
--rw-rw-r--   0 david     (1001) david     (1001)     7631 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/apple-icon-120x120.png
--rw-rw-r--   0 david     (1001) david     (1001)     9448 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/apple-icon-144x144.png
--rw-rw-r--   0 david     (1001) david     (1001)    10058 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/apple-icon-152x152.png
--rw-rw-r--   0 david     (1001) david     (1001)    12668 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/apple-icon-180x180.png
--rw-rw-r--   0 david     (1001) david     (1001)     2618 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/apple-icon-57x57.png
--rw-rw-r--   0 david     (1001) david     (1001)     3820 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/apple-icon-60x60.png
--rw-rw-r--   0 david     (1001) david     (1001)     4171 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/apple-icon-72x72.png
--rw-rw-r--   0 david     (1001) david     (1001)     4491 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/apple-icon-76x76.png
--rw-rw-r--   0 david     (1001) david     (1001)    12219 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/apple-icon-precomposed.png
--rw-rw-r--   0 david     (1001) david     (1001)    12219 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/apple-icon.png
--rw-rw-r--   0 david     (1001) david     (1001)      281 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/browserconfig.xml
--rw-rw-r--   0 david     (1001) david     (1001)     1249 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/favicon-16x16.png
--rw-rw-r--   0 david     (1001) david     (1001)     1899 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/favicon-32x32.png
--rw-rw-r--   0 david     (1001) david     (1001)     5857 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/favicon-96x96.png
--rw-rw-r--   0 david     (1001) david     (1001)     1150 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/favicon.ico
--rw-rw-r--   0 david     (1001) david     (1001)     1165 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/manifest.json
--rw-rw-r--   0 david     (1001) david     (1001)     9448 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/ms-icon-144x144.png
--rw-rw-r--   0 david     (1001) david     (1001)    10073 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/ms-icon-150x150.png
--rw-rw-r--   0 david     (1001) david     (1001)    27390 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/ms-icon-310x310.png
--rw-rw-r--   0 david     (1001) david     (1001)     4125 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/ms-icon-70x70.png
-drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-05-23 20:32:22.015588 hxl-proxy-2.0/hxl_proxy/static/images/
--rw-rw-r--   0 david     (1001) david     (1001)     8850 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/images/csv-icon.png
--rw-rw-r--   0 david     (1001) david     (1001)    13225 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/images/dropbox-logo.png
--rw-rw-r--   0 david     (1001) david     (1001)    22085 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/images/google-drive-logo.png
--rw-rw-r--   0 david     (1001) david     (1001)     7767 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/images/hdx-logo.png
--rw-rw-r--   0 david     (1001) david     (1001)     2454 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/images/hxl-logo-white.png
--rw-rw-r--   0 david     (1001) david     (1001)    55429 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/images/json-icon.png
-drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-05-23 20:32:22.015588 hxl-proxy-2.0/hxl_proxy/static/jquery/
--rw-rw-r--   0 david     (1001) david     (1001)   240427 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/jquery/jquery-ui.min.js
--rw-rw-r--   0 david     (1001) david     (1001)    10469 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/jquery/jquery.csv.js
--rw-rw-r--   0 david     (1001) david     (1001)    84320 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/jquery/jquery.js
--rw-rw-r--   0 david     (1001) david     (1001)     1291 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/static/jquery/jquery.ui.touch-punch.min.js
-drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-05-23 20:32:22.015588 hxl-proxy-2.0/hxl_proxy/templates/
--rw-rw-r--   0 david     (1001) david     (1001)     4570 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/about.html
--rw-rw-r--   0 david     (1001) david     (1001)     5224 2023-03-20 15:47:35.000000 hxl-proxy-2.0/hxl_proxy/templates/api-data-preview.html
--rw-rw-r--   0 david     (1001) david     (1001)     4462 2023-03-20 15:47:35.000000 hxl-proxy-2.0/hxl_proxy/templates/api-from-spec.html
--rw-rw-r--   0 david     (1001) david     (1001)     3506 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/data-advanced.html
--rw-rw-r--   0 david     (1001) david     (1001)     2227 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/data-logs.html
--rw-rw-r--   0 david     (1001) david     (1001)     9122 2023-04-04 17:11:40.000000 hxl-proxy-2.0/hxl_proxy/templates/data-recipe.html
--rw-rw-r--   0 david     (1001) david     (1001)     5109 2023-03-20 15:47:35.000000 hxl-proxy-2.0/hxl_proxy/templates/data-source.html
--rw-rw-r--   0 david     (1001) david     (1001)     6758 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/data-tagger.html
--rw-rw-r--   0 david     (1001) david     (1001)     2547 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/data-view.html
--rw-rw-r--   0 david     (1001) david     (1001)     1206 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/error.html
--rw-rw-r--   0 david     (1001) david     (1001)     1247 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/hash.html
--rw-rw-r--   0 david     (1001) david     (1001)     2672 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/hxl-test.html
-drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-05-23 20:32:22.019588 hxl-proxy-2.0/hxl_proxy/templates/includes/
--rw-rw-r--   0 david     (1001) david     (1001)      153 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/admin-alert.html
--rw-rw-r--   0 david     (1001) david     (1001)      496 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/chooser-scripts.html
--rw-rw-r--   0 david     (1001) david     (1001)      959 2023-03-20 15:47:35.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/data-tabs.html
-drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-05-23 20:32:22.019588 hxl-proxy-2.0/hxl_proxy/templates/includes/filters/
--rw-rw-r--   0 david     (1001) david     (1001)     1815 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/filters/add.html
--rw-rw-r--   0 david     (1001) david     (1001)     1737 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/filters/append-list.html
--rw-rw-r--   0 david     (1001) david     (1001)     2308 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/filters/append.html
--rw-rw-r--   0 david     (1001) david     (1001)     5188 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/filters/clean.html
--rw-rw-r--   0 david     (1001) david     (1001)     6021 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/filters/count.html
--rw-rw-r--   0 david     (1001) david     (1001)     1510 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/filters/cut.html
--rw-rw-r--   0 david     (1001) david     (1001)     1258 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/filters/dedup.html
--rw-rw-r--   0 david     (1001) david     (1001)     2166 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/filters/expand.html
--rw-rw-r--   0 david     (1001) david     (1001)     1344 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/filters/explode.html
--rw-rw-r--   0 david     (1001) david     (1001)     1227 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/filters/fill.html
--rw-rw-r--   0 david     (1001) david     (1001)      630 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/filters/filter-list.html
--rw-rw-r--   0 david     (1001) david     (1001)      643 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/filters/filter-selector.html
--rw-rw-r--   0 david     (1001) david     (1001)      691 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/filters/filter-types.j2
--rw-rw-r--   0 david     (1001) david     (1001)     1191 2023-03-20 15:47:35.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/filters/filter-variables.j2
--rw-rw-r--   0 david     (1001) david     (1001)     1258 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/filters/implode.html
--rw-rw-r--   0 david     (1001) david     (1001)     2051 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/filters/jsonpath.html
--rw-rw-r--   0 david     (1001) david     (1001)      334 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/filters/label-field-multicol.html
--rw-rw-r--   0 david     (1001) david     (1001)      324 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/filters/label-field.html
--rw-rw-r--   0 david     (1001) david     (1001)     2480 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/filters/merge.html
--rw-rw-r--   0 david     (1001) david     (1001)     1931 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/filters/rename.html
--rw-rw-r--   0 david     (1001) david     (1001)     1311 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/filters/replace-map.html
--rw-rw-r--   0 david     (1001) david     (1001)     2192 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/filters/replace.html
--rw-rw-r--   0 david     (1001) david     (1001)     1240 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/filters/select.html
--rw-rw-r--   0 david     (1001) david     (1001)      963 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/filters/sort.html
--rw-rw-r--   0 david     (1001) david     (1001)     2317 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/headers.html
--rw-rw-r--   0 david     (1001) david     (1001)      171 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/help.html
--rw-rw-r--   0 david     (1001) david     (1001)      847 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/hxltable.html
--rw-rw-r--   0 david     (1001) david     (1001)      259 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/messages.html
--rw-rw-r--   0 david     (1001) david     (1001)      365 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/metadata-params.html
--rw-rw-r--   0 david     (1001) david     (1001)     3378 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/navbar.html
--rw-rw-r--   0 david     (1001) david     (1001)      153 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/params.html
--rw-rw-r--   0 david     (1001) david     (1001)      790 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/postcards.html
--rw-rw-r--   0 david     (1001) david     (1001)      142 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/recipe-form.html
--rw-rw-r--   0 david     (1001) david     (1001)      412 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/recipe-params.html
--rw-rw-r--   0 david     (1001) david     (1001)      443 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/scripts.html
--rw-rw-r--   0 david     (1001) david     (1001)      368 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/selectors.html
--rw-rw-r--   0 david     (1001) david     (1001)      182 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/source.html
--rw-rw-r--   0 david     (1001) david     (1001)      382 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/includes/tagger-params.html
--rw-rw-r--   0 david     (1001) david     (1001)     1633 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/settings-user.html
--rw-rw-r--   0 david     (1001) david     (1001)     2433 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/validate-issue.html
--rw-rw-r--   0 david     (1001) david     (1001)     5437 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/templates/validate-summary.html
--rw-rw-r--   0 david     (1001) david     (1001)    16476 2023-03-20 15:47:35.000000 hxl-proxy-2.0/hxl_proxy/util.py
--rw-rw-r--   0 david     (1001) david     (1001)     3270 2022-10-28 23:21:23.000000 hxl-proxy-2.0/hxl_proxy/validate.py
-drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-05-23 20:32:22.003588 hxl-proxy-2.0/hxl_proxy.egg-info/
--rw-rw-r--   0 david     (1001) david     (1001)     3514 2023-05-23 20:32:21.000000 hxl-proxy-2.0/hxl_proxy.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1001) david     (1001)     5980 2023-05-23 20:32:21.000000 hxl-proxy-2.0/hxl_proxy.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1001) david     (1001)       64 2023-05-23 20:32:21.000000 hxl-proxy-2.0/hxl_proxy.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1001) david     (1001)        1 2022-10-29 17:11:19.000000 hxl-proxy-2.0/hxl_proxy.egg-info/not-zip-safe
--rw-rw-r--   0 david     (1001) david     (1001)      151 2023-05-23 20:32:21.000000 hxl-proxy-2.0/hxl_proxy.egg-info/requires.txt
--rw-rw-r--   0 david     (1001) david     (1001)       10 2023-05-23 20:32:21.000000 hxl-proxy-2.0/hxl_proxy.egg-info/top_level.txt
--rw-rw-r--   0 david     (1001) david     (1001)       38 2023-05-23 20:32:22.019588 hxl-proxy-2.0/setup.cfg
--rwxrwxr-x   0 david     (1001) david     (1001)     1337 2023-05-23 20:30:05.000000 hxl-proxy-2.0/setup.py
+drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-06-01 16:49:14.901283 hxl_proxy-2.0.1/
+-rw-rw-r--   0 david     (1001) david     (1001)     1210 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/LICENSE.md
+-rw-rw-r--   0 david     (1001) david     (1001)       77 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/MANIFEST.in
+-rw-rw-r--   0 david     (1001) david     (1001)     3829 2023-06-01 16:49:14.901283 hxl_proxy-2.0.1/PKG-INFO
+-rw-rw-r--   0 david     (1001) david     (1001)     3209 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/README.md
+drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-06-01 16:49:14.897283 hxl_proxy-2.0.1/hxl_proxy/
+-rw-rw-r--   0 david     (1001) david     (1001)     4358 2023-06-01 16:48:29.000000 hxl_proxy-2.0.1/hxl_proxy/__init__.py
+-rw-rw-r--   0 david     (1001) david     (1001)     3194 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/admin.py
+-rw-rw-r--   0 david     (1001) david     (1001)     1925 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/auth.py
+-rw-rw-r--   0 david     (1001) david     (1001)     1660 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/caching.py
+-rw-rw-r--   0 david     (1001) david     (1001)    51906 2023-06-01 16:48:29.000000 hxl_proxy-2.0.1/hxl_proxy/controllers.py
+-rw-rw-r--   0 david     (1001) david     (1001)    12898 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/dao.py
+-rw-rw-r--   0 david     (1001) david     (1001)      341 2023-06-01 16:48:29.000000 hxl_proxy-2.0.1/hxl_proxy/default_config.py
+-rw-rw-r--   0 david     (1001) david     (1001)     1878 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/exceptions.py
+-rw-rw-r--   0 david     (1001) david     (1001)    14423 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/filters.py
+-rw-rw-r--   0 david     (1001) david     (1001)     4223 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/pcodes.py
+-rw-rw-r--   0 david     (1001) david     (1001)      929 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/preview.py
+-rw-rw-r--   0 david     (1001) david     (1001)     5398 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/recipes.py
+-rw-rw-r--   0 david     (1001) david     (1001)     1465 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/reverse_proxied.py
+-rw-rw-r--   0 david     (1001) david     (1001)      929 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/schema-mysql.sql
+-rw-rw-r--   0 david     (1001) david     (1001)      650 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/schema-sqlite3.sql
+drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-06-01 16:49:14.897283 hxl_proxy-2.0.1/hxl_proxy/static/
+drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-06-01 16:49:14.897283 hxl_proxy-2.0.1/hxl_proxy/static/bootstrap/
+drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-06-01 16:49:14.897283 hxl_proxy-2.0.1/hxl_proxy/static/bootstrap/css/
+-rw-rw-r--   0 david     (1001) david     (1001)    22608 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/bootstrap/css/bootstrap-theme.css
+-rw-rw-r--   0 david     (1001) david     (1001)    43339 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/bootstrap/css/bootstrap-theme.css.map
+-rw-rw-r--   0 david     (1001) david     (1001)    19963 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/bootstrap/css/bootstrap-theme.min.css
+-rw-rw-r--   0 david     (1001) david     (1001)   141414 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/bootstrap/css/bootstrap.css
+-rw-rw-r--   0 david     (1001) david     (1001)   379710 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/bootstrap/css/bootstrap.css.map
+-rw-rw-r--   0 david     (1001) david     (1001)   117150 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/bootstrap/css/bootstrap.min.css
+drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-06-01 16:49:14.897283 hxl_proxy-2.0.1/hxl_proxy/static/bootstrap/fonts/
+-rw-rw-r--   0 david     (1001) david     (1001)    20127 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/bootstrap/fonts/glyphicons-halflings-regular.eot
+-rw-rw-r--   0 david     (1001) david     (1001)   108738 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/bootstrap/fonts/glyphicons-halflings-regular.svg
+-rw-rw-r--   0 david     (1001) david     (1001)    45404 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/bootstrap/fonts/glyphicons-halflings-regular.ttf
+-rw-rw-r--   0 david     (1001) david     (1001)    23424 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/bootstrap/fonts/glyphicons-halflings-regular.woff
+-rw-rw-r--   0 david     (1001) david     (1001)    18028 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/bootstrap/fonts/glyphicons-halflings-regular.woff2
+drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-06-01 16:49:14.897283 hxl_proxy-2.0.1/hxl_proxy/static/bootstrap/js/
+-rw-rw-r--   0 david     (1001) david     (1001)    66732 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/bootstrap/js/bootstrap.js
+-rw-rw-r--   0 david     (1001) david     (1001)    35452 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/bootstrap/js/bootstrap.min.js
+-rw-rw-r--   0 david     (1001) david     (1001)      484 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/bootstrap/js/npm.js
+drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-06-01 16:49:14.897283 hxl_proxy-2.0.1/hxl_proxy/static/compat/
+-rw-rw-r--   0 david     (1001) david     (1001)     2636 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/compat/html5shiv.min.js
+-rw-rw-r--   0 david     (1001) david     (1001)      694 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/compat/ie10-viewport-bug-workaround.js
+-rw-rw-r--   0 david     (1001) david     (1001)     4377 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/compat/respond.min.js
+drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-06-01 16:49:14.897283 hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/
+-rw-rw-r--   0 david     (1001) david     (1001)     3470 2023-04-04 17:11:40.000000 hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/hxl-proxy.css
+-rw-rw-r--   0 david     (1001) david     (1001)    15879 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/hxl-proxy.js
+drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-06-01 16:49:14.897283 hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/
+-rw-rw-r--   0 david     (1001) david     (1001)     9448 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/android-icon-144x144.png
+-rw-rw-r--   0 david     (1001) david     (1001)    11645 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/android-icon-192x192.png
+-rw-rw-r--   0 david     (1001) david     (1001)     1960 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/android-icon-36x36.png
+-rw-rw-r--   0 david     (1001) david     (1001)     3057 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/android-icon-48x48.png
+-rw-rw-r--   0 david     (1001) david     (1001)     4171 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/android-icon-72x72.png
+-rw-rw-r--   0 david     (1001) david     (1001)     5857 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/android-icon-96x96.png
+-rw-rw-r--   0 david     (1001) david     (1001)     7317 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/apple-icon-114x114.png
+-rw-rw-r--   0 david     (1001) david     (1001)     7631 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/apple-icon-120x120.png
+-rw-rw-r--   0 david     (1001) david     (1001)     9448 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/apple-icon-144x144.png
+-rw-rw-r--   0 david     (1001) david     (1001)    10058 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/apple-icon-152x152.png
+-rw-rw-r--   0 david     (1001) david     (1001)    12668 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/apple-icon-180x180.png
+-rw-rw-r--   0 david     (1001) david     (1001)     2618 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/apple-icon-57x57.png
+-rw-rw-r--   0 david     (1001) david     (1001)     3820 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/apple-icon-60x60.png
+-rw-rw-r--   0 david     (1001) david     (1001)     4171 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/apple-icon-72x72.png
+-rw-rw-r--   0 david     (1001) david     (1001)     4491 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/apple-icon-76x76.png
+-rw-rw-r--   0 david     (1001) david     (1001)    12219 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/apple-icon-precomposed.png
+-rw-rw-r--   0 david     (1001) david     (1001)    12219 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/apple-icon.png
+-rw-rw-r--   0 david     (1001) david     (1001)      281 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/browserconfig.xml
+-rw-rw-r--   0 david     (1001) david     (1001)     1249 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/favicon-16x16.png
+-rw-rw-r--   0 david     (1001) david     (1001)     1899 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/favicon-32x32.png
+-rw-rw-r--   0 david     (1001) david     (1001)     5857 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/favicon-96x96.png
+-rw-rw-r--   0 david     (1001) david     (1001)     1150 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/favicon.ico
+-rw-rw-r--   0 david     (1001) david     (1001)     1165 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/manifest.json
+-rw-rw-r--   0 david     (1001) david     (1001)     9448 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/ms-icon-144x144.png
+-rw-rw-r--   0 david     (1001) david     (1001)    10073 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/ms-icon-150x150.png
+-rw-rw-r--   0 david     (1001) david     (1001)    27390 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/ms-icon-310x310.png
+-rw-rw-r--   0 david     (1001) david     (1001)     4125 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/ms-icon-70x70.png
+drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-06-01 16:49:14.901283 hxl_proxy-2.0.1/hxl_proxy/static/images/
+-rw-rw-r--   0 david     (1001) david     (1001)     8850 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/images/csv-icon.png
+-rw-rw-r--   0 david     (1001) david     (1001)    13225 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/images/dropbox-logo.png
+-rw-rw-r--   0 david     (1001) david     (1001)    22085 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/images/google-drive-logo.png
+-rw-rw-r--   0 david     (1001) david     (1001)     7767 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/images/hdx-logo.png
+-rw-rw-r--   0 david     (1001) david     (1001)     2454 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/images/hxl-logo-white.png
+-rw-rw-r--   0 david     (1001) david     (1001)    55429 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/images/json-icon.png
+drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-06-01 16:49:14.901283 hxl_proxy-2.0.1/hxl_proxy/static/jquery/
+-rw-rw-r--   0 david     (1001) david     (1001)   240427 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/jquery/jquery-ui.min.js
+-rw-rw-r--   0 david     (1001) david     (1001)    10469 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/jquery/jquery.csv.js
+-rw-rw-r--   0 david     (1001) david     (1001)    84320 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/jquery/jquery.js
+-rw-rw-r--   0 david     (1001) david     (1001)     1291 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/static/jquery/jquery.ui.touch-punch.min.js
+drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-06-01 16:49:14.901283 hxl_proxy-2.0.1/hxl_proxy/templates/
+-rw-rw-r--   0 david     (1001) david     (1001)     4570 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/templates/about.html
+-rw-rw-r--   0 david     (1001) david     (1001)     5224 2023-03-20 15:47:35.000000 hxl_proxy-2.0.1/hxl_proxy/templates/api-data-preview.html
+-rw-rw-r--   0 david     (1001) david     (1001)     4462 2023-03-20 15:47:35.000000 hxl_proxy-2.0.1/hxl_proxy/templates/api-from-spec.html
+-rw-rw-r--   0 david     (1001) david     (1001)     3506 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/templates/data-advanced.html
+-rw-rw-r--   0 david     (1001) david     (1001)     2227 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/templates/data-logs.html
+-rw-rw-r--   0 david     (1001) david     (1001)     9122 2023-04-04 17:11:40.000000 hxl_proxy-2.0.1/hxl_proxy/templates/data-recipe.html
+-rw-rw-r--   0 david     (1001) david     (1001)     5109 2023-03-20 15:47:35.000000 hxl_proxy-2.0.1/hxl_proxy/templates/data-source.html
+-rw-rw-r--   0 david     (1001) david     (1001)     6758 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/templates/data-tagger.html
+-rw-rw-r--   0 david     (1001) david     (1001)     2547 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/templates/data-view.html
+-rw-rw-r--   0 david     (1001) david     (1001)     1206 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/templates/error.html
+-rw-rw-r--   0 david     (1001) david     (1001)     1247 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/templates/hash.html
+-rw-rw-r--   0 david     (1001) david     (1001)     2672 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/templates/hxl-test.html
+drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-06-01 16:49:14.901283 hxl_proxy-2.0.1/hxl_proxy/templates/includes/
+-rw-rw-r--   0 david     (1001) david     (1001)      153 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/templates/includes/admin-alert.html
+-rw-rw-r--   0 david     (1001) david     (1001)      496 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/templates/includes/chooser-scripts.html
+-rw-rw-r--   0 david     (1001) david     (1001)      959 2023-03-20 15:47:35.000000 hxl_proxy-2.0.1/hxl_proxy/templates/includes/data-tabs.html
+drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-06-01 16:49:14.901283 hxl_proxy-2.0.1/hxl_proxy/templates/includes/filters/
+-rw-rw-r--   0 david     (1001) david     (1001)     1815 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/templates/includes/filters/add.html
+-rw-rw-r--   0 david     (1001) david     (1001)     1737 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/templates/includes/filters/append-list.html
+-rw-rw-r--   0 david     (1001) david     (1001)     2308 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/templates/includes/filters/append.html
+-rw-rw-r--   0 david     (1001) david     (1001)     5188 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/templates/includes/filters/clean.html
+-rw-rw-r--   0 david     (1001) david     (1001)     6021 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/templates/includes/filters/count.html
+-rw-rw-r--   0 david     (1001) david     (1001)     1510 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/templates/includes/filters/cut.html
+-rw-rw-r--   0 david     (1001) david     (1001)     1258 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/templates/includes/filters/dedup.html
+-rw-rw-r--   0 david     (1001) david     (1001)     2166 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/templates/includes/filters/expand.html
+-rw-rw-r--   0 david     (1001) david     (1001)     1344 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/templates/includes/filters/explode.html
+-rw-rw-r--   0 david     (1001) david     (1001)     1227 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/templates/includes/filters/fill.html
+-rw-rw-r--   0 david     (1001) david     (1001)      630 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/templates/includes/filters/filter-list.html
+-rw-rw-r--   0 david     (1001) david     (1001)      643 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/templates/includes/filters/filter-selector.html
+-rw-rw-r--   0 david     (1001) david     (1001)      691 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/templates/includes/filters/filter-types.j2
+-rw-rw-r--   0 david     (1001) david     (1001)     1191 2023-03-20 15:47:35.000000 hxl_proxy-2.0.1/hxl_proxy/templates/includes/filters/filter-variables.j2
+-rw-rw-r--   0 david     (1001) david     (1001)     1258 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/templates/includes/filters/implode.html
+-rw-rw-r--   0 david     (1001) david     (1001)     2051 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/templates/includes/filters/jsonpath.html
+-rw-rw-r--   0 david     (1001) david     (1001)      334 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/templates/includes/filters/label-field-multicol.html
+-rw-rw-r--   0 david     (1001) david     (1001)      324 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/templates/includes/filters/label-field.html
+-rw-rw-r--   0 david     (1001) david     (1001)     2480 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/templates/includes/filters/merge.html
+-rw-rw-r--   0 david     (1001) david     (1001)     1931 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/templates/includes/filters/rename.html
+-rw-rw-r--   0 david     (1001) david     (1001)     1311 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/templates/includes/filters/replace-map.html
+-rw-rw-r--   0 david     (1001) david     (1001)     2192 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/templates/includes/filters/replace.html
+-rw-rw-r--   0 david     (1001) david     (1001)     1240 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/templates/includes/filters/select.html
+-rw-rw-r--   0 david     (1001) david     (1001)      963 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/templates/includes/filters/sort.html
+-rw-rw-r--   0 david     (1001) david     (1001)     2317 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/templates/includes/headers.html
+-rw-rw-r--   0 david     (1001) david     (1001)      171 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/templates/includes/help.html
+-rw-rw-r--   0 david     (1001) david     (1001)      847 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/templates/includes/hxltable.html
+-rw-rw-r--   0 david     (1001) david     (1001)      259 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/templates/includes/messages.html
+-rw-rw-r--   0 david     (1001) david     (1001)      365 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/templates/includes/metadata-params.html
+-rw-rw-r--   0 david     (1001) david     (1001)     3378 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/templates/includes/navbar.html
+-rw-rw-r--   0 david     (1001) david     (1001)      153 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/templates/includes/params.html
+-rw-rw-r--   0 david     (1001) david     (1001)      790 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/templates/includes/postcards.html
+-rw-rw-r--   0 david     (1001) david     (1001)      142 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/templates/includes/recipe-form.html
+-rw-rw-r--   0 david     (1001) david     (1001)      412 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/templates/includes/recipe-params.html
+-rw-rw-r--   0 david     (1001) david     (1001)      443 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/templates/includes/scripts.html
+-rw-rw-r--   0 david     (1001) david     (1001)      368 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/templates/includes/selectors.html
+-rw-rw-r--   0 david     (1001) david     (1001)      182 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/templates/includes/source.html
+-rw-rw-r--   0 david     (1001) david     (1001)      382 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/templates/includes/tagger-params.html
+-rw-rw-r--   0 david     (1001) david     (1001)     1633 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/templates/settings-user.html
+-rw-rw-r--   0 david     (1001) david     (1001)     2433 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/templates/validate-issue.html
+-rw-rw-r--   0 david     (1001) david     (1001)     5437 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/templates/validate-summary.html
+-rw-rw-r--   0 david     (1001) david     (1001)    16476 2023-03-20 15:47:35.000000 hxl_proxy-2.0.1/hxl_proxy/util.py
+-rw-rw-r--   0 david     (1001) david     (1001)     3270 2022-10-28 23:21:23.000000 hxl_proxy-2.0.1/hxl_proxy/validate.py
+drwxrwxr-x   0 david     (1001) david     (1001)        0 2023-06-01 16:49:14.897283 hxl_proxy-2.0.1/hxl_proxy.egg-info/
+-rw-rw-r--   0 david     (1001) david     (1001)     3829 2023-06-01 16:49:14.000000 hxl_proxy-2.0.1/hxl_proxy.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1001) david     (1001)     5986 2023-06-01 16:49:14.000000 hxl_proxy-2.0.1/hxl_proxy.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1001) david     (1001)       64 2023-06-01 16:49:14.000000 hxl_proxy-2.0.1/hxl_proxy.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1001) david     (1001)      159 2023-06-01 16:49:14.000000 hxl_proxy-2.0.1/hxl_proxy.egg-info/requires.txt
+-rw-rw-r--   0 david     (1001) david     (1001)       10 2023-06-01 16:49:14.000000 hxl_proxy-2.0.1/hxl_proxy.egg-info/top_level.txt
+-rw-rw-r--   0 david     (1001) david     (1001)        1 2023-05-30 16:34:19.000000 hxl_proxy-2.0.1/hxl_proxy.egg-info/zip-safe
+-rw-rw-r--   0 david     (1001) david     (1001)     1160 2023-06-01 16:49:14.901283 hxl_proxy-2.0.1/setup.cfg
+-rwxrwxr-x   0 david     (1001) david     (1001)       69 2023-06-01 16:48:29.000000 hxl_proxy-2.0.1/setup.py
```

### Comparing `hxl-proxy-2.0/LICENSE.md` & `hxl_proxy-2.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/PKG-INFO` & `hxl_proxy-2.0.1/hxl_proxy.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 Metadata-Version: 2.1
 Name: hxl-proxy
-Version: 2.0
-Summary: Flask-based web proxy for HXL
-Home-page: https://github.com/HXLStandard/hxl-proxy
+Version: 2.0.1
+Summary: Flask-based web data proxy for the Humanitarian Exchange Language (HXL)
+Home-page: UNKNOWN
 Author: David Megginson
-Author-email: contact@megginson.com
-License: UNKNOWN
+Author-email: megginson@un.org
+License: Public Domain
+Project-URL: Documentation, https://github.com/HXLStandard/hxl-proxy/wiki
+Project-URL: GitHub, https://github.com/HXLStandard/hxl-proxy/
+Project-URL: Changelog, https://github.com/HXLStandard/hxl-proxy/blob/prod/CHANGELOG
+Keywords: data,hxl
 Platform: UNKNOWN
-Description-Content-Type: text/markdown
+Classifier: Framework :: Flask
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
 License-File: LICENSE.md
 
 hxl-proxy
 =========
 
 Python-/flask-based web proxy for transforming a HXL dataset
 dynamically. Requires Python3.
```

### Comparing `hxl-proxy-2.0/README.md` & `hxl_proxy-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/__init__.py` & `hxl_proxy-2.0.1/hxl_proxy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 January 2015
 
 License: Public Domain
 Documentation: http://hxlstandard.org
 
 """
 
-__version__="2.0"
+__version__="2.0.1"
 """Module version number
 See https://www.python.org/dev/peps/pep-0396/
 
 """
 
 #
 # Ignore nuisance warnings from flask_caching (for now)
```

### Comparing `hxl-proxy-2.0/hxl_proxy/admin.py` & `hxl_proxy-2.0.1/hxl_proxy/admin.py`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/auth.py` & `hxl_proxy-2.0.1/hxl_proxy/auth.py`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/caching.py` & `hxl_proxy-2.0.1/hxl_proxy/caching.py`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/controllers.py` & `hxl_proxy-2.0.1/hxl_proxy/controllers.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 """
 
 import hxl_proxy
 from hxl.input import HXLIOException
 
 from hxl_proxy import admin, app, auth, cache, caching, dao, exceptions, filters, pcodes, preview, recipes, util, validate
 
-import datetime, flask, hxl, io, json, logging, requests, requests_cache, signal, werkzeug, csv, urllib
+import datetime, flask, hxl, importlib, io, json, logging, requests, requests_cache, signal, werkzeug, csv, urllib
 
 from hxl.util import logup
 
 logger = logging.getLogger(__name__)
 """ Python logger for this module """
 
 from structlog import contextvars, get_logger, wrap_logger
@@ -88,15 +88,16 @@
         response.headers['Access-Control-Allow-Origin'] = '*'
         return response
     else:
         # Generic HTML error page
         return flask.render_template('error.html', e=e, category=type(e)), status
 
 # Register the general error handler UNLESS we're in debug mode
-app.register_error_handler(Exception, handle_default_exception)
+if not app.debug:
+    app.register_error_handler(Exception, handle_default_exception)
 
 
 def handle_redirect_exception(e):
     """ Error handler: catch a redirection exception
     Different parts of the code throw exceptions.RedirectException
     when they need the HXL Proxy to jump to a different page. This is especially
     important for workflow (e.g. if there's no URL, jump to /data/source)
@@ -201,19 +202,21 @@
 def about():
     """ Flask controller: show the about page
     Includes version information for major packages, so that
     we can tell easily what's deployed.
     """
     # include version information for these packages
     releases = {
-        'hxl-proxy': hxl_proxy.__version__,
-        'libhxl': hxl.__version__,
-        'flask': flask.__version__,
-        'requests': requests.__version__
+        'hxl_proxy': hxl_proxy.__version__,
     }
+    for package in ['libhxl', 'flask', 'flask-caching', 'redis', 'requests', 'requests_cache', 'structlog', 'urllib3',]:
+        try:
+            releases[package] = importlib.metadata.version(package)
+        except Exception as e:
+            releases[package] = str(e)
 
     # draw the web page
     return flask.render_template('about.html', releases=releases)
 
 
 
 ########################################################################
```

### Comparing `hxl-proxy-2.0/hxl_proxy/dao.py` & `hxl_proxy-2.0.1/hxl_proxy/dao.py`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/exceptions.py` & `hxl_proxy-2.0.1/hxl_proxy/exceptions.py`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/filters.py` & `hxl_proxy-2.0.1/hxl_proxy/filters.py`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/pcodes.py` & `hxl_proxy-2.0.1/hxl_proxy/pcodes.py`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/preview.py` & `hxl_proxy-2.0.1/hxl_proxy/preview.py`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/recipes.py` & `hxl_proxy-2.0.1/hxl_proxy/recipes.py`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/reverse_proxied.py` & `hxl_proxy-2.0.1/hxl_proxy/reverse_proxied.py`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/schema-mysql.sql` & `hxl_proxy-2.0.1/hxl_proxy/schema-mysql.sql`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/schema-sqlite3.sql` & `hxl_proxy-2.0.1/hxl_proxy/schema-sqlite3.sql`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/bootstrap/css/bootstrap-theme.css` & `hxl_proxy-2.0.1/hxl_proxy/static/bootstrap/css/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/bootstrap/css/bootstrap-theme.css.map` & `hxl_proxy-2.0.1/hxl_proxy/static/bootstrap/css/bootstrap-theme.css.map`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/bootstrap/css/bootstrap-theme.min.css` & `hxl_proxy-2.0.1/hxl_proxy/static/bootstrap/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/bootstrap/css/bootstrap.css` & `hxl_proxy-2.0.1/hxl_proxy/static/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/bootstrap/css/bootstrap.css.map` & `hxl_proxy-2.0.1/hxl_proxy/static/bootstrap/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/bootstrap/css/bootstrap.min.css` & `hxl_proxy-2.0.1/hxl_proxy/static/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/bootstrap/fonts/glyphicons-halflings-regular.eot` & `hxl_proxy-2.0.1/hxl_proxy/static/bootstrap/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/bootstrap/fonts/glyphicons-halflings-regular.svg` & `hxl_proxy-2.0.1/hxl_proxy/static/bootstrap/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/bootstrap/fonts/glyphicons-halflings-regular.ttf` & `hxl_proxy-2.0.1/hxl_proxy/static/bootstrap/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/bootstrap/fonts/glyphicons-halflings-regular.woff` & `hxl_proxy-2.0.1/hxl_proxy/static/bootstrap/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/bootstrap/fonts/glyphicons-halflings-regular.woff2` & `hxl_proxy-2.0.1/hxl_proxy/static/bootstrap/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/bootstrap/js/bootstrap.js` & `hxl_proxy-2.0.1/hxl_proxy/static/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/bootstrap/js/bootstrap.min.js` & `hxl_proxy-2.0.1/hxl_proxy/static/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/compat/html5shiv.min.js` & `hxl_proxy-2.0.1/hxl_proxy/static/compat/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/compat/ie10-viewport-bug-workaround.js` & `hxl_proxy-2.0.1/hxl_proxy/static/compat/ie10-viewport-bug-workaround.js`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/compat/respond.min.js` & `hxl_proxy-2.0.1/hxl_proxy/static/compat/respond.min.js`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/hxl-proxy.css` & `hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/hxl-proxy.css`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/hxl-proxy.js` & `hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/hxl-proxy.js`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/android-icon-144x144.png` & `hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/android-icon-144x144.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/android-icon-192x192.png` & `hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/android-icon-192x192.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/android-icon-36x36.png` & `hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/android-icon-36x36.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/android-icon-48x48.png` & `hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/android-icon-48x48.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/android-icon-72x72.png` & `hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/android-icon-72x72.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/android-icon-96x96.png` & `hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/android-icon-96x96.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/apple-icon-114x114.png` & `hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/apple-icon-114x114.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/apple-icon-120x120.png` & `hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/apple-icon-120x120.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/apple-icon-144x144.png` & `hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/apple-icon-144x144.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/apple-icon-152x152.png` & `hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/apple-icon-152x152.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/apple-icon-180x180.png` & `hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/apple-icon-180x180.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/apple-icon-57x57.png` & `hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/apple-icon-57x57.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/apple-icon-60x60.png` & `hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/apple-icon-60x60.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/apple-icon-72x72.png` & `hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/apple-icon-72x72.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/apple-icon-76x76.png` & `hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/apple-icon-76x76.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/apple-icon-precomposed.png` & `hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/apple-icon-precomposed.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/apple-icon.png` & `hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/apple-icon.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/favicon-16x16.png` & `hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/favicon-32x32.png` & `hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/favicon-96x96.png` & `hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/favicon.ico` & `hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/favicon.ico`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/manifest.json` & `hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/manifest.json`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/ms-icon-144x144.png` & `hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/ms-icon-144x144.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/ms-icon-150x150.png` & `hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/ms-icon-150x150.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/ms-icon-310x310.png` & `hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/ms-icon-310x310.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/hxl-proxy/icons/ms-icon-70x70.png` & `hxl_proxy-2.0.1/hxl_proxy/static/hxl-proxy/icons/ms-icon-70x70.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/images/csv-icon.png` & `hxl_proxy-2.0.1/hxl_proxy/static/images/csv-icon.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/images/dropbox-logo.png` & `hxl_proxy-2.0.1/hxl_proxy/static/images/dropbox-logo.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/images/google-drive-logo.png` & `hxl_proxy-2.0.1/hxl_proxy/static/images/google-drive-logo.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/images/hdx-logo.png` & `hxl_proxy-2.0.1/hxl_proxy/static/images/hdx-logo.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/images/hxl-logo-white.png` & `hxl_proxy-2.0.1/hxl_proxy/static/images/hxl-logo-white.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/images/json-icon.png` & `hxl_proxy-2.0.1/hxl_proxy/static/images/json-icon.png`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/jquery/jquery-ui.min.js` & `hxl_proxy-2.0.1/hxl_proxy/static/jquery/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/jquery/jquery.csv.js` & `hxl_proxy-2.0.1/hxl_proxy/static/jquery/jquery.csv.js`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/jquery/jquery.js` & `hxl_proxy-2.0.1/hxl_proxy/static/jquery/jquery.js`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/static/jquery/jquery.ui.touch-punch.min.js` & `hxl_proxy-2.0.1/hxl_proxy/static/jquery/jquery.ui.touch-punch.min.js`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/templates/about.html` & `hxl_proxy-2.0.1/hxl_proxy/templates/about.html`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/templates/api-data-preview.html` & `hxl_proxy-2.0.1/hxl_proxy/templates/api-data-preview.html`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/templates/api-from-spec.html` & `hxl_proxy-2.0.1/hxl_proxy/templates/api-from-spec.html`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/templates/data-advanced.html` & `hxl_proxy-2.0.1/hxl_proxy/templates/data-advanced.html`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/templates/data-logs.html` & `hxl_proxy-2.0.1/hxl_proxy/templates/data-logs.html`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/templates/data-recipe.html` & `hxl_proxy-2.0.1/hxl_proxy/templates/data-recipe.html`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/templates/data-source.html` & `hxl_proxy-2.0.1/hxl_proxy/templates/data-source.html`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/templates/data-tagger.html` & `hxl_proxy-2.0.1/hxl_proxy/templates/data-tagger.html`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/templates/data-view.html` & `hxl_proxy-2.0.1/hxl_proxy/templates/data-view.html`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/templates/error.html` & `hxl_proxy-2.0.1/hxl_proxy/templates/error.html`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/templates/hash.html` & `hxl_proxy-2.0.1/hxl_proxy/templates/hash.html`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/templates/hxl-test.html` & `hxl_proxy-2.0.1/hxl_proxy/templates/hxl-test.html`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/templates/includes/data-tabs.html` & `hxl_proxy-2.0.1/hxl_proxy/templates/includes/data-tabs.html`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/templates/includes/filters/add.html` & `hxl_proxy-2.0.1/hxl_proxy/templates/includes/filters/add.html`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/templates/includes/filters/append-list.html` & `hxl_proxy-2.0.1/hxl_proxy/templates/includes/filters/append-list.html`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/templates/includes/filters/append.html` & `hxl_proxy-2.0.1/hxl_proxy/templates/includes/filters/append.html`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/templates/includes/filters/clean.html` & `hxl_proxy-2.0.1/hxl_proxy/templates/includes/filters/clean.html`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/templates/includes/filters/count.html` & `hxl_proxy-2.0.1/hxl_proxy/templates/includes/filters/count.html`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/templates/includes/filters/cut.html` & `hxl_proxy-2.0.1/hxl_proxy/templates/includes/filters/cut.html`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/templates/includes/filters/dedup.html` & `hxl_proxy-2.0.1/hxl_proxy/templates/includes/filters/dedup.html`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/templates/includes/filters/expand.html` & `hxl_proxy-2.0.1/hxl_proxy/templates/includes/filters/expand.html`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/templates/includes/filters/explode.html` & `hxl_proxy-2.0.1/hxl_proxy/templates/includes/filters/explode.html`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/templates/includes/filters/fill.html` & `hxl_proxy-2.0.1/hxl_proxy/templates/includes/filters/fill.html`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/templates/includes/filters/filter-list.html` & `hxl_proxy-2.0.1/hxl_proxy/templates/includes/filters/filter-list.html`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/templates/includes/filters/filter-selector.html` & `hxl_proxy-2.0.1/hxl_proxy/templates/includes/filters/filter-selector.html`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/templates/includes/filters/filter-types.j2` & `hxl_proxy-2.0.1/hxl_proxy/templates/includes/filters/filter-types.j2`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/templates/includes/filters/filter-variables.j2` & `hxl_proxy-2.0.1/hxl_proxy/templates/includes/filters/filter-variables.j2`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/templates/includes/filters/implode.html` & `hxl_proxy-2.0.1/hxl_proxy/templates/includes/filters/implode.html`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/templates/includes/filters/jsonpath.html` & `hxl_proxy-2.0.1/hxl_proxy/templates/includes/filters/jsonpath.html`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/templates/includes/filters/merge.html` & `hxl_proxy-2.0.1/hxl_proxy/templates/includes/filters/merge.html`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/templates/includes/filters/rename.html` & `hxl_proxy-2.0.1/hxl_proxy/templates/includes/filters/rename.html`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/templates/includes/filters/replace-map.html` & `hxl_proxy-2.0.1/hxl_proxy/templates/includes/filters/replace-map.html`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/templates/includes/filters/replace.html` & `hxl_proxy-2.0.1/hxl_proxy/templates/includes/filters/replace.html`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/templates/includes/filters/select.html` & `hxl_proxy-2.0.1/hxl_proxy/templates/includes/filters/select.html`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/templates/includes/filters/sort.html` & `hxl_proxy-2.0.1/hxl_proxy/templates/includes/filters/sort.html`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/templates/includes/headers.html` & `hxl_proxy-2.0.1/hxl_proxy/templates/includes/headers.html`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/templates/includes/hxltable.html` & `hxl_proxy-2.0.1/hxl_proxy/templates/includes/hxltable.html`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/templates/includes/navbar.html` & `hxl_proxy-2.0.1/hxl_proxy/templates/includes/navbar.html`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/templates/includes/postcards.html` & `hxl_proxy-2.0.1/hxl_proxy/templates/includes/postcards.html`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/templates/settings-user.html` & `hxl_proxy-2.0.1/hxl_proxy/templates/settings-user.html`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/templates/validate-issue.html` & `hxl_proxy-2.0.1/hxl_proxy/templates/validate-issue.html`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/templates/validate-summary.html` & `hxl_proxy-2.0.1/hxl_proxy/templates/validate-summary.html`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/util.py` & `hxl_proxy-2.0.1/hxl_proxy/util.py`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy/validate.py` & `hxl_proxy-2.0.1/hxl_proxy/validate.py`

 * *Files identical despite different names*

### Comparing `hxl-proxy-2.0/hxl_proxy.egg-info/PKG-INFO` & `hxl_proxy-2.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 Metadata-Version: 2.1
-Name: hxl-proxy
-Version: 2.0
-Summary: Flask-based web proxy for HXL
-Home-page: https://github.com/HXLStandard/hxl-proxy
+Name: hxl_proxy
+Version: 2.0.1
+Summary: Flask-based web data proxy for the Humanitarian Exchange Language (HXL)
+Home-page: UNKNOWN
 Author: David Megginson
-Author-email: contact@megginson.com
-License: UNKNOWN
+Author-email: megginson@un.org
+License: Public Domain
+Project-URL: Documentation, https://github.com/HXLStandard/hxl-proxy/wiki
+Project-URL: GitHub, https://github.com/HXLStandard/hxl-proxy/
+Project-URL: Changelog, https://github.com/HXLStandard/hxl-proxy/blob/prod/CHANGELOG
+Keywords: data,hxl
 Platform: UNKNOWN
-Description-Content-Type: text/markdown
+Classifier: Framework :: Flask
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
 License-File: LICENSE.md
 
 hxl-proxy
 =========
 
 Python-/flask-based web proxy for transforming a HXL dataset
 dynamically. Requires Python3.
```

### Comparing `hxl-proxy-2.0/hxl_proxy.egg-info/SOURCES.txt` & `hxl_proxy-2.0.1/hxl_proxy.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE.md
 MANIFEST.in
 README.md
+setup.cfg
 setup.py
 hxl_proxy/__init__.py
 hxl_proxy/admin.py
 hxl_proxy/auth.py
 hxl_proxy/caching.py
 hxl_proxy/controllers.py
 hxl_proxy/dao.py
@@ -18,17 +19,17 @@
 hxl_proxy/schema-mysql.sql
 hxl_proxy/schema-sqlite3.sql
 hxl_proxy/util.py
 hxl_proxy/validate.py
 hxl_proxy.egg-info/PKG-INFO
 hxl_proxy.egg-info/SOURCES.txt
 hxl_proxy.egg-info/dependency_links.txt
-hxl_proxy.egg-info/not-zip-safe
 hxl_proxy.egg-info/requires.txt
 hxl_proxy.egg-info/top_level.txt
+hxl_proxy.egg-info/zip-safe
 hxl_proxy/static/bootstrap/css/bootstrap-theme.css
 hxl_proxy/static/bootstrap/css/bootstrap-theme.css.map
 hxl_proxy/static/bootstrap/css/bootstrap-theme.min.css
 hxl_proxy/static/bootstrap/css/bootstrap.css
 hxl_proxy/static/bootstrap/css/bootstrap.css.map
 hxl_proxy/static/bootstrap/css/bootstrap.min.css
 hxl_proxy/static/bootstrap/fonts/glyphicons-halflings-regular.eot
```

