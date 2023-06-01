# Comparing `tmp/ryantam626_jupyterlab_vim-0.13.3.tar.gz` & `tmp/ryantam626_jupyterlab_vim-0.16.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ryantam626_jupyterlab_vim-0.13.3.tar", last modified: Sat Mar  6 21:51:41 2021, max compression
+gzip compressed data, was "ryantam626_jupyterlab_vim-0.16.0.tar", last modified: Thu Jun  1 16:22:23 2023, max compression
```

## Comparing `ryantam626_jupyterlab_vim-0.13.3.tar` & `ryantam626_jupyterlab_vim-0.16.0.tar`

### file list

```diff
@@ -1,23 +1,37 @@
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2021-03-06 21:51:41.178732 ryantam626_jupyterlab_vim-0.13.3/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     1069 2021-01-06 11:34:39.688118 ryantam626_jupyterlab_vim-0.13.3/LICENSE
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      824 2021-03-06 21:51:41.178732 ryantam626_jupyterlab_vim-0.13.3/PKG-INFO
--rw-rw-r--   0 ryan      (1000) ryan      (1000)       84 2021-01-06 11:35:44.868415 ryantam626_jupyterlab_vim-0.13.3/README.md
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      189 2021-01-06 11:34:39.688118 ryantam626_jupyterlab_vim-0.13.3/install.json
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2021-03-06 21:51:41.178732 ryantam626_jupyterlab_vim-0.13.3/jupyterlab_vim/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      326 2021-01-06 11:34:39.688118 ryantam626_jupyterlab_vim-0.13.3/jupyterlab_vim/__init__.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      459 2021-01-06 11:34:39.692118 ryantam626_jupyterlab_vim-0.13.3/jupyterlab_vim/_version.py
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2021-03-06 21:51:41.178732 ryantam626_jupyterlab_vim-0.13.3/jupyterlab_vim/labextension/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     2576 2021-03-06 21:51:40.590730 ryantam626_jupyterlab_vim-0.13.3/jupyterlab_vim/labextension/package.json
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2021-03-06 21:51:41.178732 ryantam626_jupyterlab_vim-0.13.3/jupyterlab_vim/labextension/static/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)    12418 2021-03-06 21:51:40.586730 ryantam626_jupyterlab_vim-0.13.3/jupyterlab_vim/labextension/static/568.77f14860c14d333f240e.js
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     6224 2021-03-06 21:51:40.586730 ryantam626_jupyterlab_vim-0.13.3/jupyterlab_vim/labextension/static/remoteEntry.8a4d529403fef9ea25e1.js
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      118 2021-03-06 21:51:39.898727 ryantam626_jupyterlab_vim-0.13.3/jupyterlab_vim/labextension/static/style.js
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     2460 2021-03-06 21:50:53.978541 ryantam626_jupyterlab_vim-0.13.3/package.json
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      153 2021-01-06 11:34:39.692118 ryantam626_jupyterlab_vim-0.13.3/pyproject.toml
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     2254 2021-03-06 21:50:37.010473 ryantam626_jupyterlab_vim-0.13.3/setup.py
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2021-03-06 21:51:41.178732 ryantam626_jupyterlab_vim-0.13.3/src/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)    23695 2021-01-06 11:35:03.656228 ryantam626_jupyterlab_vim-0.13.3/src/index.ts
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2021-03-06 21:51:41.178732 ryantam626_jupyterlab_vim-0.13.3/style/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)        0 2021-01-06 11:34:39.692118 ryantam626_jupyterlab_vim-0.13.3/style/index.css
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      555 2021-01-06 11:34:39.692118 ryantam626_jupyterlab_vim-0.13.3/tsconfig.json
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     3103 2021-01-06 11:34:39.692118 ryantam626_jupyterlab_vim-0.13.3/tslint.json
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-06-01 16:22:23.490469 ryantam626_jupyterlab_vim-0.16.0/
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1069 2023-06-01 14:12:55.000000 ryantam626_jupyterlab_vim-0.16.0/LICENSE
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      413 2023-06-01 14:12:55.000000 ryantam626_jupyterlab_vim-0.16.0/MANIFEST.in
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1088 2023-06-01 16:22:23.490469 ryantam626_jupyterlab_vim-0.16.0/PKG-INFO
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)       93 2023-06-01 16:00:47.000000 ryantam626_jupyterlab_vim-0.16.0/README.md
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      189 2023-06-01 14:12:55.000000 ryantam626_jupyterlab_vim-0.16.0/install.json
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-06-01 16:22:23.486469 ryantam626_jupyterlab_vim-0.16.0/jupyterlab_vim/
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      319 2023-06-01 14:12:55.000000 ryantam626_jupyterlab_vim-0.16.0/jupyterlab_vim/__init__.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      440 2023-06-01 14:12:55.000000 ryantam626_jupyterlab_vim-0.16.0/jupyterlab_vim/_version.py
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-06-01 16:22:23.486469 ryantam626_jupyterlab_vim-0.16.0/jupyterlab_vim/labextension/
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     2640 2023-06-01 15:29:47.000000 ryantam626_jupyterlab_vim-0.16.0/jupyterlab_vim/labextension/package.json
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-06-01 16:22:23.486469 ryantam626_jupyterlab_vim-0.16.0/jupyterlab_vim/labextension/schemas/
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-06-01 16:22:23.486469 ryantam626_jupyterlab_vim-0.16.0/jupyterlab_vim/labextension/schemas/@axlair/
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-06-01 16:22:23.486469 ryantam626_jupyterlab_vim-0.16.0/jupyterlab_vim/labextension/schemas/@axlair/jupyterlab_vim/
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     2640 2023-06-01 15:29:47.000000 ryantam626_jupyterlab_vim-0.16.0/jupyterlab_vim/labextension/schemas/@axlair/jupyterlab_vim/package.json.orig
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)    10940 2023-06-01 15:29:47.000000 ryantam626_jupyterlab_vim-0.16.0/jupyterlab_vim/labextension/schemas/@axlair/jupyterlab_vim/plugin.json
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-06-01 16:22:23.486469 ryantam626_jupyterlab_vim-0.16.0/jupyterlab_vim/labextension/static/
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      165 2023-06-01 15:29:47.000000 ryantam626_jupyterlab_vim-0.16.0/jupyterlab_vim/labextension/static/style.js
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     2616 2023-06-01 16:00:47.000000 ryantam626_jupyterlab_vim-0.16.0/package.json
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      591 2023-06-01 14:12:55.000000 ryantam626_jupyterlab_vim-0.16.0/pyproject.toml
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-06-01 16:22:23.486469 ryantam626_jupyterlab_vim-0.16.0/ryantam626_jupyterlab_vim.egg-info/
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1088 2023-06-01 16:22:23.000000 ryantam626_jupyterlab_vim-0.16.0/ryantam626_jupyterlab_vim.egg-info/PKG-INFO
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      723 2023-06-01 16:22:23.000000 ryantam626_jupyterlab_vim-0.16.0/ryantam626_jupyterlab_vim.egg-info/SOURCES.txt
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)        1 2023-06-01 16:22:23.000000 ryantam626_jupyterlab_vim-0.16.0/ryantam626_jupyterlab_vim.egg-info/dependency_links.txt
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)        1 2023-06-01 16:22:23.000000 ryantam626_jupyterlab_vim-0.16.0/ryantam626_jupyterlab_vim.egg-info/not-zip-safe
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)       15 2023-06-01 16:22:23.000000 ryantam626_jupyterlab_vim-0.16.0/ryantam626_jupyterlab_vim.egg-info/top_level.txt
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)       38 2023-06-01 16:22:23.490469 ryantam626_jupyterlab_vim-0.16.0/setup.cfg
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     2710 2023-06-01 16:00:47.000000 ryantam626_jupyterlab_vim-0.16.0/setup.py
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-06-01 16:22:23.490469 ryantam626_jupyterlab_vim-0.16.0/src/
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     9510 2023-06-01 14:12:55.000000 ryantam626_jupyterlab_vim-0.16.0/src/codemirrorCommands.ts
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     3842 2023-06-01 14:12:55.000000 ryantam626_jupyterlab_vim-0.16.0/src/index.ts
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)    12229 2023-06-01 16:00:47.000000 ryantam626_jupyterlab_vim-0.16.0/src/labCommands.ts
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-06-01 16:22:23.490469 ryantam626_jupyterlab_vim-0.16.0/style/
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)        0 2023-06-01 14:12:55.000000 ryantam626_jupyterlab_vim-0.16.0/style/index.css
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)        0 2023-06-01 14:12:55.000000 ryantam626_jupyterlab_vim-0.16.0/style/index.js
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      554 2023-06-01 14:12:55.000000 ryantam626_jupyterlab_vim-0.16.0/tsconfig.json
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)   191574 2023-06-01 14:58:00.000000 ryantam626_jupyterlab_vim-0.16.0/yarn.lock
```

### Comparing `ryantam626_jupyterlab_vim-0.13.3/LICENSE` & `ryantam626_jupyterlab_vim-0.16.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ryantam626_jupyterlab_vim-0.13.3/jupyterlab_vim/labextension/package.json` & `ryantam626_jupyterlab_vim-0.16.0/package.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8121323529411765%*

 * *Differences: {"'bugs'": "{'url': 'https://github.com/ryantam626/jupyterlab-vim/issues'}",*

 * * "'dependencies'": "{'@jupyterlab/settingregistry': '^3.0.0-rc.13', delete: ['@types/codemirror']}",*

 * * "'devDependencies'": "{'@typescript-eslint/eslint-plugin': '^4.8.1', '@typescript-eslint/parser': "*

 * *                      "'^4.8.1', 'eslint': '^7.14.0', 'eslint-config-prettier': '^6.15.0', "*

 * *                      "'eslint-plugin-prettier': '^3.1.4', 'prettier': '^2.1.1', 'typescript': "*

 * *                      "'~4.1.3', '@types/co […]*

```diff
@@ -1,77 +1,78 @@
 {
     "author": "Axel Fahy",
     "bugs": {
-        "url": "https://github.com/axelfahy/jupyterlab-vim/issues"
+        "url": "https://github.com/ryantam626/jupyterlab-vim/issues"
     },
     "dependencies": {
         "@jupyterlab/application": "^3.0.0-rc.13",
         "@jupyterlab/cells": "^3.0.0-rc.13",
         "@jupyterlab/codemirror": "^3.0.0-rc.13",
         "@jupyterlab/notebook": "^3.0.0-rc.13",
+        "@jupyterlab/settingregistry": "^3.0.0-rc.13",
         "@lumino/commands": "^1.12.0",
         "@lumino/coreutils": "^1.5.3",
         "@lumino/domutils": "^1.2.3",
-        "@types/codemirror": "^0.0.87",
         "react": "^17.0.1"
     },
     "description": "Code cell vim bindings",
     "devDependencies": {
         "@jupyterlab/builder": "^3.0.0-rc.2",
-        "@typescript-eslint/eslint-plugin": "^2.27.0",
-        "@typescript-eslint/parser": "^2.27.0",
-        "eslint": "^7.5.0",
-        "eslint-config-prettier": "^6.10.1",
-        "eslint-plugin-prettier": "^3.1.2",
+        "@types/codemirror": "^0.0.87",
+        "@typescript-eslint/eslint-plugin": "^4.8.1",
+        "@typescript-eslint/parser": "^4.8.1",
+        "eslint": "^7.14.0",
+        "eslint-config-prettier": "^6.15.0",
+        "eslint-plugin-prettier": "^3.1.4",
         "npm-run-all": "^4.1.5",
-        "prettier": "^1.19.0",
+        "prettier": "^2.1.1",
         "rimraf": "^3.0.2",
         "tslint": "^6.1.2",
-        "typescript": "~4.0.3"
+        "typescript": "~4.1.3"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
-        "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
+        "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
+        "schema/**/*.{json,}",
+        "style/index.js"
     ],
-    "homepage": "https://github.com/axelfahy/jupyterlab-vim",
+    "homepage": "https://github.com/ryantam626/jupyterlab-vim",
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.8a4d529403fef9ea25e1.js"
-        },
         "extension": true,
-        "outputDir": "jupyterlab_vim/labextension"
+        "outputDir": "jupyterlab_vim/labextension",
+        "schemaDir": "schema"
     },
     "keywords": [
         "extension",
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
     ],
     "license": "MIT",
     "main": "lib/index.js",
     "name": "@axlair/jupyterlab_vim",
     "repository": {
         "type": "git",
-        "url": "https://github.com/axelfahy/jupyterlab-vim.git"
+        "url": "https://github.com/ryantam626/jupyterlab-vim.git"
     },
     "scripts": {
         "build": "jlpm run build:lib && jlpm run build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:lib": "tsc",
-        "build:prod": "jlpm run build:lib && jlpm run build:labextension",
+        "build:prod": "jlpm run clean && jlpm run build:lib && jlpm run build:labextension",
         "clean": "jlpm run clean:lib",
         "clean:all": "jlpm run clean:lib && jlpm run clean:labextension",
         "clean:labextension": "rimraf jupyterlab_vim/labextension",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
         "eslint": "eslint . --ext .ts,.tsx --fix",
         "eslint:check": "eslint . --ext .ts,.tsx",
-        "install:extension": "jupyter labextension develop --overwrite .",
+        "install:extension": "jlpm run build",
         "prepare": "jlpm run clean && jlpm run build:prod",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
+    "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.13.3"
+    "version": "0.16.0"
 }
```

### Comparing `ryantam626_jupyterlab_vim-0.13.3/package.json` & `ryantam626_jupyterlab_vim-0.16.0/jupyterlab_vim/labextension/package.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8170343137254903%*

 * *Differences: {"'bugs'": "{'url': 'https://github.com/jupyterlab-contrib/jupyterlab-vim/issues'}",*

 * * "'dependencies'": "{'@jupyterlab/settingregistry': '^3.0.0-rc.13', delete: ['@types/codemirror']}",*

 * * "'devDependencies'": "{'@typescript-eslint/eslint-plugin': '^4.8.1', '@typescript-eslint/parser': "*

 * *                      "'^4.8.1', 'eslint': '^7.14.0', 'eslint-config-prettier': '^6.15.0', "*

 * *                      "'eslint-plugin-prettier': '^3.1.4', 'prettier': '^2.1.1', 'typescript': "*

 * *                      "'~4.1.3', '@ […]*

```diff
@@ -1,73 +1,78 @@
 {
     "author": "Axel Fahy",
     "bugs": {
-        "url": "https://github.com/axelfahy/jupyterlab-vim/issues"
+        "url": "https://github.com/jupyterlab-contrib/jupyterlab-vim/issues"
     },
     "dependencies": {
         "@jupyterlab/application": "^3.0.0-rc.13",
         "@jupyterlab/cells": "^3.0.0-rc.13",
         "@jupyterlab/codemirror": "^3.0.0-rc.13",
         "@jupyterlab/notebook": "^3.0.0-rc.13",
+        "@jupyterlab/settingregistry": "^3.0.0-rc.13",
         "@lumino/commands": "^1.12.0",
         "@lumino/coreutils": "^1.5.3",
         "@lumino/domutils": "^1.2.3",
-        "@types/codemirror": "^0.0.87",
         "react": "^17.0.1"
     },
     "description": "Code cell vim bindings",
     "devDependencies": {
         "@jupyterlab/builder": "^3.0.0-rc.2",
-        "@typescript-eslint/eslint-plugin": "^2.27.0",
-        "@typescript-eslint/parser": "^2.27.0",
-        "eslint": "^7.5.0",
-        "eslint-config-prettier": "^6.10.1",
-        "eslint-plugin-prettier": "^3.1.2",
+        "@types/codemirror": "^0.0.87",
+        "@typescript-eslint/eslint-plugin": "^4.8.1",
+        "@typescript-eslint/parser": "^4.8.1",
+        "eslint": "^7.14.0",
+        "eslint-config-prettier": "^6.15.0",
+        "eslint-plugin-prettier": "^3.1.4",
         "npm-run-all": "^4.1.5",
-        "prettier": "^1.19.0",
+        "prettier": "^2.1.1",
         "rimraf": "^3.0.2",
         "tslint": "^6.1.2",
-        "typescript": "~4.0.3"
+        "typescript": "~4.1.3"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
-        "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
+        "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
+        "schema/**/*.{json,}",
+        "style/index.js"
     ],
-    "homepage": "https://github.com/axelfahy/jupyterlab-vim",
+    "homepage": "https://github.com/jupyterlab-contrib/jupyterlab-vim",
     "jupyterlab": {
         "extension": true,
-        "outputDir": "jupyterlab_vim/labextension"
+        "outputDir": "jupyterlab_vim/labextension",
+        "schemaDir": "schema"
     },
     "keywords": [
         "extension",
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
     ],
     "license": "MIT",
     "main": "lib/index.js",
     "name": "@axlair/jupyterlab_vim",
     "repository": {
         "type": "git",
-        "url": "https://github.com/axelfahy/jupyterlab-vim.git"
+        "url": "https://github.com/jupyterlab-contrib/jupyterlab-vim.git"
     },
     "scripts": {
         "build": "jlpm run build:lib && jlpm run build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:lib": "tsc",
-        "build:prod": "jlpm run build:lib && jlpm run build:labextension",
+        "build:prod": "jlpm run clean && jlpm run build:lib && jlpm run build:labextension",
         "clean": "jlpm run clean:lib",
         "clean:all": "jlpm run clean:lib && jlpm run clean:labextension",
         "clean:labextension": "rimraf jupyterlab_vim/labextension",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
         "eslint": "eslint . --ext .ts,.tsx --fix",
         "eslint:check": "eslint . --ext .ts,.tsx",
-        "install:extension": "jupyter labextension develop --overwrite .",
+        "install:extension": "jlpm run build",
         "prepare": "jlpm run clean && jlpm run build:prod",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
+    "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.13.3"
+    "version": "0.16.0"
 }
```

### Comparing `ryantam626_jupyterlab_vim-0.13.3/tsconfig.json` & `ryantam626_jupyterlab_vim-0.16.0/tsconfig.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.993421052631579%*

 * *Differences: {"'compilerOptions'": "{'strictNullChecks': True}"}*

```diff
@@ -12,15 +12,15 @@
         "noImplicitAny": true,
         "noUnusedLocals": true,
         "outDir": "lib",
         "preserveWatchOutput": true,
         "resolveJsonModule": true,
         "rootDir": "src",
         "strict": true,
-        "strictNullChecks": false,
+        "strictNullChecks": true,
         "target": "es2017",
         "types": []
     },
     "include": [
         "src/*"
     ]
 }
```

