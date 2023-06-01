# Comparing `tmp/pollination-apps-0.7.2.tar.gz` & `tmp/pollination-apps-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pollination-apps-0.7.2.tar", last modified: Mon May  8 19:13:08 2023, max compression
+gzip compressed data, was "dist/pollination-apps-0.8.0.tar", last modified: Thu Jun  1 00:44:11 2023, max compression
```

## Comparing `pollination-apps-0.7.2.tar` & `pollination-apps-0.8.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:13:08.000000 pollination-apps-0.7.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:13:08.000000 pollination-apps-0.7.2/.dependabot/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/.dependabot/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:13:08.000000 pollination-apps-0.7.2/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:13:08.000000 pollination-apps-0.7.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:13:08.000000 pollination-apps-0.7.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-08 19:13:08.000000 pollination-apps-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:13:08.000000 pollination-apps-0.7.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/docs/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/docs/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7136 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/docs/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:13:08.000000 pollination-apps-0.7.2/pollination_apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/pollination_apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:13:08.000000 pollination-apps-0.7.2/pollination_apps/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     8352 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/pollination_apps/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:13:08.000000 pollination-apps-0.7.2/pollination_apps/cli/assets/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/pollination_apps/cli/assets/art.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/pollination_apps/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/pollination_apps/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/pollination_apps/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/pollination_apps/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/pollination_apps/login.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:13:08.000000 pollination-apps-0.7.2/pollination_apps/template/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/pollination_apps/template/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:13:08.000000 pollination-apps-0.7.2/pollination_apps/template/assets/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/pollination_apps/template/assets/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:13:08.000000 pollination-apps-0.7.2/pollination_apps/template/assets/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/pollination_apps/template/assets/hooks/post_gen_project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:13:08.000000 pollination-apps-0.7.2/pollination_apps/template/assets/{{cookiecutter.app_slug}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:13:08.000000 pollination-apps-0.7.2/pollination_apps/template/assets/{{cookiecutter.app_slug}}/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:13:08.000000 pollination-apps-0.7.2/pollination_apps/template/assets/{{cookiecutter.app_slug}}/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/pollination_apps/template/assets/{{cookiecutter.app_slug}}/.github/workflows/ci-automated.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/pollination_apps/template/assets/{{cookiecutter.app_slug}}/.github/workflows/ci-manual.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/pollination_apps/template/assets/{{cookiecutter.app_slug}}/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/pollination_apps/template/assets/{{cookiecutter.app_slug}}/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/pollination_apps/template/assets/{{cookiecutter.app_slug}}/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:13:08.000000 pollination-apps-0.7.2/pollination_apps/template/assets/{{cookiecutter.app_slug}}/app/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:13:08.000000 pollination-apps-0.7.2/pollination_apps/template/assets/{{cookiecutter.app_slug}}/app/.pollination/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/pollination_apps/template/assets/{{cookiecutter.app_slug}}/app/.pollination/config.ini
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/pollination_apps/template/assets/{{cookiecutter.app_slug}}/app/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/pollination_apps/template/assets/{{cookiecutter.app_slug}}/app/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/pollination_apps/template/assets/{{cookiecutter.app_slug}}/app/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/pollination_apps/template/assets/{{cookiecutter.app_slug}}/app/vtk.Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:13:08.000000 pollination-apps-0.7.2/pollination_apps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-08 19:13:07.000000 pollination-apps-0.7.2/pollination_apps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-08 19:13:08.000000 pollination-apps-0.7.2/pollination_apps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 19:13:07.000000 pollination-apps-0.7.2/pollination_apps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-08 19:13:07.000000 pollination-apps-0.7.2/pollination_apps.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-08 19:13:07.000000 pollination-apps-0.7.2/pollination_apps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-08 19:13:07.000000 pollination-apps-0.7.2/pollination_apps.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-08 19:13:08.000000 pollination-apps-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:13:08.000000 pollination-apps-0.7.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-08 19:11:53.000000 pollination-apps-0.7.2/tests/test_true.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:44:11.000000 pollination-apps-0.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:44:11.000000 pollination-apps-0.8.0/.dependabot/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-01 00:42:44.000000 pollination-apps-0.8.0/.dependabot/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:44:11.000000 pollination-apps-0.8.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-01 00:42:44.000000 pollination-apps-0.8.0/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-01 00:42:44.000000 pollination-apps-0.8.0/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:44:11.000000 pollination-apps-0.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:44:11.000000 pollination-apps-0.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-06-01 00:42:44.000000 pollination-apps-0.8.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-01 00:42:44.000000 pollination-apps-0.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-01 00:42:44.000000 pollination-apps-0.8.0/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-01 00:42:44.000000 pollination-apps-0.8.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-01 00:42:44.000000 pollination-apps-0.8.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-01 00:42:44.000000 pollination-apps-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-01 00:44:11.000000 pollination-apps-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-01 00:42:44.000000 pollination-apps-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-01 00:42:44.000000 pollination-apps-0.8.0/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-01 00:42:44.000000 pollination-apps-0.8.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:44:11.000000 pollination-apps-0.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 00:42:44.000000 pollination-apps-0.8.0/docs/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-01 00:42:44.000000 pollination-apps-0.8.0/docs/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-01 00:42:44.000000 pollination-apps-0.8.0/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7136 2023-06-01 00:42:44.000000 pollination-apps-0.8.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-01 00:42:44.000000 pollination-apps-0.8.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-01 00:42:44.000000 pollination-apps-0.8.0/docs/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:44:11.000000 pollination-apps-0.8.0/pollination_apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 00:42:44.000000 pollination-apps-0.8.0/pollination_apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:44:11.000000 pollination-apps-0.8.0/pollination_apps/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     8700 2023-06-01 00:42:44.000000 pollination-apps-0.8.0/pollination_apps/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:44:11.000000 pollination-apps-0.8.0/pollination_apps/cli/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-01 00:42:44.000000 pollination-apps-0.8.0/pollination_apps/cli/assets/art.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-01 00:42:44.000000 pollination-apps-0.8.0/pollination_apps/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-06-01 00:42:44.000000 pollination-apps-0.8.0/pollination_apps/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-01 00:42:44.000000 pollination-apps-0.8.0/pollination_apps/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-01 00:42:44.000000 pollination-apps-0.8.0/pollination_apps/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-01 00:42:44.000000 pollination-apps-0.8.0/pollination_apps/login.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:44:11.000000 pollination-apps-0.8.0/pollination_apps/template/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-01 00:42:44.000000 pollination-apps-0.8.0/pollination_apps/template/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:44:11.000000 pollination-apps-0.8.0/pollination_apps/template/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-01 00:42:44.000000 pollination-apps-0.8.0/pollination_apps/template/assets/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:44:11.000000 pollination-apps-0.8.0/pollination_apps/template/assets/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-01 00:42:44.000000 pollination-apps-0.8.0/pollination_apps/template/assets/hooks/post_gen_project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:44:11.000000 pollination-apps-0.8.0/pollination_apps/template/assets/{{cookiecutter.app_slug}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:44:11.000000 pollination-apps-0.8.0/pollination_apps/template/assets/{{cookiecutter.app_slug}}/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:44:11.000000 pollination-apps-0.8.0/pollination_apps/template/assets/{{cookiecutter.app_slug}}/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-06-01 00:42:44.000000 pollination-apps-0.8.0/pollination_apps/template/assets/{{cookiecutter.app_slug}}/.github/workflows/ci-automated.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-01 00:42:44.000000 pollination-apps-0.8.0/pollination_apps/template/assets/{{cookiecutter.app_slug}}/.github/workflows/ci-manual.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-01 00:42:44.000000 pollination-apps-0.8.0/pollination_apps/template/assets/{{cookiecutter.app_slug}}/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-01 00:42:44.000000 pollination-apps-0.8.0/pollination_apps/template/assets/{{cookiecutter.app_slug}}/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-06-01 00:42:44.000000 pollination-apps-0.8.0/pollination_apps/template/assets/{{cookiecutter.app_slug}}/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:44:11.000000 pollination-apps-0.8.0/pollination_apps/template/assets/{{cookiecutter.app_slug}}/app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:44:11.000000 pollination-apps-0.8.0/pollination_apps/template/assets/{{cookiecutter.app_slug}}/app/.pollination/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-01 00:42:44.000000 pollination-apps-0.8.0/pollination_apps/template/assets/{{cookiecutter.app_slug}}/app/.pollination/config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-01 00:42:44.000000 pollination-apps-0.8.0/pollination_apps/template/assets/{{cookiecutter.app_slug}}/app/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-01 00:42:44.000000 pollination-apps-0.8.0/pollination_apps/template/assets/{{cookiecutter.app_slug}}/app/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-01 00:42:44.000000 pollination-apps-0.8.0/pollination_apps/template/assets/{{cookiecutter.app_slug}}/app/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-01 00:42:44.000000 pollination-apps-0.8.0/pollination_apps/template/assets/{{cookiecutter.app_slug}}/app/vtk.Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:44:11.000000 pollination-apps-0.8.0/pollination_apps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-01 00:44:11.000000 pollination-apps-0.8.0/pollination_apps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-01 00:44:11.000000 pollination-apps-0.8.0/pollination_apps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 00:44:11.000000 pollination-apps-0.8.0/pollination_apps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-01 00:44:11.000000 pollination-apps-0.8.0/pollination_apps.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-01 00:44:11.000000 pollination-apps-0.8.0/pollination_apps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-01 00:44:11.000000 pollination-apps-0.8.0/pollination_apps.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-01 00:42:44.000000 pollination-apps-0.8.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-01 00:44:11.000000 pollination-apps-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-01 00:42:44.000000 pollination-apps-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:44:11.000000 pollination-apps-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 00:42:44.000000 pollination-apps-0.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 00:42:44.000000 pollination-apps-0.8.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-01 00:42:44.000000 pollination-apps-0.8.0/tests/test_true.py
```

### Comparing `pollination-apps-0.7.2/.devcontainer/Dockerfile` & `pollination-apps-0.8.0/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `pollination-apps-0.7.2/.devcontainer/devcontainer.json` & `pollination-apps-0.8.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `pollination-apps-0.7.2/.github/workflows/ci.yaml` & `pollination-apps-0.8.0/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pollination-apps-0.7.2/LICENSE` & `pollination-apps-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pollination-apps-0.7.2/PKG-INFO` & `pollination-apps-0.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-apps
-Version: 0.7.2
+Version: 0.8.0
 Summary: A library to setup and deploy Apps to Pollination!
 Home-page: https://github.com/pollination/pollination-apps
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: MIT
 Description: # Pollination Apps
```

### Comparing `pollination-apps-0.7.2/README.md` & `pollination-apps-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `pollination-apps-0.7.2/docs/conf.py` & `pollination-apps-0.8.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pollination-apps-0.7.2/pollination_apps/cli/__init__.py` & `pollination-apps-0.8.0/pollination_apps/cli/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,32 +62,39 @@
 
 @main.command('deploy')
 @click.argument('path', type=click.Path(exists=True))
 @click.option('-o', '--owner', help='the owner of the app on pollination.')
 @click.option('-n', '--name', help='the name of the app.')
 @click.option('-t', '--tag', help='the tag for this version of the app')
 @click.option(
-    '-m', '--message', help='the commit message for this version of the app', show_default=True,
+    '-m', '--message', help='the commit message for this version of the app', 
+    show_default=True,
     default='A new version of the app.'
 )
 @click.option(
     '-e', '--environment', help='the pollination environment',
     type=click.Choice(['staging', 'production']),
     default='production', show_default=True
 )
 @click.option(
     '--public/--private', help='Indicate if the application should be created as '
     'a public or a private resource. This option does not change the visibility of a '
     'resource if it already exist.', is_flag=True, default=True, show_default=True
 )
 @click.option(
+    '--custom-entrypoint', help='Indicate that the entry point module '
+    ' of the application is named something other than "app.py".',
+    is_flag=True, default=False, show_default=True
+)
+@click.option(
     '-at', '--api-token', type=str, help='A valid Pollination API token', default=None,
     show_default=True
 )
-def deploy(path, owner, name, tag, message, environment, public, api_token):
+def deploy(path, owner, name, tag, message, environment, public, custom_entrypoint, 
+           api_token):
     """Deploy a new version of the application.
 
     \b
     Args:
         path: Full path to apps folder.
     """
 
@@ -104,15 +111,21 @@
 
     client = ctx.client
     env = Environment.from_string(environment)
     client.set_host(env.api_host)
 
     path = Path(path).absolute()
 
-    for required_file in ('Dockerfile', 'app.py'):
+
+    required_files = ['Dockerfile', 'app.py']
+
+    if custom_entrypoint:
+        required_files = ['Dockerfile']
+
+    for required_file in required_files:
         if not path.joinpath(required_file).is_file():
             raise ClickException(
                 f'Application folder is missing a required file: {required_file}'
             )
 
     owner, name, slug = _read_config(path, owner, name)
     slug = slug or _slugify(name)
```

### Comparing `pollination-apps-0.7.2/pollination_apps/cli/assets/art.txt` & `pollination-apps-0.8.0/pollination_apps/cli/assets/art.txt`

 * *Files identical despite different names*

### Comparing `pollination-apps-0.7.2/pollination_apps/cli/context.py` & `pollination-apps-0.8.0/pollination_apps/cli/context.py`

 * *Files identical despite different names*

### Comparing `pollination-apps-0.7.2/pollination_apps/client.py` & `pollination-apps-0.8.0/pollination_apps/client.py`

 * *Files identical despite different names*

### Comparing `pollination-apps-0.7.2/pollination_apps/config.py` & `pollination-apps-0.8.0/pollination_apps/config.py`

 * *Files identical despite different names*

### Comparing `pollination-apps-0.7.2/pollination_apps/env.py` & `pollination-apps-0.8.0/pollination_apps/env.py`

 * *Files identical despite different names*

### Comparing `pollination-apps-0.7.2/pollination_apps/login.py` & `pollination-apps-0.8.0/pollination_apps/login.py`

 * *Files identical despite different names*

### Comparing `pollination-apps-0.7.2/pollination_apps/template/assets/hooks/post_gen_project.py` & `pollination-apps-0.8.0/pollination_apps/template/assets/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `pollination-apps-0.7.2/pollination_apps/template/assets/{{cookiecutter.app_slug}}/.github/workflows/ci-automated.yaml` & `pollination-apps-0.8.0/pollination_apps/template/assets/{{cookiecutter.app_slug}}/.github/workflows/ci-automated.yaml`

 * *Files identical despite different names*

### Comparing `pollination-apps-0.7.2/pollination_apps/template/assets/{{cookiecutter.app_slug}}/.github/workflows/ci-manual.yaml` & `pollination-apps-0.8.0/pollination_apps/template/assets/{{cookiecutter.app_slug}}/.github/workflows/ci-manual.yaml`

 * *Files identical despite different names*

### Comparing `pollination-apps-0.7.2/pollination_apps/template/assets/{{cookiecutter.app_slug}}/README.md` & `pollination-apps-0.8.0/pollination_apps/template/assets/{{cookiecutter.app_slug}}/README.md`

 * *Files identical despite different names*

### Comparing `pollination-apps-0.7.2/pollination_apps.egg-info/PKG-INFO` & `pollination-apps-0.8.0/pollination_apps.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-apps
-Version: 0.7.2
+Version: 0.8.0
 Summary: A library to setup and deploy Apps to Pollination!
 Home-page: https://github.com/pollination/pollination-apps
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: MIT
 Description: # Pollination Apps
```

### Comparing `pollination-apps-0.7.2/pollination_apps.egg-info/SOURCES.txt` & `pollination-apps-0.8.0/pollination_apps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pollination-apps-0.7.2/setup.py` & `pollination-apps-0.8.0/setup.py`

 * *Files identical despite different names*

