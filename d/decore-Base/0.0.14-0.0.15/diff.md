# Comparing `tmp/decore_Base-0.0.14.tar.gz` & `tmp/decore_Base-0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decore_Base-0.0.14.tar", last modified: Wed May 31 12:31:49 2023, max compression
+gzip compressed data, was "decore_Base-0.0.15.tar", last modified: Thu Jun  1 12:53:01 2023, max compression
```

## Comparing `decore_Base-0.0.14.tar` & `decore_Base-0.0.15.tar`

### file list

```diff
@@ -1,159 +1,159 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.295996 decore_Base-0.0.14/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.251995 decore_Base-0.0.14/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-31 12:31:41.000000 decore_Base-0.0.14/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.251995 decore_Base-0.0.14/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-31 12:31:41.000000 decore_Base-0.0.14/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-31 12:31:41.000000 decore_Base-0.0.14/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.251995 decore_Base-0.0.14/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-31 12:31:41.000000 decore_Base-0.0.14/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-31 12:31:41.000000 decore_Base-0.0.14/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-31 12:31:41.000000 decore_Base-0.0.14/KOFI.md
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-31 12:31:41.000000 decore_Base-0.0.14/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-31 12:31:49.295996 decore_Base-0.0.14/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-05-31 12:31:41.000000 decore_Base-0.0.14/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-05-31 12:31:41.000000 decore_Base-0.0.14/README_DE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.255995 decore_Base-0.0.14/decore_Base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-31 12:31:49.000000 decore_Base-0.0.14/decore_Base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-05-31 12:31:49.000000 decore_Base-0.0.14/decore_Base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 12:31:49.000000 decore_Base-0.0.14/decore_Base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-31 12:31:49.000000 decore_Base-0.0.14/decore_Base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-31 12:31:49.000000 decore_Base-0.0.14/decore_Base.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.255995 decore_Base-0.0.14/decore_base/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.259995 decore_Base-0.0.14/decore_base/classes/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/classes/decore_action.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/classes/decore_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/classes/decore_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/classes/decore_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/classes/decore_element.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/classes/decore_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/classes/decore_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    15687 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/classes/decore_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/classes/decore_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/classes/decore_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/classes/decore_prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/classes/decore_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/classes/decore_return.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/classes/decore_translate.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/classes/decore_view.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/classes/decore_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    16843 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/decore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.259995 decore_Base-0.0.14/decore_base/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/docs/social_header.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.263995 decore_Base-0.0.14/decore_base/library/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/library/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.263995 decore_Base-0.0.14/decore_base/library/particl_market/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/library/particl_market/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10733 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/library/particl_market/particl_market.py
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/library/powershell.py
--rw-r--r--   0 runner    (1001) docker     (123)    90489 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/library/powershell2.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/library/return_value.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.263995 decore_Base-0.0.14/decore_base/library/roaster/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/library/roaster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/library/roaster/roaster_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12453 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/library/roaster/roaster_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/library/roaster/roaster_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.263995 decore_Base-0.0.14/decore_base/prepare/
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/prepare/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.263995 decore_Base-0.0.14/decore_base/prepare/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/prepare/.vscode/launch.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.243995 decore_Base-0.0.14/decore_base/prepare/spa/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.263995 decore_Base-0.0.14/decore_base/prepare/spa/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.267995 decore_Base-0.0.14/decore_base/prepare/spa/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/prepare/spa/static/css/912.77e6bcbe.css
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/prepare/spa/static/css/app.d398f07d.css
--rw-r--r--   0 runner    (1001) docker     (123)   466611 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/prepare/spa/static/css/vendor.14c9ac7a.css
--rw-r--r--   0 runner    (1001) docker     (123)    64483 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/prepare/spa/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.271995 decore_Base-0.0.14/decore_base/prepare/spa/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    20436 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/prepare/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20544 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20416 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20408 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20424 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20344 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/prepare/spa/static/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-r--r--   0 runner    (1001) docker     (123)   164912 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-r--r--   0 runner    (1001) docker     (123)   128360 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   465188 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff
--rw-r--r--   0 runner    (1001) docker     (123)   325244 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.271995 decore_Base-0.0.14/decore_base/prepare/spa/static/icons/
--rw-r--r--   0 runner    (1001) docker     (123)    12324 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/prepare/spa/static/icons/favicon-128x128.png
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/prepare/spa/static/icons/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/prepare/spa/static/icons/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     9643 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/prepare/spa/static/icons/favicon-96x96.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.275995 decore_Base-0.0.14/decore_base/prepare/spa/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/prepare/spa/static/js/65.940d9b80.js
--rw-r--r--   0 runner    (1001) docker     (123)    29907 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/prepare/spa/static/js/912.f638ed14.js
--rw-r--r--   0 runner    (1001) docker     (123)    18107 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/prepare/spa/static/js/app.465385a3.js
--rw-r--r--   0 runner    (1001) docker     (123)   380277 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/prepare/spa/static/js/vendor.03c46c80.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.275995 decore_Base-0.0.14/decore_base/prepare/spa/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/prepare/spa/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.275995 decore_Base-0.0.14/decore_base/sample/
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.275995 decore_Base-0.0.14/decore_base/sample/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.279996 decore_Base-0.0.14/decore_base/sample/bases/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/bases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/bases/account_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/bases/company_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/bases/global_management_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/bases/information_stytem_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/bases/person_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/bases/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/config.json
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/language.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.279996 decore_Base-0.0.14/decore_base/sample/models/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/models/account_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/models/company_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/models/person_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/models/test_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.247995 decore_Base-0.0.14/decore_base/sample/spa/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.279996 decore_Base-0.0.14/decore_base/sample/spa/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.279996 decore_Base-0.0.14/decore_base/sample/spa/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/spa/static/css/912.77e6bcbe.css
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/spa/static/css/app.d398f07d.css
--rw-r--r--   0 runner    (1001) docker     (123)   466611 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/spa/static/css/vendor.14c9ac7a.css
--rw-r--r--   0 runner    (1001) docker     (123)    64483 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/spa/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.287996 decore_Base-0.0.14/decore_base/sample/spa/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    20436 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20544 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20416 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20408 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20424 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20344 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/spa/static/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-r--r--   0 runner    (1001) docker     (123)   164912 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-r--r--   0 runner    (1001) docker     (123)   128360 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   465188 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff
--rw-r--r--   0 runner    (1001) docker     (123)   325244 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.287996 decore_Base-0.0.14/decore_base/sample/spa/static/icons/
--rw-r--r--   0 runner    (1001) docker     (123)    12324 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/spa/static/icons/favicon-128x128.png
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/spa/static/icons/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/spa/static/icons/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     9643 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/spa/static/icons/favicon-96x96.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.287996 decore_Base-0.0.14/decore_base/sample/spa/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/spa/static/js/65.940d9b80.js
--rw-r--r--   0 runner    (1001) docker     (123)    29907 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/spa/static/js/912.f638ed14.js
--rw-r--r--   0 runner    (1001) docker     (123)    18107 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/spa/static/js/app.465385a3.js
--rw-r--r--   0 runner    (1001) docker     (123)   380277 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/spa/static/js/vendor.03c46c80.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.291996 decore_Base-0.0.14/decore_base/sample/spa/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/spa/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.291996 decore_Base-0.0.14/decore_base/sample/state/
--rw-r--r--   0 runner    (1001) docker     (123)  1306624 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/state/database.db
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/state/keybase.kdbx
--rw-r--r--   0 runner    (1001) docker     (123)    16384 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/sample/state/querybase.db
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.295996 decore_Base-0.0.14/decore_base/uniform/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/uniform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/uniform/conform_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:31:49.295996 decore_Base-0.0.14/decore_base/uniform/depricated/
--rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/uniform/depricated/askform_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/uniform/depricated/buyform_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7613 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/uniform/depricated/conform_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/uniform/depricated/deform_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/uniform/perform_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/uniform/reform_client_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-31 12:31:41.000000 decore_Base-0.0.14/decore_base/uniform/reform_server_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-31 12:31:41.000000 decore_Base-0.0.14/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-31 12:31:41.000000 decore_Base-0.0.14/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-31 12:31:49.295996 decore_Base-0.0.14/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:53:01.715616 decore_Base-0.0.15/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:53:01.699615 decore_Base-0.0.15/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-01 12:52:53.000000 decore_Base-0.0.15/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:53:01.699615 decore_Base-0.0.15/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-01 12:52:53.000000 decore_Base-0.0.15/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-01 12:52:53.000000 decore_Base-0.0.15/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:53:01.699615 decore_Base-0.0.15/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-01 12:52:53.000000 decore_Base-0.0.15/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-01 12:52:53.000000 decore_Base-0.0.15/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-01 12:52:53.000000 decore_Base-0.0.15/KOFI.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-01 12:52:53.000000 decore_Base-0.0.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-01 12:53:01.715616 decore_Base-0.0.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-06-01 12:52:53.000000 decore_Base-0.0.15/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-06-01 12:52:53.000000 decore_Base-0.0.15/README_DE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:53:01.699615 decore_Base-0.0.15/decore_Base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-01 12:53:01.000000 decore_Base-0.0.15/decore_Base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-06-01 12:53:01.000000 decore_Base-0.0.15/decore_Base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 12:53:01.000000 decore_Base-0.0.15/decore_Base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-01 12:53:01.000000 decore_Base-0.0.15/decore_Base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-01 12:53:01.000000 decore_Base-0.0.15/decore_Base.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:53:01.699615 decore_Base-0.0.15/decore_base/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:53:01.699615 decore_Base-0.0.15/decore_base/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/classes/decore_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/classes/decore_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/classes/decore_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/classes/decore_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/classes/decore_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/classes/decore_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/classes/decore_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15687 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/classes/decore_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/classes/decore_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/classes/decore_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/classes/decore_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/classes/decore_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/classes/decore_return.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/classes/decore_translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/classes/decore_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/classes/decore_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17133 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/decore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:53:01.699615 decore_Base-0.0.15/decore_base/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/docs/social_header.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:53:01.699615 decore_Base-0.0.15/decore_base/library/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/library/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:53:01.703616 decore_Base-0.0.15/decore_base/library/particl_market/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/library/particl_market/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10733 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/library/particl_market/particl_market.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/library/powershell.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90489 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/library/powershell2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/library/return_value.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:53:01.703616 decore_Base-0.0.15/decore_base/library/roaster/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/library/roaster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/library/roaster/roaster_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12453 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/library/roaster/roaster_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/library/roaster/roaster_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:53:01.703616 decore_Base-0.0.15/decore_base/prepare/
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/prepare/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:53:01.703616 decore_Base-0.0.15/decore_base/prepare/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/prepare/.vscode/launch.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:53:01.695615 decore_Base-0.0.15/decore_base/prepare/spa/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:53:01.703616 decore_Base-0.0.15/decore_base/prepare/spa/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:53:01.703616 decore_Base-0.0.15/decore_base/prepare/spa/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/prepare/spa/static/css/912.77e6bcbe.css
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/prepare/spa/static/css/app.d398f07d.css
+-rw-r--r--   0 runner    (1001) docker     (123)   466611 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/prepare/spa/static/css/vendor.14c9ac7a.css
+-rw-r--r--   0 runner    (1001) docker     (123)    64483 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/prepare/spa/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:53:01.703616 decore_Base-0.0.15/decore_base/prepare/spa/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    20436 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/prepare/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20544 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20416 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20408 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20424 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20344 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/prepare/spa/static/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   164912 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   128360 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   465188 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   325244 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:53:01.707615 decore_Base-0.0.15/decore_base/prepare/spa/static/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)    12324 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/prepare/spa/static/icons/favicon-128x128.png
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/prepare/spa/static/icons/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/prepare/spa/static/icons/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9643 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/prepare/spa/static/icons/favicon-96x96.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:53:01.707615 decore_Base-0.0.15/decore_base/prepare/spa/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/prepare/spa/static/js/65.940d9b80.js
+-rw-r--r--   0 runner    (1001) docker     (123)    29907 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/prepare/spa/static/js/912.f638ed14.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18107 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/prepare/spa/static/js/app.465385a3.js
+-rw-r--r--   0 runner    (1001) docker     (123)   380277 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/prepare/spa/static/js/vendor.03c46c80.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:53:01.707615 decore_Base-0.0.15/decore_base/prepare/spa/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/prepare/spa/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:53:01.707615 decore_Base-0.0.15/decore_base/sample/
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/sample/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:53:01.707615 decore_Base-0.0.15/decore_base/sample/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/sample/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/sample/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/sample/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:53:01.707615 decore_Base-0.0.15/decore_base/sample/bases/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/sample/bases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/sample/bases/account_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/sample/bases/company_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/sample/bases/global_management_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/sample/bases/information_stytem_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/sample/bases/person_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/sample/bases/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/sample/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/sample/language.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:53:01.707615 decore_Base-0.0.15/decore_base/sample/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/sample/models/account_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/sample/models/company_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/sample/models/person_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/sample/models/test_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:53:01.695615 decore_Base-0.0.15/decore_base/sample/spa/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:53:01.707615 decore_Base-0.0.15/decore_base/sample/spa/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:53:01.707615 decore_Base-0.0.15/decore_base/sample/spa/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/sample/spa/static/css/912.77e6bcbe.css
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/sample/spa/static/css/app.d398f07d.css
+-rw-r--r--   0 runner    (1001) docker     (123)   466611 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/sample/spa/static/css/vendor.14c9ac7a.css
+-rw-r--r--   0 runner    (1001) docker     (123)    64483 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/sample/spa/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:53:01.711615 decore_Base-0.0.15/decore_base/sample/spa/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    20436 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/sample/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20544 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20416 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20408 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20424 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20344 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/sample/spa/static/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   164912 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/sample/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   128360 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/sample/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   465188 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/sample/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   325244 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/sample/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:53:01.711615 decore_Base-0.0.15/decore_base/sample/spa/static/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)    12324 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/sample/spa/static/icons/favicon-128x128.png
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/sample/spa/static/icons/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/sample/spa/static/icons/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9643 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/sample/spa/static/icons/favicon-96x96.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:53:01.711615 decore_Base-0.0.15/decore_base/sample/spa/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/sample/spa/static/js/65.940d9b80.js
+-rw-r--r--   0 runner    (1001) docker     (123)    29907 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/sample/spa/static/js/912.f638ed14.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18107 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/sample/spa/static/js/app.465385a3.js
+-rw-r--r--   0 runner    (1001) docker     (123)   380277 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/sample/spa/static/js/vendor.03c46c80.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:53:01.715616 decore_Base-0.0.15/decore_base/sample/spa/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/sample/spa/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:53:01.715616 decore_Base-0.0.15/decore_base/sample/state/
+-rw-r--r--   0 runner    (1001) docker     (123)  1306624 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/sample/state/database.db
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/sample/state/keybase.kdbx
+-rw-r--r--   0 runner    (1001) docker     (123)    16384 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/sample/state/querybase.db
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:53:01.715616 decore_Base-0.0.15/decore_base/uniform/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/uniform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/uniform/conform_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:53:01.715616 decore_Base-0.0.15/decore_base/uniform/depricated/
+-rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/uniform/depricated/askform_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/uniform/depricated/buyform_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7613 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/uniform/depricated/conform_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/uniform/depricated/deform_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/uniform/perform_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/uniform/reform_client_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-01 12:52:53.000000 decore_Base-0.0.15/decore_base/uniform/reform_server_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-01 12:52:53.000000 decore_Base-0.0.15/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-01 12:52:53.000000 decore_Base-0.0.15/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-01 12:53:01.715616 decore_Base-0.0.15/setup.cfg
```

### Comparing `decore_Base-0.0.14/.github/FUNDING.yml` & `decore_Base-0.0.15/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/.gitignore` & `decore_Base-0.0.15/.gitignore`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/.vscode/launch.json` & `decore_Base-0.0.15/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/KOFI.md` & `decore_Base-0.0.15/KOFI.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # decore Base | crafting UI simply
+decore Base is an out-of-the-box "Python to Vue.js" data application dashboard that helps you go from idea to view in a few simple steps. It is aimed at those who want to focus on the results of their algorithms , do scientific work, or perform teaching or learning functions.
 
 # decore Base | open source on github
-
 decore Base is now available on github. 
 
 Still very incomplete but to better visualize the running process I decided to publish the code on github.
 
 The documentation is not yet complete and will be expanded over time. 
 
 To install the sample application, please check the documentation, maybe there are already problems or ambiguities at this point.
@@ -26,8 +26,17 @@
 https://github.com/users/KemoPanzah/projects/1
 
 # decore Base | Twitter sponsoring
 In order to move my milestones forward with Twitter sponsorship, I desperately need support on Ko-fi.
 
 Twitter sponsorship helps me as a newbie to get a social reach.
 
-I hope to get feature requests or problem sets quickly to improve decore base.
+I hope to get feature requests or problem sets quickly to improve decore base.
+
+# decore Base | Release 0.0.14
+Main customization in this release is the improvement of the metafield for the back references.
+
+https://github.com/KemoPanzah/decore_Base/compare/0.0.13...0.0.14
+
+# decore Base | Application
+Here is a first image of the rendered sample application (0.0.14) with a table as the selected view.
+#Python #Vue #Dashboard
```

