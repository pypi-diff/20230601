# Comparing `tmp/FastAPI-JSONAPI-0.2.2.tar.gz` & `tmp/FastAPI-JSONAPI-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FastAPI-JSONAPI-0.2.2.tar", last modified: Sat Mar 11 14:07:06 2023, max compression
+gzip compressed data, was "FastAPI-JSONAPI-1.0.0.tar", last modified: Thu Jun  1 15:49:43 2023, max compression
```

## Comparing `FastAPI-JSONAPI-0.2.2.tar` & `FastAPI-JSONAPI-1.0.0.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 14:07:06.568017 FastAPI-JSONAPI-0.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 14:07:06.560017 FastAPI-JSONAPI-0.2.2/FastAPI_JSONAPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-03-11 14:07:06.000000 FastAPI-JSONAPI-0.2.2/FastAPI_JSONAPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-03-11 14:07:06.000000 FastAPI-JSONAPI-0.2.2/FastAPI_JSONAPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-11 14:07:06.000000 FastAPI-JSONAPI-0.2.2/FastAPI_JSONAPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-11 14:07:06.000000 FastAPI-JSONAPI-0.2.2/FastAPI_JSONAPI.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-03-11 14:07:06.000000 FastAPI-JSONAPI-0.2.2/FastAPI_JSONAPI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-11 14:07:06.000000 FastAPI-JSONAPI-0.2.2/FastAPI_JSONAPI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-03-11 14:07:06.568017 FastAPI-JSONAPI-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 14:07:06.560017 FastAPI-JSONAPI-0.2.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 14:07:06.560017 FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 14:07:06.560017 FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/api/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/api/user.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/asgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 14:07:06.560017 FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/extensions/sqlalchemy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 14:07:06.560017 FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 14:07:06.564017 FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/helpers/factories/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/helpers/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/helpers/factories/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/helpers/factories/faker.py
--rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/helpers/factories/meta_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/helpers/factories/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 14:07:06.564017 FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/helpers/updaters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/helpers/updaters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/helpers/updaters/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/helpers/updaters/meta_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/helpers/updaters/update_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 14:07:06.564017 FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/models/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/models/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 14:07:06.564017 FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/models/pydantic/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/models/pydantic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/models/pydantic/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 14:07:06.564017 FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/models/sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/models/sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/models/sqlalchemy/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 14:07:06.564017 FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 14:07:06.564017 FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/utils/sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/utils/sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/utils/sqlalchemy/base_model_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 14:07:06.564017 FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/utils/sqlalchemy/fields/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/utils/sqlalchemy/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/utils/sqlalchemy/fields/enum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 14:07:06.564017 FastAPI-JSONAPI-0.2.2/examples/api_for_tortoise_orm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/examples/api_for_tortoise_orm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 14:07:06.564017 FastAPI-JSONAPI-0.2.2/examples/api_for_tortoise_orm/api/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/examples/api_for_tortoise_orm/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/examples/api_for_tortoise_orm/api/user.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/examples/api_for_tortoise_orm/asgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 14:07:06.564017 FastAPI-JSONAPI-0.2.2/examples/api_for_tortoise_orm/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/examples/api_for_tortoise_orm/helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 14:07:06.564017 FastAPI-JSONAPI-0.2.2/examples/api_for_tortoise_orm/helpers/factories/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/examples/api_for_tortoise_orm/helpers/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/examples/api_for_tortoise_orm/helpers/factories/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/examples/api_for_tortoise_orm/helpers/factories/faker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/examples/api_for_tortoise_orm/helpers/factories/meta_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/examples/api_for_tortoise_orm/helpers/factories/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 14:07:06.564017 FastAPI-JSONAPI-0.2.2/examples/api_for_tortoise_orm/helpers/updaters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/examples/api_for_tortoise_orm/helpers/updaters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/examples/api_for_tortoise_orm/helpers/updaters/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/examples/api_for_tortoise_orm/helpers/updaters/meta_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/examples/api_for_tortoise_orm/helpers/updaters/update_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/examples/api_for_tortoise_orm/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 14:07:06.564017 FastAPI-JSONAPI-0.2.2/examples/api_for_tortoise_orm/models/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/examples/api_for_tortoise_orm/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/examples/api_for_tortoise_orm/models/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 14:07:06.564017 FastAPI-JSONAPI-0.2.2/examples/api_for_tortoise_orm/models/pydantic/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/examples/api_for_tortoise_orm/models/pydantic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/examples/api_for_tortoise_orm/models/pydantic/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 14:07:06.564017 FastAPI-JSONAPI-0.2.2/examples/api_for_tortoise_orm/models/tortoise/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/examples/api_for_tortoise_orm/models/tortoise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/examples/api_for_tortoise_orm/models/tortoise/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/examples/api_for_tortoise_orm/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 14:07:06.568017 FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9952 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 14:07:06.568017 FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/data_layers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/data_layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13474 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/data_layers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/data_layers/data_typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 14:07:06.568017 FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/data_layers/fields/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/data_layers/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/data_layers/fields/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/data_layers/fields/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 14:07:06.568017 FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/data_layers/filtering/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/data_layers/filtering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10033 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/data_layers/filtering/sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/data_layers/filtering/tortoise_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/data_layers/filtering/tortoise_orm.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/data_layers/orm.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/data_layers/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 14:07:06.568017 FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/data_layers/sorting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/data_layers/sorting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/data_layers/sorting/sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/data_layers/sorting/tortoise_orm.py
--rw-r--r--   0 runner    (1001) docker     (123)    23495 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/data_layers/sqlalchemy_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    17518 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/data_layers/tortoise_orm_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 14:07:06.568017 FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/exceptions/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/exceptions/json_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/jsonapi_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)    14120 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/openapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     9616 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/querystring.py
--rw-r--r--   0 runner    (1001) docker     (123)     7331 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/signature.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-11 14:07:06.568017 FastAPI-JSONAPI-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 14:07:06.560017 FastAPI-JSONAPI-0.2.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 14:07:06.568017 FastAPI-JSONAPI-0.2.2/tests/misc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/tests/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-03-11 14:06:52.000000 FastAPI-JSONAPI-0.2.2/tests/misc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.422194 FastAPI-JSONAPI-1.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.414194 FastAPI-JSONAPI-1.0.0/FastAPI_JSONAPI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-06-01 15:49:43.000000 FastAPI-JSONAPI-1.0.0/FastAPI_JSONAPI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-06-01 15:49:43.000000 FastAPI-JSONAPI-1.0.0/FastAPI_JSONAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 15:49:43.000000 FastAPI-JSONAPI-1.0.0/FastAPI_JSONAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 15:49:43.000000 FastAPI-JSONAPI-1.0.0/FastAPI_JSONAPI.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-01 15:49:43.000000 FastAPI-JSONAPI-1.0.0/FastAPI_JSONAPI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-01 15:49:43.000000 FastAPI-JSONAPI-1.0.0/FastAPI_JSONAPI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-06-01 15:49:43.422194 FastAPI-JSONAPI-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.414194 FastAPI-JSONAPI-1.0.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.414194 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.414194 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/asgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.414194 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/extensions/sqlalchemy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.414194 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.414194 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/helpers/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/helpers/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/helpers/factories/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/helpers/factories/faker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/helpers/factories/meta_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/helpers/factories/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.414194 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/helpers/updaters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/helpers/updaters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/helpers/updaters/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/helpers/updaters/meta_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/helpers/updaters/update_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.414194 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/models/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.414194 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/models/pydantic/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/models/pydantic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/models/pydantic/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.414194 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/models/sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/models/sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/models/sqlalchemy/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.418194 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.418194 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/utils/sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/utils/sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/utils/sqlalchemy/base_model_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.418194 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/utils/sqlalchemy/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/utils/sqlalchemy/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/utils/sqlalchemy/fields/enum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.418194 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.418194 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/asgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.418194 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.418194 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/helpers/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/helpers/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/helpers/factories/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/helpers/factories/faker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/helpers/factories/meta_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/helpers/factories/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.418194 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/helpers/updaters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/helpers/updaters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/helpers/updaters/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/helpers/updaters/meta_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/helpers/updaters/update_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.418194 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/models/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.418194 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/models/pydantic/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/models/pydantic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/models/pydantic/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.418194 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/models/tortoise/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/models/tortoise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/models/tortoise/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.418194 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9952 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.418194 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13474 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/data_typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.418194 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/fields/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/fields/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.418194 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/filtering/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/filtering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10033 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/filtering/sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/filtering/tortoise_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/filtering/tortoise_orm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/orm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.422194 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/sorting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/sorting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/sorting/sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/sorting/tortoise_orm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23495 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/sqlalchemy_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17518 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/tortoise_orm_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.422194 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/exceptions/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/exceptions/json_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/jsonapi_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14120 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9616 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/querystring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7331 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-01 15:49:43.422194 FastAPI-JSONAPI-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.410194 FastAPI-JSONAPI-1.0.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:43.422194 FastAPI-JSONAPI-1.0.0/tests/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/tests/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-01 15:49:33.000000 FastAPI-JSONAPI-1.0.0/tests/misc/utils.py
```

### Comparing `FastAPI-JSONAPI-0.2.2/FastAPI_JSONAPI.egg-info/PKG-INFO` & `FastAPI-JSONAPI-1.0.0/FastAPI_JSONAPI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FastAPI-JSONAPI
-Version: 0.2.2
+Version: 1.0.0
 Summary: FastAPI extension to create REST web api according to JSON:API 1.0 specification with FastAPI, Pydantic and data provider of your choice (SQLAlchemy, Tortoise ORM)
 Home-page: https://github.com/mts-ai/FastAPI-JSONAPI
 Author: Team MTS AI
 Author-email: a.nekrasov@mts.ru
 License: MIT
 Keywords: fastapi jsonapi mts ai
 Platform: any
