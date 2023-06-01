# Comparing `tmp/resilient_sdk-48.2.4321.tar.gz` & `tmp/resilient_sdk-49.0.4423.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resilient_sdk-48.2.4321.tar", last modified: Fri May  5 12:35:37 2023, max compression
+gzip compressed data, was "resilient_sdk-49.0.4423.tar", last modified: Thu Jun  1 15:59:18 2023, max compression
```

## Comparing `resilient_sdk-48.2.4321.tar` & `resilient_sdk-49.0.4423.tar`

### file list

```diff
@@ -1,256 +1,258 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.939470 resilient_sdk-48.2.4321/
--rw-rw-r--   0 travis    (2000) travis    (2000)     8523 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/CHANGES
--rw-rw-r--   0 travis    (2000) travis    (2000)     3152 2023-05-05 12:35:37.939470 resilient_sdk-48.2.4321/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     2385 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.619470 resilient_sdk-48.2.4321/assets/
--rwxrwxr-x   0 travis    (2000) travis    (2000)    62353 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/assets/IBM_Security_lockup_pos_RGB.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      441 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/pyproject.toml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.619470 resilient_sdk-48.2.4321/resilient_sdk/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1057 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      105 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6354 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/app.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.619470 resilient_sdk-48.2.4321/resilient_sdk/cmds/
--rw-rw-r--   0 travis    (2000) travis    (2000)      507 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/cmds/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8183 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/cmds/base_cmd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    36429 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/cmds/clone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35393 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/cmds/codegen.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10010 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/cmds/dev.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21294 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/cmds/docgen.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.619470 resilient_sdk-48.2.4321/resilient_sdk/cmds/ext/
--rw-rw-r--   0 travis    (2000) travis    (2000)      105 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/cmds/ext/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8445 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/cmds/ext/ext_package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7602 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/cmds/extract.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5757 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/cmds/run_init.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    48148 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/cmds/validate.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.615470 resilient_sdk-48.2.4321/resilient_sdk/data/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.611470 resilient_sdk-48.2.4321/resilient_sdk/data/codegen/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.611470 resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.623470 resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2853 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/Dockerfile.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)      454 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/MANIFEST.in.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)      342 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/README.md.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)     1687 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/apikey_permissions.txt.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.623470 resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)      534 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/data/workflow.md.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.611470 resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/doc/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.623470 resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/doc/screenshots/
--rw-rw-r--   0 travis    (2000) travis    (2000)   111993 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/doc/screenshots/main.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      743 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/entrypoint.sh.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.623470 resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/package/
--rw-rw-r--   0 travis    (2000) travis    (2000)       19 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/package/LICENSE.jinja2
--rwxrwxr-x   0 travis    (2000) travis    (2000)      145 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/package/__init__.py.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.623470 resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/package/components/
--rwxrwxr-x   0 travis    (2000) travis    (2000)        1 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/package/components/__init__.py.jinja2
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3082 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/package/components/atomic_function.py.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.623470 resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/package/lib/
--rwxrwxr-x   0 travis    (2000) travis    (2000)        1 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/package/lib/__init__.py.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)     7886 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/package/lib/app_common.py.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.623470 resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/package/poller/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/package/poller/__init__.py.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.623470 resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/package/poller/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)      497 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/package/poller/data/soar_close_case.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)     2976 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/package/poller/data/soar_create_case.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)      351 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/package/poller/data/soar_update_case.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)    10722 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/package/poller/poller.py.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.627470 resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/package/util/
--rwxrwxr-x   0 travis    (2000) travis    (2000)        1 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/package/util/__init__.py.jinja2
--rwxrwxr-x   0 travis    (2000) travis    (2000)      913 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/package/util/config.py.jinja2
--rwxrwxr-x   0 travis    (2000) travis    (2000)     4885 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/package/util/customize.py.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.627470 resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/package/util/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)       33 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/package/util/data/export.res.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)      975 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/package/util/selftest.py.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.615470 resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/payload_samples/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.627470 resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/payload_samples/function_name/
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/payload_samples/function_name/blank.json.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/payload_samples/function_name/mock_json_expectation_fail.json.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/payload_samples/function_name/mock_json_expectation_success.json.jinja2
--rw-rw-r--   0 travis    (2000) travis    (2000)     2018 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/setup.py.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.627470 resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/tests/
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3132 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/tests/test_function.py.jinja2
--rwxrwxr-x   0 travis    (2000) travis    (2000)      750 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/tox.ini.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.615470 resilient_sdk-48.2.4321/resilient_sdk/data/docgen/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.627470 resilient_sdk-48.2.4321/resilient_sdk/data/docgen/templates/
--rw-rw-r--   0 travis    (2000) travis    (2000)    15077 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/data/docgen/templates/README.md.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.615470 resilient_sdk-48.2.4321/resilient_sdk/data/ext/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.627470 resilient_sdk-48.2.4321/resilient_sdk/data/ext/icons/
--rw-rw-r--   0 travis    (2000) travis    (2000)    45545 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/data/ext/icons/app_logo.png
--rw-rw-r--   0 travis    (2000) travis    (2000)     3414 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/data/ext/icons/company_logo.png
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.627470 resilient_sdk-48.2.4321/resilient_sdk/data/run_init/
--rw-rw-r--   0 travis    (2000) travis    (2000)      773 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/data/run_init/sdk_settings.json.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.627470 resilient_sdk-48.2.4321/resilient_sdk/data/validate/
--rw-rw-r--   0 travis    (2000) travis    (2000)    18106 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/data/validate/.pylintrc
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.627470 resilient_sdk-48.2.4321/resilient_sdk/data/validate/templates/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4979 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/data/validate/templates/validate_report.md.jinja2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.631470 resilient_sdk-48.2.4321/resilient_sdk/util/
--rw-rw-r--   0 travis    (2000) travis    (2000)      105 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/util/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8225 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/util/constants.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3006 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/util/jinja2_filters.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    53165 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/util/package_file_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2464 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/util/resilient_objects.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1243 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/util/sdk_argparse.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      817 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/util/sdk_exception.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3168 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/util/sdk_genson_overwrites.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    58615 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/util/sdk_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    28324 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/util/sdk_validate_configs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    86171 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/util/sdk_validate_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3388 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/resilient_sdk/util/sdk_validate_issue.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.619470 resilient_sdk-48.2.4321/resilient_sdk.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3152 2023-05-05 12:35:37.000000 resilient_sdk-48.2.4321/resilient_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    15575 2023-05-05 12:35:37.000000 resilient_sdk-48.2.4321/resilient_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-05-05 12:35:37.000000 resilient_sdk-48.2.4321/resilient_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       57 2023-05-05 12:35:37.000000 resilient_sdk-48.2.4321/resilient_sdk.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      108 2023-05-05 12:35:37.000000 resilient_sdk-48.2.4321/resilient_sdk.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       14 2023-05-05 12:35:37.000000 resilient_sdk-48.2.4321/resilient_sdk.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1171 2023-05-05 12:35:37.939470 resilient_sdk-48.2.4321/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      183 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.631470 resilient_sdk-48.2.4321/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16619 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/conftest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3772 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/helpers.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.631470 resilient_sdk-48.2.4321/tests/integration/
--rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/integration/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1227 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/integration/test_installation.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.635470 resilient_sdk-48.2.4321/tests/shared_mock_data/
--rw-rw-r--   0 travis    (2000) travis    (2000)      806 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/.mock_sdk_settings.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        3 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      274 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock.zip
--rw-rw-r--   0 travis    (2000) travis    (2000)    24687 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_app.log
--rw-rw-r--   0 travis    (2000) travis    (2000)      292 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_data.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   224427 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_export.res
--rw-rw-r--   0 travis    (2000) travis    (2000)    58851 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_export.resz
--rw-rw-r--   0 travis    (2000) travis    (2000)   223680 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_export_corrupt.res
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.639470 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/
--rw-rw-r--   0 travis    (2000) travis    (2000)      627 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    57247 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/customize.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   191223 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/customize_old.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.639470 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_app_zip_files/
--rw-rw-r--   0 travis    (2000) travis    (2000)    66751 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_app.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    41671 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_export.res
--rw-rw-r--   0 travis    (2000) travis    (2000)    41951 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_with_payload_samples_export.res
--rw-rw-r--   0 travis    (2000) travis    (2000)     2773 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_customize_w_playbook.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   539154 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_export_w_playbook.res
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.615470 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.671470 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2604 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/Dockerfile
--rw-rw-r--   0 travis    (2000) travis    (2000)      214 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     5843 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     1619 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/apikey_permissions.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.671470 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)      712 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/wf_mock_workflow_one.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     1196 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/wf_mock_workflow_two.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.615470 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/doc/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.671470 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/doc/screenshots/
--rw-rw-r--   0 travis    (2000) travis    (2000)   111993 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/doc/screenshots/main.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      566 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/entrypoint.sh
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.671470 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/
--rw-rw-r--   0 travis    (2000) travis    (2000)       30 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      145 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.675470 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2254 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_a_mock_function_with_no_unicode_characters_in_name.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2061 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function__three.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3465 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function_one.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2355 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function_two.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.675470 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/lib/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/lib/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6889 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/lib/app_common.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.723470 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.727470 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)      497 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/data/soar_close_case.jinja
--rw-rw-r--   0 travis    (2000) travis    (2000)     2976 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/data/soar_create_case.jinja
--rw-rw-r--   0 travis    (2000) travis    (2000)      351 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/data/soar_update_case.jinja
--rw-rw-r--   0 travis    (2000) travis    (2000)    10660 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/poller.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.731470 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      591 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2967 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2967 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165718.bak
--rw-rw-r--   0 travis    (2000) travis    (2000)     2967 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165719.bak
--rw-rw-r--   0 travis    (2000) travis    (2000)     2967 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165720.bak
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.775470 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)    49696 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res
--rw-rw-r--   0 travis    (2000) travis    (2000)    50432 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165718.bak
--rw-rw-r--   0 travis    (2000) travis    (2000)    50432 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165719.bak
--rw-rw-r--   0 travis    (2000) travis    (2000)    50432 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165720.bak
--rw-rw-r--   0 travis    (2000) travis    (2000)      594 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/selftest.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.775470 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/icons/
--rw-rw-r--   0 travis    (2000) travis    (2000)    45545 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/icons/app_logo.png
--rw-rw-r--   0 travis    (2000) travis    (2000)     3414 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/icons/company_logo.png
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.615470 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.775470 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/mock_json_endpoint_fail.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/mock_json_endpoint_success.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/mock_json_expectation_fail.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/mock_json_expectation_success.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/output_json_example.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/output_json_schema.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.835470 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/mock_json_endpoint_fail.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/mock_json_endpoint_success.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/mock_json_expectation_fail.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/mock_json_expectation_success.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/output_json_example.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/output_json_schema.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.835470 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/mock_json_endpoint_fail.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/mock_json_endpoint_success.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/mock_json_expectation_fail.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/mock_json_expectation_success.json
--rw-rw-r--   0 travis    (2000) travis    (2000)       56 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/output_json_example.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/output_json_schema.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.887470 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/mock_json_endpoint_fail.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/mock_json_endpoint_success.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/mock_json_expectation_fail.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/mock_json_expectation_success.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/output_json_example.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/output_json_schema.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     2005 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.887470 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2536 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_a_mock_function_with_no_unicode_characters_in_name.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2325 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function__three.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2684 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function_one.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2381 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function_two.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      741 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tox.ini
--rw-rw-r--   0 travis    (2000) travis    (2000)    53354 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_reload_export_w_playbook.res
--rw-rw-r--   0 travis    (2000) travis    (2000)     2352 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1955 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/setup_callable_data.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1798 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/setup_py_lines.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2795 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_paths.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   413882 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_reload_export.res
--rw-rw-r--   0 travis    (2000) travis    (2000)     1102 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/mock_xml_test_report.xml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.895470 resilient_sdk-48.2.4321/tests/shared_mock_data/resilient_api_data/
--rw-rw-r--   0 travis    (2000) travis    (2000)  3241462 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/resilient_api_data/export-with-playbook.JSON
--rw-rw-r--   0 travis    (2000) travis    (2000)   594886 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/resilient_api_data/export.JSON
--rw-rw-r--   0 travis    (2000) travis    (2000)     1449 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/resilient_api_data/orgs.JSON
--rw-rw-r--   0 travis    (2000) travis    (2000)     2049 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/resilient_api_data/session.JSON
--rw-rw-r--   0 travis    (2000) travis    (2000)     2056 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/shared_mock_data/resilient_api_mock.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.895470 resilient_sdk-48.2.4321/tests/unit/
--rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/unit/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1830 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/unit/test_app.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.895470 resilient_sdk-48.2.4321/tests/unit/test_cmds/
--rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/unit/test_cmds/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.895470 resilient_sdk-48.2.4321/tests/unit/test_cmds/ext/
--rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/unit/test_cmds/ext/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6916 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/unit/test_cmds/ext/test_ext_package.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2070 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/unit/test_cmds/test_base_cmd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20782 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/unit/test_cmds/test_clone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    32212 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/unit/test_cmds/test_codegen.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2736 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/unit/test_cmds/test_dev.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10659 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/unit/test_cmds/test_docgen.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1145 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/unit/test_cmds/test_extract.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5876 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/unit/test_cmds/test_run_init.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23815 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/unit/test_cmds/test_validate.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 12:35:37.939470 resilient_sdk-48.2.4321/tests/unit/test_util/
--rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/unit/test_util/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2148 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/unit/test_util/test_jinja_filters.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18754 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/unit/test_util/test_package_file_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1567 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/unit/test_util/test_resilient_objects.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      470 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/unit/test_util/test_sdk_argparse.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      947 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/unit/test_util/test_sdk_exception.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27286 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/unit/test_util/test_sdk_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3988 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/unit/test_util/test_sdk_validate_configs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    48045 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/unit/test_util/test_sdk_validate_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1623 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tests/unit/test_util/test_sdk_validate_issue.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      943 2023-05-05 12:33:36.000000 resilient_sdk-48.2.4321/tox.ini
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:18.217552 resilient_sdk-49.0.4423/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8830 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/CHANGES
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3152 2023-06-01 15:59:18.217552 resilient_sdk-49.0.4423/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2385 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.897552 resilient_sdk-49.0.4423/assets/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    62353 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/assets/IBM_Security_lockup_pos_RGB.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      441 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/pyproject.toml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.897552 resilient_sdk-49.0.4423/resilient_sdk/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1057 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)      105 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6354 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/app.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.901552 resilient_sdk-49.0.4423/resilient_sdk/cmds/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      507 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/cmds/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8183 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/cmds/base_cmd.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36429 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/cmds/clone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36585 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/cmds/codegen.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10400 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/cmds/dev.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21294 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/cmds/docgen.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.901552 resilient_sdk-49.0.4423/resilient_sdk/cmds/ext/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      105 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/cmds/ext/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8445 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/cmds/ext/ext_package.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7602 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/cmds/extract.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5757 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/cmds/run_init.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48148 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/cmds/validate.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.897552 resilient_sdk-49.0.4423/resilient_sdk/data/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.893552 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.893552 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.901552 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2853 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/Dockerfile.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)      454 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/MANIFEST.in.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)      342 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/README.md.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1687 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/apikey_permissions.txt.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.901552 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1105 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/data/playbook.md.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)      534 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/data/workflow.md.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.897552 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/doc/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.901552 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/doc/screenshots/
+-rw-rw-r--   0 travis    (2000) travis    (2000)   111993 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/doc/screenshots/main.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      743 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/entrypoint.sh.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.901552 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       19 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/LICENSE.jinja2
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      145 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/__init__.py.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.901552 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/components/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)        1 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/components/__init__.py.jinja2
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     3082 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/components/atomic_function.py.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.901552 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/lib/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)        1 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/lib/__init__.py.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7886 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/lib/app_common.py.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.901552 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/poller/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/poller/__init__.py.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.901552 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/poller/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      497 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/poller/data/soar_close_case.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2976 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/poller/data/soar_create_case.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)      351 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/poller/data/soar_update_case.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10768 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/poller/poller.py.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.901552 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/util/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)        1 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/util/__init__.py.jinja2
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      913 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/util/config.py.jinja2
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     4885 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/util/customize.py.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.901552 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/util/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       33 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/util/data/export.res.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)      975 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/util/selftest.py.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.897552 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/payload_samples/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.901552 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/payload_samples/function_name/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/payload_samples/function_name/blank.json.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/payload_samples/function_name/mock_json_expectation_fail.json.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/payload_samples/function_name/mock_json_expectation_success.json.jinja2
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2018 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/setup.py.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.901552 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/tests/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     3132 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/tests/test_function.py.jinja2
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      750 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/tox.ini.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.897552 resilient_sdk-49.0.4423/resilient_sdk/data/docgen/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.905552 resilient_sdk-49.0.4423/resilient_sdk/data/docgen/templates/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15077 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/docgen/templates/README.md.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.897552 resilient_sdk-49.0.4423/resilient_sdk/data/ext/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.905552 resilient_sdk-49.0.4423/resilient_sdk/data/ext/icons/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45545 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/ext/icons/app_logo.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3414 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/ext/icons/company_logo.png
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.905552 resilient_sdk-49.0.4423/resilient_sdk/data/run_init/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      773 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/run_init/sdk_settings.json.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.905552 resilient_sdk-49.0.4423/resilient_sdk/data/validate/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18106 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/validate/.pylintrc
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.905552 resilient_sdk-49.0.4423/resilient_sdk/data/validate/templates/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4979 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/data/validate/templates/validate_report.md.jinja2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.905552 resilient_sdk-49.0.4423/resilient_sdk/util/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      105 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/util/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8225 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/util/constants.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3006 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/util/jinja2_filters.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    53165 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/util/package_file_helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3080 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/util/resilient_objects.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1243 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/util/sdk_argparse.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      817 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/util/sdk_exception.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3168 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/util/sdk_genson_overwrites.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    65385 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/util/sdk_helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28321 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/util/sdk_validate_configs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    86171 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/util/sdk_validate_helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3388 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/resilient_sdk/util/sdk_validate_issue.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.901552 resilient_sdk-49.0.4423/resilient_sdk.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3152 2023-06-01 15:59:17.000000 resilient_sdk-49.0.4423/resilient_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15768 2023-06-01 15:59:17.000000 resilient_sdk-49.0.4423/resilient_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-01 15:59:17.000000 resilient_sdk-49.0.4423/resilient_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       57 2023-06-01 15:59:17.000000 resilient_sdk-49.0.4423/resilient_sdk.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      108 2023-06-01 15:59:17.000000 resilient_sdk-49.0.4423/resilient_sdk.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       14 2023-06-01 15:59:17.000000 resilient_sdk-49.0.4423/resilient_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1171 2023-06-01 15:59:18.221552 resilient_sdk-49.0.4423/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)      183 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.905552 resilient_sdk-49.0.4423/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16904 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/conftest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3772 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/helpers.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.905552 resilient_sdk-49.0.4423/tests/integration/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/integration/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1227 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/integration/test_installation.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.909552 resilient_sdk-49.0.4423/tests/shared_mock_data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      806 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/.mock_sdk_settings.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        3 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      274 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock.zip
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24687 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_app.log
+-rw-rw-r--   0 travis    (2000) travis    (2000)      292 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_data.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   224427 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_export.res
+-rw-rw-r--   0 travis    (2000) travis    (2000)    58851 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_export.resz
+-rw-rw-r--   0 travis    (2000) travis    (2000)   223680 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_export_corrupt.res
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.909552 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      627 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    57247 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/customize.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   191223 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/customize_old.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.909552 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_app_zip_files/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    66751 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_app.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41671 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_export.res
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41951 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_with_payload_samples_export.res
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2773 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_customize_w_playbook.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   539154 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_export_w_playbook.res
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.897552 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.945552 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2604 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/Dockerfile
+-rw-rw-r--   0 travis    (2000) travis    (2000)      214 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5843 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1619 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/apikey_permissions.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.949552 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4342 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/pb_test_resilient_sdk.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      712 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/wf_mock_workflow_one.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1196 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/wf_mock_workflow_two.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.897552 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/doc/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.949552 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/doc/screenshots/
+-rw-rw-r--   0 travis    (2000) travis    (2000)   111993 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/doc/screenshots/main.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)      566 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/entrypoint.sh
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.949552 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       30 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)      145 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.949552 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2254 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_a_mock_function_with_no_unicode_characters_in_name.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2061 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function__three.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3465 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function_one.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2355 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function_two.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.949552 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/lib/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/lib/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6889 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/lib/app_common.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.997552 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.997552 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      497 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/data/soar_close_case.jinja
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2976 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/data/soar_create_case.jinja
+-rw-rw-r--   0 travis    (2000) travis    (2000)      351 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/data/soar_update_case.jinja
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10660 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/poller.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.997552 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      591 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2967 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2967 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165718.bak
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2967 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165719.bak
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2967 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165720.bak
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:18.045552 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    49696 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res
+-rw-rw-r--   0 travis    (2000) travis    (2000)    50432 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165718.bak
+-rw-rw-r--   0 travis    (2000) travis    (2000)    50432 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165719.bak
+-rw-rw-r--   0 travis    (2000) travis    (2000)    50432 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165720.bak
+-rw-rw-r--   0 travis    (2000) travis    (2000)      594 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/selftest.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:18.049552 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/icons/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45545 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/icons/app_logo.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3414 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/icons/company_logo.png
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:17.897552 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:18.049552 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/mock_json_endpoint_fail.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/mock_json_endpoint_success.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/mock_json_expectation_fail.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/mock_json_expectation_success.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/output_json_example.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/a_mock_function_with_no_unicode_characters_in_name/output_json_schema.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:18.101552 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/mock_json_endpoint_fail.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/mock_json_endpoint_success.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/mock_json_expectation_fail.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/mock_json_expectation_success.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/output_json_example.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function__three/output_json_schema.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:18.101552 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/mock_json_endpoint_fail.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/mock_json_endpoint_success.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/mock_json_expectation_fail.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/mock_json_expectation_success.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)       56 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/output_json_example.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_one/output_json_schema.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:18.157552 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/mock_json_endpoint_fail.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/mock_json_endpoint_success.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/mock_json_expectation_fail.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/mock_json_expectation_success.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/output_json_example.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/payload_samples/mock_function_two/output_json_schema.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2005 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:18.157552 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2536 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_a_mock_function_with_no_unicode_characters_in_name.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2325 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function__three.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2684 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function_one.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2381 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function_two.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      741 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tox.ini
+-rw-rw-r--   0 travis    (2000) travis    (2000)    53354 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_reload_export_w_playbook.res
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2352 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/setup.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1955 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/setup_callable_data.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1798 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/setup_py_lines.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2795 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_paths.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   413882 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_reload_export.res
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1102 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/mock_xml_test_report.xml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:18.165552 resilient_sdk-49.0.4423/tests/shared_mock_data/resilient_api_data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)  3278485 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/resilient_api_data/export-with-playbook.JSON
+-rw-rw-r--   0 travis    (2000) travis    (2000)   594886 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/resilient_api_data/export.JSON
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1449 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/resilient_api_data/orgs.JSON
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2049 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/resilient_api_data/session.JSON
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2056 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/shared_mock_data/resilient_api_mock.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:18.165552 resilient_sdk-49.0.4423/tests/unit/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/unit/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1830 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/unit/test_app.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:18.165552 resilient_sdk-49.0.4423/tests/unit/test_cmds/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/unit/test_cmds/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:18.169552 resilient_sdk-49.0.4423/tests/unit/test_cmds/ext/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/unit/test_cmds/ext/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6916 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/unit/test_cmds/ext/test_ext_package.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2070 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/unit/test_cmds/test_base_cmd.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20782 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/unit/test_cmds/test_clone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34439 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/unit/test_cmds/test_codegen.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2736 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/unit/test_cmds/test_dev.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10659 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/unit/test_cmds/test_docgen.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1145 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/unit/test_cmds/test_extract.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5876 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/unit/test_cmds/test_run_init.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23815 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/unit/test_cmds/test_validate.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-01 15:59:18.217552 resilient_sdk-49.0.4423/tests/unit/test_util/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        2 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/unit/test_util/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2148 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/unit/test_util/test_jinja_filters.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18754 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/unit/test_util/test_package_file_helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1567 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/unit/test_util/test_resilient_objects.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      470 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/unit/test_util/test_sdk_argparse.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      947 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/unit/test_util/test_sdk_exception.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29770 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/unit/test_util/test_sdk_helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3988 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/unit/test_util/test_sdk_validate_configs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48045 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/unit/test_util/test_sdk_validate_helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1623 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tests/unit/test_util/test_sdk_validate_issue.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      991 2023-06-01 15:57:43.000000 resilient_sdk-49.0.4423/tox.ini
```

### Comparing `resilient_sdk-48.2.4321/CHANGES` & `resilient_sdk-49.0.4423/CHANGES`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+**2023-05: version 49.0**
+
+* Added support to create markdown files for Playbooks as they would have been created with Workflows.
+  Includes automatic detection of global scripts in ``codegen`` when exporting playbooks. Expanded support for
+  playbooks with ``docgen`` will be included in a future release
+
 **2023-04: version 48.1**
 
 * Added new ``init`` functionality to the SDK
 * Added ``--settings`` option for ``codegen``, ``docgen``, and ``validate``
 * Bug fixes for ``validate``
 
 **2023-02: version 48.0**
```