### Comparing `decore_Base-0.0.14/LICENSE` & `decore_Base-0.0.15/LICENSE`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/PKG-INFO` & `decore_Base-0.0.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decore_Base
-Version: 0.0.14
+Version: 0.0.15
 Summary: decore Base is a "Python to Vue.js" open source package that helps you go from idea to view in a few simple steps. It is targeted to those who want to focus on the results of their algorithms, do scientific work, perform promotional teaching or learning functions.
 Home-page: https://github.com/KemoPanzah/decore_Base
 Author: Kemo Panzah
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.9
```

### Comparing `decore_Base-0.0.14/README.md` & `decore_Base-0.0.15/README.md`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/README_DE.md` & `decore_Base-0.0.15/README_DE.md`

 * *Files 1% similar despite different names*

```diff
@@ -128,14 +128,15 @@
 #### PasswordField
 #### TextField
 
 ## Component processing
 ```mermaid
 graph
 A[Base] --> B[View]
+A --> Y[Function]
 B --> Z[Action]
 B --> C[Dialog]
 C --> D[Widget]
 D --> F[Sub Dialog]
 D --> G[Sub Widget]
 F --> G[Sub Widget]
 G --> Z[Action]
```

### Comparing `decore_Base-0.0.14/decore_Base.egg-info/PKG-INFO` & `decore_Base-0.0.15/decore_Base.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decore-Base
-Version: 0.0.14
+Version: 0.0.15
 Summary: decore Base is a "Python to Vue.js" open source package that helps you go from idea to view in a few simple steps. It is targeted to those who want to focus on the results of their algorithms, do scientific work, perform promotional teaching or learning functions.
 Home-page: https://github.com/KemoPanzah/decore_Base
 Author: Kemo Panzah
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.9
```

### Comparing `decore_Base-0.0.14/decore_Base.egg-info/SOURCES.txt` & `decore_Base-0.0.15/decore_Base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_Base.egg-info/requires.txt` & `decore_Base-0.0.15/decore_Base.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/classes/decore_base.py` & `decore_Base-0.0.15/decore_base/classes/decore_base.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/classes/decore_list.py` & `decore_Base-0.0.15/decore_base/classes/decore_list.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/classes/decore_model.py` & `decore_Base-0.0.15/decore_base/classes/decore_model.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/classes/decore_pool.py` & `decore_Base-0.0.15/decore_base/classes/decore_pool.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/classes/decore_prompt.py` & `decore_Base-0.0.15/decore_base/classes/decore_prompt.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,17 @@
                     '--add-data=spa;spa',
                     '--collect-data=pykeepass',
                     'app.py'
                 ])
             else:
                 pass
         else:
-            print ('Unknown arguments: ' + str(t_unknown_args))
+            print('Unknown arguments: ' + str(t_unknown_args) + ' Use --help for more information')
+            exit()
+
 
     def copy_launch(self):
         t_prepare_path = Path(__file__).parent.parent.joinpath('prepare')
         t_launch_source = t_prepare_path.joinpath('.vscode').joinpath('launch.json')
         t_launch_destination = Path('.vscode').joinpath('launch.json')
         t_launch_destination.parent.mkdir(parents=True, exist_ok=True)
         copyfile(str(t_launch_source.absolute()), str(t_launch_destination.absolute()))
```

### Comparing `decore_Base-0.0.14/decore_base/classes/decore_query.py` & `decore_Base-0.0.15/decore_base/classes/decore_query.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/classes/decore_return.py` & `decore_Base-0.0.15/decore_base/classes/decore_return.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/classes/decore_translate.py` & `decore_Base-0.0.15/decore_base/classes/decore_translate.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 from translate import Translator
 
 
 class Decore_translate(object):
     __source_language__ = 'en'
-    __output_language__ = 'de'
-    __trans_language_s__ = ['de']
+    __output_language__ = 'en'
+    __translate_language_s__ = ['de']
 
     __data__ = None
     __file_data__ = {}
 
     def __init__(self, p_string):
         self.load_data()
         self.id = p_string
