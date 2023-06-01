# Comparing `tmp/quetz-server-0.7.0.tar.gz` & `tmp/quetz-server-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quetz-server-0.7.0.tar", last modified: Tue Apr 11 08:48:50 2023, max compression
+gzip compressed data, was "quetz-server-0.8.0.tar", last modified: Thu Jun  1 07:34:21 2023, max compression
```

## Comparing `quetz-server-0.7.0.tar` & `quetz-server-0.8.0.tar`

### file list

```diff
@@ -1,216 +1,216 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.886885 quetz-server-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-11 08:48:34.000000 quetz-server-0.7.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-11 08:48:34.000000 quetz-server-0.7.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-11 08:48:34.000000 quetz-server-0.7.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-11 08:48:34.000000 quetz-server-0.7.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    19648 2023-04-11 08:48:41.000000 quetz-server-0.7.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-11 08:48:34.000000 quetz-server-0.7.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-11 08:48:34.000000 quetz-server-0.7.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-11 08:48:34.000000 quetz-server-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-11 08:48:34.000000 quetz-server-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17908 2023-04-11 08:48:50.886885 quetz-server-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-04-11 08:48:34.000000 quetz-server-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-11 08:48:34.000000 quetz-server-0.7.0/RELEASE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-11 08:48:34.000000 quetz-server-0.7.0/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-11 08:48:34.000000 quetz-server-0.7.0/dev_config.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.870885 quetz-server-0.7.0/docker/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docker/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docker/Dockerfile.jupyterhub
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docker/docker_config.toml
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docker/grafana.env
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docker/graphana_datasources.yml
--rw-r--r--   0 runner    (1001) docker     (123)    44096 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docker/jupyterhub_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docker/nginx.conf
--rw-r--r--   0 runner    (1001) docker     (123)    26521 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docker/postgres.conf
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docker/postgres.env
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docker/prometheus.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      272 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docker/wait-for-postgres.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.870885 quetz-server-0.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.870885 quetz-server-0.7.0/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    40864 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docs/assets/quetz_header.png
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.870885 quetz-server-0.7.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.870885 quetz-server-0.7.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docs/source/_static/quetz_favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    26122 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docs/source/_static/quetz_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.870885 quetz-server-0.7.0/docs/source/deploying/
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docs/source/deploying/authenticators.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9874 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docs/source/deploying/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docs/source/deploying/database.rst
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docs/source/deploying/frontend.rst
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docs/source/deploying/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docs/source/deploying/migrations.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docs/source/deploying/nginx.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docs/source/deploying/workers.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docs/source/plugins.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.870885 quetz-server-0.7.0/docs/source/qeps/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docs/source/qeps/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docs/source/qeps/qep-001-user-permissions.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.870885 quetz-server-0.7.0/docs/source/using/
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docs/source/using/basics.rst
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docs/source/using/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9431 2023-04-11 08:48:34.000000 quetz-server-0.7.0/docs/source/using/mirroring.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      255 2023-04-11 08:48:34.000000 quetz-server-0.7.0/download-test-package.sh
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-11 08:48:34.000000 quetz-server-0.7.0/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-11 08:48:34.000000 quetz-server-0.7.0/init_db.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-11 08:48:34.000000 quetz-server-0.7.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-11 08:48:39.000000 quetz-server-0.7.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.874884 quetz-server-0.7.0/quetz/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-11 08:48:39.000000 quetz-server-0.7.0/quetz/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.874884 quetz-server-0.7.0/quetz/authentication/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/authentication/auth_dao.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/authentication/azuread.py
--rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/authentication/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/authentication/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/authentication/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/authentication/google.py
--rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/authentication/jupyterhub.py
--rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/authentication/oauth2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/authentication/pam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/authentication/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/authorization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.874884 quetz-server-0.7.0/quetz/basic_frontend/
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/basic_frontend/avatar.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/basic_frontend/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/basic_frontend/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/channel_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    23731 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/condainfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    20035 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/config.toml
--rw-r--r--   0 runner    (1001) docker     (123)    42862 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/dao.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/database_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11299 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/db_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/deps.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.874884 quetz-server-0.7.0/quetz/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/jobs/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/jobs/dao.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/jobs/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/jobs/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/jobs/rest_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    12029 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/jobs/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    56922 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.878884 quetz-server-0.7.0/quetz/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/metrics/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/metrics/db_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/metrics/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/metrics/rest_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/metrics/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/metrics/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.878884 quetz-server-0.7.0/quetz/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/migrations/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/migrations/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.878884 quetz-server-0.7.0/quetz/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/migrations/versions/0653794b6252_adding_url_and_platforms_dirs.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/migrations/versions/0a0ab48887ab_adding_function_args_to_job_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/migrations/versions/30241b33d849_add_task_pending_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/migrations/versions/303ff70c27fc_configure_mirror_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/migrations/versions/3c3288034362_add_channel_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/migrations/versions/53f81aba78ce_use_biginteger_for_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/migrations/versions/794249a0b1bd_adding_jobs_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/migrations/versions/8d1e9a9e0b1f_adding_download_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/migrations/versions/8dfb7c4bfbd7_new_package_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/migrations/versions/98c04a65df4a_register_mirrors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/migrations/versions/a3ffa287d074_case_insensitive_channel_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     9084 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/migrations/versions/a80fb051a659_create_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/migrations/versions/b9886d9cadb0_create_indexes_for_download_count_.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/migrations/versions/cd404ed93cc0_add_per_channel_ttl.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/migrations/versions/cddba8e6e639_scheduling_spec_for_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/migrations/versions/d212023a8e0b_add_useremail_table_for_email_addresses.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/migrations/versions/db1c56bf4d57_add_channel_size_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/migrations/versions/ea6eba9a9ffc_merge_ebe550f9fbbe_and_b9886d9cadb0.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/migrations/versions/ebe550f9fbbe_added_create_at_and_expire_at_date_to_.py
--rw-r--r--   0 runner    (1001) docker     (123)    24546 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/pkgstores.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/repo_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8571 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/rest_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.882885 quetz-server-0.7.0/quetz/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tasks/assertions.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tasks/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tasks/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tasks/indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)    18320 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tasks/mirror.py
--rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tasks/reindexing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9671 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tasks/workers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.882885 quetz-server-0.7.0/quetz/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/templates/channeldata-index.html.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/templates/subdir-index.html.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.882885 quetz-server-0.7.0/quetz/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7159 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/testing/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/testing/mockups.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/testing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.882885 quetz-server-0.7.0/quetz/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.882885 quetz-server-0.7.0/quetz/tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/api/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/api/test_api_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)    22577 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/api/test_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/api/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    23467 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/api/test_main_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)     9173 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/api/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/api/test_users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.886885 quetz-server-0.7.0/quetz/tests/authentification/
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/authentification/test_auth_dao.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/authentification/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17757 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/authentification/test_oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/authentification/test_pam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.886885 quetz-server-0.7.0/quetz/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.866885 quetz-server-0.7.0/quetz/tests/data/dummy-plugin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.886885 quetz-server-0.7.0/quetz/tests/data/dummy-plugin/quetz_dummyplugin/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/data/dummy-plugin/quetz_dummyplugin/jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.886885 quetz-server-0.7.0/quetz/tests/data/dummy-plugin/quetz_dummyplugin-1.0-py3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/data/dummy-plugin/quetz_dummyplugin-1.0-py3.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/data/dummy-plugin/quetz_dummyplugin-1.0-py3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/data/other-package-0.1-0.tar.bz2
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/data/other-package-0.2-0.tar.bz2
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/data/test-package-0.1-0.tar.bz2
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/data/test-package-0.1-0_copy.tar.bz2
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/data/test-package-0.2-0.tar.bz2
--rw-r--r--   0 runner    (1001) docker     (123)    20798 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    18709 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13028 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/test_dao.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/test_db_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/test_health.py
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/test_indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)    27357 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)    38275 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/test_mirror.py
--rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/test_pkg_stores.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/test_versionorder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/tests/test_workers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8985 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11429 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz/versionorder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.886885 quetz-server-0.7.0/quetz_db_ext/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz_db_ext/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz_db_ext/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz_db_ext/LIBSOLV_LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14617 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz_db_ext/conda.c
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz_db_ext/conda.h
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz_db_ext/quetz_pg.c
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-11 08:48:34.000000 quetz-server-0.7.0/quetz_db_ext/quetz_sqlite.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:48:50.886885 quetz-server-0.7.0/quetz_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17908 2023-04-11 08:48:50.000000 quetz-server-0.7.0/quetz_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-04-11 08:48:50.000000 quetz-server-0.7.0/quetz_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:48:50.000000 quetz-server-0.7.0/quetz_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-11 08:48:50.000000 quetz-server-0.7.0/quetz_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-11 08:48:50.000000 quetz-server-0.7.0/quetz_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-11 08:48:50.000000 quetz-server-0.7.0/quetz_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-11 08:48:50.886885 quetz-server-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 08:48:34.000000 quetz-server-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.390586 quetz-server-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-01 07:34:02.000000 quetz-server-0.8.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-01 07:34:02.000000 quetz-server-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-01 07:34:02.000000 quetz-server-0.8.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    22389 2023-06-01 07:34:11.000000 quetz-server-0.8.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-01 07:34:02.000000 quetz-server-0.8.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-01 07:34:02.000000 quetz-server-0.8.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-01 07:34:02.000000 quetz-server-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-01 07:34:02.000000 quetz-server-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    18021 2023-06-01 07:34:21.390586 quetz-server-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17446 2023-06-01 07:34:02.000000 quetz-server-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-01 07:34:02.000000 quetz-server-0.8.0/RELEASE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-01 07:34:02.000000 quetz-server-0.8.0/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-01 07:34:02.000000 quetz-server-0.8.0/dev_config.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.370586 quetz-server-0.8.0/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docker/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docker/Dockerfile.jupyterhub
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docker/docker_config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docker/grafana.env
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docker/graphana_datasources.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    44096 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docker/jupyterhub_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docker/nginx.conf
+-rw-r--r--   0 runner    (1001) docker     (123)    26521 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docker/postgres.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docker/postgres.env
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docker/prometheus.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      272 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docker/wait-for-postgres.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.370586 quetz-server-0.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.370586 quetz-server-0.8.0/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    40864 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docs/assets/quetz_header.png
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.370586 quetz-server-0.8.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.370586 quetz-server-0.8.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docs/source/_static/quetz_favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    26122 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docs/source/_static/quetz_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.370586 quetz-server-0.8.0/docs/source/deploying/
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docs/source/deploying/authenticators.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docs/source/deploying/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docs/source/deploying/database.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docs/source/deploying/frontend.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docs/source/deploying/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docs/source/deploying/migrations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docs/source/deploying/nginx.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docs/source/deploying/workers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docs/source/plugins.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.374586 quetz-server-0.8.0/docs/source/qeps/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docs/source/qeps/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docs/source/qeps/qep-001-user-permissions.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.374586 quetz-server-0.8.0/docs/source/using/
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docs/source/using/basics.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docs/source/using/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9431 2023-06-01 07:34:02.000000 quetz-server-0.8.0/docs/source/using/mirroring.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      410 2023-06-01 07:34:02.000000 quetz-server-0.8.0/download-test-package.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-01 07:34:02.000000 quetz-server-0.8.0/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-06-01 07:34:02.000000 quetz-server-0.8.0/init_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-06-01 07:34:09.000000 quetz-server-0.8.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.374586 quetz-server-0.8.0/quetz/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-01 07:34:09.000000 quetz-server-0.8.0/quetz/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.378586 quetz-server-0.8.0/quetz/authentication/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/authentication/auth_dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/authentication/azuread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/authentication/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/authentication/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/authentication/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/authentication/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/authentication/jupyterhub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/authentication/oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/authentication/pam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/authentication/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/authorization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.378586 quetz-server-0.8.0/quetz/basic_frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/basic_frontend/avatar.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/basic_frontend/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/basic_frontend/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/channel_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23996 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/condainfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20496 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    42862 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/database_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11299 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/db_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/deps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.378586 quetz-server-0.8.0/quetz/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/jobs/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/jobs/dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/jobs/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/jobs/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/jobs/rest_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12029 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/jobs/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57621 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.378586 quetz-server-0.8.0/quetz/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/metrics/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/metrics/db_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/metrics/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/metrics/rest_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/metrics/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/metrics/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.378586 quetz-server-0.8.0/quetz/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/migrations/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/migrations/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.382586 quetz-server-0.8.0/quetz/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/migrations/versions/0653794b6252_adding_url_and_platforms_dirs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/migrations/versions/0a0ab48887ab_adding_function_args_to_job_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/migrations/versions/30241b33d849_add_task_pending_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/migrations/versions/303ff70c27fc_configure_mirror_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/migrations/versions/3c3288034362_add_channel_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/migrations/versions/53f81aba78ce_use_biginteger_for_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/migrations/versions/794249a0b1bd_adding_jobs_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/migrations/versions/8d1e9a9e0b1f_adding_download_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/migrations/versions/8dfb7c4bfbd7_new_package_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/migrations/versions/98c04a65df4a_register_mirrors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/migrations/versions/a3ffa287d074_case_insensitive_channel_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9084 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/migrations/versions/a80fb051a659_create_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/migrations/versions/b9886d9cadb0_create_indexes_for_download_count_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/migrations/versions/cd404ed93cc0_add_per_channel_ttl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/migrations/versions/cddba8e6e639_scheduling_spec_for_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/migrations/versions/d212023a8e0b_add_useremail_table_for_email_addresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/migrations/versions/db1c56bf4d57_add_channel_size_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/migrations/versions/ea6eba9a9ffc_merge_ebe550f9fbbe_and_b9886d9cadb0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/migrations/versions/ebe550f9fbbe_added_create_at_and_expire_at_date_to_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24546 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/pkgstores.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/repo_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8571 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/rest_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.382586 quetz-server-0.8.0/quetz/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tasks/assertions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tasks/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tasks/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tasks/indexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18320 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tasks/mirror.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tasks/reindexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9671 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tasks/workers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.382586 quetz-server-0.8.0/quetz/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/templates/channeldata-index.html.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/templates/subdir-index.html.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.382586 quetz-server-0.8.0/quetz/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/testing/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/testing/mockups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/testing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.386586 quetz-server-0.8.0/quetz/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.386586 quetz-server-0.8.0/quetz/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/api/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/api/test_api_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22577 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/api/test_channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/api/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23467 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/api/test_main_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9173 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/api/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/api/test_users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.386586 quetz-server-0.8.0/quetz/tests/authentification/
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/authentification/test_auth_dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/authentification/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17757 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/authentification/test_oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/authentification/test_pam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.386586 quetz-server-0.8.0/quetz/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.366586 quetz-server-0.8.0/quetz/tests/data/dummy-plugin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.386586 quetz-server-0.8.0/quetz/tests/data/dummy-plugin/quetz_dummyplugin/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/data/dummy-plugin/quetz_dummyplugin/jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.386586 quetz-server-0.8.0/quetz/tests/data/dummy-plugin/quetz_dummyplugin-1.0-py3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/data/dummy-plugin/quetz_dummyplugin-1.0-py3.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/data/dummy-plugin/quetz_dummyplugin-1.0-py3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/data/other-package-0.1-0.tar.bz2
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/data/other-package-0.2-0.tar.bz2
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/data/test-package-0.1-0.tar.bz2
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/data/test-package-0.1-0_copy.tar.bz2
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/data/test-package-0.2-0.tar.bz2
+-rw-r--r--   0 runner    (1001) docker     (123)    20798 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18709 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13028 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/test_dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/test_db_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/test_health.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/test_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27357 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38275 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/test_mirror.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/test_pkg_stores.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/test_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/test_versionorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/tests/test_workers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8985 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11429 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz/versionorder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.386586 quetz-server-0.8.0/quetz_db_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz_db_ext/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz_db_ext/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz_db_ext/LIBSOLV_LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14617 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz_db_ext/conda.c
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz_db_ext/conda.h
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz_db_ext/quetz_pg.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-01 07:34:02.000000 quetz-server-0.8.0/quetz_db_ext/quetz_sqlite.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:34:21.390586 quetz-server-0.8.0/quetz_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18021 2023-06-01 07:34:21.000000 quetz-server-0.8.0/quetz_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-06-01 07:34:21.000000 quetz-server-0.8.0/quetz_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 07:34:21.000000 quetz-server-0.8.0/quetz_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-01 07:34:21.000000 quetz-server-0.8.0/quetz_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-01 07:34:21.000000 quetz-server-0.8.0/quetz_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-01 07:34:21.000000 quetz-server-0.8.0/quetz_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-01 07:34:21.390586 quetz-server-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 07:34:02.000000 quetz-server-0.8.0/setup.py
```

### Comparing `quetz-server-0.7.0/.pre-commit-config.yaml` & `quetz-server-0.8.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/CHANGELOG.md` & `quetz-server-0.8.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,37 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 0.8.0
+
+([Full Changelog](https://github.com/mamba-org/quetz/compare/v0.7.0...b1ac607ed0900b6242519cd452e92539f83a6721))
+
+### Enhancements made
+
+- Sanitize DB urls before printing [#633](https://github.com/mamba-org/quetz/pull/633) ([@AndreasAlbertQC](https://github.com/AndreasAlbertQC))
+- Make sqlalchemy pool settings configurable [#632](https://github.com/mamba-org/quetz/pull/632) ([@AndreasAlbertQC](https://github.com/AndreasAlbertQC))
+- Avoid exposing the Postgres credentials [#628](https://github.com/mamba-org/quetz/pull/628) ([@sbivol](https://github.com/sbivol))
+- Add sampler profiling [#623](https://github.com/mamba-org/quetz/pull/623) ([@ivergara](https://github.com/ivergara))
+
+### Maintenance and upkeep improvements
+
+- Fix pre-commit / micromamba interplay [#634](https://github.com/mamba-org/quetz/pull/634) ([@AndreasAlbertQC](https://github.com/AndreasAlbertQC))
+- Add osx-arm64 version for testing on newer apple devices [#631](https://github.com/mamba-org/quetz/pull/631) ([@YYYasin19](https://github.com/YYYasin19))
+- Migrate to setup-micromamba [#627](https://github.com/mamba-org/quetz/pull/627) ([@pavelzw](https://github.com/pavelzw))
+- Move configurations to `pyproject.toml` [#624](https://github.com/mamba-org/quetz/pull/624) ([@SauravMaheshkar](https://github.com/SauravMaheshkar))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/mamba-org/quetz/graphs/contributors?from=2023-04-11&to=2023-06-01&type=c))
+
+[@AndreasAlbertQC](https://github.com/search?q=repo%3Amamba-org%2Fquetz+involves%3AAndreasAlbertQC+updated%3A2023-04-11..2023-06-01&type=Issues) | [@codecov-commenter](https://github.com/search?q=repo%3Amamba-org%2Fquetz+involves%3Acodecov-commenter+updated%3A2023-04-11..2023-06-01&type=Issues) | [@ivergara](https://github.com/search?q=repo%3Amamba-org%2Fquetz+involves%3Aivergara+updated%3A2023-04-11..2023-06-01&type=Issues) | [@janjagusch](https://github.com/search?q=repo%3Amamba-org%2Fquetz+involves%3Ajanjagusch+updated%3A2023-04-11..2023-06-01&type=Issues) | [@martinRenou](https://github.com/search?q=repo%3Amamba-org%2Fquetz+involves%3AmartinRenou+updated%3A2023-04-11..2023-06-01&type=Issues) | [@pavelzw](https://github.com/search?q=repo%3Amamba-org%2Fquetz+involves%3Apavelzw+updated%3A2023-04-11..2023-06-01&type=Issues) | [@SauravMaheshkar](https://github.com/search?q=repo%3Amamba-org%2Fquetz+involves%3ASauravMaheshkar+updated%3A2023-04-11..2023-06-01&type=Issues) | [@sbivol](https://github.com/search?q=repo%3Amamba-org%2Fquetz+involves%3Asbivol+updated%3A2023-04-11..2023-06-01&type=Issues) | [@YYYasin19](https://github.com/search?q=repo%3Amamba-org%2Fquetz+involves%3AYYYasin19+updated%3A2023-04-11..2023-06-01&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 0.7.0
 
 ([Full Changelog](https://github.com/mamba-org/quetz/compare/v0.6.3...bc0ac65796d14083ae587eba103d6d60250759ff))
 
 ### Enhancements made
 
 - Add endpoints for health checks [#622](https://github.com/mamba-org/quetz/pull/622) ([@janjagusch](https://github.com/janjagusch))
@@ -16,16 +42,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/mamba-org/quetz/graphs/contributors?from=2023-04-05&to=2023-04-11&type=c))
 
 [@codecov-commenter](https://github.com/search?q=repo%3Amamba-org%2Fquetz+involves%3Acodecov-commenter+updated%3A2023-04-05..2023-04-11&type=Issues) | [@janjagusch](https://github.com/search?q=repo%3Amamba-org%2Fquetz+involves%3Ajanjagusch+updated%3A2023-04-05..2023-04-11&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 0.6.3
 
 ([Full Changelog](https://github.com/mamba-org/quetz/compare/v0.6.2...794eccb91e775e3ff3466839dbfe65a226926615))
 
 ### Bugs fixed
 
 - Cast starlette URL to str [#618](https://github.com/mamba-org/quetz/pull/618) ([@janjagusch](https://github.com/janjagusch))
```

### Comparing `quetz-server-0.7.0/CONTRIBUTING.md` & `quetz-server-0.8.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/Dockerfile` & `quetz-server-0.8.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/LICENSE` & `quetz-server-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/MANIFEST.in` & `quetz-server-0.8.0/MANIFEST.in`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 include *.md
 include alembic.ini
 include dev_config.toml
 include environment.yml
 include init_db.py
-include .coveragerc
 include .flake8
 include .pre-commit-config.yaml
 include .readthedocs.yml
-include mypy.ini
 include download-test-package.sh
 
 recursive-include quetz/migrations *.*
 recursive-include quetz/tests *.*
 recursive-include quetz_db_ext *
 recursive-include quetz_frontend *.*
```

### Comparing `quetz-server-0.7.0/PKG-INFO` & `quetz-server-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quetz-server
-Version: 0.7.0
+Version: 0.8.0
 Summary: The mamba-org server for conda packages
 Home-page: https://github.com/mamba-org/quetz
 Author: QuantStack & Quetz contributors
 Author-email: wolf.vollprecht@quantstack.net
 Keywords: conda,mamba,server
 Platform: Linux
 Platform: Mac OS X
@@ -104,16 +104,17 @@
 ```
 
 To run the upload, you need to set environment variables for the quetz API key (which authenticates you) and the quetz server URL. As we passed the `--dev` flag to quetz, a testing API key can be found in quetz's output which you can use for this example.
 
 ```bash
 export QUETZ_API_KEY=E_KaBFstCKI9hTdPM7DQq56GglRHf2HW7tQtq6si370
 export QUETZ_SERVER_URL=http://localhost:8000
-quetz-client post_file_to_channel channel0 xtensor/linux-64/xtensor-0.16.1-0.tar.bz2
-quetz-client post_file_to_channel channel0 xtensor/osx-64/xtensor-0.16.1-0.tar.bz2
+quetz-client post_file_to_channel channel0 xtensor/linux-64/xtensor-0.24.3-h924138e_1.tar.bz2
+quetz-client post_file_to_channel channel0 xtensor/osx-64/xtensor-0.24.3-h1b54a9f_1.tar.bz2
+quetz-client post_file_to_channel channel0 xtensor/osx-arm64/xtensor-0.24.3-hf86a087_1.tar.bz2
 ```
 
 Install the test package with conda:
 
 ```bash
 mamba install --strict-channel-priority -c http://localhost:8000/get/channel0 -c conda-forge xtensor
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: quetz-server Version: 0.7.0 Summary: The mamba-org
+Metadata-Version: 2.1 Name: quetz-server Version: 0.8.0 Summary: The mamba-org
 server for conda packages Home-page: https://github.com/mamba-org/quetz Author:
 QuantStack & Quetz contributors Author-email: wolf.vollprecht@quantstack.net
 Keywords: conda,mamba,server Platform: Linux Platform: Mac OS X Requires-
 Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra: azure
 Provides-Extra: gcs Provides-Extra: pam Provides-Extra: postgre Provides-Extra:
 s3 Provides-Extra: all Provides-Extra: client Provides-Extra: dev Provides-
 Extra: test License-File: LICENSE ![quetz header image](docs/assets/
@@ -35,19 +35,21 @@
 install the [quetz-client](https://github.com/mamba-org/quetz-client): ```bash
 mamba install quetz-client ``` To run the upload, you need to set environment
 variables for the quetz API key (which authenticates you) and the quetz server
 URL. As we passed the `--dev` flag to quetz, a testing API key can be found in
 quetz's output which you can use for this example. ```bash export
 QUETZ_API_KEY=E_KaBFstCKI9hTdPM7DQq56GglRHf2HW7tQtq6si370 export
 QUETZ_SERVER_URL=http://localhost:8000 quetz-client post_file_to_channel
-channel0 xtensor/linux-64/xtensor-0.16.1-0.tar.bz2 quetz-client
-post_file_to_channel channel0 xtensor/osx-64/xtensor-0.16.1-0.tar.bz2 ```
-Install the test package with conda: ```bash mamba install --strict-channel-
-priority -c http://localhost:8000/get/channel0 -c conda-forge xtensor ```
-Output: ```text ... Package Version Build Channel Size
+channel0 xtensor/linux-64/xtensor-0.24.3-h924138e_1.tar.bz2 quetz-client
+post_file_to_channel channel0 xtensor/osx-64/xtensor-0.24.3-h1b54a9f_1.tar.bz2
+quetz-client post_file_to_channel channel0 xtensor/osx-arm64/xtensor-0.24.3-
+hf86a087_1.tar.bz2 ``` Install the test package with conda: ```bash mamba
+install --strict-channel-priority -c http://localhost:8000/get/channel0 -
+c conda-forge xtensor ``` Output: ```text ... Package Version Build Channel
+Size
 âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ
 Install:
 âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ
 xtensor 0.16.1 0 http://localhost:8000/get/channel0/osx-64 109 KB xtl 0.4.16
 h04f5b5a_1000 conda-forge/osx-64 47 KB Summary: Install: 2 packages Total
 download: 156 KB
 âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ
```

### Comparing `quetz-server-0.7.0/README.md` & `quetz-server-0.8.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -81,16 +81,17 @@
 ```
 
 To run the upload, you need to set environment variables for the quetz API key (which authenticates you) and the quetz server URL. As we passed the `--dev` flag to quetz, a testing API key can be found in quetz's output which you can use for this example.
 
 ```bash
 export QUETZ_API_KEY=E_KaBFstCKI9hTdPM7DQq56GglRHf2HW7tQtq6si370
 export QUETZ_SERVER_URL=http://localhost:8000
-quetz-client post_file_to_channel channel0 xtensor/linux-64/xtensor-0.16.1-0.tar.bz2
-quetz-client post_file_to_channel channel0 xtensor/osx-64/xtensor-0.16.1-0.tar.bz2
+quetz-client post_file_to_channel channel0 xtensor/linux-64/xtensor-0.24.3-h924138e_1.tar.bz2
+quetz-client post_file_to_channel channel0 xtensor/osx-64/xtensor-0.24.3-h1b54a9f_1.tar.bz2
+quetz-client post_file_to_channel channel0 xtensor/osx-arm64/xtensor-0.24.3-hf86a087_1.tar.bz2
 ```
 
 Install the test package with conda:
 
 ```bash
 mamba install --strict-channel-priority -c http://localhost:8000/get/channel0 -c conda-forge xtensor
 ```
```

#### html2text {}

```diff
@@ -28,19 +28,21 @@
 install the [quetz-client](https://github.com/mamba-org/quetz-client): ```bash
 mamba install quetz-client ``` To run the upload, you need to set environment
 variables for the quetz API key (which authenticates you) and the quetz server
 URL. As we passed the `--dev` flag to quetz, a testing API key can be found in
 quetz's output which you can use for this example. ```bash export
 QUETZ_API_KEY=E_KaBFstCKI9hTdPM7DQq56GglRHf2HW7tQtq6si370 export
 QUETZ_SERVER_URL=http://localhost:8000 quetz-client post_file_to_channel
-channel0 xtensor/linux-64/xtensor-0.16.1-0.tar.bz2 quetz-client
-post_file_to_channel channel0 xtensor/osx-64/xtensor-0.16.1-0.tar.bz2 ```
-Install the test package with conda: ```bash mamba install --strict-channel-
-priority -c http://localhost:8000/get/channel0 -c conda-forge xtensor ```
-Output: ```text ... Package Version Build Channel Size
+channel0 xtensor/linux-64/xtensor-0.24.3-h924138e_1.tar.bz2 quetz-client
+post_file_to_channel channel0 xtensor/osx-64/xtensor-0.24.3-h1b54a9f_1.tar.bz2
+quetz-client post_file_to_channel channel0 xtensor/osx-arm64/xtensor-0.24.3-
+hf86a087_1.tar.bz2 ``` Install the test package with conda: ```bash mamba
+install --strict-channel-priority -c http://localhost:8000/get/channel0 -
+c conda-forge xtensor ``` Output: ```text ... Package Version Build Channel
+Size
 âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ
 Install:
 âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ
 xtensor 0.16.1 0 http://localhost:8000/get/channel0/osx-64 109 KB xtl 0.4.16
 h04f5b5a_1000 conda-forge/osx-64 47 KB Summary: Install: 2 packages Total
 download: 156 KB
 âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ
```

### Comparing `quetz-server-0.7.0/RELEASE.md` & `quetz-server-0.8.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/alembic.ini` & `quetz-server-0.8.0/alembic.ini`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/docker/Dockerfile` & `quetz-server-0.8.0/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/docker/docker_config.toml` & `quetz-server-0.8.0/docker/docker_config.toml`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/docker/jupyterhub_config.py` & `quetz-server-0.8.0/docker/jupyterhub_config.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/docker/nginx.conf` & `quetz-server-0.8.0/docker/nginx.conf`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/docker/postgres.conf` & `quetz-server-0.8.0/docker/postgres.conf`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/docker-compose.yml` & `quetz-server-0.8.0/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/docs/Makefile` & `quetz-server-0.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/docs/assets/quetz_header.png` & `quetz-server-0.8.0/docs/assets/quetz_header.png`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/docs/make.bat` & `quetz-server-0.8.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/docs/source/_static/quetz_favicon.ico` & `quetz-server-0.8.0/docs/source/_static/quetz_favicon.ico`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/docs/source/_static/quetz_logo.png` & `quetz-server-0.8.0/docs/source/_static/quetz_logo.png`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/docs/source/conf.py` & `quetz-server-0.8.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/docs/source/deploying/authenticators.rst` & `quetz-server-0.8.0/docs/source/deploying/authenticators.rst`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/docs/source/deploying/configuration.rst` & `quetz-server-0.8.0/docs/source/deploying/configuration.rst`

 * *Files 16% similar despite different names*

```diff
@@ -15,18 +15,41 @@
 ^^^^^^^^^^^^^^^^^^^^^^
 
 Quetz can be run with SQLlite or PostgreSQL as database backends (PostgreSQL is recommended for production use). You can configure the backend by setting the URI prefixed with the backend name. To configure, PostgreSQL, you may use:
 
 .. code::
 
    [sqlalchemy]
+   # The URL to the database to use.
    database_url = "postgresql://postgres:mysecretpassword@localhost:5432/quetz"
 
+   # Undocumented setting, unknown use
+   database_plugin_path = ""
+
+   # Passed directly to the "echo" argument of sqlalchemy.create_engine
+   echo_sql = false
+
+   # The pool size for sqlalchemy engine connections to postgres DBs
+   # see https://docs.sqlalchemy.org/en/latest/core/pooling.html
+   postgres_pool_size = 100
+
+   # The maximal number of overflow connections beyond the pool size
+   # see https://docs.sqlalchemy.org/en/latest/core/pooling.html
+   postgres_max_overflow = 100
+
 :database_url: URL of the database (may contain user credentials) prefixed with either ``sqlite://`` or ``postgresql://``.
 
+:database_plugin_path: Undocumented setting, unknown use, default: `""`.
+
+:echo_sql: Passed directly to the "echo" argument of sqlalchemy.create_engine, default: `false`.
+
+:postgres_pool_size: The pool size for sqlalchemy engine connections to postgres DBs. See `sqlalchemy docs <https://docs.sqlalchemy.org/en/latest/core/pooling.html>`_. Default: `100`
+
+:postgres_max_overflow: The maximal number of overflow connections beyond the pool size. See `sqlalchemy docs <https://docs.sqlalchemy.org/en/latest/core/pooling.html>`_. Default: `100`
+
 ``github`` section
 ^^^^^^^^^^^^^^^^^^
 
 You can use github as identity provider, i.e., users will connect to quetz with their github accounts. To register quetz as a github application, please go to the URL: `<https://github.com/settings/applications/new>`_ and add your quetz application, than copy-and-paste the provided ``client_id`` and ``client_secret`` credentials in this section.
 
 :client_id: 
 :client_secret: application credentials retrieved from github
@@ -221,14 +244,23 @@
 ``quotas`` section
 ^^^^^^^^^^^^^^^^^^
 
 You can configure the limits (quota) on the size of uploaded packages for each channel:
 
 :channel_quota: maximum total size (in bytes) of packages uploaded to the channel
 
+``profiling`` section
+^^^^^^^^^^^^^^^^^^^^^
+
+Quetz provides instrumentation for profiling its endpoints.
+
+:enable_sampling: enables sampling profiling by providing the query parameter `profile=true` (or any truth value) to the request. When active and provided the query parameter, the returned response will be highjacked to provide an HTML version of the profile output.
+
+:interval_seconds: sampling interval in seconds. If not set, it has a default value of `0.001`.
+
 Environment
 -----------
 
 You can also use a couple of environment variables to configure the behaviour of quetz:
 
 =======================  ======================================  ===========================  ===================
 Variable                 description                             values                       default
```

### Comparing `quetz-server-0.7.0/docs/source/deploying/database.rst` & `quetz-server-0.8.0/docs/source/deploying/database.rst`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/docs/source/deploying/migrations.rst` & `quetz-server-0.8.0/docs/source/deploying/migrations.rst`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/docs/source/deploying/nginx.rst` & `quetz-server-0.8.0/docs/source/deploying/nginx.rst`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/docs/source/deploying/workers.rst` & `quetz-server-0.8.0/docs/source/deploying/workers.rst`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/docs/source/index.rst` & `quetz-server-0.8.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/docs/source/plugins.rst` & `quetz-server-0.8.0/docs/source/plugins.rst`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/docs/source/qeps/qep-001-user-permissions.rst` & `quetz-server-0.8.0/docs/source/qeps/qep-001-user-permissions.rst`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/docs/source/using/basics.rst` & `quetz-server-0.8.0/docs/source/using/basics.rst`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/docs/source/using/mirroring.rst` & `quetz-server-0.8.0/docs/source/using/mirroring.rst`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/environment.yml` & `quetz-server-0.8.0/environment.yml`

 * *Files 15% similar despite different names*

```diff
@@ -43,9 +43,10 @@
   - pre-commit
   - pytest
   - pytest-mock
   - rq
   - libcflib
   - mamba
   - conda-content-trust
+  - pyinstrument
   - pip:
       - git+https://github.com/jupyter-server/jupyter_releaser.git@v2
```

### Comparing `quetz-server-0.7.0/init_db.py` & `quetz-server-0.8.0/init_db.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/pyproject.toml` & `quetz-server-0.8.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 [tool.jupyter-releaser.options]
 check-imports = ["quetz"]
 
 [tool.check-wheel-contents]
 ignore = ["W004"]
 
 [tool.tbump.version]
-current = "0.7.0"
+current = "0.8.0"
 regex = '''
   (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)
   ((?P<channel>a|b|rc|.dev)(?P<release>\d+))?
 '''
 
 [[tool.tbump.field]]
 name = "channel"
@@ -52,7 +52,21 @@
 reportOptionalOperand = true
 reportOptionalSubscript = true
 reportPrivateImportUsage = true
 reportUnboundVariable = true
 reportUndefinedVariable = false
 venv = ".venv"
 venvPath= "."
+
+[tool.mypy]
+ignore_missing_imports = true
+plugins = [
+  "sqlmypy"
+]
+disable_error_code = [
+  "misc"
+]
+
+[tool.coverage.run]
+omit = [
+  "quetz/tests/*",
+]
```

### Comparing `quetz-server-0.7.0/quetz/authentication/auth_dao.py` & `quetz-server-0.8.0/quetz/authentication/auth_dao.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/authentication/azuread.py` & `quetz-server-0.8.0/quetz/authentication/azuread.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/authentication/base.py` & `quetz-server-0.8.0/quetz/authentication/base.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/authentication/github.py` & `quetz-server-0.8.0/quetz/authentication/github.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/authentication/gitlab.py` & `quetz-server-0.8.0/quetz/authentication/gitlab.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/authentication/google.py` & `quetz-server-0.8.0/quetz/authentication/google.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/authentication/jupyterhub.py` & `quetz-server-0.8.0/quetz/authentication/jupyterhub.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/authentication/oauth2.py` & `quetz-server-0.8.0/quetz/authentication/oauth2.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/authentication/pam.py` & `quetz-server-0.8.0/quetz/authentication/pam.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/authentication/registry.py` & `quetz-server-0.8.0/quetz/authentication/registry.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/authorization.py` & `quetz-server-0.8.0/quetz/authorization.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/basic_frontend/avatar.jpg` & `quetz-server-0.8.0/quetz/basic_frontend/avatar.jpg`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/basic_frontend/favicon.ico` & `quetz-server-0.8.0/quetz/basic_frontend/favicon.ico`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/basic_frontend/index.html` & `quetz-server-0.8.0/quetz/basic_frontend/index.html`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/channel_data.py` & `quetz-server-0.8.0/quetz/channel_data.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/cli.py` & `quetz-server-0.8.0/quetz/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from quetz.config import (
     Config,
     _env_config_file,
     _env_prefix,
     configure_logger,
     create_config,
 )
-from quetz.database import get_session
+from quetz.database import get_session, sanitize_db_url
 from quetz.db_models import (
     ApiKey,
     Channel,
     ChannelMember,
     Identity,
     Package,
     PackageMember,
@@ -86,17 +86,24 @@
 
 
 def _run_migrations(
     db_url: Optional[str] = None,
     alembic_config: Optional[AlembicConfig] = None,
     branch_name: str = "heads",
 ) -> None:
-    logger.info('Running DB migrations on %r', db_url)
-    if not alembic_config and db_url:
-        alembic_config = _alembic_config(db_url)
+    if db_url:
+        if db_url.startswith("postgre"):
+            db_engine = "PostgreSQL"
+        elif db_url.startswith("sqlite"):
+            db_engine = "SQLite"
+        else:
+            db_engine = db_url.split("/")[0]
+        logger.info('Running DB migrations on %s', db_engine)
+        if not alembic_config:
+            alembic_config = _alembic_config(db_url)
     command.upgrade(alembic_config, branch_name)
 
 
 def _make_migrations(
     db_url: Optional[str],
     message: str,
     plugin_name: str = "quetz",
@@ -304,15 +311,15 @@
         else:
             config = Config()
             db_path = Path(os.getcwd())
         with working_directory(db_path):
             if not database_exists(config.sqlalchemy_database_url):
                 logger.error(
                     "Cannot verify that specified database exists. "
-                    + config.sqlalchemy_database_url
+                    + sanitize_db_url(config.sqlalchemy_database_url)
                 )
                 return False
             else:
                 return True
 
     return False
```

### Comparing `quetz-server-0.7.0/quetz/condainfo.py` & `quetz-server-0.8.0/quetz/condainfo.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/config.py` & `quetz-server-0.8.0/quetz/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,14 +102,16 @@
         ),
         ConfigSection(
             "sqlalchemy",
             [
                 ConfigEntry("database_url", str),
                 ConfigEntry("database_plugin_path", str, default="", required=False),
                 ConfigEntry("echo_sql", bool, default=False, required=False),
+                ConfigEntry("postgres_pool_size", int, default=100, required=False),
+                ConfigEntry("postgres_max_overflow", int, default=100, required=False),
             ],
         ),
         ConfigSection(
             "session",
             [ConfigEntry("secret", str), ConfigEntry("https_only", bool, default=True)],
         ),
         ConfigSection(
@@ -210,14 +212,22 @@
         ConfigSection(
             "quotas",
             [
                 ConfigEntry("channel_quota", int, required=False),
             ],
             required=False,
         ),
+        ConfigSection(
+            "profiling",
+            [
+                ConfigEntry("enable_sampling", bool, required=False, default=False),
+                ConfigEntry("interval_seconds", float, required=False, default=0.001),
+            ],
+            required=False,
+        ),
     ]
     _config_dirs = [_site_dir, _user_dir]
     _config_files = [os.path.join(d, _filename) for d in _config_dirs]
 
     _instances: Dict[Optional[str], "Config"] = {}
 
     def __new__(cls, deployment_config: str = None):
```

### Comparing `quetz-server-0.7.0/quetz/dao.py` & `quetz-server-0.8.0/quetz/dao.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/database.py` & `quetz-server-0.8.0/quetz/database.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 # Copyright 2020 QuantStack
 # Distributed under the terms of the Modified BSD License.
 import logging
+import re
 from contextlib import contextmanager
 from typing import Callable
 
 from sqlalchemy import create_engine, event
 from sqlalchemy.engine import Engine
+from sqlalchemy.engine.url import make_url
+from sqlalchemy.exc import ArgumentError
 from sqlalchemy.orm import sessionmaker
 from sqlalchemy.orm.session import Session
 from sqlalchemy.pool import StaticPool
 
 from quetz.config import Config
 from quetz.metrics.middleware import DATABASE_CONNECTIONS_USED, DATABASE_POOL_SIZE
 
@@ -22,35 +25,32 @@
     checked_in = engine.pool.checkedin()
     checked_out = engine.pool.checkedout()
     pool_size = checked_in + checked_out
     DATABASE_POOL_SIZE.set(pool_size)
     DATABASE_CONNECTIONS_USED.set(checked_out)
 
 
-def get_engine(db_url, echo: bool = False, reuse_engine=True, **kwargs) -> Engine:
+def get_engine(db_url, reuse_engine=True, **kwargs) -> Engine:
     if db_url.startswith('sqlite'):
         kwargs.setdefault('connect_args', {'check_same_thread': False})
 
     if db_url.endswith(':memory:'):
         # If we're using an in-memory database, ensure that only one connection
         # is ever created.
         kwargs.setdefault('poolclass', StaticPool)
 
     global engine
 
     if not engine or not reuse_engine:
-        # TODO make configurable!
         if db_url.startswith('postgres'):
-            engine = create_engine(
-                db_url, echo=echo, pool_size=200, max_overflow=100, **kwargs
-            )
+            engine = create_engine(db_url, **kwargs)
             for event_name in ['connect', 'close', 'checkin', 'checkout']:
                 event.listen(engine, event_name, set_metrics)
         else:
-            engine = create_engine(db_url, echo=echo, **kwargs)
+            engine = create_engine(db_url, **kwargs)
 
         def on_connect(dbapi_conn, conn_record):
             logger.debug("connection opened: %s", engine.pool.status())
 
         def on_close(dbapi_conn, conn_record):
             logger.debug("connection closed: %s", engine.pool.status())
 
@@ -60,26 +60,59 @@
     return engine
 
 
 def get_session_maker(engine) -> Callable[[], Session]:
     return sessionmaker(autocommit=False, autoflush=True, bind=engine)
 
 
-def get_session(db_url: str, echo: bool = False, **kwargs) -> Session:
+def get_session(db_url: str, **kwargs) -> Session:
     """Get a database session.
 
     Important note: this function is mocked during tests!
 
     """
-    return get_session_maker(get_engine(db_url, echo, **kwargs))()
+    return get_session_maker(get_engine(db_url, **kwargs))()
 
 
 @contextmanager
 def get_db_manager():
     config = Config()
-    database_url = config.sqlalchemy_database_url
-    db = get_session(database_url, echo=config.sqlalchemy_echo_sql)
+    db = get_session(
+        db_url=config.sqlalchemy_database_url,
+        echo=config.sqlalchemy_echo_sql,
+        pool_size=config.sqlalchemy_postgres_pool_size,
+        max_overflow=config.sqlalchemy_postgres_max_overflow,
+    )
 
     try:
         yield db
     finally:
         db.close()
+
+
+def sanitize_db_url(db_url: str) -> str:
+    """
+    Sanitizes the DB url so it is safe to print.
+
+    If the URL is parseable with sqlalchemy's make_url,
+    it is parsed and the password is replaced.
+    If not, we try to replace everything between ":" and "@",
+    if those characters are present.
+
+    If neither method succeeds, we give up and return the
+    full initial URL.
+    """
+
+    # Attempt 1: Actual parsing, this is ideal but may fail
+    try:
+        parsed_url = make_url(db_url)
+        if parsed_url.password:
+            return db_url.replace(parsed_url.password, "***")
+    except ArgumentError:
+        pass
+
+    # Attempt 2: Poor man's parsing: Just replacing everything between ":" and "@"
+    if ":" in db_url and "@" in db_url:
+        return re.sub(":[^:@]*@", ":***@", db_url)
+
+    # Fallback: We don't understand the URL format, so we do nothing
+    return db_url
```

### Comparing `quetz-server-0.7.0/quetz/database_extensions.py` & `quetz-server-0.8.0/quetz/database_extensions.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/db_models.py` & `quetz-server-0.8.0/quetz/db_models.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/deps.py` & `quetz-server-0.8.0/quetz/deps.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/frontend.py` & `quetz-server-0.8.0/quetz/frontend.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/hooks.py` & `quetz-server-0.8.0/quetz/hooks.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/jobs/api.py` & `quetz-server-0.8.0/quetz/jobs/api.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/jobs/dao.py` & `quetz-server-0.8.0/quetz/jobs/dao.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/jobs/handlers.py` & `quetz-server-0.8.0/quetz/jobs/handlers.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/jobs/models.py` & `quetz-server-0.8.0/quetz/jobs/models.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/jobs/rest_models.py` & `quetz-server-0.8.0/quetz/jobs/rest_models.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/jobs/runner.py` & `quetz-server-0.8.0/quetz/jobs/runner.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/main.py` & `quetz-server-0.8.0/quetz/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,35 +10,36 @@
 import time
 import uuid
 from collections import Counter
 from concurrent.futures import ThreadPoolExecutor
 from contextlib import contextmanager
 from email.utils import formatdate
 from tempfile import SpooledTemporaryFile, TemporaryFile
-from typing import List, Optional, Tuple, Type
+from typing import Awaitable, Callable, List, Optional, Tuple, Type
 
 import pydantic
 import pydantic.error_wrappers
 import requests
 from fastapi import (
     APIRouter,
     BackgroundTasks,
     Depends,
     FastAPI,
     File,
     Form,
     Header,
     HTTPException,
     Request,
+    Response,
     UploadFile,
     responses,
     status,
 )
 from fastapi.middleware.cors import CORSMiddleware
-from fastapi.responses import RedirectResponse, StreamingResponse
+from fastapi.responses import HTMLResponse, RedirectResponse, StreamingResponse
 from importlib_metadata import entry_points
 from sqlalchemy.exc import IntegrityError
 from sqlalchemy.orm import Session
 from starlette.concurrency import run_in_threadpool
 from starlette.middleware.base import BaseHTTPMiddleware
 from starlette.middleware.httpsredirect import HTTPSRedirectMiddleware
 from starlette.middleware.sessions import SessionMiddleware
@@ -159,14 +160,35 @@
         response = await call_next(request)
 
         return response
 
 
 app.add_middleware(CondaTokenMiddleware)
 
+
+if config.configured_section("profiling") and config.profiling_enable_sampling:
+    from pyinstrument.profiler import Profiler
+
+    @app.middleware("http")
+    async def profile_request(
+        request: Request,
+        call_next: Callable[[Request], Awaitable[Response]],
+    ):
+        if not request.query_params.get("profile", False):
+            return await call_next(request)
+        profiler = Profiler(
+            interval=config.profiling_interval_seconds,
+            async_mode="enabled",
+        )
+        profiler.start()
+        await call_next(request)
+        profiler.stop()
+        return HTMLResponse(profiler.output_html())
+
+
 pkgstore = config.get_package_store()
 
 # authenticators
 
 
 builtin_authenticators: List[Type[BaseAuthenticator]] = [
     authenticator
```

### Comparing `quetz-server-0.7.0/quetz/metrics/api.py` & `quetz-server-0.8.0/quetz/metrics/api.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/metrics/db_models.py` & `quetz-server-0.8.0/quetz/metrics/db_models.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/metrics/middleware.py` & `quetz-server-0.8.0/quetz/metrics/middleware.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/metrics/rest_models.py` & `quetz-server-0.8.0/quetz/metrics/rest_models.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/metrics/tasks.py` & `quetz-server-0.8.0/quetz/metrics/tasks.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/metrics/view.py` & `quetz-server-0.8.0/quetz/metrics/view.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/migrations/env.py` & `quetz-server-0.8.0/quetz/migrations/env.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/migrations/versions/0653794b6252_adding_url_and_platforms_dirs.py` & `quetz-server-0.8.0/quetz/migrations/versions/0653794b6252_adding_url_and_platforms_dirs.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/migrations/versions/0a0ab48887ab_adding_function_args_to_job_spec.py` & `quetz-server-0.8.0/quetz/migrations/versions/0a0ab48887ab_adding_function_args_to_job_spec.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/migrations/versions/30241b33d849_add_task_pending_state.py` & `quetz-server-0.8.0/quetz/migrations/versions/30241b33d849_add_task_pending_state.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/migrations/versions/303ff70c27fc_configure_mirror_endpoints.py` & `quetz-server-0.8.0/quetz/migrations/versions/303ff70c27fc_configure_mirror_endpoints.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/migrations/versions/3c3288034362_add_channel_metadata.py` & `quetz-server-0.8.0/quetz/migrations/versions/3c3288034362_add_channel_metadata.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/migrations/versions/53f81aba78ce_use_biginteger_for_size.py` & `quetz-server-0.8.0/quetz/migrations/versions/53f81aba78ce_use_biginteger_for_size.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/migrations/versions/794249a0b1bd_adding_jobs_tables.py` & `quetz-server-0.8.0/quetz/migrations/versions/794249a0b1bd_adding_jobs_tables.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/migrations/versions/8d1e9a9e0b1f_adding_download_metrics.py` & `quetz-server-0.8.0/quetz/migrations/versions/8d1e9a9e0b1f_adding_download_metrics.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/migrations/versions/8dfb7c4bfbd7_new_package_versions.py` & `quetz-server-0.8.0/quetz/migrations/versions/8dfb7c4bfbd7_new_package_versions.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/migrations/versions/98c04a65df4a_register_mirrors.py` & `quetz-server-0.8.0/quetz/migrations/versions/98c04a65df4a_register_mirrors.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/migrations/versions/a3ffa287d074_case_insensitive_channel_names.py` & `quetz-server-0.8.0/quetz/migrations/versions/a3ffa287d074_case_insensitive_channel_names.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/migrations/versions/a80fb051a659_create_tables.py` & `quetz-server-0.8.0/quetz/migrations/versions/a80fb051a659_create_tables.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/migrations/versions/b9886d9cadb0_create_indexes_for_download_count_.py` & `quetz-server-0.8.0/quetz/migrations/versions/b9886d9cadb0_create_indexes_for_download_count_.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/migrations/versions/cd404ed93cc0_add_per_channel_ttl.py` & `quetz-server-0.8.0/quetz/migrations/versions/cd404ed93cc0_add_per_channel_ttl.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/migrations/versions/cddba8e6e639_scheduling_spec_for_jobs.py` & `quetz-server-0.8.0/quetz/migrations/versions/cddba8e6e639_scheduling_spec_for_jobs.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/migrations/versions/d212023a8e0b_add_useremail_table_for_email_addresses.py` & `quetz-server-0.8.0/quetz/migrations/versions/d212023a8e0b_add_useremail_table_for_email_addresses.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/migrations/versions/db1c56bf4d57_add_channel_size_limit.py` & `quetz-server-0.8.0/quetz/migrations/versions/db1c56bf4d57_add_channel_size_limit.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/migrations/versions/ebe550f9fbbe_added_create_at_and_expire_at_date_to_.py` & `quetz-server-0.8.0/quetz/migrations/versions/ebe550f9fbbe_added_create_at_and_expire_at_date_to_.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/pkgstores.py` & `quetz-server-0.8.0/quetz/pkgstores.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/repo_data.py` & `quetz-server-0.8.0/quetz/repo_data.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/rest_models.py` & `quetz-server-0.8.0/quetz/rest_models.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/tasks/common.py` & `quetz-server-0.8.0/quetz/tasks/common.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/tasks/indexing.py` & `quetz-server-0.8.0/quetz/tasks/indexing.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/tasks/mirror.py` & `quetz-server-0.8.0/quetz/tasks/mirror.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/tasks/reindexing.py` & `quetz-server-0.8.0/quetz/tasks/reindexing.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/tasks/workers.py` & `quetz-server-0.8.0/quetz/tasks/workers.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/templates/channeldata-index.html.j2` & `quetz-server-0.8.0/quetz/templates/channeldata-index.html.j2`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/templates/subdir-index.html.j2` & `quetz-server-0.8.0/quetz/templates/subdir-index.html.j2`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/testing/fixtures.py` & `quetz-server-0.8.0/quetz/testing/fixtures.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,15 +178,18 @@
 [plugins]
 enabled = {plugins}
 """
 
 
 @pytest.fixture
 def config_extra():
-    return ""
+    return """
+[profiling]
+enable_sampling = true
+"""
 
 
 @pytest.fixture
 def config_str(config_base, config_extra):
     return "\n".join([config_base, config_extra])
```

### Comparing `quetz-server-0.7.0/quetz/testing/mockups.py` & `quetz-server-0.8.0/quetz/testing/mockups.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/testing/utils.py` & `quetz-server-0.8.0/quetz/testing/utils.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/tests/api/conftest.py` & `quetz-server-0.8.0/quetz/tests/api/conftest.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/tests/api/test_api_keys.py` & `quetz-server-0.8.0/quetz/tests/api/test_api_keys.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/tests/api/test_channels.py` & `quetz-server-0.8.0/quetz/tests/api/test_channels.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/tests/api/test_main.py` & `quetz-server-0.8.0/quetz/tests/api/test_main.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/tests/api/test_main_packages.py` & `quetz-server-0.8.0/quetz/tests/api/test_main_packages.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/tests/api/test_metrics.py` & `quetz-server-0.8.0/quetz/tests/api/test_metrics.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/tests/api/test_users.py` & `quetz-server-0.8.0/quetz/tests/api/test_users.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/tests/authentification/test_auth_dao.py` & `quetz-server-0.8.0/quetz/tests/authentification/test_auth_dao.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/tests/authentification/test_base.py` & `quetz-server-0.8.0/quetz/tests/authentification/test_base.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/tests/authentification/test_oauth.py` & `quetz-server-0.8.0/quetz/tests/authentification/test_oauth.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/tests/authentification/test_pam.py` & `quetz-server-0.8.0/quetz/tests/authentification/test_pam.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/tests/conftest.py` & `quetz-server-0.8.0/quetz/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/tests/data/other-package-0.1-0.tar.bz2` & `quetz-server-0.8.0/quetz/tests/data/other-package-0.1-0.tar.bz2`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/tests/data/other-package-0.2-0.tar.bz2` & `quetz-server-0.8.0/quetz/tests/data/other-package-0.2-0.tar.bz2`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/tests/data/test-package-0.1-0.tar.bz2` & `quetz-server-0.8.0/quetz/tests/data/test-package-0.1-0.tar.bz2`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/tests/data/test-package-0.1-0_copy.tar.bz2` & `quetz-server-0.8.0/quetz/tests/data/test-package-0.1-0_copy.tar.bz2`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/tests/data/test-package-0.2-0.tar.bz2` & `quetz-server-0.8.0/quetz/tests/data/test-package-0.2-0.tar.bz2`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/tests/test_auth.py` & `quetz-server-0.8.0/quetz/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/tests/test_cli.py` & `quetz-server-0.8.0/quetz/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/tests/test_config.py` & `quetz-server-0.8.0/quetz/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/tests/test_dao.py` & `quetz-server-0.8.0/quetz/tests/test_dao.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/tests/test_indexing.py` & `quetz-server-0.8.0/quetz/tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/tests/test_jobs.py` & `quetz-server-0.8.0/quetz/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/tests/test_mirror.py` & `quetz-server-0.8.0/quetz/tests/test_mirror.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/tests/test_pkg_stores.py` & `quetz-server-0.8.0/quetz/tests/test_pkg_stores.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/tests/test_tasks.py` & `quetz-server-0.8.0/quetz/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/tests/test_versionorder.py` & `quetz-server-0.8.0/quetz/tests/test_versionorder.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/tests/test_workers.py` & `quetz-server-0.8.0/quetz/tests/test_workers.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/utils.py` & `quetz-server-0.8.0/quetz/utils.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz/versionorder.py` & `quetz-server-0.8.0/quetz/versionorder.py`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz_db_ext/CMakeLists.txt` & `quetz-server-0.8.0/quetz_db_ext/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz_db_ext/LIBSOLV_LICENSE.txt` & `quetz-server-0.8.0/quetz_db_ext/LIBSOLV_LICENSE.txt`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz_db_ext/conda.c` & `quetz-server-0.8.0/quetz_db_ext/conda.c`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz_db_ext/conda.h` & `quetz-server-0.8.0/quetz_db_ext/conda.h`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz_db_ext/quetz_pg.c` & `quetz-server-0.8.0/quetz_db_ext/quetz_pg.c`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz_db_ext/quetz_sqlite.c` & `quetz-server-0.8.0/quetz_db_ext/quetz_sqlite.c`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/quetz_server.egg-info/PKG-INFO` & `quetz-server-0.8.0/quetz_server.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quetz-server
-Version: 0.7.0
+Version: 0.8.0
 Summary: The mamba-org server for conda packages
 Home-page: https://github.com/mamba-org/quetz
 Author: QuantStack & Quetz contributors
 Author-email: wolf.vollprecht@quantstack.net
 Keywords: conda,mamba,server
 Platform: Linux
 Platform: Mac OS X
@@ -104,16 +104,17 @@
 ```
 
 To run the upload, you need to set environment variables for the quetz API key (which authenticates you) and the quetz server URL. As we passed the `--dev` flag to quetz, a testing API key can be found in quetz's output which you can use for this example.
 
 ```bash
 export QUETZ_API_KEY=E_KaBFstCKI9hTdPM7DQq56GglRHf2HW7tQtq6si370
 export QUETZ_SERVER_URL=http://localhost:8000
-quetz-client post_file_to_channel channel0 xtensor/linux-64/xtensor-0.16.1-0.tar.bz2
-quetz-client post_file_to_channel channel0 xtensor/osx-64/xtensor-0.16.1-0.tar.bz2
+quetz-client post_file_to_channel channel0 xtensor/linux-64/xtensor-0.24.3-h924138e_1.tar.bz2
+quetz-client post_file_to_channel channel0 xtensor/osx-64/xtensor-0.24.3-h1b54a9f_1.tar.bz2
+quetz-client post_file_to_channel channel0 xtensor/osx-arm64/xtensor-0.24.3-hf86a087_1.tar.bz2
 ```
 
 Install the test package with conda:
 
 ```bash
 mamba install --strict-channel-priority -c http://localhost:8000/get/channel0 -c conda-forge xtensor
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: quetz-server Version: 0.7.0 Summary: The mamba-org
+Metadata-Version: 2.1 Name: quetz-server Version: 0.8.0 Summary: The mamba-org
 server for conda packages Home-page: https://github.com/mamba-org/quetz Author:
 QuantStack & Quetz contributors Author-email: wolf.vollprecht@quantstack.net
 Keywords: conda,mamba,server Platform: Linux Platform: Mac OS X Requires-
 Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra: azure
 Provides-Extra: gcs Provides-Extra: pam Provides-Extra: postgre Provides-Extra:
 s3 Provides-Extra: all Provides-Extra: client Provides-Extra: dev Provides-
 Extra: test License-File: LICENSE ![quetz header image](docs/assets/
@@ -35,19 +35,21 @@
 install the [quetz-client](https://github.com/mamba-org/quetz-client): ```bash
 mamba install quetz-client ``` To run the upload, you need to set environment
 variables for the quetz API key (which authenticates you) and the quetz server
 URL. As we passed the `--dev` flag to quetz, a testing API key can be found in
 quetz's output which you can use for this example. ```bash export
 QUETZ_API_KEY=E_KaBFstCKI9hTdPM7DQq56GglRHf2HW7tQtq6si370 export
 QUETZ_SERVER_URL=http://localhost:8000 quetz-client post_file_to_channel
-channel0 xtensor/linux-64/xtensor-0.16.1-0.tar.bz2 quetz-client
-post_file_to_channel channel0 xtensor/osx-64/xtensor-0.16.1-0.tar.bz2 ```
-Install the test package with conda: ```bash mamba install --strict-channel-
-priority -c http://localhost:8000/get/channel0 -c conda-forge xtensor ```
-Output: ```text ... Package Version Build Channel Size
+channel0 xtensor/linux-64/xtensor-0.24.3-h924138e_1.tar.bz2 quetz-client
+post_file_to_channel channel0 xtensor/osx-64/xtensor-0.24.3-h1b54a9f_1.tar.bz2
+quetz-client post_file_to_channel channel0 xtensor/osx-arm64/xtensor-0.24.3-
+hf86a087_1.tar.bz2 ``` Install the test package with conda: ```bash mamba
+install --strict-channel-priority -c http://localhost:8000/get/channel0 -
+c conda-forge xtensor ``` Output: ```text ... Package Version Build Channel
+Size
 âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ
 Install:
 âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ
 xtensor 0.16.1 0 http://localhost:8000/get/channel0/osx-64 109 KB xtl 0.4.16
 h04f5b5a_1000 conda-forge/osx-64 47 KB Summary: Install: 2 packages Total
 download: 156 KB
 âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ
```

### Comparing `quetz-server-0.7.0/quetz_server.egg-info/SOURCES.txt` & `quetz-server-0.8.0/quetz_server.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-.coveragerc
 .flake8
 .pre-commit-config.yaml
 .readthedocs.yml
 CHANGELOG.md
 CONTRIBUTING.md
 Dockerfile
 LICENSE
@@ -11,15 +10,14 @@
 RELEASE.md
 alembic.ini
 dev_config.toml
 docker-compose.yml
 download-test-package.sh
 environment.yml
 init_db.py
-mypy.ini
 pyproject.toml
 setup.cfg
 setup.py
 docker/Dockerfile
 docker/Dockerfile.jupyterhub
 docker/docker_config.toml
 docker/grafana.env
@@ -139,20 +137,22 @@
 quetz/testing/utils.py
 quetz/tests/__init__.py
 quetz/tests/conftest.py
 quetz/tests/test_auth.py
 quetz/tests/test_cli.py
 quetz/tests/test_config.py
 quetz/tests/test_dao.py
+quetz/tests/test_database.py
 quetz/tests/test_db_models.py
 quetz/tests/test_health.py
 quetz/tests/test_indexing.py
 quetz/tests/test_jobs.py
 quetz/tests/test_mirror.py
 quetz/tests/test_pkg_stores.py
+quetz/tests/test_profiling.py
 quetz/tests/test_tasks.py
 quetz/tests/test_versionorder.py
 quetz/tests/test_workers.py
 quetz/tests/api/__init__.py
 quetz/tests/api/conftest.py
 quetz/tests/api/test_api_keys.py
 quetz/tests/api/test_channels.py
```

### Comparing `quetz-server-0.7.0/quetz_server.egg-info/requires.txt` & `quetz-server-0.8.0/quetz_server.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `quetz-server-0.7.0/setup.cfg` & `quetz-server-0.8.0/setup.cfg`

 * *Files identical despite different names*