### Comparing `resilient_sdk-48.2.4321/PKG-INFO` & `resilient_sdk-49.0.4423/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resilient_sdk
-Version: 48.2.4321
+Version: 49.0.4423
 Summary: Python SDK for developing Apps for IBM SOAR
 Home-page: https://github.com/ibmresilient/resilient-python-api/tree/main/resilient-sdk
 Author: IBM SOAR
 License: MIT
 Project-URL: Documentation, https://ibm.biz/soar-python-docs
 Project-URL: IBM Community, https://ibm.biz/soarcommunity
 Project-URL: Change Log, https://ibm.biz/resilient-sdk-changes
```

### Comparing `resilient_sdk-48.2.4321/README.md` & `resilient_sdk-49.0.4423/README.md`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/assets/IBM_Security_lockup_pos_RGB.png` & `resilient_sdk-49.0.4423/assets/IBM_Security_lockup_pos_RGB.png`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/resilient_sdk/LICENSE` & `resilient_sdk-49.0.4423/resilient_sdk/LICENSE`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/resilient_sdk/app.py` & `resilient_sdk-49.0.4423/resilient_sdk/app.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/resilient_sdk/cmds/base_cmd.py` & `resilient_sdk-49.0.4423/resilient_sdk/cmds/base_cmd.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/resilient_sdk/cmds/clone.py` & `resilient_sdk-49.0.4423/resilient_sdk/cmds/clone.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/resilient_sdk/cmds/codegen.py` & `resilient_sdk-49.0.4423/resilient_sdk/cmds/codegen.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import shutil
 
 from resilient import ensure_unicode
 from resilient_sdk.cmds.base_cmd import BaseCmd
 from resilient_sdk.util import constants
 from resilient_sdk.util import package_file_helpers as package_helpers
 from resilient_sdk.util import sdk_helpers
-from resilient_sdk.util.resilient_objects import ResilientObjMap
+from resilient_sdk.util.resilient_objects import ResilientObjMap, MD_FILE_PROPERTIES
 from resilient_sdk.util.sdk_exception import SDKException
 from resilient_sdk.util.sdk_genson_overwrites import main_genson_builder_overwrites, CustomSchemaBuilder
 
 # Get the same logger object that is used in app.py
 LOG = logging.getLogger(constants.LOGGER_NAME)
 
 
@@ -251,14 +251,55 @@
             ps_dict[package_helpers.BASE_NAME_PAYLOAD_SAMPLES_EX_SUCCESS] = (u"{0}/mock_json_expectation_success.json.jinja2".format(package_helpers.PATH_TEMPLATE_PAYLOAD_SAMPLES), jinja_data)
             ps_dict[package_helpers.BASE_NAME_PAYLOAD_SAMPLES_EP_SUCCESS] = (u"{0}/blank.json.jinja2".format(package_helpers.PATH_TEMPLATE_PAYLOAD_SAMPLES), jinja_data)
             ps_dict[package_helpers.BASE_NAME_PAYLOAD_SAMPLES_EX_FAIL] = (u"{0}/mock_json_expectation_fail.json.jinja2".format(package_helpers.PATH_TEMPLATE_PAYLOAD_SAMPLES), jinja_data)
             ps_dict[package_helpers.BASE_NAME_PAYLOAD_SAMPLES_EP_FAIL] = (u"{0}/blank.json.jinja2".format(package_helpers.PATH_TEMPLATE_PAYLOAD_SAMPLES), jinja_data)
         """
 
     @staticmethod
+    def _check_and_create_md_files(package_mapping_dict, object_type, jinja_data):
+        """
+        Creates md files for workflows and playbooks using jinja2 templates.
+        
+        Note: as the mapping_dict is passed by reference,
+        there is no need to return it.
+        
+        :param package_mapping_dict: Dictionary of all the files to render
+        :type package_mapping_dict: dict
+        :param object_type: Type of object to create md files for (workflow or playbook)
+        :type object_type: str
+        :param jinja_data: A dictionary of the data to render the associated template with
+        :type jinja_data: dict
+        """
+        _obj_properties = MD_FILE_PROPERTIES[object_type]
+
+        # Get a list of workflow/playbooks names in export.
+        ob_names = [obj.get(_obj_properties["ResilientObj"]) for obj in jinja_data.get(object_type)]
+
+        for obj in jinja_data.get(object_type, []):
+            # Get workflow/playbooks name
+            ob_name = obj.get(_obj_properties["ResilientObj"])
+
+            # add sdk version to workflow data
+            obj["sdk_version"] = sdk_helpers.get_resilient_sdk_version()
+
+            # Generate pb_xx.md/wf_xx.md file name
+            # Don't add prefix if workflow/playbook name already begins with "wf_/pb_".
+            if re.search(_obj_properties["prefix_pattern"], ob_name):
+                file_name = u"{0}.md".format(ob_name)
+            else:
+                file_name = _obj_properties["obj_file_name"].format(ob_name)
+                # Check if file_name without extension already exists in workflow/playbooks names list.
+                if os.path.splitext(file_name)[0] in ob_names:
+                    raise SDKException(u"File name '{0}' already in use please recreate the {1} '{2}'."
+                        .format(file_name, object_type, ob_name))
+
+            # Add workflow/playbook to data directory
+            package_mapping_dict["data"][file_name] = (_obj_properties["jinja_file_path"], obj)
+
+    @staticmethod
     def _gen_function(args):
         # TODO: Handle just generating a FunctionComponent for the /components directory
         LOG.info("codegen _gen_function called")
 
     @staticmethod
     def _gen_package(args, setup_py_attributes={}):
 
@@ -464,38 +505,19 @@
 
             # Add to 'tests' directory
             package_mapping_dict["tests"][u"test_{0}".format(file_name)] = ("tests/test_function.py.jinja2", f)
 
             # Add a 'payload_samples/fn_name' directory and the files to it
             CmdCodegen.add_payload_samples(package_mapping_dict, fn_name, f)
 
-        # Get a list of workflow names in export.
-        wf_names = [w.get(ResilientObjMap.WORKFLOWS) for w in jinja_data.get("workflows")]
-
-        for w in jinja_data.get("workflows"):
-            # Get workflow name
-            wf_name = w.get(ResilientObjMap.WORKFLOWS)
-
-            # add sdk version to workflow data
-            w["sdk_version"] = sdk_helpers.get_resilient_sdk_version()
-
-
-            # Generate wf_xx.md file name
-            # Don't add prefix if workflow name already begins with "wf_".
-            if re.search(r"^wf_", wf_name):
-                file_name = u"{0}.md".format(wf_name)
-            else:
-                file_name = u"wf_{0}.md".format(wf_name)
-                # Check if file_name without extension already exists in workflow names list.
-                if os.path.splitext(file_name)[0] in wf_names:
-                    raise SDKException(u"File name '{0}' already in use please recreate the workflow '{1}'."
-                                       .format(file_name, wf_name))
+        # checks and creates data for .md files for workflow
+        CmdCodegen._check_and_create_md_files(package_mapping_dict, "workflows", jinja_data)
 
-            # Add workflow to data directory
-            package_mapping_dict["data"][file_name] = ("data/workflow.md.jinja2", w)
+        # checks and creates .md files for playbooks
+        CmdCodegen._check_and_create_md_files(package_mapping_dict, "playbooks", jinja_data)
 
         newly_generated_files, skipped_files = CmdCodegen.render_jinja_mapping(
             jinja_mapping_dict=package_mapping_dict,
             jinja_env=jinja_env,
             target_dir=output_base,
             package_dir=output_base)
```