@@ -18,17 +18,17 @@
             self.translate()
         self.save_data()
 
     def __str__(self):
         return self.__data__[self.id][self.__output_language__]
 
     def translate(self):
-        for trans_language in self.__trans_language_s__:
-            if not trans_language in self.__data__[self.id]:
-                self.__data__[self.id][trans_language] = Translator(from_lang=self.__source_language__, to_lang=trans_language).translate(self.id)
+        for language in self.__translate_language_s__:
+            if not language in self.__data__[self.id]:
+                self.__data__[self.id][language] = Translator(from_lang=self.__source_language__, to_lang=language).translate(self.id)
 
     @property
     def output(self):
         return self.__data__[self.id][self.__output_language__]
 
     @classmethod
     def load_data(cls):
```

### Comparing `decore_Base-0.0.14/decore_base/classes/decore_view.py` & `decore_Base-0.0.15/decore_base/classes/decore_view.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/decore.py` & `decore_Base-0.0.15/decore_base/decore.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from str2type import str2type
 from pathlib import Path
 from collections import OrderedDict
 
 
 class Decore(object):
     def __init__(self):
-        if not globals.flags.build_mode:
+        if not globals.flags.production_mode:
             self.prompt = Decore_prompt()
         self.pool = Decore_pool()
         self.api = self.get_api()
         Decore_query.create_table(safe=True)
         
     def get_api(self):
         t_static_folder = Path('spa/static')
