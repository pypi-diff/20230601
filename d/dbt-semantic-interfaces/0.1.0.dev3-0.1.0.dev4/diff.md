# Comparing `tmp/dbt_semantic_interfaces-0.1.0.dev3.tar.gz` & `tmp/dbt_semantic_interfaces-0.1.0.dev4.tar.gz`

## Comparing `dbt_semantic_interfaces-0.1.0.dev3.tar` & `dbt_semantic_interfaces-0.1.0.dev4.tar`

### file list

```diff
@@ -1,99 +1,79 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/.tool-versions
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/CHANGELOG.md
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/Makefile
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/mypy.ini
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/__init__.py
--rw-r--r--   0        0        0    18186 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/dataclass_serialization.py
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/enum_extension.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/errors.py
--rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/pretty_print.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/py.typed
--rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/references.py
--rw-r--r--   0        0        0     6119 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/implementations/__init__.py
--rw-r--r--   0        0        0     7622 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/implementations/base.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/implementations/metadata.py
--rw-r--r--   0        0        0     7556 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/implementations/metric.py
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/implementations/semantic_manifest.py
--rw-r--r--   0        0        0     6502 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/implementations/semantic_model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/implementations/elements/__init__.py
--rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/implementations/elements/dimension.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/implementations/elements/entity.py
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/implementations/elements/measure.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/implementations/filters/__init__.py
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/implementations/filters/call_parameter_sets.py
--rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/implementations/filters/where_filter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/parsing/__init__.py
--rw-r--r--   0        0        0    13889 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/parsing/dir_to_model.py
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/parsing/explicit_schema.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/parsing/objects.py
--rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/parsing/schema_validator.py
--rw-r--r--   0        0        0     9628 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/parsing/schemas.py
--rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/parsing/yaml_loader.py
--rw-r--r--   0        0        0    14950 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/parsing/schemas/default_explicit_schema.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/protocols/__init__.py
--rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/protocols/dimension.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/protocols/entity.py
--rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/protocols/measure.py
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/protocols/metadata.py
--rw-r--r--   0        0        0     5436 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/protocols/metric.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/protocols/protocol_hint.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/protocols/semantic_manifest.py
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/protocols/semantic_model.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/protocols/where_filter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/transformations/__init__.py
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/transformations/add_input_metric_measures.py
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/transformations/agg_time_dimension.py
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/transformations/boolean_measure.py
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/transformations/convert_count.py
--rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/transformations/convert_median.py
--rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/transformations/names.py
--rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/transformations/proxy_measure.py
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/transformations/pydantic_rule_set.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/transformations/rule_set.py
--rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/transformations/semantic_manifest_transformer.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/transformations/transform_rule.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/type_enums/__init__.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/type_enums/aggregation_type.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/type_enums/dimension_type.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/type_enums/entity_type.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/type_enums/metric_type.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/type_enums/time_granularity.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/__init__.py
--rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/agg_time_dimension.py
--rw-r--r--   0        0        0     3891 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/common_entities.py
--rw-r--r--   0        0        0     7681 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/dimension_const.py
--rw-r--r--   0        0        0     4167 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/element_const.py
--rw-r--r--   0        0        0     5107 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/entities.py
--rw-r--r--   0        0        0    28504 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/measures.py
--rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/metrics.py
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/non_empty.py
--rw-r--r--   0        0        0     6827 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/reserved_keywords.py
--rw-r--r--   0        0        0     5150 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/semantic_manifest_validator.py
--rw-r--r--   0        0        0     9051 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/semantic_models.py
--rw-r--r--   0        0        0    10051 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/unique_valid_name.py
--rw-r--r--   0        0        0    14682 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/validator_helpers.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/venv-3.9.16/pyvenv.cfg
--rw-r--r--   0        0        0     8834 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/venv-3.9.16/bin/Activate.ps1
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/venv-3.9.16/bin/activate
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/venv-3.9.16/bin/activate.csh
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/venv-3.9.16/bin/activate.fish
--rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/venv-3.9.16/bin/hatch
--rwxr-xr-x   0        0        0      293 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/venv-3.9.16/bin/hatchling
--rwxr-xr-x   0        0        0      275 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/venv-3.9.16/bin/httpx
--rwxr-xr-x   0        0        0      281 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/venv-3.9.16/bin/keyring
--rwxr-xr-x   0        0        0      291 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/venv-3.9.16/bin/markdown-it
--rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/venv-3.9.16/bin/pip
--rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/venv-3.9.16/bin/pip3
--rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/venv-3.9.16/bin/pip3.9
--rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/venv-3.9.16/bin/pygmentize
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/venv-3.9.16/bin/python -> /Users/quigleymalcolm/.asdf/installs/python/3.9.16/bin/python
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/venv-3.9.16/bin/python3 -> python
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/venv-3.9.16/bin/python3.9 -> python
--rwxr-xr-x   0        0        0      290 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/venv-3.9.16/bin/userpath
--rwxr-xr-x   0        0        0      309 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/venv-3.9.16/bin/virtualenv
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/LICENSE
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/README.md
--rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/pyproject.toml
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/PKG-INFO
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/CHANGELOG.md
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/Makefile
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/mypy.ini
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/__init__.py
+-rw-r--r--   0        0        0    18186 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/dataclass_serialization.py
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/enum_extension.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/errors.py
+-rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/pretty_print.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/py.typed
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/references.py
+-rw-r--r--   0        0        0     6119 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/implementations/__init__.py
+-rw-r--r--   0        0        0     7622 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/implementations/base.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/implementations/metadata.py
+-rw-r--r--   0        0        0     7556 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/implementations/metric.py
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/implementations/semantic_manifest.py
+-rw-r--r--   0        0        0     6502 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/implementations/semantic_model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/implementations/elements/__init__.py
+-rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/implementations/elements/dimension.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/implementations/elements/entity.py
+-rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/implementations/elements/measure.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/implementations/filters/__init__.py
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/implementations/filters/call_parameter_sets.py
+-rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/implementations/filters/where_filter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/parsing/__init__.py
+-rw-r--r--   0        0        0    14122 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/parsing/dir_to_model.py
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/parsing/explicit_schema.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/parsing/objects.py
+-rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/parsing/schema_validator.py
+-rw-r--r--   0        0        0     9628 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/parsing/schemas.py
+-rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/parsing/yaml_loader.py
+-rw-r--r--   0        0        0    14950 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/parsing/schemas/default_explicit_schema.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/protocols/__init__.py
+-rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/protocols/dimension.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/protocols/entity.py
+-rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/protocols/measure.py
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/protocols/metadata.py
+-rw-r--r--   0        0        0     5436 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/protocols/metric.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/protocols/protocol_hint.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/protocols/semantic_manifest.py
+-rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/protocols/semantic_model.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/protocols/where_filter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/transformations/__init__.py
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/transformations/add_input_metric_measures.py
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/transformations/agg_time_dimension.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/transformations/boolean_measure.py
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/transformations/convert_count.py
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/transformations/convert_median.py
+-rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/transformations/names.py
+-rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/transformations/proxy_measure.py
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/transformations/pydantic_rule_set.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/transformations/rule_set.py
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/transformations/semantic_manifest_transformer.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/transformations/transform_rule.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/type_enums/__init__.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/type_enums/aggregation_type.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/type_enums/dimension_type.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/type_enums/entity_type.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/type_enums/metric_type.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/type_enums/time_granularity.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/__init__.py
+-rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/agg_time_dimension.py
+-rw-r--r--   0        0        0     3891 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/common_entities.py
+-rw-r--r--   0        0        0     7681 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/dimension_const.py
+-rw-r--r--   0        0        0     4167 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/element_const.py
+-rw-r--r--   0        0        0     5107 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/entities.py
+-rw-r--r--   0        0        0    28504 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/measures.py
+-rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/metrics.py
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/non_empty.py
+-rw-r--r--   0        0        0     6827 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/reserved_keywords.py
+-rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/semantic_manifest_validator.py
+-rw-r--r--   0        0        0     9051 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/semantic_models.py
+-rw-r--r--   0        0        0    10051 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/unique_valid_name.py
+-rw-r--r--   0        0        0    14682 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/validator_helpers.py
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/LICENSE
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/README.md
+-rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/pyproject.toml
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev4/PKG-INFO
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/Makefile` & `dbt_semantic_interfaces-0.1.0.dev4/Makefile`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/dataclass_serialization.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/dataclass_serialization.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/enum_extension.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/enum_extension.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/errors.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/errors.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/pretty_print.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/pretty_print.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/references.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/references.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/test_utils.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/test_utils.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/implementations/base.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/implementations/base.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/implementations/metric.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/implementations/metric.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/implementations/semantic_manifest.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/implementations/semantic_manifest.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/implementations/semantic_model.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/implementations/semantic_model.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/implementations/elements/dimension.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/implementations/elements/dimension.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/implementations/elements/entity.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/implementations/elements/entity.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/implementations/elements/measure.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/implementations/elements/measure.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/implementations/filters/call_parameter_sets.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/implementations/filters/call_parameter_sets.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/implementations/filters/where_filter.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/implementations/filters/where_filter.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/parsing/dir_to_model.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/parsing/dir_to_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,16 +39,16 @@
 VERSION_KEY = "mf_config_schema"
 METRIC_TYPE = "metric"
 SEMANTIC_MODEL_TYPE = "semantic_model"
 DOCUMENT_TYPES = [METRIC_TYPE, SEMANTIC_MODEL_TYPE]
 
 
 @dataclass(frozen=True)