### Comparing `resilient_sdk-48.2.4321/resilient_sdk/cmds/dev.py` & `resilient_sdk-49.0.4423/resilient_sdk/cmds/dev.py`

 * *Files 3% similar despite different names*

```diff
@@ -127,33 +127,37 @@
                                                      functions=old_params.get("functions"),
                                                      workflows=old_params.get("workflows"),
                                                      rules=old_params.get("actions"),
                                                      fields=old_params.get("incident_fields"),
                                                      artifact_types=old_params.get("incident_artifact_types"),
                                                      datatables=old_params.get("datatables"),
                                                      tasks=old_params.get("automatic_tasks"),
-                                                     scripts=old_params.get("scripts"))
+                                                     scripts=old_params.get("scripts"),
+                                                     playbooks=old_params.get("playbooks"))
 
             jinja_data["export_data"] = sdk_helpers.minify_export(customize_py_import_definition,
                                                                   message_destinations=sdk_helpers.get_object_api_names(ResilientObjMap.MESSAGE_DESTINATIONS, jinja_data.get("message_destinations")),
                                                                   functions=sdk_helpers.get_object_api_names(ResilientObjMap.FUNCTIONS, jinja_data.get("functions")),
                                                                   workflows=sdk_helpers.get_object_api_names(ResilientObjMap.WORKFLOWS, jinja_data.get("workflows")),
                                                                   rules=sdk_helpers.get_object_api_names(ResilientObjMap.RULES, jinja_data.get("rules")),
                                                                   fields=jinja_data.get("all_fields"),
                                                                   artifact_types=sdk_helpers.get_object_api_names(ResilientObjMap.INCIDENT_ARTIFACT_TYPES, jinja_data.get("artifact_types")),
                                                                   datatables=sdk_helpers.get_object_api_names(ResilientObjMap.DATATABLES, jinja_data.get("datatables")),
                                                                   tasks=sdk_helpers.get_object_api_names(ResilientObjMap.TASKS, jinja_data.get("tasks")),
                                                                   phases=sdk_helpers.get_object_api_names(ResilientObjMap.PHASES, jinja_data.get("phases")),
-                                                                  scripts=sdk_helpers.get_object_api_names(ResilientObjMap.SCRIPTS, jinja_data.get("scripts")))
+                                                                  scripts=sdk_helpers.get_object_api_names(ResilientObjMap.SCRIPTS, jinja_data.get("scripts")),
+                                                                  playbooks=sdk_helpers.get_object_api_names(ResilientObjMap.PLAYBOOKS, jinja_data.get("playbooks")))
 
             # Add package_name to jinja_data
             jinja_data["package_name"] = package_name
 
             # Add version
             jinja_data["version"] = setup_py_attributes.get("version", package_helpers.MIN_SETUP_PY_VERSION)
+            # add current SDK version to jinja data
+            jinja_data["sdk_version"] = sdk_helpers.get_resilient_sdk_version()
 
             # Instansiate Jinja2 Environment with path to Jinja2 templates for customize.py
             jinja_env = sdk_helpers.setup_jinja_env("data/codegen/templates/package_template/package/util")
             jinja_template = jinja_env.get_template("customize.py.jinja2")
 
             LOG.info("Writing new customize.py file")
```

### Comparing `resilient_sdk-48.2.4321/resilient_sdk/cmds/docgen.py` & `resilient_sdk-49.0.4423/resilient_sdk/cmds/docgen.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/resilient_sdk/cmds/ext/ext_package.py` & `resilient_sdk-49.0.4423/resilient_sdk/cmds/ext/ext_package.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/resilient_sdk/cmds/extract.py` & `resilient_sdk-49.0.4423/resilient_sdk/cmds/extract.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/resilient_sdk/cmds/run_init.py` & `resilient_sdk-49.0.4423/resilient_sdk/cmds/run_init.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/resilient_sdk/cmds/validate.py` & `resilient_sdk-49.0.4423/resilient_sdk/cmds/validate.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/Dockerfile.jinja2` & `resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/apikey_permissions.txt.jinja2` & `resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/apikey_permissions.txt.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/data/workflow.md.jinja2` & `resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/data/workflow.md.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/doc/screenshots/main.png` & `resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/doc/screenshots/main.png`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/entrypoint.sh.jinja2` & `resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/entrypoint.sh.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/package/components/atomic_function.py.jinja2` & `resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/components/atomic_function.py.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/package/lib/app_common.py.jinja2` & `resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/lib/app_common.py.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/package/poller/data/soar_create_case.jinja2` & `resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/poller/data/soar_create_case.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/package/poller/poller.py.jinja2` & `resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/poller/poller.py.jinja2`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,16 @@
         """
         self.polling_interval = float(options.get("polling_interval", 0))
         if not self.polling_interval or is_this_a_selftest(self):
             LOG.debug("Exiting poller because polling interval set to 0 or this run is a selftest.")
             return False
 
         LOG.info("Poller initiated, polling interval %s", self.polling_interval)
-        self.last_poller_time = get_last_poller_date(int(options.get("polling_lookback", 0)))
+        polling_lookback = options.get("polling_lookback") or 0
+        self.last_poller_time = get_last_poller_date(int(polling_lookback))
         LOG.info("Poller lookback: %s", self.last_poller_time)
 
         # collect the override templates to use when creating, updating and closing cases
         self.soar_create_case_template = options.get("soar_create_case_template")
         self.soar_update_case_template = options.get("soar_update_case_template")
         self.soar_close_case_template = options.get("soar_close_case_template")
```

### Comparing `resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/package/util/config.py.jinja2` & `resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/util/config.py.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/package/util/customize.py.jinja2` & `resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/util/customize.py.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/package/util/selftest.py.jinja2` & `resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/package/util/selftest.py.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/setup.py.jinja2` & `resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/setup.py.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/tests/test_function.py.jinja2` & `resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/tests/test_function.py.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/resilient_sdk/data/codegen/templates/package_template/tox.ini.jinja2` & `resilient_sdk-49.0.4423/resilient_sdk/data/codegen/templates/package_template/tox.ini.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/resilient_sdk/data/docgen/templates/README.md.jinja2` & `resilient_sdk-49.0.4423/resilient_sdk/data/docgen/templates/README.md.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/resilient_sdk/data/ext/icons/app_logo.png` & `resilient_sdk-49.0.4423/resilient_sdk/data/ext/icons/app_logo.png`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/resilient_sdk/data/ext/icons/company_logo.png` & `resilient_sdk-49.0.4423/resilient_sdk/data/ext/icons/company_logo.png`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/resilient_sdk/data/run_init/sdk_settings.json.jinja2` & `resilient_sdk-49.0.4423/resilient_sdk/data/run_init/sdk_settings.json.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/resilient_sdk/data/validate/.pylintrc` & `resilient_sdk-49.0.4423/resilient_sdk/data/validate/.pylintrc`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/resilient_sdk/data/validate/templates/validate_report.md.jinja2` & `resilient_sdk-49.0.4423/resilient_sdk/data/validate/templates/validate_report.md.jinja2`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/resilient_sdk/util/constants.py` & `resilient_sdk-49.0.4423/resilient_sdk/util/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 PATH_RES_DEFAULT_LOG_FILE = os.path.join(PATH_RES_DEFAULT_LOG_DIR, "app.log")
 
 LOGGER_NAME = "resilient_sdk_log"
 LOG_DIVIDER = "\n------------------------\n"
 ENV_VAR_DEV = "RES_SDK_DEV"
 ENV_VAR_APP_CONFIG_FILE = "APP_CONFIG_FILE"
 
-RESILIENT_LIBRARIES_VERSION = "48.1.0"
-RESILIENT_LIBRARIES_VERSION_DEV = "48.1.0"
+RESILIENT_LIBRARIES_VERSION = "49.0.0"
+RESILIENT_LIBRARIES_VERSION_DEV = "49.0.0"
 RESILIENT_VERSION_WITH_PROXY_SUPPORT = (42, 0, 0)
 CURRENT_SOAR_SERVER_VERSION = None
 MIN_SOAR_SERVER_VERSION_PLAYBOOKS = 44.0
 
 MIN_SUPPORTED_PY_VERSION = (3, 6)
 SDK_PACKAGE_NAME = "resilient-sdk"
 SDK_RESOURCE_NAME = "resilient_sdk"
```

### Comparing `resilient_sdk-48.2.4321/resilient_sdk/util/jinja2_filters.py` & `resilient_sdk-49.0.4423/resilient_sdk/util/jinja2_filters.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/resilient_sdk/util/package_file_helpers.py` & `resilient_sdk-49.0.4423/resilient_sdk/util/package_file_helpers.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/resilient_sdk/util/resilient_objects.py` & `resilient_sdk-49.0.4423/resilient_sdk/util/resilient_objects.py`

 * *Files 24% similar despite different names*

```diff
@@ -38,21 +38,26 @@
     "name": "internal_customizations_field",
     "read_only": True,
     "text": "Customizations Field (internal)",
     "type_id": 0,
     "uuid": str(DEFAULT_INCIDENT_FIELD_UUID)
 }
 
+# Used to determine if a script is local or global in a playbook (codegen)
+SCRIPT_TYPE_MAP = {
+    "local"  : "Local script",
+    "global" : "Global script"
+}
+
 # Default field names we should ignore (mainly in docgen)
 IGNORED_INCIDENT_FIELDS = [
     u"incident/internal_customizations_field",
     u"incident/inc_training"
 ]
 
-
 class ResilientObjMap(object):
     """
     A single location to map Resilient Objects
     access names in an export
 
     E.g. some are 'programmatic_name' others are 'name'
     """
@@ -89,7 +94,23 @@
 
 
 class ResilientFieldTypes(object):
     """A single location for Resilient Field Types"""
 
     ACTIVITY_FIELD = "actioninvocation"
     FUNCTION_INPUT = "__function"
+
+
+MD_FILE_PROPERTIES = {
+    "workflows" : {
+        "prefix_pattern"  : r"^wf_",
+        "obj_file_name"   : u"wf_{0}.md",
+        "ResilientObj"    : ResilientObjMap.WORKFLOWS,
+        "jinja_file_path" : "data/workflow.md.jinja2",
+    },
+    "playbooks" : {
+        "prefix_pattern"  : r"^pb_",
+        "obj_file_name"   : u"pb_{0}.md",
+        "ResilientObj"    : ResilientObjMap.PLAYBOOKS,
+        "jinja_file_path" : "data/playbook.md.jinja2",
+    }
+}
```

### Comparing `resilient_sdk-48.2.4321/resilient_sdk/util/sdk_argparse.py` & `resilient_sdk-49.0.4423/resilient_sdk/util/sdk_argparse.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/resilient_sdk/util/sdk_exception.py` & `resilient_sdk-49.0.4423/resilient_sdk/util/sdk_exception.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/resilient_sdk/util/sdk_genson_overwrites.py` & `resilient_sdk-49.0.4423/resilient_sdk/util/sdk_genson_overwrites.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/resilient_sdk/util/sdk_helpers.py` & `resilient_sdk-49.0.4423/resilient_sdk/util/sdk_helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 import requests
 import requests.exceptions
 from jinja2 import Environment, PackageLoader
 from resilient_sdk.util import constants
 from resilient_sdk.util.jinja2_filters import add_filters_to_jinja_env
 from resilient_sdk.util.resilient_objects import (DEFAULT_INCIDENT_FIELD,
                                                   DEFAULT_INCIDENT_TYPE,
+                                                  SCRIPT_TYPE_MAP,
                                                   ResilientFieldTypes,
                                                   ResilientObjMap,
                                                   ResilientTypeIds)
 from resilient_sdk.util.sdk_exception import SDKException
 
 from resilient import ArgumentParser
 from resilient import constants as res_constants
@@ -550,14 +551,40 @@
     """
     if list_objs:
         return [o.get(api_name) for o in list_objs]
     else:
         return []
 
 