@@ -91,25 +91,29 @@
                 i_base.start_inits()
                 i_base.start_worker()
             self.start_api()
         return wrapper
 
     def base(self, p_icon=None, p_title=None, p_desc=None, p_model=Decore_model):
         def wrapper(cls):
-            Base = type(cls.__name__, (cls, Decore_base), {})
-            t_base = Base()
-            t_base.id = cls.__name__
-            t_base.icon = p_icon
-            t_base.title = p_title
-            t_base.desc = p_desc
-            t_base.doc = cls.__doc__
-            t_base.model = p_model.register()
-            t_base.field_s = p_model.field_s
-            t_base.rel_field_s = p_model.rel_field_s
-            t_base.schema = p_model.build_schema()
+            class Base(cls, Decore_base):
+                def __init__(self):
+                    # cls.__init__(self)
+                    Decore_base.__init__(self)
+                    #TODO doppelt gemoppelte attribute aus decore_base oder decore_object entfernen
+                    self.id = cls.__name__
+                    self.icon = p_icon
+                    self.title = p_title
+                    self.desc = p_desc
+                    self.doc = cls.__doc__
+                    self.model = p_model.register()
+                    self.field_s = p_model.field_s
+                    self.rel_field_s = p_model.rel_field_s
+                    self.schema = p_model.build_schema()
+            t_base = type(cls.__name__, (Base,), {})()
             self.pool.register(t_base)
         return wrapper
 
     l_view_type = Literal['table']
     l_view_pag_type = Literal['client']
 
     def view(self, p_parent_id=None, p_icon=None, p_title=None, p_desc=None, p_type: l_view_type = 'table', p_active_s=[], p_filter_s=[], p_query={}, p_pag_type: l_view_pag_type = 'client', p_pag_recs=16):