```

### Comparing `FastAPI-JSONAPI-0.2.2/FastAPI_JSONAPI.egg-info/SOURCES.txt` & `FastAPI-JSONAPI-1.0.0/FastAPI_JSONAPI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-0.2.2/LICENSE` & `FastAPI-JSONAPI-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-0.2.2/PKG-INFO` & `FastAPI-JSONAPI-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FastAPI-JSONAPI
-Version: 0.2.2
+Version: 1.0.0
 Summary: FastAPI extension to create REST web api according to JSON:API 1.0 specification with FastAPI, Pydantic and data provider of your choice (SQLAlchemy, Tortoise ORM)
 Home-page: https://github.com/mts-ai/FastAPI-JSONAPI
 Author: Team MTS AI
 Author-email: a.nekrasov@mts.ru
 License: MIT
 Keywords: fastapi jsonapi mts ai
 Platform: any
```

### Comparing `FastAPI-JSONAPI-0.2.2/README.md` & `FastAPI-JSONAPI-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/api/user.py` & `FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/api/user.py`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/extensions/sqlalchemy.py` & `FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/extensions/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/helpers/factories/exceptions.py` & `FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/helpers/factories/exceptions.py`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/helpers/factories/meta_base.py` & `FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/helpers/factories/meta_base.py`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/helpers/factories/user.py` & `FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/helpers/factories/user.py`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/helpers/updaters/exceptions.py` & `FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/helpers/updaters/exceptions.py`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/helpers/updaters/meta_base.py` & `FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/helpers/updaters/meta_base.py`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/helpers/updaters/update_user.py` & `FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/helpers/updaters/update_user.py`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/main.py` & `FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/main.py`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/models/pydantic/user.py` & `FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/models/pydantic/user.py`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/models/sqlalchemy/user.py` & `FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/models/sqlalchemy/user.py`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/urls.py` & `FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/urls.py`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/utils/sqlalchemy/base_model_mixin.py` & `FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/utils/sqlalchemy/base_model_mixin.py`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-0.2.2/examples/api_for_sqlalchemy/utils/sqlalchemy/fields/enum.py` & `FastAPI-JSONAPI-1.0.0/examples/api_for_sqlalchemy/utils/sqlalchemy/fields/enum.py`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-0.2.2/examples/api_for_tortoise_orm/api/user.py` & `FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/api/user.py`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-0.2.2/examples/api_for_tortoise_orm/helpers/factories/exceptions.py` & `FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/helpers/factories/exceptions.py`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-0.2.2/examples/api_for_tortoise_orm/helpers/factories/meta_base.py` & `FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/helpers/factories/meta_base.py`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-0.2.2/examples/api_for_tortoise_orm/helpers/factories/user.py` & `FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/helpers/factories/user.py`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-0.2.2/examples/api_for_tortoise_orm/helpers/updaters/exceptions.py` & `FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/helpers/updaters/exceptions.py`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-0.2.2/examples/api_for_tortoise_orm/helpers/updaters/meta_base.py` & `FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/helpers/updaters/meta_base.py`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-0.2.2/examples/api_for_tortoise_orm/helpers/updaters/update_user.py` & `FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/helpers/updaters/update_user.py`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-0.2.2/examples/api_for_tortoise_orm/main.py` & `FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/main.py`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-0.2.2/examples/api_for_tortoise_orm/models/pydantic/user.py` & `FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/models/pydantic/user.py`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-0.2.2/examples/api_for_tortoise_orm/models/tortoise/user.py` & `FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/models/tortoise/user.py`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-0.2.2/examples/api_for_tortoise_orm/urls.py` & `FastAPI-JSONAPI-1.0.0/examples/api_for_tortoise_orm/urls.py`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/api.py` & `FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/api.py`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/data_layers/base.py` & `FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/base.py`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/data_layers/fields/mixins.py` & `FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/fields/mixins.py`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/data_layers/filtering/sqlalchemy.py` & `FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/filtering/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/data_layers/filtering/tortoise_operation.py` & `FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/filtering/tortoise_operation.py`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/data_layers/filtering/tortoise_orm.py` & `FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/filtering/tortoise_orm.py`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/data_layers/shared.py` & `FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/shared.py`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/data_layers/sorting/sqlalchemy.py` & `FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/sorting/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/data_layers/sorting/tortoise_orm.py` & `FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/sorting/tortoise_orm.py`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/data_layers/sqlalchemy_engine.py` & `FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/sqlalchemy_engine.py`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/data_layers/tortoise_orm_engine.py` & `FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/data_layers/tortoise_orm_engine.py`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/exceptions/__init__.py` & `FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/exceptions/base.py` & `FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/exceptions/base.py`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/exceptions/json_api.py` & `FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/exceptions/json_api.py`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/methods.py` & `FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/methods.py`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/openapi.py` & `FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/openapi.py`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/querystring.py` & `FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/querystring.py`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/schema.py` & `FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/schema.py`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-0.2.2/fastapi_jsonapi/signature.py` & `FastAPI-JSONAPI-1.0.0/fastapi_jsonapi/signature.py`

 * *Files identical despite different names*

### Comparing `FastAPI-JSONAPI-0.2.2/setup.py` & `FastAPI-JSONAPI-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from setuptools import setup, find_packages
 
-__version__ = "0.2.2"
+__version__ = "1.0.0"
 
 
 requirements_filepath = os.path.join(os.path.dirname(__name__), "requirements.txt")
 readme_filepath = os.path.join(os.path.dirname(__name__), "README.md")
 with open(requirements_filepath) as fp:
     install_requires = fp.read()
```