+def _get_script_info(each_script_in_playbook, scripts_in_location, script_type):
+    '''
+    Extracts script related information for playbooks. Scripts can be of 2 types: local or global.
+    Local scripts live within the playbook itself, while global scripts are stored in the global_export dict.
+    
+    Note: The scripts are passed by reference. They need not be returned. They are directly updated.
+    :param each_script_in_playbook: Individual scripts found in the playbook
+    :type each_script_in_playbook: dict
+    :param scripts_in_location: All scripts in the location (global or local). Global scripts are pulled directly from the global_export dict. Local scripts are pulled from the playbook
+    :type scripts_in_location: list
+    :param script_type: The type of script (global or local)
+    :type script_type: str
+    '''
+    found_script = False
+    for sc in scripts_in_location:
+        if each_script_in_playbook.get("uuid", "uuid_not_found_pb") == sc.get("uuid", "uuid_not_found_sc"):
+            each_script_in_playbook["name"] = sc.get("name")
+            each_script_in_playbook["script_type"] = script_type
+            each_script_in_playbook["description"] = sc.get("description")
+            each_script_in_playbook["object_type"] = sc.get("object_type")
+            each_script_in_playbook["script_text"] = sc.get("script_text", "")
+            found_script = True
+            break
+    return found_script
+
+
 def get_obj_from_list(identifer, obj_list, condition=lambda o: True):
     """
     Return a dict the name of the object as its Key
     e.g. {
         "fn_mock_function_1": {...},
         "fn_mock_function_2": {...}
     }
@@ -795,14 +822,52 @@
 
     # Get Playbooks
     if playbooks and constants.CURRENT_SOAR_SERVER_VERSION and constants.CURRENT_SOAR_SERVER_VERSION < constants.MIN_SOAR_SERVER_VERSION_PLAYBOOKS:
         raise SDKException(constants.ERROR_PLAYBOOK_SUPPORT)
     else:
         return_dict["playbooks"] = get_res_obj("playbooks", ResilientObjMap.PLAYBOOKS, "Playbook", playbooks, export)
 
+        if get_related_objects:
+            # For Playbooks we attempt to locate related functions and scripts
+            # Get Functions in Playbooks
+            for playbook in return_dict.get("playbooks", []):
+                # This gets all the functions and scripts in the Playbooks's XML
+                pb_objects = get_playbook_objects(playbook)
+
+                # Add the Display Name and Name to each wf_function
+                for pb_fn in pb_objects.get("functions", []):
+                    for fn in return_dict["functions"]:
+                        if pb_fn.get("uuid", "uuid_not_found_pb") == fn.get("uuid", "uuid_not_found_fn"):
+                            pb_fn["name"] = fn.get("name")
+                            pb_fn["display_name"] = fn.get("display_name")
+                            pb_fn["message_destination"] = fn.get("destination_handle", "")
+                            break
+
+                # If a playbook script is local, its information can be directly extracted from the playbook,
+                # if not, the script's information has to be extracted from the global scripts
+                for pb_sc in pb_objects.get("scripts", []):
+                    # If the script is a local script, then we need to find the script in the Playbook
+                    found_script = _get_script_info(pb_sc, playbook.get("local_scripts"), SCRIPT_TYPE_MAP.get("local"))
+
+                    # If script not found in playbook, searching Global Scripts
+                    found_script = _get_script_info(pb_sc, return_dict["scripts"], SCRIPT_TYPE_MAP.get("global")) if not found_script else True
+
+                    # If the script is not found in the Playbook or Global Scripts, then its UUID is used to find the script form the org export
+                    if not found_script:
+                        _unfound_scripts = get_res_obj("scripts", "uuid", "Script", [pb_sc.get("uuid")], export)
+                        for script in _unfound_scripts:
+                            # Renaming the x_api_name to name. Since the script was fetched with UUID, the x_api_name is the UUID
+                            script["x_api_name"] = script["name"]
+                        found_script = _get_script_info(pb_sc, _unfound_scripts, SCRIPT_TYPE_MAP.get("global"))
+                        # Adding script to return_dict. This is to make sure that its included in the export.res and customize.py
+                        return_dict["scripts"].extend(_unfound_scripts)
+
+                playbook["pb_functions"] = pb_objects.get("functions")
+                playbook["pb_scripts"]   = pb_objects.get("scripts")
+
     return return_dict
 
 
 def minify_export(export,
                   keys_to_keep=[],
                   message_destinations=[],
                   functions=[],
@@ -1159,14 +1224,77 @@
         return_function["pre_processing_script"] = return_function.get("pre_processing_script", None)
 
         return_functions.append(return_function)
 
     return return_functions
 
 
+def get_playbook_objects(playbook, function_uuid=None):
+    """Parses the XML of the Playbook Object and returns
+    a List of all Functions and Scripts found. The scripts
+    returned only has the uuid attribute. This can later
+    be used to extract all script-related information either
+    form the playbook export or from global scripts. If
+    function_uuid is defined returns all occurrences of that
+    function only.
+
+    Function Attributes:
+    - uuid: String
+    - inputs: Dict
+    - pre_processing_script: String
+    - result_name: String
+
+    Script Attributes:
+    - uuid: String
+    """
+    playbook_elements = {"functions": [], "scripts": []}
+
+    # Playbook XML text
+    pb_xml = playbook.get("content", {}).get("xml", None)
+
+    if pb_xml is None:
+        raise SDKException("Could not load xml content from Playbooks: {0}".format(playbook))
+
+    # Get the root element + encoded in utf8 in order to handle Unicode
+    root = ET.fromstring(pb_xml.encode("utf8"))
+
+    # Get the prefix for each element's tag
+    tag_prefix = root.tag.replace("definitions", "")
+
+    xml_function_path = "./{0}process/{0}serviceTask/{0}extensionElements/*".format(tag_prefix)
+    xml_script_path   = "./{0}process/{0}scriptTask/{0}extensionElements/*".format(tag_prefix)
+
+    if function_uuid is not None:
+        xml_function_path = "{0}[@uuid='{1}']".format(xml_function_path, function_uuid)
+
+        # Get all elements at xml_path that have the uuid of the function
+        playbook_elements += root.findall(xml_function_path)
+    else:
+        # Paths to functions and scripts in the XML
+        the_extension_elements  = root.findall(xml_function_path)
+        the_extension_elements += root.findall(xml_script_path)
+
+        for extension_element in the_extension_elements:
+            return_function = {}
+            # Extracting Function related data from the XML
+            if "function" in extension_element.tag:
+                return_function = json.loads(extension_element.text)
+                return_function["uuid"] = extension_element.attrib.get("uuid", "")
+                return_function["result_name"] = return_function.get("result_name", None)
+                return_function["pre_processing_script"] = return_function.get("pre_processing_script", None)
+                playbook_elements["functions"].append(return_function)
+
+            # Extracting Script related data from the XML
+            if "script" in extension_element.tag:
+                return_function["uuid"] = extension_element.get("uuid", "")
+                playbook_elements["scripts"].append(return_function)
+
+    return playbook_elements
+
+
 def get_main_cmd():
     """
     Return the "main" command from the command line.
 
     E.g. with command line: '$ resilient-sdk codegen -p abc'
     this function will return 'codegen'
     """
```

### Comparing `resilient_sdk-48.2.4321/resilient_sdk/util/sdk_validate_configs.py` & `resilient_sdk-49.0.4423/resilient_sdk/util/sdk_validate_configs.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         "severity": SDKValidateIssue.SEVERITY_LEVEL_CRITICAL
     }),
     ("install_requires", {
         "parse_func": package_helpers.parse_setup_py,
         "fail_func": lambda x: bool(sdk_validate_helpers.check_dependencies_version_specifiers(x)),
         "fail_msg": u"'{0}' has the following improperly formatted dependencies: {2}",
         "fail_msg_lambda_supplement": lambda x: sdk_validate_helpers.check_dependencies_version_specifiers(x),
-        "solution": u"All dependencies (other than resilient-circuits) must be include a version in the format '~=' or '=='",
+        "solution": u"All dependencies (other than resilient-circuits) must include a version in the format '~=' or '=='",
         "severity": SDKValidateIssue.SEVERITY_LEVEL_WARN
     }),
     ("python_requires", {
         "parse_func": package_helpers.parse_setup_py,
         "fail_func": lambda x: package_helpers.get_required_python_version(x) < constants.MIN_SUPPORTED_PY_VERSION,
         "fail_msg": u"'{0}' version '{2[0]}.{2[1]}' is not supported",
         "fail_msg_lambda_supplement": lambda x: package_helpers.get_required_python_version(x),
```

### Comparing `resilient_sdk-48.2.4321/resilient_sdk/util/sdk_validate_helpers.py` & `resilient_sdk-49.0.4423/resilient_sdk/util/sdk_validate_helpers.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/resilient_sdk/util/sdk_validate_issue.py` & `resilient_sdk-49.0.4423/resilient_sdk/util/sdk_validate_issue.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/resilient_sdk.egg-info/PKG-INFO` & `resilient_sdk-49.0.4423/resilient_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resilient-sdk
-Version: 48.2.4321
+Version: 49.0.4423
 Summary: Python SDK for developing Apps for IBM SOAR
 Home-page: https://github.com/ibmresilient/resilient-python-api/tree/main/resilient-sdk
 Author: IBM SOAR
 License: MIT
 Project-URL: Documentation, https://ibm.biz/soar-python-docs
 Project-URL: IBM Community, https://ibm.biz/soarcommunity
 Project-URL: Change Log, https://ibm.biz/resilient-sdk-changes
```

### Comparing `resilient_sdk-48.2.4321/resilient_sdk.egg-info/SOURCES.txt` & `resilient_sdk-49.0.4423/resilient_sdk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 resilient_sdk/data/codegen/templates/package_template/Dockerfile.jinja2
 resilient_sdk/data/codegen/templates/package_template/MANIFEST.in.jinja2
 resilient_sdk/data/codegen/templates/package_template/README.md.jinja2
 resilient_sdk/data/codegen/templates/package_template/apikey_permissions.txt.jinja2
 resilient_sdk/data/codegen/templates/package_template/entrypoint.sh.jinja2
 resilient_sdk/data/codegen/templates/package_template/setup.py.jinja2
 resilient_sdk/data/codegen/templates/package_template/tox.ini.jinja2
+resilient_sdk/data/codegen/templates/package_template/data/playbook.md.jinja2
 resilient_sdk/data/codegen/templates/package_template/data/workflow.md.jinja2
 resilient_sdk/data/codegen/templates/package_template/doc/screenshots/main.png
 resilient_sdk/data/codegen/templates/package_template/package/LICENSE.jinja2
 resilient_sdk/data/codegen/templates/package_template/package/__init__.py.jinja2
 resilient_sdk/data/codegen/templates/package_template/package/components/__init__.py.jinja2
 resilient_sdk/data/codegen/templates/package_template/package/components/atomic_function.py.jinja2
 resilient_sdk/data/codegen/templates/package_template/package/lib/__init__.py.jinja2
@@ -104,14 +105,15 @@
 tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/Dockerfile
 tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/MANIFEST.in
 tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/README.md
 tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/apikey_permissions.txt
 tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/entrypoint.sh
 tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/setup.py
 tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tox.ini
+tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/pb_test_resilient_sdk.md
 tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/wf_mock_workflow_one.md
 tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/wf_mock_workflow_two.md
 tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/doc/screenshots/main.png
 tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/LICENSE
 tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/__init__.py
 tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/__init__.py
 tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_a_mock_function_with_no_unicode_characters_in_name.py
```

### Comparing `resilient_sdk-48.2.4321/setup.cfg` & `resilient_sdk-49.0.4423/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 [options]
 packages = find:
 include_package_data = True
 python_requires = >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*
 setup_requires = setuptools_scm
 platforms = any
 install_requires = 
-	resilient >= 48.1
+	resilient >= 49.0
 	
 	genson    ~= 1.2
 	
 	jinja2    ~= 3.0; python_version >= "3.6"
 	
 	jinja2    ~= 2.0; python_version == "2.7"
```

### Comparing `resilient_sdk-48.2.4321/tests/conftest.py` & `resilient_sdk-49.0.4423/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -399,14 +399,28 @@
 
     _add_to_cmd_line_args(args_to_add)
 
     yield
 
     sys.argv = original_cmd_line
 
+
+@pytest.fixture
+def fx_reset_argv():
+    """
+    Before: Takes a copy of sys.argv and allows functions to add args to it
+    After: Set the cmd line args back to its original value
+    """
+    original_cmd_line = copy.deepcopy(sys.argv)
+
+    yield
+
+    sys.argv = original_cmd_line
+
+
 @pytest.fixture
 def fx_mock_settings_file_path():
     """
     Before: Change the settings file path to point to the test temp directory
     After: Change the settings file path back to the original value
     """
     old_sdk_settings_path = constants.SDK_SETTINGS_FILE_PATH
```

### Comparing `resilient_sdk-48.2.4321/tests/helpers.py` & `resilient_sdk-49.0.4423/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/integration/test_installation.py` & `resilient_sdk-49.0.4423/tests/integration/test_installation.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/.mock_sdk_settings.json` & `resilient_sdk-49.0.4423/tests/shared_mock_data/.mock_sdk_settings.json`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/mock_app.log` & `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_app.log`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/mock_export.res` & `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_export.res`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/mock_export.resz` & `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_export.resz`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/mock_export_corrupt.res` & `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_export_corrupt.res`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/config.py` & `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/config.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/customize.py` & `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/customize.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/customize_old.py` & `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/customize_old.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_app.json` & `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_app.json`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_export.res` & `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_export.res`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_with_payload_samples_export.res` & `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_app_zip_files/mock_with_payload_samples_export.res`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_customize_w_playbook.py` & `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_customize_w_playbook.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_export_w_playbook.res` & `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_export_w_playbook.res`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/Dockerfile` & `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/Dockerfile`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/README.md` & `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/README.md`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/apikey_permissions.txt` & `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/apikey_permissions.txt`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/wf_mock_workflow_one.md` & `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/wf_mock_workflow_one.md`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/wf_mock_workflow_two.md` & `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/data/wf_mock_workflow_two.md`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/doc/screenshots/main.png` & `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/doc/screenshots/main.png`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/entrypoint.sh` & `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_a_mock_function_with_no_unicode_characters_in_name.py` & `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_a_mock_function_with_no_unicode_characters_in_name.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function__three.py` & `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function__three.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function_one.py` & `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function_one.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function_two.py` & `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/components/funct_mock_function_two.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/lib/app_common.py` & `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/lib/app_common.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/data/soar_create_case.jinja` & `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/data/soar_create_case.jinja`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/poller.py` & `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/poller/poller.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/config.py` & `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/config.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py` & `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165718.bak` & `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165718.bak`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165719.bak` & `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165719.bak`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165720.bak` & `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/customize.py-20210906165720.bak`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res` & `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165718.bak` & `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165718.bak`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165719.bak` & `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165719.bak`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165720.bak` & `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/data/export.res-20210906165720.bak`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/selftest.py` & `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/fn_main_mock_integration/util/selftest.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/icons/app_logo.png` & `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/icons/app_logo.png`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/icons/company_logo.png` & `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/icons/company_logo.png`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/setup.py` & `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/setup.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_a_mock_function_with_no_unicode_characters_in_name.py` & `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_a_mock_function_with_no_unicode_characters_in_name.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function__three.py` & `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function__three.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function_one.py` & `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function_one.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function_two.py` & `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tests/test_funct_mock_function_two.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tox.ini` & `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_integrations/fn_main_mock_integration/tox.ini`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/mock_reload_export_w_playbook.res` & `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/mock_reload_export_w_playbook.res`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/setup.py` & `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/setup.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/setup_callable_data.txt` & `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/setup_callable_data.txt`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/mock_package_files/setup_py_lines.py` & `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_package_files/setup_py_lines.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/mock_paths.py` & `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_paths.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/mock_reload_export.res` & `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_reload_export.res`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/mock_xml_test_report.xml` & `resilient_sdk-49.0.4423/tests/shared_mock_data/mock_xml_test_report.xml`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/resilient_api_data/export-with-playbook.JSON` & `resilient_sdk-49.0.4423/tests/shared_mock_data/resilient_api_data/export-with-playbook.JSON`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9933283090550066%*

 * *Differences: {"'fields'": "{insert: [(0, OrderedDict([('allow_default_value', False), ('blank_option', False), "*

 * *             "('calculated', False), ('changeable', True), ('chosen', False), "*

 * *             "('default_chosen_by_server', False), ('deprecated', False), ('export_key', "*

 * *             "'__function/scheduler_label'), ('hide_notification', False), ('id', 420), "*

 * *             "('input_type', 'text'), ('internal', False), ('is_tracked', False), ('name', "*

 * *             "'scheduler_label'), ('operation_perms', Orde […]*

```diff
@@ -15178,14 +15178,68 @@
             "allow_default_value": false,
             "blank_option": false,
             "calculated": false,
             "changeable": true,
             "chosen": false,
             "default_chosen_by_server": false,
             "deprecated": false,
+            "export_key": "__function/scheduler_label",
+            "hide_notification": false,
+            "id": 420,
+            "input_type": "text",
+            "internal": false,
+            "is_tracked": false,
+            "name": "scheduler_label",
+            "operation_perms": {},
+            "operations": [],
+            "placeholder": "",
+            "prefix": null,
+            "read_only": false,
+            "rich_text": false,
+            "tags": [
+                {
+                    "tag_handle": "fn_scheduler",
+                    "value": null
+                },
+                {
+                    "tag_handle": "playbook_16c168c0_628f_4f50_9523_ae5c0287b76d",
+                    "value": "Playbook Tag"
+                },
+                {
+                    "tag_handle": "playbook_19f67260_22c1_4871_9a9f_31b6889ab9ea",
+                    "value": "Playbook Tag"
+                },
+                {
+                    "tag_handle": "playbook_3da68bad_7a31_4e0d_bb23_36ddf5303fb6",
+                    "value": "Playbook Tag"
+                },
+                {
+                    "tag_handle": "playbook_cb82c8f1_c294_4a01_8a3a_12e581bca983",
+                    "value": "Playbook Tag"
+                },
+                {
+                    "tag_handle": "playbook_e6557d98_6d8b_4fa3_bad3_cf0e61d1ad04",
+                    "value": "Playbook Tag"
+                }
+            ],
+            "templates": [],
+            "text": "scheduler_label",
+            "tooltip": "Scheduled job name for identification",
+            "type_id": 11,
+            "uuid": "a8315456-7803-4a4d-a482-aeec5ca91c4e",
+            "values": []
+        },
+        {
+            "allow_default_value": false,
+            "blank_option": false,
+            "calculated": false,
+            "changeable": true,
+            "chosen": false,
+            "default_chosen_by_server": false,
+            "deprecated": false,
             "export_key": "__function/utilities_parse_email_attachments",
             "hide_notification": false,
             "id": 1020,
             "input_type": "boolean",
             "internal": false,
             "is_tracked": false,
             "name": "utilities_parse_email_attachments",
@@ -34163,14 +34217,113 @@
             "type_id": 0,
             "uuid": "7d587ba0-8771-48c7-9d72-acae3a19db87",
             "values": []
         }
     ],
     "functions": [
         {
+            "created_date": 1682677405132,
+            "creator": {
+                "display_name": "Admin User",
+                "id": 1,
+                "name": "admin@example.com",
+                "type": "user"
+            },
+            "description": {
+                "content": "Pause a scheduled rule",
+                "format": "text"
+            },
+            "destination_handle": "fn_scheduler",
+            "display_name": "Scheduled Rule Pause",
+            "export_key": "scheduled_rule_pause",
+            "id": 19,
+            "last_modified_by": {
+                "display_name": "Admin User",
+                "id": 1,
+                "name": "admin@example.com",
+                "type": "user"
+            },
+            "last_modified_time": 1682677405160,
+            "name": "scheduled_rule_pause",
+            "output_json_example": "{\"version\": \"1.0\", \"success\": true, \"reason\": null, \"content\": {\"id\": \"domain2-5640\", \"args\": [5640, null, null, \"domain2-5640\", \"test scheduled rule\", 212, 0, {\"artifact_value\": \"abc.com\", \"artifact_type\": \"domain\"}, null, {\"timezone\": \"America/New_York\", \"thread_max\": \"20\", \"datastore_dir\": \"/tmp/scheduler.sqlite\"}], \"next_run_time\": \"Apr 27 2022 05:00AM\", \"type\": \"date\", \"value\": \"Apr 28 2022 04:05AM\"}, \"raw\": \"{\\\"id\\\": \\\"domain2-5640\\\", \\\"args\\\": [5640, null, null, \\\"domain2-5640\\\", \\\"test scheduled rule\\\", 212, 0, {\\\"artifact_value\\\": \\\"abc.com\\\", \\\"artifact_type\\\": \\\"domain\\\"}, null, {\\\"timezone\\\": \\\"America/New_York\\\", \\\"thread_max\\\": \\\"20\\\", \\\"datastore_dir\\\": \\\"/tmp/scheduler.sqlite\\\"}], \\\"next_run_time\\\": \\\"Apr 27 2022 05:00AM\\\", \\\"type\\\": \\\"date\\\", \\\"value\\\": \\\"Apr 28 2022 04:05AM\\\"}\", \"inputs\": {\"scheduler_label\": \"domain2-5640\"}, \"metrics\": {\"version\": \"1.0\", \"package\": \"fn-scheduler\", \"package_version\": \"1.2.0\", \"host\": \"local\", \"execution_time_ms\": 14, \"timestamp\": \"2022-04-26 09:07:44\"}}",
+            "output_json_schema": "{\"$schema\": \"http://json-schema.org/draft-06/schema\", \"type\": \"object\", \"properties\": {\"version\": {\"type\": \"string\"}, \"success\": {\"type\": \"boolean\"}, \"reason\": {}, \"content\": {\"type\": \"object\", \"properties\": {\"id\": {\"type\": \"string\"}, \"args\": {\"type\": \"array\", \"items\": {\"anyOf\": [{\"type\": [\"integer\", \"null\", \"string\"]}, {\"type\": \"object\", \"properties\": {\"artifact_value\": {\"type\": \"string\"}, \"artifact_type\": {\"type\": \"string\"}, \"timezone\": {\"type\": \"string\"}, \"thread_max\": {\"type\": \"string\"}, \"datastore_dir\": {\"type\": \"string\"}}}]}}, \"next_run_time\": {\"type\": \"string\"}, \"type\": {\"type\": \"string\"}, \"value\": {\"type\": \"string\"}}}, \"raw\": {\"type\": \"string\"}, \"inputs\": {\"type\": \"object\", \"properties\": {\"scheduler_label\": {\"type\": \"string\"}}}, \"metrics\": {\"type\": \"object\", \"properties\": {\"version\": {\"type\": \"string\"}, \"package\": {\"type\": \"string\"}, \"package_version\": {\"type\": \"string\"}, \"host\": {\"type\": \"string\"}, \"execution_time_ms\": {\"type\": \"integer\"}, \"timestamp\": {\"type\": \"string\"}}}}}",
+            "tags": [
+                {
+                    "tag_handle": "fn_scheduler",
+                    "value": null
+                },
+                {
+                    "tag_handle": "playbook_e6557d98_6d8b_4fa3_bad3_cf0e61d1ad04",
+                    "value": "Playbook Tag"
+                }
+            ],
+            "uuid": "aa278752-98c2-4866-b477-0eb19fd81b34",
+            "version": 1,
+            "view_items": [
+                {
+                    "content": "a8315456-7803-4a4d-a482-aeec5ca91c4e",
+                    "element": "field_uuid",
+                    "field_type": "__function",
+                    "show_if": null,
+                    "show_link_header": false,
+                    "step_label": null
+                }
+            ],
+            "workflows": []
+        },
+        {
+            "created_date": 1682677404972,
+            "creator": {
+                "display_name": "Admin User",
+                "id": 1,
+                "name": "admin@example.com",
+                "type": "user"
+            },
+            "description": {
+                "content": "Schedule a rule to run on a schedule. This rule will be executed for a given incident, artifact, task, etc.",
+                "format": "text"
+            },
+            "destination_handle": "fn_scheduler",
+            "display_name": "Scheduled Rule Create",
+            "export_key": "create_a_scheduled_rule",
+            "id": 14,
+            "last_modified_by": {
+                "display_name": "Admin User",
+                "id": 1,
+                "name": "admin@example.com",
+                "type": "user"
+            },
+            "last_modified_time": 1682677405000,
+            "name": "create_a_scheduled_rule",
+            "output_json_example": "{\"version\": \"1.0\", \"success\": true, \"reason\": null, \"content\": {\"version\": 1, \"id\": \"domain2-5640\", \"func\": \"fn_scheduler.components.create_a_scheduled_rule:triggered_job\", \"trigger\": null, \"executor\": \"default\", \"args\": [5640, null, null, \"domain2-5640\", \"test scheduled rule\", 212, 0, {\"artifact_value\": \"abc.com\", \"artifact_type\": \"domain\"}, null, {\"timezone\": \"America/New_York\", \"thread_max\": \"20\", \"datastore_dir\": \"/tmp/scheduler.sqlite\"}], \"kwargs\": {\"artifact_value\": \"abc.com\", \"artifact_type\": \"domain\"}, \"name\": \"triggered_job\", \"misfire_grace_time\": 1, \"coalesce\": false, \"max_instances\": 1, \"next_run_time\": \"Apr 27 2022 05:00AM\"}, \"raw\": \"{\\\"version\\\": 1, \\\"id\\\": \\\"domain2-5640\\\", \\\"func\\\": \\\"fn_scheduler.components.create_a_scheduled_rule:triggered_job\\\", \\\"trigger\\\": null, \\\"executor\\\": \\\"default\\\", \\\"args\\\": [5640, null, null, \\\"domain2-5640\\\", \\\"test scheduled rule\\\", 212, 0, {\\\"artifact_value\\\": \\\"abc.com\\\", \\\"artifact_type\\\": \\\"domain\\\"}, null, {\\\"timezone\\\": \\\"America/New_York\\\", \\\"thread_max\\\": \\\"20\\\", \\\"datastore_dir\\\": \\\"/tmp/scheduler.sqlite\\\"}], \\\"kwargs\\\": {\\\"artifact_value\\\": \\\"abc.com\\\", \\\"artifact_type\\\": \\\"domain\\\"}, \\\"name\\\": \\\"triggered_job\\\", \\\"misfire_grace_time\\\": 1, \\\"coalesce\\\": false, \\\"max_instances\\\": 1, \\\"next_run_time\\\": \\\"Apr 27 2022 05:00AM\\\"}\", \"inputs\": {\"scheduler_type_value\": \"* 5 * * *\", \"incident_id\": 5640, \"scheduler_type\": {\"id\": 2109, \"name\": \"cron\"}, \"scheduler_label_prefix\": \"domain2\", \"scheduler_rule_name\": \"test scheduled rule\", \"scheduler_rule_parameters\": \"artifact_value=abc.com;artifact_type=domain\", \"scheduler_is_playbook\": false}, \"metrics\": {\"version\": \"1.0\", \"package\": \"fn-scheduler\", \"package_version\": \"1.2.0\", \"host\": \"local\", \"execution_time_ms\": 21, \"timestamp\": \"2022-04-26 08:38:13\"}}",
+            "output_json_schema": "{\"$schema\": \"http://json-schema.org/draft-06/schema\", \"type\": \"object\", \"properties\": {\"version\": {\"type\": \"string\"}, \"success\": {\"type\": \"boolean\"}, \"reason\": {}, \"content\": {\"type\": \"object\", \"properties\": {\"version\": {\"type\": \"integer\"}, \"id\": {\"type\": \"string\"}, \"func\": {\"type\": \"string\"}, \"trigger\": {}, \"executor\": {\"type\": \"string\"}, \"args\": {\"type\": \"array\", \"items\": {\"anyOf\": [{\"type\": [\"integer\", \"null\", \"string\"]}, {\"type\": \"object\", \"properties\": {\"artifact_value\": {\"type\": \"string\"}, \"artifact_type\": {\"type\": \"string\"}, \"timezone\": {\"type\": \"string\"}, \"thread_max\": {\"type\": \"string\"}, \"datastore_dir\": {\"type\": \"string\"}}}]}}, \"kwargs\": {\"type\": \"object\", \"properties\": {\"artifact_value\": {\"type\": \"string\"}, \"artifact_type\": {\"type\": \"string\"}}}, \"name\": {\"type\": \"string\"}, \"misfire_grace_time\": {\"type\": \"integer\"}, \"coalesce\": {\"type\": \"boolean\"}, \"max_instances\": {\"type\": \"integer\"}, \"next_run_time\": {\"type\": \"string\"}}}, \"raw\": {\"type\": \"string\"}, \"inputs\": {\"type\": \"object\", \"properties\": {\"scheduler_type_value\": {\"type\": \"string\"}, \"incident_id\": {\"type\": \"integer\"}, \"scheduler_type\": {\"type\": \"object\", \"properties\": {\"id\": {\"type\": \"integer\"}, \"name\": {\"type\": \"string\"}}}, \"scheduler_label_prefix\": {\"type\": \"string\"}, \"scheduler_rule_name\": {\"type\": \"string\"}, \"scheduler_rule_parameters\": {\"type\": \"string\"}, \"scheduler_is_playbook\": {\"type\": \"boolean\"}}}, \"metrics\": {\"type\": \"object\", \"properties\": {\"version\": {\"type\": \"string\"}, \"package\": {\"type\": \"string\"}, \"package_version\": {\"type\": \"string\"}, \"host\": {\"type\": \"string\"}, \"execution_time_ms\": {\"type\": \"integer\"}, \"timestamp\": {\"type\": \"string\"}}}}}",
+            "tags": [
+                {
+                    "tag_handle": "fn_scheduler",
+                    "value": null
+                },
+                {
+                    "tag_handle": "playbook_1881ad3e_e539_47e1_b6e5_6f1c84df0864",
+                    "value": "Playbook Tag"
+                },
+                {
+                    "tag_handle": "playbook_2405a12b_1f53_4ebf_b87e_d2f91866635a",
+                    "value": "Playbook Tag"
+                },
+                {
+                    "tag_handle": "playbook_a486c165_85d1_4d15_ac7a_e6b8352efc05",
+                    "value": "Playbook Tag"
+                }
+            ],
+            "uuid": "bde7b5b2-f454-4435-9103-de31d991b924",
+            "version": 1,
+            "view_items": [],
+            "workflows": []
+        },
+        {
             "created_date": 1652112576323,
             "creator": {
                 "display_name": "all",
                 "id": 9,
                 "name": "e547eeb2-6855-41dc-a403-6fe0d8b5288c",
                 "type": "apikey"
             },
@@ -46567,14 +46720,68 @@
             "uuid": "e6c2d3f4-194b-4dc5-84da-1756a63ca6c1"
         }
     ],
     "locale": "en",
     "message_destinations": [
         {
             "api_keys": [
+                "75a0ad62-5cdc-4889-b2f4-66cf88d32e89"
+            ],
+            "destination_type": 0,
+            "expect_ack": true,
+            "export_key": "fn_scheduler",
+            "name": "fn_scheduler",
+            "programmatic_name": "fn_scheduler",
+            "tags": [
+                {
+                    "tag_handle": "fn_scheduler",
+                    "value": null
+                },
+                {
+                    "tag_handle": "playbook_16c168c0_628f_4f50_9523_ae5c0287b76d",
+                    "value": "Playbook Tag"
+                },
+                {
+                    "tag_handle": "playbook_1881ad3e_e539_47e1_b6e5_6f1c84df0864",
+                    "value": "Playbook Tag"
+                },
+                {
+                    "tag_handle": "playbook_19f67260_22c1_4871_9a9f_31b6889ab9ea",
+                    "value": "Playbook Tag"
+                },
+                {
+                    "tag_handle": "playbook_2405a12b_1f53_4ebf_b87e_d2f91866635a",
+                    "value": "Playbook Tag"
+                },
+                {
+                    "tag_handle": "playbook_3da68bad_7a31_4e0d_bb23_36ddf5303fb6",
+                    "value": "Playbook Tag"
+                },
+                {
+                    "tag_handle": "playbook_a486c165_85d1_4d15_ac7a_e6b8352efc05",
+                    "value": "Playbook Tag"
+                },
+                {
+                    "tag_handle": "playbook_cb82c8f1_c294_4a01_8a3a_12e581bca983",
+                    "value": "Playbook Tag"
+                },
+                {
+                    "tag_handle": "playbook_e6557d98_6d8b_4fa3_bad3_cf0e61d1ad04",
+                    "value": "Playbook Tag"
+                },
+                {
+                    "tag_handle": "playbook_f48af589_3237_4bf3_8b34_8a35d56dfcf0",
+                    "value": "Playbook Tag"
+                }
+            ],
+            "users": [],
+            "uuid": "02927d03-a71c-4662-9520-4010fa2ac284"
+        },
+        {
+            "api_keys": [
                 "f318f499-94f9-4a25-aefb-c8e06a19712f"
             ],
             "destination_type": 0,
             "expect_ack": true,
             "export_key": "abuseipdb",
             "name": "AbuseIPDB",
             "programmatic_name": "abuseipdb",
@@ -47578,14 +47785,397 @@
                 "type": "playbook",
                 "uuid": "450c9388-0ca9-41ed-a08b-26266ccd9e2e"
             },
             "tags": [],
             "type": "default",
             "uuid": "f880d96f-839b-47cd-9956-be7125f8273c",
             "version": 7
+        },
+        {
+            "activation_type": "manual",
+            "content": {
+                "content_version": 8,
+                "xml": "<?xml version=\"1.0\" encoding=\"UTF-8\"?><definitions xmlns=\"http://www.omg.org/spec/BPMN/20100524/MODEL\" targetNamespace=\"http://www.camunda.org/test\" xmlns:bpmndi=\"http://www.omg.org/spec/BPMN/20100524/DI\" xmlns:omgdc=\"http://www.omg.org/spec/DD/20100524/DC\" xmlns:omgdi=\"http://www.omg.org/spec/DD/20100524/DI\" xmlns:resilient=\"http://resilient.ibm.com/bpmn\" xmlns:xsd=\"http://www.w3.org/2001/XMLSchema\" xmlns:xsi=\"http://www.w3.org/2001/XMLSchema-instance\"><process id=\"playbook_f9bcb3b9_fe40_40e8_87eb_f761ed94a4a7\" isExecutable=\"true\" name=\"playbook_f9bcb3b9_fe40_40e8_87eb_f761ed94a4a7\"><documentation/><startEvent id=\"StartEvent_155asxm\"><outgoing>Flow_162tnn7</outgoing></startEvent><serviceTask id=\"ServiceTask_1\" name=\"Scheduled Rule Create\" resilient:type=\"function\"><extensionElements><resilient:function uuid=\"bde7b5b2-f454-4435-9103-de31d991b924\">{\"inputs\":{\"6742aa35-eb76-4fa4-85f8-a86015cf888a\":{\"input_type\":\"static\",\"static_input\":{\"multiselect_value\":[],\"text_value\":\"\"}},\"bfacefb1-5b39-4e7f-919c-84ccc54442f0\":{\"input_type\":\"static\",\"static_input\":{\"multiselect_value\":[],\"text_value\":\"\"}},\"a5074a34-6d40-4d03-8bf0-a8ad65b31f59\":{\"input_type\":\"static\",\"static_input\":{\"multiselect_value\":[],\"text_value\":\"\"}},\"6b4b65f3-a243-48b5-8fea-e412bf2cf9f7\":{\"input_type\":\"static\",\"static_input\":{\"multiselect_value\":[]}},\"0e1330b2-0b91-462b-acf2-2772a02299f8\":{\"input_type\":\"static\",\"static_input\":{\"multiselect_value\":[],\"select_value\":\"eb8f0588-a416-4bf9-9154-665ed20bcdf9\"}},\"4d308c31-9056-4d34-b977-99d58f89076c\":{\"input_type\":\"static\",\"static_input\":{\"multiselect_value\":[],\"text_value\":\"\"}},\"5eaaeb87-cb70-4877-aa5e-0a5b10f73f3a\":{\"input_type\":\"static\",\"static_input\":{\"multiselect_value\":[]}},\"8690362f-626a-4c93-a68e-c2fb3b746003\":{\"input_type\":\"static\",\"static_input\":{\"multiselect_value\":[]}},\"5ad21089-a73c-4408-ae52-d636e154351c\":{\"input_type\":\"static\",\"static_input\":{\"multiselect_value\":[]}}},\"pre_processing_script\":\"inputs.scheduler_type = getattr(playbook.inputs, \\\"schedule_type\\\", \\\"cron\\\")\\n\\nif getattr(playbook.inputs, \\\"schedule_type\\\", \\\"cron\\\") == \\\"date\\\":\\n  # date format converted to use dashes\\n  inputs.scheduler_type_value = getattr(playbook.inputs, \\\"schedule_type_value\\\", \\\"\\\").replace(\\\"/\\\", \\\"-\\\")\\nelse:\\n  inputs.scheduler_type_value = getattr(playbook.inputs, \\\"schedule_type_value\\\", \\\"\\\")\\n\\ninputs.scheduler_rule_name = getattr(playbook.inputs, \\\"schedule_rule_name\\\", None)\\ninputs.scheduler_rule_parameters = getattr(playbook.inputs, \\\"schedule_rule_parameters\\\", None)\\ninputs.scheduler_label_prefix = getattr(playbook.inputs, \\\"schedule_label_prefix\\\", None)\\ninputs.incident_id = incident.id\\ninputs.scheduler_is_playbook = getattr(playbook.inputs, \\\"schedule_is_playbook\\\", False)\\n\",\"pre_processing_script_language\":\"python3\",\"result_name\":\"output_scheduled_rule_create\"}</resilient:function></extensionElements><incoming>Flow_162tnn7</incoming><outgoing>Flow_00vaatr</outgoing></serviceTask><sequenceFlow id=\"Flow_162tnn7\" sourceRef=\"StartEvent_155asxm\" targetRef=\"ServiceTask_1\"/><sequenceFlow id=\"Flow_00vaatr\" sourceRef=\"ServiceTask_1\" targetRef=\"ScriptTask_4\"/><endEvent id=\"EndPoint_3\" resilient:documentation=\"End point\"><incoming>Flow_1u0jgw1</incoming></endEvent><scriptTask id=\"ScriptTask_4\" name=\"Write scheduled job to DataTable\"><extensionElements><resilient:script uuid=\"38d9b9df-35c7-48ec-adec-8a082f5be517\"/></extensionElements><incoming>Flow_00vaatr</incoming><outgoing>Flow_1m4jj08</outgoing><script>script</script></scriptTask><sequenceFlow id=\"Flow_1m4jj08\" sourceRef=\"ScriptTask_4\" targetRef=\"ServiceTask_7\"/><scriptTask id=\"ScriptTask_5\" name=\"limestone_script\"><extensionElements><resilient:script uuid=\"8486e707-2ad9-48bb-b995-0cd81788dc2d\"/></extensionElements><incoming>Flow_12srssw</incoming><outgoing>Flow_0cf7sfi</outgoing><script>script</script></scriptTask><scriptTask id=\"ScriptTask_6\" name=\"syl_script\"><extensionElements><resilient:script uuid=\"9bcaae01-3521-4385-bee3-2c078e76d053\"/></extensionElements><incoming>Flow_0cf7sfi</incoming><outgoing>Flow_0i0zmgt</outgoing><script>script</script></scriptTask><sequenceFlow id=\"Flow_0cf7sfi\" sourceRef=\"ScriptTask_5\" targetRef=\"ScriptTask_6\"/><sequenceFlow id=\"Flow_0i0zmgt\" sourceRef=\"ScriptTask_6\" targetRef=\"ScriptTask_8\"/><serviceTask id=\"ServiceTask_7\" name=\"Scheduled Rule Pause\" resilient:type=\"function\"><extensionElements><resilient:function uuid=\"aa278752-98c2-4866-b477-0eb19fd81b34\">{\"inputs\":{},\"pre_processing_script\":\"'''\\n\\n\\n\\nPREPROCESSING FUNCTION\\n\\n\\n\\n\\n'''\",\"pre_processing_script_language\":\"python3\",\"result_name\":\"output_scheduler_pause\"}</resilient:function></extensionElements><incoming>Flow_1m4jj08</incoming><outgoing>Flow_12srssw</outgoing></serviceTask><sequenceFlow id=\"Flow_12srssw\" sourceRef=\"ServiceTask_7\" targetRef=\"ScriptTask_5\"/><scriptTask id=\"ScriptTask_8\" name=\"workflow_calvin_global_Script\"><extensionElements><resilient:script uuid=\"c423148c-c842-43e6-ae32-bb763f72cecf\"/></extensionElements><incoming>Flow_0i0zmgt</incoming><outgoing>Flow_1u0jgw1</outgoing><script>script</script></scriptTask><sequenceFlow id=\"Flow_1u0jgw1\" sourceRef=\"ScriptTask_8\" targetRef=\"EndPoint_3\"/></process><bpmndi:BPMNDiagram id=\"BPMNDiagram_1\"><bpmndi:BPMNPlane bpmnElement=\"playbook_f9bcb3b9_fe40_40e8_87eb_f761ed94a4a7\" id=\"BPMNPlane_1\"><bpmndi:BPMNEdge bpmnElement=\"Flow_12srssw\" id=\"Flow_12srssw_di\"><omgdi:waypoint x=\"700\" y=\"552\"/><omgdi:waypoint x=\"700\" y=\"588\"/></bpmndi:BPMNEdge><bpmndi:BPMNEdge bpmnElement=\"Flow_0i0zmgt\" id=\"Flow_0i0zmgt_di\"><omgdi:waypoint x=\"700\" y=\"782\"/><omgdi:waypoint x=\"700\" y=\"808\"/></bpmndi:BPMNEdge><bpmndi:BPMNEdge bpmnElement=\"Flow_0cf7sfi\" id=\"Flow_0cf7sfi_di\"><omgdi:waypoint x=\"700\" y=\"672\"/><omgdi:waypoint x=\"700\" y=\"698\"/></bpmndi:BPMNEdge><bpmndi:BPMNEdge bpmnElement=\"Flow_1m4jj08\" id=\"Flow_1m4jj08_di\"><omgdi:waypoint x=\"700\" y=\"422\"/><omgdi:waypoint x=\"700\" y=\"468\"/></bpmndi:BPMNEdge><bpmndi:BPMNEdge bpmnElement=\"Flow_00vaatr\" id=\"Flow_00vaatr_di\"><omgdi:waypoint x=\"700\" y=\"272\"/><omgdi:waypoint x=\"700\" y=\"338\"/></bpmndi:BPMNEdge><bpmndi:BPMNEdge bpmnElement=\"Flow_162tnn7\" id=\"Flow_162tnn7_di\"><omgdi:waypoint x=\"700\" y=\"117\"/><omgdi:waypoint x=\"700\" y=\"188\"/></bpmndi:BPMNEdge><bpmndi:BPMNEdge bpmnElement=\"Flow_1u0jgw1\" id=\"Flow_1u0jgw1_di\"><omgdi:waypoint x=\"700\" y=\"892\"/><omgdi:waypoint x=\"700\" y=\"918\"/><omgdi:waypoint x=\"694\" y=\"918\"/><omgdi:waypoint x=\"694\" y=\"944\"/></bpmndi:BPMNEdge><bpmndi:BPMNShape bpmnElement=\"StartEvent_155asxm\" id=\"StartEvent_155asxm_di\"><omgdc:Bounds height=\"52\" width=\"187.083\" x=\"600\" y=\"65\"/><bpmndi:BPMNLabel><omgdc:Bounds height=\"0\" width=\"90\" x=\"616\" y=\"100\"/></bpmndi:BPMNLabel></bpmndi:BPMNShape><bpmndi:BPMNShape bpmnElement=\"ServiceTask_1\" id=\"ServiceTask_1_di\"><omgdc:Bounds height=\"84\" width=\"196\" x=\"602\" y=\"188\"/></bpmndi:BPMNShape><bpmndi:BPMNShape bpmnElement=\"ScriptTask_4\" id=\"ScriptTask_4_di\"><omgdc:Bounds height=\"84\" width=\"196\" x=\"602\" y=\"338\"/></bpmndi:BPMNShape><bpmndi:BPMNShape bpmnElement=\"ScriptTask_5\" id=\"ScriptTask_5_di\"><omgdc:Bounds height=\"84\" width=\"196\" x=\"602\" y=\"588\"/></bpmndi:BPMNShape><bpmndi:BPMNShape bpmnElement=\"ScriptTask_6\" id=\"ScriptTask_6_di\"><omgdc:Bounds height=\"84\" width=\"196\" x=\"602\" y=\"698\"/></bpmndi:BPMNShape><bpmndi:BPMNShape bpmnElement=\"ServiceTask_7\" id=\"ServiceTask_7_di\"><omgdc:Bounds height=\"84\" width=\"196\" x=\"601.5\" y=\"467.5\"/></bpmndi:BPMNShape><bpmndi:BPMNShape bpmnElement=\"ScriptTask_8\" id=\"ScriptTask_8_di\"><omgdc:Bounds height=\"84\" width=\"196\" x=\"601.5\" y=\"807.5\"/></bpmndi:BPMNShape><bpmndi:BPMNShape bpmnElement=\"EndPoint_3\" id=\"EndPoint_3_di\"><omgdc:Bounds height=\"52\" width=\"132.15\" x=\"628\" y=\"944\"/></bpmndi:BPMNShape></bpmndi:BPMNPlane></bpmndi:BPMNDiagram></definitions>"
+            },
+            "create_date": 1682673556531,
+            "creator_principal": {
+                "display_name": "Admin User",
+                "id": 1,
+                "name": "admin@example.com",
+                "type": "user"
+            },
+            "deployment_id": "playbook_f9bcb3b9_fe40_40e8_87eb_f761ed94a4a7",
+            "description": {
+                "content": "Schedule a rule/playbook to run in the future for a given incident",
+                "format": "text"
+            },
+            "display_name": "test_resilient_sdk",
+            "export_key": "test_resilient_sdk",
+            "field_type_handle": "playbook_f9bcb3b9_fe40_40e8_87eb_f761ed94a4a7",
+            "fields_type": {
+                "actions": [],
+                "display_name": "test_resilient_sdk",
+                "export_key": "playbook_f9bcb3b9_fe40_40e8_87eb_f761ed94a4a7",
+                "fields": {
+                    "schedule_is_playbook": {
+                        "allow_default_value": false,
+                        "blank_option": false,
+                        "calculated": false,
+                        "changeable": true,
+                        "chosen": false,
+                        "default_chosen_by_server": false,
+                        "deprecated": false,
+                        "export_key": "playbook_f9bcb3b9_fe40_40e8_87eb_f761ed94a4a7/schedule_is_playbook",
+                        "hide_notification": false,
+                        "id": 816,
+                        "input_type": "boolean",
+                        "internal": false,
+                        "is_tracked": false,
+                        "name": "schedule_is_playbook",
+                        "operation_perms": {},
+                        "operations": [],
+                        "placeholder": "",
+                        "prefix": null,
+                        "read_only": false,
+                        "required": "always",
+                        "rich_text": false,
+                        "tags": [],
+                        "templates": [],
+                        "text": "Is Playbook",
+                        "tooltip": "Yes - Playbook, No - Rule",
+                        "type_id": 1044,
+                        "uuid": "ab04da71-366c-4362-a918-52207f34efc1",
+                        "values": []
+                    },
+                    "schedule_label_prefix": {
+                        "allow_default_value": false,
+                        "blank_option": false,
+                        "calculated": false,
+                        "changeable": true,
+                        "chosen": false,
+                        "default_chosen_by_server": false,
+                        "deprecated": false,
+                        "export_key": "playbook_f9bcb3b9_fe40_40e8_87eb_f761ed94a4a7/schedule_label_prefix",
+                        "hide_notification": false,
+                        "id": 817,
+                        "input_type": "text",
+                        "internal": false,
+                        "is_tracked": false,
+                        "name": "schedule_label_prefix",
+                        "operation_perms": {},
+                        "operations": [],
+                        "placeholder": "",
+                        "prefix": null,
+                        "read_only": false,
+                        "required": "always",
+                        "rich_text": false,
+                        "tags": [],
+                        "templates": [],
+                        "text": "Schedule Label Prefix",
+                        "tooltip": "name of schedule for future reference",
+                        "type_id": 1044,
+                        "uuid": "acfcc667-5781-423f-88a7-b70b480229ad",
+                        "values": []
+                    },
+                    "schedule_rule_name": {
+                        "allow_default_value": false,
+                        "blank_option": false,
+                        "calculated": false,
+                        "changeable": true,
+                        "chosen": false,
+                        "default_chosen_by_server": false,
+                        "deprecated": false,
+                        "export_key": "playbook_f9bcb3b9_fe40_40e8_87eb_f761ed94a4a7/schedule_rule_name",
+                        "hide_notification": false,
+                        "id": 818,
+                        "input_type": "text",
+                        "internal": false,
+                        "is_tracked": false,
+                        "name": "schedule_rule_name",
+                        "operation_perms": {},
+                        "operations": [],
+                        "placeholder": "",
+                        "prefix": null,
+                        "read_only": false,
+                        "required": "always",
+                        "rich_text": false,
+                        "tags": [],
+                        "templates": [],
+                        "text": "Schedule Rule Name",
+                        "tooltip": "Name of Rule to schedule",
+                        "type_id": 1044,
+                        "uuid": "f1ee326f-bd1f-44a8-bd6b-91461ca201d7",
+                        "values": []
+                    },
+                    "schedule_rule_parameters": {
+                        "allow_default_value": false,
+                        "blank_option": false,
+                        "calculated": false,
+                        "changeable": true,
+                        "chosen": false,
+                        "default_chosen_by_server": false,
+                        "deprecated": false,
+                        "export_key": "playbook_f9bcb3b9_fe40_40e8_87eb_f761ed94a4a7/schedule_rule_parameters",
+                        "hide_notification": false,
+                        "id": 819,
+                        "input_type": "text",
+                        "internal": false,
+                        "is_tracked": false,
+                        "name": "schedule_rule_parameters",
+                        "operation_perms": {},
+                        "operations": [],
+                        "placeholder": "schedule_type=cron; schedule_value= * 5 * * *",
+                        "prefix": null,
+                        "read_only": false,
+                        "rich_text": false,
+                        "tags": [],
+                        "templates": [],
+                        "text": "Schedule Rule Parameters",
+                        "tooltip": "field1=value;field2=value format of optional rule parameters",
+                        "type_id": 1044,
+                        "uuid": "51a05941-e06f-4ff1-8f33-c876f43efc17",
+                        "values": []
+                    },
+                    "schedule_type": {
+                        "allow_default_value": false,
+                        "blank_option": false,
+                        "calculated": false,
+                        "changeable": true,
+                        "chosen": false,
+                        "default_chosen_by_server": false,
+                        "deprecated": false,
+                        "export_key": "playbook_f9bcb3b9_fe40_40e8_87eb_f761ed94a4a7/schedule_type",
+                        "hide_notification": false,
+                        "id": 820,
+                        "input_type": "select",
+                        "internal": false,
+                        "is_tracked": false,
+                        "name": "schedule_type",
+                        "operation_perms": {},
+                        "operations": [],
+                        "placeholder": "",
+                        "prefix": null,
+                        "read_only": false,
+                        "rich_text": false,
+                        "tags": [],
+                        "templates": [],
+                        "text": "Schedule Type",
+                        "tooltip": "",
+                        "type_id": 1044,
+                        "uuid": "6b5e8cd7-78c2-4acd-9b8a-a27bcac9cb0e",
+                        "values": [
+                            {
+                                "default": false,
+                                "enabled": true,
+                                "hidden": false,
+                                "label": "cron",
+                                "properties": null,
+                                "uuid": "7700f03e-af26-4379-b3f5-a8f4739f7605",
+                                "value": 136
+                            },
+                            {
+                                "default": false,
+                                "enabled": true,
+                                "hidden": false,
+                                "label": "date",
+                                "properties": null,
+                                "uuid": "dc31d35b-9751-4f5e-a395-ce79d791582d",
+                                "value": 137
+                            },
+                            {
+                                "default": false,
+                                "enabled": true,
+                                "hidden": false,
+                                "label": "delta",
+                                "properties": null,
+                                "uuid": "64097d31-caa8-48a5-b7af-db5a5740e44a",
+                                "value": 138
+                            },
+                            {
+                                "default": false,
+                                "enabled": true,
+                                "hidden": false,
+                                "label": "interval",
+                                "properties": null,
+                                "uuid": "98bbe7c0-37d0-4350-bdcf-24867ab158ca",
+                                "value": 139
+                            }
+                        ]
+                    },
+                    "schedule_type_value": {
+                        "allow_default_value": false,
+                        "blank_option": false,
+                        "calculated": false,
+                        "changeable": true,
+                        "chosen": false,
+                        "default_chosen_by_server": false,
+                        "deprecated": false,
+                        "export_key": "playbook_f9bcb3b9_fe40_40e8_87eb_f761ed94a4a7/schedule_type_value",
+                        "hide_notification": false,
+                        "id": 821,
+                        "input_type": "text",
+                        "internal": false,
+                        "is_tracked": false,
+                        "name": "schedule_type_value",
+                        "operation_perms": {},
+                        "operations": [],
+                        "placeholder": "cron (* 5 * * *); date (yyyy/mm/dd hh:mm:ss) ; interval (10m)",
+                        "prefix": null,
+                        "read_only": false,
+                        "required": "always",
+                        "rich_text": false,
+                        "tags": [],
+                        "templates": [],
+                        "text": "Schedule Type Value",
+                        "tooltip": "cron (* 5 * * *); date (yyyy/mm/dd hh:mm:ss) ; interval (10m)",
+                        "type_id": 1044,
+                        "uuid": "d51de07e-eaac-47cf-8bc8-e92276c1d879",
+                        "values": []
+                    }
+                },
+                "for_actions": false,
+                "for_custom_fields": false,
+                "for_notifications": false,
+                "for_workflows": false,
+                "id": null,
+                "parent_types": [
+                    "__playbook"
+                ],
+                "properties": {
+                    "can_create": false,
+                    "can_destroy": false,
+                    "for_who": []
+                },
+                "scripts": [],
+                "tags": [],
+                "type_id": 28,
+                "type_name": "playbook_f9bcb3b9_fe40_40e8_87eb_f761ed94a4a7",
+                "uuid": "945c6914-4efc-4ff3-b904-5c2ed885c89d"
+            },
+            "has_logical_errors": false,
+            "id": 42,
+            "is_deleted": false,
+            "is_locked": false,
+            "last_modified_principal": {
+                "display_name": "Admin User",
+                "id": 1,
+                "name": "admin@example.com",
+                "type": "user"
+            },
+            "last_modified_time": 1683119617190,
+            "local_scripts": [
+                {
+                    "actions": [],
+                    "created_date": 1682673556664,
+                    "creator_id": "admin@example.com",
+                    "description": "ASCII art : limestone",
+                    "enabled": false,
+                    "export_key": "limestone_script",
+                    "id": 41,
+                    "language": "python3",
+                    "last_modified_by": "admin@example.com",
+                    "last_modified_time": 1682673556673,
+                    "name": "limestone_script",
+                    "object_type": "incident",
+                    "playbook_handle": "test_resilient_sdk",
+                    "programmatic_name": "test_resilient_sdk_limestone_script",
+                    "script_text": "'''\n  \\/________________        \n /     _____________)\n/     /     /   \\ |         \n\\/\\/\\/     (O) (O)|           \n  |           ------, \n  |  _       ______/ \n  | (_      /   \\  \\\n  |        /  ___\\_ \\       \n  |        \\      / / \n__|_________\\______/\n\\______________\\./__\\   \n /     .       | \\  |\n \\    /_\\   .  |  \\ |\\     \n |`\\       /_\\ |   \\| \\\n'''",
+                    "tags": [],
+                    "uuid": "8486e707-2ad9-48bb-b995-0cd81788dc2d"
+                },
+                {
+                    "actions": [],
+                    "created_date": 1682673556675,
+                    "creator_id": "admin@example.com",
+                    "description": "ASCII art : syl",
+                    "enabled": false,
+                    "export_key": "syl_script",
+                    "id": 42,
+                    "language": "python3",
+                    "last_modified_by": "admin@example.com",
+                    "last_modified_time": 1682673556684,
+                    "name": "syl_script",
+                    "object_type": "incident",
+                    "playbook_handle": "test_resilient_sdk",
+                    "programmatic_name": "test_resilient_sdk_syl_script",
+                    "script_text": "'''\n               / ,\n          /\\  \\|/  /\\\n          |\\\\_;=._//|\n           \\.\"   \"./\n           //^\\ /^\\\\\n    .'``\",/ |0| |0| \\,\"``'.\n   /   ,  `'\\.---./'`  ,   \\\n  /`  /`\\,.\"(     )\".,/`\\  `\\\n  /`     ( '.'-.-'.' )     `\\\n  /\"`     \"._  :  _.\"     `\"\\\n   `/.'`\"=.,_``=``_,.=\"`'.\\`\n             )   (\n'''",
+                    "tags": [],
+                    "uuid": "9bcaae01-3521-4385-bee3-2c078e76d053"
+                }
+            ],
+            "manual_settings": {
+                "activation_conditions": {
+                    "conditions": [],
+                    "logic_type": "all"
+                },
+                "view_items": [
+                    {
+                        "content": "6b5e8cd7-78c2-4acd-9b8a-a27bcac9cb0e",
+                        "element": "field_uuid",
+                        "field_type": "playbook_f9bcb3b9_fe40_40e8_87eb_f761ed94a4a7",
+                        "show_if": null,
+                        "show_link_header": false,
+                        "step_label": null
+                    },
+                    {
+                        "content": "d51de07e-eaac-47cf-8bc8-e92276c1d879",
+                        "element": "field_uuid",
+                        "field_type": "playbook_f9bcb3b9_fe40_40e8_87eb_f761ed94a4a7",
+                        "show_if": null,
+                        "show_link_header": false,
+                        "step_label": null
+                    },
+                    {
+                        "content": "f1ee326f-bd1f-44a8-bd6b-91461ca201d7",
+                        "element": "field_uuid",
+                        "field_type": "playbook_f9bcb3b9_fe40_40e8_87eb_f761ed94a4a7",
+                        "show_if": null,
+                        "show_link_header": false,
+                        "step_label": null
+                    },
+                    {
+                        "content": "ab04da71-366c-4362-a918-52207f34efc1",
+                        "element": "field_uuid",
+                        "field_type": "playbook_f9bcb3b9_fe40_40e8_87eb_f761ed94a4a7",
+                        "show_if": null,
+                        "show_link_header": false,
+                        "step_label": null
+                    },
+                    {
+                        "content": "51a05941-e06f-4ff1-8f33-c876f43efc17",
+                        "element": "field_uuid",
+                        "field_type": "playbook_f9bcb3b9_fe40_40e8_87eb_f761ed94a4a7",
+                        "show_if": null,
+                        "show_link_header": false,
+                        "step_label": null
+                    },
+                    {
+                        "content": "acfcc667-5781-423f-88a7-b70b480229ad",
+                        "element": "field_uuid",
+                        "field_type": "playbook_f9bcb3b9_fe40_40e8_87eb_f761ed94a4a7",
+                        "show_if": null,
+                        "show_link_header": false,
+                        "step_label": null
+                    }
+                ]
+            },
+            "name": "test_resilient_sdk",
+            "object_type": "incident",
+            "status": "draft",
+            "tag": {
+                "display_name": "Playbook_f9bcb3b9-fe40-40e8-87eb-f761ed94a4a7",
+                "id": 44,
+                "name": "playbook_f9bcb3b9_fe40_40e8_87eb_f761ed94a4a7",
+                "type": "playbook",
+                "uuid": "83744eb7-bf95-4e2b-a0ca-c39c2f691a58"
+            },
+            "tags": [],
+            "type": "default",
+            "uuid": "f9bcb3b9-fe40-40e8-87eb-f761ed94a4a7",
+            "version": 13
         }
     ],
     "regulators": null,
     "roles": [
         {
             "description": "Manage all incidents and run simulations.",
             "display_name": "Administrator",
@@ -47901,14 +48491,78 @@
             "name": "test script",
             "object_type": "incident",
             "playbook_handle": null,
             "programmatic_name": "test_script",
             "script_text": "import json\n\ndef test_results():\n    # is object non null\n    if not results:\n        helper.fail(\"results object is None\")\n    # does object contain the success property\n    if not isinstance(results.get('success', None), bool):\n      helper.fail(\"results.success not found or not bool\")\n     # does the object have a content property\n    if not isinstance(results.get('content', None), (str, dict, list)):\n      helper.fail(\"results.content not found or not string, dict or list\")\n    # if success if False, is there a reason\n    if not results.success and not results.reason:\n      helper.fail(\"results.success = False and missing results.reason\")\n    # is the content json string encoded (BAD)\n    if isinstance(results.content, str):\n      try:\n        json.loads(results.content)\n        helper.fail(\"results.content appears to be string encoded json. Return json instead\")\n      except Exception:\n        pass\n    # does the content return the api content or the python requests response object (bad)\n    if isinstance(results.content, bool) and results.content.get('apparent_encoding'):\n        helper.fail(\"request response object returned. Return response.json() or response.text instead\")\n\n\nresults = workflow.properties.test_results\ntest_results()\n\n# return the results in a note for review\ncontent = json.dumps(results.content, indent=3) if isinstance(results.content, bool) else results.content\nnote = \"success: {}\\nreason: {}\\ncontent type: {}\\ncontent: {}\".format(results.success, results.reason, type(results.content), content)\nincident.addNote(helper.createPlainText(note))\nnote1= workflow.properties.name\nincident.addNote(helper.createPlainText(note1))",
             "tags": [],
             "uuid": "4751e689-4f49-45e0-8f72-041b622440b8"
+        },
+        {
+            "actions": [],
+            "created_date": 1681819042470,
+            "creator_id": "admin@example.com",
+            "description": "Write out scheduled job information to a datatable",
+            "enabled": false,
+            "export_key": "Write scheduled job to DataTable",
+            "id": 29,
+            "language": "python3",
+            "last_modified_by": "admin@example.com",
+            "last_modified_time": 1681819042473,
+            "name": "Write scheduled job to DataTable",
+            "object_type": "incident",
+            "playbook_handle": null,
+            "programmatic_name": "write_scheduled_job_to_datatable",
+            "script_text": "from datetime import datetime\n\nresults = playbook.functions.results.output_scheduled_rule_create\nnow = datetime.now().strftime(\"%Y-%m-%d %H:%M:%S\") # '2023-03-24 11:28:34'\nTYPE_LOOKUP = {\n  0: 'Incident',\n  1: \"Task\",\n  4: \"Artifact\",\n  5: \"Attachment\"}\n\nif results.get(\"success\"):\n  job = results.get(\"content\")\n  row = incident.addRow(\"scheduler_rules\")\n  row['reported_on'] = now\n  row['schedule_label'] = job['id']\n  row['schedule_type'] = job['type']\n  row['incident_id'] = job['args'][0]\n  row['schedule'] = job['value']\n  row['status'] = 'Active'\n  row['next_run_time'] = job['next_run_time']\n  row['rule_type'] = TYPE_LOOKUP.get(job['args'][6], \"Datatable\")\n  if job['args'][8]:\n    row['rule'] = \"<a href='#playbooks/designer/{}'>{}</a>\".format(job['args'][5], job['args'][4])\n  else:\n    row['rule'] = \"<a href='#customize?tab=actions&id={}'>{}</a>\".format(job['args'][5], job['args'][4])\nelse:\n  incident.addNote(\"Schedule a Rule/Playbook failed: {}\".format(result.get(\"reason\")))",
+            "tags": [
+                {
+                    "tag_handle": "playbook_1881ad3e_e539_47e1_b6e5_6f1c84df0864",
+                    "value": "Playbook Tag"
+                },
+                {
+                    "tag_handle": "playbook_2405a12b_1f53_4ebf_b87e_d2f91866635a",
+                    "value": "Playbook Tag"
+                },
+                {
+                    "tag_handle": "playbook_a486c165_85d1_4d15_ac7a_e6b8352efc05",
+                    "value": "Playbook Tag"
+                },
+                {
+                    "tag_handle": "playbook_cb82c8f1_c294_4a01_8a3a_12e581bca983",
+                    "value": "Playbook Tag"
+                },
+                {
+                    "tag_handle": "playbook_f9bcb3b9_fe40_40e8_87eb_f761ed94a4a7",
+                    "value": "Playbook Tag"
+                }
+            ],
+            "uuid": "38d9b9df-35c7-48ec-adec-8a082f5be517"
+        },
+        {
+            "actions": [],
+            "created_date": 1682519277706,
+            "creator_id": "admin@example.com",
+            "description": "",
+            "enabled": false,
+            "export_key": "workflow_sample_global_Script",
+            "id": 39,
+            "language": "python3",
+            "last_modified_by": "admin@example.com",
+            "last_modified_time": 1682519277709,
+            "name": "workflow_sample_global_Script",
+            "object_type": "incident",
+            "playbook_handle": null,
+            "programmatic_name": "workflow_sample_global_script",
+            "script_text": "'''\n  \\/________________        \n /     _____________)\n/     /     /   \\ |         \n\\/\\/\\/     (O) (O)|           \n  |           ------, \n  |  _       ______/ \n  | (_      /   \\  \\\n  |        /  ___\\_ \\       \n  |        \\      / / \n__|_________\\______/\n\\______________\\./__\\   \n /     .       | \\  |\n \\    /_\\   .  |  \\ |\\     \n |`\\       /_\\ |   \\| \\\n'''",
+            "tags": [
+                {
+                    "tag_handle": "playbook_f9bcb3b9_fe40_40e8_87eb_f761ed94a4a7",
+                    "value": "Playbook Tag"
+                }
+            ],
+            "uuid": "c423148c-c842-43e6-ae32-bb763f72cecf"
         }
     ],
     "server_version": {
         "build_number": 7888,
         "major": 45,
         "minor": 0,
         "version": "45.0.7888"
```

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/resilient_api_data/export.JSON` & `resilient_sdk-49.0.4423/tests/shared_mock_data/resilient_api_data/export.JSON`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/resilient_api_data/orgs.JSON` & `resilient_sdk-49.0.4423/tests/shared_mock_data/resilient_api_data/orgs.JSON`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/resilient_api_data/session.JSON` & `resilient_sdk-49.0.4423/tests/shared_mock_data/resilient_api_data/session.JSON`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/shared_mock_data/resilient_api_mock.py` & `resilient_sdk-49.0.4423/tests/shared_mock_data/resilient_api_mock.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/unit/test_app.py` & `resilient_sdk-49.0.4423/tests/unit/test_app.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/unit/test_cmds/ext/test_ext_package.py` & `resilient_sdk-49.0.4423/tests/unit/test_cmds/ext/test_ext_package.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/unit/test_cmds/test_base_cmd.py` & `resilient_sdk-49.0.4423/tests/unit/test_cmds/test_base_cmd.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/unit/test_cmds/test_clone.py` & `resilient_sdk-49.0.4423/tests/unit/test_cmds/test_clone.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/unit/test_cmds/test_codegen.py` & `resilient_sdk-49.0.4423/tests/unit/test_cmds/test_codegen.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     'fn_main_mock_integration',
     'icons',
     'payload_samples',
     'setup.py',
     'tests',
     'tox.ini'
 ]
-
+PB_MD_FILE = "pb_test_resilient_sdk.md"
 EXPECTED_FILES_DATA_DIR = ['wf_mock_workflow_one.md', 'wf_mock_workflow_two.md']
 EXPECTED_FILES_DOC_DIR = ['screenshots']
 EXPECTED_FILES_DOC_SCREENSHOTS_DIR = ['main.png']
 EXPECTED_FILES_PACKAGE_DIR = ['LICENSE', '__init__.py', 'components', 'util', 'poller', 'lib']
 EXPECTED_FILES_PACKAGE_COMPONENTS_DIR = ['__init__.py', 'funct_mock_function_one.py', 'funct_mock_function_two.py']
 EXPECTED_FILES_PACKAGE_UTIL_DIR = ['__init__.py', 'config.py', 'customize.py', 'data', 'selftest.py']
 EXPECTED_FILES_PACKAGE_UTIL_DATA_DIR = ['export.res']
@@ -82,14 +82,30 @@
 
     if poller:
         assert helpers.verify_expected_list(EXPECTED_FILES_POLLER_DIR, os.listdir(os.path.join(package_path, package_name, "poller")))
         assert helpers.verify_expected_list(EXPECTED_FILES_POLLER_DATA_DIR, os.listdir(os.path.join(package_path, package_name, "poller", "data")))
         assert helpers.verify_expected_list(EXPECTED_FILES_LIB_DIR, os.listdir(os.path.join(package_path, package_name, "lib")))
 
 
+def compare_playbooks_md_file(package_name, package_path):
+    # Compares pb_test_resilient_sdk.md file generated by gen_package with the one in the mock_integration
+    assert PB_MD_FILE in os.listdir(os.path.join(package_path, "data"))
+    with open(os.path.join(mock_paths.MOCK_INT_FN_MAIN_MOCK_INTEGRATION, "data", PB_MD_FILE)) as expected_md_file:
+        expected_md = expected_md_file.readlines()
+    with open(os.path.join(package_path, "data", PB_MD_FILE)) as expected_md_file:
+        generated_md = expected_md_file.readlines()
+
+    len(generated_md) > 0 # checking if file is not empty
+    assert len(expected_md) == len(generated_md) 
+    
+    expected_md, generated_md = expected_md[7:], generated_md[7:] # removing the first 7 lines of the file as resilient_sdk version can change
+    for exp, gen in zip(expected_md, generated_md):
+        assert exp == gen
+
+
 def test_cmd_codegen(fx_get_sub_parser, fx_cmd_line_args_codegen_package):
     cmd_codegen = CmdCodegen(fx_get_sub_parser)
 
     assert isinstance(cmd_codegen, base_cmd.BaseCmd)
     assert cmd_codegen.CMD_NAME == "codegen"
     assert cmd_codegen.CMD_HELP == "Generates boilerplate code used to begin developing an app."
     assert cmd_codegen.CMD_USAGE == """