-class ModelBuildResult:  # noqa: D
-    model: PydanticSemanticManifest
+class SemanticManifestBuildResult:  # noqa: D
+    semantic_manifest: PydanticSemanticManifest
     # Issues found in the model.
     issues: SemanticManifestValidationResults = SemanticManifestValidationResults()
 
 
 @dataclass(frozen=True)
 class FileParsingResult:
     """Results of parsing a config file.
@@ -85,40 +85,40 @@
 
             file_path = os.path.join(root, file)
             config_file_paths.append(file_path)
 
     return config_file_paths
 
 
-def parse_directory_of_yaml_files_to_model(
+def parse_directory_of_yaml_files_to_semantic_manifest(
     directory: str,
     template_mapping: Optional[Dict[str, str]] = None,
     apply_transformations: Optional[bool] = True,
     raise_issues_as_exceptions: bool = True,
-) -> ModelBuildResult:
+) -> SemanticManifestBuildResult:
     """Parse files in the given directory to a SemanticManifest.
 
     Strings in the file following the Python string template format are replaced
     according to the template_mapping dict.
     """
     file_paths = collect_yaml_config_file_paths(directory=directory)
-    return parse_yaml_file_paths_to_model(
+    return parse_yaml_file_paths_to_semantic_manifest(
         file_paths=file_paths,
         template_mapping=template_mapping,
         apply_transformations=apply_transformations,
         raise_issues_as_exceptions=raise_issues_as_exceptions,
     )
 
 
-def parse_yaml_file_paths_to_model(
+def parse_yaml_file_paths_to_semantic_manifest(
     file_paths: List[str],
     template_mapping: Optional[Dict[str, str]] = None,
     apply_transformations: Optional[bool] = True,
     raise_issues_as_exceptions: bool = True,
-) -> ModelBuildResult:
+) -> SemanticManifestBuildResult:
     """Parse files the given list of file paths to a SemanticManifest.
 
     Strings in the files following the Python string template format are replaced
     according to the template_mapping dict.
     """
     template_mapping = template_mapping or {}
     yaml_config_files = []
@@ -127,67 +127,67 @@
             with open(file_path) as f:
                 contents = Template(f.read()).substitute(template_mapping)
                 yaml_config_files.append(
                     YamlConfigFile(filepath=file_path, contents=contents),
                 )
         except UnicodeDecodeError as e:
             # We could alternatively return this as a validation issue, but this
-            # exception is hit *before* building the model. Currently the
-            # ModelBuildResult guarantees a SemanticManifest. We could make
+            # exception is hit *before* building the semantic manifest. Currently, the
+            # SemanticManifestBuildResult guarantees a SemanticManifest. We could make
             # SemanticManifest optional on ModelBuildResult, but this has
             # undesirable consequences.
             raise Exception(
                 f"The content of file `{file_path}` doesn't match the encoding of the file."
                 " If you know the encoding the content is in, try resaving the file with that encoding explicitly."
                 " Alternatively this error generally arises due to copy and pasted content,"
                 " try manually typing up the problem file instead of copy and pasting"
             ) from e
 
-    return parse_yaml_files_to_validation_ready_model(
+    return parse_yaml_files_to_validation_ready_semantic_manifest(
         yaml_config_files=yaml_config_files,
         apply_transformations=apply_transformations,
         raise_issues_as_exceptions=raise_issues_as_exceptions,
     )
 
 
-def parse_yaml_files_to_validation_ready_model(
+def parse_yaml_files_to_validation_ready_semantic_manifest(
     yaml_config_files: List[YamlConfigFile],
     apply_transformations: Optional[bool] = True,
     raise_issues_as_exceptions: bool = True,
-) -> ModelBuildResult:
+) -> SemanticManifestBuildResult:
     """Parse and transform the given set of in-memory YamlConfigFiles to a UserConfigured model.
 
     This model result is, by default, validation-ready, although different callsites (mainly in testing)
     might wish to override the transformation state.
 
     TODO: Restructure this module and provide an improved API for managing these different input types
     """
-    build_result = parse_yaml_files_to_model(yaml_config_files)
-    model = build_result.model
+    build_result = parse_yaml_files_to_semantic_manifest(yaml_config_files)
+    model = build_result.semantic_manifest
     assert model
 
     build_issues = build_result.issues
     try:
         if apply_transformations:
             model = PydanticSemanticManifestTransformer.transform(model)
     except Exception as e:
         transformation_issue_results = SemanticManifestValidationResults(errors=(ValidationError(message=str(e)),))
         build_issues = SemanticManifestValidationResults.merge([build_issues, transformation_issue_results])
 
     if raise_issues_as_exceptions and build_issues.has_blocking_issues:
         raise SemanticManifestValidationException(build_issues.all_issues)
 
-    return ModelBuildResult(model=model, issues=build_issues)
+    return SemanticManifestBuildResult(semantic_manifest=model, issues=build_issues)
 
 
-def parse_yaml_files_to_model(
+def parse_yaml_files_to_semantic_manifest(
     files: List[YamlConfigFile],
     semantic_model_class: Type[PydanticSemanticModel] = PydanticSemanticModel,
     metric_class: Type[PydanticMetric] = PydanticMetric,
-) -> ModelBuildResult:
+) -> SemanticManifestBuildResult:
     """Builds SemanticManifest from list of config files (as strings).
 
     Persistent storage connection may be passed to write parsed objects=
     to storage and populate object metadata
 
     Note: this function does not finalize the model
     """
@@ -214,16 +214,16 @@
                         context=FileContext(file_name=config_file.filepath),
                         message=f"Unexpected model object {obj.__class__.__name__}. Expected {valid_object_classes}.",
                     )
                 )
 
         issues += file_issues
 
-    return ModelBuildResult(
-        model=PydanticSemanticManifest(
+    return SemanticManifestBuildResult(
+        semantic_manifest=PydanticSemanticManifest(
             semantic_models=semantic_models,
             metrics=metrics,
         ),
         issues=SemanticManifestValidationResults.from_issues_sequence(issues),
     )
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/parsing/explicit_schema.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/parsing/explicit_schema.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/parsing/objects.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/parsing/objects.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/parsing/schema_validator.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/parsing/schema_validator.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/parsing/schemas.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/parsing/schemas.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/parsing/yaml_loader.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/parsing/yaml_loader.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/parsing/schemas/default_explicit_schema.json` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/parsing/schemas/default_explicit_schema.json`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/protocols/dimension.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/protocols/dimension.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/protocols/entity.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/protocols/entity.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/protocols/measure.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/protocols/measure.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/protocols/metadata.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/protocols/metadata.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/protocols/metric.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/protocols/metric.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/protocols/protocol_hint.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/protocols/protocol_hint.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/protocols/semantic_manifest.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/protocols/semantic_manifest.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/protocols/semantic_model.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/protocols/semantic_model.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/transformations/add_input_metric_measures.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/transformations/add_input_metric_measures.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/transformations/agg_time_dimension.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/transformations/agg_time_dimension.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/transformations/boolean_measure.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/transformations/boolean_measure.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/transformations/convert_count.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/transformations/convert_count.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/transformations/convert_median.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/transformations/convert_median.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/transformations/names.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/transformations/names.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/transformations/proxy_measure.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/transformations/proxy_measure.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/transformations/pydantic_rule_set.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/transformations/pydantic_rule_set.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/transformations/rule_set.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/transformations/rule_set.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/transformations/semantic_manifest_transformer.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/transformations/semantic_manifest_transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,17 @@
     @override
     def _implements_protocol(self) -> SemanticManifestTransformer[PydanticSemanticManifest]:  # noqa: D
         return self
 
     @staticmethod
     def transform(  # noqa: D
         model: PydanticSemanticManifest,
-        ordered_rule_sequences: Optional[Sequence[Sequence[SemanticManifestTransformRule]]] = None,
+        ordered_rule_sequences: Optional[
+            Sequence[Sequence[SemanticManifestTransformRule[PydanticSemanticManifest]]]
+        ] = None,
     ) -> PydanticSemanticManifest:
         if ordered_rule_sequences is None:
             ordered_rule_sequences = PydanticSemanticManifestTransformRuleSet().all_rules
 
         model_copy = copy.deepcopy(model)
 
         for rule_sequence in ordered_rule_sequences:
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/transformations/transform_rule.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/transformations/transform_rule.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/type_enums/time_granularity.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/type_enums/time_granularity.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/agg_time_dimension.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/agg_time_dimension.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/common_entities.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/common_entities.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/dimension_const.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/dimension_const.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/element_const.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/element_const.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/entities.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/entities.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/measures.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/measures.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/metrics.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/metrics.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/non_empty.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/non_empty.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/reserved_keywords.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/reserved_keywords.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/semantic_manifest_validator.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/semantic_manifest_validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,16 +94,16 @@
             raise ValueError(
                 "SemanticManifestValidator 'rules' must be a sequence with at least one SemanticManifestValidationRule."
             )
 
         self._rules = rules
         self._executor = ProcessPoolExecutor(max_workers=max_workers)
 
-    def validate_model(self, semantic_manifest: SemanticManifestT) -> SemanticManifestValidationResults:
-        """Validate a model according to configured rules."""
+    def validate_semantic_manifest(self, semantic_manifest: SemanticManifestT) -> SemanticManifestValidationResults:
+        """Validate a manifest according to configured rules."""
         results: List[SemanticManifestValidationResults] = []
 
         futures = [
             self._executor.submit(_validate_manifest_with_one_rule, validation_rule, semantic_manifest)
             for validation_rule in self._rules
         ]
         for future in as_completed(futures):
@@ -112,10 +112,10 @@
             results.append(result)
 
         return SemanticManifestValidationResults.merge(results)
 
     def checked_validations(self, semantic_manifest: SemanticManifestT) -> None:
         """Similar to validate(), but throws an exception if validation fails."""
         model_copy = copy.deepcopy(semantic_manifest)
-        model_issues = self.validate_model(model_copy)
+        model_issues = self.validate_semantic_manifest(model_copy)
         if model_issues.has_blocking_issues:
             raise SemanticManifestValidationException(issues=tuple(model_issues.all_issues))
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/semantic_models.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/semantic_models.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/unique_valid_name.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/unique_valid_name.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/validator_helpers.py` & `dbt_semantic_interfaces-0.1.0.dev4/dbt_semantic_interfaces/validations/validator_helpers.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/.gitignore` & `dbt_semantic_interfaces-0.1.0.dev4/.gitignore`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/LICENSE` & `dbt_semantic_interfaces-0.1.0.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/README.md` & `dbt_semantic_interfaces-0.1.0.dev4/README.md`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/pyproject.toml` & `dbt_semantic_interfaces-0.1.0.dev4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dbt-semantic-interfaces"
-version = "0.1.0.dev3"
+version = "0.1.0.dev4"
 description = 'The shared semantic layer definitions that dbt-core and MetricFlow use'
 readme = "README.md"
 requires-python = ">=3.8"
 license = "Apache-2.0"
 keywords = []
 authors = [
   { name = "dbt Labs", email = "info@dbtlabs.com" },
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev3/PKG-INFO` & `dbt_semantic_interfaces-0.1.0.dev4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-semantic-interfaces
-Version: 0.1.0.dev3
+Version: 0.1.0.dev4
 Summary: The shared semantic layer definitions that dbt-core and MetricFlow use
 Author-email: dbt Labs <info@dbtlabs.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-semantic-interfaces Version: 0.1.0.dev3
+Metadata-Version: 2.1 Name: dbt-semantic-interfaces Version: 0.1.0.dev4
 Summary: The shared semantic layer definitions that dbt-core and MetricFlow use
 Author-email: dbt Labs
 dbtlabs.com> License-Expression: Apache-2.0 License-File: LICENSE Classifier:
 Development Status :: 4 - Beta Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
```