```

### Comparing `decore_Base-0.0.14/decore_base/docs/social_header.txt` & `decore_Base-0.0.15/decore_base/docs/social_header.txt`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/globals.py` & `decore_Base-0.0.15/decore_base/globals.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 from uuid import uuid4
 import json,logging,sys
 
 logging.basicConfig(format='[%(levelname)s] | %(message)s', level=logging.INFO)
 
 class Global_flags(object):
     def __init__(self):
-        self.build_mode = self.set_build_mode()
+        self.production_mode = self.set_production_mode()
         self.dev_mode = False
         self.purge_unused_database_cols = False
     
-    def set_build_mode(self):
+    def set_production_mode(self):
         if getattr(sys, 'frozen', False) and hasattr(sys, '_MEIPASS'):
             return True
         else:
             return False
 
 class Global_config(object):
     def __init__(self):
```

### Comparing `decore_Base-0.0.14/decore_base/library/particl_market/particl_market.py` & `decore_Base-0.0.15/decore_base/library/particl_market/particl_market.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/library/powershell.py` & `decore_Base-0.0.15/decore_base/library/powershell.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/library/powershell2.py` & `decore_Base-0.0.15/decore_base/library/powershell2.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/library/return_value.py` & `decore_Base-0.0.15/decore_base/library/return_value.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/library/roaster/roaster_client.py` & `decore_Base-0.0.15/decore_base/library/roaster/roaster_client.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/library/roaster/roaster_functions.py` & `decore_Base-0.0.15/decore_base/library/roaster/roaster_functions.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/library/roaster/roaster_server.py` & `decore_Base-0.0.15/decore_base/library/roaster/roaster_server.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/prepare/.gitignore` & `decore_Base-0.0.15/decore_base/prepare/.gitignore`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/prepare/.vscode/launch.json` & `decore_Base-0.0.15/decore_base/prepare/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/prepare/spa/static/css/912.77e6bcbe.css` & `decore_Base-0.0.15/decore_base/prepare/spa/static/css/912.77e6bcbe.css`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/prepare/spa/static/css/app.d398f07d.css` & `decore_Base-0.0.15/decore_base/prepare/spa/static/css/app.d398f07d.css`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/prepare/spa/static/css/vendor.14c9ac7a.css` & `decore_Base-0.0.15/decore_base/prepare/spa/static/css/vendor.14c9ac7a.css`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/prepare/spa/static/favicon.ico` & `decore_Base-0.0.15/decore_base/prepare/spa/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/prepare/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `decore_Base-0.0.15/decore_base/prepare/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `decore_Base-0.0.15/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `decore_Base-0.0.15/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `decore_Base-0.0.15/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `decore_Base-0.0.15/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/prepare/spa/static/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `decore_Base-0.0.15/decore_base/prepare/spa/static/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `decore_Base-0.0.15/decore_base/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2` & `decore_Base-0.0.15/decore_base/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff` & `decore_Base-0.0.15/decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2` & `decore_Base-0.0.15/decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/prepare/spa/static/icons/favicon-128x128.png` & `decore_Base-0.0.15/decore_base/prepare/spa/static/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/prepare/spa/static/icons/favicon-16x16.png` & `decore_Base-0.0.15/decore_base/prepare/spa/static/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/prepare/spa/static/icons/favicon-32x32.png` & `decore_Base-0.0.15/decore_base/prepare/spa/static/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/prepare/spa/static/icons/favicon-96x96.png` & `decore_Base-0.0.15/decore_base/prepare/spa/static/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/prepare/spa/static/js/65.940d9b80.js` & `decore_Base-0.0.15/decore_base/prepare/spa/static/js/65.940d9b80.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/prepare/spa/static/js/912.f638ed14.js` & `decore_Base-0.0.15/decore_base/prepare/spa/static/js/912.f638ed14.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/prepare/spa/static/js/app.465385a3.js` & `decore_Base-0.0.15/decore_base/prepare/spa/static/js/app.465385a3.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/prepare/spa/static/js/vendor.03c46c80.js` & `decore_Base-0.0.15/decore_base/prepare/spa/static/js/vendor.03c46c80.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/prepare/spa/templates/index.html` & `decore_Base-0.0.15/decore_base/prepare/spa/templates/index.html`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/sample/.gitignore` & `decore_Base-0.0.15/decore_base/sample/.gitignore`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/sample/.vscode/launch.json` & `decore_Base-0.0.15/decore_base/sample/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/sample/bases/account_base.py` & `decore_Base-0.0.15/decore_base/sample/bases/account_base.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/sample/bases/company_base.py` & `decore_Base-0.0.15/decore_base/sample/bases/company_base.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/sample/bases/global_management_base.py` & `decore_Base-0.0.15/decore_base/sample/bases/global_management_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 from models.company_model import Company_model
 
 
 from mimesis import Person, Finance
 from random import randrange
 
 @decore.base(p_title='Global Management', p_icon='mdi-account-supervisor-circle-outline')