@@ -193,14 +209,43 @@
     files_in_components = sorted(os.listdir(os.path.join(mock_paths.TEST_TEMP_DIR, "test_package", "components")))
     assert files_in_components == ['__init__.py']
 
     customize_py = sdk_helpers.read_file(os.path.join(mock_paths.TEST_TEMP_DIR, "test_package", "util", "customize.py"))
     assert '        "functions": [u"fn_mock_function_1", u"fn_mock_function_2"],\n' in customize_py
 
 
+def test_gen_package_with_playbooks(fx_get_sub_parser, fx_reset_argv, fx_mk_temp_dir, fx_add_dev_env_var):
+    """
+    This tests that when a package is generated with codegen
+    that each of the EXPECTED_FILES exist in each directory.
+    This test is NOT concerned about the contents of each file,
+    just that it exists
+    """
+    output_path = mock_paths.TEST_TEMP_DIR
+    constants.CURRENT_SOAR_SERVER_VERSION = 46.0 # setting SOAR server version to 46.0
+
+    # Add paths to an output base and an export.res file
+    sys.argv.extend(["codegen"])
+    sys.argv.extend(["-p", "test_resilient_sdk_with_playbooks"])
+    sys.argv.extend(["-pb", "test_resilient_sdk"])
+    sys.argv.extend(["-f", "create_a_scheduled_rule", "scheduled_rule_pause"])
+    sys.argv.extend(["-o", output_path])
+    sys.argv.extend(["-e", os.path.join(mock_paths.SHARED_MOCK_DATA_DIR, mock_paths.RESILIENT_API_DATA, "export-with-playbook.JSON")])
+
+    cmd_codegen = CmdCodegen(fx_get_sub_parser)
+    args = cmd_codegen.parser.parse_known_args()[0]
+    cmd_codegen._gen_package(args)
+
+    package_name = args.package
+    package_path = os.path.join(output_path, args.package)
+    compare_playbooks_md_file(package_name, package_path)
+    
+    constants.CURRENT_SOAR_SERVER_VERSION = 39.0 # resetting SOAR server version back to 39.0
+
+
 def test_run_tests_with_settings_file(fx_get_sub_parser, fx_mk_temp_dir, fx_mock_res_client, fx_cmd_line_args_codegen_package):
     with patch("resilient_sdk.cmds.codegen.sdk_helpers.get_resilient_client") as mock_client:
 
         mock_client.return_value = fx_mock_res_client
         output_path = mock_paths.TEST_TEMP_DIR
 
         # Add paths to an output base and an export.res file
