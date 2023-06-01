# Comparing `tmp/cdktf-cdktf-provider-postgresql-6.0.0.tar.gz` & `tmp/cdktf-cdktf-provider-postgresql-6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-postgresql-6.0.0.tar", last modified: Tue Apr 18 21:28:20 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-postgresql-6.0.1.tar", last modified: Thu Jun  1 14:30:53 2023, max compression
```

## Comparing `cdktf-cdktf-provider-postgresql-6.0.0.tar` & `cdktf-cdktf-provider-postgresql-6.0.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:28:20.214242 cdktf-cdktf-provider-postgresql-6.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-04-18 21:28:05.000000 cdktf-cdktf-provider-postgresql-6.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-18 21:28:05.000000 cdktf-cdktf-provider-postgresql-6.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-04-18 21:28:20.214242 cdktf-cdktf-provider-postgresql-6.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-04-18 21:28:05.000000 cdktf-cdktf-provider-postgresql-6.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-18 21:28:05.000000 cdktf-cdktf-provider-postgresql-6.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 21:28:20.214242 cdktf-cdktf-provider-postgresql-6.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-04-18 21:28:05.000000 cdktf-cdktf-provider-postgresql-6.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:28:20.206241 cdktf-cdktf-provider-postgresql-6.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:28:20.210241 cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-18 21:28:05.000000 cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:28:20.210241 cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-18 21:28:05.000000 cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   521780 2023-04-18 21:28:05.000000 cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/_jsii/provider-postgresql@6.0.0.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:28:20.210241 cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/data_postgresql_schemas/
--rw-r--r--   0 runner    (1001) docker     (123)    34317 2023-04-18 21:28:05.000000 cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/data_postgresql_schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:28:20.214242 cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/data_postgresql_sequences/
--rw-r--r--   0 runner    (1001) docker     (123)    43102 2023-04-18 21:28:05.000000 cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/data_postgresql_sequences/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:28:20.214242 cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/data_postgresql_tables/
--rw-r--r--   0 runner    (1001) docker     (123)    45760 2023-04-18 21:28:05.000000 cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/data_postgresql_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:28:20.214242 cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/database/
--rw-r--r--   0 runner    (1001) docker     (123)    41869 2023-04-18 21:28:05.000000 cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/database/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:28:20.214242 cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/default_privileges/
--rw-r--r--   0 runner    (1001) docker     (123)    33200 2023-04-18 21:28:05.000000 cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/default_privileges/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:28:20.214242 cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/extension/
--rw-r--r--   0 runner    (1001) docker     (123)    31436 2023-04-18 21:28:05.000000 cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/extension/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:28:20.214242 cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/function_resource/
--rw-r--r--   0 runner    (1001) docker     (123)    54689 2023-04-18 21:28:05.000000 cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/function_resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:28:20.214242 cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/grant/
--rw-r--r--   0 runner    (1001) docker     (123)    35689 2023-04-18 21:28:05.000000 cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/grant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:28:20.214242 cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/grant_role/
--rw-r--r--   0 runner    (1001) docker     (123)    23253 2023-04-18 21:28:05.000000 cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/grant_role/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:28:20.214242 cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/physical_replication_slot/
--rw-r--r--   0 runner    (1001) docker     (123)    17945 2023-04-18 21:28:05.000000 cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/physical_replication_slot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:28:20.214242 cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/provider/
--rw-r--r--   0 runner    (1001) docker     (123)    57620 2023-04-18 21:28:05.000000 cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/provider/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:28:20.214242 cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/publication/
--rw-r--r--   0 runner    (1001) docker     (123)    38127 2023-04-18 21:28:05.000000 cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/publication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 21:28:05.000000 cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:28:20.214242 cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/replication_slot/
--rw-r--r--   0 runner    (1001) docker     (123)    22283 2023-04-18 21:28:05.000000 cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/replication_slot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:28:20.214242 cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/role/
--rw-r--r--   0 runner    (1001) docker     (123)    73740 2023-04-18 21:28:05.000000 cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/role/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:28:20.214242 cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/schema/
--rw-r--r--   0 runner    (1001) docker     (123)    54800 2023-04-18 21:28:05.000000 cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:28:20.214242 cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/server/
--rw-r--r--   0 runner    (1001) docker     (123)    34546 2023-04-18 21:28:05.000000 cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:28:20.214242 cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/subscription/
--rw-r--r--   0 runner    (1001) docker     (123)    31163 2023-04-18 21:28:05.000000 cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/subscription/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:28:20.214242 cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/user_mapping/
--rw-r--r--   0 runner    (1001) docker     (123)    24312 2023-04-18 21:28:05.000000 cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/user_mapping/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:28:20.210241 cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-04-18 21:28:20.000000 cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-18 21:28:20.000000 cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 21:28:20.000000 cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-18 21:28:20.000000 cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-18 21:28:20.000000 cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:30:53.081448 cdktf-cdktf-provider-postgresql-6.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-01 14:30:41.000000 cdktf-cdktf-provider-postgresql-6.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 14:30:41.000000 cdktf-cdktf-provider-postgresql-6.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-06-01 14:30:53.081448 cdktf-cdktf-provider-postgresql-6.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-06-01 14:30:41.000000 cdktf-cdktf-provider-postgresql-6.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-01 14:30:41.000000 cdktf-cdktf-provider-postgresql-6.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 14:30:53.081448 cdktf-cdktf-provider-postgresql-6.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-06-01 14:30:41.000000 cdktf-cdktf-provider-postgresql-6.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:30:53.073448 cdktf-cdktf-provider-postgresql-6.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:30:53.077448 cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-06-01 14:30:41.000000 cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:30:53.077448 cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-01 14:30:41.000000 cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   134146 2023-06-01 14:30:41.000000 cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/_jsii/provider-postgresql@6.0.1.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:30:53.077448 cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/data_postgresql_schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)    34317 2023-06-01 14:30:41.000000 cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/data_postgresql_schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:30:53.077448 cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/data_postgresql_sequences/
+-rw-r--r--   0 runner    (1001) docker     (123)    43102 2023-06-01 14:30:41.000000 cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/data_postgresql_sequences/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:30:53.077448 cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/data_postgresql_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)    45760 2023-06-01 14:30:41.000000 cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/data_postgresql_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:30:53.077448 cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/database/
+-rw-r--r--   0 runner    (1001) docker     (123)    41869 2023-06-01 14:30:41.000000 cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/database/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:30:53.077448 cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/default_privileges/
+-rw-r--r--   0 runner    (1001) docker     (123)    33200 2023-06-01 14:30:41.000000 cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/default_privileges/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:30:53.077448 cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/extension/
+-rw-r--r--   0 runner    (1001) docker     (123)    31436 2023-06-01 14:30:41.000000 cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/extension/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:30:53.077448 cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/function_resource/
+-rw-r--r--   0 runner    (1001) docker     (123)    54689 2023-06-01 14:30:41.000000 cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/function_resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:30:53.077448 cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/grant/
+-rw-r--r--   0 runner    (1001) docker     (123)    35689 2023-06-01 14:30:41.000000 cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/grant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:30:53.077448 cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/grant_role/
+-rw-r--r--   0 runner    (1001) docker     (123)    23253 2023-06-01 14:30:41.000000 cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/grant_role/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:30:53.077448 cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/physical_replication_slot/
+-rw-r--r--   0 runner    (1001) docker     (123)    17945 2023-06-01 14:30:41.000000 cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/physical_replication_slot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:30:53.077448 cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)    57620 2023-06-01 14:30:41.000000 cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/provider/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:30:53.077448 cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/publication/
+-rw-r--r--   0 runner    (1001) docker     (123)    38127 2023-06-01 14:30:41.000000 cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/publication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:30:41.000000 cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:30:53.077448 cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/replication_slot/
+-rw-r--r--   0 runner    (1001) docker     (123)    22283 2023-06-01 14:30:41.000000 cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/replication_slot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:30:53.077448 cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/role/
+-rw-r--r--   0 runner    (1001) docker     (123)    73740 2023-06-01 14:30:41.000000 cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/role/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:30:53.077448 cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)    54800 2023-06-01 14:30:41.000000 cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:30:53.077448 cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/server/
+-rw-r--r--   0 runner    (1001) docker     (123)    34546 2023-06-01 14:30:41.000000 cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:30:53.077448 cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/subscription/
+-rw-r--r--   0 runner    (1001) docker     (123)    31163 2023-06-01 14:30:41.000000 cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/subscription/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:30:53.081448 cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/user_mapping/
+-rw-r--r--   0 runner    (1001) docker     (123)    24312 2023-06-01 14:30:41.000000 cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/user_mapping/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:30:53.077448 cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-06-01 14:30:53.000000 cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-01 14:30:53.000000 cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:30:53.000000 cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-01 14:30:53.000000 cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-01 14:30:53.000000 cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-postgresql-6.0.0/LICENSE` & `cdktf-cdktf-provider-postgresql-6.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-postgresql-6.0.0/PKG-INFO` & `cdktf-cdktf-provider-postgresql-6.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-postgresql
-Version: 6.0.0
+Version: 6.0.1
 Summary: Prebuilt postgresql Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-postgresql.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-postgresql.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -79,15 +79,17 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform postgresql Provider version 1:1. In fact, it always tracks `latest` of `~> 1.14` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [Terraform CDK](https://cdk.tf)
-* [Terraform postgresql Provider](https://github.com/terraform-providers/terraform-provider-postgresql)
+* [Terraform postgresql Provider](https://registry.terraform.io/providers/cyrilgdn/postgresql/1.14.0)
+
+  * This links to the minimum version being tracked, you can find the latest released version [in our releases](https://github.com/cdktf/cdktf-provider-postgresql/releases)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [terraform cdk](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-postgresql-6.0.0/README.md` & `cdktf-cdktf-provider-postgresql-6.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -55,15 +55,17 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform postgresql Provider version 1:1. In fact, it always tracks `latest` of `~> 1.14` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [Terraform CDK](https://cdk.tf)
-* [Terraform postgresql Provider](https://github.com/terraform-providers/terraform-provider-postgresql)
+* [Terraform postgresql Provider](https://registry.terraform.io/providers/cyrilgdn/postgresql/1.14.0)
+
+  * This links to the minimum version being tracked, you can find the latest released version [in our releases](https://github.com/cdktf/cdktf-provider-postgresql/releases)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [terraform cdk](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-postgresql-6.0.0/setup.py` & `cdktf-cdktf-provider-postgresql-6.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-postgresql",
-    "version": "6.0.0",
+    "version": "6.0.1",
     "description": "Prebuilt postgresql Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-postgresql.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -40,25 +40,25 @@
         "cdktf_cdktf_provider_postgresql.schema",
         "cdktf_cdktf_provider_postgresql.server",
         "cdktf_cdktf_provider_postgresql.subscription",
         "cdktf_cdktf_provider_postgresql.user_mapping"
     ],
     "package_data": {
         "cdktf_cdktf_provider_postgresql._jsii": [
-            "provider-postgresql@6.0.0.jsii.tgz"
+            "provider-postgresql@6.0.1.jsii.tgz"
         ],
         "cdktf_cdktf_provider_postgresql": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "cdktf>=0.16.0, <0.17.0",
+        "cdktf>=0.16.3, <0.17.0",
         "constructs>=10.0.0, <11.0.0",
-        "jsii>=1.80.0, <2.0.0",
+        "jsii>=1.81.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/__init__.py` & `cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,15 +56,17 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform postgresql Provider version 1:1. In fact, it always tracks `latest` of `~> 1.14` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [Terraform CDK](https://cdk.tf)
-* [Terraform postgresql Provider](https://github.com/terraform-providers/terraform-provider-postgresql)
+* [Terraform postgresql Provider](https://registry.terraform.io/providers/cyrilgdn/postgresql/1.14.0)
+
+  * This links to the minimum version being tracked, you can find the latest released version [in our releases](https://github.com/cdktf/cdktf-provider-postgresql/releases)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [terraform cdk](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/data_postgresql_schemas/__init__.py` & `cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/data_postgresql_schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/data_postgresql_sequences/__init__.py` & `cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/data_postgresql_sequences/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/data_postgresql_tables/__init__.py` & `cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/data_postgresql_tables/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/database/__init__.py` & `cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/database/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/default_privileges/__init__.py` & `cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/default_privileges/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/extension/__init__.py` & `cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/extension/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/function_resource/__init__.py` & `cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/function_resource/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/grant/__init__.py` & `cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/grant/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/grant_role/__init__.py` & `cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/grant_role/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/physical_replication_slot/__init__.py` & `cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/physical_replication_slot/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/provider/__init__.py` & `cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/publication/__init__.py` & `cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/publication/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/replication_slot/__init__.py` & `cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/replication_slot/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/role/__init__.py` & `cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/role/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/schema/__init__.py` & `cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/server/__init__.py` & `cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/server/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/subscription/__init__.py` & `cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/subscription/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql/user_mapping/__init__.py` & `cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql/user_mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql.egg-info/PKG-INFO` & `cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-postgresql
-Version: 6.0.0
+Version: 6.0.1
 Summary: Prebuilt postgresql Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-postgresql.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-postgresql.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -79,15 +79,17 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform postgresql Provider version 1:1. In fact, it always tracks `latest` of `~> 1.14` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [Terraform CDK](https://cdk.tf)
-* [Terraform postgresql Provider](https://github.com/terraform-providers/terraform-provider-postgresql)
+* [Terraform postgresql Provider](https://registry.terraform.io/providers/cyrilgdn/postgresql/1.14.0)
+
+  * This links to the minimum version being tracked, you can find the latest released version [in our releases](https://github.com/cdktf/cdktf-provider-postgresql/releases)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [terraform cdk](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-postgresql-6.0.0/src/cdktf_cdktf_provider_postgresql.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-postgresql-6.0.1/src/cdktf_cdktf_provider_postgresql.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/cdktf_cdktf_provider_postgresql/py.typed
 src/cdktf_cdktf_provider_postgresql.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_postgresql.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_postgresql.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_postgresql.egg-info/requires.txt
 src/cdktf_cdktf_provider_postgresql.egg-info/top_level.txt
 src/cdktf_cdktf_provider_postgresql/_jsii/__init__.py
-src/cdktf_cdktf_provider_postgresql/_jsii/provider-postgresql@6.0.0.jsii.tgz
+src/cdktf_cdktf_provider_postgresql/_jsii/provider-postgresql@6.0.1.jsii.tgz
 src/cdktf_cdktf_provider_postgresql/data_postgresql_schemas/__init__.py
 src/cdktf_cdktf_provider_postgresql/data_postgresql_sequences/__init__.py
 src/cdktf_cdktf_provider_postgresql/data_postgresql_tables/__init__.py
 src/cdktf_cdktf_provider_postgresql/database/__init__.py
 src/cdktf_cdktf_provider_postgresql/default_privileges/__init__.py
 src/cdktf_cdktf_provider_postgresql/extension/__init__.py
 src/cdktf_cdktf_provider_postgresql/function_resource/__init__.py
```