-class Global_management_base(object):
+class Global_management_base:
+    def __init__(self):
+        self.supertest = 'supertest'
     
     @decore.function(p_type='init')
     def query_tester(self):
         t_item_s = Person_model.query({'companies__title__eq':'NetApp'})
         pass
 
     @decore.function(p_type='init')
```

### Comparing `decore_Base-0.0.14/decore_base/sample/bases/person_base.py` & `decore_Base-0.0.15/decore_base/sample/bases/person_base.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/sample/bases/test_base.py` & `decore_Base-0.0.15/decore_base/sample/bases/test_base.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/sample/models/test_model.py` & `decore_Base-0.0.15/decore_base/sample/models/test_model.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/sample/spa/static/css/912.77e6bcbe.css` & `decore_Base-0.0.15/decore_base/sample/spa/static/css/912.77e6bcbe.css`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/sample/spa/static/css/app.d398f07d.css` & `decore_Base-0.0.15/decore_base/sample/spa/static/css/app.d398f07d.css`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/sample/spa/static/css/vendor.14c9ac7a.css` & `decore_Base-0.0.15/decore_base/sample/spa/static/css/vendor.14c9ac7a.css`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/sample/spa/static/favicon.ico` & `decore_Base-0.0.15/decore_base/sample/spa/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/sample/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `decore_Base-0.0.15/decore_base/sample/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `decore_Base-0.0.15/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `decore_Base-0.0.15/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `decore_Base-0.0.15/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `decore_Base-0.0.15/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/sample/spa/static/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `decore_Base-0.0.15/decore_base/sample/spa/static/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/sample/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `decore_Base-0.0.15/decore_base/sample/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/sample/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2` & `decore_Base-0.0.15/decore_base/sample/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/sample/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff` & `decore_Base-0.0.15/decore_base/sample/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/sample/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2` & `decore_Base-0.0.15/decore_base/sample/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/sample/spa/static/icons/favicon-128x128.png` & `decore_Base-0.0.15/decore_base/sample/spa/static/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/sample/spa/static/icons/favicon-16x16.png` & `decore_Base-0.0.15/decore_base/sample/spa/static/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/sample/spa/static/icons/favicon-32x32.png` & `decore_Base-0.0.15/decore_base/sample/spa/static/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/sample/spa/static/icons/favicon-96x96.png` & `decore_Base-0.0.15/decore_base/sample/spa/static/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/sample/spa/static/js/65.940d9b80.js` & `decore_Base-0.0.15/decore_base/sample/spa/static/js/65.940d9b80.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/sample/spa/static/js/912.f638ed14.js` & `decore_Base-0.0.15/decore_base/sample/spa/static/js/912.f638ed14.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/sample/spa/static/js/app.465385a3.js` & `decore_Base-0.0.15/decore_base/sample/spa/static/js/app.465385a3.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/sample/spa/static/js/vendor.03c46c80.js` & `decore_Base-0.0.15/decore_base/sample/spa/static/js/vendor.03c46c80.js`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/sample/spa/templates/index.html` & `decore_Base-0.0.15/decore_base/sample/spa/templates/index.html`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/sample/state/database.db` & `decore_Base-0.0.15/decore_base/sample/state/database.db`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/sample/state/keybase.kdbx` & `decore_Base-0.0.15/decore_base/sample/state/keybase.kdbx`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/sample/state/querybase.db` & `decore_Base-0.0.15/decore_base/sample/state/querybase.db`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/uniform/conform_model.py` & `decore_Base-0.0.15/decore_base/uniform/conform_model.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/uniform/depricated/askform_base.py` & `decore_Base-0.0.15/decore_base/uniform/depricated/askform_base.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/uniform/depricated/buyform_base.py` & `decore_Base-0.0.15/decore_base/uniform/depricated/buyform_base.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/uniform/depricated/conform_base.py` & `decore_Base-0.0.15/decore_base/uniform/depricated/conform_base.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/uniform/depricated/deform_base.py` & `decore_Base-0.0.15/decore_base/uniform/depricated/deform_base.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/uniform/perform_model.py` & `decore_Base-0.0.15/decore_base/uniform/perform_model.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/uniform/reform_client_model.py` & `decore_Base-0.0.15/decore_base/uniform/reform_client_model.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/decore_base/uniform/reform_server_model.py` & `decore_Base-0.0.15/decore_base/uniform/reform_server_model.py`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/requirements.txt` & `decore_Base-0.0.15/requirements.txt`

 * *Files identical despite different names*

### Comparing `decore_Base-0.0.14/setup.cfg` & `decore_Base-0.0.15/setup.cfg`

 * *Files identical despite different names*