```

### Comparing `resilient_sdk-48.2.4321/tests/unit/test_cmds/test_dev.py` & `resilient_sdk-49.0.4423/tests/unit/test_cmds/test_dev.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/unit/test_cmds/test_docgen.py` & `resilient_sdk-49.0.4423/tests/unit/test_cmds/test_docgen.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/unit/test_cmds/test_extract.py` & `resilient_sdk-49.0.4423/tests/unit/test_cmds/test_extract.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/unit/test_cmds/test_run_init.py` & `resilient_sdk-49.0.4423/tests/unit/test_cmds/test_run_init.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/unit/test_cmds/test_validate.py` & `resilient_sdk-49.0.4423/tests/unit/test_cmds/test_validate.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/unit/test_util/test_jinja_filters.py` & `resilient_sdk-49.0.4423/tests/unit/test_util/test_jinja_filters.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/unit/test_util/test_package_file_helpers.py` & `resilient_sdk-49.0.4423/tests/unit/test_util/test_package_file_helpers.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/unit/test_util/test_resilient_objects.py` & `resilient_sdk-49.0.4423/tests/unit/test_util/test_resilient_objects.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/unit/test_util/test_sdk_exception.py` & `resilient_sdk-49.0.4423/tests/unit/test_util/test_sdk_exception.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/unit/test_util/test_sdk_helpers.py` & `resilient_sdk-49.0.4423/tests/unit/test_util/test_sdk_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -284,14 +284,42 @@
         constants.CURRENT_SOAR_SERVER_VERSION = 44.0
         org_export = sdk_helpers.get_latest_org_export(fx_mock_res_client)
         export_data = sdk_helpers.get_from_export(org_export, playbooks=["main_mock_playbook"])
 
         assert export_data.get("playbooks")[0].get(ResilientObjMap.PLAYBOOKS) == "main_mock_playbook"
         constants.CURRENT_SOAR_SERVER_VERSION = None # reset for other tests
 
+def test_get_playbooks_with_functions_and_script(fx_mock_res_client):
+    with patch("resilient_sdk.util.sdk_helpers.get_resilient_server_version") as mock_server_version:
+
+        mock_server_version.return_value = 44.0
+        constants.CURRENT_SOAR_SERVER_VERSION = 44.0
+        org_export = sdk_helpers.get_latest_org_export(fx_mock_res_client)
+        export_data = sdk_helpers.get_from_export(org_export, playbooks=["test_resilient_sdk"])
+
+        assert export_data.get("playbooks")[0].get(ResilientObjMap.PLAYBOOKS) == "test_resilient_sdk"
+        assert len(export_data.get("playbooks")[0].get("pb_functions")) == 2
+        for function in export_data.get("playbooks")[0].get("pb_functions"):
+            assert "pre_processing_script" in function
+            assert function.get("pre_processing_script") is not None
+            assert "result_name" in function
+            assert "uuid" in function
+            assert "post_processing_script" not in function
+            
+        assert len(export_data.get("playbooks")[0].get("pb_scripts")) == 4
+        for script in export_data.get("playbooks")[0].get("pb_scripts"):
+            assert "uuid" in script
+            assert "name" in script
+            assert "script_type" in script
+            assert "description" in script
+            assert "object_type" in script
+            assert script.get("name") is not None
+            assert script.get("script_type") is not None
+
+        constants.CURRENT_SOAR_SERVER_VERSION = None # reset for other tests
 
 def test_get_playbooks_from_export_incompatible_version(fx_mock_res_client):
 
     org_export = sdk_helpers.get_latest_org_export(fx_mock_res_client)
 
     with pytest.raises(SDKException, match=r"Playbooks are only supported in resilient_sdk for IBM SOAR >= 44"):
         sdk_helpers.get_from_export(org_export, playbooks=["main_mock_playbook"])
@@ -436,14 +464,40 @@
 
 
 def test_get_workflow_functions():
     # TODO: taken from docgen
     pass
 
 
+def test_get_playbook_objects(fx_mock_res_client):
+    with patch("resilient_sdk.util.sdk_helpers.get_resilient_server_version") as mock_server_version:
+        playbook = None
+        mock_server_version.return_value = 44.0
+        constants.CURRENT_SOAR_SERVER_VERSION = 44.0
+        org_export = sdk_helpers.get_latest_org_export(fx_mock_res_client)
+
+        for pb in org_export.get("playbooks"):
+            if pb.get("export_key") == "test_resilient_sdk":
+                playbook = pb
+                break
+
+        assert playbook
+        pb_elements = sdk_helpers.get_playbook_objects(playbook)
+
+        assert "functions" in pb_elements
+        for function in pb_elements.get("functions"):
+            assert "uuid" in function
+            assert "result_name" in function
+            assert "pre_processing_script" in function
+
+        assert "scripts" in pb_elements
+        for script in pb_elements.get("scripts"):
+            assert "uuid" in script
+
+
 def test_get_main_cmd(monkeypatch):
     mock_args = ["resilient-sdk", "codegen", "-p", "fn_mock_package"]
     monkeypatch.setattr(sys, "argv", mock_args)
     main_cmd = sdk_helpers.get_main_cmd()
     assert main_cmd == "codegen"
```

### Comparing `resilient_sdk-48.2.4321/tests/unit/test_util/test_sdk_validate_configs.py` & `resilient_sdk-49.0.4423/tests/unit/test_util/test_sdk_validate_configs.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/unit/test_util/test_sdk_validate_helpers.py` & `resilient_sdk-49.0.4423/tests/unit/test_util/test_sdk_validate_helpers.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tests/unit/test_util/test_sdk_validate_issue.py` & `resilient_sdk-49.0.4423/tests/unit/test_util/test_sdk_validate_issue.py`

 * *Files identical despite different names*

### Comparing `resilient_sdk-48.2.4321/tox.ini` & `resilient_sdk-49.0.4423/tox.ini`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     pytest-cov
     pathlib ; python_version=="2.7"
 
 setenv = 
     SETUPTOOLS_SCM_PRETEND_VERSION={env:SETUPTOOLS_SCM_PRETEND_VERSION}
 
 commands = 
+    pip install ../resilient-app-config-plugins
     pip install ../resilient
     pip install ../resilient-lib
     pip install ../resilient-circuits
     pip install .
     pytest --cov --cov-report xml --capture=no tests/unit/ --durations=0
```

