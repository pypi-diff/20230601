# Comparing `tmp/pydantic-2.0a4.tar.gz` & `tmp/pydantic-2.0b1.tar.gz`

## Comparing `pydantic-2.0a4.tar` & `pydantic-2.0b1.tar`

### file list

```diff
@@ -1,168 +1,202 @@
--rw-r--r--   0        0        0    79544 2020-02-02 00:00:00.000000 pydantic-2.0a4/HISTORY.md
--rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 pydantic-2.0a4/Makefile
--rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 pydantic-2.0a4/README.md
--rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/__init__.py
--rw-r--r--   0        0        0    10452 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/_migration.py
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/alias_generators.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/annotated.py
--rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/annotated_arguments.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/class_validators.py
--rw-r--r--   0        0        0    21440 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/color.py
--rw-r--r--   0        0        0     4799 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/config.py
--rw-r--r--   0        0        0     7592 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/dataclasses.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/datetime_parse.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/decorator.py
--rw-r--r--   0        0        0    21294 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/decorators.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/env_settings.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/error_wrappers.py
--rw-r--r--   0        0        0     4586 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/errors.py
--rw-r--r--   0        0        0    33208 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/fields.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/generics.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/json.py
--rw-r--r--   0        0        0    57653 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/json_schema.py
--rw-r--r--   0        0        0    51187 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/main.py
--rw-r--r--   0        0        0    38033 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/mypy.py
--rw-r--r--   0        0        0    10857 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/networks.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/parse.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/py.typed
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/schema.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/tools.py
--rw-r--r--   0        0        0    12736 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/type_adapter.py
--rw-r--r--   0        0        0    30542 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/types.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/typing.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/utils.py
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/validate_call.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/validators.py
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/_internal/__init__.py
--rw-r--r--   0        0        0     8549 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/_internal/_config.py
--rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/_internal/_core_metadata.py
--rw-r--r--   0        0        0    22912 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/_internal/_core_utils.py
--rw-r--r--   0        0        0     5642 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/_internal/_dataclasses.py
--rw-r--r--   0        0        0    19880 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/_internal/_decorators.py
--rw-r--r--   0        0        0     5223 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/_internal/_decorators_v1.py
--rw-r--r--   0        0        0    22018 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/_internal/_discriminated_union.py
--rw-r--r--   0        0        0     7967 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/_internal/_fields.py
--rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/_internal/_forward_ref.py
--rw-r--r--   0        0        0    65036 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/_internal/_generate_schema.py
--rw-r--r--   0        0        0    20565 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/_internal/_generics.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/_internal/_internal_dataclass.py
--rw-r--r--   0        0        0     3576 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/_internal/_known_annotated_metadata.py
--rw-r--r--   0        0        0    13403 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/_internal/_model_construction.py
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/_internal/_repr.py
--rw-r--r--   0        0        0     6609 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/_internal/_schema_generation_shared.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/_internal/_serializers.py
--rw-r--r--   0        0        0    24466 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/_internal/_std_types_schema.py
--rw-r--r--   0        0        0    17278 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/_internal/_typing_extra.py
--rw-r--r--   0        0        0    12401 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/_internal/_utils.py
--rw-r--r--   0        0        0     3162 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/_internal/_validate_call.py
--rw-r--r--   0        0        0     9486 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/_internal/_validators.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/deprecated/__init__.py
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/deprecated/config.py
--rw-r--r--   0        0        0     7751 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/deprecated/copy_internals.py
--rw-r--r--   0        0        0    10584 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/deprecated/decorator.py
--rw-r--r--   0        0        0     4100 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/deprecated/json.py
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/deprecated/parse.py
--rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 pydantic-2.0a4/pydantic/deprecated/tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/__init__.py
--rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/conftest.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/test_abc.py
--rw-r--r--   0        0        0    14285 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/test_aliases.py
--rw-r--r--   0        0        0     8683 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/test_annotated.py
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/test_assert_in_validators.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/test_callable.py
--rw-r--r--   0        0        0     7605 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/test_color.py
--rw-r--r--   0        0        0    13551 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/test_computed_fields.py
--rw-r--r--   0        0        0    18017 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/test_config.py
--rw-r--r--   0        0        0    12932 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/test_construction.py
--rw-r--r--   0        0        0     9488 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/test_create_model.py
--rw-r--r--   0        0        0    50553 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/test_dataclasses.py
--rw-r--r--   0        0        0    18712 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/test_datetime.py
--rw-r--r--   0        0        0    21331 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/test_deprecated.py
--rw-r--r--   0        0        0    12182 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/test_deprecated_validate_arguments.py
--rw-r--r--   0        0        0    40790 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/test_discriminated_union.py
--rw-r--r--   0        0        0     6405 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/test_docs.py
--rw-r--r--   0        0        0    77818 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/test_edge_cases.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/test_errors.py
--rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/test_fastapi.sh
--rw-r--r--   0        0        0     4980 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/test_fastapi_json_schema.py
--rw-r--r--   0        0        0    27927 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/test_forward_ref.py
--rw-r--r--   0        0        0    68261 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/test_generics.py
--rw-r--r--   0        0        0     5101 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/test_internal.py
--rw-r--r--   0        0        0    11139 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/test_json.py
--rw-r--r--   0        0        0   116306 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/test_json_schema.py
--rw-r--r--   0        0        0    63352 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/test_main.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/test_migration.py
--rw-r--r--   0        0        0     5631 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/test_model_signature.py
--rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/test_model_validator.py
--rw-r--r--   0        0        0    29249 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/test_networks.py
--rw-r--r--   0        0        0    15801 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/test_networks_ipaddress.py
--rw-r--r--   0        0        0     7069 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/test_parse.py
--rw-r--r--   0        0        0     5963 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/test_prepare_annotations.py
--rw-r--r--   0        0        0     9086 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/test_private_attributes.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/test_rich_repr.py
--rw-r--r--   0        0        0    24419 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/test_serialize.py
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/test_strict.py
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/test_structural_pattern_matching.py
--rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/test_tools.py
--rw-r--r--   0        0        0   143004 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/test_types.py
--rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/test_types_namedtuple.py
--rw-r--r--   0        0        0     4994 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/test_types_payment_card_number.py
--rw-r--r--   0        0        0    20446 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/test_types_typeddict.py
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/test_typing.py
--rw-r--r--   0        0        0    16517 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/test_utils.py
--rw-r--r--   0        0        0    18202 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/test_validate_call.py
--rw-r--r--   0        0        0     7272 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/test_validator.py
--rw-r--r--   0        0        0    69050 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/test_validators.py
--rwxr-xr-x   0        0        0     4656 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/test_validators_dataclass.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/test_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/mypy/__init__.py
--rw-r--r--   0        0        0    10802 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/mypy/test_mypy.py
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/mypy/configs/mypy-default.ini
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/mypy/configs/mypy-plugin-strict-no-any.ini
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/mypy/configs/mypy-plugin-strict.ini
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/mypy/configs/mypy-plugin.ini
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/mypy/configs/pyproject-default.toml
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/mypy/configs/pyproject-plugin-bad-param.toml
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/mypy/configs/pyproject-plugin-strict.toml
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/mypy/configs/pyproject-plugin.toml
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/mypy/modules/computed_fields.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/mypy/modules/custom_constructor.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/mypy/modules/dataclass_no_any.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/mypy/modules/fail1.py
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/mypy/modules/fail2.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/mypy/modules/fail3.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/mypy/modules/fail4.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/mypy/modules/fail_defaults.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/mypy/modules/plugin_default_factory.py
--rw-r--r--   0        0        0     5822 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/mypy/modules/plugin_fail.py
--rw-r--r--   0        0        0     5840 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/mypy/modules/plugin_fail_baseConfig.py
--rw-r--r--   0        0        0     5611 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/mypy/modules/plugin_success.py
--rw-r--r--   0        0        0     4533 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/mypy/modules/plugin_success_baseConfig.py
--rw-r--r--   0        0        0     7553 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/mypy/modules/success.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/mypy/outputs/latest/computed_fields.txt
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/mypy/outputs/latest/custom_constructor.txt
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/mypy/outputs/latest/fail1.txt
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/mypy/outputs/latest/fail2.txt
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/mypy/outputs/latest/fail3.txt
--rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/mypy/outputs/latest/fail4.txt
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/mypy/outputs/latest/fail_defaults.txt
--rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/mypy/outputs/latest/plugin-fail-baseConfig.txt
--rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/mypy/outputs/latest/plugin-fail-strict-baseConfig.txt
--rw-r--r--   0        0        0     4874 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/mypy/outputs/latest/plugin-fail-strict.txt
--rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/mypy/outputs/latest/plugin-fail.txt
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/mypy/outputs/latest/plugin-success-strict-baseConfig.txt
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/mypy/outputs/latest/plugin-success-strict.txt
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/mypy/outputs/latest/plugin_default_factory.txt
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/mypy/outputs/latest/plugin_success.txt
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/mypy/outputs/latest/plugin_success_baseConfig.txt
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/mypy/outputs/v1.0.1/fail1.txt
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/mypy/outputs/v1.0.1/fail2.txt
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/mypy/outputs/v1.0.1/plugin_success.txt
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/mypy/outputs/v1.0.1/plugin_success_baseConfig.txt
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/pyright/pyproject.toml
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 pydantic-2.0a4/tests/pyright/pyright_example.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 pydantic-2.0a4/.gitignore
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 pydantic-2.0a4/LICENSE
--rw-r--r--   0        0        0     5706 2020-02-02 00:00:00.000000 pydantic-2.0a4/pyproject.toml
--rw-r--r--   0        0        0   114845 2020-02-02 00:00:00.000000 pydantic-2.0a4/PKG-INFO
+-rw-r--r--   0        0        0    79696 2020-02-02 00:00:00.000000 pydantic-2.0b1/HISTORY.md
+-rw-r--r--   0        0        0     3577 2020-02-02 00:00:00.000000 pydantic-2.0b1/Makefile
+-rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 pydantic-2.0b1/README.md
+-rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/__init__.py
+-rw-r--r--   0        0        0    10818 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/_migration.py
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/alias_generators.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/class_validators.py
+-rw-r--r--   0        0        0    21146 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/color.py
+-rw-r--r--   0        0        0     4588 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/config.py
+-rw-r--r--   0        0        0    11650 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/dataclasses.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/datetime_parse.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/decorator.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/env_settings.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/error_wrappers.py
+-rw-r--r--   0        0        0     4561 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/errors.py
+-rw-r--r--   0        0        0    37298 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/fields.py
+-rw-r--r--   0        0        0     8882 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/functional_serializers.py
+-rw-r--r--   0        0        0    10935 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/functional_validators.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/generics.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/json.py
+-rw-r--r--   0        0        0    70647 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/json_schema.py
+-rw-r--r--   0        0        0    54953 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/main.py
+-rw-r--r--   0        0        0    38603 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/mypy.py
+-rw-r--r--   0        0        0    10944 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/networks.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/parse.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/py.typed
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/schema.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/tools.py
+-rw-r--r--   0        0        0    15373 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/type_adapter.py
+-rw-r--r--   0        0        0    37702 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/types.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/typing.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/utils.py
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/validate_call.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/validators.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/_internal/__init__.py
+-rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/_internal/_annotated_handlers.py
+-rw-r--r--   0        0        0     8755 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/_internal/_config.py
+-rw-r--r--   0        0        0     3486 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/_internal/_core_metadata.py
+-rw-r--r--   0        0        0    23517 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/_internal/_core_utils.py
+-rw-r--r--   0        0        0     7205 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/_internal/_dataclasses.py
+-rw-r--r--   0        0        0    24182 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/_internal/_decorators.py
+-rw-r--r--   0        0        0     5223 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/_internal/_decorators_v1.py
+-rw-r--r--   0        0        0    22184 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/_internal/_discriminated_union.py
+-rw-r--r--   0        0        0     8649 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/_internal/_fields.py
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/_internal/_forward_ref.py
+-rw-r--r--   0        0        0    66087 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/_internal/_generate_schema.py
+-rw-r--r--   0        0        0    20566 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/_internal/_generics.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/_internal/_internal_dataclass.py
+-rw-r--r--   0        0        0     8225 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/_internal/_known_annotated_metadata.py
+-rw-r--r--   0        0        0    23972 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/_internal/_model_construction.py
+-rw-r--r--   0        0        0     4285 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/_internal/_repr.py
+-rw-r--r--   0        0        0     4947 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/_internal/_schema_generation_shared.py
+-rw-r--r--   0        0        0    37641 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/_internal/_std_types_schema.py
+-rw-r--r--   0        0        0    16535 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/_internal/_typing_extra.py
+-rw-r--r--   0        0        0    12277 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/_internal/_utils.py
+-rw-r--r--   0        0        0     3162 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/_internal/_validate_call.py
+-rw-r--r--   0        0        0     9965 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/_internal/_validators.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/deprecated/__init__.py
+-rw-r--r--   0        0        0     9379 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/deprecated/class_validators.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/deprecated/config.py
+-rw-r--r--   0        0        0     7644 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/deprecated/copy_internals.py
+-rw-r--r--   0        0        0    10595 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/deprecated/decorator.py
+-rw-r--r--   0        0        0     4100 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/deprecated/json.py
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/deprecated/parse.py
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/deprecated/tools.py
+-rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/__init__.py
+-rw-r--r--   0        0        0    14586 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/_hypothesis_plugin.py
+-rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/annotated_types.py
+-rw-r--r--   0        0        0    14595 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/class_validators.py
+-rw-r--r--   0        0        0    16811 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/color.py
+-rw-r--r--   0        0        0     6429 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/config.py
+-rw-r--r--   0        0        0    17515 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/dataclasses.py
+-rw-r--r--   0        0        0     7714 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/datetime_parse.py
+-rw-r--r--   0        0        0    10263 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/decorator.py
+-rw-r--r--   0        0        0    13893 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/env_settings.py
+-rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/error_wrappers.py
+-rw-r--r--   0        0        0    17693 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/errors.py
+-rw-r--r--   0        0        0    50418 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/fields.py
+-rw-r--r--   0        0        0    17424 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/generics.py
+-rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/json.py
+-rw-r--r--   0        0        0    44378 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/main.py
+-rw-r--r--   0        0        0    38097 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/mypy.py
+-rw-r--r--   0        0        0    21826 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/networks.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/parse.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/py.typed
+-rw-r--r--   0        0        0    47615 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/schema.py
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/tools.py
+-rw-r--r--   0        0        0    35219 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/types.py
+-rw-r--r--   0        0        0    19358 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/typing.py
+-rw-r--r--   0        0        0    25809 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/utils.py
+-rw-r--r--   0        0        0    21874 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/validators.py
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 pydantic-2.0b1/pydantic/v1/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/__init__.py
+-rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/conftest.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_abc.py
+-rw-r--r--   0        0        0    14786 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_aliases.py
+-rw-r--r--   0        0        0     8718 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_annotated.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_assert_in_validators.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_callable.py
+-rw-r--r--   0        0        0     7605 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_color.py
+-rw-r--r--   0        0        0    16774 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_computed_fields.py
+-rw-r--r--   0        0        0    21049 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_config.py
+-rw-r--r--   0        0        0    13497 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_construction.py
+-rw-r--r--   0        0        0    15572 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_create_model.py
+-rw-r--r--   0        0        0    63335 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_dataclasses.py
+-rw-r--r--   0        0        0    21265 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_datetime.py
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_decorators.py
+-rw-r--r--   0        0        0    20440 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_deprecated.py
+-rw-r--r--   0        0        0    12182 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_deprecated_validate_arguments.py
+-rw-r--r--   0        0        0    40531 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_discriminated_union.py
+-rw-r--r--   0        0        0     6506 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_docs.py
+-rw-r--r--   0        0        0    76384 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_edge_cases.py
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_errors.py
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_exports.py
+-rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_fastapi.sh
+-rw-r--r--   0        0        0     4980 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_fastapi_json_schema.py
+-rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_fields.py
+-rw-r--r--   0        0        0    26896 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_forward_ref.py
+-rw-r--r--   0        0        0    71065 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_generics.py
+-rw-r--r--   0        0        0     8338 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_internal.py
+-rw-r--r--   0        0        0    13165 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_json.py
+-rw-r--r--   0        0        0   140193 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_json_schema.py
+-rw-r--r--   0        0        0    65906 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_main.py
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_migration.py
+-rw-r--r--   0        0        0     5953 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_model_signature.py
+-rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_model_validator.py
+-rw-r--r--   0        0        0    29249 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_networks.py
+-rw-r--r--   0        0        0    15801 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_networks_ipaddress.py
+-rw-r--r--   0        0        0     6977 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_parse.py
+-rw-r--r--   0        0        0     8039 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_prepare_annotations.py
+-rw-r--r--   0        0        0     8610 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_private_attributes.py
+-rwxr-xr-x   0        0        0      131 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_pydantic_settings.sh
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_rich_repr.py
+-rw-r--r--   0        0        0    10304 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_root_model.py
+-rw-r--r--   0        0        0    29452 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_serialize.py
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_strict.py
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_structural_pattern_matching.py
+-rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_tools.py
+-rw-r--r--   0        0        0     6548 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_type_adapter.py
+-rw-r--r--   0        0        0    10667 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_type_alias_type.py
+-rw-r--r--   0        0        0   177998 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_types.py
+-rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_types_namedtuple.py
+-rw-r--r--   0        0        0     4994 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_types_payment_card_number.py
+-rw-r--r--   0        0        0    25240 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_types_typeddict.py
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_typing.py
+-rw-r--r--   0        0        0    21503 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_utils.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_v1.py
+-rw-r--r--   0        0        0    19485 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_validate_call.py
+-rw-r--r--   0        0        0    72494 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_validators.py
+-rwxr-xr-x   0        0        0     4606 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_validators_dataclass.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/test_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/__init__.py
+-rw-r--r--   0        0        0    10878 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/test_mypy.py
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/configs/mypy-default.ini
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/configs/mypy-plugin-strict-no-any.ini
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/configs/mypy-plugin-strict.ini
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/configs/mypy-plugin.ini
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/configs/pyproject-default.toml
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/configs/pyproject-plugin-bad-param.toml
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/configs/pyproject-plugin-strict.toml
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/configs/pyproject-plugin.toml
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/modules/computed_fields.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/modules/custom_constructor.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/modules/dataclass_no_any.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/modules/fail1.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/modules/fail2.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/modules/fail3.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/modules/fail4.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/modules/fail_defaults.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/modules/plugin_default_factory.py
+-rw-r--r--   0        0        0     5822 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/modules/plugin_fail.py
+-rw-r--r--   0        0        0     5840 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/modules/plugin_fail_baseConfig.py
+-rw-r--r--   0        0        0     5644 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/modules/plugin_success.py
+-rw-r--r--   0        0        0     4412 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/modules/plugin_success_baseConfig.py
+-rw-r--r--   0        0        0     7416 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/modules/success.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/outputs/latest/computed_fields.txt
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/outputs/latest/custom_constructor.txt
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/outputs/latest/fail1.txt
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/outputs/latest/fail2.txt
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/outputs/latest/fail3.txt
+-rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/outputs/latest/fail4.txt
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/outputs/latest/fail_defaults.txt
+-rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/outputs/latest/plugin-fail-baseConfig.txt
+-rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/outputs/latest/plugin-fail-strict-baseConfig.txt
+-rw-r--r--   0        0        0     4874 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/outputs/latest/plugin-fail-strict.txt
+-rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/outputs/latest/plugin-fail.txt
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/outputs/latest/plugin-success-strict-baseConfig.txt
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/outputs/latest/plugin-success-strict.txt
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/outputs/latest/plugin_default_factory.txt
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/outputs/latest/plugin_success.txt
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/outputs/latest/plugin_success_baseConfig.txt
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/outputs/v1.0.1/fail1.txt
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/outputs/v1.0.1/fail2.txt
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/outputs/v1.0.1/plugin_success.txt
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/mypy/outputs/v1.0.1/plugin_success_baseConfig.txt
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/pyright/pyproject.toml
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 pydantic-2.0b1/tests/pyright/pyright_example.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 pydantic-2.0b1/.gitignore
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 pydantic-2.0b1/LICENSE
+-rw-r--r--   0        0        0     6035 2020-02-02 00:00:00.000000 pydantic-2.0b1/pyproject.toml
+-rw-r--r--   0        0        0   114997 2020-02-02 00:00:00.000000 pydantic-2.0b1/PKG-INFO
```

### Comparing `pydantic-2.0a4/HISTORY.md` & `pydantic-2.0b1/HISTORY.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## v2.0b1 (2023-06-01)
+
+First beta pre-release of Pydantic V2
+
+See the full changelog [here](https://github.com/pydantic/pydantic/releases/tag/v2.0b1)
+
 ## v2.0a4 (2023-05-05)
 
 Fourth pre-release of Pydantic V2
 
 See the full changelog [here](https://github.com/pydantic/pydantic/releases/tag/v2.0a4)
 
 ## v2.0a3 (2023-04-20)
```

### Comparing `pydantic-2.0a4/Makefile` & `pydantic-2.0b1/Makefile`

 * *Files 10% similar despite different names*

```diff
@@ -20,21 +20,21 @@
 
 .PHONY: rebuild-lockfiles  ## Rebuild lockfiles from scratch, updating all dependencies
 rebuild-lockfiles: .pdm
 	pdm lock --dev --group :all
 
 .PHONY: format  ## Auto-format python source files
 format: .pdm
-	pdm run black $(sources)
+	pdm run black --exclude 'pydantic/v1' $(sources)
 	pdm run ruff --fix $(sources)
 
 .PHONY: lint  ## Lint python source files
 lint: .pdm
 	pdm run ruff $(sources)
-	pdm run black $(sources) --check --diff
+	pdm run black --exclude 'pydantic/v1' $(sources) --check --diff
 
 .PHONY: codespell  ## Use Codespell to do spellchecking
 codespell: .pre-commit
 	pre-commit run codespell --all-files
 
 .PHONY: typecheck  ## Perform type-checking
 typecheck: .pre-commit .pdm
@@ -52,25 +52,32 @@
 test: .pdm
 	pdm run coverage run -m pytest --durations=10
 
 .PHONY: testcov  ## Run tests and generate a coverage report, skipping the type-checker integration tests
 testcov: test
 	@echo "building coverage html"
 	@pdm run coverage html
+	@echo "building coverage lcov"
+	@pdm run coverage lcov
 
 .PHONY: test-examples  ## Run only the tests from the documentation
 test-examples: .pdm
 	@echo "running examples"
 	@find docs/examples -type f -name '*.py' | xargs -I'{}' sh -c 'pdm run python {} >/dev/null 2>&1 || (echo "{} failed")'
 
 .PHONY: test-fastapi  ## Run the FastAPI tests with this version of pydantic
 test-fastapi: .pdm
 	git clone https://github.com/tiangolo/fastapi.git --single-branch
 	pdm run ./tests/test_fastapi.sh
 
+.PHONY: test-pydantic-settings  ## Run the pydantic-settings tests with this version of pydantic
+test-pydantic-settings: .pdm
+	git clone https://github.com/pydantic/pydantic-settings.git --single-branch
+	bash ./tests/test_pydantic_settings.sh
+
 .PHONY: all  ## Run the standard set of checks performed in CI
 all: lint typecheck codespell testcov
 
 .PHONY: clean  ## Clear local caches and build artifacts
 clean:
 	rm -rf `find . -name __pycache__`
 	rm -f `find . -type f -name '*.py[co]'`
@@ -97,7 +104,11 @@
 
 .PHONY: help  ## Display this message
 help:
 	@grep -E \
 		'^.PHONY: .*?## .*$$' $(MAKEFILE_LIST) | \
 		sort | \
 		awk 'BEGIN {FS = ".PHONY: |## "}; {printf "\033[36m%-19s\033[0m %s\n", $$2, $$3}'
+
+.PHONY: update-v1  ## Update V1 namespace
+update-v1:
+	pdm run ./update_v1.sh
```

### Comparing `pydantic-2.0a4/README.md` & `pydantic-2.0b1/README.md`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a4/pydantic/__init__.py` & `pydantic-2.0b1/pydantic/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,72 +1,90 @@
-from pydantic_core import ValidationError
+import pydantic_core
 from pydantic_core.core_schema import (
     FieldSerializationInfo,
     FieldValidationInfo,
     SerializationInfo,
     SerializerFunctionWrapHandler,
     ValidationInfo,
     ValidatorFunctionWrapHandler,
 )
 
 from . import dataclasses
+from ._internal._annotated_handlers import (
+    GetCoreSchemaHandler as GetCoreSchemaHandler,
+)
+from ._internal._annotated_handlers import (
+    GetJsonSchemaHandler as GetJsonSchemaHandler,
+)
 from ._migration import getattr_migration
 from .config import ConfigDict, Extra
-from .decorators import field_serializer, field_validator, model_serializer, model_validator, root_validator, validator
-from .deprecated.config import BaseConfig
+from .deprecated.class_validators import root_validator, validator
+from .deprecated.config import BaseConfig  # type: ignore
 from .deprecated.tools import *
 from .errors import *
 from .fields import AliasChoices, AliasPath, Field, PrivateAttr, computed_field
+from .functional_serializers import PlainSerializer, WrapSerializer, field_serializer, model_serializer
+from .functional_validators import field_validator, model_validator
 from .main import *
 from .networks import *
 from .type_adapter import TypeAdapter
 from .types import *
 from .validate_call import validate_call
 from .version import VERSION
 
 __version__ = VERSION
 
+# this encourages pycharm to import `ValidationError` from here, not pydantic_core
+ValidationError = pydantic_core.ValidationError
+
 # WARNING __all__ from .errors is not included here, it will be removed as an export here in v2
 # please use "from pydantic.errors import ..." instead
 __all__ = [
     # dataclasses
     'dataclasses',
-    # decorators
+    # functional validators
+    'ValidationInfo',
+    'FieldValidationInfo',
+    'ValidatorFunctionWrapHandler',
     'field_validator',
     'model_validator',
+    # deprecated V1 functional validators
     'root_validator',
     'validator',
+    # functional serializers
     'field_serializer',
     'model_serializer',
-    'ValidationInfo',
-    'FieldValidationInfo',
-    'SerializationInfo',
+    'PlainSerializer',
+    'WrapSerializer',
     'FieldSerializationInfo',
-    'ValidatorFunctionWrapHandler',
+    'SerializationInfo',
     'SerializerFunctionWrapHandler',
     # config
     'BaseConfig',
     'ConfigDict',
     'Extra',
     # validate_call
     'validate_call',
-    # error_wrappers
+    # pydantic_core errors
     'ValidationError',
+    # errors
     'PydanticUserError',
     'PydanticSchemaGenerationError',
     'PydanticImportError',
     'PydanticUndefinedAnnotation',
+    'PydanticInvalidForJsonSchema',
     # fields
     'AliasPath',
     'AliasChoices',
     'Field',
     'computed_field',
     # main
     'BaseModel',
     'create_model',
+    'RootModel',
     # network
     'AnyUrl',
     'AnyHttpUrl',
     'FileUrl',
     'HttpUrl',
     'UrlConstraints',
     'EmailStr',
@@ -125,24 +143,32 @@
     'StrictInt',
     'StrictFloat',
     'PaymentCardNumber',
     'PrivateAttr',
     'ByteSize',
     'PastDate',
     'FutureDate',
+    'PastDatetime',
+    'FutureDatetime',
     'AwareDatetime',
     'NaiveDatetime',
     'AllowInfNan',
     'EncoderProtocol',
     'EncodedBytes',
     'EncodedStr',
     'Base64Encoder',
     'Base64Bytes',
     'Base64Str',
+    'SkipValidation',
+    'InstanceOf',
+    'WithJsonSchema',
     # type_adapter
     'TypeAdapter',
     # version
     'VERSION',
+    # annotated handlers
+    'GetCoreSchemaHandler',
+    'GetJsonSchemaHandler',
 ]
 
 
 __getattr__ = getattr_migration(__name__)
```

### Comparing `pydantic-2.0a4/pydantic/_migration.py` & `pydantic-2.0b1/pydantic/_migration.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,241 +1,249 @@
+import sys
 import warnings
-from typing import Any, Callable
+from typing import Any, Callable, Dict
 
 from ._internal._validators import import_string
 
 MOVED_IN_V2 = {
-    'pydantic.utils.version_info': 'pydantic.version.version_info',
-    'pydantic.error_wrappers.ValidationError': 'pydantic.ValidationError',
-    'pydantic.utils.to_camel': 'pydantic.alias_generators.to_pascal',
-    'pydantic.utils.to_lower_camel': 'pydantic.alias_generators.to_camel',
+    'pydantic.utils:version_info': 'pydantic.version:version_info',
+    'pydantic.error_wrappers:ValidationError': 'pydantic:ValidationError',
+    'pydantic.utils:to_camel': 'pydantic.alias_generators:to_pascal',
+    'pydantic.utils:to_lower_camel': 'pydantic.alias_generators:to_camel',
 }
 
 DEPRECATED_MOVED_IN_V2 = {
-    'pydantic.tools.schema_of': 'pydantic.deprecated.tools.schema_of',
-    'pydantic.tools.parse_obj_as': 'pydantic.deprecated.tools.parse_obj_as',
-    'pydantic.tools.schema_json_of': 'pydantic.deprecated.tools.schema_json_of',
-    'pydantic.json.pydantic_encoder': 'pydantic.deprecated.json.pydantic_encoder',
-    'pydantic.validate_arguments': 'pydantic.deprecated.decorator.validate_arguments',
-    'pydantic.json.custom_pydantic_encoder': 'pydantic.deprecated.json.custom_pydantic_encoder',
-    'pydantic.json.timedelta_isoformat': 'pydantic.deprecated.json.timedelta_isoformat',
-    'pydantic.decorator.validate_arguments': 'pydantic.deprecated.decorator.validate_arguments',
+    'pydantic.tools:schema_of': 'pydantic.deprecated.tools:schema_of',
+    'pydantic.tools:parse_obj_as': 'pydantic.deprecated.tools:parse_obj_as',
+    'pydantic.tools:schema_json_of': 'pydantic.deprecated.tools:schema_json_of',
+    'pydantic.json:pydantic_encoder': 'pydantic.deprecated.json:pydantic_encoder',
+    'pydantic:validate_arguments': 'pydantic.deprecated.decorator:validate_arguments',
+    'pydantic.json:custom_pydantic_encoder': 'pydantic.deprecated.json:custom_pydantic_encoder',
+    'pydantic.json:timedelta_isoformat': 'pydantic.deprecated.json:timedelta_isoformat',
+    'pydantic.decorator:validate_arguments': 'pydantic.deprecated.decorator:validate_arguments',
+    'pydantic.class_validators:validator': 'pydantic.deprecated.class_validators:validator',
+    'pydantic.class_validators:root_validator': 'pydantic.deprecated.class_validators:root_validator',
+    **{
+        f'pydantic.utils:{obj}': f'pydantic.v1.utils:{obj}'
+        for obj in (
+            'deep_update',
+            'GetterDict',
+            'lenient_issubclass',
+            'lenient_isinstance',
+            'is_valid_field',
+            'update_not_none',
+            'import_string',
+            'Representation',
+            'ROOT_KEY',
+            'smart_deepcopy',
+            'sequence_like',
+        )
+    },
 }
 
 REMOVED_IN_V2 = {
-    'pydantic.BaseSettings',
-    'pydantic.ConstrainedBytes',
-    'pydantic.ConstrainedDate',
-    'pydantic.ConstrainedDecimal',
-    'pydantic.ConstrainedFloat',
-    'pydantic.ConstrainedFrozenSet',
-    'pydantic.ConstrainedInt',
-    'pydantic.ConstrainedList',
-    'pydantic.ConstrainedSet',
-    'pydantic.ConstrainedStr',
-    'pydantic.JsonWrapper',
-    'pydantic.NoneBytes',
-    'pydantic.NoneStr',
-    'pydantic.NoneStrBytes',
-    'pydantic.Protocol',
-    'pydantic.PyObject',
-    'pydantic.Required',
-    'pydantic.StrBytes',
-    'pydantic.compiled',
-    'pydantic.config.get_config',
-    'pydantic.config.inherit_config',
-    'pydantic.config.prepare_config',
-    'pydantic.create_model_from_namedtuple',
-    'pydantic.create_model_from_typeddict',
-    'pydantic.dataclasses.create_pydantic_model_from_dataclass',
-    'pydantic.dataclasses.make_dataclass_validator',
-    'pydantic.dataclasses.set_validation',
-    'pydantic.datetime_parse.parse_date',
-    'pydantic.datetime_parse.parse_time',
-    'pydantic.datetime_parse.parse_datetime',
-    'pydantic.datetime_parse.parse_duration',
-    'pydantic.error_wrappers.ErrorWrapper',
-    'pydantic.errors.AnyStrMaxLengthError',
-    'pydantic.errors.AnyStrMinLengthError',
-    'pydantic.errors.ArbitraryTypeError',
-    'pydantic.errors.BoolError',
-    'pydantic.errors.BytesError',
-    'pydantic.errors.CallableError',
-    'pydantic.errors.ClassError',
-    'pydantic.errors.ColorError',
-    'pydantic.errors.ConfigError',
-    'pydantic.errors.DataclassTypeError',
-    'pydantic.errors.DateError',
-    'pydantic.errors.DateNotInTheFutureError',
-    'pydantic.errors.DateNotInThePastError',
-    'pydantic.errors.DateTimeError',
-    'pydantic.errors.DecimalError',
-    'pydantic.errors.DecimalIsNotFiniteError',
-    'pydantic.errors.DecimalMaxDigitsError',
-    'pydantic.errors.DecimalMaxPlacesError',
-    'pydantic.errors.DecimalWholeDigitsError',
-    'pydantic.errors.DictError',
-    'pydantic.errors.DurationError',
-    'pydantic.errors.EmailError',
-    'pydantic.errors.EnumError',
-    'pydantic.errors.EnumMemberError',
-    'pydantic.errors.ExtraError',
-    'pydantic.errors.FloatError',
-    'pydantic.errors.FrozenSetError',
-    'pydantic.errors.FrozenSetMaxLengthError',
-    'pydantic.errors.FrozenSetMinLengthError',
-    'pydantic.errors.HashableError',
-    'pydantic.errors.IPv4AddressError',
-    'pydantic.errors.IPv4InterfaceError',
-    'pydantic.errors.IPv4NetworkError',
-    'pydantic.errors.IPv6AddressError',
-    'pydantic.errors.IPv6InterfaceError',
-    'pydantic.errors.IPv6NetworkError',
-    'pydantic.errors.IPvAnyAddressError',
-    'pydantic.errors.IPvAnyInterfaceError',
-    'pydantic.errors.IPvAnyNetworkError',
-    'pydantic.errors.IntEnumError',
-    'pydantic.errors.IntegerError',
-    'pydantic.errors.InvalidByteSize',
-    'pydantic.errors.InvalidByteSizeUnit',
-    'pydantic.errors.InvalidDiscriminator',
-    'pydantic.errors.InvalidLengthForBrand',
-    'pydantic.errors.JsonError',
-    'pydantic.errors.JsonTypeError',
-    'pydantic.errors.ListError',
-    'pydantic.errors.ListMaxLengthError',
-    'pydantic.errors.ListMinLengthError',
-    'pydantic.errors.ListUniqueItemsError',
-    'pydantic.errors.LuhnValidationError',
-    'pydantic.errors.MissingDiscriminator',
-    'pydantic.errors.MissingError',
-    'pydantic.errors.NoneIsAllowedError',
-    'pydantic.errors.NoneIsNotAllowedError',
-    'pydantic.errors.NotDigitError',
-    'pydantic.errors.NotNoneError',
-    'pydantic.errors.NumberNotGeError',
-    'pydantic.errors.NumberNotGtError',
-    'pydantic.errors.NumberNotLeError',
-    'pydantic.errors.NumberNotLtError',
-    'pydantic.errors.NumberNotMultipleError',
-    'pydantic.errors.PathError',
-    'pydantic.errors.PathNotADirectoryError',
-    'pydantic.errors.PathNotAFileError',
-    'pydantic.errors.PathNotExistsError',
-    'pydantic.errors.PatternError',
-    'pydantic.errors.PyObjectError',
-    'pydantic.errors.PydanticTypeError',
-    'pydantic.errors.PydanticValueError',
-    'pydantic.errors.SequenceError',
-    'pydantic.errors.SetError',
-    'pydantic.errors.SetMaxLengthError',
-    'pydantic.errors.SetMinLengthError',
-    'pydantic.errors.StrError',
-    'pydantic.errors.StrRegexError',
-    'pydantic.errors.StrictBoolError',
-    'pydantic.errors.SubclassError',
-    'pydantic.errors.TimeError',
-    'pydantic.errors.TupleError',
-    'pydantic.errors.TupleLengthError',
-    'pydantic.errors.UUIDError',
-    'pydantic.errors.UUIDVersionError',
-    'pydantic.errors.UrlError',
-    'pydantic.errors.UrlExtraError',
-    'pydantic.errors.UrlHostError',
-    'pydantic.errors.UrlHostTldError',
-    'pydantic.errors.UrlPortError',
-    'pydantic.errors.UrlSchemeError',
-    'pydantic.errors.UrlSchemePermittedError',
-    'pydantic.errors.UrlUserInfoError',
-    'pydantic.errors.WrongConstantError',
-    'pydantic.main.validate_model',
-    'pydantic.networks.stricturl',
-    'pydantic.parse_file_as',
-    'pydantic.parse_raw_as',
-    'pydantic.stricturl',
-    'pydantic.tools.parse_file_as',
-    'pydantic.tools.parse_raw_as',
-    'pydantic.types.ConstrainedBytes',
-    'pydantic.types.ConstrainedDate',
-    'pydantic.types.ConstrainedDecimal',
-    'pydantic.types.ConstrainedFloat',
-    'pydantic.types.ConstrainedFrozenSet',
-    'pydantic.types.ConstrainedInt',
-    'pydantic.types.ConstrainedList',
-    'pydantic.types.ConstrainedSet',
-    'pydantic.types.ConstrainedStr',
-    'pydantic.types.JsonWrapper',
-    'pydantic.types.NoneBytes',
-    'pydantic.types.NoneStr',
-    'pydantic.types.NoneStrBytes',
-    'pydantic.types.PyObject',
-    'pydantic.types.StrBytes',
-    'pydantic.typing.evaluate_forwardref',
-    'pydantic.typing.AbstractSetIntStr',
-    'pydantic.typing.AnyCallable',
-    'pydantic.typing.AnyClassMethod',
-    'pydantic.typing.CallableGenerator',
-    'pydantic.typing.DictAny',
-    'pydantic.typing.DictIntStrAny',
-    'pydantic.typing.DictStrAny',
-    'pydantic.typing.IntStr',
-    'pydantic.typing.ListStr',
-    'pydantic.typing.MappingIntStrAny',
-    'pydantic.typing.NoArgAnyCallable',
-    'pydantic.typing.NoneType',
-    'pydantic.typing.ReprArgs',
-    'pydantic.typing.SetStr',
-    'pydantic.typing.StrPath',
-    'pydantic.typing.TupleGenerator',
-    'pydantic.typing.WithArgsTypes',
-    'pydantic.typing.all_literal_values',
-    'pydantic.typing.display_as_type',
-    'pydantic.typing.get_all_type_hints',
-    'pydantic.typing.get_args',
-    'pydantic.typing.get_origin',
-    'pydantic.typing.get_sub_types',
-    'pydantic.typing.is_callable_type',
-    'pydantic.typing.is_classvar',
-    'pydantic.typing.is_finalvar',
-    'pydantic.typing.is_literal_type',
-    'pydantic.typing.is_namedtuple',
-    'pydantic.typing.is_new_type',
-    'pydantic.typing.is_none_type',
-    'pydantic.typing.is_typeddict',
-    'pydantic.typing.is_typeddict_special',
-    'pydantic.typing.is_union',
-    'pydantic.typing.new_type_supertype',
-    'pydantic.typing.resolve_annotations',
-    'pydantic.typing.typing_base',
-    'pydantic.typing.update_field_forward_refs',
-    'pydantic.typing.update_model_forward_refs',
-    'pydantic.utils.ClassAttribute',
-    'pydantic.utils.DUNDER_ATTRIBUTES',
-    'pydantic.utils.GetterDict',
-    'pydantic.utils.PyObjectStr',
-    'pydantic.utils.ROOT_KEY',
-    'pydantic.utils.Representation',
-    'pydantic.utils.ValueItems',
-    'pydantic.utils.almost_equal_floats',
-    'pydantic.utils.deep_update',
-    'pydantic.utils.get_discriminator_alias_and_values',
-    'pydantic.utils.get_model',
-    'pydantic.utils.get_unique_discriminator_alias',
-    'pydantic.utils.import_string',
-    'pydantic.utils.in_ipython',
-    'pydantic.utils.is_valid_field',
-    'pydantic.utils.is_valid_identifier',
-    'pydantic.utils.lenient_isinstance',
-    'pydantic.utils.lenient_issubclass',
-    'pydantic.utils.path_type',
-    'pydantic.utils.sequence_like',
-    'pydantic.utils.smart_deepcopy',
-    'pydantic.utils.update_not_none',
-    'pydantic.utils.validate_field_name',
-    'pydantic.validate_model',
+    'pydantic:BaseSettings',
+    'pydantic:ConstrainedBytes',
+    'pydantic:ConstrainedDate',
+    'pydantic:ConstrainedDecimal',
+    'pydantic:ConstrainedFloat',
+    'pydantic:ConstrainedFrozenSet',
+    'pydantic:ConstrainedInt',
+    'pydantic:ConstrainedList',
+    'pydantic:ConstrainedSet',
+    'pydantic:ConstrainedStr',
+    'pydantic:JsonWrapper',
+    'pydantic:NoneBytes',
+    'pydantic:NoneStr',
+    'pydantic:NoneStrBytes',
+    'pydantic:Protocol',
+    'pydantic:PyObject',
+    'pydantic:Required',
+    'pydantic:StrBytes',
+    'pydantic:compiled',
+    'pydantic.config:get_config',
+    'pydantic.config:inherit_config',
+    'pydantic.config:prepare_config',
+    'pydantic:create_model_from_namedtuple',
+    'pydantic:create_model_from_typeddict',
+    'pydantic.dataclasses:create_pydantic_model_from_dataclass',
+    'pydantic.dataclasses:make_dataclass_validator',
+    'pydantic.dataclasses:set_validation',
+    'pydantic.datetime_parse:parse_date',
+    'pydantic.datetime_parse:parse_time',
+    'pydantic.datetime_parse:parse_datetime',
+    'pydantic.datetime_parse:parse_duration',
+    'pydantic.error_wrappers:ErrorWrapper',
+    'pydantic.errors:AnyStrMaxLengthError',
+    'pydantic.errors:AnyStrMinLengthError',
+    'pydantic.errors:ArbitraryTypeError',
+    'pydantic.errors:BoolError',
+    'pydantic.errors:BytesError',
+    'pydantic.errors:CallableError',
+    'pydantic.errors:ClassError',
+    'pydantic.errors:ColorError',
+    'pydantic.errors:ConfigError',
+    'pydantic.errors:DataclassTypeError',
+    'pydantic.errors:DateError',
+    'pydantic.errors:DateNotInTheFutureError',
+    'pydantic.errors:DateNotInThePastError',
+    'pydantic.errors:DateTimeError',
+    'pydantic.errors:DecimalError',
+    'pydantic.errors:DecimalIsNotFiniteError',
+    'pydantic.errors:DecimalMaxDigitsError',
+    'pydantic.errors:DecimalMaxPlacesError',
+    'pydantic.errors:DecimalWholeDigitsError',
+    'pydantic.errors:DictError',
+    'pydantic.errors:DurationError',
+    'pydantic.errors:EmailError',
+    'pydantic.errors:EnumError',
+    'pydantic.errors:EnumMemberError',
+    'pydantic.errors:ExtraError',
+    'pydantic.errors:FloatError',
+    'pydantic.errors:FrozenSetError',
+    'pydantic.errors:FrozenSetMaxLengthError',
+    'pydantic.errors:FrozenSetMinLengthError',
+    'pydantic.errors:HashableError',
+    'pydantic.errors:IPv4AddressError',
+    'pydantic.errors:IPv4InterfaceError',
+    'pydantic.errors:IPv4NetworkError',
+    'pydantic.errors:IPv6AddressError',
+    'pydantic.errors:IPv6InterfaceError',
+    'pydantic.errors:IPv6NetworkError',
+    'pydantic.errors:IPvAnyAddressError',
+    'pydantic.errors:IPvAnyInterfaceError',
+    'pydantic.errors:IPvAnyNetworkError',
+    'pydantic.errors:IntEnumError',
+    'pydantic.errors:IntegerError',
+    'pydantic.errors:InvalidByteSize',
+    'pydantic.errors:InvalidByteSizeUnit',
+    'pydantic.errors:InvalidDiscriminator',
+    'pydantic.errors:InvalidLengthForBrand',
+    'pydantic.errors:JsonError',
+    'pydantic.errors:JsonTypeError',
+    'pydantic.errors:ListError',
+    'pydantic.errors:ListMaxLengthError',
+    'pydantic.errors:ListMinLengthError',
+    'pydantic.errors:ListUniqueItemsError',
+    'pydantic.errors:LuhnValidationError',
+    'pydantic.errors:MissingDiscriminator',
+    'pydantic.errors:MissingError',
+    'pydantic.errors:NoneIsAllowedError',
+    'pydantic.errors:NoneIsNotAllowedError',
+    'pydantic.errors:NotDigitError',
+    'pydantic.errors:NotNoneError',
+    'pydantic.errors:NumberNotGeError',
+    'pydantic.errors:NumberNotGtError',
+    'pydantic.errors:NumberNotLeError',
+    'pydantic.errors:NumberNotLtError',
+    'pydantic.errors:NumberNotMultipleError',
+    'pydantic.errors:PathError',
+    'pydantic.errors:PathNotADirectoryError',
+    'pydantic.errors:PathNotAFileError',
+    'pydantic.errors:PathNotExistsError',
+    'pydantic.errors:PatternError',
+    'pydantic.errors:PyObjectError',
+    'pydantic.errors:PydanticTypeError',
+    'pydantic.errors:PydanticValueError',
+    'pydantic.errors:SequenceError',
+    'pydantic.errors:SetError',
+    'pydantic.errors:SetMaxLengthError',
+    'pydantic.errors:SetMinLengthError',
+    'pydantic.errors:StrError',
+    'pydantic.errors:StrRegexError',
+    'pydantic.errors:StrictBoolError',
+    'pydantic.errors:SubclassError',
+    'pydantic.errors:TimeError',
+    'pydantic.errors:TupleError',
+    'pydantic.errors:TupleLengthError',
+    'pydantic.errors:UUIDError',
+    'pydantic.errors:UUIDVersionError',
+    'pydantic.errors:UrlError',
+    'pydantic.errors:UrlExtraError',
+    'pydantic.errors:UrlHostError',
+    'pydantic.errors:UrlHostTldError',
+    'pydantic.errors:UrlPortError',
+    'pydantic.errors:UrlSchemeError',
+    'pydantic.errors:UrlSchemePermittedError',
+    'pydantic.errors:UrlUserInfoError',
+    'pydantic.errors:WrongConstantError',
+    'pydantic.main:validate_model',
+    'pydantic.networks:stricturl',
+    'pydantic:parse_file_as',
+    'pydantic:parse_raw_as',
+    'pydantic:stricturl',
+    'pydantic.tools:parse_file_as',
+    'pydantic.tools:parse_raw_as',
+    'pydantic.types:ConstrainedBytes',
+    'pydantic.types:ConstrainedDate',
+    'pydantic.types:ConstrainedDecimal',
+    'pydantic.types:ConstrainedFloat',
+    'pydantic.types:ConstrainedFrozenSet',
+    'pydantic.types:ConstrainedInt',
+    'pydantic.types:ConstrainedList',
+    'pydantic.types:ConstrainedSet',
+    'pydantic.types:ConstrainedStr',
+    'pydantic.types:JsonWrapper',
+    'pydantic.types:NoneBytes',
+    'pydantic.types:NoneStr',
+    'pydantic.types:NoneStrBytes',
+    'pydantic.types:PyObject',
+    'pydantic.types:StrBytes',
+    'pydantic.typing:evaluate_forwardref',
+    'pydantic.typing:AbstractSetIntStr',
+    'pydantic.typing:AnyCallable',
+    'pydantic.typing:AnyClassMethod',
+    'pydantic.typing:CallableGenerator',
+    'pydantic.typing:DictAny',
+    'pydantic.typing:DictIntStrAny',
+    'pydantic.typing:DictStrAny',
+    'pydantic.typing:IntStr',
+    'pydantic.typing:ListStr',
+    'pydantic.typing:MappingIntStrAny',
+    'pydantic.typing:NoArgAnyCallable',
+    'pydantic.typing:NoneType',
+    'pydantic.typing:ReprArgs',
+    'pydantic.typing:SetStr',
+    'pydantic.typing:StrPath',
+    'pydantic.typing:TupleGenerator',
+    'pydantic.typing:WithArgsTypes',
+    'pydantic.typing:all_literal_values',
+    'pydantic.typing:display_as_type',
+    'pydantic.typing:get_all_type_hints',
+    'pydantic.typing:get_args',
+    'pydantic.typing:get_origin',
+    'pydantic.typing:get_sub_types',
+    'pydantic.typing:is_callable_type',
+    'pydantic.typing:is_classvar',
+    'pydantic.typing:is_finalvar',
+    'pydantic.typing:is_literal_type',
+    'pydantic.typing:is_namedtuple',
+    'pydantic.typing:is_new_type',
+    'pydantic.typing:is_none_type',
+    'pydantic.typing:is_typeddict',
+    'pydantic.typing:is_typeddict_special',
+    'pydantic.typing:is_union',
+    'pydantic.typing:new_type_supertype',
+    'pydantic.typing:resolve_annotations',
+    'pydantic.typing:typing_base',
+    'pydantic.typing:update_field_forward_refs',
+    'pydantic.typing:update_model_forward_refs',
+    'pydantic.utils:ClassAttribute',
+    'pydantic.utils:DUNDER_ATTRIBUTES',
+    'pydantic.utils:PyObjectStr',
+    'pydantic.utils:ValueItems',
+    'pydantic.utils:almost_equal_floats',
+    'pydantic.utils:get_discriminator_alias_and_values',
+    'pydantic.utils:get_model',
+    'pydantic.utils:get_unique_discriminator_alias',
+    'pydantic.utils:in_ipython',
+    'pydantic.utils:is_valid_identifier',
+    'pydantic.utils:path_type',
+    'pydantic.utils:validate_field_name',
+    'pydantic:validate_model',
 }
 
 
 def getattr_migration(module: str) -> Callable[[str], Any]:
     """Implement PEP 562 for objects that were either moved or removed on the migration
     to V2.
 
@@ -255,20 +263,23 @@
 
         Args:
             name: The object name.
 
         Returns:
             The object.
         """
-        import_path = f'{module}.{name}'
+        import_path = f'{module}:{name}'
         if import_path in MOVED_IN_V2.keys():
             new_location = MOVED_IN_V2[import_path]
             warnings.warn(f'`{import_path}` has been moved to `{new_location}`.')
             return import_string(MOVED_IN_V2[import_path])
         if import_path in DEPRECATED_MOVED_IN_V2.keys():
             # skip the warning here because a deprecation warning will be raised elsewhere
             return import_string(DEPRECATED_MOVED_IN_V2[import_path])
         if import_path in REMOVED_IN_V2:
             raise PydanticImportError(f'`{import_path}` has been removed in V2.')
+        globals: Dict[str, Any] = sys.modules[module].__dict__
+        if name in globals:
+            return globals[name]
         raise AttributeError(f'module {__name__!r} has no attribute {name!r}')
 
     return wrapper
```

### Comparing `pydantic-2.0a4/pydantic/alias_generators.py` & `pydantic-2.0b1/pydantic/alias_generators.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,41 +4,41 @@
 __all__ = ('to_pascal', 'to_camel', 'to_snake')
 
 
 def to_pascal(snake: str) -> str:
     """Convert a snake_case string to PascalCase.
 
     Args:
-        snake (str): The snake_case string to convert.
+        snake: The snake_case string to convert.
 
     Returns:
         str: The PascalCase string.
     """
     camel = snake.title()
     return re.sub('([0-9A-Za-z])_(?=[0-9A-Z])', lambda m: m.group(1), camel)
 
 
 def to_camel(snake: str) -> str:
     """Convert a snake_case string to camelCase.
 
     Args:
-        snake (str): The snake_case string to convert.
+        snake: The snake_case string to convert.
 
     Returns:
         str: The converted camelCase string.
     """
     camel = to_pascal(snake)
     return re.sub('(^_*[A-Z])', lambda m: m.group(1).lower(), camel)
 
 
 def to_snake(camel: str) -> str:
     """Convert a PascalCase or camelCase string to snake_case.
 
     Args:
-        camel (str): The string to convert.
+        camel: The string to convert.
 
     Returns:
         str: The converted string in snake_case.
     """
     snake = re.sub(r'([a-zA-Z])([0-9])', lambda m: f'{m.group(1)}_{m.group(2)}', camel)
     snake = re.sub(r'([a-z0-9])([A-Z])', lambda m: f'{m.group(1)}_{m.group(2)}', snake)
     return snake.lower()
```

### Comparing `pydantic-2.0a4/pydantic/color.py` & `pydantic-2.0b1/pydantic/color.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import re
 from colorsys import hls_to_rgb, rgb_to_hls
 from typing import Any, Callable, Optional, Tuple, Type, Union, cast
 
 from pydantic_core import CoreSchema, PydanticCustomError, core_schema
 
 from ._internal import _repr, _utils
-from ._internal._schema_generation_shared import GetJsonSchemaHandler
+from ._internal._schema_generation_shared import GetJsonSchemaHandler as _GetJsonSchemaHandler
 from .json_schema import JsonSchemaValue
 
 ColorTuple = Union[Tuple[int, int, int], Tuple[int, int, int, float]]
 ColorType = Union[ColorTuple, str]
 HslColorTuple = Union[Tuple[float, float, float], Tuple[float, float, float, float]]
 
 
@@ -87,15 +87,15 @@
             )
 
         # if we've got here value must be a valid color
         self._original = value
 
     @classmethod
     def __get_pydantic_json_schema__(
-        cls, core_schema: core_schema.CoreSchema, handler: GetJsonSchemaHandler
+        cls, core_schema: core_schema.CoreSchema, handler: _GetJsonSchemaHandler
     ) -> JsonSchemaValue:
         field_schema = {}
         field_schema.update(type='string', format='color')
         return field_schema
 
     def original(self) -> ColorType:
         """
@@ -105,19 +105,19 @@
 
     def as_named(self, *, fallback: bool = False) -> str:
         """
         Returns the name of the color if it can be found in `COLORS_BY_VALUE` dictionary,
         otherwise returns the hexadecimal representation of the color or raises `ValueError`.
 
         Args:
-            fallback (bool): If True, falls back to returning the hexadecimal representation of
+            fallback: If True, falls back to returning the hexadecimal representation of
                 the color instead of raising a ValueError when no named color is found.
 
         Returns:
-            str: The name of the color, or the hexadecimal representation of the color.
+            The name of the color, or the hexadecimal representation of the color.
 
         Raises:
             ValueError: When no named color is found and fallback is `False`.
         """
         if self._rgba.alpha is None:
             rgb = cast(Tuple[int, int, int], self.as_rgb_tuple())
             try:
@@ -133,15 +133,15 @@
     def as_hex(self) -> str:
         """Returns the hexadecimal representation of the color.
 
         Hex string representing the color can be 3, 4, 6, or 8 characters depending on whether the string
         a "short" representation of the color is possible and whether there's an alpha channel.
 
         Returns:
-            str: The hexadecimal representation of the color.
+            The hexadecimal representation of the color.
         """
         values = [float_to_255(c) for c in self._rgba[:3]]
         if self._rgba.alpha is not None:
             values.append(float_to_255(self._rgba.alpha))
 
         as_hex = ''.join(f'{v:02x}' for v in values)
         if all(c in repeat_colors for c in values):
@@ -161,22 +161,23 @@
             )
 
     def as_rgb_tuple(self, *, alpha: Optional[bool] = None) -> ColorTuple:
         """
         Returns the color as an RGB or RGBA tuple.
 
         Args:
-            alpha (Optional[bool]): Whether to include the alpha channel. There are three options for this input:
-                `None` (default): Include alpha only if it's set. (e.g. not `None`)
-                `True`: Always include alpha.
-                `False`: Always omit alpha.
+            alpha: Whether to include the alpha channel. There are three options for this input:
+
+                - `None` (default): Include alpha only if it's set. (e.g. not `None`)
+                - `True`: Always include alpha.
+                - `False`: Always omit alpha.
 
         Returns:
-            ColorTuple: A tuple that contains the values of the red, green, and blue channels in the range 0 to 255.
-            If alpha is included, it is in the range 0 to 1.
+            A tuple that contains the values of the red, green, and blue channels in the range 0 to 255.
+                If alpha is included, it is in the range 0 to 1.
         """
         r, g, b = (float_to_255(c) for c in self._rgba[:3])
         if alpha is None:
             if self._rgba.alpha is None:
                 return r, g, b
             else:
                 return r, g, b, self._alpha_float()
@@ -198,21 +199,22 @@
             return f'hsl({h * 360:0.0f}, {s:0.0%}, {li:0.0%}, {round(a, 2)})'
 
     def as_hsl_tuple(self, *, alpha: Optional[bool] = None) -> HslColorTuple:
         """
         Returns the color as an HSL or HSLA tuple.
 
         Args:
-            alpha (Optional[bool]): Whether to include the alpha channel.
-                `None` (default): Include the alpha channel only if it's set (e.g. not `None`).
-                `True`: Always include alpha.
-                `False`: Always omit alpha.
+            alpha: Whether to include the alpha channel.
+
+                - `None` (default): Include the alpha channel only if it's set (e.g. not `None`).
+                - `True`: Always include alpha.
+                - `False`: Always omit alpha.
 
         Returns:
-            HslColorTuple: The color as a tuple of hue, saturation, lightness, and alpha (if included).
+            The color as a tuple of hue, saturation, lightness, and alpha (if included).
                 All elements are in the range 0 to 1.
 
         Note:
             This is HSL as used in HTML and most other places, not HLS as used in Python's `colorsys`.
         """
         h, l, s = rgb_to_hls(self._rgba.r, self._rgba.g, self._rgba.b)  # noqa: E741
         if alpha is None:
@@ -254,18 +256,18 @@
         return hash(self.as_rgb_tuple())
 
 
 def parse_tuple(value: Tuple[Any, ...]) -> RGBA:
     """Parse a tuple or list to get RGBA values.
 
     Args:
-        value (Tuple[Any, ...]): A tuple or list.
+        value: A tuple or list.
 
     Returns:
-        RGBA: An RGBA tuple parsed from the input tuple.
+        An `RGBA` tuple parsed from the input tuple.
 
     Raises:
         PydanticCustomError: If tuple is not valid.
     """
     if len(value) == 3:
         r, g, b = (parse_color_value(v) for v in value)
         return RGBA(r, g, b, None)
@@ -285,18 +287,18 @@
     * named color, see `COLORS_BY_NAME`
     * hex short eg. `<prefix>fff` (prefix can be `#`, `0x` or nothing)
     * hex long eg. `<prefix>ffffff` (prefix can be `#`, `0x` or nothing)
     * `rgb(<r>, <g>, <b>)`
     * `rgba(<r>, <g>, <b>, <a>)`
 
     Args:
-        value (str): A string representing a color.
+        value: A string representing a color.
 
     Returns:
-        RGBA: An RGBA tuple parsed from the input string.
+        An `RGBA` tuple parsed from the input string.
 
     Raises:
         ValueError: If the input string cannot be parsed to an RGBA tuple.
     """
     value_lower = value.lower()
     try:
         r, g, b = COLORS_BY_NAME[value_lower]
@@ -337,38 +339,38 @@
 
 
 def ints_to_rgba(r: Union[int, str], g: Union[int, str], b: Union[int, str], alpha: Optional[float] = None) -> RGBA:
     """
     Converts integer or string values for RGB color and an optional alpha value to an `RGBA` object.
 
     Args:
-        r (Union[int, str]): An integer or string representing the red color value.
-        g (Union[int, str]): An integer or string representing the green color value.
-        b (Union[int, str]): An integer or string representing the blue color value.
-        alpha (float, optional): A float representing the alpha value. Defaults to None.
+        r: An integer or string representing the red color value.
+        g: An integer or string representing the green color value.
+        b: An integer or string representing the blue color value.
+        alpha: A float representing the alpha value. Defaults to None.
 
     Returns:
-        RGBA: An instance of the `RGBA` class with the corresponding color and alpha values.
+        An instance of the `RGBA` class with the corresponding color and alpha values.
     """
     return RGBA(parse_color_value(r), parse_color_value(g), parse_color_value(b), parse_float_alpha(alpha))
 
 
 def parse_color_value(value: Union[int, str], max_val: int = 255) -> float:
     """
     Parse the color value provided and return a number between 0 and 1.
 
     Args:
-        value (Union[int, str]): An integer or string color value.
-        max_val (int, optional): Maximum range value. Defaults to 255.
+        value: An integer or string color value.
+        max_val: Maximum range value. Defaults to 255.
 
     Raises:
         PydanticCustomError: If the value is not a valid color.
 
     Returns:
-        float: A number between 0 and 1.
+        A number between 0 and 1.
     """
     try:
         color = float(value)
     except ValueError:
         raise PydanticCustomError('color_error', 'value is not a valid color: color values must be a valid number')
     if 0 <= color <= max_val:
         return color / max_val
@@ -381,18 +383,18 @@
 
 
 def parse_float_alpha(value: Union[None, str, float, int]) -> Optional[float]:
     """
     Parse an alpha value checking it's a valid float in the range 0 to 1.
 
     Args:
-        value (Union[None, str, float, int]): The input value to parse.
+        value: The input value to parse.
 
     Returns:
-        Optional[float]: The parsed value as a float, or `None` if the value was None or equal 1.
+        The parsed value as a float, or `None` if the value was None or equal 1.
 
     Raises:
         PydanticCustomError: If the input value cannot be successfully parsed as a float in the expected range.
     """
     if value is None:
         return None
     try:
@@ -412,22 +414,22 @@
 
 
 def parse_hsl(h: str, h_units: str, sat: str, light: str, alpha: Optional[float] = None) -> RGBA:
     """
     Parse raw hue, saturation, lightness, and alpha values and convert to RGBA.
 
     Args:
-        h (str): The hue value.
-        h_units (str): The unit for hue value.
-        sat (str): The saturation value.
-        light (str): The lightness value.
-        alpha (Optional[float]): Alpha value.
+        h: The hue value.
+        h_units: The unit for hue value.
+        sat: The saturation value.
+        light: The lightness value.
+        alpha: Alpha value.
 
     Returns:
-        RGBA: An instance of `RGBA`.
+        An instance of `RGBA`.
     """
     s_value, l_value = parse_color_value(sat, 100), parse_color_value(light, 100)
 
     h_value = float(h)
     if h_units in {None, 'deg'}:
         h_value = h_value % 360 / 360
     elif h_units == 'rad':
@@ -441,18 +443,18 @@
 
 
 def float_to_255(c: float) -> int:
     """
     Converts a float value between 0 and 1 (inclusive) to an integer between 0 and 255 (inclusive).
 
     Args:
-        c (float): The float value to be converted. Must be between 0 and 1 (inclusive).
+        c: The float value to be converted. Must be between 0 and 1 (inclusive).
 
     Returns:
-        int: The integer equivalent of the given float value rounded to the nearest whole number.
+        The integer equivalent of the given float value rounded to the nearest whole number.
 
     Raises:
         ValueError: If the given float value is outside the acceptable range of 0 to 1 (inclusive).
     """
     return int(round(c * 255))
```

### Comparing `pydantic-2.0a4/pydantic/config.py` & `pydantic-2.0b1/pydantic/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,54 +41,52 @@
 ExtraValues = Literal['allow', 'ignore', 'forbid']
 
 
 class ConfigDict(TypedDict, total=False):
     """A dictionary-like class for configuring Pydantic models.
 
     Attributes:
-        title (Optional[str]): Optional title for the configuration. Defaults to None.
-        str_to_lower (bool): Whether to convert strings to lowercase. Defaults to False.
-        str_to_upper (bool): Whether to convert strings to uppercase. Defaults to False.
-        str_strip_whitespace (bool): Whether to strip whitespace from strings. Defaults to False.
-        str_min_length (int): The minimum length for strings. Defaults to None.
-        str_max_length (int): The maximum length for strings. Defaults to None.
-        extra (ExtraValues): Extra values to include in this configuration. Defaults to None.
-        frozen (bool): Whether to freeze the configuration. Defaults to False.
-        populate_by_name (bool): Whether to populate fields by name. Defaults to False.
-        use_enum_values (bool): Whether to use enum values. Defaults to False.
-        validate_assignment (bool): Whether to validate assignments. Defaults to False.
-        arbitrary_types_allowed (bool): Whether to allow arbitrary types. Defaults to True.
-        undefined_types_warning (bool): Whether to show a warning for undefined types. Defaults to True.
-        from_attributes (bool): Whether to set attributes from the configuration. Defaults to False.
-        loc_by_alias (bool): Whether to use the alias for error `loc`s. Defaults to True.
-        alias_generator (Optional[Callable[[str], str]]): A function to generate aliases. Defaults to None.
-        ignored_types (Tuple[type, ...]): A tuple of types to ignore. Defaults to ().
-        allow_inf_nan (bool): Whether to allow infinity and NaN. Defaults to False.
-        strict (bool): Whether to make the configuration strict. Defaults to False.
-        revalidate_instances (Literal['always', 'never', 'subclass-instances']):
-            When and how to revalidate models and dataclasses during validation. Defaults to 'never'.
-        ser_json_timedelta (Literal['iso8601', 'float']): The format of JSON serialized timedeltas.
-            Defaults to 'iso8601'.
-        ser_json_bytes (Literal['utf8', 'base64']): The encoding of JSON serialized bytes. Defaults to 'utf8'.
-        validate_default (bool): Whether to validate default values during validation. Defaults to False.
+        title: Optional title for the configuration. Defaults to `None`.
+        str_to_lower: Whether to convert strings to lowercase. Defaults to `False`.
+        str_to_upper: Whether to convert strings to uppercase. Defaults to `False`.
+        str_strip_whitespace: Whether to strip whitespace from strings. Defaults to `False`.
+        str_min_length: The minimum length for strings. Defaults to `None`.
+        str_max_length: The maximum length for strings. Defaults to `None`.
+        extra: Extra values to include in this configuration. Defaults to `None`.
+        frozen: Whether to freeze the configuration. Defaults to `False`.
+        populate_by_name: Whether to populate fields by name. Defaults to `False`.
+        use_enum_values: Whether to use enum values. Defaults to `False`.
+        validate_assignment: Whether to validate assignments. Defaults to `False`.
+        arbitrary_types_allowed: Whether to allow arbitrary types. Defaults to `False`.
+        from_attributes: Whether to set attributes from the configuration. Defaults to `False`.
+        loc_by_alias: Whether to use the alias for error `loc`s. Defaults to `True`.
+        alias_generator: A function to generate aliases. Defaults to `None`.
+        ignored_types: A tuple of types to ignore. Defaults to `()`.
+        allow_inf_nan: Whether to allow infinity and NaN. Defaults to `False`.
+        strict: Whether to make the configuration strict. Defaults to `False`.
+        revalidate_instances: When and how to revalidate models and dataclasses during validation. Defaults to 'never'.
+        ser_json_timedelta: The format of JSON serialized timedeltas. Defaults to 'iso8601'.
+        ser_json_bytes: The encoding of JSON serialized bytes. Defaults to 'utf8'.
+        validate_default: Whether to validate default values during validation. Defaults to `False`.
+        protected_namespaces: A list of protected namespaces. Defaults to `('model_', )`.
+        hide_input_in_errors: Whether to hide inputs when printing errors. Defaults to `False`.
     """
 
     title: str | None
     str_to_lower: bool
     str_to_upper: bool
     str_strip_whitespace: bool
     str_min_length: int
     str_max_length: int | None
     extra: ExtraValues | None
     frozen: bool
     populate_by_name: bool
     use_enum_values: bool
     validate_assignment: bool
-    arbitrary_types_allowed: bool  # TODO default True, or remove
-    undefined_types_warning: bool  # TODO review docs
+    arbitrary_types_allowed: bool
     from_attributes: bool
     # whether to use the used alias (or first alias for "field required" errors) instead of field_names
     # to construct error `loc`s, default True
     loc_by_alias: bool
     alias_generator: Callable[[str], str] | None
     ignored_types: tuple[type, ...]
     allow_inf_nan: bool
@@ -100,10 +98,12 @@
     revalidate_instances: Literal['always', 'never', 'subclass-instances']
     ser_json_timedelta: Literal['iso8601', 'float']
     ser_json_bytes: Literal['utf8', 'base64']
     # whether to validate default values during validation, default False
     validate_default: bool
     # whether to validate the return value from call validator
     validate_return: bool
+    protected_namespaces: tuple[str, ...]
+    hide_input_in_errors: bool
 
 
 __getattr__ = getattr_migration(__name__)
```

### Comparing `pydantic-2.0a4/pydantic/decorators.py` & `pydantic-2.0b1/pydantic/_internal/_decorators.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,587 +1,649 @@
 """
-Public methods used as decorators within pydantic models and dataclasses.
+Logic related to validators applied to models etc. via the `@field_validator` and `@root_validator` decorators.
 """
-
 from __future__ import annotations as _annotations
 
+from collections import deque
+from dataclasses import dataclass, field
 from functools import partial, partialmethod
-from types import FunctionType
-from typing import TYPE_CHECKING, Any, Callable, TypeVar, Union, overload
-from warnings import warn
+from inspect import Parameter, Signature, isdatadescriptor, ismethoddescriptor, signature
+from itertools import islice
+from typing import TYPE_CHECKING, Any, Callable, ClassVar, Generic, Iterable, TypeVar, Union
+
+from pydantic_core import core_schema
+from typing_extensions import Literal, TypeAlias, is_typeddict
+
+from ..errors import PydanticUserError
+from ..fields import ComputedFieldInfo
+from ._core_utils import get_type_ref
+from ._internal_dataclass import slots_dataclass
+from ._typing_extra import get_function_type_hints
 
-from pydantic_core import core_schema as _core_schema
-from typing_extensions import Literal, Protocol, TypeAlias
+if TYPE_CHECKING:
+    from ..functional_validators import FieldValidatorModes
 
-from ._internal import _decorators, _decorators_v1
-from .errors import PydanticUserError
+try:
+    from functools import cached_property  # type: ignore
+except ImportError:
+    # python 3.7
+    cached_property = None
 
-_ALLOW_REUSE_WARNING_MESSAGE = '`allow_reuse` is deprecated and will be ignored; it should no longer be necessary'
 
+@slots_dataclass
+class ValidatorDecoratorInfo:
+    """
+    A container for data from `@validator` so that we can access it
+    while building the pydantic-core schema.
+    """
 
-if TYPE_CHECKING:
+    decorator_repr: ClassVar[str] = '@validator'
 
-    class _OnlyValueValidatorClsMethod(Protocol):
-        def __call__(self, __cls: Any, __value: Any) -> Any:
-            ...
-
-    class _V1ValidatorWithValuesClsMethod(Protocol):
-        def __call__(self, __cls: Any, __value: Any, values: dict[str, Any]) -> Any:
-            ...
-
-    class _V1ValidatorWithValuesKwOnlyClsMethod(Protocol):
-        def __call__(self, __cls: Any, __value: Any, *, values: dict[str, Any]) -> Any:
-            ...
-
-    class _V1ValidatorWithKwargsClsMethod(Protocol):
-        def __call__(self, __cls: Any, **kwargs: Any) -> Any:
-            ...
-
-    class _V1ValidatorWithValuesAndKwargsClsMethod(Protocol):
-        def __call__(self, __cls: Any, values: dict[str, Any], **kwargs: Any) -> Any:
-            ...
-
-    class _V2ValidatorClsMethod(Protocol):
-        def __call__(self, __cls: Any, __input_value: Any, __info: _core_schema.FieldValidationInfo) -> Any:
-            ...
-
-    class _V2WrapValidatorClsMethod(Protocol):
-        def __call__(
-            self,
-            __cls: Any,
-            __input_value: Any,
-            __validator: _core_schema.ValidatorFunctionWrapHandler,
-            __info: _core_schema.ValidationInfo,
-        ) -> Any:
-            ...
-
-    class _V1RootValidatorClsMethod(Protocol):
-        def __call__(
-            self, __cls: Any, __values: _decorators_v1.RootValidatorValues
-        ) -> _decorators_v1.RootValidatorValues:
-            ...
-
-    V1Validator = Union[
-        _OnlyValueValidatorClsMethod,
-        _V1ValidatorWithValuesClsMethod,
-        _V1ValidatorWithValuesKwOnlyClsMethod,
-        _V1ValidatorWithKwargsClsMethod,
-        _V1ValidatorWithValuesAndKwargsClsMethod,
-        _decorators_v1.V1ValidatorWithValues,
-        _decorators_v1.V1ValidatorWithValuesKwOnly,
-        _decorators_v1.V1ValidatorWithKwargs,
-        _decorators_v1.V1ValidatorWithValuesAndKwargs,
-    ]
-
-    V2Validator = Union[
-        _V2ValidatorClsMethod,
-        _core_schema.FieldValidatorFunction,
-        _OnlyValueValidatorClsMethod,
-        _core_schema.NoInfoValidatorFunction,
-    ]
-
-    V2WrapValidator = Union[
-        _V2WrapValidatorClsMethod,
-        _core_schema.GeneralWrapValidatorFunction,
-        _core_schema.FieldWrapValidatorFunction,
-    ]
-
-    V1RootValidator = Union[
-        _V1RootValidatorClsMethod,
-        _decorators_v1.V1RootValidatorFunction,
-    ]
-
-    _PartialClsOrStaticMethod: TypeAlias = Union[classmethod[Any, Any, Any], staticmethod[Any, Any], partialmethod[Any]]
-
-    # Allow both a V1 (assumed pre=False) or V2 (assumed mode='after') validator
-    # We lie to type checkers and say we return the same thing we get
-    # but in reality we return a proxy object that _mostly_ behaves like the wrapped thing
-    _V1ValidatorType = TypeVar('_V1ValidatorType', V1Validator, _PartialClsOrStaticMethod)
-    _V2BeforeAfterOrPlainValidatorType = TypeVar(
-        '_V2BeforeAfterOrPlainValidatorType',
-        V2Validator,
-        _PartialClsOrStaticMethod,
-    )
-    _V2WrapValidatorType = TypeVar('_V2WrapValidatorType', V2WrapValidator, _PartialClsOrStaticMethod)
-    _V1RootValidatorFunctionType = TypeVar(
-        '_V1RootValidatorFunctionType',
-        _decorators_v1.V1RootValidatorFunction,
-        _V1RootValidatorClsMethod,
-        _PartialClsOrStaticMethod,
-    )
+    fields: tuple[str, ...]
+    mode: Literal['before', 'after']
+    each_item: bool
+    always: bool
+    check_fields: bool | None
 
 
-def validator(
-    __field: str,
-    *fields: str,
-    pre: bool = False,
-    each_item: bool = False,
-    always: bool = False,
-    check_fields: bool | None = None,
-    allow_reuse: bool = False,
-) -> Callable[[_V1ValidatorType], _V1ValidatorType]:
+@slots_dataclass
+class FieldValidatorDecoratorInfo:
+    """
+    A container for data from `@field_validator` so that we can access it
+    while building the pydantic-core schema.
     """
-    Decorate methods on the class indicating that they should be used to validate fields.
 
-    Args:
-        __field (str): The first field the validator should be called on; this is separate
-            from `fields` to ensure an error is raised if you don't pass at least one.
-        *fields (str): Additional field(s) the validator should be called on.
-        pre (bool, optional): Whether or not this validator should be called before the standard
-            validators (else after). Defaults to False.
-        each_item (bool, optional): For complex objects (sets, lists etc.) whether to validate
-            individual elements rather than the whole object. Defaults to False.
-        always (bool, optional): Whether this method and other validators should be called even if
-            the value is missing. Defaults to False.
-        check_fields (bool | None, optional): Whether to check that the fields actually exist on the model.
-            Defaults to None.
-        allow_reuse (bool, optional): Whether to track and raise an error if another validator refers to
-            the decorated function. Defaults to False.
+    decorator_repr: ClassVar[str] = '@field_validator'
 
-    Returns:
-        Callable: A decorator that can be used to decorate a
-            function to be used as a validator.
+    fields: tuple[str, ...]
+    mode: FieldValidatorModes
+    check_fields: bool | None
+
+
+@slots_dataclass
+class RootValidatorDecoratorInfo:
+    """
+    A container for data from `@root_validator` so that we can access it
+    while building the pydantic-core schema.
     """
-    if allow_reuse is True:  # pragma: no cover
-        warn(_ALLOW_REUSE_WARNING_MESSAGE, DeprecationWarning)
-    fields = tuple((__field, *fields))
-    if isinstance(fields[0], FunctionType):
-        raise PydanticUserError(
-            "validators should be used with fields and keyword arguments, not bare. "
-            "E.g. usage should be `@validator('<field_name>', ...)`",
-            code='validator-no-fields',
-        )
-    elif not all(isinstance(field, str) for field in fields):
-        raise PydanticUserError(
-            "validator fields should be passed as separate string args. "
-            "E.g. usage should be `@validator('<field_name_1>', '<field_name_2>', ...)`",
-            code='validator-invalid-fields',
-        )
 
-    warn(
-        'Pydantic V1 style `@validator` validators are deprecated.'
-        ' You should migrate to Pydantic V2 style `@field_validator` validators,'
-        ' see the migration guide for more details',
-        DeprecationWarning,
-        stacklevel=2,
-    )
+    decorator_repr: ClassVar[str] = '@root_validator'
+    mode: Literal['before', 'after']
 
-    mode: Literal['before', 'after'] = 'before' if pre is True else 'after'
 
-    def dec(f: Any) -> _decorators.PydanticDescriptorProxy[Any]:
-        if _decorators.is_instance_method_from_sig(f):
-            raise PydanticUserError(
-                '`@validator` cannot be applied to instance methods', code='validator-instance-method'
-            )
-        # auto apply the @classmethod decorator
-        f = _decorators.ensure_classmethod_based_on_signature(f)
-        wrap = _decorators_v1.make_generic_v1_field_validator
-        validator_wrapper_info = _decorators.ValidatorDecoratorInfo(
-            fields=fields,
-            mode=mode,
-            each_item=each_item,
-            always=always,
-            check_fields=check_fields,
-        )
-        return _decorators.PydanticDescriptorProxy(f, validator_wrapper_info, shim=wrap)
+@slots_dataclass
+class FieldSerializerDecoratorInfo:
+    """
+    A container for data from `@field_serializer` so that we can access it
+    while building the pydantic-core schema.
+    """
 
-    return dec  # type: ignore[return-value]
+    decorator_repr: ClassVar[str] = '@field_serializer'
+    fields: tuple[str, ...]
+    mode: Literal['plain', 'wrap']
+    return_type: Any
+    when_used: core_schema.WhenUsed
+    check_fields: bool | None
 
 
-@overload
-def field_validator(
-    __field: str,
-    *fields: str,
-    mode: Literal['before', 'after', 'plain'] = ...,
-    check_fields: bool | None = ...,
-) -> Callable[[_V2BeforeAfterOrPlainValidatorType], _V2BeforeAfterOrPlainValidatorType]:
-    ...
+@slots_dataclass
+class ModelSerializerDecoratorInfo:
+    """
+    A container for data from `@model_serializer` so that we can access it
+    while building the pydantic-core schema.
+    """
 
+    decorator_repr: ClassVar[str] = '@model_serializer'
+    mode: Literal['plain', 'wrap']
+    return_type: Any
+    when_used: core_schema.WhenUsed
 
-@overload
-def field_validator(
-    __field: str,
-    *fields: str,
-    mode: Literal['wrap'],
-    check_fields: bool | None = ...,
-) -> Callable[[_V2WrapValidatorType], _V2WrapValidatorType]:
-    ...
 
+@slots_dataclass
+class ModelValidatorDecoratorInfo:
+    """
+    A container for data from `@model_validator` so that we can access it
+    while building the pydantic-core schema.
+    """
 
-FieldValidatorModes: TypeAlias = Literal['before', 'after', 'wrap', 'plain']
+    decorator_repr: ClassVar[str] = '@model_validator'
+    mode: Literal['wrap', 'before', 'after']
 
 
-def field_validator(
-    __field: str,
-    *fields: str,
-    mode: FieldValidatorModes = 'after',
-    check_fields: bool | None = None,
-) -> Callable[[Any], Any]:
-    """
-    Decorate methods on the class indicating that they should be used to validate fields.
+DecoratorInfo = Union[
+    ValidatorDecoratorInfo,
+    FieldValidatorDecoratorInfo,
+    RootValidatorDecoratorInfo,
+    FieldSerializerDecoratorInfo,
+    ModelSerializerDecoratorInfo,
+    ModelValidatorDecoratorInfo,
+    ComputedFieldInfo,
+]
 
-    Args:
-        __field (str): The first field the field_validator should be called on; this is separate
-            from `fields` to ensure an error is raised if you don't pass at least one.
-        *fields (tuple): Additional field(s) the field_validator should be called on.
-        mode (FieldValidatorModes): Specifies whether to validate the fields before or after validation.
-             Defaults to 'after'.
-        check_fields (bool | None): If set to True, checks that the fields actually exist on the model.
-            Defaults to None.
+ReturnType = TypeVar('ReturnType')
+DecoratedType: TypeAlias = (
+    'Union[classmethod[Any, Any, ReturnType], staticmethod[Any, ReturnType], Callable[..., ReturnType], property]'
+)
 
-    Returns:
-        Callable: A decorator that can be used to decorate a function to be used as a field_validator.
-    """
-    if isinstance(__field, FunctionType):
-        raise PydanticUserError(
-            'field_validators should be used with fields and keyword arguments, not bare. '
-            "E.g. usage should be `@validator('<field_name>', ...)`",
-            code='validator-no-fields',
-        )
-    fields = __field, *fields
-    if not all(isinstance(field, str) for field in fields):
-        raise PydanticUserError(
-            'field_validator fields should be passed as separate string args. '
-            "E.g. usage should be `@validator('<field_name_1>', '<field_name_2>', ...)`",
-            code='validator-invalid-fields',
-        )
 
-    def dec(
-        f: Callable[..., Any] | staticmethod[Any, Any] | classmethod[Any, Any, Any]
-    ) -> _decorators.PydanticDescriptorProxy[Any]:
-        if _decorators.is_instance_method_from_sig(f):
-            raise PydanticUserError(
-                '`@field_validator` cannot be applied to instance methods', code='validator-instance-method'
-            )
+@dataclass  # can't use slots here since we set attributes on `__post_init__`
+class PydanticDescriptorProxy(Generic[ReturnType]):
+    """
+    Wrap a classmethod, staticmethod, property or unbound function
+    and act as a descriptor that allows us to detect decorated items
+    from the class' attributes.
 
-        # auto apply the @classmethod decorator
-        f = _decorators.ensure_classmethod_based_on_signature(f)
+    This class' __get__ returns the wrapped item's __get__ result,
+    which makes it transparent for classmethods and staticmethods.
+    """
 
-        dec_info = _decorators.FieldValidatorDecoratorInfo(fields=fields, mode=mode, check_fields=check_fields)
-        return _decorators.PydanticDescriptorProxy(f, dec_info)
+    wrapped: DecoratedType[ReturnType]
+    decorator_info: DecoratorInfo
+    shim: Callable[[Callable[..., Any]], Callable[..., Any]] | None = None
 
-    return dec
+    def __post_init__(self):
+        for attr in 'setter', 'deleter':
+            if hasattr(self.wrapped, attr):
+                f = partial(self._call_wrapped_attr, name=attr)
+                setattr(self, attr, f)
 
+    def _call_wrapped_attr(self, func: Callable[[Any], None], *, name: str) -> PydanticDescriptorProxy[ReturnType]:
+        self.wrapped = getattr(self.wrapped, name)(func)
+        return self
 
-@overload
-def root_validator(
-    *,
-    # if you don't specify `pre` the default is `pre=False`
-    # which means you need to specify `skip_on_failure=True`
-    skip_on_failure: Literal[True],
-    allow_reuse: bool = ...,
-) -> Callable[[_V1RootValidatorFunctionType], _V1RootValidatorFunctionType,]:
-    ...
+    def __get__(self, obj: object | None, obj_type: type[object] | None = None) -> PydanticDescriptorProxy[ReturnType]:
+        try:
+            return self.wrapped.__get__(obj, obj_type)
+        except AttributeError:
+            # not a descriptor, e.g. a partial object
+            return self.wrapped  # type: ignore[return-value]
 
+    def __set_name__(self, instance: Any, name: str) -> None:
+        if hasattr(self.wrapped, '__set_name__'):
+            self.wrapped.__set_name__(instance, name)
 
-@overload
-def root_validator(
-    *,
-    # if you specify `pre=True` then you don't need to specify
-    # `skip_on_failure`, in fact it is not allowed as an argument!
-    pre: Literal[True],
-    allow_reuse: bool = ...,
-) -> Callable[[_V1RootValidatorFunctionType], _V1RootValidatorFunctionType,]:
-    ...
+    def __getattr__(self, __name: str) -> Any:
+        """Forward checks for __isabstractmethod__ and such"""
+        return getattr(self.wrapped, __name)
 
 
-@overload
-def root_validator(
-    *,
-    # if you explicitly specify `pre=False` then you
-    # MUST specify `skip_on_failure=True`
-    pre: Literal[False],
-    skip_on_failure: Literal[True],
-    allow_reuse: bool = ...,
-) -> Callable[[_V1RootValidatorFunctionType], _V1RootValidatorFunctionType,]:
-    ...
+DecoratorInfoType = TypeVar('DecoratorInfoType', bound=DecoratorInfo)
 
 
-def root_validator(
-    *,
-    pre: bool = False,
-    skip_on_failure: bool = False,
-    allow_reuse: bool = False,
-) -> Any:
+@slots_dataclass
+class Decorator(Generic[DecoratorInfoType]):
+    """
+    A generic container class to join together the decorator metadata
+    (metadata from decorator itself, which we have when the
+    decorator is called but not when we are building the core-schema)
+    and the bound function (which we have after the class itself is created).
     """
-    Decorate methods on a model indicating that they should be used to validate (and perhaps
-    modify) data either before or after standard model parsing/validation is performed.
+
+    cls_ref: str
+    cls_var_name: str
+    func: Callable[..., Any]
+    shim: Callable[[Any], Any] | None
+    info: DecoratorInfoType
+
+    @staticmethod
+    def build(
+        cls_: Any,
+        *,
+        cls_var_name: str,
+        shim: Callable[[Any], Any] | None,
+        info: DecoratorInfoType,
+    ) -> Decorator[DecoratorInfoType]:
+        func = get_attribute_from_bases(cls_, cls_var_name)
+        if shim is not None:
+            func = shim(func)
+        return Decorator(
+            cls_ref=get_type_ref(cls_),
+            cls_var_name=cls_var_name,
+            func=func,
+            shim=shim,
+            info=info,
+        )
+
+    def bind_to_cls(self, cls: Any) -> Decorator[DecoratorInfoType]:
+        return self.build(
+            cls,
+            cls_var_name=self.cls_var_name,
+            shim=self.shim,
+            info=self.info,
+        )
+
+
+def get_bases(tp: type[Any]) -> tuple[type[Any], ...]:
+    if is_typeddict(tp):
+        return tp.__orig_bases__  # type: ignore
+    try:
+        return tp.__bases__
+    except AttributeError:
+        return ()
+
+
+def mro(tp: type[Any]) -> tuple[type[Any], ...]:
+    """
+    Calculate the Method Resolution Order of bases using the C3 algorithm.
+
+    See https://www.python.org/download/releases/2.3/mro/
+    """
+
+    # try to use the existing mro, for performance mainly
+    # but also because it helps verify the implementation below
+    if not is_typeddict(tp):
+        try:
+            return tp.__mro__
+        except AttributeError:
+            # GenericAlias and some other cases
+            pass
+
+    def merge_seqs(seqs: list[deque[type[Any]]]) -> Iterable[type[Any]]:
+        while True:
+            non_empty = [seq for seq in seqs if seq]
+            if not non_empty:
+                # Nothing left to process, we're done.
+                return
+            candidate: type[Any] | None = None
+            for seq in non_empty:  # Find merge candidates among seq heads.
+                candidate = seq[0]
+                not_head = [s for s in non_empty if candidate in islice(s, 1, None)]
+                if not_head:
+                    # Reject the candidate.
+                    candidate = None
+                else:
+                    break
+            if not candidate:
+                raise TypeError('Inconsistent hierarchy, no C3 MRO is possible')
+            yield candidate
+            for seq in non_empty:
+                # Remove candidate.
+                if seq[0] == candidate:
+                    seq.popleft()
+
+    bases = get_bases(tp)
+    seqs = [deque(mro(base)) for base in bases] + [deque(bases)]
+    res = tuple(merge_seqs(seqs))
+
+    return (tp,) + res
+
+
+def get_attribute_from_bases(tp: type[Any], name: str) -> Any:
+    """
+    Get the attribute from the next class in the MRO that has it,
+    aiming to simulate calling the method on the actual class.
+
+    The reason for iterating over the mro instead of just getting
+    the attribute (which would do that for us) is to support TypedDict,
+    which lacks a real __mro__, but can have a virtual one constructed
+    from its bases (as done here).
 
     Args:
-        pre (bool, optional): Whether or not this validator should be called before the standard
-            validators (else after). Defaults to False.
-        skip_on_failure (bool, optional): Whether to stop validation and return as soon as a
-            failure is encountered. Defaults to False.
-        allow_reuse (bool, optional): Whether to track and raise an error if another validator
-            refers to the decorated function. Defaults to False.
+        tp (type[Any]): The type or class to search for the attribute.
+        name (str): The name of the attribute to retrieve.
 
     Returns:
-        Any: A decorator that can be used to decorate a function to be used as a root_validator.
+        Any: The attribute value, if found.
+
+    Raises:
+        AttributeError: If the attribute is not found in any class in the MRO.
     """
-    if allow_reuse is True:  # pragma: no cover
-        warn(_ALLOW_REUSE_WARNING_MESSAGE, DeprecationWarning)
-    mode: Literal['before', 'after'] = 'before' if pre is True else 'after'
-    if pre is False and skip_on_failure is not True:
-        raise PydanticUserError(
-            'If you use `@root_validator` with pre=False (the default) you MUST specify `skip_on_failure=True`.',
-            code='root-validator-pre-skip',
-        )
+    try:
+        return getattr(tp, name)
+    except Exception as e:
+        for base in reversed(mro(tp)):
+            if hasattr(base, name):
+                return getattr(base, name)
+        raise e
+
+
+@slots_dataclass
+class DecoratorInfos:
+    # mapping of name in the class namespace to decorator info
+    # note that the name in the class namespace is the function or attribute name
+    # not the field name!
+    validators: dict[str, Decorator[ValidatorDecoratorInfo]] = field(default_factory=dict)
+    field_validators: dict[str, Decorator[FieldValidatorDecoratorInfo]] = field(default_factory=dict)
+    root_validators: dict[str, Decorator[RootValidatorDecoratorInfo]] = field(default_factory=dict)
+    field_serializers: dict[str, Decorator[FieldSerializerDecoratorInfo]] = field(default_factory=dict)
+    model_serializers: dict[str, Decorator[ModelSerializerDecoratorInfo]] = field(default_factory=dict)
+    model_validators: dict[str, Decorator[ModelValidatorDecoratorInfo]] = field(default_factory=dict)
+    computed_fields: dict[str, Decorator[ComputedFieldInfo]] = field(default_factory=dict)
 
-    wrap = partial(_decorators_v1.make_v1_generic_root_validator, pre=pre)
+    @staticmethod
+    def build(model_dc: type[Any]) -> DecoratorInfos:  # noqa: C901 (ignore complexity)
+        """
+        We want to collect all DecFunc instances that exist as
+        attributes in the namespace of the class (a BaseModel or dataclass)
+        that called us
+        But we want to collect these in the order of the bases
+        So instead of getting them all from the leaf class (the class that called us),
+        we traverse the bases from root (the oldest ancestor class) to leaf
+        and collect all of the instances as we go, taking care to replace
+        any duplicate ones with the last one we see to mimic how function overriding
+        works with inheritance.
+        If we do replace any functions we put the replacement into the position
+        the replaced function was in; that is, we maintain the order.
+        """
+
+        # reminder: dicts are ordered and replacement does not alter the order
+        res = DecoratorInfos()
+        for base in reversed(mro(model_dc)[1:]):
+            existing: DecoratorInfos | None = base.__dict__.get('__pydantic_decorators__')
+            if existing is None:
+                existing = DecoratorInfos.build(base)
+            res.validators.update({k: v.bind_to_cls(model_dc) for k, v in existing.validators.items()})
+            res.field_validators.update({k: v.bind_to_cls(model_dc) for k, v in existing.field_validators.items()})
+            res.root_validators.update({k: v.bind_to_cls(model_dc) for k, v in existing.root_validators.items()})
+            res.field_serializers.update({k: v.bind_to_cls(model_dc) for k, v in existing.field_serializers.items()})
+            res.model_serializers.update({k: v.bind_to_cls(model_dc) for k, v in existing.model_serializers.items()})
+            res.model_validators.update({k: v.bind_to_cls(model_dc) for k, v in existing.model_validators.items()})
+            res.computed_fields.update({k: v.bind_to_cls(model_dc) for k, v in existing.computed_fields.items()})
+
+        to_replace: list[tuple[str, Any]] = []
+
+        for var_name, var_value in vars(model_dc).items():
+            if isinstance(var_value, PydanticDescriptorProxy):
+                info = var_value.decorator_info
+                if isinstance(info, ValidatorDecoratorInfo):
+                    res.validators[var_name] = Decorator.build(
+                        model_dc, cls_var_name=var_name, shim=var_value.shim, info=info
+                    )
+                elif isinstance(info, FieldValidatorDecoratorInfo):
+                    res.field_validators[var_name] = Decorator.build(
+                        model_dc, cls_var_name=var_name, shim=var_value.shim, info=info
+                    )
+                elif isinstance(info, RootValidatorDecoratorInfo):
+                    res.root_validators[var_name] = Decorator.build(
+                        model_dc, cls_var_name=var_name, shim=var_value.shim, info=info
+                    )
+                elif isinstance(info, FieldSerializerDecoratorInfo):
+                    # check whether a serializer function is already registered for fields
+                    for field_serializer_decorator in res.field_serializers.values():
+                        # check that each field has at most one serializer function.
+                        # serializer functions for the same field in subclasses are allowed,
+                        # and are treated as overrides
+                        if field_serializer_decorator.cls_var_name == var_name:
+                            continue
+                        for f in info.fields:
+                            if f in field_serializer_decorator.info.fields:
+                                raise PydanticUserError(
+                                    'Multiple field serializer functions were defined '
+                                    f'for field {f!r}, this is not allowed.',
+                                    code='multiple-field-serializers',
+                                )
+                    res.field_serializers[var_name] = Decorator.build(
+                        model_dc, cls_var_name=var_name, shim=var_value.shim, info=info
+                    )
+                elif isinstance(info, ModelValidatorDecoratorInfo):
+                    res.model_validators[var_name] = Decorator.build(
+                        model_dc, cls_var_name=var_name, shim=var_value.shim, info=info
+                    )
+                elif isinstance(info, ModelSerializerDecoratorInfo):
+                    res.model_serializers[var_name] = Decorator.build(
+                        model_dc, cls_var_name=var_name, shim=var_value.shim, info=info
+                    )
+                else:
+                    isinstance(var_value, ComputedFieldInfo)
+                    res.computed_fields[var_name] = Decorator.build(
+                        model_dc, cls_var_name=var_name, shim=None, info=info
+                    )
+                to_replace.append((var_name, var_value.wrapped))
+        if to_replace:
+            # If we can save `__pydantic_decorators__` on the class we'll be able to check for it above
+            # so then we don't need to re-process the type, which means we can discard our descriptor wrappers
+            # and replace them with the thing they are wrapping (see the other setattr call below)
+            # which allows validator class methods to also function as regular class methods
+            setattr(model_dc, '__pydantic_decorators__', res)
+            for name, value in to_replace:
+                setattr(model_dc, name, value)
+        return res
 
-    def dec(f: Callable[..., Any] | classmethod[Any, Any, Any] | staticmethod[Any, Any]) -> Any:
-        if _decorators.is_instance_method_from_sig(f):
-            raise TypeError('`@root_validator` cannot be applied to instance methods')
-        # auto apply the @classmethod decorator
-        res = _decorators.ensure_classmethod_based_on_signature(f)
-        dec_info = _decorators.RootValidatorDecoratorInfo(mode=mode)
-        return _decorators.PydanticDescriptorProxy(res, dec_info, shim=wrap)
 
-    return dec
+def inspect_validator(validator: Callable[..., Any], mode: FieldValidatorModes) -> bool:
+    """
+    Look at a field or model validator function and determine if it whether it takes an info argument.
 
+    An error is raised if the function has an invalid signature.
 
-if TYPE_CHECKING:
-    _PlainSerializationFunction = Union[_core_schema.SerializerFunction, _PartialClsOrStaticMethod]
+    Args:
+        validator: The validator function to inspect.
+        mode: The proposed validator mode.
 
-    _WrapSerializationFunction = Union[_core_schema.WrapSerializerFunction, _PartialClsOrStaticMethod]
+    Returns:
+        Whether the validator takes an info argument.
+    """
+    sig = signature(validator)
+    n_positional = count_positional_params(sig)
+    if mode == 'wrap':
+        if n_positional == 3:
+            return True
+        elif n_positional == 2:
+            return False
+    else:
+        assert mode in {'before', 'after', 'plain'}, f"invalid mode: {mode!r}, expected 'before', 'after' or 'plain"
+        if n_positional == 2:
+            return True
+        elif n_positional == 1:
+            return False
+
+    raise PydanticUserError(
+        f'Unrecognized field_validator function signature for {validator} with `mode={mode}`:{sig}',
+        code='validator-signature',
+    )
 
-    _PlainSerializeMethodType = TypeVar('_PlainSerializeMethodType', bound=_PlainSerializationFunction)
-    _WrapSerializeMethodType = TypeVar('_WrapSerializeMethodType', bound=_WrapSerializationFunction)
 
+def inspect_field_serializer(serializer: Callable[..., Any], mode: Literal['plain', 'wrap']) -> tuple[bool, bool]:
+    """
+    Look at a field serializer function and determine if it is a field serializer,
+    and whether it takes an info argument.
 
-@overload
-def field_serializer(
-    __field: str,
-    *fields: str,
-    json_return_type: _core_schema.JsonReturnTypes | None = ...,
-    when_used: Literal['always', 'unless-none', 'json', 'json-unless-none'] = ...,
-    check_fields: bool | None = ...,
-) -> Callable[[_PlainSerializeMethodType], _PlainSerializeMethodType]:
-    ...
-
-
-@overload
-def field_serializer(
-    __field: str,
-    *fields: str,
-    mode: Literal['plain'],
-    json_return_type: _core_schema.JsonReturnTypes | None = ...,
-    when_used: Literal['always', 'unless-none', 'json', 'json-unless-none'] = ...,
-    check_fields: bool | None = ...,
-) -> Callable[[_PlainSerializeMethodType], _PlainSerializeMethodType]:
-    ...
-
-
-@overload
-def field_serializer(
-    __field: str,
-    *fields: str,
-    mode: Literal['wrap'],
-    json_return_type: _core_schema.JsonReturnTypes | None = ...,
-    when_used: Literal['always', 'unless-none', 'json', 'json-unless-none'] = ...,
-    check_fields: bool | None = ...,
-) -> Callable[[_WrapSerializeMethodType], _WrapSerializeMethodType]:
-    ...
-
-
-def field_serializer(
-    *fields: str,
-    mode: Literal['plain', 'wrap'] = 'plain',
-    json_return_type: _core_schema.JsonReturnTypes | None = None,
-    when_used: Literal['always', 'unless-none', 'json', 'json-unless-none'] = 'always',
-    check_fields: bool | None = None,
-) -> Callable[[Any], Any]:
-    """
-    Decorate methods on the class indicating that they should be used to serialize fields.
-
-    Four signatures are supported:
-
-    - `(self, value: Any, info: FieldSerializationInfo)`
-    - `(self, value: Any, nxt: SerializerFunctionWrapHandler, info: FieldSerializationInfo)`
-    - `(value: Any, info: SerializationInfo)`
-    - `(value: Any, nxt: SerializerFunctionWrapHandler, info: SerializationInfo)`
+    An error is raised if the function has an invalid signature.
 
     Args:
-        fields (str): Which field(s) the method should be called on.
-        mode (str): `plain` means the function will be called instead of the default serialization logic,
-            `wrap` means the function will be called with an argument to optionally call the
-            default serialization logic.
-        json_return_type (str): The type that the function returns if the serialization mode is JSON.
-        when_used (str): When the function should be called.
-        check_fields (bool): Whether to check that the fields actually exist on the model.
+        serializer: The serializer function to inspect.
+        mode: The serializer mode, either 'plain' or 'wrap'.
 
     Returns:
-        Callable: A decorator that can be used to decorate a function to be used as a field serializer.
+        Tuple of (is_field_serializer, info_arg)
     """
+    sig = signature(serializer)
 
-    def dec(
-        f: Callable[..., Any] | staticmethod[Any, Any] | classmethod[Any, Any, Any]
-    ) -> _decorators.PydanticDescriptorProxy[Any]:
-        dec_info = _decorators.FieldSerializerDecoratorInfo(
-            fields=fields,
-            mode=mode,
-            json_return_type=json_return_type,
-            when_used=when_used,
-            check_fields=check_fields,
-        )
-        return _decorators.PydanticDescriptorProxy(f, dec_info)
+    first = next(iter(sig.parameters.values()), None)
+    is_field_serializer = first is not None and first.name == 'self'
 
-    return dec
+    n_positional = count_positional_params(sig)
+    if is_field_serializer:
+        # -1 to correct for self parameter
+        info_arg = _serializer_info_arg(mode, n_positional - 1)
+    else:
+        info_arg = _serializer_info_arg(mode, n_positional)
+
+    if info_arg is None:
+        raise PydanticUserError(
+            f'Unrecognized field_serializer function signature for {serializer} with `mode={mode}`:{sig}',
+            code='field-serializer-signature',
+        )
+    else:
+        return is_field_serializer, info_arg
 
 
-def model_serializer(
-    __f: Callable[..., Any] | None = None,
-    *,
-    mode: Literal['plain', 'wrap'] = 'plain',
-    json_return_type: _core_schema.JsonReturnTypes | None = None,
-) -> Callable[[Any], _decorators.PydanticDescriptorProxy[Any]] | _decorators.PydanticDescriptorProxy[Any]:
+def inspect_annotated_serializer(serializer: Callable[..., Any], mode: Literal['plain', 'wrap']) -> bool:
     """
-    Decorate a function which will be called to serialize the model.
+    Look at a serializer function used via `Annotated` and determine whether it takes an info argument.
 
-    (`when_used` is not permitted here since it makes no sense.)
+    An error is raised if the function has an invalid signature.
 
     Args:
-        __f (Callable[..., Any] | None): The function to be decorated.
-        mode (Literal['plain', 'wrap']): The serialization mode. `'plain'` means the function will be called
-            instead of the default serialization logic, `'wrap'` means the function will be called with an argument
-            to optionally call the default serialization logic.
-        json_return_type (_core_schema.JsonReturnTypes | None): The type that the function returns if the
-            serialization mode is JSON.
+        serializer: The serializer function to check.
+        mode: The serializer mode, either 'plain' or 'wrap'.
 
     Returns:
-        Callable: A decorator that can be used to decorate a function to be used as a model serializer.
+        info_arg
     """
+    sig = signature(serializer)
+    info_arg = _serializer_info_arg(mode, count_positional_params(sig))
+    if info_arg is None:
+        raise PydanticUserError(
+            f'Unrecognized field_serializer function signature for {serializer} with `mode={mode}`:{sig}',
+            code='field-serializer-signature',
+        )
+    else:
+        return info_arg
 
-    def dec(f: Callable[..., Any]) -> _decorators.PydanticDescriptorProxy[Any]:
-        dec_info = _decorators.ModelSerializerDecoratorInfo(mode=mode, json_return_type=json_return_type)
-        return _decorators.PydanticDescriptorProxy(f, dec_info)
 
-    if __f is None:
-        return dec
-    else:
-        return dec(__f)
+def inspect_model_serializer(serializer: Callable[..., Any], mode: Literal['plain', 'wrap']) -> bool:
+    """
+    Look at a model serializer function and determine whether it takes an info argument.
 
+    An error is raised if the function has an invalid signature.
 
-ModelType = TypeVar('ModelType')
-ModelWrapValidatorHandler = Callable[[Any], ModelType]
+    Args:
+        serializer: The serializer function to check.
+        mode: The serializer mode, either 'plain' or 'wrap'.
 
+    Returns:
+        `info_arg` - whether the function expects an info argument
+    """
 
-class ModelWrapValidatorWithoutInfo(Protocol):
-    def __call__(
-        self,
-        cls: type[ModelType],
-        # this can be a dict, a model instance
-        # or anything else that gets passed to validate_python
-        # thus validators _must_ handle all cases
-        __value: Any,
-        __handler: Callable[[Any], ModelType],
-    ) -> ModelType:
-        ...
-
-
-class ModelWrapValidator(Protocol):
-    def __call__(
-        self,
-        cls: type[ModelType],
-        # this can be a dict, a model instance
-        # or anything else that gets passed to validate_python
-        # thus validators _must_ handle all cases
-        __value: Any,
-        __handler: Callable[[Any], ModelType],
-        __info: _core_schema.ValidationInfo,
-    ) -> ModelType:
-        ...
-
-
-class ModelBeforeValidatorWithoutInfo(Protocol):
-    def __call__(
-        self,
-        cls: Any,
-        # this can be a dict, a model instance
-        # or anything else that gets passed to validate_python
-        # thus validators _must_ handle all cases
-        __value: Any,
-    ) -> Any:
-        ...
-
-
-class ModelBeforeValidator(Protocol):
-    def __call__(
-        self,
-        cls: Any,
-        # this can be a dict, a model instance
-        # or anything else that gets passed to validate_python
-        # thus validators _must_ handle all cases
-        __value: Any,
-        __info: _core_schema.ValidationInfo,
-    ) -> Any:
-        ...
+    if isinstance(serializer, (staticmethod, classmethod)) or not is_instance_method_from_sig(serializer):
+        raise PydanticUserError(
+            '`@model_serializer` must be applied to instance methods', code='model-serializer-instance-method'
+        )
 
+    sig = signature(serializer)
+    info_arg = _serializer_info_arg(mode, count_positional_params(sig))
+    if info_arg is None:
+        raise PydanticUserError(
+            f'Unrecognized model_serializer function signature for {serializer} with `mode={mode}`:{sig}',
+            code='model-serializer-signature',
+        )
+    else:
+        return info_arg
 
-class ModelAfterValidatorWithoutInfo(Protocol):
-    @staticmethod
-    def __call__(
-        self: ModelType,  # type: ignore
-    ) -> ModelType:
-        ...
 
+def _serializer_info_arg(mode: Literal['plain', 'wrap'], n_positional: int) -> bool | None:
+    if mode == 'plain':
+        if n_positional == 1:
+            # (__input_value: Any) -> Any
+            return False
+        elif n_positional == 2:
+            # (__model: Any, __input_value: Any) -> Any
+            return True
+    else:
+        assert mode == 'wrap', f"invalid mode: {mode!r}, expected 'plain' or 'wrap'"
+        if n_positional == 2:
+            # (__input_value: Any, __serializer: SerializerFunctionWrapHandler) -> Any
+            return False
+        elif n_positional == 3:
+            # (__input_value: Any, __serializer: SerializerFunctionWrapHandler, __info: SerializationInfo) -> Any
+            return True
 
-class ModelAfterValidator(Protocol):
-    @staticmethod
-    def __call__(
-        self: ModelType,  # type: ignore
-        __info: _core_schema.ValidationInfo,
-    ) -> ModelType:
-        ...
+    return None
 
 
-AnyModelWrapValidator = Union[ModelWrapValidator, ModelWrapValidatorWithoutInfo]
-AnyModeBeforeValidator = Union[ModelBeforeValidator, ModelBeforeValidatorWithoutInfo]
-AnyModeAfterValidator = Union[ModelAfterValidator, ModelAfterValidatorWithoutInfo]
+AnyDecoratorCallable: TypeAlias = (
+    'Union[classmethod[Any, Any, Any], staticmethod[Any, Any], partialmethod[Any], Callable[..., Any]]'
+)
 
 
-@overload
-def model_validator(
-    *,
-    mode: Literal['wrap'],
-) -> Callable[[AnyModelWrapValidator], _decorators.PydanticDescriptorProxy[_decorators.ModelValidatorDecoratorInfo]]:
-    ...
+def is_instance_method_from_sig(function: AnyDecoratorCallable) -> bool:
+    sig = signature(unwrap_wrapped_function(function))
+    first = next(iter(sig.parameters.values()), None)
+    if first and first.name == 'self':
+        return True
+    return False
 
 
-@overload
-def model_validator(
-    *,
-    mode: Literal['before'],
-) -> Callable[[AnyModeBeforeValidator], _decorators.PydanticDescriptorProxy[_decorators.ModelValidatorDecoratorInfo]]:
-    ...
+def ensure_classmethod_based_on_signature(function: AnyDecoratorCallable) -> Any:
+    if not isinstance(
+        unwrap_wrapped_function(function, unwrap_class_static_method=False), classmethod
+    ) and _is_classmethod_from_sig(function):
+        return classmethod(function)  # type: ignore[arg-type]
+    return function
 
 
-@overload
-def model_validator(
-    *,
-    mode: Literal['after'],
-) -> Callable[[AnyModeAfterValidator], _decorators.PydanticDescriptorProxy[_decorators.ModelValidatorDecoratorInfo]]:
-    ...
+def _is_classmethod_from_sig(function: AnyDecoratorCallable) -> bool:
+    sig = signature(unwrap_wrapped_function(function))
+    first = next(iter(sig.parameters.values()), None)
+    if first and first.name == 'cls':
+        return True
+    return False
 
 
-def model_validator(
+def unwrap_wrapped_function(
+    func: Any,
     *,
-    mode: Literal['wrap', 'before', 'after'],
+    unwrap_class_static_method: bool = True,
 ) -> Any:
     """
-    Decorate model methods for validation purposes.
+    Recursively unwraps a wrapped function until the underlying function is reached.
+    This handles functools.partial, functools.partialmethod, staticmethod and classmethod.
 
     Args:
-        mode (Literal['wrap', 'before', 'after']): A required string literal that specifies the validation mode.
-            It can be one of the following: 'wrap', 'before', or 'after'.
+        func: The function to unwrap.
+        unwrap_class_static_method: If True (default), also unwrap classmethod and staticmethod
+            decorators. If False, only unwrap partial and partialmethod decorators.
 
     Returns:
-        Any: A decorator that can be used to decorate a function to be used as a model validator.
+        The underlying function of the wrapped function.
+    """
+    all: set[Any] = {partial, partialmethod, property}
+
+    try:
+        from functools import cached_property  # type: ignore
+    except ImportError:
+        cached_property = type('', (), {})  # type: ignore
+    else:
+        all.add(cached_property)
+
+    if unwrap_class_static_method:
+        all.update({staticmethod, classmethod})
+
+    while isinstance(func, tuple(all)):
+        if unwrap_class_static_method and isinstance(func, (classmethod, staticmethod)):
+            func = func.__func__
+        elif isinstance(func, (partial, partialmethod)):
+            func = func.func
+        elif isinstance(func, property):
+            func = func.fget  # arbitrary choice, convenient for computed fields
+        else:
+            # Make coverage happy as it can only get here in the last possible case
+            assert isinstance(func, cached_property)
+            func = func.func  # type: ignore
+
+    return func
+
+
+def get_function_return_type(func: Any, explicit_return_type: Any) -> Any:
+    if explicit_return_type is None:
+        # try to get it from the type annotation
+        func = unwrap_wrapped_function(func)
+        hints = get_function_type_hints(unwrap_wrapped_function(func), include_keys={'return'})
+        return hints.get('return', None)
+    else:
+        return explicit_return_type
+
+
+def count_positional_params(sig: Signature) -> int:
+    return sum(1 for param in sig.parameters.values() if can_be_positional(param))
+
+
+def can_be_positional(param: Parameter) -> bool:
+    return param.kind in (Parameter.POSITIONAL_ONLY, Parameter.POSITIONAL_OR_KEYWORD)
+
+
+def ensure_property(f: Any) -> Any:
     """
+    Ensure that a function is a `property` or `cached_property`, or is a valid descriptor.
+
+    Args:
+        f: The function to check.
 
-    def dec(f: Any) -> _decorators.PydanticDescriptorProxy[Any]:
-        # auto apply the @classmethod decorator
-        f = _decorators.ensure_classmethod_based_on_signature(f)
-        dec_info = _decorators.ModelValidatorDecoratorInfo(mode=mode)
-        return _decorators.PydanticDescriptorProxy(f, dec_info)
+    Returns:
+        The function, or a `property` or `cached_property` instance wrapping the function.
+    """
 
-    return dec
+    if ismethoddescriptor(f) or isdatadescriptor(f):
+        return f
+    else:
+        return property(f)
```

### Comparing `pydantic-2.0a4/pydantic/errors.py` & `pydantic-2.0b1/pydantic/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,43 @@
 """
 Pydantic errors.
 """
 from __future__ import annotations as _annotations
 
 import re
 
-from typing_extensions import Literal
+from typing_extensions import Literal, Self
 
 from ._migration import getattr_migration
 from .version import VERSION
 
 __all__ = (
     'PydanticUserError',
     'PydanticUndefinedAnnotation',
     'PydanticImportError',
     'PydanticSchemaGenerationError',
     'PydanticInvalidForJsonSchema',
 )
 
-# TODO set up a cloudflare worker to redirect to the correct page
 # We use this URL to allow for future flexibility about how we host the docs, while allowing for Pydantic
 # code in the while with "old" URLs to still work.
 # 'u' refers to "user errors" - e.g. errors caused by developers using pydantic, as opposed to validation errors.
 DEV_ERROR_DOCS_URL = f'https://errors.pydantic.dev/{VERSION}/u/'
 PydanticErrorCodes = Literal[
+    'class-not-fully-defined',
     'decorator-missing-field',
-    'dataclass-not-fully-defined',
     'discriminator-no-field',
     'discriminator-alias-type',
     'discriminator-needs-literal',
     'discriminator-alias',
     'typed-dict-version',
     'model-field-overridden',
     'model-field-missing-annotation',
-    'model-not-fully-defined',
     'config-both',
-    'deprecated_kwargs',
+    'deprecated-kwargs',
     'invalid-for-json-schema',
     'json-schema-already-used',
     'base-model-instantiated',
     'undefined-annotation',
     'schema-for-unknown-type',
     'import-error',
     'create-model-field-definitions',
@@ -47,18 +45,20 @@
     'validator-no-fields',
     'validator-invalid-fields',
     'validator-instance-method',
     'root-validator-pre-skip',
     'model-serializer-instance-method',
     'validator-field-config-info',
     'validator-v1-signature',
-    'field-validator-signature',
+    'validator-signature',
     'field-serializer-signature',
     'model-serializer-signature',
     'multiple-field-serializers',
+    'invalid_annotated_type',
+    'type-adapter-config-unused',
 ]
 
 
 class PydanticErrorMixin:
     """
     A mixin class for common functionality shared by all Pydantic-specific errors.
 
@@ -93,33 +93,38 @@
     """
 
     def __init__(self, name: str, message: str) -> None:
         self.name = name
         super().__init__(message=message, code='undefined-annotation')
 
     @classmethod
-    def from_name_error(cls, name_error: NameError) -> PydanticUndefinedAnnotation:
+    def from_name_error(cls, name_error: NameError) -> Self:
         """
         Convert a `NameError` to a `PydanticUndefinedAnnotation` error.
 
         Args:
-            name_error (NameError): `NameError` to be converted.
+            name_error: `NameError` to be converted.
 
         Returns:
-            PydanticUndefinedAnnotation: Converted `PydanticUndefinedAnnotation` error.
+            Converted `PydanticUndefinedAnnotation` error.
         """
         try:
             name = name_error.name  # type: ignore  # python > 3.10
         except AttributeError:
             name = re.search(r".*'(.+?)'", str(name_error)).group(1)  # type: ignore[union-attr]
         return cls(name=name, message=str(name_error))
 
 
 class PydanticImportError(PydanticErrorMixin, ImportError):
-    """Error occurs when an import fails due to module changes between V1 and V2."""
+    """
+    Error raised when an import fails due to module changes between V1 and V2.
+
+    Attributes:
+        message (str): Description of the error.
+    """
 
     def __init__(self, message: str) -> None:
         super().__init__(message, code='import-error')
 
 
 class PydanticSchemaGenerationError(PydanticUserError):
     """
```

### Comparing `pydantic-2.0a4/pydantic/fields.py` & `pydantic-2.0b1/pydantic/fields.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,175 +12,246 @@
 from typing import Any
 from warnings import warn
 
 import annotated_types
 import typing_extensions
 
 from . import types
-from ._internal import _decorators, _fields, _forward_ref, _internal_dataclass, _repr, _typing_extra, _utils
-from ._internal._fields import Undefined
-from ._internal._generics import replace_types
+from ._internal import _decorators, _fields, _generics, _internal_dataclass, _repr, _typing_extra, _utils
 from .errors import PydanticUserError
 
 if typing.TYPE_CHECKING:
-    from pydantic_core import core_schema as _core_schema
-
     from ._internal._repr import ReprArgs
 
+_Undefined = _fields.Undefined
 
-class FieldInfo(_repr.Representation):
+
+class _FromFieldInfoInputs(typing_extensions.TypedDict, total=False):
+    """
+    This class exists solely to add type checking for the `**kwargs` in `FieldInfo.from_field`.
+    """
+
+    annotation: type[Any] | None
+    default_factory: typing.Callable[[], Any] | None
+    alias: str | None
+    alias_priority: int | None
+    validation_alias: str | AliasPath | AliasChoices | None
+    serialization_alias: str | None
+    title: str | None
+    description: str | None
+    examples: list[Any] | None
+    exclude: bool | None
+    include: bool | None
+    gt: float | None
+    ge: float | None
+    lt: float | None
+    le: float | None
+    multiple_of: float | None
+    strict: bool | None
+    min_length: int | None
+    max_length: int | None
+    pattern: str | None
+    allow_inf_nan: bool | None
+    max_digits: int | None
+    decimal_places: int | None
+    discriminator: str | None
+    json_schema_extra: dict[str, Any] | None
+    frozen: bool | None
+    final: bool | None
+    validate_default: bool | None
+    repr: bool
+    init_var: bool | None
+    kw_only: bool | None
+
+
+class _FieldInfoInputs(_FromFieldInfoInputs, total=False):
+    """
+    This class exists solely to add type checking for the `**kwargs` in `FieldInfo.__init__`.
     """
-    Hold information about a field.
 
-    FieldInfo is used for any field definition whether or not the `Field()` function is explicitly used.
+    default: Any
 
-    Attributes:
-        annotation (type): The type annotation of the field.
-        default (Any): The default value of the field.
-        default_factory (callable): The factory function used to construct the default value of the field.
-        alias (str): The alias name of the field.
-        alias_priority (int): The priority of the field's alias.
-        validation_alias (str): The validation alias name of the field.
-        serialization_alias (str): The serialization alias name of the field.
-        title (str): The title of the field.
-        description (str): The description of the field.
-        examples (List[str]): List of examples of the field.
-        exclude (bool): Whether or not to exclude the field from the model schema.
-        include (bool): Whether or not to include the field in the model schema.
-        metadata (Dict[str, Any]): Dictionary of metadata constraints.
-        repr (bool): Whether or not to include the field in representation of the model.
-        discriminator (bool): Whether or not to include the field in the "discriminator" schema property of the model.
-        json_schema_extra (Dict[str, Any]): Dictionary of extra JSON schema properties.
-        init_var (bool): Whether or not the field should be included in the constructor of the model.
-        kw_only (bool): Whether or not the field should be a keyword-only argument in the constructor of the model.
-        validate_default (bool): Whether or not to validate the default value of the field.
-        frozen (bool): Whether or not the field is frozen.
-        final (bool): Whether or not the field is final.
+
+class FieldInfo(_repr.Representation):
     """
+    This class holds information about a field.
 
-    # TODO: Need to add attribute annotations
+    `FieldInfo` is used for any field definition regardless of whether the `Field()` function is explicitly used.
+
+    Attributes:
+        annotation: The type annotation of the field.
+        default: The default value of the field.
+        default_factory: The factory function used to construct the default for the field.
+        alias: The alias name of the field.
+        alias_priority: The priority of the field's alias.
+        validation_alias: The validation alias name of the field.
+        serialization_alias: The serialization alias name of the field.
+        title: The title of the field.
+        description: The description of the field.
+        examples: List of examples of the field.
+        exclude: Whether to exclude the field from the model schema.
+        include: Whether to include the field in the model schema.
+        discriminator: Field name for discriminating the type in a tagged union.
+        json_schema_extra: Dictionary of extra JSON schema properties.
+        frozen: Whether the field is frozen.
+        final: Whether the field is final.
+        validate_default: Whether to validate the default value of the field.
+        repr: Whether to include the field in representation of the model.
+        init_var: Whether the field should be included in the constructor of the dataclass.
+        kw_only: Whether the field should be a keyword-only argument in the constructor of the dataclass.
+        metadata: List of metadata constraints.
+    """
+
+    annotation: type[Any] | None
+    default: Any
+    default_factory: typing.Callable[[], Any] | None
+    alias: str | None
+    alias_priority: int | None
+    validation_alias: str | AliasPath | AliasChoices | None
+    serialization_alias: str | None
+    title: str | None
+    description: str | None
+    examples: list[Any] | None
+    exclude: bool | None
+    include: bool | None
+    discriminator: str | None
+    json_schema_extra: dict[str, Any] | None
+    frozen: bool | None
+    final: bool | None
+    validate_default: bool | None
+    repr: bool
+    init_var: bool | None
+    kw_only: bool | None
+    metadata: list[Any]
 
     __slots__ = (
         'annotation',
         'default',
         'default_factory',
         'alias',
         'alias_priority',
         'validation_alias',
         'serialization_alias',
         'title',
         'description',
         'examples',
         'exclude',
         'include',
-        'metadata',
-        'repr',
         'discriminator',
         'json_schema_extra',
-        'init_var',
-        'kw_only',
-        'validate_default',
         'frozen',
         'final',
+        'validate_default',
+        'repr',
+        'init_var',
+        'kw_only',
+        'metadata',
     )
 
     # used to convert kwargs to metadata/constraints,
     # None has a special meaning - these items are collected into a `PydanticGeneralMetadata`
-    metadata_lookup: dict[str, typing.Callable[[Any], Any] | None] = {
+    metadata_lookup: typing.ClassVar[dict[str, typing.Callable[[Any], Any] | None]] = {
+        'strict': types.Strict,
         'gt': annotated_types.Gt,
         'ge': annotated_types.Ge,
         'lt': annotated_types.Lt,
         'le': annotated_types.Le,
         'multiple_of': annotated_types.MultipleOf,
-        'strict': types.Strict,
         'min_length': annotated_types.MinLen,
         'max_length': annotated_types.MaxLen,
         'pattern': None,
         'allow_inf_nan': None,
         'max_digits': None,
         'decimal_places': None,
     }
 
-    def __init__(self, **kwargs: Any) -> None:
-        # TODO: This is a good place to add migration warnings; we should use overload for type-hinting the signature
+    def __init__(self, **kwargs: typing_extensions.Unpack[_FieldInfoInputs]) -> None:
+        """
+        This class should generally not be initialized directly; instead, use the `pydantic.fields.Field` function
+        or one of the constructor classmethods.
+
+        See the signature of `pydantic.fields.Field` for more details about the expected arguments.
+        """
         self.annotation, annotation_metadata = self._extract_metadata(kwargs.get('annotation'))
 
-        default = kwargs.pop('default', Undefined)
+        default = kwargs.pop('default', _Undefined)
         if default is Ellipsis:
-            self.default = Undefined
+            self.default = _Undefined
         else:
             self.default = default
 
-        self.default_factory = kwargs.get('default_factory')
+        self.default_factory = kwargs.pop('default_factory', None)
 
-        if self.default is not Undefined and self.default_factory is not None:
+        if self.default is not _Undefined and self.default_factory is not None:
             raise TypeError('cannot specify both default and default_factory')
 
-        self.alias = kwargs.get('alias')
-        self.alias_priority = kwargs.get('alias_priority') or 2 if self.alias is not None else None
-        self.title = kwargs.get('title')
-        self.validation_alias = kwargs.get('validation_alias', None)
-        self.serialization_alias = kwargs.get('serialization_alias', None)
-        self.description = kwargs.get('description')
-        self.examples = kwargs.get('examples')
-        self.exclude = kwargs.get('exclude')
-        self.include = kwargs.get('include')
-        self.metadata = self._collect_metadata(kwargs) + annotation_metadata
-        self.discriminator = kwargs.get('discriminator')
-        self.repr = kwargs.get('repr', True)
-        self.json_schema_extra = kwargs.get('json_schema_extra')
-        self.validate_default = kwargs.get('validate_default', None)
-        self.frozen = kwargs.get('frozen', None)
-        self.final = kwargs.get('final', None)
+        self.alias = kwargs.pop('alias', None)
+        self.alias_priority = kwargs.pop('alias_priority', None) or 2 if self.alias is not None else None
+        self.title = kwargs.pop('title', None)
+        self.validation_alias = kwargs.pop('validation_alias', None)
+        self.serialization_alias = kwargs.pop('serialization_alias', None)
+        self.description = kwargs.pop('description', None)
+        self.examples = kwargs.pop('examples', None)
+        self.exclude = kwargs.pop('exclude', None)
+        self.include = kwargs.pop('include', None)
+        self.discriminator = kwargs.pop('discriminator', None)
+        self.repr = kwargs.pop('repr', True)
+        self.json_schema_extra = kwargs.pop('json_schema_extra', None)
+        self.validate_default = kwargs.pop('validate_default', None)
+        self.frozen = kwargs.pop('frozen', None)
+        self.final = kwargs.pop('final', None)
         # currently only used on dataclasses
-        self.init_var = kwargs.get('init_var', None)
-        self.kw_only = kwargs.get('kw_only', None)
+        self.init_var = kwargs.pop('init_var', None)
+        self.kw_only = kwargs.pop('kw_only', None)
+
+        self.metadata = self._collect_metadata(kwargs) + annotation_metadata  # type: ignore
 
     @classmethod
-    def from_field(cls, default: Any = Undefined, **kwargs: Any) -> FieldInfo:
+    def from_field(
+        cls, default: Any = _Undefined, **kwargs: typing_extensions.Unpack[_FromFieldInfoInputs]
+    ) -> typing_extensions.Self:
         """
         Create a new `FieldInfo` object with the `Field` function.
 
         Args:
-            default (Any): The default value for the field. Defaults to Undefined.
+            default: The default value for the field. Defaults to Undefined.
             **kwargs: Additional arguments dictionary.
 
         Raises:
             TypeError: If 'annotation' is passed as a keyword argument.
 
         Returns:
-            FieldInfo: A new FieldInfo object with the given parameters.
+            A new FieldInfo object with the given parameters.
 
-        Examples:
+        Example:
             This is how you can create a field with default value like this:
 
             ```python
             import pydantic
 
             class MyModel(pydantic.BaseModel):
                 foo: int = pydantic.Field(4, ...)
             ```
         """
-        # TODO: This is a good place to add migration warnings; should we use overload for type-hinting the signature?
         if 'annotation' in kwargs:
             raise TypeError('"annotation" is not permitted as a Field keyword argument')
         return cls(default=default, **kwargs)
 
     @classmethod
-    def from_annotation(cls, annotation: type[Any] | _forward_ref.PydanticForwardRef) -> FieldInfo:
+    def from_annotation(cls, annotation: type[Any]) -> typing_extensions.Self:
         """
         Creates a `FieldInfo` instance from a bare annotation.
 
         Args:
-            annotation (Union[type[Any], _forward_ref.PydanticForwardRef]): An annotation object.
+            annotation: An annotation object.
 
         Returns:
-            FieldInfo: An instance of the field metadata.
+            An instance of the field metadata.
 
-        Examples:
+        Example:
             This is how you can create a field from a bare annotation like this:
 
             ```python
             import pydantic
             class MyModel(pydantic.BaseModel):
                 foo: int  # <-- like this
             ```
@@ -214,34 +285,34 @@
                 new_field_info.final = final
                 new_field_info.metadata += [a for a in extra_args if not isinstance(a, FieldInfo)]
                 return new_field_info
 
         return cls(annotation=annotation, final=final)
 
     @classmethod
-    def from_annotated_attribute(cls, annotation: type[Any], default: Any) -> FieldInfo:
+    def from_annotated_attribute(cls, annotation: type[Any], default: Any) -> typing_extensions.Self:
         """
         Create `FieldInfo` from an annotation with a default value.
 
         Args:
-            annotation (type[Any]): The type annotation of the field.
-            default (Any): The default value of the field.
+            annotation: The type annotation of the field.
+            default: The default value of the field.
 
         Returns:
-            FieldInfo: A field object with the passed values.
+            A field object with the passed values.
 
-        Examples:
-        ```python
-        import pydantic, annotated_types, typing
+        Example:
+            ```python
+            import pydantic, annotated_types, typing
 
-        class MyModel(pydantic.BaseModel):
-            foo: int = 4  # <-- like this
-            bar: typing.Annotated[int, annotated_types.Gt(4)] = 4  # <-- or this
-            spam: typing.Annotated[int, pydantic.Field(gt=4)] = 4  # <-- or this
-        ```
+            class MyModel(pydantic.BaseModel):
+                foo: int = 4  # <-- like this
+                bar: typing.Annotated[int, annotated_types.Gt(4)] = 4  # <-- or this
+                spam: typing.Annotated[int, pydantic.Field(gt=4)] = 4  # <-- or this
+            ```
         """
         final = False
         if _typing_extra.is_finalvar(annotation):
             final = True
             if annotation is not typing_extensions.Final:
                 annotation = typing_extensions.get_args(annotation)[0]
 
@@ -280,30 +351,30 @@
                     new_field_info.annotation = first_arg
                     new_field_info.metadata += [a for a in extra_args if not isinstance(a, FieldInfo)]
                     return new_field_info
 
             return cls(annotation=annotation, default=default, final=final)
 
     @classmethod
-    def _from_dataclass_field(cls, dc_field: DataclassField[Any]) -> FieldInfo:
+    def _from_dataclass_field(cls, dc_field: DataclassField[Any]) -> typing_extensions.Self:
         """
         Return a new `FieldInfo` instance from a `dataclasses.Field` instance.
 
         Args:
-            dc_field (dataclasses.Field): The `dataclasses.Field` instance to convert.
+            dc_field: The `dataclasses.Field` instance to convert.
 
         Returns:
-            FieldInfo: The corresponding `FieldInfo` instance.
+            The corresponding `FieldInfo` instance.
 
         Raises:
             TypeError: If any of the `FieldInfo` kwargs does not match the `dataclass.Field` kwargs.
         """
         default = dc_field.default
         if default is dataclasses.MISSING:
-            default = Undefined
+            default = _Undefined
 
         if dc_field.default_factory is dataclasses.MISSING:
             default_factory: typing.Callable[[], Any] | None = None
         else:
             default_factory = dc_field.default_factory
 
         # use the `Field` function so in correct kwargs raise the correct `TypeError`
@@ -314,19 +385,18 @@
         return field
 
     @classmethod
     def _extract_metadata(cls, annotation: type[Any] | None) -> tuple[type[Any] | None, list[Any]]:
         """Tries to extract metadata/constraints from an annotation if it uses `Annotated`.
 
         Args:
-            annotation (type[Any] | None): The type hint annotation for which metadata has to be extracted.
+            annotation: The type hint annotation for which metadata has to be extracted.
 
         Returns:
-            tuple[type[Any] | None, list[Any]]: A tuple containing the extracted metadata type and the list
-            of extra arguments.
+            A tuple containing the extracted metadata type and the list of extra arguments.
 
         Raises:
             TypeError: If a `Field` is used twice on the same field.
         """
         if annotation is not None:
             if _typing_extra.is_annotated(annotation):
                 first_arg, *extra_args = typing_extensions.get_args(annotation)
@@ -338,34 +408,34 @@
 
     @staticmethod
     def _find_field_info_arg(args: Any) -> FieldInfo | None:
         """
         Find an instance of `FieldInfo` in the provided arguments.
 
         Args:
-            args (Any): The argument list to search for `FieldInfo`.
+            args: The argument list to search for `FieldInfo`.
 
         Returns:
-            FieldInfo | None: An instance of `FieldInfo` if found, otherwise `None`.
+            An instance of `FieldInfo` if found, otherwise `None`.
         """
         return next((a for a in args if isinstance(a, FieldInfo)), None)
 
     @classmethod
     def _collect_metadata(cls, kwargs: dict[str, Any]) -> list[Any]:
         """
         Collect annotations from kwargs.
 
         The return type is actually `annotated_types.BaseMetadata | PydanticMetadata`,
         but it gets combined with `list[Any]` from `Annotated[T, ...]`, hence types.
 
         Args:
-            kwargs (dict[str, Any]): Keyword arguments passed to the function.
+            kwargs: Keyword arguments passed to the function.
 
         Returns:
-            list[Any]: A list of metadata objects - a combination of `annotated_types.BaseMetadata` and
+            A list of metadata objects - a combination of `annotated_types.BaseMetadata` and
                 `PydanticMetadata`.
         """
         metadata: list[Any] = []
         general_metadata = {}
         for key, value in list(kwargs.items()):
             try:
                 marker = cls.metadata_lookup[key]
@@ -387,53 +457,67 @@
         Get the default value.
 
         We expose an option for whether to call the default_factory (if present), as calling it may
         result in side effects that we want to avoid. However, there are times when it really should
         be called (namely, when instantiating a model via `model_construct`).
 
         Args:
-            call_default_factory (bool, optional): Whether to call the default_factory or not. Defaults to False.
+            call_default_factory: Whether to call the default_factory or not. Defaults to `False`.
 
         Returns:
-            Any: The default value, calling the default factory if requested or `None` if not set.
+            The default value, calling the default factory if requested or `None` if not set.
         """
         if self.default_factory is None:
             return _utils.smart_deepcopy(self.default)
         elif call_default_factory:
             return self.default_factory()
         else:
             return None
 
     def is_required(self) -> bool:
         """Check if the argument is required.
 
         Returns:
-            bool: `True` if the argument is required, `False` otherwise.
+            `True` if the argument is required, `False` otherwise.
         """
-        return self.default is Undefined and self.default_factory is None
+        return self.default is _Undefined and self.default_factory is None
 
     def rebuild_annotation(self) -> Any:
         """
-        Rebuild the original annotation for use in signatures.
+        Rebuilds the original annotation for use in function signatures.
+
+        If metadata is present, it adds it to the original annotation using an
+        `AnnotatedAlias`. Otherwise, it returns the original annotation as is.
+
+        Returns:
+            The rebuilt annotation.
         """
         if not self.metadata:
             return self.annotation
         else:
             return typing_extensions._AnnotatedAlias(self.annotation, self.metadata)
 
     def apply_typevars_map(self, typevars_map: dict[Any, Any] | None, types_namespace: dict[str, Any] | None) -> None:
         """
-        Apply a typevars_map to the annotation.
+        Apply a `typevars_map` to the annotation.
+
+        This method is used when analyzing parametrized generic types to replace typevars with their concrete types.
 
-        This is used when analyzing parametrized generic types to replace typevars with their concrete types.
+        This method applies the `typevars_map` to the annotation in place.
 
-        See pydantic._internal._generics.replace_types for more details.
+        Args:
+            typevars_map: A dictionary mapping type variables to their concrete types.
+            types_namespace (dict | None): A dictionary containing related types to the annotated type.
+
+        See Also:
+            pydantic._internal._generics.replace_types is used for replacing the typevars with
+                their concrete types.
         """
         annotation = _typing_extra.eval_type_lenient(self.annotation, types_namespace, None)
-        self.annotation = replace_types(annotation, typevars_map)
+        self.annotation = _generics.replace_types(annotation, typevars_map)
 
     def __repr_args__(self) -> ReprArgs:
         yield 'annotation', _repr.PlainRepr(_repr.display_as_type(self.annotation))
         yield 'required', self.is_required()
 
         for s in self.__slots__:
             if s == 'annotation':
@@ -450,326 +534,390 @@
                 continue
             if s == 'serialization_alias' and self.serialization_alias == self.alias:
                 continue
             if s == 'default_factory' and self.default_factory is not None:
                 yield 'default_factory', _repr.PlainRepr(_repr.display_as_type(self.default_factory))
             else:
                 value = getattr(self, s)
-                if value is not None and value is not Undefined:
+                if value is not None and value is not _Undefined:
                     yield s, value
 
 
 @_internal_dataclass.slots_dataclass
 class AliasPath:
+    """
+    A data class used by `validation_alias` as a convenience to create aliases.
+
+    Attributes:
+        path: A list of string or integer aliases.
+    """
+
     path: list[int | str]
 
     def __init__(self, first_arg: str, *args: str | int) -> None:
         self.path = [first_arg] + list(args)
 
     def convert_to_aliases(self) -> list[str | int]:
+        """
+        Converts arguments to a list of string or integer aliases.
+
+        Returns:
+            The list of aliases.
+        """
         return self.path
 
 
 @_internal_dataclass.slots_dataclass
 class AliasChoices:
+    """
+    A data class used by `validation_alias` as a convenience to create aliases.
+
+    Attributes:
+        choices: A list containing a string or `AliasPath`.
+    """
+
     choices: list[str | AliasPath]
 
-    def __init__(self, *args: str | AliasPath) -> None:
-        self.choices = list(args)
+    def __init__(self, first_choice: str | AliasPath, *choices: str | AliasPath) -> None:
+        self.choices = [first_choice] + list(choices)
 
     def convert_to_aliases(self) -> list[list[str | int]]:
+        """
+        Converts arguments to a list of lists containing string or integer aliases.
+
+        Returns:
+            The list of aliases.
+        """
         aliases: list[list[str | int]] = []
         for c in self.choices:
             if isinstance(c, AliasPath):
                 aliases.append(c.convert_to_aliases())
             else:
                 aliases.append([c])
         return aliases
 
 
+class _EmptyKwargs(typing_extensions.TypedDict):
+    """
+    This class exists solely to ensure that type checking warns about passing `**extra` in `Field`.
+    """
+
+    pass
+
+
 def Field(  # noqa C901
-    default: Any = Undefined,
+    default: Any = _Undefined,
     *,
     default_factory: typing.Callable[[], Any] | None = None,
     alias: str | None = None,
     alias_priority: int | None = None,
     validation_alias: str | AliasPath | AliasChoices | None = None,
     serialization_alias: str | None = None,
     title: str | None = None,
     description: str | None = None,
     examples: list[Any] | None = None,
-    exclude: typing.AbstractSet[int | str] | typing.Mapping[int | str, Any] | Any = None,
-    include: typing.AbstractSet[int | str] | typing.Mapping[int | str, Any] | Any = None,
+    exclude: bool | None = None,
+    include: bool | None = None,
+    discriminator: str | None = None,
+    json_schema_extra: dict[str, Any] | None = None,
+    frozen: bool | None = None,
+    final: bool | None = None,
+    validate_default: bool | None = None,
+    repr: bool = True,
+    init_var: bool | None = None,
+    kw_only: bool | None = None,
+    pattern: str | None = None,
+    strict: bool | None = None,
     gt: float | None = None,
     ge: float | None = None,
     lt: float | None = None,
     le: float | None = None,
     multiple_of: float | None = None,
     allow_inf_nan: bool | None = None,
     max_digits: int | None = None,
     decimal_places: int | None = None,
-    min_items: int | None = None,
-    max_items: int | None = None,
     min_length: int | None = None,
     max_length: int | None = None,
-    frozen: bool = False,
-    pattern: str | None = None,
-    discriminator: str | None = None,
-    repr: bool = True,
-    strict: bool | None = None,
-    json_schema_extra: dict[str, Any] | None = None,
-    validate_default: bool | None = None,
-    const: bool | None = None,
-    unique_items: bool | None = None,
-    allow_mutation: bool = True,
-    regex: str | None = None,
-    **extra: Any,
+    **extra: typing_extensions.Unpack[_EmptyKwargs],
 ) -> Any:
     """
     Create a field for objects that can be configured.
 
     Used to provide extra information about a field, either for the model schema or complex validation. Some arguments
     apply only to number fields (`int`, `float`, `Decimal`) and some apply only to `str`.
 
     Args:
-        default (Any, optional): default value if the field is not set.
-        default_factory (callable, optional): A callable to generate the default value like :func:`~datetime.utcnow`.
-        alias (str, optional): an alternative name for the attribute.
-        alias_priority (int, optional): priority of the alias. This defines which alias should be used in serialization.
-        validation_alias (str, list of str, list of list of str, optional): 'whitelist' validation step. The field
-            will be the single one allowed by the alias or set of aliases defined.
-        serialization_alias (str, optional): 'blacklist' validation step. The vanilla field will be the single one of
-            the alias' or set of aliases' fields and all the other fields will be ignored at serialization time.
-        title (str, optional): human-readable title.
-        description (str, optional): human-readable description.
-        examples (list[Any], optional): An example value for this field.
-        exclude (Union[AbstractSet[Union[str, int]], Mapping[Union[str, int], Any], Any]):
-            Parameters that should be excluded from the field. If `None`, default
-            Pydantic behaviors are used.
-        include (Union[AbstractSet[Union[str, int]], Mapping[Union[str, int], Any], Any]):
-            Parameters that should be included in the field. If `None`, default
-            Pydantic behaviors are used.
-        gt (float, optional): Greater than. If set, value must be greater than this. Only applicable to numbers.
-        ge (float, optional): Greater than or equal. If set, value must be
-            greater than or equal to this. Only applicable to numbers.
-        lt (float, optional): Less than. If set, value must be
-            less than this. Only applicable to numbers.
-        le (float, optional): Less than or equal. If set, value must be
-            less than or equal to this. Only applicable to numbers.
-        multiple_of (float, optional): Value must be a multiple of this. Only applicable to numbers.
-        allow_inf_nan (bool, optional): Allow `inf`, `-inf`, `nan`. Only applicable to numbers.
-        max_digits (int, optional): Maximum number of allow digits for strings.
-        decimal_places (int, optional): Maximum number decimal places allowed for numbers.
-        min_items (int, optional): Minimum number of items in a collection.
-        max_items (int, optional): Maximum number of items in a collection.
-        min_length (int, optional): Minimum length for strings.
-        max_length (int, optional): Maximum length for strings.
-        frozen (bool, optional): Store the value as a frozen object if is mutable.
-        pattern (str, optional): Pattern for strings.
-        discriminator (str, optional): Codename for discriminating a field among others of the same type.
-        repr (bool, optional): If `True` (the default), return a string representation of the field.
-        strict (bool, optional): If `True` (the default is `None`), the field should be validated strictly.
-        json_schema_extra (dict[str, Any]): Any other additional JSON schema data for the schema property.
-        validate_default (bool, optional): Run validation that isn't only checking existence of defaults. This is
-            `True` by default.
-        const (bool, optional): Value is always the same literal object. This is typically a singleton object,
-            such as `True` or `None`.
-        unique_items (bool, optional): Require that collection items be unique.
-        allow_mutation (bool, optional): If `False`, the dataclass will be frozen (made immutable).
-        regex (str, optional): Regular expression pattern that the field must match against.
-
+        default: Default value if the field is not set.
+        default_factory: A callable to generate the default value, such as :func:`~datetime.utcnow`.
+        alias: An alternative name for the attribute.
+        alias_priority: Priority of the alias. This affects whether an alias generator is used.
+        validation_alias: 'Whitelist' validation step. The field will be the single one allowed by the alias or set of
+            aliases defined.
+        serialization_alias: 'Blacklist' validation step. The vanilla field will be the single one of the alias' or set
+            of aliases' fields and all the other fields will be ignored at serialization time.
+        title: Human-readable title.
+        description: Human-readable description.
+        examples: Example values for this field.
+        exclude: Whether to exclude the field from the model schema.
+        include: Whether to include the field in the model schema.
+        discriminator: Field name for discriminating the type in a tagged union.
+        json_schema_extra: Any additional JSON schema data for the schema property.
+        frozen: Whether the field is frozen.
+        final: Whether the field is final.
+        validate_default: Run validation that isn't only checking existence of defaults. `True` by default.
+        repr: If `True` (the default), return a string representation of the field.
+        init_var: Whether the field should be included in the constructor of the dataclass.
+        kw_only: Whether the field should be a keyword-only argument in the constructor of the dataclass.
+        strict: If `True` (the default is `None`), the field should be validated strictly.
+        gt: Greater than. If set, value must be greater than this. Only applicable to numbers.
+        ge: Greater than or equal. If set, value must be greater than or equal to this. Only applicable to numbers.
+        lt: Less than. If set, value must be less than this. Only applicable to numbers.
+        le: Less than or equal. If set, value must be less than or equal to this. Only applicable to numbers.
+        multiple_of: Value must be a multiple of this. Only applicable to numbers.
+        min_length: Minimum length for strings.
+        max_length: Maximum length for strings.
+        pattern: Pattern for strings.
+        allow_inf_nan: Allow `inf`, `-inf`, `nan`. Only applicable to numbers.
+        max_digits: Maximum number of allow digits for strings.
+        decimal_places: Maximum number of decimal places allowed for numbers.
 
     Returns:
-        Any: return the generated field object.
+        The generated `FieldInfo` object
     """
-    # Check deprecated & removed params of V1.
-    # This has to be removed deprecation period over.
-    if const:
-        raise PydanticUserError('`const` is removed. use `Literal` instead', code='deprecated_kwargs')
-    if min_items:
-        warn('`min_items` is deprecated and will be removed. use `min_length` instead', DeprecationWarning)
+    # Check deprecated and removed params from V1. This logic should eventually be removed.
+    const = extra.pop('const', None)  # type: ignore
+    if const is not None:
+        raise PydanticUserError('`const` is removed, use `Literal` instead', code='deprecated-kwargs')
+
+    min_items = extra.pop('min_items', None)  # type: ignore
+    if min_items is not None:
+        warn('`min_items` is deprecated and will be removed, use `min_length` instead', DeprecationWarning)
         if min_length is None:
-            min_length = min_items
-    if max_items:
-        warn('`max_items` is deprecated and will be removed. use `max_length` instead', DeprecationWarning)
+            min_length = min_items  # type: ignore
+
+    max_items = extra.pop('max_items', None)  # type: ignore
+    if max_items is not None:
+        warn('`max_items` is deprecated and will be removed, use `max_length` instead', DeprecationWarning)
         if max_length is None:
-            max_length = max_items
+            max_length = max_items  # type: ignore
+
+    unique_items = extra.pop('unique_items', None)  # type: ignore
     if unique_items is not None:
         raise PydanticUserError(
             (
                 '`unique_items` is removed, use `Set` instead'
                 '(this feature is discussed in https://github.com/pydantic/pydantic-core/issues/296)'
             ),
-            code='deprecated_kwargs',
+            code='deprecated-kwargs',
         )
-    if allow_mutation is False:
+
+    allow_mutation = extra.pop('allow_mutation', None)  # type: ignore
+    if allow_mutation is not None:
         warn('`allow_mutation` is deprecated and will be removed. use `frozen` instead', DeprecationWarning)
-        frozen = True
-    if regex:
-        raise PydanticUserError('`regex` is removed. use `Pattern` instead', code='deprecated_kwargs')
+        if allow_mutation is False:
+            frozen = True
+
+    regex = extra.pop('regex', None)  # type: ignore
+    if regex is not None:
+        raise PydanticUserError('`regex` is removed. use `pattern` instead', code='deprecated-kwargs')
+
     if extra:
         warn(
             'Extra keyword arguments on `Field` is deprecated and will be removed. use `json_schema_extra` instead',
             DeprecationWarning,
         )
         if not json_schema_extra:
-            json_schema_extra = extra
+            json_schema_extra = extra  # type: ignore
 
-    converted_validation_alias: str | list[str | int] | list[list[str | int]] | None = None
     if validation_alias:
         if not isinstance(validation_alias, (str, AliasChoices, AliasPath)):
             raise TypeError('Invalid `validation_alias` type. it should be `str`, `AliasChoices`, or `AliasPath`')
 
-        if isinstance(validation_alias, (AliasChoices, AliasPath)):
-            converted_validation_alias = validation_alias.convert_to_aliases()
-        else:
-            converted_validation_alias = validation_alias
-
     if serialization_alias is None and isinstance(alias, str):
         serialization_alias = alias
 
     return FieldInfo.from_field(
         default,
         default_factory=default_factory,
         alias=alias,
         alias_priority=alias_priority,
-        validation_alias=converted_validation_alias or alias,
+        validation_alias=validation_alias or alias,
         serialization_alias=serialization_alias,
         title=title,
         description=description,
         examples=examples,
         exclude=exclude,
         include=include,
+        discriminator=discriminator,
+        json_schema_extra=json_schema_extra,
+        frozen=frozen,
+        final=final,
+        pattern=pattern,
+        validate_default=validate_default,
+        repr=repr,
+        init_var=init_var,
+        kw_only=kw_only,
+        strict=strict,
         gt=gt,
         ge=ge,
         lt=lt,
         le=le,
         multiple_of=multiple_of,
+        min_length=min_length,
+        max_length=max_length,
         allow_inf_nan=allow_inf_nan,
         max_digits=max_digits,
         decimal_places=decimal_places,
-        min_items=min_items,
-        max_items=max_items,
-        min_length=min_length,
-        max_length=max_length,
-        frozen=frozen,
-        pattern=pattern,
-        discriminator=discriminator,
-        repr=repr,
-        json_schema_extra=json_schema_extra,
-        strict=strict,
-        validate_default=validate_default,
     )
 
 
 class ModelPrivateAttr(_repr.Representation):
     """A descriptor for private attributes in class models.
 
     Attributes:
         default (Any): The default value of the attribute if not provided.
         default_factory (typing.Callable[[], Any]): A callable function that generates the default value of the
             attribute if not provided.
     """
 
     __slots__ = 'default', 'default_factory'
 
-    def __init__(self, default: Any = Undefined, *, default_factory: typing.Callable[[], Any] | None = None) -> None:
+    def __init__(self, default: Any = _Undefined, *, default_factory: typing.Callable[[], Any] | None = None) -> None:
         self.default = default
         self.default_factory = default_factory
 
+    def __getattr__(self, item: str) -> Any:
+        """
+        This function improves compatibility with custom descriptors by ensuring delegation happens
+        as expected when the default value of a private attribute is a descriptor.
+        """
+        if item in {'__get__', '__set__', '__delete__'}:
+            if hasattr(self.default, item):
+                return getattr(self.default, item)
+        raise AttributeError(f'{type(self).__name__!r} object has no attribute {item!r}')
+
     def __set_name__(self, cls: type[Any], name: str) -> None:
         """
-        preserve `__set_name__` protocol defined in https://peps.python.org/pep-0487
+        Preserve `__set_name__` protocol defined in https://peps.python.org/pep-0487.
         """
-        if self.default is not Undefined:
-            try:
-                set_name = getattr(self.default, '__set_name__')
-            except AttributeError:
-                pass
-            else:
-                if callable(set_name):
-                    set_name(cls, name)
+        if self.default is _Undefined:
+            return
+        if not hasattr(self.default, '__set_name__'):
+            return
+        set_name = self.default.__set_name__
+        if callable(set_name):
+            set_name(cls, name)
 
     def get_default(self) -> Any:
         """Returns the default value for the object.
 
         If `self.default_factory` is `None`, the method will return a deep copy of the `self.default` object.
+
         If `self.default_factory` is not `None`, it will call `self.default_factory` and return the value returned.
 
         Returns:
-            Any: The default value of the object.
+            The default value of the object.
         """
         return _utils.smart_deepcopy(self.default) if self.default_factory is None else self.default_factory()
 
     def __eq__(self, other: Any) -> bool:
         return isinstance(other, self.__class__) and (self.default, self.default_factory) == (
             other.default,
             other.default_factory,
         )
 
 
 def PrivateAttr(
-    default: Any = Undefined,
+    default: Any = _Undefined,
     *,
     default_factory: typing.Callable[[], Any] | None = None,
 ) -> Any:
     """
     Indicates that attribute is only used internally and never mixed with regular fields.
 
     Private attributes are not checked by Pydantic, so it's up to you to maintain their accuracy.
 
     Private attributes are stored in the model `__slots__`.
 
     Args:
-        default (Any): The attribute's default value. Defaults to Undefined.
-        default_factory (typing.Callable[[], Any], optional): Callable that will be
+        default: The attribute's default value. Defaults to Undefined.
+        default_factory: Callable that will be
             called when a default value is needed for this attribute.
             If both `default` and `default_factory` are set, an error will be raised.
 
     Returns:
-        Any: An instance of `ModelPrivateAttr` class.
+        An instance of `ModelPrivateAttr` class.
 
     Raises:
         ValueError: If both `default` and `default_factory` are set.
     """
-    if default is not Undefined and default_factory is not None:
+    if default is not _Undefined and default_factory is not None:
         raise TypeError('cannot specify both default and default_factory')
 
     return ModelPrivateAttr(
         default,
         default_factory=default_factory,
     )
 
 
 @_internal_dataclass.slots_dataclass
 class ComputedFieldInfo:
     """
-    A container for data from `@computed_field` so that we can access it
-    while building the pydantic-core schema.
+    A container for data from `@computed_field` so that we can access it while building the pydantic-core schema.
+
+    Attributes:
+        decorator_repr: A class variable representing the decorator string, '@computed_field'.
+        wrapped_property: The wrapped computed field property.
+        return_type: The type of the computed field property's return value.
+        alias: The alias of the property to be used during encoding and decoding.
+        alias_priority: priority of the alias. This affects whether an alias generator is used
+        title: Title of the computed field as in OpenAPI document, should be a short summary.
+        description: Description of the computed field as in OpenAPI document.
+        repr: A boolean indicating whether or not to include the field in the __repr__ output.
     """
 
     decorator_repr: typing.ClassVar[str] = '@computed_field'
     wrapped_property: property
-    json_return_type: _core_schema.JsonReturnTypes | None
+    return_type: type[Any]
     alias: str | None
+    alias_priority: int | None
     title: str | None
     description: str | None
     repr: bool
 
 
 # this should really be `property[T], cached_proprety[T]` but property is not generic unlike cached_property
 # See https://github.com/python/typing/issues/985 and linked issues
 PropertyT = typing.TypeVar('PropertyT')
+"""
+`TypeVar` that can be used to specify the type of a property.
+
+This can be used in combination with the `@property` decorator to specify the type
+of the property.
+
+Example:
+    ```py
+    class MyClass:
+        @property
+        def my_property(self) -> PropertyT:
+            return self._my_property
+
+        @my_property.setter
+        def my_property(self, value: PropertyT) -> None:
+            self._my_property = value
+    ```
+"""
 
 
 @typing.overload
 def computed_field(
     *,
-    json_return_type: _core_schema.JsonReturnTypes | None = None,
+    return_type: Any = None,
     alias: str | None = None,
+    alias_priority: int | None = None,
     title: str | None = None,
     description: str | None = None,
     repr: bool = True,
 ) -> typing.Callable[[PropertyT], PropertyT]:
     ...
 
 
@@ -778,46 +926,59 @@
     ...
 
 
 def computed_field(
     __f: PropertyT | None = None,
     *,
     alias: str | None = None,
+    alias_priority: int | None = None,
     title: str | None = None,
     description: str | None = None,
     repr: bool = True,
-    json_return_type: _core_schema.JsonReturnTypes | None = None,
+    return_type: Any = None,
 ) -> PropertyT | typing.Callable[[PropertyT], PropertyT]:
     """
     Decorate to include `property` and `cached_property` when serialising models.
 
     If applied to functions not yet decorated with `@property` or `@cached_property`, the function is
     automatically wrapped with `property`.
 
     Args:
         __f: the function to wrap.
         alias: alias to use when serializing this computed field, only used when `by_alias=True`
+        alias_priority: priority of the alias. This affects whether an alias generator is used
         title: Title to used when including this computed field in JSON Schema, currently unused waiting for #4697
         description: Description to used when including this computed field in JSON Schema, defaults to the functions
             docstring, currently unused waiting for #4697
         repr: whether to include this computed field in model repr
-        json_return_type: optional return for serialization logic to expect when serialising to JSON, if included
-            this must be correct, otherwise a `TypeError` is raised
+        return_type: optional return for serialization logic to expect when serialising to JSON, if included
+            this must be correct, otherwise a `TypeError` is raised.
+            If you don't include a return type Any is used, which does runtime introspection to handle arbitrary
+            objects.
 
     Returns:
         A proxy wrapper for the property.
     """
 
     def dec(f: Any) -> Any:
-        nonlocal description
+        nonlocal description, return_type, alias_priority
         if description is None and f.__doc__:
             description = inspect.cleandoc(f.__doc__)
 
+        return_type = _decorators.get_function_return_type(f, return_type)
+        if return_type is None:
+            raise PydanticUserError(
+                'Computed field is missing return type annotation or specifying `return_type`'
+                ' to the `@computed_field` decorator (e.g. `@computed_field(return_type=int|str)`)',
+                code='model-field-missing-annotation',
+            )
+
         # if the function isn't already decorated with `@property` (or another descriptor), then we wrap it now
         f = _decorators.ensure_property(f)
-        dec_info = ComputedFieldInfo(f, json_return_type, alias, title, description, repr)
+        alias_priority = (alias_priority or 2) if alias is not None else None
+        dec_info = ComputedFieldInfo(f, return_type, alias, alias_priority, title, description, repr)
         return _decorators.PydanticDescriptorProxy(f, dec_info)
 
     if __f is None:
         return dec
     else:
         return dec(__f)
```

### Comparing `pydantic-2.0a4/pydantic/json_schema.py` & `pydantic-2.0b1/pydantic/json_schema.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,127 +1,102 @@
 from __future__ import annotations as _annotations
 
 import inspect
 import math
 import re
-import sys
 import warnings
 from dataclasses import is_dataclass
 from enum import Enum
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Counter,
     Dict,
+    Hashable,
     Iterable,
     List,
     NewType,
     Sequence,
     Tuple,
-    Type,
+    TypeVar,
     Union,
     cast,
 )
-from weakref import WeakKeyDictionary
 
 import pydantic_core
-from typing_extensions import Literal
-
-from pydantic._internal._schema_generation_shared import GenerateJsonSchemaHandler
+from pydantic_core import CoreSchema, PydanticOmit, core_schema
+from pydantic_core.core_schema import ComputedField
+from typing_extensions import Literal, assert_never
 
 from ._internal import _core_metadata, _core_utils, _schema_generation_shared, _typing_extra
-from ._internal._core_utils import CoreSchemaOrField, is_core_schema, is_core_schema_field
 from .config import JsonSchemaExtraCallable
 from .errors import PydanticInvalidForJsonSchema, PydanticUserError
 
 if TYPE_CHECKING:
-    from pydantic_core import CoreSchema, core_schema
-
     from . import ConfigDict
+    from ._internal._core_utils import CoreSchemaField, CoreSchemaOrField
     from ._internal._dataclasses import PydanticDataclass
     from .main import BaseModel
 
-CoreSchemaOrFieldType = Literal[
-    'any',
-    'none',
-    'bool',
-    'int',
-    'float',
-    'str',
-    'bytes',
-    'date',
-    'time',
-    'datetime',
-    'timedelta',
-    'literal',
-    'is-instance',
-    'is-subclass',
-    'callable',
-    'list',
-    'tuple-positional',
-    'tuple-variable',
-    'set',
-    'frozenset',
-    'generator',
-    'dict',
-    'function-after',
-    'function-before',
-    'function-wrap',
-    'function-plain',
-    'default',
-    'nullable',
-    'union',
-    'tagged-union',
-    'chain',
-    'lax-or-strict',
-    'typed-dict',
-    'model-fields',
-    'model',
-    'dataclass-args',
-    'dataclass',
-    'arguments',
-    'call',
-    'custom-error',
-    'json',
-    'url',
-    'multi-host-url',
-    'definitions',
-    'definition-ref',
-    'model-field',
-    'dataclass-field',
-    'typed-dict-field',
-]
-
-
-JsonSchemaValue = _schema_generation_shared.JsonSchemaValue
-# re export GetJsonSchemaHandler
-GetJsonSchemaHandler = _schema_generation_shared.GetJsonSchemaHandler
+
+CoreSchemaOrFieldType = Literal[core_schema.CoreSchemaType, core_schema.CoreSchemaFieldType]
+"""
+A type alias for defined schema types that represents a union of `core_schema.CoreSchemaType` and
+`core_schema.CoreSchemaFieldType`.
+"""
+
+JsonSchemaValue = Dict[str, Any]
+"""
+A type alias for a JSON schema value. This is a dictionary of string keys to arbitrary values.
+"""
+
+JsonSchemaMode = Literal['validation', 'serialization']
+"""
+A type alias that represents the mode of a JSON schema; either 'validation' or 'serialization'.
+
+For some types, the inputs to validation differ from the outputs of serialization. For example,
+computed fields will only be present when serializing, and should not be provided when
+validating. This flag provides a way to indicate whether you want the JSON schema required
+for validation inputs, or that will be matched by serialization outputs.
+"""
+
+_MODE_TITLE_MAPPING: dict[JsonSchemaMode, str] = {'validation': 'Input', 'serialization': 'Output'}
 
 
 def update_json_schema(schema: JsonSchemaValue, updates: dict[str, Any]) -> JsonSchemaValue:
     """
-    A convenience function useful for creating `js_modify_function` functions that just set values for some keys.
+    Update a JSON schema by providing a dictionary of updates.
+
+    This function sets the provided key-value pairs in the schema and returns the updated schema.
+
+    Args:
+        schema (JsonSchemaValue): The JSON schema to update.
+        updates (dict[str, Any]): A dictionary of key-value pairs to set in the schema.
 
-    TODO: This is basically just a wrapper for dict.update that returns the dict.
-        Would it be better to just make this a less-"domain-specific" utility function?
+    Returns:
+        JsonSchemaValue: The updated JSON schema.
     """
     schema.update(updates)
     return schema
 
 
-# These are "kind" labels that can be used to control warnings. See `GenerateJsonSchema.render_warning_message`
 JsonSchemaWarningKind = Literal['skipped-choice', 'non-serializable-default']
+"""
+A type alias representing the kinds of warnings that can be emitted during JSON schema generation.
+
+See `GenerateJsonSchema.render_warning_message` for more details.
+"""
 
 
 class PydanticJsonSchemaWarning(UserWarning):
     """
     This class is used to emit warnings produced during JSON schema generation.
     See the `GenerateJsonSchema.emit_warning` and `GenerateJsonSchema.render_warning_message`
-    methods for more details; these can be overridden to control warning behavior
+    methods for more details; these can be overridden to control warning behavior.
     """
 
 
 # ##### JSON Schema Generation #####
 DEFAULT_REF_TEMPLATE = '#/$defs/{model}'
 
 # There are three types of references relevant to building JSON schemas:
@@ -132,83 +107,181 @@
 #       * by default, these look like "MyModel", though may change in the presence of collisions
 #       * eventually, we may want to make it easier to modify the way these names are generated
 DefsRef = NewType('DefsRef', str)
 #   3. the values corresponding to the "$ref" key in the schema
 #       * By default, these look like "#/$defs/MyModel", as in {"$ref": "#/$defs/MyModel"}
 JsonRef = NewType('JsonRef', str)
 
+CoreModeRef = Tuple[CoreRef, JsonSchemaMode]
+JsonSchemaKeyT = TypeVar('JsonSchemaKeyT', bound=Hashable)
+
 
 class GenerateJsonSchema:
-    # See https://json-schema.org/understanding-json-schema/reference/schema.html#id4 for more info about dialects
+    """
+    A class for generating JSON schemas.
+
+    This class generates JSON schemas based on configured parameters. The default schema dialect
+    is 'https://json-schema.org/draft/2020-12/schema'. The class uses `by_alias` to configure how fields with
+    multiple names are handled and `ref_template` to format reference names.
+
+    Attributes:
+        schema_dialect (str): The JSON schema dialect used to generate the schema. See
+            [Declaring a Dialect](https://json-schema.org/understanding-json-schema/reference/schema.html#id4)
+            in the JSON Schema documentation for more information about dialects.
+        ignored_warning_kinds (set): Warnings to ignore when generating the schema. `self.render_warning_message` will
+            do nothing if its argument `kind` is in `ignored_warning_kinds`;
+            this value can be modified on subclasses to easily control which warnings are emitted.
+        by_alias (bool): Whether or not to use field names when generating the schema.
+        ref_template (str): The format string used when generating reference names.
+        core_to_json_refs (dict): A mapping of core refs to JSON refs.
+        core_to_defs_refs (dict): A mapping of core refs to definition refs.
+        defs_to_core_refs (dict): A mapping of definition refs to core refs.
+        json_to_defs_refs (dict): A mapping of JSON refs to definition refs.
+        definitions (dict): Definitions in the schema.
+        collisions (set): Definitions with colliding names. When collisions are detected, we choose a non-colliding
+            name during generation, but we also track the colliding tag so that it can be remapped for the first
+            occurrence at the end of the process.
+        defs_ref_fallbacks (dict): Core refs to fallback definitions refs.
+        _schema_type_to_method (dict): A mapping of schema types to generator methods.
+        _used (bool): Set to `True` after generating a schema to avoid re-use issues.
+        mode (JsonSchemaMode): The schema mode.
+
+    Args:
+        by_alias (bool): Whether or not to include field names.
+        ref_template (str): The format string to use when generating reference names.
+
+    Raises:
+        JsonSchemaError: If the instance of the class is inadvertently re-used after generating a schema.
+    """
+
     schema_dialect = 'https://json-schema.org/draft/2020-12/schema'
 
     # `self.render_warning_message` will do nothing if its argument `kind` is in `ignored_warning_kinds`;
     # this value can be modified on subclasses to easily control which warnings are emitted
     ignored_warning_kinds: set[JsonSchemaWarningKind] = {'skipped-choice'}
 
     def __init__(self, by_alias: bool = True, ref_template: str = DEFAULT_REF_TEMPLATE):
         self.by_alias = by_alias
         self.ref_template = ref_template
 
-        self.core_to_json_refs: dict[CoreRef, JsonRef] = {}
-        self.core_to_defs_refs: dict[CoreRef, DefsRef] = {}
-        self.defs_to_core_refs: dict[DefsRef, CoreRef] = {}
+        self.core_to_json_refs: dict[CoreModeRef, JsonRef] = {}
+        self.core_to_defs_refs: dict[CoreModeRef, DefsRef] = {}
+        self.defs_to_core_refs: dict[DefsRef, CoreModeRef] = {}
         self.json_to_defs_refs: dict[JsonRef, DefsRef] = {}
 
         self.definitions: dict[DefsRef, JsonSchemaValue] = {}
 
         # When collisions are detected, we choose a non-colliding name
         # during generation, but we also track the colliding tag so that it
         # can be remapped for the first occurrence at the end of the process
         self.collisions: set[DefsRef] = set()
-        self.defs_ref_fallbacks: dict[CoreRef, list[DefsRef]] = {}
+        self.defs_ref_fallbacks: dict[CoreModeRef, list[DefsRef]] = {}
 
         self._schema_type_to_method = self.build_schema_type_to_method()
 
         # This changes to True after generating a schema, to prevent issues caused by accidental re-use
         # of a single instance of a schema generator
         self._used = False
 
+        self.mode: JsonSchemaMode = 'validation'
+
     def build_schema_type_to_method(
         self,
     ) -> dict[CoreSchemaOrFieldType, Callable[[CoreSchemaOrField], JsonSchemaValue]]:
+        """
+        Builds a dictionary mapping `CoreSchemaOrFieldType` to a callable method that generates a `JsonSchema` value
+        for a given `CoreSchemaOrField`.
+
+        Returns:
+            dict: A dictionary containing the mapping of `CoreSchemaOrFieldType` to a callable method.
+
+        Raises:
+            TypeError: If no method has been defined for generating a JSON schema for a given pydantic core schema type.
+        """
         mapping: dict[CoreSchemaOrFieldType, Callable[[CoreSchemaOrField], JsonSchemaValue]] = {}
         core_schema_types: list[CoreSchemaOrFieldType] = _typing_extra.all_literal_values(
             CoreSchemaOrFieldType  # type: ignore
         )
         for key in core_schema_types:
             method_name = f"{key.replace('-', '_')}_schema"
             try:
                 mapping[key] = getattr(self, method_name)
-            except AttributeError as e:
+            except AttributeError as e:  # pragma: no cover
                 raise TypeError(
                     f'No method for generating JsonSchema for core_schema.type={key!r} '
                     f'(expected: {type(self).__name__}.{method_name})'
                 ) from e
         return mapping
 
-    def generate_definitions(self, schemas: list[CoreSchema]) -> dict[DefsRef, JsonSchemaValue]:
-        """
-        Given a list of core_schema, generate all JSON schema definitions, and return the generated definitions.
+    def generate_definitions(
+        self, inputs: Sequence[tuple[JsonSchemaKeyT, JsonSchemaMode, core_schema.CoreSchema]]
+    ) -> tuple[dict[tuple[JsonSchemaKeyT, JsonSchemaMode], DefsRef], dict[DefsRef, JsonSchemaValue]]:
+        """
+        Given a list of core_schema, generates all JSON schema definitions from a list of core schemas, and
+        returns the generated definitions paired with a mapping from the input keys to the definition references.
+
+        Args:
+            inputs: A sequence of tuples, where:
+
+                - `JsonSchemaKeyT` will be paired with `JsonSchemaMode` to form the keys of the first returned
+                    dictionary.
+                - `JsonSchemaMode` is a JSON schema mode, either 'validation' or 'serialization'.
+                - `core_schema.CoreSchema` is a Pydantic `core_schema`.
+
+        Returns:
+            A 2-tuple, where:
+
+                - The first element is a dictionary whose keys are tuples of a JSON schema key type and mode, and
+                    whose values are `DefsRef`.
+                - The second element is a dictionary whose keys are `DefsRef` and whose values are `JsonSchemaValue`.
+
+        Raises:
+            PydanticUserError: Raised if the JSON schema generator has already been used to generate a JSON schema.
         """
         if self._used:
             raise PydanticUserError(
                 'This JSON schema generator has already been used to generate a JSON schema. '
                 f'You must create a new instance of {type(self).__name__} to generate a new JSON schema.',
                 code='json-schema-already-used',
             )
-        for schema in schemas:
+
+        for key, mode, schema in inputs:
+            self.mode = mode
             self.generate_inner(schema)
 
         self.resolve_collisions({})
 
+        refs_map: dict[tuple[JsonSchemaKeyT, JsonSchemaMode], DefsRef] = {}
+        for key, mode, schema in inputs:
+            self.mode = mode
+            json_schema = self.generate_inner(schema)
+            if '$ref' in json_schema:
+                json_ref = cast(JsonRef, json_schema['$ref'])
+                defs_ref = self.json_to_defs_refs.get(json_ref)
+                if defs_ref is not None:
+                    refs_map[(key, mode)] = defs_ref
+
         self._used = True
-        return self.definitions
+        return refs_map, self.definitions
 
-    def generate(self, schema: CoreSchema) -> JsonSchemaValue:
+    def generate(self, schema: CoreSchema, mode: JsonSchemaMode = 'validation') -> JsonSchemaValue:
+        """
+        Generates a JSON schema for a specified schema in a specified mode.
+
+        Args:
+            schema: A Pydantic model.
+            mode: The mode in which to generate the schema. Defaults to 'validation'.
+
+        Returns:
+            A JSON schema representing the specified schema.
+
+        Raises:
+            PydanticUserError: If the JSON schema generator has already been used to generate a JSON schema.
+        """
+        self.mode = mode
         if self._used:
             raise PydanticUserError(
                 'This JSON schema generator has already been used to generate a JSON schema. '
                 f'You must create a new instance of {type(self).__name__} to generate a new JSON schema.',
                 code='json-schema-already-used',
             )
 
@@ -243,167 +316,386 @@
         # For now, we will not set the $schema key. However, if desired, this can be easily added by overriding
         # this method and adding the following line after a call to super().generate(schema):
         # json_schema['$schema'] = self.schema_dialect
 
         self._used = True
         return json_schema
 
-    def generate_inner(self, schema: _core_metadata.CoreSchemaOrField) -> JsonSchemaValue:
+    def generate_inner(self, schema: CoreSchemaOrField) -> JsonSchemaValue:
+        """
+        Generates a JSON schema for a given `CoreSchemaOrField`.
+
+        Args:
+            schema: The given `CoreSchemaOrField` to generate JSON schema for.
+
+        Returns:
+            The generated JSON schema.
+        """
         # If a schema with the same CoreRef has been handled, just return a reference to it
         # Note that this assumes that it will _never_ be the case that the same CoreRef is used
         # on types that should have different JSON schemas
         if 'ref' in schema:
             core_ref = CoreRef(schema['ref'])  # type: ignore[typeddict-item]
-            if core_ref in self.core_to_defs_refs and self.core_to_defs_refs[core_ref] in self.definitions:
-                return {'$ref': self.core_to_json_refs[core_ref]}
+            core_mode_ref = (core_ref, self.mode)
+            if core_mode_ref in self.core_to_defs_refs and self.core_to_defs_refs[core_mode_ref] in self.definitions:
+                return {'$ref': self.core_to_json_refs[core_mode_ref]}
 
         # Generate the JSON schema, accounting for the json_schema_override and core_schema_override
         metadata_handler = _core_metadata.CoreMetadataHandler(schema)
 
-        def handler_func(schema_or_field: _core_metadata.CoreSchemaOrField) -> JsonSchemaValue:
+        def handler_func(schema_or_field: CoreSchemaOrField) -> JsonSchemaValue:
+            """
+            Generate a JSON schema based on the input schema.
+
+            Args:
+                schema_or_field: The schema data to generate a JSON schema from.
+
+            Returns:
+                The generated JSON schema.
+
+            Raises:
+                TypeError: If an unexpected schema type is encountered.
+            """
             # Generate the core-schema-type-specific bits of the schema generation:
-            if is_core_schema(schema_or_field) or is_core_schema_field(schema_or_field):
+            if _core_utils.is_core_schema(schema_or_field) or _core_utils.is_core_schema_field(schema_or_field):
                 generate_for_schema_type = self._schema_type_to_method[schema_or_field['type']]
                 json_schema = generate_for_schema_type(schema_or_field)
             else:
                 raise TypeError(f'Unexpected schema type: schema={schema_or_field}')
             # Populate the definitions
             if 'ref' in schema:
                 core_ref = CoreRef(schema['ref'])  # type: ignore[typeddict-item]
                 defs_ref, ref_json_schema = self.get_cache_defs_ref_schema(core_ref)
                 self.definitions[defs_ref] = json_schema
                 json_schema = ref_json_schema
             return json_schema
 
-        current_handler = GenerateJsonSchemaHandler(self, handler_func)
+        current_handler = _schema_generation_shared.GenerateJsonSchemaHandler(self, handler_func)
 
         for js_modify_function in metadata_handler.metadata.get('pydantic_js_functions', ()):
 
             def new_handler_func(
-                schema_or_field: _core_metadata.CoreSchemaOrField,
+                schema_or_field: CoreSchemaOrField,
                 current_handler: _core_metadata.GetJsonSchemaHandler = current_handler,
                 js_modify_function: _core_metadata.GetJsonSchemaFunction = js_modify_function,
             ) -> JsonSchemaValue:
                 return js_modify_function(schema_or_field, current_handler)
 
-            current_handler = GenerateJsonSchemaHandler(self, new_handler_func)
+            current_handler = _schema_generation_shared.GenerateJsonSchemaHandler(self, new_handler_func)
 
         return current_handler(schema)
 
     # ### Schema generation methods
     def any_schema(self, schema: core_schema.AnySchema) -> JsonSchemaValue:
+        """
+        Returns a schema that matches any value.
+
+        Args:
+            schema: The schema.
+
+        Returns:
+            The generated JSON schema.
+        """
         return {}
 
     def none_schema(self, schema: core_schema.NoneSchema) -> JsonSchemaValue:
+        """
+        Returns a schema that matches a `None` value.
+
+        Args:
+            schema: The schema.
+
+        Returns:
+            The generated JSON schema.
+        """
         return {'type': 'null'}
 
     def bool_schema(self, schema: core_schema.BoolSchema) -> JsonSchemaValue:
+        """
+        Returns a schema that matches a Boolean value.
+
+        Args:
+            schema: The schema.
+
+        Returns:
+            The generated JSON schema.
+        """
         return {'type': 'boolean'}
 
     def int_schema(self, schema: core_schema.IntSchema) -> JsonSchemaValue:
+        """
+        Returns a schema that matches an int value.
+
+        Args:
+            schema: The schema.
+
+        Returns:
+            The generated JSON schema.
+        """
         json_schema: dict[str, Any] = {'type': 'integer'}
         self.update_with_validations(json_schema, schema, self.ValidationsMapping.numeric)
         json_schema = {k: v for k, v in json_schema.items() if v not in {math.inf, -math.inf}}
         return json_schema
 
     def float_schema(self, schema: core_schema.FloatSchema) -> JsonSchemaValue:
+        """
+        Returns a schema that matches a Float value.
+
+        Args:
+            schema: The schema.
+
+        Returns:
+            The generated JSON schema.
+        """
         json_schema: dict[str, Any] = {'type': 'number'}
         self.update_with_validations(json_schema, schema, self.ValidationsMapping.numeric)
         json_schema = {k: v for k, v in json_schema.items() if v not in {math.inf, -math.inf}}
         return json_schema
 
     def str_schema(self, schema: core_schema.StringSchema) -> JsonSchemaValue:
+        """
+        Returns a schema that matches a string value.
+
+        Args:
+            schema: The schema.
+
+        Returns:
+            The generated JSON schema.
+        """
         json_schema = {'type': 'string'}
         self.update_with_validations(json_schema, schema, self.ValidationsMapping.string)
         return json_schema
 
     def bytes_schema(self, schema: core_schema.BytesSchema) -> JsonSchemaValue:
+        """
+        Returns a schema that matches a bytes value.
+
+        Args:
+            schema: The schema.
+
+        Returns:
+            The generated JSON schema.
+        """
         json_schema = {'type': 'string', 'format': 'binary'}
         self.update_with_validations(json_schema, schema, self.ValidationsMapping.bytes)
         return json_schema
 
     def date_schema(self, schema: core_schema.DateSchema) -> JsonSchemaValue:
+        """
+        Returns a schema that matches a date value.
+
+        Args:
+            schema: The schema.
+
+        Returns:
+            The generated JSON schema.
+        """
         json_schema = {'type': 'string', 'format': 'date'}
         self.update_with_validations(json_schema, schema, self.ValidationsMapping.date)
         return json_schema
 
     def time_schema(self, schema: core_schema.TimeSchema) -> JsonSchemaValue:
+        """
+        Returns a schema that matches a time value.
+
+        Args:
+            schema: The schema.
+
+        Returns:
+            The generated JSON schema.
+        """
         return {'type': 'string', 'format': 'time'}
 
     def datetime_schema(self, schema: core_schema.DatetimeSchema) -> JsonSchemaValue:
+        """
+        Returns a schema that matches a `datetime` value.
+
+        Args:
+            schema: The schema.
+
+        Returns:
+            The generated JSON schema.
+        """
         return {'type': 'string', 'format': 'date-time'}
 
     def timedelta_schema(self, schema: core_schema.TimedeltaSchema) -> JsonSchemaValue:
-        # It's weird that this schema has 'type': 'number' but also specifies a 'format'.
-        # Relevant issue: https://github.com/pydantic/pydantic/issues/5034
-        # TODO: Probably should just change this to str (look at readme intro for speeddate)
-        return {'type': 'number', 'format': 'time-delta'}
+        """
+        Returns a schema that matches a `timedelta` value.
+
+        Args:
+            schema: The schema.
+
+        Returns:
+            The generated JSON schema.
+        """
+        return {'type': 'string', 'format': 'duration'}
 
     def literal_schema(self, schema: core_schema.LiteralSchema) -> JsonSchemaValue:
+        """
+        Returns a schema that matches a `Literal` value.
+
+        Args:
+            schema: The schema.
+
+        Returns:
+            The generated JSON schema.
+        """
         expected = [v.value if isinstance(v, Enum) else v for v in schema['expected']]
 
         if len(expected) == 1:
             return {'const': expected[0]}
         else:
             return {'enum': expected}
 
     def is_instance_schema(self, schema: core_schema.IsInstanceSchema) -> JsonSchemaValue:
+        """
+        Returns a schema that checks if a value is an instance of a class, equivalent to Python's `isinstance` method.
+
+        Args:
+            schema: The schema.
+
+        Returns:
+            The generated JSON schema.
+        """
         return self.handle_invalid_for_json_schema(schema, f'core_schema.IsInstanceSchema ({schema["cls"]})')
 
     def is_subclass_schema(self, schema: core_schema.IsSubclassSchema) -> JsonSchemaValue:
-        return {}  # TODO: This was for compatibility with V1 -- is this the right thing to do?
+        """
+        Returns a schema that checks if a value is a subtype of a class, equivalent to Python's `issubclass` method.
+
+        Args:
+            schema: The schema.
+
+        Returns:
+            The generated JSON schema.
+        """
+        # Note: This is for compatibility with V1; you can override if you want different behavior.
+        return {}
 
     def callable_schema(self, schema: core_schema.CallableSchema) -> JsonSchemaValue:
+        """
+        Returns a schema that checks if a value is callable, equivalent to Python's `callable` method.
+
+        Args:
+            schema: The schema.
+
+        Returns:
+            The generated JSON schema.
+        """
         return self.handle_invalid_for_json_schema(schema, 'core_schema.CallableSchema')
 
     def list_schema(self, schema: core_schema.ListSchema) -> JsonSchemaValue:
+        """
+        Returns a schema that matches a `List` value.
+
+        Args:
+            schema: The schema.
+
+        Returns:
+            The generated JSON schema.
+        """
         items_schema = {} if 'items_schema' not in schema else self.generate_inner(schema['items_schema'])
         json_schema = {'type': 'array', 'items': items_schema}
         self.update_with_validations(json_schema, schema, self.ValidationsMapping.array)
         return json_schema
 
     def tuple_positional_schema(self, schema: core_schema.TuplePositionalSchema) -> JsonSchemaValue:
+        """
+        Returns a schema that matches a tuple of schemas.
+
+        Args:
+            schema: The schema.
+
+        Returns:
+            The generated JSON schema.
+        """
         json_schema: JsonSchemaValue = {'type': 'array'}
         json_schema['minItems'] = len(schema['items_schema'])
         prefixItems = [self.generate_inner(item) for item in schema['items_schema']]
         if prefixItems:
             json_schema['prefixItems'] = prefixItems
         if 'extra_schema' in schema:
             json_schema['items'] = self.generate_inner(schema['extra_schema'])
         else:
             json_schema['maxItems'] = len(schema['items_schema'])
         self.update_with_validations(json_schema, schema, self.ValidationsMapping.array)
         return json_schema
 
     def tuple_variable_schema(self, schema: core_schema.TupleVariableSchema) -> JsonSchemaValue:
-        json_schema: JsonSchemaValue = {'type': 'array', 'items': {}}
-        if 'items_schema' in schema:
-            json_schema['items'] = self.generate_inner(schema['items_schema'])
+        """
+        Returns a schema that matches a tuple of a given schema.
+
+        Args:
+            schema: The schema.
+
+        Returns:
+            JsonSchemaValue: The generated JSON schema.
+        """
+        # NOTE: The `items_schema` is always added, even when we explicitly create a
+        # tuple variable schema without an `items_schema`.
+        items = self.generate_inner(schema['items_schema'])  # type: ignore
+        json_schema: JsonSchemaValue = {'type': 'array', 'items': items}
         self.update_with_validations(json_schema, schema, self.ValidationsMapping.array)
         return json_schema
 
     def set_schema(self, schema: core_schema.SetSchema) -> JsonSchemaValue:
+        """
+        Returns a schema that matches a `Set` schema.
+
+        Args:
+            schema: The schema.
+
+        Returns:
+            The generated JSON schema.
+        """
         return self._common_set_schema(schema)
 
     def frozenset_schema(self, schema: core_schema.FrozenSetSchema) -> JsonSchemaValue:
+        """
+        Returns a schema that matches a `frozenset` schema.
+
+        Args:
+            schema: The schema.
+
+        Returns:
+            The generated JSON schema.
+        """
         return self._common_set_schema(schema)
 
     def _common_set_schema(self, schema: core_schema.SetSchema | core_schema.FrozenSetSchema) -> JsonSchemaValue:
         items_schema = {} if 'items_schema' not in schema else self.generate_inner(schema['items_schema'])
         json_schema = {'type': 'array', 'uniqueItems': True, 'items': items_schema}
         self.update_with_validations(json_schema, schema, self.ValidationsMapping.array)
         return json_schema
 
     def generator_schema(self, schema: core_schema.GeneratorSchema) -> JsonSchemaValue:
+        """
+        Returns a JSON schema that represents the provided GeneratorSchema.
+
+        Args:
+            schema: The schema.
+
+        Returns:
+            The generated JSON schema.
+        """
         items_schema = {} if 'items_schema' not in schema else self.generate_inner(schema['items_schema'])
         json_schema = {'type': 'array', 'items': items_schema}
         self.update_with_validations(json_schema, schema, self.ValidationsMapping.array)
         return json_schema
 
     def dict_schema(self, schema: core_schema.DictSchema) -> JsonSchemaValue:
+        """
+        Returns a schema that matches a dict schema.
+
+        Args:
+            schema: The schema.
+
+        Returns:
+            The generated JSON schema.
+        """
         json_schema: JsonSchemaValue = {'type': 'object'}
 
         keys_schema = self.generate_inner(schema['keys_schema']).copy() if 'keys_schema' in schema else {}
         keys_pattern = keys_schema.pop('pattern', None)
 
         values_schema = self.generate_inner(schema['values_schema']).copy() if 'values_schema' in schema else {}
         values_schema.pop('title', None)  # don't give a title to the additionalProperties
@@ -443,15 +735,15 @@
     def default_schema(self, schema: core_schema.WithDefaultSchema) -> JsonSchemaValue:
         json_schema = self.generate_inner(schema['schema'])
 
         if 'default' in schema:
             default = schema['default']
         elif 'default_factory' in schema:
             default = schema['default_factory']()
-        else:
+        else:  # pragma: no cover
             raise ValueError('`schema` has neither default nor default_factory')
 
         try:
             encoded_default = self.encode_default(default)
         except pydantic_core.PydanticSerializationError:
             self.emit_warning(
                 'non-serializable-default',
@@ -566,19 +858,16 @@
                         break
                 if alias_is_present_on_all_choices:
                     openapi_discriminator = alias
                     break
         return openapi_discriminator
 
     def chain_schema(self, schema: core_schema.ChainSchema) -> JsonSchemaValue:
-        try:
-            # Note: If we wanted to generate a schema for the _serialization_, would want to use the _last_ step:
-            return self.generate_inner(schema['steps'][0])
-        except IndexError as e:
-            raise ValueError('Cannot generate a JsonSchema for a zero-step ChainSchema') from e
+        # Note: If we wanted to generate a schema for the _serialization_, would want to use the _last_ step:
+        return self.generate_inner(schema['steps'][0])
 
     def lax_or_strict_schema(self, schema: core_schema.LaxOrStrictSchema) -> JsonSchemaValue:
         """
         LaxOrStrict will use the strict branch for serialization internally,
         unless it was overridden here.
         """
         # TODO: Need to read the default value off of model config or whatever
@@ -586,63 +875,97 @@
         # If your JSON schema fails to generate it is probably
         # because one of the following two branches failed.
         if use_strict:
             return self.generate_inner(schema['strict_schema'])
         else:
             return self.generate_inner(schema['lax_schema'])
 
+    def json_or_python_schema(self, schema: core_schema.JsonOrPythonSchema) -> JsonSchemaValue:
+        """
+        Always uses the json schema
+        """
+        return self.generate_inner(schema['json_schema'])
+
     def typed_dict_schema(self, schema: core_schema.TypedDictSchema) -> JsonSchemaValue:
-        named_required_fields = [
-            (k, v['required'], v) for k, v in schema['fields'].items()  # type: ignore  # required is always populated
+        named_required_fields: list[tuple[str, bool, CoreSchemaField]] = [
+            (name, self.field_is_required(field), field)
+            for name, field in schema['fields'].items()
+            if self.field_is_present(field)
         ]
+        if self.mode == 'serialization':
+            named_required_fields.extend(self._name_required_computed_fields(schema.get('computed_fields', [])))
         return self._named_required_fields_schema(named_required_fields)
 
+    @staticmethod
+    def _name_required_computed_fields(
+        computed_fields: list[ComputedField],
+    ) -> list[tuple[str, bool, core_schema.ComputedField]]:
+        return [(field['property_name'], True, field) for field in computed_fields]
+
     def _named_required_fields_schema(
-        self, named_required_fields: Sequence[tuple[str, bool, CoreSchemaOrField]]
+        self, named_required_fields: Sequence[tuple[str, bool, CoreSchemaField]]
     ) -> JsonSchemaValue:
         properties: dict[str, JsonSchemaValue] = {}
         required_fields: list[str] = []
         for name, required, field in named_required_fields:
             if self.by_alias:
-                alias: Any = field.get('validation_alias', name)
-                if isinstance(alias, str):
-                    name = alias
-                elif isinstance(alias, list):
-                    alias = cast('list[str] | str', alias)
-                    for path in alias:
-                        if isinstance(path, list) and len(path) == 1 and isinstance(path[0], str):
-                            # Use the first valid single-item string path; the code that constructs the alias array
-                            # should ensure the first such item is what belongs in the JSON schema
-                            name = path[0]
-                            break
-            field_json_schema = self.generate_inner(field).copy()
+                name = self._get_alias_name(field, name)
+            try:
+                field_json_schema = self.generate_inner(field).copy()
+            except PydanticOmit:
+                continue
             if 'title' not in field_json_schema and self.field_title_should_be_set(field):
                 title = self.get_title_from_name(name)
                 field_json_schema['title'] = title
             field_json_schema = self.handle_ref_overrides(field_json_schema)
             properties[name] = field_json_schema
             if required:
                 required_fields.append(name)
 
         json_schema = {'type': 'object', 'properties': properties}
         if required_fields:
             json_schema['required'] = required_fields  # type: ignore
         return json_schema
 
+    def _get_alias_name(self, field: CoreSchemaField, name: str) -> str:
+        if field['type'] == 'computed-field':
+            alias: Any = field.get('alias', name)
+        elif self.mode == 'validation':
+            alias = field.get('validation_alias', name)
+        else:
+            alias = field.get('serialization_alias', name)
+        if isinstance(alias, str):
+            name = alias
+        elif isinstance(alias, list):
+            alias = cast('list[str] | str', alias)
+            for path in alias:
+                if isinstance(path, list) and len(path) == 1 and isinstance(path[0], str):
+                    # Use the first valid single-item string path; the code that constructs the alias array
+                    # should ensure the first such item is what belongs in the JSON schema
+                    name = path[0]
+                    break
+        else:
+            assert_never(alias)
+        return name
+
     def typed_dict_field_schema(self, schema: core_schema.TypedDictField) -> JsonSchemaValue:
         return self.generate_inner(schema['schema'])
 
     def dataclass_field_schema(self, schema: core_schema.DataclassField) -> JsonSchemaValue:
         return self.generate_inner(schema['schema'])
 
     def model_field_schema(self, schema: core_schema.ModelField) -> JsonSchemaValue:
         return self.generate_inner(schema['schema'])
 
+    def computed_field_schema(self, schema: core_schema.ComputedField) -> JsonSchemaValue:
+        return self.generate_inner(schema['return_schema'])
+
     def model_schema(self, schema: core_schema.ModelSchema) -> JsonSchemaValue:
-        # We do not use schema['model'].model_json_schema() because it could lead to inconsistent refs handling, etc.
+        # We do not use schema['model'].model_json_schema() here
+        # because it could lead to inconsistent refs handling, etc.
         json_schema = self.generate_inner(schema['schema'])
 
         cls = cast('type[BaseModel]', schema['cls'])
         config = cls.model_config
         title = config.get('title')
         forbid_additional_properties = config.get('extra') == 'forbid'
         json_schema_extra = config.get('json_schema_extra')
@@ -687,29 +1010,64 @@
             raise ValueError(
                 f"model_config['json_schema_extra']={json_schema_extra} should be a dict, callable, or None"
             )
 
         return json_schema
 
     def model_fields_schema(self, schema: core_schema.ModelFieldsSchema) -> JsonSchemaValue:
-        named_required_fields = [
-            (name, field['schema']['type'] != 'default', field) for name, field in schema['fields'].items()
+        named_required_fields: list[tuple[str, bool, CoreSchemaField]] = [
+            (name, self.field_is_required(field), field)
+            for name, field in schema['fields'].items()
+            if self.field_is_present(field)
         ]
+        if self.mode == 'serialization':
+            named_required_fields.extend(self._name_required_computed_fields(schema.get('computed_fields', [])))
         return self._named_required_fields_schema(named_required_fields)
 
+    def field_is_present(self, field: CoreSchemaField) -> bool:
+        """
+        Whether the field should be included in the generated JSON schema
+        """
+        if self.mode == 'serialization':
+            # If you still want to include the field in the generated JSON schema,
+            # override this method and return True
+            return not field.get('serialization_exclude')
+        elif self.mode == 'validation':
+            return True
+        else:
+            assert_never(self.mode)
+
+    def field_is_required(
+        self, field: core_schema.ModelField | core_schema.DataclassField | core_schema.TypedDictField
+    ) -> bool:
+        """
+        Whether the field should be marked as required in the generated JSON schema.
+        (Note that this is irrelevant if the field is not present in the JSON schema.)
+        """
+        if self.mode == 'serialization':
+            return not field.get('serialization_exclude')
+        elif self.mode == 'validation':
+            if field['type'] == 'typed-dict-field':
+                return field['required']  # type: ignore  # required is always populated
+            else:
+                return field['schema']['type'] != 'default'
+        else:
+            assert_never(self.mode)
+
     def dataclass_args_schema(self, schema: core_schema.DataclassArgsSchema) -> JsonSchemaValue:
-        named_required_fields = [
-            (field['name'], field['schema']['type'] != 'default', field) for field in schema['fields']
+        named_required_fields: list[tuple[str, bool, CoreSchemaField]] = [
+            (field['name'], self.field_is_required(field), field)
+            for field in schema['fields']
+            if self.field_is_present(field)
         ]
+        if self.mode == 'serialization':
+            named_required_fields.extend(self._name_required_computed_fields(schema.get('computed_fields', [])))
         return self._named_required_fields_schema(named_required_fields)
 
     def dataclass_schema(self, schema: core_schema.DataclassSchema) -> JsonSchemaValue:
-        # TODO: Better-share this logic with model_schema
-        #   I'd prefer to clean this up _after_ we rework the approach to customizing dataclass JSON schema though
-
         json_schema = self.generate_inner(schema['schema']).copy()
 
         cls = schema['cls']
         config: ConfigDict = getattr(cls, '__pydantic_config__', cast('ConfigDict', {}))
 
         title = config.get('title') or cls.__name__
         forbid_additional_properties = config.get('extra') == 'forbid'
@@ -750,16 +1108,18 @@
             return self.kw_arguments_schema(kw_or_p_arguments + kw_only_arguments, var_kwargs_schema)
 
         if not prefer_positional:
             positional_possible = not kw_only_arguments and not var_kwargs_schema
             if positional_possible:
                 return self.p_arguments_schema(p_only_arguments + kw_or_p_arguments, var_args_schema)
 
-        raise PydanticInvalidForJsonSchema(
-            'Unable to generate JSON schema for arguments validator with positional only and keyword only arguments'
+        # TODO: When support for Python 3.7 is dropped, uncomment the block on `test_json_schema`
+        # to cover this test case.
+        raise PydanticInvalidForJsonSchema(  # pragma: no cover
+            'Unable to generate JSON schema for arguments validator with positional-only and keyword-only arguments'
         )
 
     def kw_arguments_schema(
         self, arguments: list[core_schema.ArgumentsParameter], var_kwargs_schema: CoreSchema | None
     ) -> JsonSchemaValue:
         properties: dict[str, JsonSchemaValue] = {}
         required: list[str] = []
@@ -832,21 +1192,21 @@
     def call_schema(self, schema: core_schema.CallSchema) -> JsonSchemaValue:
         return self.generate_inner(schema['arguments_schema'])
 
     def custom_error_schema(self, schema: core_schema.CustomErrorSchema) -> JsonSchemaValue:
         return self.generate_inner(schema['schema'])
 
     def json_schema(self, schema: core_schema.JsonSchema) -> JsonSchemaValue:
-        # TODO: For v1 compatibility, we should probably be using `schema['schema']` to produce the schema.
-        #   This is a serialization vs. validation thing; see https://github.com/pydantic/pydantic/issues/5072
-        #   -
-        #   The behavior below is not currently consistent with the v1 behavior, so should probably be changed.
-        #   I think making it work like v1 should be as easy as handling schema['schema'] instead, with the note
-        #   that we'll need to make generics work with Json (there is a test for this in test_generics.py).
-        return {'type': 'string', 'format': 'json-string'}
+        if self.mode == 'validation':
+            return {'type': 'string', 'format': 'json-string'}
+        elif 'schema' in schema:
+            return self.generate_inner(schema['schema'])
+        else:
+            # No wrapped schema, so return the same thing we would for an Any schema
+            return self.generate_inner(core_schema.any_schema())
 
     def url_schema(self, schema: core_schema.UrlSchema) -> JsonSchemaValue:
         json_schema = {'type': 'string', 'format': 'uri', 'minLength': 1}
         self.update_with_validations(json_schema, schema, self.ValidationsMapping.string)
         return json_schema
 
     def multi_host_url_schema(self, schema: core_schema.MultiHostUrlSchema) -> JsonSchemaValue:
@@ -874,15 +1234,19 @@
         """
         Returns true if a field with the given schema should have a title set based on the field name.
 
         Intuitively, we want this to return true for schemas that wouldn't otherwise provide their own title
         (e.g., int, float, str), and false for those that would (e.g., BaseModel subclasses).
         """
         if _core_utils.is_core_schema_field(schema):
-            return self.field_title_should_be_set(schema['schema'])
+            if schema['type'] == 'computed-field':
+                field_schema = schema['return_schema']
+            else:
+                field_schema = schema['schema']
+            return self.field_title_should_be_set(field_schema)
 
         elif _core_utils.is_core_schema(schema):
             if schema.get('ref'):  # things with refs, such as models and enums, should not have titles set
                 return False
             if schema['type'] in {'default', 'nullable', 'definitions'}:
                 return self.field_title_should_be_set(schema['schema'])  # type: ignore[typeddict-item]
             if _core_utils.is_function_with_inner_schema(schema):
@@ -890,44 +1254,50 @@
             if schema['type'] == 'definition-ref':
                 # Referenced schemas should not have titles set for the same reason
                 # schemas with refs should not
                 return False
             return True  # anything else should have title set
 
         else:
-            raise PydanticInvalidForJsonSchema(f'Unexpected schema type: schema={schema}')
+            raise PydanticInvalidForJsonSchema(f'Unexpected schema type: schema={schema}')  # pragma: no cover
 
     def normalize_name(self, name: str) -> str:
         return re.sub(r'[^a-zA-Z0-9.\-_]', '_', name).replace('.', '__')
 
-    def get_defs_ref(self, core_ref: CoreRef) -> DefsRef:
+    def get_defs_ref(self, core_mode_ref: CoreModeRef) -> DefsRef:
         """
         Override this method to change the way that definitions keys are generated from a core reference.
         """
         # Split the core ref into "components"; generic origins and arguments are each separate components
+        core_ref, mode = core_mode_ref
         components = re.split(r'([\][,])', core_ref)
         # Remove IDs from each component
         components = [x.split(':')[0] for x in components]
         core_ref_no_id = ''.join(components)
         # Remove everything before the last period from each "component"
         components = [re.sub(r'(?:[^.[\]]+\.)+((?:[^.[\]]+))', r'\1', x) for x in components]
         short_ref = ''.join(components)
 
-        first_choice = DefsRef(self.normalize_name(short_ref))  # name
-        second_choice = DefsRef(self.normalize_name(core_ref_no_id))  # module + qualname
-        third_choice = DefsRef(self.normalize_name(core_ref))  # module + qualname + id
-
+        mode_title = _MODE_TITLE_MAPPING[mode]
         # It is important that the generated defs_ref values be such that at least one could not
         # be generated for any other core_ref. Currently, this should be the case because we include
-        # the id of the source type in the core_ref, and therefore in the third_choice
-        choices = [first_choice, second_choice, third_choice]
-        self.defs_ref_fallbacks[core_ref] = choices[1:]
+        # the id of the source type in the core_ref
+        choices = [
+            DefsRef(self.normalize_name(short_ref)),  # name
+            DefsRef(self.normalize_name(short_ref + mode_title)),  # name + mode
+            DefsRef(self.normalize_name(core_ref_no_id)),  # module + qualname
+            DefsRef(self.normalize_name(core_ref_no_id + mode_title)),  # module + qualname + mode
+            DefsRef(self.normalize_name(core_ref)),  # module + qualname + id
+            DefsRef(self.normalize_name(core_ref + mode_title)),  # module + qualname + id + mode
+        ]
+
+        self.defs_ref_fallbacks[core_mode_ref] = choices[1:]
 
         for choice in choices:
-            if self.defs_to_core_refs.get(choice, core_ref) == core_ref:
+            if self.defs_to_core_refs.get(choice, core_mode_ref) == core_mode_ref:
                 return choice
             else:
                 self.collisions.add(choice)
 
         return choices[-1]  # should never get here if the final choice is guaranteed unique
 
     def resolve_collisions(self, json_schema: JsonSchemaValue) -> JsonSchemaValue:
@@ -942,46 +1312,47 @@
         made_changes = True
 
         # Note that because the defs ref choices eventually produce values that use the IDs and
         # should _never_ collide, it should not be possible for this while loop to run forever
         while made_changes:
             made_changes = False
 
-            for defs_ref, core_ref in self.defs_to_core_refs.items():
+            for defs_ref, core_mode_ref in self.defs_to_core_refs.items():
                 if defs_ref not in self.collisions:
                     continue
 
-                for choice in self.defs_ref_fallbacks[core_ref]:
+                for choice in self.defs_ref_fallbacks[core_mode_ref]:
                     if choice == defs_ref or choice in self.collisions:
                         continue
 
-                    if self.defs_to_core_refs.get(choice, core_ref) == core_ref:
+                    if self.defs_to_core_refs.get(choice, core_mode_ref) == core_mode_ref:
                         json_schema = self.change_defs_ref(defs_ref, choice, json_schema)
                         made_changes = True
                         break
                     else:
                         self.collisions.add(choice)
 
                 if made_changes:
                     break
 
         return json_schema
 
     def change_defs_ref(self, old: DefsRef, new: DefsRef, json_schema: JsonSchemaValue) -> JsonSchemaValue:
         if new == old:
             return json_schema
-        core_ref = self.defs_to_core_refs[old]
-        old_json_ref = self.core_to_json_refs[core_ref]
+        core_mode_ref = self.defs_to_core_refs[old]
+        old_json_ref = self.core_to_json_refs[core_mode_ref]
         new_json_ref = JsonRef(self.ref_template.format(model=new))
 
         self.definitions[new] = self.definitions.pop(old)
         self.defs_to_core_refs[new] = self.defs_to_core_refs.pop(old)
-        self.json_to_defs_refs[new_json_ref] = self.json_to_defs_refs.pop(old_json_ref)
-        self.core_to_defs_refs[core_ref] = new
-        self.core_to_json_refs[core_ref] = new_json_ref
+        assert self.json_to_defs_refs.pop(old_json_ref) == old
+        self.json_to_defs_refs[new_json_ref] = new
+        self.core_to_defs_refs[core_mode_ref] = new
+        self.core_to_json_refs[core_mode_ref] = new_json_ref
 
         def walk_replace_json_schema_ref(item: Any) -> Any:
             """
             Recursively update the JSON schema to use the new defs_ref.
             """
             if isinstance(item, list):
                 return [walk_replace_json_schema_ref(item) for item in item]
@@ -989,34 +1360,38 @@
                 ref = item.get('$ref')
                 if ref == old_json_ref:
                     item['$ref'] = new_json_ref
                 return {k: walk_replace_json_schema_ref(v) for k, v in item.items()}
             else:
                 return item
 
+        for k, v in self.definitions.items():
+            self.definitions[k] = walk_replace_json_schema_ref(v)
+
         return walk_replace_json_schema_ref(json_schema)
 
     def get_cache_defs_ref_schema(self, core_ref: CoreRef) -> tuple[DefsRef, JsonSchemaValue]:
         """
         This method wraps the get_defs_ref method with some cache-lookup/population logic,
         and returns both the produced defs_ref and the JSON schema that will refer to the right definition.
         """
-        maybe_defs_ref = self.core_to_defs_refs.get(core_ref)
+        core_mode_ref = (core_ref, self.mode)
+        maybe_defs_ref = self.core_to_defs_refs.get(core_mode_ref)
         if maybe_defs_ref is not None:
-            json_ref = self.core_to_json_refs[core_ref]
+            json_ref = self.core_to_json_refs[core_mode_ref]
             return maybe_defs_ref, {'$ref': json_ref}
 
-        defs_ref = self.get_defs_ref(core_ref)
+        defs_ref = self.get_defs_ref(core_mode_ref)
 
         # populate the ref translation mappings
-        self.core_to_defs_refs[core_ref] = defs_ref
-        self.defs_to_core_refs[defs_ref] = core_ref
+        self.core_to_defs_refs[core_mode_ref] = defs_ref
+        self.defs_to_core_refs[defs_ref] = core_mode_ref
 
         json_ref = JsonRef(self.ref_template.format(model=defs_ref))
-        self.core_to_json_refs[core_ref] = json_ref
+        self.core_to_json_refs[core_mode_ref] = json_ref
         self.json_to_defs_refs[json_ref] = defs_ref
         ref_json_schema = {'$ref': json_ref}
         return defs_ref, ref_json_schema
 
     def handle_ref_overrides(self, json_schema: JsonSchemaValue) -> JsonSchemaValue:
         """
         It is not valid for a schema with a top-level $ref to have sibling keys.
@@ -1148,20 +1523,15 @@
                 for v in schema:
                     _add_json_refs(v)
 
         _add_json_refs(json_schema)
         return json_refs
 
     def handle_invalid_for_json_schema(self, schema: CoreSchemaOrField, error_info: str) -> JsonSchemaValue:
-        if _core_metadata.CoreMetadataHandler(schema).metadata.get('pydantic_js_modify_function') is not None:
-            # Since there is a json schema modify function, assume that this type is meant to be handled,
-            # and the modify function will set all properties as appropriate
-            return {}
-        else:
-            raise PydanticInvalidForJsonSchema(f'Cannot generate a JsonSchema for {error_info}')
+        raise PydanticInvalidForJsonSchema(f'Cannot generate a JsonSchema for {error_info}')
 
     def emit_warning(self, kind: JsonSchemaWarningKind, detail: str) -> None:
         """
         This method simply emits PydanticJsonSchemaWarnings based on handling in the `warning_message` method.
         """
         message = self.render_warning_message(kind, detail)
         if message is not None:
@@ -1177,70 +1547,66 @@
         """
         if kind in self.ignored_warning_kinds:
             return None
         return f'{detail} [{kind}]'
 
 
 # ##### Start JSON Schema Generation Functions #####
-# TODO: These should be moved to the pydantic.funcs module or whatever when appropriate.
+
+
+def model_json_schema(
+    cls: type[BaseModel] | type[PydanticDataclass],
+    by_alias: bool = True,
+    ref_template: str = DEFAULT_REF_TEMPLATE,
+    schema_generator: type[GenerateJsonSchema] = GenerateJsonSchema,
+    mode: JsonSchemaMode = 'validation',
+) -> dict[str, Any]:
+    """Utility function to generate a JSON Schema for a model."""
+    schema_generator_instance = schema_generator(by_alias=by_alias, ref_template=ref_template)
+    return schema_generator_instance.generate(cls.__pydantic_core_schema__, mode=mode)
 
 
 def models_json_schema(
-    models: Sequence[type[BaseModel] | type[PydanticDataclass]],
+    models: Sequence[tuple[type[BaseModel] | type[PydanticDataclass], JsonSchemaMode]],
     *,
     by_alias: bool = True,
     title: str | None = None,
     description: str | None = None,
     ref_template: str = DEFAULT_REF_TEMPLATE,
     schema_generator: type[GenerateJsonSchema] = GenerateJsonSchema,
-) -> dict[str, Any]:
-    # TODO: Put this in the "methods" module once that is created?
+) -> tuple[dict[tuple[type[BaseModel] | type[PydanticDataclass], JsonSchemaMode], DefsRef], JsonSchemaValue]:
+    """Utility function to generate a JSON Schema for multiple models.
+
+    Args:
+        models: A sequence of tuples of the form (model, mode).
+        by_alias: Whether field aliases should be used as keys in the generated JSON Schema.
+        title: The title of the generated JSON Schema.
+        description: The description of the generated JSON Schema.
+        ref_template: The reference template to use for generating JSON Schema references.
+        schema_generator: The schema generator to use for generating the JSON Schema.
+
+    Returns:
+        A 2-tuple, where:
+            - The first element is a dictionary whose keys are tuples of a JSON schema key type and mode, and
+                whose values are `DefsRef`.
+            - The second element is the generated JSON Schema.
+    """
     instance = schema_generator(by_alias=by_alias, ref_template=ref_template)
-    definitions = instance.generate_definitions([x.__pydantic_core_schema__ for x in models])
+    inputs = [(m, mode, m.__pydantic_core_schema__) for m, mode in models]
+    key_map, definitions = instance.generate_definitions(inputs)
 
     json_schema: dict[str, Any] = {}
     if definitions:
         json_schema['$defs'] = definitions
     if title:
         json_schema['title'] = title
     if description:
         json_schema['description'] = description
 
-    return json_schema
-
-
-# TODO: Consider removing this cache, as it already gets used pretty infrequently.
-
-if sys.version_info >= (3, 9):  # Typing for weak dictionaries available at 3.9
-    _JsonSchemaCache = WeakKeyDictionary[Type[Any], Dict[Any, Any]]
-else:
-    _JsonSchemaCache = WeakKeyDictionary
-
-_JSON_SCHEMA_CACHE = _JsonSchemaCache()
-
-
-def model_json_schema(
-    cls: type[BaseModel] | type[PydanticDataclass],
-    by_alias: bool = True,
-    ref_template: str = DEFAULT_REF_TEMPLATE,
-    schema_generator: type[GenerateJsonSchema] = GenerateJsonSchema,
-) -> dict[str, Any]:
-    # TODO: Put this in the "methods" module once that is created
-    cls_json_schema_cache = _JSON_SCHEMA_CACHE.get(cls)
-    if cls_json_schema_cache is None:
-        _JSON_SCHEMA_CACHE[cls] = cls_json_schema_cache = {}
-
-    cached = cls_json_schema_cache.get((by_alias, ref_template, schema_generator))
-    if cached is not None:
-        return cached
-
-    json_schema = schema_generator(by_alias=by_alias, ref_template=ref_template).generate(cls.__pydantic_core_schema__)
-    cls_json_schema_cache[(by_alias, ref_template, schema_generator)] = json_schema
-
-    return json_schema
+    return key_map, json_schema
 
 
 # ##### End JSON Schema Generation Functions #####
 
 
 _Json = Union[Dict[str, Any], List[Any], str, int, float, bool, None]
 _JsonDict = Dict[str, _Json]
```

### Comparing `pydantic-2.0a4/pydantic/main.py` & `pydantic-2.0b1/pydantic/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,257 +1,148 @@
 """
-Logic for creating models, could perhaps be renamed to `models.py`.
+Logic for creating models.
 """
 from __future__ import annotations as _annotations
 
+import types
 import typing
 import warnings
-from abc import ABCMeta
 from copy import copy, deepcopy
-from inspect import getdoc
-from pathlib import Path
-from types import prepare_class, resolve_bases
-from typing import Any, Callable, Generic, Mapping, Tuple, cast
+from typing import Any
 
 import pydantic_core
 import typing_extensions
-from typing_extensions import deprecated
 
 from ._internal import (
+    _annotated_handlers,
     _config,
     _decorators,
+    _fields,
     _forward_ref,
     _generics,
     _model_construction,
     _repr,
     _typing_extra,
     _utils,
 )
-from ._internal._fields import Undefined
 from ._migration import getattr_migration
 from .config import ConfigDict
 from .deprecated import copy_internals as _deprecated_copy_internals
 from .deprecated import parse as _deprecated_parse
 from .errors import PydanticUndefinedAnnotation, PydanticUserError
-from .fields import ComputedFieldInfo, Field, FieldInfo, ModelPrivateAttr
+from .fields import ComputedFieldInfo, FieldInfo, ModelPrivateAttr
 from .json_schema import (
     DEFAULT_REF_TEMPLATE,
     GenerateJsonSchema,
-    GetJsonSchemaHandler,
+    JsonSchemaMode,
     JsonSchemaValue,
     model_json_schema,
 )
 
 if typing.TYPE_CHECKING:
     from inspect import Signature
+    from pathlib import Path
 
     from pydantic_core import CoreSchema, SchemaSerializer, SchemaValidator
+    from typing_extensions import Literal, Unpack
 
     from ._internal._utils import AbstractSetIntStr, MappingIntStrAny
+    from .fields import Field as _Field
 
     AnyClassMethod = classmethod[Any, Any, Any]
-    TupleGenerator = typing.Generator[Tuple[str, Any], None, None]
+    TupleGenerator = typing.Generator[typing.Tuple[str, Any], None, None]
     Model = typing.TypeVar('Model', bound='BaseModel')
     # should be `set[int] | set[str] | dict[int, IncEx] | dict[str, IncEx] | None`, but mypy can't cope
     IncEx: typing_extensions.TypeAlias = 'set[int] | set[str] | dict[int, Any] | dict[str, Any] | None'
 
-__all__ = 'BaseModel', 'create_model'
+__all__ = 'BaseModel', 'RootModel', 'create_model'
 
 _object_setattr = _model_construction.object_setattr
-# Note `ModelMetaclass` refers to `BaseModel`, but is also used to *create* `BaseModel`, so we need to add this extra
-# (somewhat hacky) boolean to keep track of whether we've created the `BaseModel` class yet, and therefore whether it's
-# safe to refer to it. If it *hasn't* been created, we assume that the `__new__` call we're in the middle of is for
-# the `BaseModel` class, since that's defined immediately after the metaclass.
-_base_class_defined = False
+_Undefined = _fields.Undefined
 
 
-class _ModelNamespaceDict(dict):  # type: ignore[type-arg]
+class BaseModel(metaclass=_model_construction.ModelMetaclass):
     """
-    Intercept attributes being set on model classes and warn about overriding of decorators (`@field_validator`, etc.)
-    """
-
-    def __setitem__(self, k: str, v: object) -> None:
-        existing: Any = self.get(k, None)
-        if existing and v is not existing and isinstance(existing, _decorators.PydanticDescriptorProxy):
-            warnings.warn(f'`{k}` overrides an existing Pydantic `{existing.decorator_info.decorator_repr}` decorator')
-
-        return super().__setitem__(k, v)
-
-
-@typing_extensions.dataclass_transform(kw_only_default=True, field_specifiers=(Field,))
-class ModelMetaclass(ABCMeta):
-    def __new__(
-        mcs,
-        cls_name: str,
-        bases: tuple[type[Any], ...],
-        namespace: dict[str, Any],
-        __pydantic_generic_metadata__: _generics.PydanticGenericMetadata | None = None,
-        __pydantic_reset_parent_namespace__: bool = True,
-        **kwargs: Any,
-    ) -> type:
-        if _base_class_defined:
-            base_field_names, class_vars, base_private_attributes = _collect_bases_data(bases)
-
-            config_wrapper = _config.ConfigWrapper.for_model(bases, namespace, kwargs)
-            namespace['model_config'] = config_wrapper.config_dict
-            private_attributes = _model_construction.inspect_namespace(
-                namespace, config_wrapper.ignored_types, class_vars, base_field_names
-            )
-            if private_attributes:
-                slots: set[str] = set(namespace.get('__slots__', ()))
-                namespace['__slots__'] = slots | private_attributes.keys()
-
-                if 'model_post_init' in namespace:
-                    # if there are private_attributes and a model_post_init function, we handle both
-                    original_model_post_init = namespace['model_post_init']
-
-                    def wrapped_model_post_init(self: BaseModel, __context: Any) -> None:
-                        """
-                        We need to both initialize private attributes and call the user-defined model_post_init method
-                        """
-                        _model_construction.init_private_attributes(self, __context)
-                        original_model_post_init(self, __context)
-
-                    namespace['model_post_init'] = wrapped_model_post_init
-                else:
-                    namespace['model_post_init'] = _model_construction.init_private_attributes
-
-            namespace['__class_vars__'] = class_vars
-            namespace['__private_attributes__'] = {**base_private_attributes, **private_attributes}
-
-            if config_wrapper.extra == 'allow':
-                namespace['__getattr__'] = _model_construction.model_extra_getattr
-
-            if '__hash__' not in namespace and config_wrapper.frozen:
-
-                def hash_func(self: Any) -> int:
-                    return hash(self.__class__) + hash(tuple(self.__dict__.values()))
-
-                namespace['__hash__'] = hash_func
-
-            cls: type[BaseModel] = super().__new__(mcs, cls_name, bases, namespace, **kwargs)  # type: ignore
-
-            cls.__pydantic_decorators__ = _decorators.DecoratorInfos.build(cls)
-
-            # Use the getattr below to grab the __parameters__ from the `typing.Generic` parent class
-            if __pydantic_generic_metadata__:
-                cls.__pydantic_generic_metadata__ = __pydantic_generic_metadata__
-            else:
-                parameters = getattr(cls, '__parameters__', ())
-                parent_parameters = getattr(cls, '__pydantic_generic_metadata__', {}).get('parameters', ())
-                if parameters and parent_parameters and not all(x in parameters for x in parent_parameters):
-                    combined_parameters = parent_parameters + tuple(x for x in parameters if x not in parent_parameters)
-                    parameters_str = ', '.join([str(x) for x in combined_parameters])
-                    error_message = (
-                        f'All parameters must be present on typing.Generic;'
-                        f' you should inherit from typing.Generic[{parameters_str}]'
-                    )
-                    if Generic not in bases:  # pragma: no cover
-                        # This branch will only be hit if I have misunderstood how `__parameters__` works.
-                        # If that is the case, and a user hits this, I could imagine it being very helpful
-                        # to have this extra detail in the reported traceback.
-                        error_message += f' (bases={bases})'
-                    raise TypeError(error_message)
-
-                cls.__pydantic_generic_metadata__ = {
-                    'origin': None,
-                    'args': (),
-                    'parameters': parameters,
-                }
-
-            cls.__pydantic_model_complete__ = False  # Ensure this specific class gets completed
-
-            # preserve `__set_name__` protocol defined in https://peps.python.org/pep-0487
-            # for attributes not in `new_namespace` (e.g. private attributes)
-            for name, obj in private_attributes.items():
-                set_name = getattr(obj, '__set_name__', None)
-                if callable(set_name):
-                    set_name(cls, name)
-
-            if __pydantic_reset_parent_namespace__:
-                cls.__pydantic_parent_namespace__ = _typing_extra.parent_frame_namespace()
-            parent_namespace = getattr(cls, '__pydantic_parent_namespace__', None)
-
-            types_namespace = _typing_extra.get_cls_types_namespace(cls, parent_namespace)
-            _model_construction.set_model_fields(cls, bases, types_namespace)
-            _model_construction.complete_model_class(
-                cls,
-                cls_name,
-                config_wrapper,
-                raise_errors=False,
-                types_namespace=types_namespace,
-            )
-            # using super(cls, cls) on the next line ensures we only call the parent class's __pydantic_init_subclass__
-            # I believe the `type: ignore` is only necessary because mypy doesn't realize that this code branch is
-            # only hit for _proper_ subclasses of BaseModel
-            super(cls, cls).__pydantic_init_subclass__(**kwargs)  # type: ignore[misc]
-            return cls
-        else:
-            # this is the BaseModel class itself being created, no logic required
-            return super().__new__(mcs, cls_name, bases, namespace, **kwargs)
-
-    @classmethod
-    def __prepare__(cls, *args: Any, **kwargs: Any) -> Mapping[str, object]:
-        return _ModelNamespaceDict()
-
-    def __instancecheck__(self, instance: Any) -> bool:
-        """
-        Avoid calling ABC _abc_subclasscheck unless we're pretty sure.
-
-        See #3829 and python/cpython#92810
-        """
-        return hasattr(instance, '__pydantic_validator__') and super().__instancecheck__(instance)
+    A base model class for creating Pydantic models.
 
+    * `model_fields` is a class attribute that contains the fields defined on the model in Pydantic V2.
+        This replaces `Model.__fields__` from Pydantic V1.
+    *  `__pydantic_decorators__` contains the decorators defined on the model in Pydantic V2. This replaces
+        `Model.__validators__` and `Model.__root_validators__` from Pydantic V1.
+
+    Attributes:
+        __pydantic_validator__ (typing.ClassVar[SchemaValidator]): Validator for checking schema validity.
+        __pydantic_core_schema__ (typing.ClassVar[CoreSchema]): Schema for representing the model's core.
+        __pydantic_serializer__ (typing.ClassVar[SchemaSerializer]): Serializer for the schema.
+        __pydantic_decorators__ (_decorators.DecoratorInfos): Metadata for `@field_validator`, `@root_validator`,
+            and `@serializer` decorators.
+        model_fields (typing.ClassVar[dict[str, FieldInfo]]): Fields in the model.
+        __signature__ (typing.ClassVar[Signature]): Signature for instantiating the model.
+        __private_attributes__ (typing.ClassVar[dict[str, ModelPrivateAttr]]): Private attributes of the model.
+        __class_vars__ (typing.ClassVar[set[str]]): Class variables of the model.
+        __pydantic_fields_set__ (set[str]): Set of fields in the model.
+        __pydantic_extra__ (typing.Optional[dict[str, Any]]): Extra fields in the model.
+        __pydantic_generic_metadata__ (_generics.PydanticGenericMetadata): Metadata for generic models.
+        __pydantic_parent_namespace__ (typing.Optional[dict[str, Any]]): Parent namespace of the model.
+    """
 
-class BaseModel(_repr.Representation, metaclass=ModelMetaclass):
     if typing.TYPE_CHECKING:
         # populated by the metaclass, defined here to help IDEs only
         __pydantic_validator__: typing.ClassVar[SchemaValidator]
         __pydantic_core_schema__: typing.ClassVar[CoreSchema]
         __pydantic_serializer__: typing.ClassVar[SchemaSerializer]
         __pydantic_decorators__: typing.ClassVar[_decorators.DecoratorInfos]
-        """metadata for `@validator`, `@root_validator` and `@serializer` decorators"""
+        """metadata for `@field_validator`, `@root_validator` and `@serializer` decorators"""
         model_fields: typing.ClassVar[dict[str, FieldInfo]] = {}
         __signature__: typing.ClassVar[Signature]
         __private_attributes__: typing.ClassVar[dict[str, ModelPrivateAttr]]
         __class_vars__: typing.ClassVar[set[str]]
-        __pydantic_fields_set__: set[str] = set()
-        __pydantic_extra__: dict[str, Any] | None = None
+
+        # Use the non-existent kwarg `init=False` in pydantic.fields.Field so @dataclass_transform
+        # doesn't think these are keyword arguments for BaseModel.__init__
+        __pydantic_fields_set__: set[str] = _Field(default_factory=set, init=False)  # type: ignore
+        __pydantic_extra__: dict[str, Any] | None = _Field(default=None, init=False)  # type: ignore
+        __pydantic_private__: dict[str, Any] | None = _Field(default=None, init=False)  # type: ignore
+
         __pydantic_generic_metadata__: typing.ClassVar[_generics.PydanticGenericMetadata]
         __pydantic_parent_namespace__: typing.ClassVar[dict[str, Any] | None]
+        __pydantic_custom_init__: typing.ClassVar[bool]
+        __pydantic_post_init__: typing.ClassVar[None | Literal['model_post_init']]
     else:
         # `model_fields` and `__pydantic_decorators__` must be set for
         # pydantic._internal._generate_schema.GenerateSchema.model_schema to work for a plain BaseModel annotation
         model_fields = {}
         __pydantic_decorators__ = _decorators.DecoratorInfos()
         __pydantic_validator__ = _model_construction.MockValidator(
             'Pydantic models should inherit from BaseModel, BaseModel cannot be instantiated directly',
             code='base-model-instantiated',
         )
 
     model_config = ConfigDict()
-    __slots__ = '__dict__', '__pydantic_fields_set__', '__pydantic_extra__'
-    __doc__ = ''  # Null out the Representation docstring
-    __pydantic_model_complete__ = False
+    __slots__ = '__dict__', '__pydantic_fields_set__', '__pydantic_extra__', '__pydantic_private__'
+    __pydantic_complete__ = False
+    __pydantic_root_model__: typing.ClassVar[bool] = False
 
     def __init__(__pydantic_self__, **data: Any) -> None:  # type: ignore
         """
         Create a new model by parsing and validating input data from keyword arguments.
 
         Raises ValidationError if the input data cannot be parsed to form a valid model.
 
         Uses something other than `self` for the first arg to allow "self" as a field name.
         """
         # `__tracebackhide__` tells pytest and some other tools to omit this function from tracebacks
         __tracebackhide__ = True
         __pydantic_self__.__pydantic_validator__.validate_python(data, self_instance=__pydantic_self__)
 
+    __init__.__pydantic_base_init__ = True  # type: ignore
+
     @classmethod
     def __get_pydantic_core_schema__(
-        cls, __source: type[BaseModel], __handler: Callable[[Any], CoreSchema]
+        cls, __source: type[BaseModel], __handler: _annotated_handlers.GetCoreSchemaHandler
     ) -> CoreSchema:
         """Hook into generating the model's CoreSchema.
 
         Args:
             __source (type[BaseModel]): The class we are generating a schema for.
                 This will generally be the same as the `cls` argument if this is a classmethod.
             __handler (GetJsonSchemaHandler): Call into Pydantic's internal JSON schema generation.
@@ -271,15 +162,15 @@
 
         return __handler(__source)
 
     @classmethod
     def __get_pydantic_json_schema__(
         cls,
         __core_schema: CoreSchema,
-        __handler: GetJsonSchemaHandler,
+        __handler: _annotated_handlers.GetJsonSchemaHandler,
     ) -> JsonSchemaValue:
         """Hook into generating the model's JSON schema.
 
         Args:
             __core_schema (CoreSchema): A `pydantic-core` CoreSchema.
                 You can ignore this argument and call the handler with a new CoreSchema,
                 wrap this CoreSchema (`{'type': 'nullable', 'schema': current_schema}`),
@@ -292,130 +183,225 @@
                 for a type.
 
         Returns:
             JsonSchemaValue: A JSON schema, as a Python object.
         """
         return __handler(__core_schema)
 
+    if typing.TYPE_CHECKING:
+
+        def __init_subclass__(cls, **kwargs: Unpack[ConfigDict]):
+            """
+            This signature is included purely to help type-checkers check arguments to class declaration, which
+            provides a way to conveniently set model_config key/value pairs:
+
+                class MyModel(BaseModel, extra='allow'):
+                    ...
+
+            However, this may be deceiving, since the _actual_ calls to `__init_subclass__` will not receive any
+            of the config arguments, and will only receive any keyword arguments passed during class initialization
+            that are _not_ expected keys in ConfigDict. (This is due to the way `ModelMetaclass.__new__` works.)
+
+            Args:
+                **kwargs (Unpack[ConfigDict]): Keyword arguments passed to the class definition, which set model_config
+            """
+
     @classmethod
     def __pydantic_init_subclass__(cls, **kwargs: Any) -> None:
         """
-        This is intended to behave just like `__init_subclass__`, but is called by ModelMetaclass
+        This is intended to behave just like `__init_subclass__`, but is called by `ModelMetaclass`
         only after the class is actually fully initialized. In particular, attributes like `model_fields` will
         be present when this is called.
 
         This is necessary because `__init_subclass__` will always be called by `type.__new__`,
         and it would require a prohibitively large refactor to the `ModelMetaclass` to ensure that
         `type.__new__` was called in such a manner that the class would already be sufficiently initialized.
 
         This will receive the same `kwargs` that would be passed to the standard `__init_subclass__`, namely,
         any kwargs passed to the class definition that aren't used internally by pydantic.
+
+        Args:
+            **kwargs (Any): Any keyword arguments passed to the class definition that aren't used internally
+            by pydantic.
         """
         pass
 
     @classmethod
     def model_validate(
         cls: type[Model], obj: Any, *, strict: bool | None = None, context: dict[str, Any] | None = None
     ) -> Model:
+        """Validate a pydantic model instance.
+
+        Args:
+            cls (type[Model]): The model class to use.
+            obj (Any): The object to validate.
+            strict (bool | None, optional): Whether to raise an exception on invalid fields. Defaults to None.
+            context (dict[str, Any] | None, optional): Additional context to pass to the validator. Defaults to None.
+
+        Raises:
+            ValidationError: If the object could not be validated.
+
+        Returns:
+            Model: The validated model instance.
+        """
         # `__tracebackhide__` tells pytest and some other tools to omit this function from tracebacks
         __tracebackhide__ = True
         return cls.__pydantic_validator__.validate_python(obj, strict=strict, context=context)
 
     @property
     def model_fields_set(self) -> set[str]:
         """
-        The set of fields that have been set on this model instance, i.e. that were not filled from defaults.
+        Returns the set of fields that have been set on this model instance.
+
+        Returns:
+            A set of strings representing the fields that have been set,
+                i.e. that were not filled from defaults.
         """
         return self.__pydantic_fields_set__
 
     @property
     def model_extra(self) -> dict[str, Any] | None:
         """
-        Extra fields set during validation, this will be `None` if `config.extra` is not set to `"allow"`.
+        Get extra fields set during validation.
+
+        Returns:
+            A dictionary of extra fields, or `None` if `config.extra` is not set to `"allow"`.
         """
         return self.__pydantic_extra__
 
     @property
     def model_computed_fields(self) -> dict[str, ComputedFieldInfo]:
         """
-        The computed fields of this model instance.
+        Get the computed fields of this model instance.
+
+        Returns:
+            Dict: A dictionary of computed field names and their corresponding `ComputedFieldInfo` objects.
         """
         return {k: v.info for k, v in self.__pydantic_decorators__.computed_fields.items()}
 
     @classmethod
     def model_validate_json(
         cls: type[Model],
         json_data: str | bytes | bytearray,
         *,
         strict: bool | None = None,
         context: dict[str, Any] | None = None,
     ) -> Model:
+        """Validate the given JSON data against the Pydantic model.
+
+        Args:
+            cls (type[Model]): The Pydantic model class to validate against.
+            json_data (Union[str, bytes, bytearray]): The JSON data to validate.
+
+        Keyword Args:
+            strict (Optional[bool]): Whether to enforce types strictly (default: `None`).
+            context (Optional[Dict[str, Any]]): Extra variables to pass to the validator (default: `None`).
+
+        Returns:
+            Model: The validated Pydantic model.
+
+        Raises:
+            ValueError: If `json_data` is not a JSON string.
+        """
         # `__tracebackhide__` tells pytest and some other tools to omit this function from tracebacks
         __tracebackhide__ = True
         return cls.__pydantic_validator__.validate_json(json_data, strict=strict, context=context)
 
     def model_post_init(self, __context: Any) -> None:
         """
-        If you override `model_post_init`, it will be called at the end of `__init__` and `model_construct`
+        Override this method to perform additional initialization after `__init__` and `model_construct`.
+        This is useful if you want to do some validation that requires the entire model to be initialized.
         """
         pass
 
     def __setattr__(self, name: str, value: Any) -> None:
         if name in self.__class_vars__:
             raise AttributeError(
                 f'"{name}" is a ClassVar of `{self.__class__.__name__}` and cannot be set on an instance. '
                 f'If you want to set a value on the class, use `{self.__class__.__name__}.{name} = value`.'
             )
         elif name.startswith('_'):
-            _object_setattr(self, name, value)
+            if self.__pydantic_private__ is None or name not in self.__private_attributes__:
+                _object_setattr(self, name, value)
+            else:
+                attribute = self.__private_attributes__[name]
+                if hasattr(attribute, '__set__'):
+                    attribute.__set__(self, value)  # type: ignore
+                else:
+                    self.__pydantic_private__[name] = value
             return
         elif self.model_config.get('frozen', None):
-            raise TypeError(f'"{self.__class__.__name__}" is frozen and does not support item assignment')
+            error: pydantic_core.InitErrorDetails = {
+                'type': 'frozen_instance',
+                'loc': (name,),
+                'input': value,
+            }
+            raise pydantic_core.ValidationError.from_exception_data(self.__class__.__name__, [error])
 
         attr = getattr(self.__class__, name, None)
         if isinstance(attr, property):
             attr.__set__(self, value)
         elif self.model_config.get('validate_assignment', None):
             self.__pydantic_validator__.validate_assignment(self, name, value)
         elif self.model_config.get('extra') != 'allow' and name not in self.model_fields:
             # TODO - matching error
             raise ValueError(f'"{self.__class__.__name__}" object has no field "{name}"')
         else:
             self.__dict__[name] = value
             self.__pydantic_fields_set__.add(name)
 
     def __getstate__(self) -> dict[Any, Any]:
-        private_attrs = ((k, getattr(self, k, Undefined)) for k in self.__private_attributes__)
+        private = self.__pydantic_private__
+        if private:
+            private = {k: v for k, v in private.items() if v is not _Undefined}
         return {
             '__dict__': self.__dict__,
+            '__pydantic_extra__': self.__pydantic_extra__,
             '__pydantic_fields_set__': self.__pydantic_fields_set__,
-            '__private_attribute_values__': {k: v for k, v in private_attrs if v is not Undefined},
+            '__pydantic_private__': private,
         }
 
     def __setstate__(self, state: dict[Any, Any]) -> None:
         _object_setattr(self, '__dict__', state['__dict__'])
         _object_setattr(self, '__pydantic_fields_set__', state['__pydantic_fields_set__'])
-        for name, value in state.get('__private_attribute_values__', {}).items():
-            _object_setattr(self, name, value)
+        _object_setattr(self, '__pydantic_extra__', state['__pydantic_extra__'])
+        _object_setattr(self, '__pydantic_private__', state['__pydantic_private__'])
 
     def model_dump(
         self,
         *,
-        mode: typing_extensions.Literal['json', 'python'] | str = 'python',
+        mode: Literal['json', 'python'] | str = 'python',
         include: IncEx = None,
         exclude: IncEx = None,
         by_alias: bool = False,
         exclude_unset: bool = False,
         exclude_defaults: bool = False,
         exclude_none: bool = False,
         round_trip: bool = False,
         warnings: bool = True,
     ) -> dict[str, Any]:
         """
         Generate a dictionary representation of the model, optionally specifying which fields to include or exclude.
+
+        Args:
+            self (object): The instance of the class that this method is attached to.
+            mode (Literal['json', 'python'] | str): The mode in which `to_python` should run.
+                If mode is 'json', the dictionary will only contain JSON serializable types.
+                If mode is 'python', the dictionary may contain any Python objects.
+            include (Optional[List[str]]): A list of fields to include in the output.
+            exclude (Optional[List[str]]): A list of fields to exclude from the output.
+            by_alias (bool): Whether to use the field's alias in the dictionary key if defined.
+            exclude_unset (bool): Whether to exclude fields that are unset or None from the output.
+            exclude_defaults (bool): Whether to exclude fields that are set to their default value from the output.
+            exclude_none (bool): Whether to exclude fields that have a value of None from the output.
+            round_trip (bool): Whether to enable serialization and deserialization round-trip support.
+            warnings (bool): Whether to log warnings when invalid fields are encountered.
+
+        Returns:
+            Dict: A dictionary representation of the model.
         """
         return self.__pydantic_serializer__.to_python(
             self,
             mode=mode,
             by_alias=by_alias,
             include=include,
             exclude=exclude,
@@ -436,15 +422,33 @@
         exclude_unset: bool = False,
         exclude_defaults: bool = False,
         exclude_none: bool = False,
         round_trip: bool = False,
         warnings: bool = True,
     ) -> str:
         """
-        Generate a JSON representation of the model, `include` and `exclude` arguments as per `dict()`.
+        Generates a JSON representation of the model using Pydantic's `to_json` method.
+
+        Args:
+            indent (Optional[int]): Indentation to use in the JSON output. If None is passed, the output will be
+                compact.
+            include (Optional[Union[str, Set[str]]]): Field(s) to include in the JSON output. Can take either a string
+                or set of strings.
+            exclude (Optional[Union[str, Set[str]]]): Field(s) to exclude from the JSON output. Can take either a
+                string or set of strings.
+            by_alias (bool): Whether to serialize using field aliases. Defaults to False.
+            exclude_unset (bool): Whether to exclude fields that have not been explicitly set. Defaults to False.
+            exclude_defaults (bool): Whether to exclude fields that have the default value. Defaults to False.
+            exclude_none (bool): Whether to exclude fields that have a value of None. Defaults to False.
+            round_trip (bool): Whether to use serialization/deserialization between JSON and class instance. Defaults
+                to False.
+            warnings (bool): Whether to show any warnings that occurred during serialization. Defaults to True.
+
+        Returns:
+            str: A JSON string representation of the model.
         """
         return self.__pydantic_serializer__.to_json(
             self,
             indent=indent,
             include=include,
             exclude=exclude,
             by_alias=by_alias,
@@ -454,88 +458,111 @@
             round_trip=round_trip,
             warnings=warnings,
         ).decode()
 
     @classmethod
     def model_construct(cls: type[Model], _fields_set: set[str] | None = None, **values: Any) -> Model:
         """
-        Creates a new model setting __dict__ and __pydantic_fields_set__ from trusted or pre-validated data.
+        Creates a new instance of the `Model` class with validated data.
+
+        Creates a new model setting `__dict__` and `__pydantic_fields_set__` from trusted or pre-validated data.
         Default values are respected, but no other validation is performed.
         Behaves as if `Config.extra = 'allow'` was set since it adds all passed values
+
+        Args:
+            cls (type[Model]): The `Model` class.
+            _fields_set (set[str], optional): The set of field names accepted for the Model instance.
+            values (Any): Trusted or pre-validated data dictionary.
+
+        Returns:
+            Model: A new instance of the `Model` class with validated data.
         """
         m = cls.__new__(cls)
         fields_values: dict[str, Any] = {}
         for name, field in cls.model_fields.items():
             if field.alias and field.alias in values:
                 fields_values[name] = values[field.alias]
             elif name in values:
                 fields_values[name] = values[name]
             elif not field.is_required():
                 fields_values[name] = field.get_default(call_default_factory=True)
         _extra: dict[str, Any] | None = None
         if cls.model_config.get('extra') == 'allow':
             _extra = {}
             for k, v in values.items():
-                if k in cls.model_fields:
-                    fields_values[k] = v
-                else:
-                    _extra[k] = v
+                _extra[k] = v
         else:
             fields_values.update(values)
         _object_setattr(m, '__dict__', fields_values)
         if _fields_set is None:
             _fields_set = set(values.keys())
         _object_setattr(m, '__pydantic_fields_set__', _fields_set)
         _object_setattr(m, '__pydantic_extra__', _extra)
-        if type(m).model_post_init is not BaseModel.model_post_init:
+
+        if cls.__pydantic_post_init__:
             m.model_post_init(None)
+        else:
+            # Note: if there are any private attributes, cls.__pydantic_post_init__ would exist
+            # Since it doesn't, that means that `__pydantic_private__` should be set to None
+            _object_setattr(m, '__pydantic_private__', None)
+
         return m
 
     @classmethod
     def model_json_schema(
         cls,
         by_alias: bool = True,
         ref_template: str = DEFAULT_REF_TEMPLATE,
         schema_generator: type[GenerateJsonSchema] = GenerateJsonSchema,
+        mode: JsonSchemaMode = 'validation',
     ) -> dict[str, Any]:
         """
-        To override the logic used to generate the JSON schema, you can create a subclass of GenerateJsonSchema
+        Generates a JSON schema for a model class.
+
+        To override the logic used to generate the JSON schema, you can create a subclass of `GenerateJsonSchema`
         with your desired modifications, then override this method on a custom base class and set the default
         value of `schema_generator` to be your subclass.
-        """
-        return model_json_schema(cls, by_alias=by_alias, ref_template=ref_template, schema_generator=schema_generator)
 
-    @classmethod
-    def model_modify_json_schema(cls, json_schema: JsonSchemaValue) -> JsonSchemaValue:
-        """
-        Overriding this method provides a simple way to modify the JSON schema generated for the model.
-
-        This is a convenience method primarily intended to control how the "generic" properties of the JSON schema
-        are populated. See https://json-schema.org/understanding-json-schema/reference/generic.html for more details.
+        Args:
+            cls (type): The model class for which the JSON schema is to be generated.
+            by_alias (bool): Whether to use attribute aliases or not. Defaults to `True`.
+            ref_template (str): The reference template. Defaults to `DEFAULT_REF_TEMPLATE`.
+            schema_generator (Type[GenerateJsonSchema]): The JSON schema generator. Defaults to `GenerateJsonSchema`.
 
-        If you want to make more sweeping changes to how the JSON schema is generated, you will probably want to create
-        a subclass of `GenerateJsonSchema` and pass it as `schema_generator` in `BaseModel.model_json_schema`.
+        Returns:
+            Dict: The JSON schema for the given `cls` model class.
         """
-        metadata = {'title': cls.model_config.get('title', None) or cls.__name__, 'description': getdoc(cls) or None}
-        metadata = {k: v for k, v in metadata.items() if v is not None}
-        return {**metadata, **json_schema}
+        return model_json_schema(
+            cls, by_alias=by_alias, ref_template=ref_template, schema_generator=schema_generator, mode=mode
+        )
 
     @classmethod
     def model_rebuild(
         cls,
         *,
         force: bool = False,
         raise_errors: bool = True,
         _parent_namespace_depth: int = 2,
         _types_namespace: dict[str, Any] | None = None,
     ) -> bool | None:
         """
-        Try to (Re)construct the model schema.
+        Try to rebuild or reconstruct the model core schema
+
+        Args:
+            cls (type): The class to build the model core schema for.
+            force (bool): Whether to force the rebuilding of the model schema, defaults to `False`.
+            raise_errors (bool): Whether to raise errors, defaults to `True`.
+            _parent_namespace_depth (int): The depth level of the parent namespace, defaults to 2.
+            _types_namespace (dict[str, Any] | None): The types namespace, defaults to `None`.
+
+        Returns:
+            bool or None: Returns `None` if model schema is complete and no rebuilding is required.
+                If rebuilding _is_ required, returns `True` if rebuilding was successful, otherwise `False`.
         """
-        if not force and cls.__pydantic_model_complete__:
+        if not force and cls.__pydantic_complete__:
             return None
         else:
             if _types_namespace is not None:
                 types_namespace: dict[str, Any] | None = _types_namespace.copy()
             else:
                 if _parent_namespace_depth > 0:
                     frame_parent_ns = _typing_extra.parent_frame_namespace(parent_depth=_parent_namespace_depth) or {}
@@ -563,37 +590,34 @@
         if isinstance(other, BaseModel):
             # When comparing instances of generic types for equality, as long as all field values are equal,
             # only require their generic origin types to be equal, rather than exact type equality.
             # This prevents headaches like MyGeneric(x=1) != MyGeneric[Any](x=1).
             self_type = self.__pydantic_generic_metadata__['origin'] or self.__class__
             other_type = other.__pydantic_generic_metadata__['origin'] or other.__class__
 
-            if self_type != other_type:
-                return False
-
-            if self.__dict__ != other.__dict__:
-                return False
-
-            # If the types and field values match, check for equality of private attributes
-            for k in self.__private_attributes__:
-                if getattr(self, k, Undefined) != getattr(other, k, Undefined):
-                    return False
-
-            return True
+            return (
+                self_type == other_type
+                and self.__dict__ == other.__dict__
+                and self.__pydantic_private__ == other.__pydantic_private__
+                and self.__pydantic_extra__ == other.__pydantic_extra__
+            )
         else:
             return NotImplemented  # delegate to the other item in the comparison
 
     def model_copy(self: Model, *, update: dict[str, Any] | None = None, deep: bool = False) -> Model:
         """
-        Returns a copy of the model.
+        Returns a copy of the Model.
 
-        :param update: values to change/add in the new model. Note: the data is not validated before creating
-            the new model: you should trust this data
-        :param deep: set to `True` to make a deep copy of the model
-        :return: new model instance
+        Args:
+            update (Optional[Dict[str, Any]]): Values to change/add in the new model. Note: the data is not validated
+                before creating the new model. You should trust this data.
+            deep (bool): Set to `True` to make a deep copy of the model.
+
+        Returns:
+            Model: New model instance.
         """
         copied = self.__deepcopy__() if deep else self.__copy__()
         if update:
             if self.model_config.get('extra') == 'allow':
                 for k, v in update.items():
                     if k in self.model_fields:
                         copied.__dict__[k] = v
@@ -611,60 +635,82 @@
         Returns a shallow copy of the model
         """
         cls = type(self)
         m = cls.__new__(cls)
         _object_setattr(m, '__dict__', copy(self.__dict__))
         _object_setattr(m, '__pydantic_extra__', copy(self.__pydantic_extra__))
         _object_setattr(m, '__pydantic_fields_set__', copy(self.__pydantic_fields_set__))
-        for name in self.__private_attributes__:
-            value = getattr(self, name, Undefined)
-            if value is not Undefined:
-                _object_setattr(m, name, value)
+
+        if self.__pydantic_private__ is None:
+            _object_setattr(m, '__pydantic_private__', None)
+        else:
+            _object_setattr(
+                m, '__pydantic_private__', {k: v for k, v in self.__pydantic_private__.items() if v is not _Undefined}
+            )
+
         return m
 
     def __deepcopy__(self: Model, memo: dict[int, Any] | None = None) -> Model:
         """
         Returns a deep copy of the model
         """
         cls = type(self)
         m = cls.__new__(cls)
         _object_setattr(m, '__dict__', deepcopy(self.__dict__, memo=memo))
         _object_setattr(m, '__pydantic_extra__', deepcopy(self.__pydantic_extra__, memo=memo))
         # This next line doesn't need a deepcopy because __pydantic_fields_set__ is a set[str],
         # and attempting a deepcopy would be marginally slower.
         _object_setattr(m, '__pydantic_fields_set__', copy(self.__pydantic_fields_set__))
-        for name in self.__private_attributes__:
-            value = getattr(self, name, Undefined)
-            if value is not Undefined:
-                _object_setattr(m, name, deepcopy(value, memo=memo))
+
+        if self.__pydantic_private__ is None:
+            _object_setattr(m, '__pydantic_private__', None)
+        else:
+            _object_setattr(
+                m,
+                '__pydantic_private__',
+                deepcopy({k: v for k, v in self.__pydantic_private__.items() if v is not _Undefined}, memo=memo),
+            )
+
         return m
 
     def __repr_args__(self) -> _repr.ReprArgs:
         yield from (
             (k, v)
             for k, v in self.__dict__.items()
             if not k.startswith('_') and (k not in self.model_fields or self.model_fields[k].repr)
         )
         pydantic_extra = self.__pydantic_extra__
         if pydantic_extra is not None:
             yield from ((k, v) for k, v in pydantic_extra.items())
         yield from ((k, getattr(self, k)) for k, v in self.model_computed_fields.items() if v.repr)
 
+    # take logic from `_repr.Representation` without the side effects of inheritance, see #5740
+    __repr_name__ = _repr.Representation.__repr_name__
+    __repr_str__ = _repr.Representation.__repr_str__
+    __pretty__ = _repr.Representation.__pretty__
+    __rich_repr__ = _repr.Representation.__rich_repr__
+
+    def __str__(self) -> str:
+        return self.__repr_str__(' ')
+
+    def __repr__(self) -> str:
+        return f'{self.__repr_name__()}({self.__repr_str__(", ")})'
+
     def __class_getitem__(
         cls, typevar_values: type[Any] | tuple[type[Any], ...]
     ) -> type[BaseModel] | _forward_ref.PydanticForwardRef | _forward_ref.PydanticRecursiveRef:
         cached = _generics.get_cached_generic_type_early(cls, typevar_values)
         if cached is not None:
             return cached
 
         if cls is BaseModel:
             raise TypeError('Type parameters should be placed on typing.Generic, not BaseModel')
         if not hasattr(cls, '__parameters__'):
             raise TypeError(f'{cls} cannot be parametrized because it does not inherit from typing.Generic')
-        if not cls.__pydantic_generic_metadata__['parameters'] and Generic not in cls.__bases__:
+        if not cls.__pydantic_generic_metadata__['parameters'] and typing.Generic not in cls.__bases__:
             raise TypeError(f'{cls} is not a generic class')
 
         if not isinstance(typevar_values, tuple):
             typevar_values = (typevar_values,)
         _generics.check_parameters_count(cls, typevar_values)
 
         # Build map from generic typevars to passed params
@@ -699,57 +745,68 @@
                 # Attempt to rebuild the origin in case new types have been defined
                 try:
                     # depth 3 gets you above this __class_getitem__ call
                     origin.model_rebuild(_parent_namespace_depth=3)
                 except PydanticUndefinedAnnotation:
                     # It's okay if it fails, it just means there are still undefined types
                     # that could be evaluated later.
-                    # TODO: Presumably we should error if validation is attempted here?
+                    # TODO: Make sure validation fails if there are still undefined types, perhaps using MockValidator
                     pass
 
                 submodel = _generics.create_generic_submodel(model_name, origin, args, params)
 
                 # Update cache
                 _generics.set_cached_generic_type(cls, typevar_values, submodel, origin, args)
 
         return submodel
 
     @classmethod
     def model_parametrized_name(cls, params: tuple[type[Any], ...]) -> str:
         """
         Compute class name for parametrizations of generic classes.
 
-        :param params: Tuple of types of the class . Given a generic class
-            `Model` with 2 type variables and a concrete model `Model[str, int]`,
-            the value `(str, int)` would be passed to `params`.
-        :return: String representing the new class where `params` are
-            passed to `cls` as type variables.
-
         This method can be overridden to achieve a custom naming scheme for generic BaseModels.
+
+        Args:
+            params (tuple[type[Any], ...]): Tuple of types of the class. Given a generic class
+                `Model` with 2 type variables and a concrete model `Model[str, int]`,
+                the value `(str, int)` would be passed to `params`.
+
+        Returns:
+            str: String representing the new class where `params` are passed to `cls` as type variables.
+
+        Raises:
+            TypeError: Raised when trying to generate concrete names for non-generic models.
         """
-        if not issubclass(cls, Generic):  # type: ignore[arg-type]
+        if not issubclass(cls, typing.Generic):  # type: ignore[arg-type]
             raise TypeError('Concrete names should only be generated for generic models.')
 
         # Any strings received should represent forward references, so we handle them specially below.
         # If we eventually move toward wrapping them in a ForwardRef in __class_getitem__ in the future,
         # we may be able to remove this special case.
         param_names = [param if isinstance(param, str) else _repr.display_as_type(param) for param in params]
         params_component = ', '.join(param_names)
         return f'{cls.__name__}[{params_component}]'
 
     # ##### Deprecated methods from v1 #####
     @property
-    @deprecated('The `__fields_set__` attribute is deprecated, use `model_fields_set` instead.')
+    @typing_extensions.deprecated('The `__fields__` attribute is deprecated, use `model_fields` instead.')
+    def __fields__(self) -> dict[str, FieldInfo]:
+        warnings.warn('The `__fields__` attribute is deprecated, use `model_fields` instead.', DeprecationWarning)
+        return self.model_fields
+
+    @property
+    @typing_extensions.deprecated('The `__fields_set__` attribute is deprecated, use `model_fields_set` instead.')
     def __fields_set__(self) -> set[str]:
         warnings.warn(
             'The `__fields_set__` attribute is deprecated, use `model_fields_set` instead.', DeprecationWarning
         )
         return self.__pydantic_fields_set__
 
-    @deprecated('The `dict` method is deprecated; use `model_dump` instead.')
+    @typing_extensions.deprecated('The `dict` method is deprecated; use `model_dump` instead.')
     def dict(
         self,
         *,
         include: IncEx = None,
         exclude: IncEx = None,
         by_alias: bool = False,
         exclude_unset: bool = False,
@@ -762,66 +819,64 @@
             exclude=exclude,
             by_alias=by_alias,
             exclude_unset=exclude_unset,
             exclude_defaults=exclude_defaults,
             exclude_none=exclude_none,
         )
 
-    @deprecated('The `json` method is deprecated; use `model_dump_json` instead.')
+    @typing_extensions.deprecated('The `json` method is deprecated; use `model_dump_json` instead.')
     def json(
         self,
         *,
         include: IncEx = None,
         exclude: IncEx = None,
         by_alias: bool = False,
         exclude_unset: bool = False,
         exclude_defaults: bool = False,
         exclude_none: bool = False,
-        # TODO: What do we do about the following arguments?
-        #   Do they need to go on model_config now, and get used by the serializer?
-        encoder: typing.Callable[[Any], Any] | None = Undefined,  # type: ignore[assignment]
-        models_as_dict: bool = Undefined,  # type: ignore[assignment]
+        encoder: typing.Callable[[Any], Any] | None = _Undefined,  # type: ignore[assignment]
+        models_as_dict: bool = _Undefined,  # type: ignore[assignment]
         **dumps_kwargs: Any,
     ) -> str:
         warnings.warn('The `json` method is deprecated; use `model_dump_json` instead.', DeprecationWarning)
-        if encoder is not Undefined:
+        if encoder is not _Undefined:
             raise TypeError('The `encoder` argument is no longer supported; use field serializers instead.')
-        if models_as_dict is not Undefined:
+        if models_as_dict is not _Undefined:
             raise TypeError('The `models_as_dict` argument is no longer supported; use a model serializer instead.')
         if dumps_kwargs:
             raise TypeError('`dumps_kwargs` keyword arguments are no longer supported.')
         return self.model_dump_json(
             include=include,
             exclude=exclude,
             by_alias=by_alias,
             exclude_unset=exclude_unset,
             exclude_defaults=exclude_defaults,
             exclude_none=exclude_none,
         )
 
     @classmethod
-    @deprecated('The `parse_obj` method is deprecated; use `model_validate` instead.')
+    @typing_extensions.deprecated('The `parse_obj` method is deprecated; use `model_validate` instead.')
     def parse_obj(cls: type[Model], obj: Any) -> Model:
         warnings.warn('The `parse_obj` method is deprecated; use `model_validate` instead.', DeprecationWarning)
         return cls.model_validate(obj)
 
     @classmethod
-    @deprecated(
+    @typing_extensions.deprecated(
         'The `parse_raw` method is deprecated; if your data is JSON use `model_validate_json`, '
         'otherwise load the data then use `model_validate` instead.'
     )
     def parse_raw(
         cls: type[Model],
         b: str | bytes,
         *,
         content_type: str | None = None,
         encoding: str = 'utf8',
         proto: _deprecated_parse.Protocol | None = None,
         allow_pickle: bool = False,
-    ) -> Model:
+    ) -> Model:  # pragma: no cover
         warnings.warn(
             'The `parse_raw` method is deprecated; if your data is JSON use `model_validate_json`, '
             'otherwise load the data then use `model_validate` instead.',
             DeprecationWarning,
         )
         try:
             obj = _deprecated_parse.load_str_bytes(
@@ -847,19 +902,19 @@
             # ctx is missing here, but since we've added `input` to the error, we're not pretending it's the same
             error: pydantic_core.InitErrorDetails = {
                 # The type: ignore on the next line is to ignore the requirement of LiteralString
                 'type': pydantic_core.PydanticCustomError(type_str, str(exc)),  # type: ignore
                 'loc': ('__root__',),
                 'input': b,
             }
-            raise pydantic_core.ValidationError(cls.__name__, [error])
+            raise pydantic_core.ValidationError.from_exception_data(cls.__name__, [error])
         return cls.model_validate(obj)
 
     @classmethod
-    @deprecated(
+    @typing_extensions.deprecated(
         'The `parse_file` method is deprecated; load the data from file, then if your data is JSON '
         'use `model_json_validate` otherwise `model_validate` instead.'
     )
     def parse_file(
         cls: type[Model],
         path: str | Path,
         *,
@@ -879,15 +934,15 @@
             content_type=content_type,
             encoding=encoding,
             allow_pickle=allow_pickle,
         )
         return cls.parse_obj(obj)
 
     @classmethod
-    # @deprecated(
+    # @typing_extensions.deprecated(
     #     "The `from_orm` method is deprecated; set "
     #     "`model_config['from_attributes']=True` and use `model_validate` instead."
     # )
     def from_orm(cls: type[Model], obj: Any) -> Model:
         warnings.warn(
             'The `from_orm` method is deprecated; set `model_config["from_attributes"]=True` '
             'and use `model_validate` instead.',
@@ -896,28 +951,28 @@
         if not cls.model_config.get('from_attributes', None):
             raise PydanticUserError(
                 'You must set the config attribute `from_attributes=True` to use from_orm', code=None
             )
         return cls.model_validate(obj)
 
     @classmethod
-    @deprecated('The `construct` method is deprecated; use `model_construct` instead.')
+    @typing_extensions.deprecated('The `construct` method is deprecated; use `model_construct` instead.')
     def construct(cls: type[Model], _fields_set: set[str] | None = None, **values: Any) -> Model:
         warnings.warn('The `construct` method is deprecated; use `model_construct` instead.', DeprecationWarning)
         return cls.model_construct(_fields_set=_fields_set, **values)
 
-    @deprecated('The copy method is deprecated; use `model_copy` instead.')
+    @typing_extensions.deprecated('The copy method is deprecated; use `model_copy` instead.')
     def copy(
         self: Model,
         *,
         include: AbstractSetIntStr | MappingIntStrAny | None = None,
         exclude: AbstractSetIntStr | MappingIntStrAny | None = None,
         update: typing.Dict[str, Any] | None = None,  # noqa UP006
         deep: bool = False,
-    ) -> Model:
+    ) -> Model:  # pragma: no cover
         """
         This method is now deprecated; use `model_copy` instead. If you need include / exclude, use:
 
             data = self.model_dump(include=include, exclude=exclude, round_trip=True)
             data = {**data, **(update or {})}
             copied = self.model_validate(data)
         """
@@ -929,14 +984,19 @@
 
         values = dict(
             _deprecated_copy_internals._iter(  # type: ignore
                 self, to_dict=False, by_alias=False, include=include, exclude=exclude, exclude_unset=False
             ),
             **(update or {}),
         )
+        if self.__pydantic_private__ is None:
+            private = None
+        else:
+            private = {k: v for k, v in self.__pydantic_private__.items() if v is not _Undefined}
+
         if self.__pydantic_extra__ is None:
             extra: dict[str, Any] | None = None
         else:
             extra = self.__pydantic_extra__.copy()
             for k in list(self.__pydantic_extra__):
                 if k not in values:  # k was in the exclude
                     extra.pop(k)
@@ -950,29 +1010,31 @@
         else:
             fields_set = set(self.__pydantic_fields_set__)
 
         # removing excluded fields from `__pydantic_fields_set__`
         if exclude:
             fields_set -= set(exclude)
 
-        return _deprecated_copy_internals._copy_and_set_values(self, values, fields_set, extra, deep=deep)
+        return _deprecated_copy_internals._copy_and_set_values(self, values, fields_set, extra, private, deep=deep)
 
     @classmethod
-    @deprecated('The `schema` method is deprecated; use `model_json_schema` instead.')
+    @typing_extensions.deprecated('The `schema` method is deprecated; use `model_json_schema` instead.')
     def schema(
         cls, by_alias: bool = True, ref_template: str = DEFAULT_REF_TEMPLATE
     ) -> typing.Dict[str, Any]:  # noqa UP006
         warnings.warn('The `schema` method is deprecated; use `model_json_schema` instead.', DeprecationWarning)
         return cls.model_json_schema(by_alias=by_alias, ref_template=ref_template)
 
     @classmethod
-    @deprecated('The `schema_json` method is deprecated; use `model_json_schema` and json.dumps instead.')
+    @typing_extensions.deprecated(
+        'The `schema_json` method is deprecated; use `model_json_schema` and json.dumps instead.'
+    )
     def schema_json(
         cls, *, by_alias: bool = True, ref_template: str = DEFAULT_REF_TEMPLATE, **dumps_kwargs: Any
-    ) -> str:
+    ) -> str:  # pragma: no cover
         import json
 
         warnings.warn(
             'The `schema_json` method is deprecated; use `model_json_schema` and json.dumps instead.',
             DeprecationWarning,
         )
         from .deprecated.json import pydantic_encoder
@@ -980,59 +1042,90 @@
         return json.dumps(
             cls.model_json_schema(by_alias=by_alias, ref_template=ref_template),
             default=pydantic_encoder,
             **dumps_kwargs,
         )
 
     @classmethod
-    @deprecated('The `validate` method is deprecated; use `model_validate` instead.')
+    @typing_extensions.deprecated('The `validate` method is deprecated; use `model_validate` instead.')
     def validate(cls: type[Model], value: Any) -> Model:
         warnings.warn('The `validate` method is deprecated; use `model_validate` instead.', DeprecationWarning)
         return cls.model_validate(value)
 
     @classmethod
-    @deprecated('The `update_forward_refs` method is deprecated; use `model_rebuild` instead.')
+    @typing_extensions.deprecated('The `update_forward_refs` method is deprecated; use `model_rebuild` instead.')
     def update_forward_refs(cls, **localns: Any) -> None:
         warnings.warn(
             'The `update_forward_refs` method is deprecated; use `model_rebuild` instead.', DeprecationWarning
         )
-        if localns:
+        if localns:  # pragma: no cover
             raise TypeError('`localns` arguments are not longer accepted.')
         cls.model_rebuild(force=True)
 
-    @deprecated('The private method `_iter` will be removed and should no longer be used.')
+    @typing_extensions.deprecated('The private method `_iter` will be removed and should no longer be used.')
     def _iter(self, *args: Any, **kwargs: Any) -> Any:
         warnings.warn('The private method `_iter` will be removed and should no longer be used.', DeprecationWarning)
         return _deprecated_copy_internals._iter(self, *args, **kwargs)  # type: ignore
 
-    @deprecated('The private method `_calculate_keys` will be removed and should no longer be used.')
+    @typing_extensions.deprecated(
+        'The private method `_copy_and_set_values` will be removed and should no longer be used.'
+    )
     def _copy_and_set_values(self, *args: Any, **kwargs: Any) -> Any:
         warnings.warn(
             'The private method  `_copy_and_set_values` will be removed and should no longer be used.',
             DeprecationWarning,
         )
         return _deprecated_copy_internals._copy_and_set_values(self, *args, **kwargs)  # type: ignore
 
     @classmethod
-    @deprecated('The private method `_get_value` will be removed and should no longer be used.')
+    @typing_extensions.deprecated('The private method `_get_value` will be removed and should no longer be used.')
     def _get_value(cls, *args: Any, **kwargs: Any) -> Any:
         warnings.warn(
             'The private method  `_get_value` will be removed and should no longer be used.', DeprecationWarning
         )
         return _deprecated_copy_internals._get_value(cls, *args, **kwargs)  # type: ignore
 
-    @deprecated('The private method `_calculate_keys` will be removed and should no longer be used.')
+    @typing_extensions.deprecated('The private method `_calculate_keys` will be removed and should no longer be used.')
     def _calculate_keys(self, *args: Any, **kwargs: Any) -> Any:
         warnings.warn(
             'The private method `_calculate_keys` will be removed and should no longer be used.', DeprecationWarning
         )
         return _deprecated_copy_internals._calculate_keys(self, *args, **kwargs)  # type: ignore
 
 
-_base_class_defined = True
+RootModelRootType = typing.TypeVar('RootModelRootType')
+
+
+class RootModel(BaseModel, typing.Generic[RootModelRootType]):
+    __pydantic_root_model__ = True
+    # TODO: Make `__pydantic_fields_set__` logic consistent with `BaseModel`, i.e. it should be `set()` if default value
+    # was used
+    __pydantic_fields_set__ = {'root'}  # It's fine having a set here as it will never change
+    __pydantic_private__ = None
+    __pydantic_extra__ = None
+
+    root: RootModelRootType
+
+    def __init__(__pydantic_self__, root: RootModelRootType) -> None:  # type: ignore
+        __tracebackhide__ = True
+        __pydantic_self__.__pydantic_validator__.validate_python(root, self_instance=__pydantic_self__)
+
+    __init__.__pydantic_base_init__ = True  # type: ignore
+
+    @classmethod
+    def model_construct(cls: type[Model], root: RootModelRootType, _fields_set: set[str] | None = None) -> Model:
+        return super().model_construct(root=root, _fields_set=_fields_set)
+
+    def __eq__(self, other: Any) -> bool:
+        if not isinstance(other, RootModel):
+            return NotImplemented
+        return self.model_fields['root'].annotation == other.model_fields['root'].annotation and super().__eq__(other)
+
+    def __repr_args__(self) -> _repr.ReprArgs:
+        yield 'root', self.root
 
 
 @typing.overload
 def create_model(
     __model_name: str,
     *,
     __config__: ConfigDict | None = None,
@@ -1067,54 +1160,57 @@
     __module__: str = __name__,
     __validators__: dict[str, AnyClassMethod] | None = None,
     __cls_kwargs__: dict[str, Any] | None = None,
     __slots__: tuple[str, ...] | None = None,
     **field_definitions: Any,
 ) -> type[Model]:
     """
-    Dynamically create a model.
-    :param __model_name: name of the created model
-    :param __config__: config dict/class to use for the new model
-    :param __base__: base class for the new model to inherit from
-    :param __module__: module of the created model
-    :param __validators__: a dict of method names and @validator class methods
-    :param __cls_kwargs__: a dict for class creation
-    :param __slots__: Deprecated, `__slots__` should not be passed to `create_model`
-    :param field_definitions: fields of the model (or extra fields if a base is supplied)
-        in the format `<name>=(<type>, <default value>)` or `<name>=<default value>, e.g.
-        `foobar=(str, ...)` or `foobar=123`, or, for complex use-cases, in the format
-        `<name>=<Field>` or `<name>=(<type>, <FieldInfo>)`, e.g.
-        `foo=Field(datetime, default_factory=datetime.utcnow, alias='bar')` or
-        `foo=(str, FieldInfo(title='Foo'))`
+    Dynamically creates and returns a new Pydantic Model.
+
+    Args:
+        __model_name (str): The name of the newly created model.
+        __config__ (Optional[ConfigDict]): The configuration of the new model.
+        __base__ (Optional[Union[type[Model], Tuple[type[Model]]]]): The base class for the new model.
+        __module__ (str): The name of the module that the model belongs to.
+        __validators__ (Optional[Dict[str, Union[Callable, ClassMethod]]]): A dictionary of methods that validate
+            fields.
+        __cls_kwargs__ (Optional[Dict[str, Any]]): A dictionary of keyword arguments for class creation.
+        __slots__ (Optional[Tuple[str]]): Deprecated. Should not be passed to `create_model`.
+        **field_definitions (Any): Attributes of the new model. They should be passed in the format:
+            `<name>=(<type>, <default value>)` or `<name>=<default value>`. For more complex cases, they can be
+            passed in the format: `<name>=<Field>` or `<name>=(<type>, <FieldInfo>)`.
+
+    Returns:
+        Model: The newly created Pydantic Model.
     """
     if __slots__ is not None:
         # __slots__ will be ignored from here on
         warnings.warn('__slots__ should not be passed to create_model', RuntimeWarning)
 
     if __base__ is not None:
         if __config__ is not None:
             raise PydanticUserError(
                 'to avoid confusion `__config__` and `__base__` cannot be used together',
                 code='create-model-config-base',
             )
         if not isinstance(__base__, tuple):
             __base__ = (__base__,)
     else:
-        __base__ = (cast(typing.Type['Model'], BaseModel),)
+        __base__ = (typing.cast(typing.Type['Model'], BaseModel),)
 
     __cls_kwargs__ = __cls_kwargs__ or {}
 
     fields = {}
     annotations = {}
 
     for f_name, f_def in field_definitions.items():
         if f_name.startswith('_'):
             warnings.warn(f'fields may not start with an underscore, ignoring "{f_name}"', RuntimeWarning)
         if isinstance(f_def, tuple):
-            f_def = cast('tuple[str, Any]', f_def)
+            f_def = typing.cast('tuple[str, Any]', f_def)
             try:
                 f_annotation, f_value = f_def
             except ValueError as e:
                 raise PydanticUserError(
                     'Field definitions should either be a `(<type>, <default>)`.',
                     code='create-model-field-definitions',
                 ) from e
@@ -1127,29 +1223,16 @@
 
     namespace: dict[str, Any] = {'__annotations__': annotations, '__module__': __module__}
     if __validators__:
         namespace.update(__validators__)
     namespace.update(fields)
     if __config__:
         namespace['model_config'] = _config.ConfigWrapper(__config__).config_dict
-    resolved_bases = resolve_bases(__base__)
-    meta, ns, kwds = prepare_class(__model_name, resolved_bases, kwds=__cls_kwargs__)
+    resolved_bases = types.resolve_bases(__base__)
+    meta, ns, kwds = types.prepare_class(__model_name, resolved_bases, kwds=__cls_kwargs__)
     if resolved_bases is not __base__:
         ns['__orig_bases__'] = __base__
     namespace.update(ns)
     return meta(__model_name, resolved_bases, namespace, __pydantic_reset_parent_namespace__=False, **kwds)
 
 
-def _collect_bases_data(bases: tuple[type[Any], ...]) -> tuple[set[str], set[str], dict[str, ModelPrivateAttr]]:
-    field_names: set[str] = set()
-    class_vars: set[str] = set()
-    private_attributes: dict[str, ModelPrivateAttr] = {}
-    for base in bases:
-        if _base_class_defined and issubclass(base, BaseModel) and base != BaseModel:
-            # model_fields might not be defined yet in the case of generics, so we use getattr here:
-            field_names.update(getattr(base, 'model_fields', {}).keys())
-            class_vars.update(base.__class_vars__)
-            private_attributes.update(base.__private_attributes__)
-    return field_names, class_vars, private_attributes
-
-
 __getattr__ = getattr_migration(__name__)
```

### Comparing `pydantic-2.0a4/pydantic/mypy.py` & `pydantic-2.0b1/pydantic/mypy.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,22 +73,24 @@
 except ImportError:  # pragma: no cover
     # Backward-compatible with TypeVarDef from Mypy 0.930.
     from mypy.types import TypeVarType as TypeVarDef
 
 CONFIGFILE_KEY = 'pydantic-mypy'
 METADATA_KEY = 'pydantic-mypy-metadata'
 BASEMODEL_FULLNAME = 'pydantic.main.BaseModel'
-MODEL_METACLASS_FULLNAME = 'pydantic.main.ModelMetaclass'
+MODEL_METACLASS_FULLNAME = 'pydantic._internal._model_construction.ModelMetaclass'
 FIELD_FULLNAME = 'pydantic.fields.Field'
 DATACLASS_FULLNAME = 'pydantic.dataclasses.dataclass'
 DECORATOR_FULLNAMES = {
-    'pydantic.decorators.validator',
-    'pydantic.decorators.field_validator',
-    'pydantic.decorators.root_validator',
-    'pydantic.decorators.serializer',
+    'pydantic.functional_validators.field_validator',
+    'pydantic.functional_validators.model_validator',
+    'pydantic.functional_serializers.serializer',
+    'pydantic.functional_serializers.model_serializer',
+    'pydantic.deprecated.class_validators.validator',
+    'pydantic.deprecated.class_validators.root_validator',
 }
 
 
 def parse_mypy_version(version: str) -> tuple[int, ...]:
     return tuple(map(int, version.partition('+')[0].split('.')))
 
 
@@ -535,16 +537,24 @@
         construct_arguments = self.get_field_arguments(fields, typed=True, force_all_optional=False, use_alias=False)
         construct_arguments = [fields_set_argument] + construct_arguments
 
         obj_type = ctx.api.named_type(f'{BUILTINS_NAME}.object')
         self_tvar_name = '_PydanticBaseModel'  # Make sure it does not conflict with other names in the class
         tvar_fullname = ctx.cls.fullname + '.' + self_tvar_name
         # requires mypy>0.910
-        self_type = TypeVarDef(self_tvar_name, tvar_fullname, -1, [], obj_type)
-        self_tvar_expr = TypeVarExpr(self_tvar_name, tvar_fullname, [], obj_type)
+        if MYPY_VERSION_TUPLE >= (1, 4):
+            self_type = TypeVarType(
+                self_tvar_name, tvar_fullname, -1, [], obj_type, AnyType(TypeOfAny.from_omitted_generics)
+            )
+            self_tvar_expr = TypeVarExpr(
+                self_tvar_name, tvar_fullname, [], obj_type, AnyType(TypeOfAny.from_omitted_generics)
+            )
+        else:
+            self_type = TypeVarDef(self_tvar_name, tvar_fullname, -1, [], obj_type)
+            self_tvar_expr = TypeVarExpr(self_tvar_name, tvar_fullname, [], obj_type)
         ctx.cls.info.names[self_tvar_name] = SymbolTableNode(MDEF, self_tvar_expr)
 
         add_method(
             ctx,
             'model_construct',
             construct_arguments,
             return_type=self_type,
```

### Comparing `pydantic-2.0a4/pydantic/networks.py` & `pydantic-2.0b1/pydantic/networks.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 import re
 from ipaddress import IPv4Address, IPv4Interface, IPv4Network, IPv6Address, IPv6Interface, IPv6Network
 from typing import TYPE_CHECKING, Any
 
 from pydantic_core import MultiHostUrl, PydanticCustomError, Url, core_schema
 from typing_extensions import Annotated, TypeAlias
 
-from ._internal import _fields, _repr
-from ._internal._schema_generation_shared import GetJsonSchemaHandler
+from ._internal import _fields, _repr, _schema_generation_shared
 from ._migration import getattr_migration
 from .json_schema import JsonSchemaValue
 
 if TYPE_CHECKING:
     import email_validator
 
     NetworkType: TypeAlias = 'str | bytes | int | tuple[str | bytes | int, str | int]'
@@ -152,15 +151,15 @@
             source: type[Any],
         ) -> core_schema.CoreSchema:
             import_email_validator()
             return core_schema.general_after_validator_function(cls.validate, core_schema.str_schema())
 
         @classmethod
         def __get_pydantic_json_schema__(
-            cls, core_schema: core_schema.CoreSchema, handler: GetJsonSchemaHandler
+            cls, core_schema: core_schema.CoreSchema, handler: _schema_generation_shared.GetJsonSchemaHandler
         ) -> JsonSchemaValue:
             field_schema = handler(core_schema)
             field_schema.update(type='string', format='email')
             return field_schema
 
         @classmethod
         def validate(cls, __input_value: str, _: core_schema.ValidationInfo) -> str:
@@ -175,15 +174,15 @@
         self.email = email
 
     def __eq__(self, other: Any) -> bool:
         return isinstance(other, NameEmail) and (self.name, self.email) == (other.name, other.email)
 
     @classmethod
     def __get_pydantic_json_schema__(
-        cls, core_schema: core_schema.CoreSchema, handler: GetJsonSchemaHandler
+        cls, core_schema: core_schema.CoreSchema, handler: _schema_generation_shared.GetJsonSchemaHandler
     ) -> JsonSchemaValue:
         field_schema = handler(core_schema)
         field_schema.update(type='string', format='name-email')
         return field_schema
 
     @classmethod
     def __get_pydantic_core_schema__(
@@ -221,15 +220,15 @@
         try:
             return IPv6Address(value)
         except ValueError:
             raise PydanticCustomError('ip_any_address', 'value is not a valid IPv4 or IPv6 address')
 
     @classmethod
     def __get_pydantic_json_schema__(
-        cls, core_schema: core_schema.CoreSchema, handler: GetJsonSchemaHandler
+        cls, core_schema: core_schema.CoreSchema, handler: _schema_generation_shared.GetJsonSchemaHandler
     ) -> JsonSchemaValue:
         field_schema = {}
         field_schema.update(type='string', format='ipvanyaddress')
         return field_schema
 
     @classmethod
     def __get_pydantic_core_schema__(
@@ -255,15 +254,15 @@
         try:
             return IPv6Interface(value)
         except ValueError:
             raise PydanticCustomError('ip_any_interface', 'value is not a valid IPv4 or IPv6 interface')
 
     @classmethod
     def __get_pydantic_json_schema__(
-        cls, core_schema: core_schema.CoreSchema, handler: GetJsonSchemaHandler
+        cls, core_schema: core_schema.CoreSchema, handler: _schema_generation_shared.GetJsonSchemaHandler
     ) -> JsonSchemaValue:
         field_schema = {}
         field_schema.update(type='string', format='ipvanyinterface')
         return field_schema
 
     @classmethod
     def __get_pydantic_core_schema__(
@@ -291,15 +290,15 @@
         try:
             return IPv6Network(value)
         except ValueError:
             raise PydanticCustomError('ip_any_network', 'value is not a valid IPv4 or IPv6 network')
 
     @classmethod
     def __get_pydantic_json_schema__(
-        cls, core_schema: core_schema.CoreSchema, handler: GetJsonSchemaHandler
+        cls, core_schema: core_schema.CoreSchema, handler: _schema_generation_shared.GetJsonSchemaHandler
     ) -> JsonSchemaValue:
         field_schema = {}
         field_schema.update(type='string', format='ipvanynetwork')
         return field_schema
 
     @classmethod
     def __get_pydantic_core_schema__(
```

### Comparing `pydantic-2.0a4/pydantic/type_adapter.py` & `pydantic-2.0b1/pydantic/type_adapter.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,30 @@
 """A class representing the type adapter."""
 from __future__ import annotations as _annotations
 
 import sys
+from dataclasses import is_dataclass
 from typing import TYPE_CHECKING, Any, Dict, Generic, Iterable, Set, TypeVar, Union, overload
 
-from pydantic_core import CoreSchema, SchemaSerializer, SchemaValidator
-from typing_extensions import Literal
+from pydantic_core import CoreSchema, SchemaSerializer, SchemaValidator, Some
+from typing_extensions import Literal, is_typeddict
 
-from ._internal import _config, _generate_schema, _typing_extra
-from ._internal._core_utils import flatten_schema_defs, inline_schema_defs
+from pydantic.errors import PydanticUserError
+from pydantic.main import BaseModel
+
+from ._internal import _config, _core_utils, _generate_schema, _typing_extra
 from .config import ConfigDict
-from .json_schema import DEFAULT_REF_TEMPLATE, GenerateJsonSchema
+from .json_schema import (
+    DEFAULT_REF_TEMPLATE,
+    DefsRef,
+    GenerateJsonSchema,
+    JsonSchemaKeyT,
+    JsonSchemaMode,
+    JsonSchemaValue,
+)
 
 T = TypeVar('T')
 
 if TYPE_CHECKING:
     # should be `set[int] | set[str] | dict[int, IncEx] | dict[str, IncEx] | None`, but mypy can't cope
     IncEx = Union[Set[int], Set[str], Dict[int, Any], Dict[str, Any]]
 
@@ -65,14 +75,31 @@
     local_ns = _typing_extra.parent_frame_namespace(parent_depth=parent_depth)
     global_ns = sys._getframe(max(parent_depth - 1, 1)).f_globals.copy()
     global_ns.update(local_ns or {})
     gen = _generate_schema.GenerateSchema(config_wrapper, types_namespace=global_ns, typevars_map={})
     return gen.generate_schema(type_)
 
 
+def _getattr_no_parents(obj: Any, attribute: str) -> Any:
+    """
+    Returns the attribute value without attempting to look up attributes from parent types
+    """
+    if hasattr(obj, '__dict__'):
+        try:
+            return obj.__dict__[attribute]
+        except KeyError:
+            pass
+
+    slots = getattr(obj, '__slots__', None)
+    if slots is not None and attribute in slots:
+        return getattr(obj, attribute)
+    else:
+        raise AttributeError(attribute)
+
+
 class TypeAdapter(Generic[T]):
     """A class representing the type adapter.
 
     Attributes:
         core_schema (CoreSchema): The core schema for the type.
         validator (SchemaValidator): The schema validator for the type.
         serializer (SchemaSerializer): The schema serializer for the type.
@@ -90,38 +117,53 @@
         @overload
         def __new__(cls, __type: T, *, config: ConfigDict | None = ...) -> TypeAdapter[T]:
             ...
 
         def __new__(cls, __type: Any, *, config: ConfigDict | None = ...) -> TypeAdapter[T]:
             raise NotImplementedError
 
-    def __init__(self, __type: Any, *, config: ConfigDict | None = None, _parent_depth: int = 2) -> None:
+    def __init__(self, type: Any, *, config: ConfigDict | None = None, _parent_depth: int = 2) -> None:
         """Initializes the TypeAdapter object."""
         config_wrapper = _config.ConfigWrapper(config)
 
+        try:
+            type_has_config = issubclass(type, BaseModel) or is_dataclass(type) or is_typeddict(type)
+        except TypeError:
+            # type is not a class
+            type_has_config = False
+
+        if type_has_config and config is not None:
+            raise PydanticUserError(
+                'Cannot use `config` when the type is a BaseModel, dataclass or TypedDict.'
+                ' These types can have their own config and setting the config via the `config`'
+                ' parameter to TypeAdapter will not override it, thus the `config` you passed to'
+                ' TypeAdapter becomes meaningless, which is probably not what you want.',
+                code='type-adapter-config-unused',
+            )
+
         core_schema: CoreSchema
         try:
-            core_schema = __type.__pydantic_core_schema__
+            core_schema = _getattr_no_parents(type, '__pydantic_core_schema__')
         except AttributeError:
-            core_schema = _get_schema(__type, config_wrapper, parent_depth=_parent_depth + 1)
+            core_schema = _get_schema(type, config_wrapper, parent_depth=_parent_depth + 1)
 
-        core_schema = flatten_schema_defs(core_schema)
-        simplified_core_schema = inline_schema_defs(core_schema)
+        core_schema = _core_utils.flatten_schema_defs(core_schema)
+        simplified_core_schema = _core_utils.inline_schema_defs(core_schema)
 
-        core_config = config_wrapper.core_config()
+        core_config = config_wrapper.core_config(None)
         validator: SchemaValidator
-        if hasattr(__type, '__pydantic_validator__') and config is None:
-            validator = __type.__pydantic_validator__
-        else:
+        try:
+            validator = _getattr_no_parents(type, '__pydantic_validator__')
+        except AttributeError:
             validator = SchemaValidator(simplified_core_schema, core_config)
 
         serializer: SchemaSerializer
-        if hasattr(__type, '__pydantic_serializer__') and config is None:
-            serializer = __type.__pydantic_serializer__
-        else:
+        try:
+            serializer = _getattr_no_parents(type, '__pydantic_serializer__')
+        except AttributeError:
             serializer = SchemaSerializer(simplified_core_schema, core_config)
 
         self.core_schema = core_schema
         self.validator = validator
         self.serializer = serializer
 
     def validate_python(self, __object: Any, *, strict: bool | None = None, context: dict[str, Any] | None = None) -> T:
@@ -151,14 +193,26 @@
 
         Returns:
             T: The validated object.
 
         """
         return self.validator.validate_json(__data, strict=strict, context=context)
 
+    def get_default_value(self, *, strict: bool | None = None, context: dict[str, Any] | None = None) -> Some[T] | None:
+        """Get the default value for this model / type.
+
+        Args:
+            strict (bool | None, optional): Whether to strictly check types. Defaults to None.
+            context (dict[str, Any] | None, optional): Additional context to use during validation. Defaults to None.
+
+        Returns:
+            Some[T] | None: The default value wrapped in a Some if there is one or None if not.
+        """
+        return self.validator.get_default_value(strict=strict, context=context)
+
     def dump_python(
         self,
         __instance: T,
         *,
         mode: Literal['json', 'python'] = 'python',
         include: IncEx | None = None,
         exclude: IncEx | None = None,
@@ -248,62 +302,66 @@
 
     def json_schema(
         self,
         *,
         by_alias: bool = True,
         ref_template: str = DEFAULT_REF_TEMPLATE,
         schema_generator: type[GenerateJsonSchema] = GenerateJsonSchema,
+        mode: JsonSchemaMode = 'validation',
     ) -> dict[str, Any]:
         """Generate a JSON schema for the model.
 
         Args:
             by_alias (bool): Whether to use alias names (default: True).
             ref_template (str): The format string used for generating $ref strings (default: DEFAULT_REF_TEMPLATE).
             schema_generator (Type[GenerateJsonSchema]): The generator class used for creating the schema
                 (default: GenerateJsonSchema).
 
         Returns:
             Dict[str, Any]: The JSON schema for the model as a dictionary.
         """
         schema_generator_instance = schema_generator(by_alias=by_alias, ref_template=ref_template)
-        return schema_generator_instance.generate(self.core_schema)
+        return schema_generator_instance.generate(self.core_schema, mode=mode)
 
     @staticmethod
     def json_schemas(
-        __types: Iterable[TypeAdapter[Any]],
+        __inputs: Iterable[tuple[JsonSchemaKeyT, JsonSchemaMode, TypeAdapter[Any]]],
         *,
         by_alias: bool = True,
-        ref_template: str = DEFAULT_REF_TEMPLATE,
         title: str | None = None,
         description: str | None = None,
+        ref_template: str = DEFAULT_REF_TEMPLATE,
         schema_generator: type[GenerateJsonSchema] = GenerateJsonSchema,
-    ) -> dict[str, Any]:
-        """Generate JSON schemas for multiple models.
+    ) -> tuple[dict[tuple[JsonSchemaKeyT, JsonSchemaMode], DefsRef], JsonSchemaValue]:
+        """Generate JSON schemas for multiple type adapters.
 
         Args:
-            __types (Iterable[TypeAdapter[Any]]): The types to generate schemas for.
+            __inputs (Iterable[tuple[JsonSchemaKeyT, JsonSchemaMode, TypeAdapter[Any]]]): Inputs to schema generation.
+                The first two items will form the keys of the (first) output mapping; the type adapters will provide
+                the core schemas that get converted into definitions in the output JSON schema.
             by_alias (bool): Whether to use alias names (default: True).
-            ref_template (str): The format string used for generating $ref strings (default: DEFAULT_REF_TEMPLATE).
             title (Optional[str]): The title for the schema (default: None).
             description (Optional[str]): The description for the schema (default: None).
+            ref_template (str): The format string used for generating $ref strings (default: DEFAULT_REF_TEMPLATE).
             schema_generator (Type[GenerateJsonSchema]): The generator class used for creating the
                 schema (default: GenerateJsonSchema).
 
         Returns:
-            Dict[str, Any]: The JSON schema for the models as a dictionary.
+            tuple[dict[tuple[Hashable, JsonSchemaMode], DefsRef], JsonSchemaValue]:
+                The first item contains the mapping of key + mode to a definitions reference, which will be a key
+                of the $defs mapping in the JSON schema included as the second member of the returned tuple.
         """
-        # TODO: can we use model.__schema_cache__?
         schema_generator_instance = schema_generator(by_alias=by_alias, ref_template=ref_template)
 
-        core_schemas = [at.core_schema for at in __types]
+        inputs = [(key, mode, adapter.core_schema) for key, mode, adapter in __inputs]
 
-        definitions = schema_generator_instance.generate_definitions(core_schemas)
+        key_map, definitions = schema_generator_instance.generate_definitions(inputs)
 
         json_schema: dict[str, Any] = {}
         if definitions:
             json_schema['$defs'] = definitions
         if title:
             json_schema['title'] = title
         if description:
             json_schema['description'] = description
 
-        return json_schema
+        return key_map, json_schema
```

### Comparing `pydantic-2.0a4/pydantic/types.py` & `pydantic-2.0b1/pydantic/types.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import base64
 import dataclasses as _dataclasses
 import re
 from datetime import date, datetime
 from decimal import Decimal
 from enum import Enum
 from pathlib import Path
+from types import ModuleType
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     ClassVar,
     FrozenSet,
     Generic,
@@ -20,24 +21,33 @@
     Set,
     TypeVar,
     cast,
 )
 from uuid import UUID
 
 import annotated_types
-from pydantic_core import CoreSchema, PydanticCustomError, PydanticKnownError, core_schema
+from pydantic_core import CoreSchema, PydanticCustomError, PydanticKnownError, PydanticOmit, core_schema
 from typing_extensions import Annotated, Literal, Protocol
 
-from ._internal import _fields, _internal_dataclass, _known_annotated_metadata, _validators
-from ._internal._internal_dataclass import slots_dataclass
+from ._internal import (
+    _annotated_handlers,
+    _core_metadata,
+    _fields,
+    _generics,
+    _internal_dataclass,
+    _known_annotated_metadata,
+    _utils,
+    _validators,
+)
 from ._migration import getattr_migration
-from .annotated import GetCoreSchemaHandler
+from .config import ConfigDict
 from .errors import PydanticUserError
+from .json_schema import JsonSchemaValue
 
-__all__ = [
+__all__ = (
     'Strict',
     'StrictStr',
     'conbytes',
     'conlist',
     'conset',
     'confrozenset',
     'constr',
@@ -69,29 +79,30 @@
     'StrictBytes',
     'StrictInt',
     'StrictFloat',
     'PaymentCardNumber',
     'ByteSize',
     'PastDate',
     'FutureDate',
+    'PastDatetime',
+    'FutureDatetime',
     'condate',
     'AwareDatetime',
     'NaiveDatetime',
     'AllowInfNan',
     'EncoderProtocol',
     'EncodedBytes',
     'EncodedStr',
     'Base64Encoder',
     'Base64Bytes',
     'Base64Str',
-]
-
-from ._internal._schema_generation_shared import GetJsonSchemaHandler
-from ._internal._utils import update_not_none
-from .json_schema import JsonSchemaValue
+    'SkipValidation',
+    'InstanceOf',
+    'WithJsonSchema',
+)
 
 
 @_dataclasses.dataclass
 class Strict(_fields.PydanticMetadata):
     strict: bool = True
 
     def __hash__(self) -> int:
@@ -258,15 +269,15 @@
     """
     if unique_items is not None:
         raise PydanticUserError(
             (
                 '`unique_items` is removed, use `Set` instead'
                 '(this feature is discussed in https://github.com/pydantic/pydantic-core/issues/296)'
             ),
-            code='deprecated_kwargs',
+            code='deprecated-kwargs',
         )
     return Annotated[  # type: ignore[return-value]
         List[item_type],  # type: ignore[valid-type]
         annotated_types.Len(min_length or 0, max_length),
     ]
 
 
@@ -280,24 +291,36 @@
     class ImportString:
         @classmethod
         def __class_getitem__(cls, item: AnyType) -> AnyType:
             return Annotated[item, cls()]
 
         @classmethod
         def __get_pydantic_core_schema__(
-            cls, source: type[Any], handler: GetCoreSchemaHandler
+            cls, source: type[Any], handler: _annotated_handlers.GetCoreSchemaHandler
         ) -> core_schema.CoreSchema:
+            serializer = core_schema.plain_serializer_function_ser_schema(cls._serialize, when_used='json')
             if cls is source:
                 # Treat bare usage of ImportString (`schema is None`) as the same as ImportString[Any]
-                return core_schema.general_plain_validator_function(lambda v, _: _validators.import_string(v))
+                return core_schema.no_info_plain_validator_function(
+                    function=_validators.import_string, serialization=serializer
+                )
             else:
-                return core_schema.general_before_validator_function(
-                    lambda v, _: _validators.import_string(v), handler(source)
+                return core_schema.no_info_before_validator_function(
+                    function=_validators.import_string, schema=handler(source), serialization=serializer
                 )
 
+        @staticmethod
+        def _serialize(v: Any) -> str:
+            if isinstance(v, ModuleType):
+                return v.__name__
+            elif hasattr(v, '__module__') and hasattr(v, '__name__'):
+                return f'{v.__module__}.{v.__name__}'
+            else:
+                return v
+
         def __repr__(self) -> str:
             return 'ImportString'
 
 
 # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ DECIMAL TYPES ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 
@@ -327,22 +350,24 @@
 
 
 @_internal_dataclass.slots_dataclass
 class UuidVersion:
     uuid_version: Literal[1, 3, 4, 5]
 
     def __get_pydantic_json_schema__(
-        self, core_schema: core_schema.CoreSchema, handler: GetJsonSchemaHandler
+        self, core_schema: core_schema.CoreSchema, handler: _annotated_handlers.GetJsonSchemaHandler
     ) -> JsonSchemaValue:
         field_schema = handler(core_schema)
         field_schema.pop('anyOf', None)  # remove the bytes/str union
         field_schema.update(type='string', format=f'uuid{self.uuid_version}')
         return field_schema
 
-    def __get_pydantic_core_schema__(self, source: Any, handler: GetCoreSchemaHandler) -> core_schema.CoreSchema:
+    def __get_pydantic_core_schema__(
+        self, source: Any, handler: _annotated_handlers.GetCoreSchemaHandler
+    ) -> core_schema.CoreSchema:
         return core_schema.general_after_validator_function(
             cast(core_schema.GeneralValidatorFunction, self.validate), handler(source)
         )
 
     def validate(self, value: UUID, _: core_schema.ValidationInfo) -> UUID:
         if value.version != self.uuid_version:
             raise PydanticCustomError(
@@ -364,22 +389,24 @@
 
 
 @_dataclasses.dataclass
 class PathType:
     path_type: Literal['file', 'dir', 'new']
 
     def __get_pydantic_json_schema__(
-        self, core_schema: core_schema.CoreSchema, handler: GetJsonSchemaHandler
+        self, core_schema: core_schema.CoreSchema, handler: _annotated_handlers.GetJsonSchemaHandler
     ) -> JsonSchemaValue:
         field_schema = handler(core_schema)
         format_conversion = {'file': 'file-path', 'dir': 'directory-path'}
         field_schema.update(format=format_conversion.get(self.path_type, 'path'), type='string')
         return field_schema
 
-    def __get_pydantic_core_schema__(self, source: Any, handler: GetCoreSchemaHandler) -> core_schema.CoreSchema:
+    def __get_pydantic_core_schema__(
+        self, source: Any, handler: _annotated_handlers.GetCoreSchemaHandler
+    ) -> core_schema.CoreSchema:
         function_lookup = {
             'file': cast(core_schema.GeneralValidatorFunction, self.validate_file),
             'dir': cast(core_schema.GeneralValidatorFunction, self.validate_directory),
             'new': cast(core_schema.GeneralValidatorFunction, self.validate_new),
         }
 
         return core_schema.general_after_validator_function(
@@ -400,15 +427,15 @@
             return path
         else:
             raise PydanticCustomError('path_not_directory', 'Path does not point to a directory')
 
     @staticmethod
     def validate_new(path: Path, _: core_schema.ValidationInfo) -> Path:
         if path.exists():
-            raise PydanticCustomError('path_exists', 'path already exists')
+            raise PydanticCustomError('path_exists', 'Path already exists')
         elif not path.parent.exists():
             raise PydanticCustomError('parent_does_not_exist', 'Parent directory does not exist')
         else:
             return path
 
     def __hash__(self) -> int:
         return hash(type(self.path_type))
@@ -428,15 +455,17 @@
 
     class Json:
         @classmethod
         def __class_getitem__(cls, item: AnyType) -> AnyType:
             return Annotated[item, cls()]
 
         @classmethod
-        def __get_pydantic_core_schema__(cls, source: Any, handler: GetCoreSchemaHandler) -> core_schema.CoreSchema:
+        def __get_pydantic_core_schema__(
+            cls, source: Any, handler: _annotated_handlers.GetCoreSchemaHandler
+        ) -> core_schema.CoreSchema:
             if cls is source:
                 return core_schema.json_schema(None)
             else:
                 return core_schema.json_schema(handler(source))
 
         def __repr__(self) -> str:
             return 'Json'
@@ -457,20 +486,26 @@
     def __init__(self, secret_value: SecretType) -> None:
         self._secret_value: SecretType = secret_value
 
     def get_secret_value(self) -> SecretType:
         return self._secret_value
 
     @classmethod
-    def __prepare_pydantic_annotations__(cls, source: type[Any], annotations: Iterable[Any]) -> Iterable[Any]:
+    def __prepare_pydantic_annotations__(
+        cls, source: type[Any], annotations: tuple[Any, ...], _config: ConfigDict
+    ) -> tuple[Any, Iterable[Any]]:
         metadata, remaining_annotations = _known_annotated_metadata.collect_known_metadata(annotations)
         _known_annotated_metadata.check_metadata(metadata, {'min_length', 'max_length'}, cls)
-        yield cls
-        yield _SecretFieldValidator(source, **metadata)
-        yield from remaining_annotations
+        return (
+            source,
+            (
+                _SecretFieldValidator(source, **metadata),
+                *remaining_annotations,
+            ),
+        )
 
     def __eq__(self, other: Any) -> bool:
         return isinstance(other, self.__class__) and self.get_secret_value() == other.get_secret_value()
 
     def __hash__(self) -> int:
         return hash(self.get_secret_value())
 
@@ -489,15 +524,15 @@
 
 def _secret_display(value: str | bytes) -> str:
     if isinstance(value, bytes):
         value = value.decode()
     return '**********' if value else ''
 
 
-@slots_dataclass
+@_internal_dataclass.slots_dataclass
 class _SecretFieldValidator:
     field_type: type[SecretField[Any]]
     min_length: int | None = None
     max_length: int | None = None
     inner_schema: CoreSchema = _dataclasses.field(init=False)
 
     def validate(self, value: SecretField[SecretType] | SecretType, _: core_schema.ValidationInfo) -> Any:
@@ -521,42 +556,47 @@
             # we want the output to always be string without the `b'` prefix for bytes,
             # hence we just use `secret_display`
             return _secret_display(value.get_secret_value())
         else:
             return value
 
     def __get_pydantic_json_schema__(
-        self, _core_schema: core_schema.CoreSchema, handler: GetJsonSchemaHandler
+        self, _core_schema: core_schema.CoreSchema, handler: _annotated_handlers.GetJsonSchemaHandler
     ) -> JsonSchemaValue:
         schema = self.inner_schema.copy()
         if self.min_length is not None:
             schema['min_length'] = self.min_length  # type: ignore
         if self.max_length is not None:
             schema['max_length'] = self.max_length  # type: ignore
         json_schema = handler(schema)
-        update_not_none(
+        _utils.update_not_none(
             json_schema,
             type='string',
             writeOnly=True,
             format='password',
         )
         return json_schema
 
-    def __get_pydantic_core_schema__(self, source: type[Any], handler: GetCoreSchemaHandler) -> core_schema.CoreSchema:
+    def __get_pydantic_core_schema__(
+        self, source: type[Any], handler: _annotated_handlers.GetCoreSchemaHandler
+    ) -> core_schema.CoreSchema:
         self.inner_schema = handler(str if self.field_type is SecretStr else bytes)
         error_kind = 'string_type' if self.field_type is SecretStr else 'bytes_type'
         return core_schema.general_after_validator_function(
             self.validate,
             core_schema.union_schema(
                 [core_schema.is_instance_schema(self.field_type), self.inner_schema],
                 strict=True,
                 custom_error_type=error_kind,
             ),
             serialization=core_schema.plain_serializer_function_ser_schema(
-                self.serialize, info_arg=True, json_return_type='str'
+                self.serialize,
+                info_arg=True,
+                return_schema=core_schema.str_schema(),
+                when_used='json',
             ),
         )
 
 
 class SecretStr(SecretField[str]):
     def _display(self) -> str:
         return _secret_display(self.get_secret_value())
@@ -598,15 +638,17 @@
         card_number = self.validate_luhn_check_digit(card_number)
 
         self.bin = card_number[:6]
         self.last4 = card_number[-4:]
         self.brand = self.validate_brand(card_number)
 
     @classmethod
-    def __get_pydantic_core_schema__(cls, source: type[Any], handler: GetCoreSchemaHandler) -> core_schema.CoreSchema:
+    def __get_pydantic_core_schema__(
+        cls, source: type[Any], handler: _annotated_handlers.GetCoreSchemaHandler
+    ) -> core_schema.CoreSchema:
         return core_schema.general_after_validator_function(
             cls.validate,
             core_schema.str_schema(
                 min_length=cls.min_length, max_length=cls.max_length, strip_whitespace=cls.strip_whitespace
             ),
         )
 
@@ -700,16 +742,17 @@
 }
 BYTE_SIZES.update({k.lower()[0]: v for k, v in BYTE_SIZES.items() if 'i' not in k})
 byte_string_re = re.compile(r'^\s*(\d*\.?\d+)\s*(\w+)?', re.IGNORECASE)
 
 
 class ByteSize(int):
     @classmethod
-    def __get_pydantic_core_schema__(cls, source: type[Any], handler: GetCoreSchemaHandler) -> core_schema.CoreSchema:
-        # TODO better schema
+    def __get_pydantic_core_schema__(
+        cls, source: type[Any], handler: _annotated_handlers.GetCoreSchemaHandler
+    ) -> core_schema.CoreSchema:
         return core_schema.general_plain_validator_function(cls.validate)
 
     @classmethod
     def validate(cls, __input_value: Any, _: core_schema.ValidationInfo) -> ByteSize:
         try:
             return cls(int(__input_value))
         except ValueError:
@@ -758,47 +801,53 @@
             raise PydanticCustomError('byte_size_unit', 'Could not interpret byte unit: {unit}', {'unit': unit})
 
         return self / unit_div
 
 
 # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ DATE TYPES ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
+
+def _check_annotated_type(annotated_type: str, expected_type: str, annotation: str) -> None:
+    if annotated_type != expected_type:
+        raise PydanticUserError(f"'{annotation}' cannot annotate '{annotated_type}'.", code='invalid_annotated_type')
+
+
 if TYPE_CHECKING:
     PastDate = Annotated[date, ...]
     FutureDate = Annotated[date, ...]
 else:
 
     class PastDate:
         @classmethod
         def __get_pydantic_core_schema__(
-            cls, source: type[Any], handler: GetCoreSchemaHandler
+            cls, source: type[Any], handler: _annotated_handlers.GetCoreSchemaHandler
         ) -> core_schema.CoreSchema:
             if cls is source:
                 # used directly as a type
                 return core_schema.date_schema(now_op='past')
             else:
                 schema = handler(source)
-                assert schema['type'] == 'date'
+                _check_annotated_type(schema['type'], 'date', cls.__name__)
                 schema['now_op'] = 'past'
                 return schema
 
         def __repr__(self) -> str:
             return 'PastDate'
 
     class FutureDate:
         @classmethod
         def __get_pydantic_core_schema__(
-            cls, source: type[Any], handler: GetCoreSchemaHandler
+            cls, source: type[Any], handler: _annotated_handlers.GetCoreSchemaHandler
         ) -> core_schema.CoreSchema:
             if cls is source:
                 # used directly as a type
                 return core_schema.date_schema(now_op='future')
             else:
                 schema = handler(source)
-                assert schema['type'] == 'date'
+                _check_annotated_type(schema['type'], 'date', cls.__name__)
                 schema['now_op'] = 'future'
                 return schema
 
         def __repr__(self) -> str:
             return 'FutureDate'
 
 
@@ -818,50 +867,87 @@
 
 
 # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ DATETIME TYPES ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 if TYPE_CHECKING:
     AwareDatetime = Annotated[datetime, ...]
     NaiveDatetime = Annotated[datetime, ...]
+    PastDatetime = Annotated[datetime, ...]
+    FutureDatetime = Annotated[datetime, ...]
+
 else:
 
     class AwareDatetime:
         @classmethod
         def __get_pydantic_core_schema__(
-            cls, source: type[Any], handler: GetCoreSchemaHandler
+            cls, source: type[Any], handler: _annotated_handlers.GetCoreSchemaHandler
         ) -> core_schema.CoreSchema:
             if cls is source:
                 # used directly as a type
                 return core_schema.datetime_schema(tz_constraint='aware')
             else:
                 schema = handler(source)
-                assert schema['type'] == 'datetime'
+                _check_annotated_type(schema['type'], 'datetime', cls.__name__)
                 schema['tz_constraint'] = 'aware'
                 return schema
 
         def __repr__(self) -> str:
             return 'AwareDatetime'
 
     class NaiveDatetime:
         @classmethod
         def __get_pydantic_core_schema__(
-            cls, source: type[Any], handler: GetCoreSchemaHandler
+            cls, source: type[Any], handler: _annotated_handlers.GetCoreSchemaHandler
         ) -> core_schema.CoreSchema:
             if cls is source:
                 # used directly as a type
                 return core_schema.datetime_schema(tz_constraint='naive')
             else:
                 schema = handler(source)
-                assert schema['type'] == 'datetime'
+                _check_annotated_type(schema['type'], 'datetime', cls.__name__)
                 schema['tz_constraint'] = 'naive'
                 return schema
 
         def __repr__(self) -> str:
             return 'NaiveDatetime'
 
+    class PastDatetime:
+        @classmethod
+        def __get_pydantic_core_schema__(
+            cls, source: type[Any], handler: _annotated_handlers.GetCoreSchemaHandler
+        ) -> core_schema.CoreSchema:
+            if cls is source:
+                # used directly as a type
+                return core_schema.datetime_schema(now_op='past')
+            else:
+                schema = handler(source)
+                _check_annotated_type(schema['type'], 'datetime', cls.__name__)
+                schema['now_op'] = 'past'
+                return schema
+
+        def __repr__(self) -> str:
+            return 'PastDatetime'
+
+    class FutureDatetime:
+        @classmethod
+        def __get_pydantic_core_schema__(
+            cls, source: type[Any], handler: _annotated_handlers.GetCoreSchemaHandler
+        ) -> core_schema.CoreSchema:
+            if cls is source:
+                # used directly as a type
+                return core_schema.datetime_schema(now_op='future')
+            else:
+                schema = handler(source)
+                _check_annotated_type(schema['type'], 'datetime', cls.__name__)
+                schema['now_op'] = 'future'
+                return schema
+
+        def __repr__(self) -> str:
+            return 'FutureDatetime'
+
 
 # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ Encoded TYPES ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 
 class EncoderProtocol(Protocol):
     @classmethod
     def decode(cls, data: bytes) -> bytes:
@@ -895,15 +981,15 @@
 
 
 @_internal_dataclass.slots_dataclass
 class EncodedBytes:
     encoder: type[EncoderProtocol]
 
     def __get_pydantic_json_schema__(
-        self, core_schema: core_schema.CoreSchema, handler: GetJsonSchemaHandler
+        self, core_schema: core_schema.CoreSchema, handler: _annotated_handlers.GetJsonSchemaHandler
     ) -> JsonSchemaValue:
         field_schema = handler(core_schema)
         field_schema.update(type='string', format=self.encoder.get_json_format())
         return field_schema
 
     def __get_pydantic_core_schema__(
         self, source: type[Any], handler: Callable[[Any], core_schema.CoreSchema]
@@ -940,8 +1026,109 @@
     def encode_str(self, value: str) -> str:
         return super().encode(value=value.encode()).decode()
 
 
 Base64Bytes = Annotated[bytes, EncodedBytes(encoder=Base64Encoder)]
 Base64Str = Annotated[str, EncodedStr(encoder=Base64Encoder)]
 
+
+if TYPE_CHECKING:
+    # If we add configurable attributes to IsInstance, we'd probably need to stop hiding it from type checkers like this
+    InstanceOf = Annotated[AnyType, ...]  # `IsInstance[Sequence]` will be recognized by type checkers as `Sequence`
+
+else:
+
+    @_internal_dataclass.slots_dataclass
+    class InstanceOf:
+        @classmethod
+        def __class_getitem__(cls, item: AnyType) -> AnyType:
+            return Annotated[item, cls()]
+
+        @classmethod
+        def __get_pydantic_core_schema__(
+            cls, source: Any, handler: _annotated_handlers.GetCoreSchemaHandler
+        ) -> core_schema.CoreSchema:
+            from pydantic import PydanticSchemaGenerationError
+
+            # use the generic _origin_ as the second argument to isinstance when appropriate
+            python_schema = core_schema.is_instance_schema(_generics.get_origin(source) or source)
+
+            try:
+                # Try to generate the "standard" schema, which will be used when loading from JSON
+                json_schema = handler(source)
+            except PydanticSchemaGenerationError:
+                # If that fails, just produce a schema that can validate from python
+                return python_schema
+            else:
+                return core_schema.json_or_python_schema(python_schema=python_schema, json_schema=json_schema)
+
+
 __getattr__ = getattr_migration(__name__)
+
+
+@_internal_dataclass.slots_dataclass
+class WithJsonSchema:
+    """
+    Add this as an annotation on a field to override the (base) JSON schema that would be generated for that field.
+
+    This provides a way to set a JSON schema for types that would otherwise raise errors when producing a JSON schema,
+    such as Callable, or types that have an is-instance core schema, without needing to go so far as creating a
+    custom subclass of pydantic.json_schema.GenerateJsonSchema.
+
+    Note that any _modifications_ to the schema that would normally be made (such as setting the title for model fields)
+    will still be performed.
+    """
+
+    json_schema: JsonSchemaValue | None
+
+    def __get_pydantic_json_schema__(
+        self, _core_schema: core_schema.CoreSchema, handler: _annotated_handlers.GetJsonSchemaHandler
+    ) -> JsonSchemaValue:
+        if self.json_schema is None:
+            # This exception is handled in pydantic.json_schema.GenerateJsonSchema._named_required_fields_schema
+            raise PydanticOmit
+        else:
+            return self.json_schema
+
+
+if TYPE_CHECKING:
+    SkipValidation = Annotated[AnyType, ...]  # SkipValidation[list[str]] will be treated by type checkers as list[str]
+else:
+
+    @_internal_dataclass.slots_dataclass
+    class SkipValidation:
+        """
+        If this is applied as an annotation (e.g., via `x: Annotated[int, SkipValidation]`), validation will be skipped.
+        You can also use `SkipValidation[int]` as a shorthand for `Annotated[int, SkipValidation]`.
+
+        This can be useful if you want to use a type annotation for documentation/IDE/type-checking purposes,
+        and know that it is safe to skip validation for one or more of the fields.
+
+        Because this converts the validation schema to `any_schema`, subsequent annotation-applied transformations
+        may not have the expected effects. Therefore, when used, this annotation should generally be the final
+        annotation applied to a type.
+        """
+
+        def __class_getitem__(cls, item: Any) -> Any:
+            return Annotated[item, SkipValidation()]
+
+        @classmethod
+        def __get_pydantic_core_schema__(
+            cls, source: Any, handler: _annotated_handlers.GetCoreSchemaHandler
+        ) -> core_schema.CoreSchema:
+            original_schema = handler.generate_schema(source)
+            metadata = _core_metadata.build_metadata_dict(js_functions=[lambda _c, h: h(original_schema)])
+            return core_schema.any_schema(metadata=metadata, serialization=original_schema)
+
+
+@_internal_dataclass.slots_dataclass
+class TransformSchema:
+    """
+    An annotation that can be used to apply a transform to a core schema.
+    """
+
+    transform: Callable[[CoreSchema], CoreSchema]
+
+    def __get_pydantic_core_schema__(
+        self, source_type: type[Any], handler: _annotated_handlers.GetCoreSchemaHandler
+    ) -> CoreSchema:
+        return self.transform(handler(source_type))
```

### Comparing `pydantic-2.0a4/pydantic/validate_call.py` & `pydantic-2.0b1/pydantic/validate_call.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,20 +31,20 @@
     config: ConfigDict | None = None,
     validate_return: bool = False,
 ) -> AnyCallableT | Callable[[AnyCallableT], AnyCallableT]:
     """
     Decorator to validate the arguments passed to a function and, optionally, the return value.
 
     Args:
-        __func (AnyCallableT): The function to be decorated.
-        config (ConfigDict): The configuration dictionary.
-        validate_return (bool): Whether to validate the return value.
+        __func: The function to be decorated.
+        config: The configuration dictionary.
+        validate_return: Whether to validate the return value.
 
     Returns:
-        Callable: The decorated function.
+        The decorated function.
     """
 
     def validate(function: AnyCallableT) -> AnyCallableT:
         return _validate_call.ValidateCallWrapper(function, config, validate_return)  # type: ignore
 
     if __func:
         return validate(__func)
```

### Comparing `pydantic-2.0a4/pydantic/version.py` & `pydantic-2.0b1/pydantic/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 __all__ = 'VERSION', 'version_info'
 
-VERSION = '2.0a4'
+VERSION = '2.0b1'
 
 
 def version_info() -> str:
     import platform
     import sys
     from importlib import import_module
     from pathlib import Path
```

### Comparing `pydantic-2.0a4/pydantic/_internal/_config.py` & `pydantic-2.0b1/pydantic/_internal/_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,14 @@
     str_max_length: int | None
     extra: ExtraValues | None
     frozen: bool
     populate_by_name: bool
     use_enum_values: bool
     validate_assignment: bool
     arbitrary_types_allowed: bool
-    undefined_types_warning: bool
     from_attributes: bool
     # whether to use the used alias (or first alias for "field required" errors) instead of field_names
     # to construct error `loc`s, default True
     loc_by_alias: bool
     alias_generator: Callable[[str], str] | None
     ignored_types: tuple[type, ...]
     allow_inf_nan: bool
@@ -50,14 +49,16 @@
     # whether instances of models and dataclasses (including subclass instances) should re-validate, default 'never'
     revalidate_instances: Literal['always', 'never', 'subclass-instances']
     ser_json_timedelta: Literal['iso8601', 'float']
     ser_json_bytes: Literal['utf8', 'base64']
     # whether to validate default values during validation, default False
     validate_default: bool
     validate_return: bool
+    protected_namespaces: tuple[str, ...]
+    hide_input_in_errors: bool
 
     def __init__(self, config: ConfigDict | dict[str, Any] | type[Any] | None, *, check: bool = True):
         if check:
             self.config_dict = prepare_config(config)
         else:
             self.config_dict = cast(ConfigDict, config)
 
@@ -105,39 +106,41 @@
                 return self.config_dict[name]
             except KeyError:
                 try:
                     return config_defaults[name]
                 except KeyError:
                     raise AttributeError(f'Config has no attribute {name!r}') from None
 
-    def core_config(self, obj: Any = None) -> core_schema.CoreConfig:
+    def core_config(self, obj: Any) -> core_schema.CoreConfig:
         """
         Create a pydantic-core config, `obj` is just used to populate `title` if not set in config.
 
+        Pass `obj=None` if you do not want to attempt to infer the `title`.
+
         We don't use getattr here since we don't want to populate with defaults.
         """
-        extra = self.config_dict.get('extra')
         core_config = core_schema.CoreConfig(
             **core_schema.dict_not_none(
                 title=self.config_dict.get('title') or (obj and obj.__name__),
-                extra_fields_behavior=extra,
+                extra_fields_behavior=self.config_dict.get('extra'),
                 allow_inf_nan=self.config_dict.get('allow_inf_nan'),
                 populate_by_name=self.config_dict.get('populate_by_name'),
                 str_strip_whitespace=self.config_dict.get('str_strip_whitespace'),
                 str_to_lower=self.config_dict.get('str_to_lower'),
                 str_to_upper=self.config_dict.get('str_to_upper'),
                 strict=self.config_dict.get('strict'),
                 ser_json_timedelta=self.config_dict.get('ser_json_timedelta'),
                 ser_json_bytes=self.config_dict.get('ser_json_bytes'),
                 from_attributes=self.config_dict.get('from_attributes'),
                 loc_by_alias=self.config_dict.get('loc_by_alias'),
                 revalidate_instances=self.config_dict.get('revalidate_instances'),
                 validate_default=self.config_dict.get('validate_default'),
                 str_max_length=self.config_dict.get('str_max_length'),
                 str_min_length=self.config_dict.get('str_min_length'),
+                hide_input_in_errors=self.config_dict.get('hide_input_in_errors'),
             )
         )
         return core_config
 
     def __repr__(self):
         c = ', '.join(f'{k}={v!r}' for k, v in self.config_dict.items())
         return f'ConfigWrapper({c})'
@@ -153,27 +156,28 @@
     # let the model / dataclass decide how to handle it
     extra=None,
     frozen=False,
     populate_by_name=False,
     use_enum_values=False,
     validate_assignment=False,
     arbitrary_types_allowed=False,
-    undefined_types_warning=True,
     from_attributes=False,
     loc_by_alias=True,
     alias_generator=None,
     ignored_types=(),
     allow_inf_nan=True,
     json_schema_extra=None,
     strict=False,
     revalidate_instances='never',
     ser_json_timedelta='iso8601',
     ser_json_bytes='utf8',
     validate_default=False,
     validate_return=False,
+    protected_namespaces=('model_',),
+    hide_input_in_errors=False,
 )
 
 
 def prepare_config(config: ConfigDict | dict[str, Any] | type[Any] | None) -> ConfigDict:
     """
     Create a `ConfigDict` instance from an existing dict, a class (e.g. old class-based config) or None.
     """
```

### Comparing `pydantic-2.0a4/pydantic/_internal/_core_metadata.py` & `pydantic-2.0b1/pydantic/_internal/_core_metadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     # If `pydantic_js_prefer_positional_arguments` is True, the JSON schema generator will
     # prefer positional over keyword arguments for an 'arguments' schema.
     pydantic_js_prefer_positional_arguments: bool | None
 
 
 class UpdateCoreSchemaCallable(typing_extensions.Protocol):
     def __call__(self, schema: CoreSchema, **kwargs: Any) -> None:
-        ...
+        ...  # pragma: no cover
 
 
 class CoreMetadataHandler:
     """
     Because the metadata field in pydantic_core is of type `Any`, we can't assume much about its contents.
 
     This class is used to interact with the metadata field on a CoreSchema object in a consistent
```

### Comparing `pydantic-2.0a4/pydantic/_internal/_core_utils.py` & `pydantic-2.0b1/pydantic/_internal/_core_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-# TODO: Should we move WalkAndApply into pydantic_core proper?
-
 from __future__ import annotations
 
 from collections import defaultdict
 from typing import Any, Callable, Iterable, TypeVar, Union, cast
 
 from pydantic_core import CoreSchema, core_schema
-from typing_extensions import TypeGuard, get_args
+from typing_extensions import TypeAliasType, TypeGuard, get_args
 
 from . import _repr
 
 AnyFunctionSchema = Union[
     core_schema.AfterValidatorFunctionSchema,
     core_schema.BeforeValidatorFunctionSchema,
     core_schema.WrapValidatorFunctionSchema,
@@ -20,18 +18,20 @@
 
 FunctionSchemaWithInnerSchema = Union[
     core_schema.AfterValidatorFunctionSchema,
     core_schema.BeforeValidatorFunctionSchema,
     core_schema.WrapValidatorFunctionSchema,
 ]
 
-CoreSchemaField = Union[core_schema.ModelField, core_schema.DataclassField, core_schema.TypedDictField]
+CoreSchemaField = Union[
+    core_schema.ModelField, core_schema.DataclassField, core_schema.TypedDictField, core_schema.ComputedField
+]
 CoreSchemaOrField = Union[core_schema.CoreSchema, CoreSchemaField]
 
-_CORE_SCHEMA_FIELD_TYPES = {'typed-dict-field', 'dataclass-field', 'model-field'}
+_CORE_SCHEMA_FIELD_TYPES = {'typed-dict-field', 'dataclass-field', 'model-field', 'computed-field'}
 _FUNCTION_WITH_INNER_SCHEMA_TYPES = {'function-before', 'function-after', 'function-wrap'}
 _LIST_LIKE_SCHEMA_WITH_ITEMS_TYPES = {'list', 'tuple-variable', 'set', 'frozenset'}
 
 
 def is_definition_ref_schema(s: core_schema.CoreSchema) -> TypeGuard[core_schema.DefinitionReferenceSchema]:
     return s['type'] == 'definition-ref'
 
@@ -77,16 +77,19 @@
     args = args_override or ()
     generic_metadata = getattr(type_, '__pydantic_generic_metadata__', None)
     if generic_metadata:
         origin = generic_metadata['origin'] or origin
         args = generic_metadata['args'] or args
 
     module_name = getattr(origin, '__module__', '<No __module__>')
-    qualname = getattr(origin, '__qualname__', f'<No __qualname__: {origin}>')
-    type_ref = f'{module_name}.{qualname}:{id(origin)}'
+    if isinstance(origin, TypeAliasType):
+        type_ref = f'{module_name}.{origin.__name__}'
+    else:
+        qualname = getattr(origin, '__qualname__', f'<No __qualname__: {origin}>')
+        type_ref = f'{module_name}.{qualname}:{id(origin)}'
 
     arg_refs: list[str] = []
     for arg in args:
         if isinstance(arg, str):
             # Handle string literals as a special case; we may be able to remove this special handling if we
             # wrap them in a ForwardRef at some point.
             arg_ref = f'{arg}:str-{id(arg)}'
@@ -197,14 +200,15 @@
 
     walk_core_schema(schema, _record_refs)
 
     expected_missing_refs = allowed_missing_refs.difference(refs)
     if expected_missing_refs:
         definitions: list[core_schema.CoreSchema] = [
             # TODO: Replace this with a (new) CoreSchema that, if present at any level, makes validation fail
+            #   Issue: https://github.com/pydantic/pydantic-core/issues/619
             core_schema.none_schema(ref=ref, metadata={'pydantic_debug_missing_ref': True, 'invalid': True})
             for ref in expected_missing_refs
         ]
         return core_schema.definitions_schema(schema, definitions)
     return schema
 
 
@@ -222,14 +226,17 @@
 
 T = TypeVar('T')
 
 
 Recurse = Callable[[core_schema.CoreSchema, 'Walk'], core_schema.CoreSchema]
 Walk = Callable[[core_schema.CoreSchema, Recurse], core_schema.CoreSchema]
 
+# TODO: Should we move _WalkCoreSchema into pydantic_core proper?
+#   Issue: https://github.com/pydantic/pydantic-core/issues/615
+
 
 class _WalkCoreSchema:
     def __init__(self):
         self._schema_type_to_method = self._build_schema_type_to_method()
 
     def _build_schema_type_to_method(self) -> dict[core_schema.CoreSchemaType, Recurse]:
         mapping: dict[core_schema.CoreSchemaType, Recurse] = {}
@@ -346,14 +353,19 @@
         return schema
 
     def handle_lax_or_strict_schema(self, schema: core_schema.LaxOrStrictSchema, f: Walk) -> core_schema.CoreSchema:
         schema['lax_schema'] = self.walk(schema['lax_schema'], f)
         schema['strict_schema'] = self.walk(schema['strict_schema'], f)
         return schema
 
+    def handle_json_or_python_schema(self, schema: core_schema.JsonOrPythonSchema, f: Walk) -> core_schema.CoreSchema:
+        schema['json_schema'] = self.walk(schema['json_schema'], f)
+        schema['python_schema'] = self.walk(schema['python_schema'], f)
+        return schema
+
     def handle_model_fields_schema(self, schema: core_schema.ModelFieldsSchema, f: Walk) -> core_schema.CoreSchema:
         if 'extra_validator' in schema:
             schema['extra_validator'] = self.walk(schema['extra_validator'], f)
         replaced_fields: dict[str, core_schema.ModelField] = {}
         for k, v in schema['fields'].items():
             replaced_field = v.copy()
             replaced_field['schema'] = self.walk(v['schema'], f)
```

### Comparing `pydantic-2.0a4/pydantic/_internal/_dataclasses.py` & `pydantic-2.0b1/pydantic/_internal/_dataclasses.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,112 +8,153 @@
 import warnings
 from functools import partial, wraps
 from typing import Any, Callable, ClassVar
 
 from pydantic_core import ArgsKwargs, SchemaSerializer, SchemaValidator, core_schema
 from typing_extensions import TypeGuard
 
+from ..errors import PydanticUndefinedAnnotation
 from ..fields import FieldInfo
-from . import _decorators, _typing_extra
+from . import _config, _decorators, _typing_extra
 from ._core_utils import flatten_schema_defs, inline_schema_defs
 from ._fields import collect_dataclass_fields
 from ._generate_schema import GenerateSchema
 from ._generics import get_standard_typevars_map
+from ._model_construction import MockValidator
+from ._schema_generation_shared import CallbackGetCoreSchemaHandler
 
 if typing.TYPE_CHECKING:
     from ..config import ConfigDict
-    from ._config import ConfigWrapper
 
     class StandardDataclass(typing.Protocol):
         __dataclass_fields__: ClassVar[dict[str, Any]]
         __dataclass_params__: ClassVar[Any]  # in reality `dataclasses._DataclassParams`
         __post_init__: ClassVar[Callable[..., None]]
 
         def __init__(self, *args: object, **kwargs: object) -> None:
             pass
 
     class PydanticDataclass(StandardDataclass, typing.Protocol):
         __pydantic_core_schema__: typing.ClassVar[core_schema.CoreSchema]
         __pydantic_validator__: typing.ClassVar[SchemaValidator]
         __pydantic_serializer__: typing.ClassVar[SchemaSerializer]
         __pydantic_decorators__: typing.ClassVar[_decorators.DecoratorInfos]
-        """metadata for `@validator`, `@root_validator` and `@serializer` decorators"""
+        """metadata for `@field_validator`, `@root_validator` and `@serializer` decorators"""
         __pydantic_fields__: typing.ClassVar[dict[str, FieldInfo]]
         __pydantic_config__: typing.ClassVar[ConfigDict]
+        __pydantic_complete__: typing.ClassVar[bool]
 
 
 def set_dataclass_fields(cls: type[StandardDataclass], types_namespace: dict[str, Any] | None = None) -> None:
     """
     Collect and set `cls.__pydantic_fields__`
     """
     typevars_map = get_standard_typevars_map(cls)
     fields = collect_dataclass_fields(cls, types_namespace, typevars_map=typevars_map)
 
     cls.__pydantic_fields__ = fields  # type: ignore
 
 
 def complete_dataclass(
     cls: type[Any],
-    config_wrapper: ConfigWrapper,
-) -> None:
+    config_wrapper: _config.ConfigWrapper,
+    *,
+    raise_errors: bool = True,
+    types_namespace: dict[str, Any] | None,
+) -> bool:
     """
-    Prepare a raw class to become a pydantic dataclass.
+    Finish building a pydantic dataclass.
 
     This logic is called on a class which is yet to be wrapped in `dataclasses.dataclass()`.
+
+    This is somewhat analogous to `pydantic._internal._model_construction.complete_model_class`.
     """
     if hasattr(cls, '__post_init_post_parse__'):
         warnings.warn(
             'Support for `__post_init_post_parse__` has been dropped, the method will not be called', DeprecationWarning
         )
 
-    types_namespace = _typing_extra.get_cls_types_namespace(cls)
+    if types_namespace is None:
+        types_namespace = _typing_extra.get_cls_types_namespace(cls)
+
+    set_dataclass_fields(cls, types_namespace)
+
     typevars_map = get_standard_typevars_map(cls)
     gen_schema = GenerateSchema(
         config_wrapper,
         types_namespace,
         typevars_map,
     )
 
+    # dataclass.__init__ must be defined here so its `__qualname__` can be changed since functions can't be copied.
+
+    def __init__(__dataclass_self__: PydanticDataclass, *args: Any, **kwargs: Any) -> None:
+        __tracebackhide__ = True
+        s = __dataclass_self__
+        s.__pydantic_validator__.validate_python(ArgsKwargs(args, kwargs), self_instance=s)
+
+    __init__.__qualname__ = f'{cls.__qualname__}.__init__'
+    cls.__init__ = __init__  # type: ignore
+    cls.__pydantic_config__ = config_wrapper.config_dict  # type: ignore
+
     get_core_schema = getattr(cls, '__get_pydantic_core_schema__', None)
-    if get_core_schema:
-        schema = get_core_schema(cls, partial(gen_schema.generate_schema, from_dunder_get_core_schema=False))
-    else:
-        schema = gen_schema.generate_schema(cls, from_dunder_get_core_schema=False)
+    try:
+        if get_core_schema:
+            schema = get_core_schema(
+                cls,
+                CallbackGetCoreSchemaHandler(
+                    partial(gen_schema.generate_schema, from_dunder_get_core_schema=False),
+                    gen_schema.generate_schema,
+                ),
+            )
+        else:
+            schema = gen_schema.generate_schema(cls, from_dunder_get_core_schema=False)
+    except PydanticUndefinedAnnotation as e:
+        cls_name = cls.__name__
+        if raise_errors:
+            raise
+        undefined_type_error_message = (
+            f'`{cls_name}` is not fully defined; you should define `{e.name}`,'
+            f' then call `pydantic.dataclasses.rebuild_dataclass({cls_name})`'
+            f' before the first `{cls_name}` instance is created.'
+        )
+
+        def attempt_rebuild() -> SchemaValidator | None:
+            from ..dataclasses import rebuild_dataclass
+
+            if rebuild_dataclass(cls, raise_errors=False, _parent_namespace_depth=5):
+                return cls.__pydantic_validator__  # type: ignore
+            else:
+                return None
+
+        cls.__pydantic_validator__ = MockValidator(  # type: ignore[assignment]
+            undefined_type_error_message, code='class-not-fully-defined', attempt_rebuild=attempt_rebuild
+        )
+        return False
 
     core_config = config_wrapper.core_config(cls)
 
     # We are about to set all the remaining required properties expected for this cast;
     # __pydantic_decorators__ and __pydantic_fields__ should already be set
     cls = typing.cast('type[PydanticDataclass]', cls)
     # debug(schema)
     cls.__pydantic_core_schema__ = schema
-    schema = flatten_schema_defs(schema)
-    simplified_core_schema = inline_schema_defs(schema)
+    simplified_core_schema = inline_schema_defs(flatten_schema_defs(schema))
     cls.__pydantic_validator__ = validator = SchemaValidator(simplified_core_schema, core_config)
     cls.__pydantic_serializer__ = SchemaSerializer(simplified_core_schema, core_config)
-    # dataclasses only:
-    cls.__pydantic_config__ = config_wrapper.config_dict
 
     if config_wrapper.validate_assignment:
 
         @wraps(cls.__setattr__)
         def validated_setattr(instance: Any, __field: str, __value: str) -> None:
             validator.validate_assignment(instance, __field, __value)
 
         cls.__setattr__ = validated_setattr.__get__(None, cls)  # type: ignore
 
-    # dataclass.__init__ must be defined here so its `__qualname__` can be changed since functions can't copied.
-
-    def __init__(__dataclass_self__: PydanticDataclass, *args: Any, **kwargs: Any) -> None:
-        __tracebackhide__ = True
-        s = __dataclass_self__
-        s.__pydantic_validator__.validate_python(ArgsKwargs(args, kwargs), self_instance=s)
-
-    __init__.__qualname__ = f'{cls.__qualname__}.__init__'
-    cls.__init__ = __init__  # type: ignore
+    return True
 
 
 def is_builtin_dataclass(_cls: type[Any]) -> TypeGuard[type[StandardDataclass]]:
     """
     Whether a class is a stdlib dataclass
     (useful to discriminated a pydantic dataclass that is actually a wrapper around a stdlib dataclass)
 
@@ -138,8 +179,8 @@
         dataclasses.is_dataclass(_cls)
         and not hasattr(_cls, '__pydantic_validator__')
         and set(_cls.__dataclass_fields__).issuperset(set(getattr(_cls, '__annotations__', {})))
     )
 
 
 def is_pydantic_dataclass(_cls: type[Any]) -> TypeGuard[type[PydanticDataclass]]:
-    return dataclasses.is_dataclass(_cls) and hasattr(_cls, '__pydantic_validator__')
+    return dataclasses.is_dataclass(_cls) and '__pydantic_validator__' in _cls.__dict__
```

### Comparing `pydantic-2.0a4/pydantic/_internal/_decorators_v1.py` & `pydantic-2.0b1/pydantic/_internal/_decorators_v1.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a4/pydantic/_internal/_discriminated_union.py` & `pydantic-2.0b1/pydantic/_internal/_discriminated_union.py`

 * *Files 0% similar despite different names*

```diff
@@ -324,14 +324,17 @@
         else:
             raise PydanticUserError(
                 f'{source} needs a discriminator field for key {self.discriminator!r}', code='discriminator-no-field'
             )
         return self._infer_discriminator_values_for_field(field, source)
 
     def _infer_discriminator_values_for_field(self, field: CoreSchemaField, source: str) -> list[str | int]:
+        if field['type'] == 'computed-field':
+            # This should never occur as a discriminator, as it is only relevant to serialization
+            return []
         alias = field.get('validation_alias', self.discriminator)
         if not isinstance(alias, str):
             raise PydanticUserError(
                 f'Alias {alias!r} is not supported in a discriminated union', code='discriminator-alias-type'
             )
         if self._discriminator_alias is None:
             self._discriminator_alias = alias
```

### Comparing `pydantic-2.0a4/pydantic/_internal/_fields.py` & `pydantic-2.0b1/pydantic/_internal/_fields.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,20 +5,22 @@
 
 import dataclasses
 import sys
 from copy import copy
 from typing import TYPE_CHECKING, Any
 
 from . import _typing_extra
+from ._config import ConfigWrapper
 from ._forward_ref import PydanticForwardRef
 from ._repr import Representation
 from ._typing_extra import get_cls_type_hints_lenient, get_type_hints, is_classvar, is_finalvar
 
 if TYPE_CHECKING:
     from ..fields import FieldInfo
+    from ..main import BaseModel
     from ._dataclasses import StandardDataclass
 
 
 def get_type_hints_infer_globalns(
     obj: Any,
     localns: dict[str, Any] | None = None,
     include_extras: bool = False,
@@ -65,16 +67,17 @@
 
 class PydanticGeneralMetadata(PydanticMetadata):
     def __init__(self, **metadata: Any):
         self.__dict__ = metadata
 
 
 def collect_model_fields(  # noqa: C901
-    cls: type[Any],
+    cls: type[BaseModel],
     bases: tuple[type[Any], ...],
+    config_wrapper: ConfigWrapper,
     types_namespace: dict[str, Any] | None,
     *,
     typevars_map: dict[Any, Any] | None = None,
 ) -> tuple[dict[str, FieldInfo], set[str]]:
     """
     Collect the fields of a nascent pydantic model
 
@@ -93,22 +96,29 @@
     # https://docs.python.org/3/howto/annotations.html#accessing-the-annotations-dict-of-an-object-in-python-3-9-and-older
     # annotations is only used for finding fields in parent classes
     annotations = cls.__dict__.get('__annotations__', {})
     fields: dict[str, FieldInfo] = {}
 
     class_vars: set[str] = set()
     for ann_name, ann_type in type_hints.items():
+        for protected_namespace in config_wrapper.protected_namespaces:
+            if ann_name.startswith(protected_namespace):
+                raise NameError(f'Field "{ann_name}" has conflict with protected namespace "{protected_namespace}"')
         if is_classvar(ann_type):
             class_vars.add(ann_name)
             continue
         if _is_finalvar_with_default_val(ann_type, getattr(cls, ann_name, Undefined)):
             class_vars.add(ann_name)
             continue
         if ann_name.startswith('_'):
             continue
+        if cls.__pydantic_root_model__ and ann_name != 'root':
+            raise NameError(
+                f"Unexpected field with name {ann_name!r}; only 'root' is allowed as a field of a `RootModel`"
+            )
 
         # when building a generic model with `MyModel[int]`, the generic_origin check makes sure we don't get
         # "... shadows an attribute" errors
         generic_origin = getattr(cls, '__pydantic_generic_metadata__', {}).get('origin')
         for base in bases:
             if hasattr(base, ann_name):
                 if base is generic_origin:
@@ -120,16 +130,18 @@
                 )
 
         try:
             default = getattr(cls, ann_name, Undefined)
             if default is Undefined:
                 raise AttributeError
         except AttributeError:
-            if ann_name in annotations or isinstance(ann_type, PydanticForwardRef):
+            if ann_name in annotations:
                 field_info = FieldInfo.from_annotation(ann_type)
+            elif isinstance(ann_type, PydanticForwardRef):
+                field_info = FieldInfo.from_annotation(annotation=ann_type)  # type: ignore
             else:
                 # if field has no default value and is not in __annotations__ this means that it is
                 # defined in a base class and we can take it from there
                 model_fields_lookup: dict[str, FieldInfo] = {}
                 for x in cls.__bases__[::-1]:
                     model_fields_lookup.update(getattr(x, 'model_fields', {}))
                 if ann_name in model_fields_lookup:
@@ -185,15 +197,15 @@
     for ann_name, dataclass_field in dataclass_fields.items():
         ann_type = _typing_extra.eval_type_lenient(dataclass_field.type, types_namespace, cls_localns)
         if is_classvar(ann_type):
             continue
 
         if not dataclass_field.init:
             # TODO: We should probably do something with this so that validate_assignment behaves properly
-            #   See https://github.com/pydantic/pydantic/issues/5470
+            #   Issue: https://github.com/pydantic/pydantic/issues/5470
             continue
 
         if isinstance(dataclass_field.default, FieldInfo):
             field_info = FieldInfo.from_annotated_attribute(ann_type, dataclass_field.default)
         else:
             field_info = FieldInfo.from_annotated_attribute(ann_type, dataclass_field)
         fields[ann_name] = field_info
```

### Comparing `pydantic-2.0a4/pydantic/_internal/_forward_ref.py` & `pydantic-2.0b1/pydantic/_internal/_forward_ref.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a4/pydantic/_internal/_generate_schema.py` & `pydantic-2.0b1/pydantic/_internal/_generate_schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 """
 Convert python types to pydantic-core schema.
 """
 from __future__ import annotations as _annotations
 
 import collections.abc
+import dataclasses
 import inspect
 import re
 import sys
 import typing
 import warnings
 from functools import partial
 from inspect import Parameter, _ParameterKind, signature
 from itertools import chain
+from operator import attrgetter
 from types import FunctionType, LambdaType, MethodType
-from typing import TYPE_CHECKING, Any, Callable, ForwardRef, Iterable, Mapping, TypeVar, Union
+from typing import TYPE_CHECKING, Any, Callable, ForwardRef, Iterable, Mapping, TypeVar, Union, cast
 
 from pydantic_core import CoreSchema, core_schema
-from typing_extensions import Annotated, Final, Literal, TypedDict, get_args, get_origin, is_typeddict
+from typing_extensions import Annotated, Final, Literal, TypeAliasType, TypedDict, get_args, get_origin, is_typeddict
 
+from ..config import ConfigDict
 from ..errors import PydanticSchemaGenerationError, PydanticUndefinedAnnotation, PydanticUserError
-from ..fields import FieldInfo
+from ..fields import AliasChoices, AliasPath, FieldInfo
+from ..json_schema import JsonSchemaValue
 from . import _discriminated_union, _known_annotated_metadata, _typing_extra
+from ._annotated_handlers import GetCoreSchemaHandler, GetJsonSchemaHandler
 from ._config import ConfigWrapper
 from ._core_metadata import (
     CoreMetadataHandler,
     build_metadata_dict,
 )
 from ._core_utils import (
+    CoreSchemaOrField,
     consolidate_refs,
     define_expected_missing_refs,
     get_type_ref,
     is_list_like_schema_with_items_schema,
     remove_unnecessary_invalid_definitions,
 )
 from ._decorators import (
@@ -52,31 +58,27 @@
     collect_dataclass_fields,
     get_type_hints_infer_globalns,
 )
 from ._forward_ref import PydanticForwardRef, PydanticRecursiveRef
 from ._generics import get_standard_typevars_map, recursively_defined_type_refs, replace_types
 from ._schema_generation_shared import (
     CallbackGetCoreSchemaHandler,
-    CoreSchemaOrField,
-    GetCoreSchemaHandler,
-    GetJsonSchemaFunction,
-    GetJsonSchemaHandler,
-    JsonSchemaValue,
     UnpackedRefJsonSchemaHandler,
     wrap_json_schema_fn_for_model_or_custom_type_with_ref_unpacking,
 )
 from ._typing_extra import is_finalvar
 from ._utils import lenient_issubclass
 
 if TYPE_CHECKING:
-    from ..decorators import FieldValidatorModes
     from ..main import BaseModel
+    from ..validators import FieldValidatorModes
     from ._dataclasses import StandardDataclass
+    from ._schema_generation_shared import GetJsonSchemaFunction
 
-_SUPPORTS_TYPEDDICT = sys.version_info >= (3, 11)
+_SUPPORTS_TYPEDDICT = sys.version_info >= (3, 12)
 
 FieldDecoratorInfo = Union[ValidatorDecoratorInfo, FieldValidatorDecoratorInfo, FieldSerializerDecoratorInfo]
 FieldDecoratorInfoType = TypeVar('FieldDecoratorInfoType', bound=FieldDecoratorInfo)
 AnyFieldDecorator = Union[
     Decorator[ValidatorDecoratorInfo],
     Decorator[FieldValidatorDecoratorInfo],
     Decorator[FieldSerializerDecoratorInfo],
@@ -105,30 +107,31 @@
         if isinstance(dec.info, (ValidatorDecoratorInfo, FieldValidatorDecoratorInfo)) and '*' in dec.info.fields:
             continue
         if dec.info.check_fields is False:
             continue
         for field in dec.info.fields:
             if field not in fields:
                 raise PydanticUserError(
-                    f'Validators defined with incorrect fields: {dec.cls_ref}.{dec.cls_var_name}'
+                    f'Decorators defined with incorrect fields: {dec.cls_ref}.{dec.cls_var_name}'
                     " (use check_fields=False if you're inheriting from the model and intended this)",
                     code='decorator-missing-field',
                 )
 
 
 def filter_field_decorator_info_by_field(
     validator_functions: Iterable[Decorator[FieldDecoratorInfoType]], field: str
 ) -> list[Decorator[FieldDecoratorInfoType]]:
     return [dec for dec in validator_functions if check_validator_fields_against_field_name(dec.info, field)]
 
 
 def apply_each_item_validators(
     schema: core_schema.CoreSchema, each_item_validators: list[Decorator[ValidatorDecoratorInfo]]
 ) -> core_schema.CoreSchema:
-    # TODO: remove this V1 compatibility shim once it's deprecated
+    # This V1 compatibility shim should eventually be removed
+
     # push down any `each_item=True` validators
     # note that this won't work for any Annotated types that get wrapped by a function validator
     # but that's okay because that didn't exist in V1
     if schema['type'] == 'nullable':
         schema['schema'] = apply_each_item_validators(schema['schema'], each_item_validators)
         return schema
     elif is_list_like_schema_with_items_schema(schema):
@@ -188,126 +191,141 @@
         return self._config_wrapper_stack[-1]
 
     @property
     def arbitrary_types(self) -> bool:
         return self.config_wrapper.arbitrary_types_allowed
 
     def generate_schema(
-        self, obj: Any, from_dunder_get_core_schema: bool = True, from_prepare_args: bool = True
+        self,
+        obj: Any,
+        from_dunder_get_core_schema: bool = True,
+        from_prepare_args: bool = True,
     ) -> core_schema.CoreSchema:
+        if isinstance(obj, type(Annotated[int, 123])):
+            return self._annotated_schema(obj)
+        return self._generate_schema_for_type(
+            obj, from_dunder_get_core_schema=from_dunder_get_core_schema, from_prepare_args=from_prepare_args
+        )
+
+    def _generate_schema_for_type(
+        self,
+        obj: Any,
+        from_dunder_get_core_schema: bool = True,
+        from_prepare_args: bool = True,
+    ) -> CoreSchema:
         schema: CoreSchema | None = None
 
         if from_prepare_args:
             schema = self._generate_schema_from_prepare_annotations(obj)
-            if schema:
-                return schema
 
         if from_dunder_get_core_schema:
             from_property = self._generate_schema_from_property(obj, obj)
             if from_property is not None:
                 schema = from_property
+
         if schema is None:
             schema = self._generate_schema(obj)
 
-        schema = remove_unnecessary_invalid_definitions(schema)
-
-        metadata_js_function = _extract_get_pydantic_json_schema(obj)
-        if metadata_js_function is None:
-            # Need to do this to handle custom generics
-            # Skip Annotated because Annotated.__origin__ will be analyzed in the next recursion
-            if hasattr(obj, '__origin__') and not isinstance(obj, type(Annotated[int, 123])):
-                metadata_js_function = _extract_get_pydantic_json_schema(obj.__origin__)
+        metadata_js_function = _extract_get_pydantic_json_schema(obj, schema)
         if metadata_js_function is not None:
             metadata = CoreMetadataHandler(schema).metadata
-            # wrap the schema so that we unpack ref schemas and always call metadata_js_function with the full schema
-            if schema['type'] != 'definition-ref':
-                # we would fail to unpack recursive ref schemas!
-                metadata_js_function = wrap_json_schema_fn_for_model_or_custom_type_with_ref_unpacking(
-                    metadata_js_function
-                )
-            metadata['pydantic_js_functions'] = metadata.get('pydantic_js_functions', [])
-            metadata['pydantic_js_functions'].append(metadata_js_function)
+            metadata.setdefault('pydantic_js_functions', []).append(metadata_js_function)
 
-        if 'ref' in schema:
+        schema = remove_unnecessary_invalid_definitions(schema)
+
+        ref = schema.get('ref', None)
+        if ref:
             # definitions and definition-ref schemas don't have 'ref', causing the type error ignored on the next line
-            schema_ref = schema['ref']  # type: ignore[typeddict-item]
-            self.definitions[schema_ref] = schema
+            self.definitions[ref] = schema
 
         return schema
 
     def model_schema(self, cls: type[BaseModel]) -> core_schema.CoreSchema:
         """
         Generate schema for a pydantic model.
 
         Since models generate schemas for themselves this method is public and can be called
         from within BaseModel's metaclass.
         """
         model_ref, schema = self._get_or_cache_recursive_ref(cls)
         if schema is not None:
             return schema
 
-        from ..main import BaseModel
-
         fields = cls.model_fields
         decorators = cls.__pydantic_decorators__
         check_decorator_fields_exist(
             chain(
-                decorators.field_validator.values(),
-                decorators.field_serializer.values(),
-                decorators.validator.values(),
+                decorators.field_validators.values(),
+                decorators.field_serializers.values(),
+                decorators.validators.values(),
             ),
             fields.keys(),
         )
-        # TODO: we need to do something similar to this for pydantic dataclasses
-        #   This should be straight forward once we expose the pydantic config on the dataclass;
-        #   I have done this in my PR for dataclasses JSON schema
         config_wrapper = ConfigWrapper(cls.model_config, check=False)
-        self._config_wrapper_stack.append(config_wrapper)
-        try:
-            fields_schema: core_schema.CoreSchema = core_schema.model_fields_schema(
-                {k: self._generate_md_field_schema(k, v, decorators) for k, v in fields.items()},
-                computed_fields=generate_computed_field(decorators.computed_fields),
-            )
-        finally:
-            self._config_wrapper_stack.pop()
-        inner_schema = apply_validators(fields_schema, decorators.root_validator.values())
+        core_config = config_wrapper.core_config(cls)
+        metadata = build_metadata_dict(js_functions=[partial(modify_model_json_schema, cls=cls)])
 
-        inner_schema = define_expected_missing_refs(inner_schema, recursively_defined_type_refs())
+        model_validators = decorators.model_validators.values()
 
-        core_config = config_wrapper.core_config()
-        model_post_init = None if cls.model_post_init is BaseModel.model_post_init else 'model_post_init'
+        if cls.__pydantic_root_model__:
+            root_field = self._common_field_schema('root', fields['root'], decorators)
+            inner_schema = root_field['schema']
+            inner_schema = apply_model_validators(inner_schema, model_validators, 'inner')
+            model_schema = core_schema.model_schema(
+                cls,
+                inner_schema,
+                custom_init=getattr(cls, '__pydantic_custom_init__', None),
+                root_model=True,
+                post_init=getattr(cls, '__pydantic_post_init__', None),
+                config=core_config,
+                ref=model_ref,
+                metadata={**metadata, **root_field['metadata']},
+            )
+        else:
+            self._config_wrapper_stack.append(config_wrapper)
+            try:
+                fields_schema: core_schema.CoreSchema = core_schema.model_fields_schema(
+                    {k: self._generate_md_field_schema(k, v, decorators) for k, v in fields.items()},
+                    computed_fields=[self._computed_field_schema(d) for d in decorators.computed_fields.values()],
+                )
+            finally:
+                self._config_wrapper_stack.pop()
 
-        metadata = build_metadata_dict(js_functions=[partial(modify_model_json_schema, cls=cls)])
+            inner_schema = apply_validators(fields_schema, decorators.root_validators.values())
+            inner_schema = define_expected_missing_refs(inner_schema, recursively_defined_type_refs())
+            inner_schema = apply_model_validators(inner_schema, model_validators, 'inner')
+
+            model_schema = core_schema.model_schema(
+                cls,
+                inner_schema,
+                custom_init=getattr(cls, '__pydantic_custom_init__', None),
+                root_model=False,
+                post_init=getattr(cls, '__pydantic_post_init__', None),
+                config=core_config,
+                ref=model_ref,
+                metadata=metadata,
+            )
 
-        model_schema = core_schema.model_schema(
-            cls,
-            inner_schema,
-            ref=model_ref,
-            config=core_config,
-            post_init=model_post_init,
-            metadata=metadata,
-            custom_init=cls.__init__ is not BaseModel.__init__,
-        )
         model_schema = consolidate_refs(model_schema)
-        schema = apply_model_serializers(model_schema, decorators.model_serializer.values())
-        return apply_model_validators(schema, decorators.model_validator.values())
+        schema = self._apply_model_serializers(model_schema, decorators.model_serializers.values())
+        return apply_model_validators(schema, model_validators, 'outer')
 
     def _generate_schema_from_prepare_annotations(self, obj: Any) -> core_schema.CoreSchema | None:
         """
         Try to generate schema from either the `__get_pydantic_core_schema__` function or
         `__pydantic_core_schema__` property.
 
         Note: `__get_pydantic_core_schema__` takes priority so it can
         decide whether to use a `__pydantic_core_schema__` attribute, or generate a fresh schema.
         """
-        obj, new_annotations = self._prepare_annotations(obj, [])
-        if new_annotations:
+        new_obj, new_annotations = self._prepare_annotations(obj, [])
+        if new_obj is not obj or new_annotations:
             return self._apply_annotations(
-                CallbackGetCoreSchemaHandler(partial(self.generate_schema, from_prepare_args=False)),
-                obj,
+                lambda x: x,
+                new_obj,
                 new_annotations,
             )
         return None
 
     def _generate_schema_from_property(self, obj: Any, source: Any) -> core_schema.CoreSchema | None:
         """
         Try to generate schema from either the `__get_pydantic_core_schema__` function or
@@ -320,15 +338,15 @@
         if get_schema is None:
             return None
 
         if len(inspect.signature(get_schema).parameters) == 1:
             # (source) -> CoreSchema
             return get_schema(source)
 
-        return get_schema(source, partial(self.generate_schema, from_dunder_get_core_schema=False))
+        return get_schema(source, CallbackGetCoreSchemaHandler(self._generate_schema, self.generate_schema))
 
     def _generate_schema(self, obj: Any) -> core_schema.CoreSchema:  # noqa: C901
         """
         Recursively generate a pydantic-core schema for any supported python type.
         """
         if isinstance(obj, dict):
             # we assume this is already a valid schema
@@ -353,14 +371,16 @@
             # if obj is still a ForwardRef, it means we can't evaluate it, raise PydanticUndefinedAnnotation
             if isinstance(obj, ForwardRef):
                 raise PydanticUndefinedAnnotation(obj.__forward_arg__, f'Unable to evaluate forward reference {obj}')
 
             if self.typevars_map:
                 obj = replace_types(obj, self.typevars_map)
 
+            return self.generate_schema(obj)
+
         from ..main import BaseModel
 
         if lenient_issubclass(obj, BaseModel):
             return self.model_schema(obj)
 
         if isinstance(obj, PydanticRecursiveRef):
             return core_schema.definition_reference_schema(schema_ref=obj.type_ref)
@@ -369,14 +389,15 @@
             if not obj.deferred_actions:
                 return obj.schema
             resolved_model = obj.resolve_model()
             if isinstance(resolved_model, PydanticForwardRef):
                 # If you still have a PydanticForwardRef after resolving, it should be deeply nested enough that it will
                 # eventually be substituted out. So it is safe to return an invalid schema here.
                 # TODO: Replace this with a (new) CoreSchema that, if present at any level, makes validation fail
+                #   Issue: https://github.com/pydantic/pydantic-core/issues/619
                 return core_schema.none_schema(
                     metadata={'invalid': True, 'pydantic_debug_self_schema': resolved_model.schema}
                 )
             else:
                 model_ref = get_type_ref(resolved_model)
                 return core_schema.definition_reference_schema(model_ref)
 
@@ -406,124 +427,82 @@
         elif _typing_extra.is_new_type(obj):
             # NewType, can't use isinstance because it fails <3.7
             return self.generate_schema(obj.__supertype__)
         elif obj == re.Pattern:
             return self._pattern_schema(obj)
         elif obj is collections.abc.Hashable or obj is typing.Hashable:
             return self._hashable_schema()
-        elif isinstance(obj, type):
-            if obj is dict:
-                return self._dict_schema(obj)
-            if issubclass(obj, dict):
-                # TODO: We would need to handle generic subclasses of certain typing dict subclasses here
-                #   This includes subclasses of typing.Counter, typing.DefaultDict, and typing.OrderedDict
-                #   Note also that we may do a better job of handling typing.DefaultDict by inspecting its arguments.
-                return self._dict_subclass_schema(obj)
-            # probably need to take care of other subclasses here
         elif isinstance(obj, typing.TypeVar):
             return self._unsubstituted_typevar_schema(obj)
         elif is_finalvar(obj):
             if obj is Final:
                 return core_schema.AnySchema(type='any')
             return self.generate_schema(get_args(obj)[0])
         elif isinstance(obj, (FunctionType, LambdaType, MethodType, partial)):
             return self._callable_schema(obj)
 
-        # TODO: _std_types_schema iterates over the __mro__ looking for an expected schema.
-        #   This will catch subclasses of typing.Deque, preventing us from properly supporting user-defined
-        #   generic subclasses. (In principle this would also catch typing.OrderedDict, but that is currently
-        #   already getting caught in the `issubclass(obj, dict):` check above.
-        std_schema = self._std_types_schema(obj)
-        if std_schema is not None:
-            return std_schema
-
         if _typing_extra.is_dataclass(obj):
             return self._dataclass_schema(obj, None)
 
         origin = get_origin(obj)
+
+        if isinstance(obj, TypeAliasType) or isinstance(origin, TypeAliasType):
+            return self._type_alias_type_schema(obj)
+
         if origin is None:
-            if self.arbitrary_types:
-                return core_schema.is_instance_schema(obj)
-            else:
-                raise PydanticSchemaGenerationError(
-                    f'Unable to generate pydantic-core schema for {obj!r}. '
-                    f'Setting `arbitrary_types_allowed=True` in the model_config may prevent this error.'
-                )
+            return self._arbitrary_type_schema(obj, obj)
 
         # Need to handle generic dataclasses before looking for the schema properties because attribute accesses
         # on _GenericAlias delegate to the origin type, so lose the information about the concrete parametrization
         # As a result, currently, there is no way to cache the schema for generic dataclasses. This may be possible
         # to resolve by modifying the value returned by `Generic.__class_getitem__`, but that is a dangerous game.
         if _typing_extra.is_dataclass(origin):
             return self._dataclass_schema(obj, origin)
 
         from_property = self._generate_schema_from_property(origin, obj)
         if from_property is not None:
             return from_property
 
         if _typing_extra.origin_is_union(origin):
             return self._union_schema(obj)
-        elif issubclass(origin, Annotated):  # type: ignore[arg-type]
-            return self._annotated_schema(obj)
-        elif issubclass(origin, typing.List):
-            return self._generic_collection_schema(list, obj, origin)
-        elif issubclass(origin, typing.Set):
-            return self._generic_collection_schema(set, obj, origin)
-        elif issubclass(origin, typing.FrozenSet):
-            return self._generic_collection_schema(frozenset, obj, origin)
         elif issubclass(origin, typing.Tuple):  # type: ignore[arg-type]
-            # TODO: To support generic subclasses of typing.Tuple, we need to better-introspect the args to origin
             return self._tuple_schema(obj)
-        elif issubclass(origin, typing.Counter):
-            # Subclasses of typing.Counter may be handled as subclasses of dict; see note above
-            return self._counter_schema(obj)
-        elif origin in (typing.Dict, dict):
-            return self._dict_schema(obj)
         elif is_typeddict(origin):
             return self._typed_dict_schema(obj, origin)
-        elif issubclass(origin, typing.Dict):
-            # Subclasses of typing.Dict may be handled as subclasses of dict; see note above
-            return self._dict_subclass_schema(obj)
-        elif issubclass(origin, typing.Mapping):
-            # Because typing.Mapping does not have a specified `__init__` signature, we don't validate into subclasses
-            return self._mapping_schema(obj)
         elif issubclass(origin, typing.Type):  # type: ignore[arg-type]
             return self._subclass_schema(obj)
-        elif issubclass(origin, typing.Deque):
-            from ._std_types_schema import deque_schema
-
-            return deque_schema(self, obj)
-        elif issubclass(origin, typing.OrderedDict):
-            # Subclasses of typing.OrderedDict may be handled as subclasses of dict; see note above
-            from ._std_types_schema import ordered_dict_schema
-
-            return ordered_dict_schema(self, obj)
         elif issubclass(origin, typing.Sequence):
             if origin in {typing.Sequence, collections.abc.Sequence}:
                 return self._sequence_schema(obj)
-            # TODO: similarly handle other generic subclasses (like Iterable, etc.) where there's no standard __init__
-            raise PydanticSchemaGenerationError(
-                'Unable to generate pydantic-core schema for custom subclasses of Sequence.'
-                ' Please define `__get_pydantic_core_schema__`. TODO: Add docs link.'
-            )
-        elif issubclass(origin, typing.MutableSet):
-            raise PydanticSchemaGenerationError('Unable to generate pydantic-core schema MutableSet TODO.')
+            else:
+                return self._arbitrary_type_schema(obj, origin)
         elif issubclass(origin, (typing.Iterable, collections.abc.Iterable)):
             # Because typing.Iterable does not have a specified `__init__` signature, we don't validate into subclasses
-            return self._iterable_schema(obj)
+            if origin in {typing.Iterable, collections.abc.Iterable, typing.Generator, collections.abc.Generator}:
+                return self._iterable_schema(obj)
+            else:
+                return self._arbitrary_type_schema(obj, origin)
         elif issubclass(origin, (re.Pattern, typing.Pattern)):
             return self._pattern_schema(obj)
         else:
-            if self.arbitrary_types and isinstance(origin, type):
-                return core_schema.is_instance_schema(origin)
-            else:
-                raise PydanticSchemaGenerationError(
-                    f'Unable to generate pydantic-core schema for {obj!r} (origin={origin!r}). '
-                    f'Setting `arbitrary_types_allowed=True` in the model_config may prevent this error.'
-                )
+            return self._arbitrary_type_schema(obj, origin)
+
+    def _arbitrary_type_schema(self, obj: Any, type_: Any) -> CoreSchema:
+        if self.arbitrary_types and isinstance(type_, type):
+            return core_schema.is_instance_schema(type_)
+        else:
+            raise PydanticSchemaGenerationError(
+                f'Unable to generate pydantic-core schema for {obj!r}. '
+                'Set `arbitrary_types_allowed=True` in the model_config to ignore this error'
+                ' or implement `__get_pydantic_core_schema__` on your type to fully support it.'
+                '\n\nIf you got this error by calling handler(<some type>) within'
+                ' `__get_pydantic_core_schema__` then you likely need to call'
+                ' `handler.generate_schema(<some type>)` since we do not call'
+                ' `__get_pydantic_core_schema__` on `<some type>` otherwise to avoid infinite recursion.'
+            )
 
     def _generate_td_field_schema(
         self,
         name: str,
         field_info: FieldInfo,
         decorators: DecoratorInfos,
         *,
@@ -584,65 +563,84 @@
             frozen=common_field['frozen'],
             metadata=common_field['metadata'],
         )
 
     def _common_field_schema(self, name: str, field_info: FieldInfo, decorators: DecoratorInfos) -> _CommonField:
         assert field_info.annotation is not None, 'field_info.annotation should not be None when generating a schema'
 
-        def generate_schema(source: Any) -> CoreSchema:
-            schema = self.generate_schema(source, from_prepare_args=False)
+        def apply_discriminator(schema: CoreSchema) -> CoreSchema:
             if field_info.discriminator is not None:
                 schema = _discriminated_union.apply_discriminator(schema, field_info.discriminator, self.definitions)
             return schema
 
+        source_type, annotations = field_info.annotation, field_info.metadata
         schema = self._apply_annotations(
-            CallbackGetCoreSchemaHandler(generate_schema), field_info.annotation, field_info.metadata
+            apply_discriminator,
+            source_type,
+            annotations,
         )
 
-        # TODO: remove this V1 compatibility shim once it's deprecated
+        # This V1 compatibility shim should eventually be removed
         # push down any `each_item=True` validators
         # note that this won't work for any Annotated types that get wrapped by a function validator
         # but that's okay because that didn't exist in V1
-        this_field_validators = filter_field_decorator_info_by_field(decorators.validator.values(), name)
+        this_field_validators = filter_field_decorator_info_by_field(decorators.validators.values(), name)
         if _validators_require_validate_default(this_field_validators):
             field_info.validate_default = True
         each_item_validators = [v for v in this_field_validators if v.info.each_item is True]
         this_field_validators = [v for v in this_field_validators if v not in each_item_validators]
         schema = apply_each_item_validators(schema, each_item_validators)
 
         schema = apply_validators(schema, filter_field_decorator_info_by_field(this_field_validators, name))
         schema = apply_validators(
-            schema, filter_field_decorator_info_by_field(decorators.field_validator.values(), name)
+            schema, filter_field_decorator_info_by_field(decorators.field_validators.values(), name)
         )
 
         # the default validator needs to go outside of any other validators
         # so that it is the topmost validator for the field validator
         # which uses it to check if the field has a default value or not
         if not field_info.is_required():
             schema = wrap_default(field_info, schema)
 
-        schema = apply_field_serializers(
-            schema, filter_field_decorator_info_by_field(decorators.field_serializer.values(), name)
+        schema = self._apply_field_serializers(
+            schema, filter_field_decorator_info_by_field(decorators.field_serializers.values(), name)
         )
         json_schema_updates = {
             'title': field_info.title,
             'description': field_info.description,
             'examples': field_info.examples,
         }
         json_schema_updates = {k: v for k, v in json_schema_updates.items() if v is not None}
         json_schema_updates.update(field_info.json_schema_extra or {})
 
         def json_schema_update_func(schema: CoreSchemaOrField, handler: GetJsonSchemaHandler) -> JsonSchemaValue:
             return {**handler(schema), **json_schema_updates}
 
         metadata = build_metadata_dict(js_functions=[json_schema_update_func])
+
+        # apply alias generator
+        alias_generator = self.config_wrapper.alias_generator
+        if alias_generator and (field_info.alias_priority is None or field_info.alias_priority <= 1):
+            alias = alias_generator(name)
+            if not isinstance(alias, str):
+                raise TypeError(f'alias_generator {alias_generator} must return str, not {alias.__class__}')
+            field_info.alias = alias
+            field_info.validation_alias = alias
+            field_info.serialization_alias = alias
+            field_info.alias_priority = 1
+
+        if isinstance(field_info.validation_alias, (AliasChoices, AliasPath)):
+            validation_alias = field_info.validation_alias.convert_to_aliases()
+        else:
+            validation_alias = field_info.validation_alias
+
         return _common_field(
             schema,
             serialization_exclude=True if field_info.exclude else None,
-            validation_alias=field_info.validation_alias,
+            validation_alias=validation_alias,
             serialization_alias=field_info.serialization_alias,
             frozen=field_info.frozen or field_info.final,
             metadata=metadata,
         )
 
     def _union_schema(self, union_type: Any) -> core_schema.CoreSchema:
         """
@@ -662,25 +660,54 @@
         else:
             s = core_schema.union_schema(choices)
 
         if nullable:
             s = core_schema.nullable_schema(s)
         return s
 
+    def _type_alias_type_schema(
+        self,
+        obj: Any,  # TypeAliasType
+    ) -> CoreSchema:
+        origin = get_origin(obj)
+        if origin is not None and _typing_extra.origin_is_type_alias_type(origin):  # type: ignore
+            origin = cast(Any, origin)
+            ref, schema = self._get_or_cache_recursive_ref(origin)
+            if schema is not None:
+                return schema
+            namespace = (self.types_namespace or {}).copy()
+            new_namespace = {**_typing_extra.get_cls_types_namespace(origin), **namespace}
+            annotation = origin.__value__
+        else:
+            ref, schema = self._get_or_cache_recursive_ref(obj)
+            if schema is not None:
+                return schema
+            namespace = (self.types_namespace or {}).copy()
+            new_namespace = {**_typing_extra.get_cls_types_namespace(obj), **namespace}
+            annotation = obj.__value__
+        self.types_namespace = new_namespace
+        typevars_map = get_standard_typevars_map(obj)
+        annotation = replace_types(annotation, typevars_map)
+        schema = self.generate_schema(annotation)
+        assert schema['type'] != 'definitions'
+        schema['ref'] = ref  # type: ignore
+        self.types_namespace = namespace or None
+        self.recursion_cache[obj] = schema  # type: ignore
+        self.definitions[ref] = schema
+        return schema
+
     def _literal_schema(self, literal_type: Any) -> core_schema.LiteralSchema:
         """
         Generate schema for a Literal.
         """
         expected = _typing_extra.all_literal_values(literal_type)
         assert expected, f'literal "expected" cannot be empty, obj={literal_type}'
         return core_schema.literal_schema(expected)
 
-    def _typed_dict_schema(
-        self, typed_dict_cls: Any, origin: Any
-    ) -> core_schema.TypedDictSchema | core_schema.DefinitionReferenceSchema:
+    def _typed_dict_schema(self, typed_dict_cls: Any, origin: Any) -> core_schema.CoreSchema:
         """
         Generate schema for a TypedDict.
 
         It is not possible to track required/optional keys in TypedDict without __required_keys__
         since TypedDict.__new__ erases the base classes (it replaces them with just `dict`)
         and thus we can track usage of total=True/False
         __required_keys__ was added in Python 3.9
@@ -696,49 +723,57 @@
 
         typevars_map = get_standard_typevars_map(typed_dict_cls)
         if origin is not None:
             typed_dict_cls = origin
 
         if not _SUPPORTS_TYPEDDICT and type(typed_dict_cls).__module__ == 'typing':
             raise PydanticUserError(
-                'Please use `typing_extensions.TypedDict` instead of `typing.TypedDict` on Python < 3.11.',
+                'Please use `typing_extensions.TypedDict` instead of `typing.TypedDict` on Python < 3.12.',
                 code='typed-dict-version',
             )
 
+        config: ConfigDict | None = getattr(typed_dict_cls, '__pydantic_config__', None)
+        config_wrapper = ConfigWrapper(config)
+        core_config = config_wrapper.core_config(None)
+
         required_keys: frozenset[str] = typed_dict_cls.__required_keys__
 
         fields: dict[str, core_schema.TypedDictField] = {}
 
+        decorators = DecoratorInfos.build(typed_dict_cls)
+
         for field_name, annotation in get_type_hints_infer_globalns(
             typed_dict_cls, localns=self.types_namespace, include_extras=True
         ).items():
             annotation = replace_types(annotation, typevars_map)
             required = field_name in required_keys
 
             if get_origin(annotation) == _typing_extra.Required:
                 required = True
                 annotation = get_args(annotation)[0]
             elif get_origin(annotation) == _typing_extra.NotRequired:
                 required = False
                 annotation = get_args(annotation)[0]
 
             field_info = FieldInfo.from_annotation(annotation)
-            fields[field_name] = self._generate_td_field_schema(
-                field_name, field_info, DecoratorInfos(), required=required
-            )
+            fields[field_name] = self._generate_td_field_schema(field_name, field_info, decorators, required=required)
 
         metadata = build_metadata_dict(js_functions=[partial(modify_model_json_schema, cls=typed_dict_cls)])
 
-        return core_schema.typed_dict_schema(
+        td_schema = core_schema.typed_dict_schema(
             fields,
             extra_behavior='forbid',
             ref=typed_dict_ref,
             metadata=metadata,
+            config=core_config,
         )
 
+        schema = self._apply_model_serializers(td_schema, decorators.model_serializers.values())
+        return apply_model_validators(schema, decorators.model_validators.values(), 'all')
+
     def _namedtuple_schema(self, namedtuple_cls: Any) -> core_schema.CallSchema:
         """
         Generate schema for a NamedTuple.
         """
         annotations: dict[str, Any] = get_type_hints_infer_globalns(
             namedtuple_cls, include_extras=True, localns=self.types_namespace
         )
@@ -767,15 +802,16 @@
         Prepare a ArgumentsParameter to represent a field in a namedtuple or function signature.
         """
         if default is Parameter.empty:
             field = FieldInfo.from_annotation(annotation)
         else:
             field = FieldInfo.from_annotated_attribute(annotation, default)
         assert field.annotation is not None, 'field.annotation should not be None when generating a schema'
-        schema = self._apply_annotations(CallbackGetCoreSchemaHandler(self.generate_schema), annotation, field.metadata)
+        source_type, annotations = field.annotation, field.metadata
+        schema = self._apply_annotations(lambda x: x, source_type, annotations)
 
         if not field.is_required():
             schema = wrap_default(field, schema)
 
         parameter_schema = core_schema.arguments_parameter(name, schema)
         if mode is not None:
             parameter_schema['mode'] = mode
@@ -783,40 +819,14 @@
             parameter_schema['alias'] = field.alias
         else:
             alias_generator = self.config_wrapper.alias_generator
             if alias_generator:
                 parameter_schema['alias'] = alias_generator(name)
         return parameter_schema
 
-    def _generic_collection_schema(
-        self, parent_type: type[Any], type_: type[Any], origin: type[Any]
-    ) -> core_schema.CoreSchema:
-        """
-        Generate schema for List, Set, and FrozenSet, possibly parameterized.
-
-        :param parent_type: Either `list`, `set` or `frozenset` - the builtin type
-        :param type_: The type of the collection, e.g. `List[int]` or `List`, or a subclass of one of them
-        :param origin: The origin type
-        """
-        schema: core_schema.CoreSchema = {  # type: ignore[misc,assignment]
-            'type': parent_type.__name__.lower(),
-            'items_schema': self.generate_schema(get_first_arg(type_)),
-        }
-
-        if origin == parent_type:
-            return schema
-        else:
-            # Ensure the validated value is converted back to the specific subclass type
-            # NOTE: we might have better performance by using a tuple or list validator for the schema here,
-            # but if you care about performance, you can define your own schema.
-            # We should optimize for compatibility, not performance in this case
-            return core_schema.general_after_validator_function(
-                lambda __input_value, __info: type_(__input_value), schema
-            )
-
     def _tuple_schema(self, tuple_type: Any) -> core_schema.CoreSchema:
         """
         Generate schema for a Tuple, e.g. `tuple[int, str]` or `tuple[int, ...]`.
         """
         params = get_args(tuple_type)
         # NOTE: subtle difference: `tuple[()]` gives `params=()`, whereas `typing.Tuple[()]` gives `params=((),)`
         if not params:
@@ -837,84 +847,14 @@
             )
         elif len(params) == 1 and params[0] == ():
             # special case for `Tuple[()]` which means `Tuple[]` - an empty tuple
             return core_schema.tuple_positional_schema([])
         else:
             return core_schema.tuple_positional_schema([self.generate_schema(p) for p in params])
 
-    def _dict_schema(self, dict_type: Any) -> core_schema.DictSchema:
-        """
-        Generate schema for a Dict, e.g. `dict[str, int]`.
-        """
-        try:
-            arg0, arg1 = get_args(dict_type)
-        except ValueError:
-            return core_schema.dict_schema()
-        else:
-            return core_schema.dict_schema(
-                keys_schema=self.generate_schema(arg0),
-                values_schema=self.generate_schema(arg1),
-            )
-
-    def _dict_subclass_schema(self, dict_subclass: Any) -> core_schema.CoreSchema:
-        """
-        Generate schema for a subclass of dict or Dict
-        """
-        try:
-            arg0, arg1 = get_args(dict_subclass)
-        except ValueError:
-            arg0, arg1 = Any, Any
-
-        from ._validators import mapping_validator
-
-        # TODO could do `core_schema.chain_schema(core_schema.is_instance_schema(dict_subclass), ...` in strict mode
-        return core_schema.no_info_wrap_validator_function(
-            mapping_validator,
-            core_schema.dict_schema(
-                keys_schema=self.generate_schema(arg0),
-                values_schema=self.generate_schema(arg1),
-            ),
-        )
-
-    def _counter_schema(self, counter_type: Any) -> core_schema.CoreSchema:
-        """
-        Generate schema for `typing.Counter`
-        """
-        arg = get_first_arg(counter_type)
-
-        from ._validators import construct_counter
-
-        # TODO could do `core_schema.chain_schema(core_schema.is_instance_schema(Counter), ...` in strict mode
-        return core_schema.no_info_after_validator_function(
-            construct_counter,
-            core_schema.dict_schema(
-                keys_schema=self.generate_schema(arg),
-                values_schema=core_schema.int_schema(),
-            ),
-        )
-
-    def _mapping_schema(self, mapping_type: Any) -> core_schema.CoreSchema:
-        """
-        Generate schema for a Dict, e.g. `dict[str, int]`.
-        """
-        try:
-            arg0, arg1 = get_args(mapping_type)
-        except ValueError:
-            return core_schema.is_instance_schema(typing.Mapping, cls_repr='Mapping')
-        else:
-            from ._validators import mapping_validator
-
-            return core_schema.no_info_wrap_validator_function(
-                mapping_validator,
-                core_schema.dict_schema(
-                    keys_schema=self.generate_schema(arg0),
-                    values_schema=self.generate_schema(arg1),
-                ),
-            )
-
     def _type_schema(self) -> core_schema.CoreSchema:
         return core_schema.custom_error_schema(
             core_schema.is_instance_schema(type),
             custom_error_type='is_type',
             custom_error_message='Input should be a type',
         )
 
@@ -939,45 +879,46 @@
 
     def _sequence_schema(self, sequence_type: Any) -> core_schema.CoreSchema:
         """
         Generate schema for a Sequence, e.g. `Sequence[int]`.
         """
         item_type = get_first_arg(sequence_type)
 
-        if item_type == Any:
-            return core_schema.is_instance_schema(typing.Sequence, cls_repr='Sequence')
-        else:
+        def json_schema_func(_schema: CoreSchemaOrField, handler: GetJsonSchemaHandler) -> JsonSchemaValue:
+            items_schema = self._generate_schema(item_type)
+            return handler(core_schema.list_schema(items_schema))
+
+        metadata = build_metadata_dict(js_functions=[json_schema_func])
+
+        list_schema = core_schema.list_schema(self.generate_schema(item_type))
+        python_schema = core_schema.is_instance_schema(typing.Sequence, cls_repr='Sequence')
+        if item_type != Any:
             from ._validators import sequence_validator
 
-            return core_schema.chain_schema(
-                [
-                    core_schema.is_instance_schema(typing.Sequence, cls_repr='Sequence'),
-                    core_schema.no_info_wrap_validator_function(
-                        sequence_validator,
-                        core_schema.list_schema(self.generate_schema(item_type), allow_any_iter=True),
-                    ),
-                ]
+            python_schema = core_schema.chain_schema(
+                [python_schema, core_schema.no_info_wrap_validator_function(sequence_validator, list_schema)],
             )
+        return core_schema.json_or_python_schema(
+            json_schema=list_schema, python_schema=python_schema, metadata=metadata
+        )
 
     def _iterable_schema(self, type_: Any) -> core_schema.GeneratorSchema:
         """
         Generate a schema for an `Iterable`.
-
-        TODO replace with pydantic-core's generator validator.
         """
         item_type = get_first_arg(type_)
 
         return core_schema.generator_schema(self.generate_schema(item_type))
 
     def _pattern_schema(self, pattern_type: Any) -> core_schema.CoreSchema:
-        from . import _serializers, _validators
+        from . import _validators
 
         metadata = build_metadata_dict(js_functions=[lambda _1, _2: {'type': 'string', 'format': 'regex'}])
         ser = core_schema.plain_serializer_function_ser_schema(
-            _serializers.pattern_serializer, info_arg=True, json_return_type='str'
+            attrgetter('pattern'), when_used='json', return_schema=core_schema.str_schema()
         )
         if pattern_type == typing.Pattern or pattern_type == re.Pattern:
             # bare type
             return core_schema.no_info_plain_validator_function(
                 _validators.pattern_either_validator, serialization=ser, metadata=metadata
             )
 
@@ -996,35 +937,14 @@
     def _hashable_schema(self) -> core_schema.CoreSchema:
         return core_schema.custom_error_schema(
             core_schema.is_instance_schema(collections.abc.Hashable),
             custom_error_type='is_hashable',
             custom_error_message='Input should be hashable',
         )
 
-    def _std_types_schema(self, obj: Any) -> core_schema.CoreSchema | None:
-        """
-        Generate schema for types in the standard library.
-        """
-        if not isinstance(obj, type):
-            return None
-
-        # Import here to avoid the extra import time earlier since _std_validators imports lots of things globally
-        from ._std_types_schema import SCHEMA_LOOKUP
-
-        # instead of iterating over a list and calling is_instance, this should be somewhat faster,
-        # especially as it should catch most types on the first iteration
-        # (same as we do/used to do in json encoding)
-        for base in obj.__mro__[:-1]:
-            try:
-                encoder = SCHEMA_LOOKUP[base]
-            except KeyError:
-                continue
-            return encoder(self, obj)
-        return None
-
     def _dataclass_schema(
         self, dataclass: type[StandardDataclass], origin: type[StandardDataclass] | None
     ) -> core_schema.CoreSchema:
         """
         Generate schema for a dataclass.
         """
         dataclass_ref, schema = self._get_or_cache_recursive_ref(dataclass)
@@ -1044,38 +964,59 @@
                     field.apply_typevars_map(typevars_map, self.types_namespace)
         else:
             fields = collect_dataclass_fields(
                 dataclass,
                 self.types_namespace,
                 typevars_map=typevars_map,
             )
-        decorators = getattr(dataclass, '__pydantic_decorators__', None) or DecoratorInfos()
-        args = [self._generate_dc_field_schema(k, v, decorators) for k, v in fields.items()]
+        decorators = dataclass.__dict__.get('__pydantic_decorators__') or DecoratorInfos.build(dataclass)
+        # Move kw_only=False args to the start of the list, as this is how vanilla dataclasses work.
+        # Note that when kw_only is missing or None, it is treated as equivalent to kw_only=True
+        args = sorted(
+            (self._generate_dc_field_schema(k, v, decorators) for k, v in fields.items()),
+            key=lambda a: a.get('kw_only') is not False,
+        )
         has_post_init = hasattr(dataclass, '__post_init__')
+        has_slots = hasattr(dataclass, '__slots__')
 
         config = getattr(dataclass, '__pydantic_config__', None)
         if config is not None:
             config_wrapper = ConfigWrapper(config, check=False)
             self._config_wrapper_stack.append(config_wrapper)
+            core_config = config_wrapper.core_config(dataclass)
+        else:
+            core_config = None
 
         try:
             args_schema = core_schema.dataclass_args_schema(
                 dataclass.__name__,
                 args,
-                computed_fields=generate_computed_field(decorators.computed_fields),
+                computed_fields=[self._computed_field_schema(d) for d in decorators.computed_fields.values()],
                 collect_init_only=has_post_init,
             )
         finally:
             if config is not None:
                 self._config_wrapper_stack.pop()
 
-        inner_schema = apply_validators(args_schema, decorators.root_validator.values())
-        dc_schema = core_schema.dataclass_schema(dataclass, inner_schema, post_init=has_post_init, ref=dataclass_ref)
-        schema = apply_model_serializers(dc_schema, decorators.model_serializer.values())
-        return apply_model_validators(schema, decorators.model_validator.values())
+        inner_schema = apply_validators(args_schema, decorators.root_validators.values())
+
+        model_validators = decorators.model_validators.values()
+        inner_schema = apply_model_validators(inner_schema, model_validators, 'inner')
+
+        dc_schema = core_schema.dataclass_schema(
+            dataclass,
+            inner_schema,
+            post_init=has_post_init,
+            ref=dataclass_ref,
+            fields=[field.name for field in dataclasses.fields(dataclass)],
+            slots=has_slots,
+            config=core_config,
+        )
+        schema = self._apply_model_serializers(dc_schema, decorators.model_serializers.values())
+        return apply_model_validators(schema, model_validators, 'outer')
 
     def _callable_schema(self, function: Callable[..., Any]) -> core_schema.CallSchema:
         """
         Generate schema for a Callable.
 
         TODO support functional validators once we support them in Config
         """
@@ -1141,89 +1082,242 @@
         obj_ref = get_type_ref(cls)
         if obj_ref in self.recursion_cache:
             return obj_ref, self.recursion_cache[obj_ref]
         else:
             self.recursion_cache[obj_ref] = core_schema.definition_reference_schema(obj_ref)
             return obj_ref, None
 
+    def _computed_field_schema(self, d: Decorator[ComputedFieldInfo]) -> core_schema.ComputedField:
+        return_type_schema = self.generate_schema(d.info.return_type)
+
+        # Handle alias_generator using similar logic to that from
+        # pydantic._internal._generate_schema.GenerateSchema._common_field_schema,
+        # with field_info -> d.info and name -> d.cls_var_name
+        alias_generator = self.config_wrapper.alias_generator
+        if alias_generator and (d.info.alias_priority is None or d.info.alias_priority <= 1):
+            alias = alias_generator(d.cls_var_name)
+            if not isinstance(alias, str):
+                raise TypeError(f'alias_generator {alias_generator} must return str, not {alias.__class__}')
+            d.info.alias = alias
+            d.info.alias_priority = 1
+
+        return core_schema.computed_field(d.cls_var_name, return_schema=return_type_schema, alias=d.info.alias)
+
     def _annotated_schema(self, annotated_type: Any) -> core_schema.CoreSchema:
         """
         Generate schema for an Annotated type, e.g. `Annotated[int, Field(...)]` or `Annotated[int, Gt(0)]`.
         """
-        first_arg, *other_args = get_args(annotated_type)
-        return self._apply_annotations(CallbackGetCoreSchemaHandler(self.generate_schema), first_arg, other_args)
-
-    def _get_prepare_pydantic_annotations_for_known_type(self, obj: Any) -> Callable[..., Any] | None:
-        from decimal import Decimal
-
-        from . import _std_types_schema as std_types
+        source_type, *annotations = get_args(annotated_type)
+        schema = self._apply_annotations(lambda x: x, source_type, annotations)
+        # put the default validator last so that TypeAdapter.get_default_value() works
+        # even if there are function validators involved
+        for annotation in annotations:
+            if isinstance(annotation, FieldInfo):
+                schema = wrap_default(annotation, schema)
+        return schema
 
-        if obj is Decimal:
-            return std_types.decimal_prepare_pydantic_annotations
+    def _get_prepare_pydantic_annotations_for_known_type(
+        self, obj: Any, annotations: tuple[Any, ...]
+    ) -> tuple[Any, list[Any]] | None:
+        from ._std_types_schema import PREPARE_METHODS
+
+        for gen in PREPARE_METHODS:
+            res = gen(obj, annotations, self.config_wrapper.config_dict)
+            if res is not None:
+                return res
 
         return None
 
     def _prepare_annotations(self, source_type: Any, annotations: Iterable[Any]) -> tuple[Any, list[Any]]:
         """
         Call `__prepare_pydantic_annotations__` if it exists and return a tuple of (new_source_type, new_annotations).
 
         This should be treated conceptually similar to the transformation
         `Annotated[source_type, *annotations]` -> `Annotated[new_source_type, *new_annotations]`
         """
+
         prepare = getattr(source_type, '__prepare_pydantic_annotations__', None)
-        if prepare is None:
-            # check if this is one of our "known" types
-            prepare = self._get_prepare_pydantic_annotations_for_known_type(source_type)
+
+        annotations = tuple(annotations)  # make them immutable to avoid confusion over mutating them
 
         if prepare is not None:
-            # make annotations a tuple to error if it gets mutated
-            # make the return type a list to support generators or returning a sequence
-            res = list(prepare(source_type, tuple(annotations)))
-            if not res:
-                raise PydanticSchemaGenerationError(
-                    f'The type {source_type} that implements `__prepare_pydantic_annotations__`'
-                    ' returned no annotations when called.'
-                    ' Custom types must return at least 1 item since the first item is the replacement source type.'
-                )
-            source_type, *annotations = res
-        return (source_type, list(annotations))
+            source_type, annotations = prepare(source_type, tuple(annotations), self.config_wrapper.config_dict)
+            annotations = list(annotations)
+        else:
+            res = self._get_prepare_pydantic_annotations_for_known_type(source_type, annotations)
+            if res is not None:
+                source_type, annotations = res
+
+        return source_type, list(annotations)
 
     def _apply_annotations(
         self,
-        get_inner_schema: GetCoreSchemaHandler,
+        transform_inner_schema: Callable[[CoreSchema], CoreSchema],
         source_type: Any,
-        annotations: typing.Iterable[Any],
+        annotations: list[Any],
     ) -> CoreSchema:
         """
         Apply arguments from `Annotated` or from `FieldInfo` to a schema.
 
         This gets called by `GenerateSchema._annotated_schema` but differs from it in that it does
         not expect `source_type` to be an `Annotated` object, it expects it to be  the first argument of that
         (in other words, `GenerateSchema._annotated_schema` just unpacks `Annotated`, this process it).
         """
-        source_type, annotations = self._prepare_annotations(source_type, annotations)
-
+        # expand annotations before we start processing them so that `__prepare_pydantic_annotations` can consume
+        # individual items from GroupedMetadata
+        annotations = list(_known_annotated_metadata.expand_grouped_metadata(annotations))
         idx = -1
+        prepare = getattr(source_type, '__prepare_pydantic_annotations__', None)
+        if prepare:
+            source_type, annotations = prepare(source_type, tuple(annotations), self.config_wrapper.config_dict)
+            annotations = list(annotations)
+        else:
+            res = self._get_prepare_pydantic_annotations_for_known_type(source_type, tuple(annotations))
+            if res is not None:
+                source_type, annotations = res
+
+        pydantic_js_functions: list[GetJsonSchemaFunction] = []
+
+        def inner_handler(obj: Any) -> CoreSchema:
+            if isinstance(obj, type(Annotated[int, 123])):
+                schema = transform_inner_schema(self._annotated_schema(obj))
+            else:
+                from_property = self._generate_schema_from_property(obj, obj)
+                if from_property is None:
+                    schema = self._generate_schema(obj)
+                else:
+                    schema = from_property
+                metadata_js_function = _extract_get_pydantic_json_schema(obj, schema)
+                if metadata_js_function is not None:
+                    pydantic_js_functions.append(metadata_js_function)
+            return transform_inner_schema(schema)
+
+        get_inner_schema = CallbackGetCoreSchemaHandler(inner_handler, self.generate_schema)
+
         while True:
             idx += 1
             if idx == len(annotations):
                 break
             annotation = annotations[idx]
             if annotation is None:
                 continue
             prepare = getattr(annotation, '__prepare_pydantic_annotations__', None)
             if prepare is not None:
                 previous = annotations[:idx]
-                remaining = annotations[idx:]
-                remaining = list(prepare(source_type, tuple(remaining)))
-                annotations = previous + remaining
+                remaining = annotations[idx + 1 :]
+                new_source_type, remaining = prepare(source_type, tuple(remaining), self.config_wrapper.config_dict)
+                annotations = previous + list(remaining)
+                if new_source_type is not source_type:
+                    return self._apply_annotations(
+                        transform_inner_schema,
+                        new_source_type,
+                        annotations,
+                    )
             annotation = annotations[idx]
-            get_inner_schema = get_wrapped_inner_schema(get_inner_schema, annotation, self.definitions)
+            get_inner_schema = self._get_wrapped_inner_schema(
+                get_inner_schema, annotation, self.definitions, pydantic_js_functions
+            )
+
+        schema = get_inner_schema(source_type)
+        metadata = CoreMetadataHandler(schema).metadata
+        metadata.setdefault('pydantic_js_functions', []).extend(pydantic_js_functions)
+        return schema
+
+    def _get_wrapped_inner_schema(
+        self,
+        get_inner_schema: GetCoreSchemaHandler,
+        annotation: Any,
+        definitions: dict[str, core_schema.CoreSchema],
+        pydantic_js_functions: list[GetJsonSchemaFunction],
+    ) -> CallbackGetCoreSchemaHandler:
+        metadata_get_schema: GetCoreSchemaFunction = getattr(annotation, '__get_pydantic_core_schema__', None) or (
+            lambda source, handler: handler(source)
+        )
+
+        def new_handler(source: Any) -> core_schema.CoreSchema:
+            schema = metadata_get_schema(source, get_inner_schema)
+            schema = apply_single_annotation(schema, annotation, definitions)
+
+            metadata_js_function = _extract_get_pydantic_json_schema(annotation, schema)
+            if metadata_js_function is not None:
+                pydantic_js_functions.append(metadata_js_function)
+            return schema
+
+        return CallbackGetCoreSchemaHandler(new_handler, self.generate_schema)
+
+    def _apply_field_serializers(
+        self, schema: core_schema.CoreSchema, serializers: list[Decorator[FieldSerializerDecoratorInfo]]
+    ) -> core_schema.CoreSchema:
+        """
+        Apply field serializers to a schema.
+        """
+        if serializers:
+            # use the last serializer to make it easy to override a serializer set on a parent model
+            serializer = serializers[-1]
+            is_field_serializer, info_arg = inspect_field_serializer(serializer.func, serializer.info.mode)
+
+            if serializer.info.return_type is None:
+                return_schema = None
+            else:
+                return_schema = self.generate_schema(serializer.info.return_type)
+
+            if serializer.info.mode == 'wrap':
+                schema['serialization'] = core_schema.wrap_serializer_function_ser_schema(
+                    serializer.func,
+                    is_field_serializer=is_field_serializer,
+                    info_arg=info_arg,
+                    return_schema=return_schema,
+                    when_used=serializer.info.when_used,
+                )
+            else:
+                assert serializer.info.mode == 'plain'
+                schema['serialization'] = core_schema.plain_serializer_function_ser_schema(
+                    serializer.func,
+                    is_field_serializer=is_field_serializer,
+                    info_arg=info_arg,
+                    return_schema=return_schema,
+                    when_used=serializer.info.when_used,
+                )
+        return schema
+
+    def _apply_model_serializers(
+        self, schema: core_schema.CoreSchema, serializers: Iterable[Decorator[ModelSerializerDecoratorInfo]]
+    ) -> core_schema.CoreSchema:
+        """
+        Apply model serializers to a schema.
+        """
+        ref: str | None = schema.pop('ref', None)  # type: ignore
+        if serializers:
+            serializer = list(serializers)[-1]
+            info_arg = inspect_model_serializer(serializer.func, serializer.info.mode)
+
+            if serializer.info.return_type is None:
+                return_schema = None
+            else:
+                return_schema = self.generate_schema(serializer.info.return_type)
 
-        return get_inner_schema(source_type)
+            if serializer.info.mode == 'wrap':
+                ser_schema: core_schema.SerSchema = core_schema.wrap_serializer_function_ser_schema(
+                    serializer.func,
+                    info_arg=info_arg,
+                    return_schema=return_schema,
+                    when_used=serializer.info.when_used,
+                )
+            else:
+                # plain
+                ser_schema = core_schema.plain_serializer_function_ser_schema(
+                    serializer.func,
+                    info_arg=info_arg,
+                    return_schema=return_schema,
+                    when_used=serializer.info.when_used,
+                )
+            schema['serialization'] = ser_schema
+        if ref:
+            schema['ref'] = ref  # type: ignore
+        return schema
 
 
 _VALIDATOR_F_MATCH: Mapping[
     tuple[FieldValidatorModes, Literal['no-info', 'general', 'field']],
     Callable[[Callable[..., Any], core_schema.CoreSchema], core_schema.CoreSchema],
 ] = {
     ('before', 'no-info'): core_schema.no_info_before_validator_function,
@@ -1275,77 +1369,32 @@
     """
     for validator in validators:
         if validator.info.always:
             return True
     return False
 
 
-def apply_field_serializers(
-    schema: core_schema.CoreSchema, serializers: list[Decorator[FieldSerializerDecoratorInfo]]
-) -> core_schema.CoreSchema:
-    """
-    Apply field serializers to a schema.
-    """
-    if serializers:
-        # use the last serializer to make it easy to override a serializer set on a parent model
-        serializer = serializers[-1]
-        is_field_serializer, info_arg = inspect_field_serializer(serializer.func, serializer.info.mode)
-        if serializer.info.mode == 'wrap':
-            schema['serialization'] = core_schema.wrap_serializer_function_ser_schema(
-                serializer.func,
-                is_field_serializer=is_field_serializer,
-                info_arg=info_arg,
-                json_return_type=serializer.info.json_return_type,
-                when_used=serializer.info.when_used,
-            )
-        else:
-            assert serializer.info.mode == 'plain'
-            schema['serialization'] = core_schema.plain_serializer_function_ser_schema(
-                serializer.func,
-                is_field_serializer=is_field_serializer,
-                info_arg=info_arg,
-                json_return_type=serializer.info.json_return_type,
-                when_used=serializer.info.when_used,
-            )
-    return schema
-
-
-def apply_model_serializers(
-    schema: core_schema.CoreSchema, serializers: Iterable[Decorator[ModelSerializerDecoratorInfo]]
-) -> core_schema.CoreSchema:
-    """
-    Apply model serializers to a schema.
-    """
-    if serializers:
-        serializer = list(serializers)[-1]
-        info_arg = inspect_model_serializer(serializer.func, serializer.info.mode)
-        if serializer.info.mode == 'wrap':
-            ser_schema: core_schema.SerSchema = core_schema.wrap_serializer_function_ser_schema(
-                serializer.func,
-                info_arg=info_arg,
-                json_return_type=serializer.info.json_return_type,
-            )
-        else:
-            # plain
-            ser_schema = core_schema.plain_serializer_function_ser_schema(
-                serializer.func,
-                info_arg=info_arg,
-                json_return_type=serializer.info.json_return_type,
-            )
-        schema['serialization'] = ser_schema
-    return schema
-
-
 def apply_model_validators(
-    schema: core_schema.CoreSchema, validators: Iterable[Decorator[ModelValidatorDecoratorInfo]]
+    schema: core_schema.CoreSchema,
+    validators: Iterable[Decorator[ModelValidatorDecoratorInfo]],
+    mode: Literal['inner', 'outer', 'all'],
 ) -> core_schema.CoreSchema:
     """
     Apply model validators to a schema.
+
+    If mode == 'inner', only "before" validators are applied
+    If mode == 'outer', validators other than "before" are applied
+    If mode == 'all', all validators are applied
     """
+    ref: str | None = schema.pop('ref', None)  # type: ignore
     for validator in validators:
+        if mode == 'inner' and validator.info.mode != 'before':
+            continue
+        if mode == 'outer' and validator.info.mode == 'before':
+            continue
         info_arg = inspect_validator(validator.func, validator.info.mode)
         if validator.info.mode == 'wrap':
             if info_arg:
                 schema = core_schema.general_wrap_validator_function(function=validator.func, schema=schema)
             else:
                 schema = core_schema.no_info_wrap_validator_function(function=validator.func, schema=schema)
         elif validator.info.mode == 'before':
@@ -1355,64 +1404,38 @@
                 schema = core_schema.no_info_before_validator_function(function=validator.func, schema=schema)
         else:
             assert validator.info.mode == 'after'
             if info_arg:
                 schema = core_schema.general_after_validator_function(function=validator.func, schema=schema)
             else:
                 schema = core_schema.no_info_after_validator_function(function=validator.func, schema=schema)
+    if ref:
+        schema['ref'] = ref  # type: ignore
     return schema
 
 
-def get_wrapped_inner_schema(
-    get_inner_schema: GetCoreSchemaHandler, annotation: Any, definitions: dict[str, core_schema.CoreSchema]
-) -> CallbackGetCoreSchemaHandler:
-    metadata_get_schema: GetCoreSchemaFunction = getattr(annotation, '__get_pydantic_core_schema__', None) or (
-        lambda source, handler: handler(source)
-    )
-
-    def new_handler(source: Any) -> core_schema.CoreSchema:
-        schema = metadata_get_schema(source, get_inner_schema)
-        schema = apply_single_annotation(schema, annotation, definitions)
-
-        metadata_js_function = _extract_get_pydantic_json_schema(annotation)
-        if metadata_js_function is not None:
-            metadata = CoreMetadataHandler(schema).metadata
-            metadata['pydantic_js_functions'] = metadata.get('pydantic_js_functions', [])
-            metadata['pydantic_js_functions'].append(metadata_js_function)
-        return schema
-
-    return CallbackGetCoreSchemaHandler(new_handler)
-
-
 def apply_single_annotation(
     schema: core_schema.CoreSchema, metadata: Any, definitions: dict[str, core_schema.CoreSchema]
 ) -> core_schema.CoreSchema:
     if isinstance(metadata, FieldInfo):
         for field_metadata in metadata.metadata:
             schema = apply_single_annotation(schema, field_metadata, definitions)
         if metadata.discriminator is not None:
             schema = _discriminated_union.apply_discriminator(schema, metadata.discriminator, definitions)
-        # TODO setting a default here needs to be tested
-        return wrap_default(metadata, schema)
-    # note that we ignore any unrecognized metadata
-    # PEP 593: "If a library (or tool) encounters a typehint Annotated[T, x] and has no
-    # special logic for metadata x, it should ignore it and simply treat the type as T."
-    # Allow, but ignore, any unknown metadata.
-    metadata_dict, _ = _known_annotated_metadata.collect_known_metadata([metadata])
-
-    if not metadata_dict:
         return schema
 
     if schema['type'] == 'nullable':
         # for nullable schemas, metadata is automatically applied to the inner schema
-        # TODO need to do the same for lists, tuples and more
-        schema['schema'].update(metadata_dict)
-    else:
-        schema.update(metadata_dict)  # type: ignore[typeddict-item]
-    return schema
+        inner = schema.get('schema', core_schema.any_schema())
+        inner = apply_single_annotation(inner, metadata, definitions)
+        if inner:
+            schema['schema'] = inner
+        return schema
+
+    return _known_annotated_metadata.apply_known_metadata(metadata, schema.copy())
 
 
 def wrap_default(field_info: FieldInfo, schema: core_schema.CoreSchema) -> core_schema.CoreSchema:
     if field_info.default_factory:
         return core_schema.with_default_schema(
             schema, default_factory=field_info.default_factory, validate_default=field_info.validate_default
         )
@@ -1430,35 +1453,46 @@
     """
     try:
         return get_args(type_)[0]
     except IndexError:
         return Any
 
 
-def _extract_get_pydantic_json_schema(tp: Any) -> GetJsonSchemaFunction | None:
+def _extract_get_pydantic_json_schema(tp: Any, schema: CoreSchema) -> GetJsonSchemaFunction | None:
     """Extract `__get_pydantic_json_schema__` from a type, handling the deprecated `__modify_schema__`"""
     js_modify_function = getattr(tp, '__get_pydantic_json_schema__', None)
 
     if js_modify_function is None and hasattr(tp, '__modify_schema__'):
         warnings.warn(
             'The __modify_schema__ method is deprecated, use __get_pydantic_json_schema__ instead',
             DeprecationWarning,
         )
         return lambda c, h: tp.__modify_schema__(h(c))
 
+    # handle GenericAlias' but ignore Annotated which "lies" about it's origin (in this case it would be `int`)
+    if hasattr(tp, '__origin__') and not isinstance(tp, type(Annotated[int, 'placeholder'])):
+        return _extract_get_pydantic_json_schema(tp.__origin__, schema)
+
+    if js_modify_function is None:
+        return None
+
+    # wrap the schema so that we unpack ref schemas and always call metadata_js_function with the full schema
+    if schema['type'] != 'definition-ref':
+        # we would fail to unpack recursive ref schemas!
+        js_modify_function = wrap_json_schema_fn_for_model_or_custom_type_with_ref_unpacking(js_modify_function)
     return js_modify_function
 
 
 class _CommonField(TypedDict):
     schema: core_schema.CoreSchema
     validation_alias: str | list[str | int] | list[list[str | int]] | None
     serialization_alias: str | None
     serialization_exclude: bool | None
     frozen: bool | None
-    metadata: Any
+    metadata: dict[str, Any]
 
 
 def _common_field(
     schema: core_schema.CoreSchema,
     *,
     validation_alias: str | list[str | int] | list[list[str | int]] | None = None,
     serialization_alias: str | None = None,
@@ -1470,19 +1504,7 @@
         'schema': schema,
         'validation_alias': validation_alias,
         'serialization_alias': serialization_alias,
         'serialization_exclude': serialization_exclude,
         'frozen': frozen,
         'metadata': metadata,
     }
-
-
-def generate_computed_field(d: dict[str, Decorator[ComputedFieldInfo]]) -> list[core_schema.ComputedField] | None:
-    r = [
-        core_schema.computed_field(
-            d.cls_var_name,
-            json_return_type=d.info.json_return_type,
-            alias=d.info.alias,
-        )
-        for d in d.values()
-    ]
-    return r
```

### Comparing `pydantic-2.0a4/pydantic/_internal/_generics.py` & `pydantic-2.0b1/pydantic/_internal/_generics.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,16 +21,16 @@
     from typing import _UnionGenericAlias  # type: ignore[attr-defined]
 
 if TYPE_CHECKING:
     from ..main import BaseModel
 
 GenericTypesCacheKey = Tuple[Any, Any, Tuple[Any, ...]]
 
-# TODO: We want to remove LimitedDict, but to do this, we'll need to improve the handling of generics caching
-#   Right now, to handle recursive generics, we some types must remain cached for brief periods without references
+# Note: We want to remove LimitedDict, but to do this, we'd need to improve the handling of generics caching.
+#   Right now, to handle recursive generics, we some types must remain cached for brief periods without references.
 #   By chaining the WeakValuesDict with a LimitedDict, we have a way to retain caching for all types with references,
 #   while also retaining a limited number of types even without references. This is generally enough to build
 #   specific recursive generic models without losing required items out of the cache.
 
 KT = TypeVar('KT')
 VT = TypeVar('VT')
 _LIMITED_DICT_SIZE = 100
```

### Comparing `pydantic-2.0a4/pydantic/_internal/_repr.py` & `pydantic-2.0b1/pydantic/_internal/_repr.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,41 +58,43 @@
         return self.__class__.__name__
 
     def __repr_str__(self, join_str: str) -> str:
         return join_str.join(repr(v) if a is None else f'{a}={v!r}' for a, v in self.__repr_args__())
 
     def __pretty__(self, fmt: typing.Callable[[Any], Any], **kwargs: Any) -> typing.Generator[Any, None, None]:
         """
-        Used by devtools (https://python-devtools.helpmanual.io/) to provide a human-readable representations of objects
+        Used by devtools (https://python-devtools.helpmanual.io/) to pretty print objects.
         """
         yield self.__repr_name__() + '('
         yield 1
         for name, value in self.__repr_args__():
             if name is not None:
                 yield name + '='
             yield fmt(value)
             yield ','
             yield 0
         yield -1
         yield ')'
 
-    def __str__(self) -> str:
-        return self.__repr_str__(' ')
-
-    def __repr__(self) -> str:
-        return f'{self.__repr_name__()}({self.__repr_str__(", ")})'
-
     def __rich_repr__(self) -> RichReprResult:
-        """Get fields for Rich library"""
+        """
+        Used by Rich (https://rich.readthedocs.io/en/stable/pretty.html) to pretty print objects.
+        """
         for name, field_repr in self.__repr_args__():
             if name is None:
                 yield field_repr
             else:
                 yield name, field_repr
 
+    def __str__(self) -> str:
+        return self.__repr_str__(' ')
+
+    def __repr__(self) -> str:
+        return f'{self.__repr_name__()}({self.__repr_str__(", ")})'
+
 
 def display_as_type(obj: Any) -> str:
     """
     Pretty representation of a type, should be as close as possible to the original type definition string.
 
     Takes some logic from `typing._type_repr`.
     """
```

### Comparing `pydantic-2.0a4/pydantic/_internal/_typing_extra.py` & `pydantic-2.0b1/pydantic/_internal/_typing_extra.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import types
 import typing
 from collections.abc import Callable
 from functools import partial
 from types import GetSetDescriptorType
 from typing import TYPE_CHECKING, Any, ForwardRef
 
-from typing_extensions import Annotated, Final, Literal, TypeGuard, get_args, get_origin
+from typing_extensions import Annotated, Final, Literal, TypeAliasType, TypeGuard, get_args, get_origin
 
 if TYPE_CHECKING:
     from ._dataclasses import StandardDataclass
 
 try:
     from typing import _TypingBase  # type: ignore[attr-defined]
 except ImportError:
@@ -53,62 +53,37 @@
     WithArgsTypes = typing._GenericAlias, types.GenericAlias, types.UnionType  # type: ignore[attr-defined]
 
 
 if sys.version_info < (3, 10):
     NoneType = type(None)
     EllipsisType = type(Ellipsis)
 else:
-    from types import EllipsisType as EllipsisType  # noqa: F401
     from types import NoneType as NoneType
 
 
-NONE_TYPES: tuple[Any, Any, Any] = (None, NoneType, Literal[None])
+LITERAL_TYPES: set[Any] = {Literal}
+if hasattr(typing, 'Literal'):
+    LITERAL_TYPES.add(typing.Literal)  # type: ignore[attr-defined]
 
-
-TypeVarType = Any  # since mypy doesn't allow the use of TypeVar as a type
+NONE_TYPES: tuple[Any, ...] = (None, NoneType, *(tp[None] for tp in LITERAL_TYPES))
 
 
-if sys.version_info < (3, 8):
-    # Even though this implementation is slower, we need it for python 3.7:
-    # In python 3.7 "Literal" is not a builtin type and uses a different
-    # mechanism.
-    # for this reason `Literal[None] is Literal[None]` evaluates to `False`,
-    # breaking the faster implementation used for the other python versions.
-
-    def is_none_type(type_: Any) -> bool:
-        return type_ in NONE_TYPES
-
-elif sys.version_info[:2] == (3, 8):
-
-    def is_none_type(type_: Any) -> bool:
-        for none_type in NONE_TYPES:
-            if type_ is none_type:
-                return True
-        # With python 3.8, specifically 3.8.10, Literal "is" checks are very flakey
-        # can change on very subtle changes like use of types in other modules,
-        # hopefully this check avoids that issue.
-        if is_literal_type(type_):  # pragma: no cover
-            return all_literal_values(type_) == [None]
-        return False
+TypeVarType = Any  # since mypy doesn't allow the use of TypeVar as a type
 
-else:
 
-    def is_none_type(type_: Any) -> bool:
-        for none_type in NONE_TYPES:
-            if type_ is none_type:
-                return True
-        return False
+def is_none_type(type_: Any) -> bool:
+    return type_ in NONE_TYPES
 
 
 def is_callable_type(type_: type[Any]) -> bool:
     return type_ is Callable or get_origin(type_) is Callable
 
 
 def is_literal_type(type_: type[Any]) -> bool:
-    return Literal is not None and get_origin(type_) is Literal
+    return Literal is not None and get_origin(type_) in LITERAL_TYPES
 
 
 def literal_values(type_: type[Any]) -> tuple[Any, ...]:
     return get_args(type_)
 
 
 def all_literal_values(type_: type[Any]) -> list[Any]:
@@ -233,15 +208,14 @@
 
 def get_cls_type_hints_lenient(obj: Any, globalns: dict[str, Any] | None = None) -> dict[str, Any]:
     """
     Collect annotations from a class, including those from parent classes.
 
     Unlike `typing.get_type_hints`, this function will not error if a forward reference is not resolvable.
     """
-    # TODO: Try handling typevars_map here
     hints = {}
     for base in reversed(obj.__mro__):
         ann = base.__dict__.get('__annotations__')
         localns = dict(vars(base))
         if ann is not None and ann is not GetSetDescriptorType:
             for name, value in ann.items():
                 hints[name] = eval_type_lenient(value, globalns, localns)
@@ -260,28 +234,30 @@
     try:
         return typing._eval_type(value, globalns, localns)  # type: ignore
     except NameError:
         # the point of this function is to be tolerant to this case
         return value
 
 
-def get_function_type_hints(function: Callable[..., Any]) -> dict[str, Any]:
+def get_function_type_hints(function: Callable[..., Any], *, include_keys: set[str] | None = None) -> dict[str, Any]:
     """
     Like `typing.get_type_hints`, but doesn't convert `X` to `Optional[X]` if the default value is `None`, also
     copes with `partial`.
     """
 
     if isinstance(function, partial):
         annotations = function.func.__annotations__
     else:
         annotations = function.__annotations__
 
     globalns = add_module_globals(function)
     type_hints = {}
     for name, value in annotations.items():
+        if include_keys is not None and name not in include_keys:
+            continue
         if value is None:
             value = NoneType
         elif isinstance(value, str):
             value = _make_forward_ref(value)
 
         type_hints[name] = typing._eval_type(value, globalns, None)  # type: ignore
 
@@ -465,7 +441,11 @@
         return ref._evaluate(globalns=globalns, localns=localns, recursive_guard=frozenset())
 
 
 def is_dataclass(_cls: type[Any]) -> TypeGuard[type[StandardDataclass]]:
     # The dataclasses.is_dataclass function doesn't seem to provide TypeGuard functionality,
     # so I created this convenience function
     return dataclasses.is_dataclass(_cls)
+
+
+def origin_is_type_alias_type(origin: Any) -> TypeGuard[TypeAliasType]:
+    return isinstance(origin, TypeAliasType)
```

### Comparing `pydantic-2.0a4/pydantic/_internal/_utils.py` & `pydantic-2.0b1/pydantic/_internal/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,22 +60,22 @@
 }
 
 
 def sequence_like(v: Any) -> bool:
     return isinstance(v, (list, tuple, set, frozenset, GeneratorType, deque))
 
 
-def lenient_isinstance(o: Any, class_or_tuple: type[Any] | tuple[type[Any], ...] | None) -> bool:
+def lenient_isinstance(o: Any, class_or_tuple: type[Any] | tuple[type[Any], ...] | None) -> bool:  # pragma: no cover
     try:
         return isinstance(o, class_or_tuple)  # type: ignore[arg-type]
     except TypeError:
         return False
 
 
-def lenient_issubclass(cls: Any, class_or_tuple: Any) -> bool:
+def lenient_issubclass(cls: Any, class_or_tuple: Any) -> bool:  # pragma: no cover
     try:
         return isinstance(cls, type) and issubclass(cls, class_or_tuple)
     except TypeError:
         if isinstance(cls, _typing_extra.WithArgsTypes):
             return False
         raise  # pragma: no cover
 
@@ -113,18 +113,14 @@
             if k in updated_mapping and isinstance(updated_mapping[k], dict) and isinstance(v, dict):
                 updated_mapping[k] = deep_update(updated_mapping[k], v)
             else:
                 updated_mapping[k] = v
     return updated_mapping
 
 
-def dict_not_none(__pos: dict[str, Any] | None = None, **kwargs: Any) -> dict[str, Any]:
-    return {k: v for k, v in (__pos or kwargs).items() if v is not None}
-
-
 def update_not_none(mapping: dict[Any, Any], **update: Any) -> None:
     mapping.update({k: v for k, v in update.items() if v is not None})
 
 
 def almost_equal_floats(value_1: float, value_2: float, *, delta: float = 1e-8) -> bool:
     """
     Return True if two floats are almost equal
```

### Comparing `pydantic-2.0a4/pydantic/_internal/_validate_call.py` & `pydantic-2.0b1/pydantic/_internal/_validate_call.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a4/pydantic/deprecated/config.py` & `pydantic-2.0b1/pydantic/deprecated/config.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a4/pydantic/deprecated/copy_internals.py` & `pydantic-2.0b1/pydantic/deprecated/copy_internals.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import typing_extensions
 
 from .._internal import (
     _model_construction,
     _typing_extra,
     _utils,
 )
-from .._internal._fields import Undefined
 
 if typing.TYPE_CHECKING:
     from .. import BaseModel
     from .._internal._utils import AbstractSetIntStr, MappingIntStrAny
 
     AnyClassMethod = classmethod[Any, Any, Any]
     TupleGenerator = typing.Generator[Tuple[str, Any], None, None]
@@ -97,32 +96,30 @@
 
 
 def _copy_and_set_values(
     self: Model,
     values: dict[str, Any],
     fields_set: set[str],
     extra: dict[str, Any] | None = None,
+    private: dict[str, Any] | None = None,
     *,
     deep: bool,  # UP006
 ) -> Model:
     if deep:
         # chances of having empty dict here are quite low for using smart_deepcopy
         values = deepcopy(values)
+        extra = deepcopy(extra)
+        private = deepcopy(private)
 
     cls = self.__class__
     m = cls.__new__(cls)
     _object_setattr(m, '__dict__', values)
     _object_setattr(m, '__pydantic_extra__', extra)
     _object_setattr(m, '__pydantic_fields_set__', fields_set)
-    for name in self.__private_attributes__:
-        value = getattr(self, name, Undefined)
-        if value is not Undefined:
-            if deep:
-                value = deepcopy(value)
-            _object_setattr(m, name, value)
+    _object_setattr(m, '__pydantic_private__', private)
 
     return m
 
 
 @typing.no_type_check
 def _get_value(
     cls: type[BaseModel],
```

### Comparing `pydantic-2.0a4/pydantic/deprecated/decorator.py` & `pydantic-2.0b1/pydantic/deprecated/decorator.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from functools import wraps
 from typing import TYPE_CHECKING, Any, Callable, Dict, List, Mapping, Optional, Tuple, Type, TypeVar, Union, overload
 
 from typing_extensions import deprecated
 
 from .._internal import _config, _typing_extra
 from ..alias_generators import to_pascal
-from ..decorators import field_validator
 from ..errors import PydanticUserError
+from ..functional_validators import field_validator
 from ..main import BaseModel, create_model
 
 __all__ = ('validate_arguments',)
 
 if TYPE_CHECKING:
     AnyCallable = Callable[..., Any]
```

### Comparing `pydantic-2.0a4/pydantic/deprecated/json.py` & `pydantic-2.0b1/pydantic/deprecated/json.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a4/pydantic/deprecated/parse.py` & `pydantic-2.0b1/pydantic/deprecated/parse.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a4/pydantic/deprecated/tools.py` & `pydantic-2.0b1/pydantic/deprecated/tools.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a4/tests/conftest.py` & `pydantic-2.0b1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a4/tests/test_abc.py` & `pydantic-2.0b1/tests/test_abc.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a4/tests/test_aliases.py` & `pydantic-2.0b1/tests/test_aliases.py`

 * *Files 4% similar despite different names*

```diff
@@ -213,17 +213,14 @@
         z: str
 
     assert [f.alias for f in Parent.model_fields.values()] == ['abc', None]
     assert [f.alias for f in Child.model_fields.values()] == ['abc', 'Y', 'Z']
 
 
 def test_low_priority_alias():
-    # TODO:
-    #  Alternative 1: we could drop alias_priority and tell people to manually override aliases in child classes
-    #  Alternative 2: we could add a new argument `override_with_alias_generator=True` equivalent to `alias_priority=1`
     class Parent(BaseModel):
         w: bool = Field(..., alias='w_', validation_alias='w_val_alias', serialization_alias='w_ser_alias')
         x: bool = Field(
             ..., alias='abc', alias_priority=1, validation_alias='x_val_alias', serialization_alias='x_ser_alias'
         )
         y: str
 
@@ -401,56 +398,79 @@
     assert m.x == 'bar'
     assert m.model_dump() == {'x': 'bar'}
     assert m.model_dump(by_alias=True) == {'foo': 'bar'}
     sig = signature(Model)
     assert 'foo' in sig.parameters
 
 
-def test_aliases_json_schema():
+@pytest.mark.parametrize(
+    'field,expected',
+    [
+        pytest.param(
+            Field(alias='x_alias', validation_alias='x_val_alias', serialization_alias='x_ser_alias'),
+            {
+                'properties': {'x_val_alias': {'title': 'X Val Alias', 'type': 'string'}},
+                'required': ['x_val_alias'],
+            },
+            id='single_alias',
+        ),
+        pytest.param(
+            Field(validation_alias=AliasChoices('y_alias', 'another_alias')),
+            {
+                'properties': {'y_alias': {'title': 'Y Alias', 'type': 'string'}},
+                'required': ['y_alias'],
+            },
+            id='multiple_aliases',
+        ),
+        pytest.param(
+            Field(validation_alias=AliasChoices(AliasPath('z_alias', 'even_another_alias'), 'and_another')),
+            {
+                'properties': {'and_another': {'title': 'And Another', 'type': 'string'}},
+                'required': ['and_another'],
+            },
+            id='multiple_aliases_with_path',
+        ),
+    ],
+)
+def test_aliases_json_schema(field, expected):
     class Model(BaseModel):
-        x: str = Field(alias='x_alias', validation_alias='x_val_alias', serialization_alias='x_ser_alias')
+        x: str = field
 
-    assert Model.model_json_schema() == {
-        'properties': {'x_val_alias': {'title': 'X Val Alias', 'type': 'string'}},
-        'required': ['x_val_alias'],
-        'title': 'Model',
-        'type': 'object',
-    }
+    assert Model.model_json_schema() == {'title': 'Model', 'type': 'object', **expected}
 
 
 @pytest.mark.parametrize(
-    'input,expected',
+    'value',
     [
-        ('a', 'a'),
-        (AliasPath('a', 'b', 1), ['a', 'b', 1]),
-        (AliasChoices('a', 'b'), [['a'], ['b']]),
-        (AliasChoices('a', AliasPath('b', 1)), [['a'], ['b', 1]]),
-        (AliasChoices(), None),
+        'a',
+        AliasPath('a', 'b', 1),
+        AliasChoices('a', 'b'),
+        AliasChoices('a', AliasPath('b', 1)),
     ],
 )
-def test_validation_alias_path(input, expected):
+def test_validation_alias_path(value):
     class Model(BaseModel):
-        x: str = Field(validation_alias=input)
+        x: str = Field(validation_alias=value)
 
-    assert Model.model_fields['x'].validation_alias == expected
+    assert Model.model_fields['x'].validation_alias == value
 
 
 def test_validation_alias_invalid_value_type():
     m = 'Invalid `validation_alias` type. it should be `str`, `AliasChoices`, or `AliasPath`'
     with pytest.raises(TypeError, match=m):
 
         class Model(BaseModel):
             x: str = Field(validation_alias=123)
 
 
 def test_validation_alias_parse_data():
     class Model(BaseModel):
         x: str = Field(validation_alias=AliasChoices('a', AliasPath('b', 1), 'c'))
 
-    assert Model.model_fields['x'].validation_alias == [['a'], ['b', 1], ['c']]
+    assert Model.model_fields['x'].validation_alias == AliasChoices('a', AliasPath('b', 1), 'c')
     assert Model.model_validate({'a': 'hello'}).x == 'hello'
     assert Model.model_validate({'b': ['hello', 'world']}).x == 'world'
     assert Model.model_validate({'c': 'test'}).x == 'test'
     with pytest.raises(ValidationError) as exc_info:
         Model.model_validate({'b': ['hello']})
     assert exc_info.value.errors(include_url=False) == [
         {
```

### Comparing `pydantic-2.0a4/tests/test_annotated.py` & `pydantic-2.0b1/tests/test_annotated.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 from typing import Any, Generic, Iterator, List, Set, TypeVar
 
 import pytest
 from annotated_types import BaseMetadata, GroupedMetadata, Gt, Lt
 from pydantic_core import core_schema
 from typing_extensions import Annotated
 
-from pydantic import BaseModel, Field
-from pydantic.annotated import GetCoreSchemaHandler
+from pydantic import BaseModel, Field, GetCoreSchemaHandler
+from pydantic._internal._fields import Undefined
 from pydantic.errors import PydanticSchemaGenerationError
-from pydantic.fields import Undefined
 
 NO_VALUE = object()
 
 
 @pytest.mark.parametrize(
     'hint_fn,value,expected_repr',
     [
@@ -228,33 +227,35 @@
             # so just register when our iter is called
             calls.append('GroupedMetadataMarker:iter')
             yield from []
 
     class _(BaseModel):
         x: Annotated[CustomType, GroupedMetadataMarker(), PydanticMetadata()]
 
+    # insert_assert(calls)
     assert calls == [
+        'GroupedMetadataMarker:iter',
         'PydanticMetadata:before',
         'CustomType:before',
         'CustomType:after',
-        'GroupedMetadataMarker:iter',
         'PydanticMetadata:after',
     ]
 
     calls.clear()
 
     class _(BaseModel):
         x: Annotated[CustomType, PydanticMetadata(), GroupedMetadataMarker()]
 
+    # insert_assert(calls)
     assert calls == [
+        'GroupedMetadataMarker:iter',
         'PydanticMetadata:before',
         'CustomType:before',
         'CustomType:after',
         'PydanticMetadata:after',
-        'GroupedMetadataMarker:iter',
     ]
 
     calls.clear()
 
 
 def test_get_pydantic_core_schema_source_type() -> None:
     types: Set[Any] = set()
```

### Comparing `pydantic-2.0a4/tests/test_assert_in_validators.py` & `pydantic-2.0b1/tests/test_assert_in_validators.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 PYTEST_DONT_REWRITE
 """
 import pytest
 
-from pydantic import BaseModel, ValidationError
-from pydantic.decorators import field_validator
+from pydantic import BaseModel, ValidationError, field_validator
 
 
 def test_assert_raises_validation_error():
     class Model(BaseModel):
         a: str
 
         @field_validator('a')
```

### Comparing `pydantic-2.0a4/tests/test_callable.py` & `pydantic-2.0b1/tests/test_callable.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a4/tests/test_color.py` & `pydantic-2.0b1/tests/test_color.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a4/tests/test_computed_fields.py` & `pydantic-2.0b1/tests/test_computed_fields.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,27 @@
-from __future__ import annotations as _annotations
-
 import random
 import sys
 from abc import ABC, abstractmethod
-from typing import Any, ClassVar
+from typing import Any, ClassVar, List, Tuple
 
 import pytest
-from pydantic_core import PydanticSerializationError, ValidationError
+from pydantic_core import ValidationError, core_schema
 
-from pydantic import BaseModel, Field, PrivateAttr, TypeAdapter, computed_field, dataclasses, field_validator
+from pydantic import (
+    BaseModel,
+    Field,
+    GetCoreSchemaHandler,
+    PrivateAttr,
+    TypeAdapter,
+    computed_field,
+    dataclasses,
+    field_validator,
+)
+from pydantic.alias_generators import to_camel
+from pydantic.errors import PydanticUserError
 
 try:
     from functools import cached_property, lru_cache, singledispatchmethod
 except ImportError:
     cached_property = None
     lru_cache = None
     singledispatchmethod = None
@@ -252,62 +261,62 @@
 
 def test_include_exclude():
     class Model(BaseModel):
         x: int
         y: int
 
         @computed_field
-        def x_list(self) -> list[int]:
+        def x_list(self) -> List[int]:
             return [self.x, self.x + 1]
 
         @computed_field
-        def y_list(self) -> list[int]:
+        def y_list(self) -> List[int]:
             return [self.y, self.y + 1, self.y + 2]
 
     m = Model(x=1, y=2)
     assert m.model_dump() == {'x': 1, 'y': 2, 'x_list': [1, 2], 'y_list': [2, 3, 4]}
     assert m.model_dump(include={'x'}) == {'x': 1}
     assert m.model_dump(include={'x': None, 'x_list': {0}}) == {'x': 1, 'x_list': [1]}
     assert m.model_dump(exclude={'x': ..., 'y_list': {2}}) == {'y': 2, 'x_list': [1, 2], 'y_list': [2, 3]}
 
 
 def test_expected_type():
     class Model(BaseModel):
         x: int
         y: int
 
-        @computed_field(json_return_type='list')
-        def x_list(self) -> list[int]:
+        @computed_field
+        def x_list(self) -> List[int]:
             return [self.x, self.x + 1]
 
-        @computed_field(json_return_type='bytes')
+        @computed_field
         def y_str(self) -> bytes:
             s = f'y={self.y}'
             return s.encode()
 
     m = Model(x=1, y=2)
     assert m.model_dump() == {'x': 1, 'y': 2, 'x_list': [1, 2], 'y_str': b'y=2'}
     assert m.model_dump(mode='json') == {'x': 1, 'y': 2, 'x_list': [1, 2], 'y_str': 'y=2'}
     assert m.model_dump_json() == '{"x":1,"y":2,"x_list":[1,2],"y_str":"y=2"}'
 
 
 def test_expected_type_wrong():
     class Model(BaseModel):
         x: int
 
-        @computed_field(json_return_type='list')
-        def x_list(self) -> list[int]:
+        @computed_field
+        def x_list(self) -> List[int]:
             return 'not a list'
 
     m = Model(x=1)
-    with pytest.raises(TypeError, match="^'str' object cannot be converted to 'PyList'$"):
+    with pytest.warns(UserWarning, match=r'Expected `list\[int\]` but got `str`'):
         m.model_dump()
-    with pytest.raises(TypeError, match="^'str' object cannot be converted to 'PyList'$"):
+    with pytest.warns(UserWarning, match=r'Expected `list\[int\]` but got `str`'):
         m.model_dump(mode='json')
-    with pytest.raises(PydanticSerializationError, match="Error serializing to JSON: 'str' object cannot be converted"):
+    with pytest.warns(UserWarning, match=r'Expected `list\[int\]` but got `str`'):
         m.model_dump_json()
 
 
 def test_inheritance():
     class Base(BaseModel):
         x: int
 
@@ -404,16 +413,19 @@
         def area(self, new_area: int):
             self.side = new_area**0.5
 
     m = Square(side=4)
     assert m.area == 16.0
     assert m.model_dump() == {'side': 4.0, 'area': 16.0}
 
-    with pytest.raises(TypeError, match='"Square" is frozen and does not support item assignment'):
+    with pytest.raises(ValidationError) as exc_info:
         m.area = 4
+    assert exc_info.value.errors(include_url=False) == [
+        {'type': 'frozen_instance', 'loc': ('area',), 'msg': 'Instance is frozen', 'input': 4}
+    ]
 
 
 def test_validate_assignment():
     class Square(BaseModel, validate_assignment=True):
         side: float
 
         @field_validator('side')
@@ -468,22 +480,117 @@
     'bases',
     [
         (BaseModel, ABC),
         (ABC, BaseModel),
         (BaseModel,),
     ],
 )
-def test_abstractmethod_missing(bases: tuple[Any, ...]):
+def test_abstractmethod_missing(bases: Tuple[Any, ...]):
     class AbstractSquare(*bases):
         side: float
 
         @computed_field
         @property
         @abstractmethod
         def area(self) -> float:
             raise NotImplementedError()
 
     class Square(AbstractSquare):
         pass
 
     with pytest.raises(TypeError, match="Can't instantiate abstract class Square with abstract methods? area"):
         Square(side=4.0)
+
+
+class CustomType(str):
+    @classmethod
+    def __get_pydantic_core_schema__(cls, source: Any, handler: GetCoreSchemaHandler) -> core_schema.CoreSchema:
+        schema = handler(str)
+        schema['serialization'] = core_schema.plain_serializer_function_ser_schema(lambda x: '123')
+        return schema
+
+
+def test_computed_fields_infer_return_type():
+    class Model(BaseModel):
+        @computed_field
+        def cfield(self) -> CustomType:
+            return CustomType('abc')
+
+    assert Model().model_dump() == {'cfield': '123'}
+    assert Model().model_dump_json() == '{"cfield":"123"}'
+
+
+def test_computed_fields_missing_return_type():
+    with pytest.raises(PydanticUserError, match='Computed field is missing return type annotation'):
+
+        class _Model(BaseModel):
+            @computed_field
+            def cfield(self):
+                raise NotImplementedError
+
+    class Model(BaseModel):
+        @computed_field(return_type=CustomType)
+        def cfield(self):
+            return CustomType('abc')
+
+    assert Model().model_dump() == {'cfield': '123'}
+    assert Model().model_dump_json() == '{"cfield":"123"}'
+
+
+def test_alias_generator():
+    class MyModel(BaseModel):
+        my_standard_field: int
+
+        @computed_field  # *will* be overridden by alias generator
+        @property
+        def my_computed_field(self) -> int:
+            return self.my_standard_field + 1
+
+        @computed_field(alias='my_alias_none')  # will *not* be overridden by alias generator
+        @property
+        def my_aliased_computed_field_none(self) -> int:
+            return self.my_standard_field + 2
+
+        @computed_field(alias='my_alias_1', alias_priority=1)  # *will* be overridden by alias generator
+        @property
+        def my_aliased_computed_field_1(self) -> int:
+            return self.my_standard_field + 3
+
+        @computed_field(alias='my_alias_2', alias_priority=2)  # will *not* be overridden by alias generator
+        @property
+        def my_aliased_computed_field_2(self) -> int:
+            return self.my_standard_field + 4
+
+    class MySubModel(MyModel):
+        model_config = dict(alias_generator=to_camel, populate_by_name=True)
+
+    model = MyModel(my_standard_field=1)
+    assert model.model_dump() == {
+        'my_standard_field': 1,
+        'my_computed_field': 2,
+        'my_aliased_computed_field_none': 3,
+        'my_aliased_computed_field_1': 4,
+        'my_aliased_computed_field_2': 5,
+    }
+    assert model.model_dump(by_alias=True) == {
+        'my_standard_field': 1,
+        'my_computed_field': 2,
+        'my_alias_none': 3,
+        'my_alias_1': 4,
+        'my_alias_2': 5,
+    }
+
+    submodel = MySubModel(my_standard_field=1)
+    assert submodel.model_dump() == {
+        'my_standard_field': 1,
+        'my_computed_field': 2,
+        'my_aliased_computed_field_none': 3,
+        'my_aliased_computed_field_1': 4,
+        'my_aliased_computed_field_2': 5,
+    }
+    assert submodel.model_dump(by_alias=True) == {
+        'myStandardField': 1,
+        'myComputedField': 2,
+        'my_alias_none': 3,
+        'myAliasedComputedField1': 4,
+        'my_alias_2': 5,
+    }
```

### Comparing `pydantic-2.0a4/tests/test_config.py` & `pydantic-2.0b1/tests/test_config.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import re
 import sys
 from contextlib import nullcontext as does_not_raise
+from decimal import Decimal
 from inspect import signature
 from typing import Any, ContextManager, Iterable, NamedTuple, Type, Union, get_type_hints
 
-from dirty_equals import HasRepr
+from dirty_equals import HasRepr, IsPartialDict
 from pydantic_core import SchemaError
 
 from pydantic import (
     BaseConfig,
     BaseModel,
     Field,
     PrivateAttr,
@@ -37,16 +38,15 @@
         # strict=False overrides the Config
         b: Annotated[int, Field(strict=False)]
         # strict=None or not including it is equivalent
         # lets this field be overridden by the Config
         c: Annotated[int, Field(strict=None)]
         d: Annotated[int, Field()]
 
-        class Config:
-            strict = True
+        model_config = ConfigDict(strict=True)
 
     return ModelWithStrictConfig
 
 
 def _equals(a: Union[str, Iterable[str]], b: Union[str, Iterable[str]]) -> bool:
     """
     Compare strings with spaces removed
@@ -62,29 +62,30 @@
 def test_config_dict_missing_keys():
     assert ConfigDict().get('missing_property') is None
 
     with pytest.raises(KeyError, match="'missing_property'"):
         ConfigDict()['missing_property']
 
 
-@pytest.mark.filterwarnings('ignore:.* is deprecated.*:DeprecationWarning')
 class TestsBaseConfig:
+    @pytest.mark.filterwarnings('ignore:.* is deprecated.*:DeprecationWarning')
     def test_base_config_equality_defaults_of_config_dict_class(self):
         for key, value in config_defaults.items():
             assert getattr(BaseConfig, key) == value
 
     def test_config_and_module_config_cannot_be_used_together(self):
         with pytest.raises(PydanticUserError):
 
             class MyModel(BaseModel):
                 model_config = ConfigDict(title='MyTitle')
 
                 class Config:
                     title = 'MyTitleConfig'
 
+    @pytest.mark.filterwarnings('ignore:.* is deprecated.*:DeprecationWarning')
     def test_base_config_properly_converted_to_dict(self):
         class MyConfig(BaseConfig):
             title = 'MyTitle'
             frozen = True
 
         class MyBaseModel(BaseModel):
             class Config(MyConfig):
@@ -99,16 +100,15 @@
 
     def test_base_config_custom_init_signature(self):
         class MyModel(BaseModel):
             id: int
             name: str = 'John Doe'
             f__: str = Field(..., alias='foo')
 
-            class Config:
-                extra = 'allow'
+            model_config = ConfigDict(extra='allow')
 
             def __init__(self, id: int = 1, bar=2, *, baz: Any, **data):
                 super().__init__(id=id, **data)
                 self.bar = bar
                 self.baz = baz
 
         sig = signature(MyModel)
@@ -123,76 +123,69 @@
             a: float
             b: int = 2
             c: int
 
             def __init__(self, a: float, b: int):
                 super().__init__(a=a, b=b, c=1)
 
-            class Config:
-                extra = 'allow'
+            model_config = ConfigDict(extra='allow')
 
         assert _equals(str(signature(Model)), '(a: float, b: int) -> None')
 
     def test_base_config_use_field_name(self):
         class Foo(BaseModel):
             foo: str = Field(..., alias='this is invalid')
 
-            class Config:
-                populate_by_name = True
+            model_config = ConfigDict(populate_by_name=True)
 
         assert _equals(str(signature(Foo)), '(*, foo: str) -> None')
 
     def test_base_config_does_not_use_reserved_word(self):
         class Foo(BaseModel):
             from_: str = Field(..., alias='from')
 
-            class Config:
-                populate_by_name = True
+            model_config = ConfigDict(populate_by_name=True)
 
         assert _equals(str(signature(Foo)), '(*, from_: str) -> None')
 
     def test_base_config_extra_allow_no_conflict(self):
         class Model(BaseModel):
             spam: str
 
-            class Config:
-                extra = 'allow'
+            model_config = ConfigDict(extra='allow')
 
         assert _equals(str(signature(Model)), '(*, spam: str, **extra_data: Any) -> None')
 
     def test_base_config_extra_allow_conflict_twice(self):
         class Model(BaseModel):
             extra_data: str
             extra_data_: str
 
-            class Config:
-                extra = 'allow'
+            model_config = ConfigDict(extra='allow')
 
         assert _equals(str(signature(Model)), '(*, extra_data: str, extra_data_: str, **extra_data__: Any) -> None')
 
     def test_base_config_extra_allow_conflict_custom_signature(self):
         class Model(BaseModel):
             extra_data: int
 
             def __init__(self, extra_data: int = 1, **foobar: Any):
                 super().__init__(extra_data=extra_data, **foobar)
 
-            class Config:
-                extra = 'allow'
+            model_config = ConfigDict(extra='allow')
 
         assert _equals(str(signature(Model)), '(extra_data: int = 1, **foobar: Any) -> None')
 
     def test_base_config_private_attribute_intersection_with_extra_field(self):
         class Model(BaseModel):
             _foo = PrivateAttr('private_attribute')
 
-            class Config:
-                extra = 'allow'
+            model_config = ConfigDict(extra='allow')
 
-        assert Model.__slots__ == {'_foo'}
+        assert set(Model.__private_attributes__) == {'_foo'}
         m = Model(_foo='field')
         assert m._foo == 'private_attribute'
         assert m.__dict__ == {}
         assert m.__pydantic_extra__ == {'_foo': 'field'}
         assert m.model_dump() == {'_foo': 'field'}
         m._foo = 'still_private'
         assert m._foo == 'still_private'
@@ -200,32 +193,30 @@
         assert m.__pydantic_extra__ == {'_foo': 'field'}
         assert m.model_dump() == {'_foo': 'field'}
 
     def test_base_config_parse_model_with_strict_config_disabled(
         self, BaseConfigModelWithStrictConfig: Type[BaseModel]
     ) -> None:
         class Model(BaseConfigModelWithStrictConfig):
-            class Config:
-                strict = False
+            model_config = ConfigDict(strict=False)
 
         values = [
             Model(a='1', b=2, c=3, d=4),
             Model(a=1, b=2, c='3', d=4),
             Model(a=1, b=2, c=3, d='4'),
             Model(a=1, b='2', c=3, d=4),
             Model(a=1, b=2, c=3, d=4),
         ]
         assert all(v.model_dump() == {'a': 1, 'b': 2, 'c': 3, 'd': 4} for v in values)
 
     def test_finite_float_config(self):
         class Model(BaseModel):
             a: float
 
-            class Config:
-                allow_inf_nan = False
+            model_config = ConfigDict(allow_inf_nan=False)
 
         assert Model(a=42).a == 42
         with pytest.raises(ValidationError) as exc_info:
             Model(a=float('nan'))
         # insert_assert(exc_info.value.errors(include_url=False))
         assert exc_info.value.errors(include_url=False) == [
             {
@@ -244,45 +235,42 @@
             (False, '  123  ', '  123  '),
         ],
     )
     def test_str_strip_whitespace(self, enabled, str_check, result_str_check):
         class Model(BaseModel):
             str_check: str
 
-            class Config:
-                str_strip_whitespace = enabled
+            model_config = ConfigDict(str_strip_whitespace=enabled)
 
         m = Model(str_check=str_check)
         assert m.str_check == result_str_check
 
     @pytest.mark.parametrize(
         'enabled,str_check,result_str_check',
         [(True, 'ABCDefG', 'ABCDEFG'), (False, 'ABCDefG', 'ABCDefG')],
     )
     def test_str_to_upper(self, enabled, str_check, result_str_check):
         class Model(BaseModel):
             str_check: str
 
-            class Config:
-                str_to_upper = enabled
+            model_config = ConfigDict(str_to_upper=enabled)
 
         m = Model(str_check=str_check)
 
         assert m.str_check == result_str_check
 
     @pytest.mark.parametrize(
         'enabled,str_check,result_str_check',
         [(True, 'ABCDefG', 'abcdefg'), (False, 'ABCDefG', 'ABCDefG')],
     )
     def test_str_to_lower(self, enabled, str_check, result_str_check):
         class Model(BaseModel):
             str_check: str
 
-            class Config:
-                str_to_lower = enabled
+            model_config = ConfigDict(str_to_lower=enabled)
 
         m = Model(str_check=str_check)
 
         assert m.str_check == result_str_check
 
     def test_namedtuple_arbitrary_type(self):
         class CustomClass:
@@ -290,16 +278,15 @@
 
         class Tup(NamedTuple):
             c: CustomClass
 
         class Model(BaseModel):
             x: Tup
 
-            class Config:
-                arbitrary_types_allowed = True
+            model_config = ConfigDict(arbitrary_types_allowed=True)
 
         data = {'x': Tup(c=CustomClass())}
         model = Model.model_validate(data)
         assert isinstance(model.x.c, CustomClass)
         with pytest.raises(PydanticSchemaGenerationError):
 
             class ModelNoArbitraryTypes(BaseModel):
@@ -326,31 +313,29 @@
         expectation: ContextManager,
     ):
         expected_value: int = 7
 
         class Foo(BaseModel):
             bar_: int = Field(..., alias='bar')
 
-            class Config(BaseConfig):
-                populate_by_name = populate_by_name_config
+            model_config = dict(populate_by_name=populate_by_name_config)
 
         with expectation:
             if use_construct:
                 f = Foo.model_construct(**{arg_name: expected_value})
             else:
                 f = Foo(**{arg_name: expected_value})
             assert f.bar_ == expected_value
 
     def test_immutable_copy_with_frozen(self):
         class Model(BaseModel):
             a: int
             b: int
 
-            class Config:
-                frozen = True
+            model_config = ConfigDict(frozen=True)
 
         m = Model(a=40, b=10)
         assert m == m.model_copy()
 
     def test_config_class_is_deprecated(self):
         with pytest.warns(
             DeprecationWarning, match='Support for class-based `config` is deprecated, use ConfigDict instead.'
@@ -368,29 +353,35 @@
 
         with pytest.warns(
             DeprecationWarning,
             match='Support for class-based `config` is deprecated, use ConfigDict instead.',
         ):
             assert BaseConfig().validate_assignment is False
 
-        class Config(BaseConfig):
-            pass
+        with pytest.warns(
+            DeprecationWarning,
+            match='Support for class-based `config` is deprecated, use ConfigDict instead.',
+        ):
+
+            class Config(BaseConfig):
+                pass
 
         with pytest.warns(
             DeprecationWarning,
             match='Support for class-based `config` is deprecated, use ConfigDict instead.',
         ):
             assert Config.validate_assignment is False
 
         with pytest.warns(
             DeprecationWarning,
             match='Support for class-based `config` is deprecated, use ConfigDict instead.',
         ):
             assert Config().validate_assignment is False
 
+    @pytest.mark.filterwarnings('ignore:.* is deprecated.*:DeprecationWarning')
     def test_config_class_missing_attributes(self):
         with pytest.raises(AttributeError, match="type object 'BaseConfig' has no attribute 'missing_attribute'"):
             BaseConfig.missing_attribute
 
         with pytest.raises(AttributeError, match="'BaseConfig' object has no attribute 'missing_attribute'"):
             BaseConfig().missing_attribute
 
@@ -476,15 +467,15 @@
 
         class MyModel(BaseModel):
             model_config = config_dict
 
     with pytest.raises(SchemaError, match=extra_error):
         create_model('MyCreatedModel', __config__=config_dict)
 
-    with pytest.raises(SchemaError, match='Invalid extra_behavior: `invalid-value`'):
+    with pytest.raises(SchemaError, match=extra_error):
 
         @pydantic_dataclass(config=config_dict)
         class MyDataclass:
             pass
 
 
 def test_invalid_config_keys():
@@ -537,7 +528,97 @@
 
 @pytest.mark.skipif(sys.version_info < (3, 10), reason='different on older versions')
 def test_config_defaults_match():
     config_dict_keys = list(get_type_hints(ConfigDict).keys())
     config_defaults_keys = list(config_defaults.keys())
 
     assert config_dict_keys == config_defaults_keys, 'ConfigDict and config_defaults must have the same keys'
+
+
+def test_config_is_not_inherited_in_model_fields():
+    from typing import List
+
+    from pydantic import BaseModel, ConfigDict
+
+    class Inner(BaseModel):
+        a: str
+
+    class Outer(BaseModel):
+        # this cause the inner model incorrectly dumpped:
+        model_config = ConfigDict(str_to_lower=True)
+
+        x: List[str]  # should be converted to lower
+        inner: Inner  # should not have fields converted to lower
+
+    m = Outer.model_validate(dict(x=['Abc'], inner=dict(a='Def')))
+
+    assert m.model_dump() == {'x': ['abc'], 'inner': {'a': 'Def'}}
+
+
+@pytest.mark.parametrize(
+    'config,input_str',
+    (
+        ({}, 'type=string_type, input_value=123, input_type=int'),
+        ({'hide_input_in_errors': False}, 'type=string_type, input_value=123, input_type=int'),
+        ({'hide_input_in_errors': True}, 'type=string_type'),
+    ),
+)
+def test_hide_input_in_errors(config, input_str):
+    class Model(BaseModel):
+        x: str
+
+        model_config = ConfigDict(**config)
+
+    with pytest.raises(ValidationError, match=re.escape(f'Input should be a valid string [{input_str}]')):
+        Model(x=123)
+
+
+parametrize_inf_nan_capable_type = pytest.mark.parametrize('inf_nan_capable_type', [float, Decimal])
+parametrize_inf_nan_capable_value = pytest.mark.parametrize('inf_nan_value', ['Inf', 'NaN'])
+
+
+@parametrize_inf_nan_capable_value
+@parametrize_inf_nan_capable_type
+def test_config_inf_nan_enabled(inf_nan_capable_type, inf_nan_value):
+    class Model(BaseModel):
+        model_config = ConfigDict(allow_inf_nan=True)
+        value: inf_nan_capable_type
+
+    assert Model(value=inf_nan_capable_type(inf_nan_value))
+
+
+@parametrize_inf_nan_capable_value
+@parametrize_inf_nan_capable_type
+def test_config_inf_nan_disabled(inf_nan_capable_type, inf_nan_value):
+    class Model(BaseModel):
+        model_config = ConfigDict(allow_inf_nan=False)
+        value: inf_nan_capable_type
+
+    with pytest.raises(ValidationError) as e:
+        Model(value=inf_nan_capable_type(inf_nan_value))
+
+    assert e.value.errors(include_url=False)[0] == IsPartialDict(
+        {
+            'loc': ('value',),
+            'msg': 'Input should be a finite number',
+            'type': 'finite_number',
+        }
+    )
+
+
+@pytest.mark.parametrize(
+    'config,expected',
+    (
+        (ConfigDict(), 'ConfigWrapper()'),
+        (ConfigDict(title='test'), "ConfigWrapper(title='test')"),
+    ),
+)
+def test_config_wrapper_repr(config, expected):
+    assert repr(ConfigWrapper(config=config)) == expected
+
+
+def test_config_wrapper_get_item():
+    config_wrapper = ConfigWrapper(config=ConfigDict(title='test'))
+
+    assert config_wrapper.title == 'test'
+    with pytest.raises(AttributeError, match="Config has no attribute 'test'"):
+        config_wrapper.test
```

### Comparing `pydantic-2.0a4/tests/test_construction.py` & `pydantic-2.0b1/tests/test_construction.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import pickle
 from typing import Any, List, Optional
 
 import pytest
+from pydantic_core import ValidationError
 
 from pydantic import BaseModel, ConfigDict, Field, PrivateAttr
-from pydantic.fields import Undefined
+from pydantic._internal._fields import Undefined
 
 
 class Model(BaseModel):
     a: float
     b: int = 10
 
 
@@ -261,14 +262,28 @@
 
     assert (
         copy_method(Foo(foo='hello'), update={'bar': 'world'}).model_dump_json(exclude_unset=True)
         == '{"foo":"hello","bar":"world"}'
     )
 
 
+class ExtraModel(BaseModel, extra='allow'):
+    pass
+
+
+def test_copy_deep_extra(copy_method):
+    class Foo(BaseModel, extra='allow'):
+        pass
+
+    m = Foo(extra=[])
+    assert copy_method(m).extra is m.extra
+    assert copy_method(m, deep=True).extra == m.extra
+    assert copy_method(m, deep=True).extra is not m.extra
+
+
 def test_copy_set_fields(ModelTwo, copy_method):
     m = ModelTwo(a=24, d=Model(a='12'))
     m2 = copy_method(m)
 
     assert m.model_dump(exclude_unset=True) == {'a': 24.0, 'd': {'a': 12}}
     assert m.model_dump(exclude_unset=True) == m2.model_dump(exclude_unset=True)
 
@@ -357,25 +372,32 @@
 
     m = Model(a=40, b=10)
     assert m == copy_method(m)
     assert repr(m) == 'Model(a=40, b=10)'
 
     m2 = copy_method(m, update={'b': 12})
     assert repr(m2) == 'Model(a=40, b=12)'
-    with pytest.raises(TypeError):
+    with pytest.raises(ValidationError):
         m2.b = 13
 
 
 def test_pickle_fields_set():
     m = Model(a=24)
     assert m.model_dump(exclude_unset=True) == {'a': 24}
     m2 = pickle.loads(pickle.dumps(m))
     assert m2.model_dump(exclude_unset=True) == {'a': 24}
 
 
+def test_pickle_preserves_extra():
+    m = ExtraModel(a=24)
+    assert m.model_extra == {'a': 24}
+    m2 = pickle.loads(pickle.dumps(m))
+    assert m2.model_extra == {'a': 24}
+
+
 def test_copy_update_exclude():
     class SubModel(BaseModel):
         a: str
         b: str
 
     class Model(BaseModel):
         c: str
```

### Comparing `pydantic-2.0a4/tests/test_create_model.py` & `pydantic-2.0b1/tests/test_create_model.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,38 @@
+import platform
 from typing import Optional, Tuple
 
 import pytest
 
-from pydantic import BaseModel, ConfigDict, Field, PydanticUserError, ValidationError, create_model, errors
-from pydantic.decorators import field_validator, validator
+from pydantic import (
+    BaseModel,
+    ConfigDict,
+    Field,
+    PrivateAttr,
+    PydanticUserError,
+    ValidationError,
+    create_model,
+    errors,
+    field_validator,
+    validator,
+)
 from pydantic.fields import ModelPrivateAttr
 
 
 def test_create_model():
     model = create_model('FooModel', foo=(str, ...), bar=(int, 123))
     assert issubclass(model, BaseModel)
     assert model.model_config == BaseModel.model_config
     assert model.__name__ == 'FooModel'
     assert model.model_fields.keys() == {'foo', 'bar'}
 
-    assert not model.__pydantic_decorators__.validator
-    assert not model.__pydantic_decorators__.root_validator
-    assert not model.__pydantic_decorators__.field_validator
-    assert not model.__pydantic_decorators__.field_serializer
+    assert not model.__pydantic_decorators__.validators
+    assert not model.__pydantic_decorators__.root_validators
+    assert not model.__pydantic_decorators__.field_validators
+    assert not model.__pydantic_decorators__.field_serializers
 
     assert model.__module__ == 'pydantic.main'
 
 
 def test_create_model_usage():
     model = create_model('FooModel', foo=(str, ...), bar=(int, 123))
     m = model(foo='hello')
@@ -78,25 +89,31 @@
         y: int = 2
 
     model = create_model('FooModel', foo=(str, ...), bar=(int, 123), __base__=BarModel)
     assert model.model_fields.keys() == {'foo', 'bar', 'x', 'y'}
     m = model(foo='a', x=4)
     assert m.model_dump() == {'bar': 123, 'foo': 'a', 'x': 4, 'y': 2}
 
+    # bases as a tuple
+    model = create_model('FooModel', foo=(str, ...), bar=(int, 123), __base__=(BarModel,))
+    assert model.model_fields.keys() == {'foo', 'bar', 'x', 'y'}
+    m = model(foo='a', x=4)
+    assert m.model_dump() == {'bar': 123, 'foo': 'a', 'x': 4, 'y': 2}
+
 
 def test_custom_config():
     config = ConfigDict(frozen=True)
     expected_config = BaseModel.model_config.copy()
     expected_config['frozen'] = True
 
     model = create_model('FooModel', foo=(int, ...), __config__=config)
     m = model(**{'foo': '987'})
     assert m.foo == 987
     assert model.model_config == expected_config
-    with pytest.raises(TypeError):
+    with pytest.raises(ValidationError):
         m.foo = 654
 
 
 def test_custom_config_inherits():
     class Config(ConfigDict):
         custom_config: bool
 
@@ -211,68 +228,229 @@
 
     DynamicA = create_model('A', x=(int, ...), y=(float, ...), z=(str, ...))
 
     for field_name in ('x', 'y', 'z'):
         assert A.model_fields[field_name].default == DynamicA.model_fields[field_name].default
 
 
-def test_config_field_info_create_model():
-    # TODO fields doesn't exist anymore, remove test?
-    # class Config:
-    #     fields = {'a': {'description': 'descr'}}
-    ConfigDict()
-
-    m1 = create_model('M1', __config__={'title': 'abc'}, a=(str, ...))
-    assert m1.model_json_schema() == {
-        'properties': {'a': {'title': 'A', 'type': 'string'}},
+def test_create_model_field_and_model_title():
+    m = create_model('M', __config__=ConfigDict(title='abc'), a=(str, Field(title='field-title')))
+    assert m.model_json_schema() == {
+        'properties': {'a': {'title': 'field-title', 'type': 'string'}},
         'required': ['a'],
         'title': 'abc',
         'type': 'object',
     }
 
-    m2 = create_model('M2', __config__={}, a=(str, Field(description='descr')))
-    assert m2.model_json_schema() == {
+
+def test_create_model_field_description():
+    m = create_model('M', a=(str, Field(description='descr')))
+    assert m.model_json_schema() == {
         'properties': {'a': {'description': 'descr', 'title': 'A', 'type': 'string'}},
         'required': ['a'],
-        'title': 'M2',
+        'title': 'M',
         'type': 'object',
     }
 
 
 @pytest.mark.parametrize('base', [ModelPrivateAttr, object])
-def test_set_name(base):
-    calls = []
+@pytest.mark.parametrize('use_annotation', [True, False])
+def test_private_descriptors(base, use_annotation):
+    set_name_calls = []
+    get_calls = []
+    set_calls = []
+    delete_calls = []
 
-    class class_deco(base):
+    class MyDescriptor(base):
         def __init__(self, fn):
             super().__init__()
             self.fn = fn
+            self.name = ''
 
         def __set_name__(self, owner, name):
-            calls.append((owner, name))
+            set_name_calls.append((owner, name))
+            self.name = name
 
         def __get__(self, obj, type=None):
+            get_calls.append((obj, type))
             return self.fn(obj) if obj else self
 
+        def __set__(self, obj, value):
+            set_calls.append((obj, value))
+            self.fn = lambda obj: value
+
+        def __delete__(self, obj):
+            delete_calls.append(obj)
+
+            def fail(obj):
+                # I have purposely not used the exact formatting you'd get if the attribute wasn't defined,
+                # to make it clear this function is being called, while also having sensible behavior
+                raise AttributeError(f'{self.name!r} is not defined on {obj!r}')
+
+            self.fn = fail
+
     class A(BaseModel):
         x: int
 
-        @class_deco
-        def _some_func(self):
-            return self.x
+        if use_annotation:
+            _some_func: MyDescriptor = MyDescriptor(lambda self: self.x)
+        else:
+            _some_func = MyDescriptor(lambda self: self.x)
+
+        @property
+        def _double_x(self):
+            return self.x * 2
+
+    if use_annotation or base is ModelPrivateAttr:
+        assert set(A.__private_attributes__) == {'_some_func'}
+    else:
+        assert set(A.__private_attributes__) == set()
+
+    assert set_name_calls == [(A, '_some_func')]
 
-    assert calls == [(A, '_some_func')]
     a = A(x=2)
 
-    # we don't test whether calling the method on a PrivateAttr works:
-    # attribute access on privateAttributes is more complicated, it doesn't
-    # get added to the class namespace (and will also get set on the instance
-    # with _init_private_attributes), so the descriptor protocol won't work.
-    if base is object:
-        assert a._some_func == 2
+    assert a._double_x == 4  # Ensure properties with leading underscores work fine and don't become private attributes
+
+    assert get_calls == []
+    assert a._some_func == 2
+    assert get_calls == [(a, A)]
+
+    assert set_calls == []
+    a._some_func = 3
+    assert set_calls == [(a, 3)]
+
+    assert a._some_func == 3
+    assert get_calls == [(a, A), (a, A)]
+
+    assert delete_calls == []
+    del a._some_func
+    assert delete_calls == [a]
+
+    with pytest.raises(AttributeError, match=r"'_some_func' is not defined on A\(x=2\)"):
+        a._some_func
+    assert get_calls == [(a, A), (a, A), (a, A)]
+
+
+def test_private_attr_set_name():
+    class SetNameInt(int):
+        _owner_attr_name: Optional[str] = None
+
+        def __set_name__(self, owner, name):
+            self._owner_attr_name = f'{owner.__name__}.{name}'
+
+    _private_attr_default = SetNameInt(1)
+
+    class Model(BaseModel):
+        _private_attr_1: int = PrivateAttr(default=_private_attr_default)
+        _private_attr_2: SetNameInt = SetNameInt(2)
+
+    assert _private_attr_default._owner_attr_name == 'Model._private_attr_1'
+
+    m = Model()
+    assert m._private_attr_1 == 1
+    assert m._private_attr_1._owner_attr_name == 'Model._private_attr_1'
+    assert m._private_attr_2 == 2
+    assert m._private_attr_2._owner_attr_name == 'Model._private_attr_2'
+
+
+def test_private_attr_default_descriptor_attribute_error():
+    class SetNameInt(int):
+        def __get__(self, obj, cls):
+            return self
+
+    _private_attr_default = SetNameInt(1)
+
+    class Model(BaseModel):
+        _private_attr: int = PrivateAttr(default=_private_attr_default)
+
+    assert Model.__private_attributes__['_private_attr'].__get__(None, Model) == _private_attr_default
+
+    with pytest.raises(AttributeError, match="'ModelPrivateAttr' object has no attribute 'some_attr'"):
+        Model.__private_attributes__['_private_attr'].some_attr
+
+
+def test_private_attr_set_name_do_not_crash_if_not_callable():
+    class SetNameInt(int):
+        __set_name__ = None
+
+    _private_attr_default = SetNameInt(2)
+
+    class Model(BaseModel):
+        _private_attr: int = PrivateAttr(default=_private_attr_default)
+
+    # Checks below are just to ensure that everything is the same as in `test_private_attr_set_name`
+    # The main check is that model class definition above doesn't crash
+    assert Model()._private_attr == 2
+
+
+def test_del_model_attr():
+    class Model(BaseModel):
+        some_field: str
+
+    m = Model(some_field='value')
+    assert hasattr(m, 'some_field')
+
+    del m.some_field
+
+    assert not hasattr(m, 'some_field')
+
+
+@pytest.mark.skipif(
+    platform.python_implementation() == 'PyPy' and platform.python_version_tuple() < ('3', '8'),
+    reason='In this single case `del` behaves weird on pypy 3.7',
+)
+def test_del_model_attr_error():
+    class Model(BaseModel):
+        some_field: str
+
+    m = Model(some_field='value')
+    assert not hasattr(m, 'other_field')
+
+    with pytest.raises(AttributeError, match='other_field'):
+        del m.other_field
+
+
+def test_del_model_attr_with_privat_attrs():
+    class Model(BaseModel):
+        _private_attr: int = PrivateAttr(default=1)
+        some_field: str
+
+    m = Model(some_field='value')
+    assert hasattr(m, 'some_field')
+
+    del m.some_field
+
+    assert not hasattr(m, 'some_field')
+
+
+def test_del_model_attr_with_privat_attrs_error():
+    class Model(BaseModel):
+        _private_attr: int = PrivateAttr(default=1)
+        some_field: str
+
+    m = Model(some_field='value')
+    assert not hasattr(m, 'other_field')
+
+    with pytest.raises(AttributeError, match="'Model' object has no attribute 'other_field'"):
+        del m.other_field
+
+
+def test_del_model_attr_with_privat_attrs_twice_error():
+    class Model(BaseModel):
+        _private_attr: int = 1
+        some_field: str
+
+    m = Model(some_field='value')
+    assert hasattr(m, '_private_attr')
+
+    del m._private_attr
+
+    with pytest.raises(AttributeError, match="'Model' object has no attribute '_private_attr'"):
+        del m._private_attr
 
 
 def test_create_model_with_slots():
     field_definitions = {'__slots__': (Optional[Tuple[str, ...]], None), 'foobar': (Optional[int], None)}
     with pytest.warns(RuntimeWarning, match='__slots__ should not be passed to create_model'):
         model = create_model('PartialPet', **field_definitions)
 
@@ -292,7 +470,33 @@
     assert model().foo == (1, 2)
     assert model(foo=(3, 4)).foo == (3, 4)
 
 
 def test_create_model_tuple_3():
     with pytest.raises(PydanticUserError, match=r'^Field definitions should either be a `\(<type>, <default>\)`\.\n'):
         create_model('FooModel', foo=(Tuple[int, int], (1, 2), 'more'))
+
+
+def test_create_model_protected_namespace_default():
+    with pytest.raises(NameError, match='Field "model_prefixed_field" has conflict with protected namespace "model_"'):
+        create_model('Model', model_prefixed_field=(str, ...))
+
+
+def test_create_model_custom_protected_namespace():
+    with pytest.raises(NameError, match='Field "test_field" has conflict with protected namespace "test_"'):
+        create_model(
+            'Model',
+            __config__=ConfigDict(protected_namespaces=('test_',)),
+            model_prefixed_field=(str, ...),
+            test_field=(str, ...),
+        )
+
+
+def test_create_model_multiple_protected_namespace():
+    with pytest.raises(
+        NameError, match='Field "also_protect_field" has conflict with protected namespace "also_protect_"'
+    ):
+        create_model(
+            'Model',
+            __config__=ConfigDict(protected_namespaces=('protect_me_', 'also_protect_')),
+            also_protect_field=(str, ...),
+        )
```

### Comparing `pydantic-2.0a4/tests/test_dataclasses.py` & `pydantic-2.0b1/tests/test_dataclasses.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,38 @@
 import dataclasses
 import pickle
 import re
 import sys
+import traceback
 from collections.abc import Hashable
+from dataclasses import InitVar
 from datetime import datetime
 from pathlib import Path
 from typing import Any, Callable, ClassVar, Dict, FrozenSet, Generic, List, Optional, Set, TypeVar, Union
 
 import pytest
 from dirty_equals import HasRepr
+from pydantic_core import ArgsKwargs, SchemaValidator
 from typing_extensions import Literal
 
 import pydantic
-from pydantic import BaseModel, ConfigDict, FieldValidationInfo, TypeAdapter, ValidationError
-from pydantic.decorators import field_validator
+from pydantic import (
+    BaseModel,
+    ConfigDict,
+    FieldValidationInfo,
+    PydanticUserError,
+    TypeAdapter,
+    ValidationError,
+    computed_field,
+    field_serializer,
+    field_validator,
+    model_validator,
+)
+from pydantic._internal._model_construction import MockValidator
+from pydantic.dataclasses import rebuild_dataclass
 from pydantic.fields import Field, FieldInfo
 from pydantic.json_schema import model_json_schema
 
 
 def test_simple():
     @pydantic.dataclasses.dataclass
     class MyDataclass:
@@ -709,34 +724,36 @@
         # Should this raise a TypeError instead? https://github.com/pydantic/pydantic/issues/5487
         MyDataclass()
     assert exc_info.value.errors(include_url=False) == [
         {'input': HasRepr('ArgsKwargs(())'), 'loc': ('v',), 'msg': 'Field required', 'type': 'missing'}
     ]
 
 
-@pytest.mark.parametrize(
-    'default',
-    [
-        1,
-        None,
-        pytest.param(
-            ...,
-            marks=pytest.mark.xfail(
-                reason='... makes field required: https://github.com/pydantic/pydantic/issues/5488'
-            ),
-        ),
-    ],
-)
-def test_hashable_optional(default):
+@pytest.mark.parametrize('default', [1, None])
+def test_default_value(default):
     @pydantic.dataclasses.dataclass
     class MyDataclass:
-        v: Hashable = default
+        v: int = default
 
-    MyDataclass()
-    MyDataclass(v=None)
+    assert dataclasses.asdict(MyDataclass()) == {'v': default}
+    assert dataclasses.asdict(MyDataclass(v=42)) == {'v': 42}
+
+
+def test_default_value_ellipsis():
+    """
+    https://github.com/pydantic/pydantic/issues/5488
+    """
+
+    @pydantic.dataclasses.dataclass
+    class MyDataclass:
+        v: int = ...
+
+    assert dataclasses.asdict(MyDataclass(v=42)) == {'v': 42}
+    with pytest.raises(ValidationError, match='type=missing'):
+        MyDataclass()
 
 
 def test_override_builtin_dataclass():
     @dataclasses.dataclass
     class File:
         hash: str
         name: Optional[str]
@@ -787,41 +804,44 @@
 
     f = File(filename=b'thefilename', modified_date='2020-01-01T00:00', seen_count='7')
     assert f.filename == 'thefilename'
     assert f.modified_date == datetime(2020, 1, 1, 0, 0)
     assert f.seen_count == 7
 
 
-@pytest.mark.xfail(reason='TODO we need to optionally run validation even on exact types')
+@pytest.mark.xfail(reason='Meta() is not being revalidated')
 def test_override_builtin_dataclass_nested():
     @dataclasses.dataclass
     class Meta:
         modified_date: Optional[datetime]
         seen_count: int
 
     @dataclasses.dataclass
     class File:
         filename: str
         meta: Meta
 
-    class Foo(BaseModel):
-        file: File
-
-    FileChecked = pydantic.dataclasses.dataclass(File)
+    FileChecked = pydantic.dataclasses.dataclass(File, config=ConfigDict(revalidate_instances='always'))
     f = FileChecked(filename=b'thefilename', meta=Meta(modified_date='2020-01-01T00:00', seen_count='7'))
     assert f.filename == 'thefilename'
     assert f.meta.modified_date == datetime(2020, 1, 1, 0, 0)
     assert f.meta.seen_count == 7
 
     with pytest.raises(ValidationError) as e:
         FileChecked(filename=b'thefilename', meta=Meta(modified_date='2020-01-01T00:00', seen_count=['7']))
+    # insert_assert(e.value.errors(include_url=False))
     assert e.value.errors(include_url=False) == [
-        {'loc': ('meta', 'seen_count'), 'msg': 'value is not a valid integer', 'type': 'type_error.integer'}
+        {'type': 'int_type', 'loc': ('meta', 'seen_count'), 'msg': 'Input should be a valid integer', 'input': ['7']}
     ]
 
+    class Foo(
+        BaseModel,
+    ):
+        file: File
+
     foo = Foo.model_validate(
         {
             'file': {
                 'filename': b'thefilename',
                 'meta': {'modified_date': '2020-01-01T00:00', 'seen_count': '7'},
             },
         }
@@ -1183,14 +1203,60 @@
         'properties': {'s': {'$ref': '#/$defs/Sentence'}},
         'required': ['s'],
         'title': 'M',
         'type': 'object',
     }
 
 
+def test_json_schema_with_computed_field():
+    @dataclasses.dataclass
+    class MyDataclass:
+        x: int
+
+        @computed_field
+        @property
+        def double_x(self) -> int:
+            return 2 * self.x
+
+    class Model(BaseModel):
+        dc: MyDataclass
+
+    assert Model.model_json_schema(mode='validation') == {
+        '$defs': {
+            'MyDataclass': {
+                'properties': {'x': {'title': 'X', 'type': 'integer'}},
+                'required': ['x'],
+                'title': 'MyDataclass',
+                'type': 'object',
+            }
+        },
+        'properties': {'dc': {'$ref': '#/$defs/MyDataclass'}},
+        'required': ['dc'],
+        'title': 'Model',
+        'type': 'object',
+    }
+    assert Model.model_json_schema(mode='serialization') == {
+        '$defs': {
+            'MyDataclass': {
+                'properties': {
+                    'double_x': {'title': 'Double X', 'type': 'integer'},
+                    'x': {'title': 'X', 'type': 'integer'},
+                },
+                'required': ['x', 'double_x'],
+                'title': 'MyDataclass',
+                'type': 'object',
+            }
+        },
+        'properties': {'dc': {'$ref': '#/$defs/MyDataclass'}},
+        'required': ['dc'],
+        'title': 'Model',
+        'type': 'object',
+    }
+
+
 def test_issue_2594():
     @dataclasses.dataclass
     class Empty:
         pass
 
     @pydantic.dataclasses.dataclass
     class M:
@@ -1325,16 +1391,19 @@
         set_wrapper: SetWrapper
 
     model = Model(set_wrapper=SetWrapper({1, 2, 3}))
     json_text = model.model_dump_json()
     assert Model.model_validate_json(json_text).model_dump() == model.model_dump()
 
 
-@pytest.mark.xfail(reason='pydantic dataclasses currently do not preserve sunder attributes set in __new__')
-def test_keeps_custom_properties():
+def test_new_not_called():
+    """
+    pydantic dataclasses do not preserve sunder attributes set in __new__
+    """
+
     class StandardClass:
         """Class which modifies instance creation."""
 
         a: str
 
         def __new__(cls, *args, **kwargs):
             instance = super().__new__(cls)
@@ -1342,21 +1411,23 @@
             instance._special_property = 1
 
             return instance
 
     StandardLibDataclass = dataclasses.dataclass(StandardClass)
     PydanticDataclass = pydantic.dataclasses.dataclass(StandardClass)
 
-    clases_to_test = [StandardLibDataclass, PydanticDataclass]
-
     test_string = 'string'
-    for cls in clases_to_test:
-        instance = cls(a=test_string)
-        assert instance._special_property == 1
-        assert instance.a == test_string
+
+    std_instance = StandardLibDataclass(a=test_string)
+    assert std_instance._special_property == 1
+    assert std_instance.a == test_string
+
+    pyd_instance = PydanticDataclass(a=test_string)
+    assert not hasattr(pyd_instance, '_special_property')
+    assert pyd_instance.a == test_string
 
 
 def test_ignore_extra():
     @pydantic.dataclasses.dataclass(config=ConfigDict(extra='ignore'))
     class Foo:
         x: int
 
@@ -1406,62 +1477,156 @@
 
     msg = re.escape("Unexpected keyword argument [type=unexpected_keyword_argument, input_value='2', input_type=str]")
 
     with pytest.raises(ValidationError, match=msg):
         Foo(**{'x': '1', 'y': '2'})
 
 
-@pytest.mark.xfail(reason='need to make it possible to rebuild dataclasses')
 def test_self_reference_dataclass():
     @pydantic.dataclasses.dataclass
     class MyDataclass:
         self_reference: Optional['MyDataclass'] = None
 
-    # rebuild_pydantic_dataclass(MyDataclass)
-
     assert MyDataclass.__pydantic_fields__['self_reference'].annotation == Optional[MyDataclass]
 
     instance = MyDataclass(self_reference=MyDataclass(self_reference=MyDataclass()))
     assert TypeAdapter(MyDataclass).dump_python(instance) == {
         'self_reference': {'self_reference': {'self_reference': None}}
     }
 
     with pytest.raises(ValidationError) as exc_info:
-        MyDataclass(self_reference=MyDataclass(self_reference=1))
+        MyDataclass(self_reference=1)
 
     assert exc_info.value.errors(include_url=False) == [
         {
             'ctx': {'dataclass_name': 'MyDataclass'},
             'input': 1,
             'loc': ('self_reference',),
             'msg': 'Input should be a dictionary or an instance of MyDataclass',
             'type': 'dataclass_type',
         }
     ]
 
 
-@pytest.mark.xfail(reason='need to make it possible to rebuild dataclasses')
-def test_cyclic_reference_dataclass():
-    @pydantic.dataclasses.dataclass
+def test_cyclic_reference_dataclass(create_module):
+    @pydantic.dataclasses.dataclass(config=ConfigDict(extra='forbid'))
     class D1:
         d2: Optional['D2'] = None
 
-    @pydantic.dataclasses.dataclass
-    class D2:
-        d1: Optional[D1] = None
+    @create_module
+    def module():
+        from typing import Optional
 
-    # rebuild_pydantic_dataclass(D1)
+        import pydantic
+
+        @pydantic.dataclasses.dataclass(config=pydantic.ConfigDict(extra='forbid'))
+        class D2:
+            d1: Optional['D1'] = None
+
+    # Ensure D2 is in the local namespace; note everything works even though it wasn't _defined_ in this namespace
+    D2 = module.D2
+
+    # Confirm D1 and D2 require rebuilding
+    assert isinstance(D1.__pydantic_validator__, MockValidator)
+    assert isinstance(D2.__pydantic_validator__, MockValidator)
 
+    # Note: the rebuilds of D1 and D2 happen automatically, and works since it grabs the locals here as the namespace,
+    # which contains D1 and D2
     instance = D1(d2=D2(d1=D1(d2=D2(d1=D1()))))
 
-    assert TypeAdapter(D1).dump_python(instance) == {...}
+    # Confirm D1 and D2 have been rebuilt
+    assert isinstance(D1.__pydantic_validator__, SchemaValidator)
+    assert isinstance(D2.__pydantic_validator__, SchemaValidator)
+
+    assert TypeAdapter(D1).dump_python(instance) == {'d2': {'d1': {'d2': {'d1': {'d2': None}}}}}
 
     with pytest.raises(ValidationError) as exc_info:
-        D1(d2=D2(d1=D1(d2=D2(d1=D2()))))
-    assert exc_info.value.errors(include_url=False) == [...]
+        D2(d1=D2())
+    assert exc_info.value.errors(include_url=False) == [
+        {
+            'ctx': {'dataclass_name': 'D1'},
+            'input': D2(d1=None),
+            'loc': ('d1',),
+            'msg': 'Input should be a dictionary or an instance of D1',
+            'type': 'dataclass_type',
+        }
+    ]
+
+    with pytest.raises(ValidationError) as exc_info:
+        TypeAdapter(D1).validate_python(dict(d2=dict(d1=dict(d2=dict(d2=dict())))))
+    assert exc_info.value.errors(include_url=False) == [
+        {
+            'input': {},
+            'loc': ('d2', 'd1', 'd2', 'd2'),
+            'msg': 'Unexpected keyword argument',
+            'type': 'unexpected_keyword_argument',
+        }
+    ]
+
+
+def test_cross_module_cyclic_reference_dataclass(create_module):
+    @pydantic.dataclasses.dataclass(config=ConfigDict(extra='forbid'))
+    class D1:
+        d2: Optional['D2'] = None  # noqa F821
+
+    @create_module
+    def module():
+        from typing import Optional
+
+        import pydantic
+
+        @pydantic.dataclasses.dataclass(config=pydantic.ConfigDict(extra='forbid'))
+        class D2:
+            d1: Optional['D1'] = None
+
+    # Since D2 is not in locals, it will not be picked up by the auto-rebuild:
+    with pytest.raises(
+        PydanticUserError,
+        match=re.escape(
+            '`D1` is not fully defined; you should define `D2`, then call'
+            ' `pydantic.dataclasses.rebuild_dataclass(D1)` before the first `D1` instance is created.'
+        ),
+    ):
+        D1()
+
+    # Explicitly rebuild D1, specifying the appropriate types namespace
+    rebuild_dataclass(D1, _types_namespace={'D2': module.D2, 'D1': D1})
+
+    # Confirm D2 still requires a rebuild (it will happen automatically)
+    assert isinstance(module.D2.__pydantic_validator__, MockValidator)
+
+    instance = D1(d2=module.D2(d1=D1(d2=module.D2(d1=D1()))))
+
+    # Confirm auto-rebuild of D2 has now happened
+    assert isinstance(module.D2.__pydantic_validator__, SchemaValidator)
+
+    assert TypeAdapter(D1).dump_python(instance) == {'d2': {'d1': {'d2': {'d1': {'d2': None}}}}}
+
+    with pytest.raises(ValidationError) as exc_info:
+        module.D2(d1=module.D2())
+    assert exc_info.value.errors(include_url=False) == [
+        {
+            'ctx': {'dataclass_name': 'D1'},
+            'input': module.D2(d1=None),
+            'loc': ('d1',),
+            'msg': 'Input should be a dictionary or an instance of D1',
+            'type': 'dataclass_type',
+        }
+    ]
+
+    with pytest.raises(ValidationError) as exc_info:
+        TypeAdapter(D1).validate_python(dict(d2=dict(d1=dict(d2=dict(d2=dict())))))
+    assert exc_info.value.errors(include_url=False) == [
+        {
+            'input': {},
+            'loc': ('d2', 'd1', 'd2', 'd2'),
+            'msg': 'Unexpected keyword argument',
+            'type': 'unexpected_keyword_argument',
+        }
+    ]
 
 
 @pytest.mark.skipif(sys.version_info < (3, 10), reason='kw_only is not available in python < 3.10')
 def test_kw_only():
     @pydantic.dataclasses.dataclass(kw_only=True)
     class A:
         a: int | None = None
@@ -1469,14 +1634,60 @@
 
     with pytest.raises(ValidationError):
         A(1, '')
 
     assert A(b='hi').b == 'hi'
 
 
+def dataclass_decorators(include_identity: bool = False, exclude_combined: bool = False):
+    decorators = [pydantic.dataclasses.dataclass, dataclasses.dataclass]
+    ids = ['pydantic', 'stdlib']
+
+    if not exclude_combined:
+
+        def combined_decorator(cls):
+            """
+            Should be equivalent to:
+            @pydantic.dataclasses.dataclass
+            @dataclasses.dataclass
+            """
+            return pydantic.dataclasses.dataclass(dataclasses.dataclass(cls))
+
+        decorators.append(combined_decorator)
+        ids.append('combined')
+
+    if include_identity:
+
+        def identity_decorator(cls):
+            return cls
+
+        decorators.append(identity_decorator)
+        ids.append('identity')
+
+    return {'argvalues': decorators, 'ids': ids}
+
+
+@pytest.mark.skipif(sys.version_info < (3, 10), reason='kw_only is not available in python < 3.10')
+@pytest.mark.parametrize('decorator1', **dataclass_decorators(exclude_combined=True))
+@pytest.mark.parametrize('decorator2', **dataclass_decorators(exclude_combined=True))
+def test_kw_only_inheritance(decorator1, decorator2):
+    # Exclude combined from the decorators since it doesn't know how to accept kw_only
+    @decorator1(kw_only=True)
+    class Parent:
+        x: int
+
+    @decorator2
+    class Child(Parent):
+        y: int
+
+    child = Child(1, x=2)
+    assert child.x == 2
+    assert child.y == 1
+
+
 def test_extra_forbid_list_no_error():
     @pydantic.dataclasses.dataclass(config=dict(extra='forbid'))
     class Bar:
         ...
 
     @pydantic.dataclasses.dataclass
     class Foo:
@@ -1490,30 +1701,62 @@
     class Bar:
         ...
 
     with pytest.raises(ValidationError, match=r'a\s+Unexpected keyword argument'):
         Bar(a=1)
 
 
-def test_validator():
+def test_field_validator():
     @pydantic.dataclasses.dataclass
     class MyDataclass:
         a: int
         b: float
 
         @field_validator('b')
         @classmethod
-        def double_b(cls, v, _):
+        def double_b(cls, v):
             return v * 2
 
     d = MyDataclass('1', '2.5')
     assert d.a == 1
     assert d.b == 5.0
 
 
+def test_model_validator_before():
+    @pydantic.dataclasses.dataclass
+    class MyDataclass:
+        a: int
+        b: float
+
+        @model_validator(mode='before')
+        def double_b(cls, v: ArgsKwargs):
+            v.kwargs['b'] *= 2
+            return v
+
+    d = MyDataclass('1', b='2')
+    assert d.a == 1
+    assert d.b == 22.0
+
+
+def test_model_validator_after():
+    @pydantic.dataclasses.dataclass
+    class MyDataclass:
+        a: int
+        b: float
+
+        @model_validator(mode='after')
+        def double_b(cls, dc: 'MyDataclass'):
+            dc.b *= 2
+            return dc
+
+    d = MyDataclass('1', b='2')
+    assert d.a == 1
+    assert d.b == 4
+
+
 def test_parent_post_init():
     """
     Test that the parent's __post_init__ gets called
     and the order in which it gets called relative to validation.
 
     In V1 we called it before validation, in V2 it gets called after.
     """
@@ -1623,15 +1866,15 @@
     'decorator1, expected_parent, expected_child',
     [
         (
             pydantic.dataclasses.dataclass,
             ['parent before', 'parent', 'parent after'],
             ['parent before', 'child', 'parent after', 'child before', 'child after'],
         ),
-        (dataclasses.dataclass, [], ['child before', 'child', 'child after']),
+        (dataclasses.dataclass, [], ['parent before', 'child', 'parent after', 'child before', 'child after']),
     ],
     ids=['pydantic', 'stdlib'],
 )
 def test_inheritance_replace(decorator1: Callable[[Any], Any], expected_parent: List[str], expected_child: List[str]):
     """We promise that if you add a validator
     with the same _function_ name as an existing validator
     it replaces the existing validator and is run instead of it.
@@ -1743,34 +1986,14 @@
             'loc': ('x',),
             'msg': 'Assertion failed, assert -1 > 0',
             'type': 'assertion_error',
         }
     ]
 
 
-def dataclass_decorators(identity: bool = False):
-    def combined(cls):
-        """
-        Should be equivalent to:
-        @pydantic.dataclasses.dataclass
-        @dataclasses.dataclass
-        """
-        return pydantic.dataclasses.dataclass(dataclasses.dataclass(cls))
-
-    def identity_decorator(cls):
-        return cls
-
-    decorators = [pydantic.dataclasses.dataclass, dataclasses.dataclass, combined]
-    ids = ['pydantic', 'stdlib', 'combined']
-    if identity:
-        decorators.append(identity_decorator)
-        ids.append('identity')
-    return {'argvalues': decorators, 'ids': ids}
-
-
 @pytest.mark.parametrize('dataclass_decorator', **dataclass_decorators())
 def test_unparametrized_generic_dataclass(dataclass_decorator):
     T = TypeVar('T')
 
     @dataclass_decorator
     class GenericDataclass(Generic[T]):
         x: T
@@ -1825,15 +2048,15 @@
         assert validator.validate_python({'x': input_value}).x == output_value
     else:
         with pytest.raises(ValidationError) as exc_info:
             validator.validate_python({'x': input_value})
         assert exc_info.value.errors(include_url=False) == output_value
 
 
-@pytest.mark.parametrize('dataclass_decorator', **dataclass_decorators(identity=True))
+@pytest.mark.parametrize('dataclass_decorator', **dataclass_decorators(include_identity=True))
 def test_pydantic_dataclass_preserves_metadata(dataclass_decorator: Callable[[Any], Any]) -> None:
     @dataclass_decorator
     class FooStd:
         """Docstring"""
 
     FooPydantic = pydantic.dataclasses.dataclass(FooStd)
 
@@ -1865,7 +2088,209 @@
     gordon = module.Cook([])
 
     burger = module.Recipe(author=gordon)
 
     me = module.Foo([burger])
 
     assert me.recipes == [burger]
+
+
+def test_dataclass_alias_generator():
+    def alias_generator(name: str) -> str:
+        return 'alias_' + name
+
+    @pydantic.dataclasses.dataclass(config=ConfigDict(alias_generator=alias_generator))
+    class User:
+        name: str
+        score: int = Field(alias='my_score')
+
+    user = User(**{'alias_name': 'test name', 'my_score': 2})
+    assert user.name == 'test name'
+    assert user.score == 2
+
+    with pytest.raises(ValidationError) as exc_info:
+        User(name='test name', score=2)
+    assert exc_info.value.errors(include_url=False) == [
+        {
+            'type': 'missing',
+            'loc': ('alias_name',),
+            'msg': 'Field required',
+            'input': ArgsKwargs((), {'name': 'test name', 'score': 2}),
+        },
+        {
+            'type': 'missing',
+            'loc': ('my_score',),
+            'msg': 'Field required',
+            'input': ArgsKwargs((), {'name': 'test name', 'score': 2}),
+        },
+    ]
+
+
+@pytest.mark.skipif(sys.version_info < (3, 8), reason='InitVar not supported in python 3.7')
+def test_init_vars_inheritance():
+    init_vars = []
+
+    @pydantic.dataclasses.dataclass
+    class Foo:
+        init: 'InitVar[int]'
+
+    @pydantic.dataclasses.dataclass
+    class Bar(Foo):
+        arg: int
+
+        def __post_init__(self, init: int) -> None:
+            init_vars.append(init)
+
+    bar = Bar(init=1, arg=2)
+    assert TypeAdapter(Bar).dump_python(bar) == {'arg': 2}
+    assert init_vars == [1]
+
+    with pytest.raises(ValidationError) as exc_info:
+        Bar(init='a', arg=2)
+    assert exc_info.value.errors(include_url=False) == [
+        {
+            'input': 'a',
+            'loc': ('init',),
+            'msg': 'Input should be a valid integer, unable to parse string as an integer',
+            'type': 'int_parsing',
+        }
+    ]
+
+
+@pytest.mark.skipif(not hasattr(pydantic.dataclasses, '_call_initvar'), reason='InitVar was not modified')
+@pytest.mark.parametrize('remove_monkeypatch', [True, False])
+def test_init_vars_call_monkeypatch(remove_monkeypatch, monkeypatch):
+    # Parametrizing like this allows us to test that the behavior is the same with or without the monkeypatch
+
+    if remove_monkeypatch:
+        monkeypatch.delattr(InitVar, '__call__')
+
+    InitVar(int)  # this is what is produced by InitVar[int]; note monkeypatching __call__ doesn't break this
+
+    with pytest.raises(TypeError, match="'InitVar' object is not callable") as exc:
+        InitVar[int]()
+
+    # Check that the custom __call__ was called precisely if the monkeypatch was not removed
+    stack_depth = len(traceback.extract_tb(exc.value.__traceback__))
+    assert stack_depth == 1 if remove_monkeypatch else 2
+
+
+@pytest.mark.parametrize('decorator1', **dataclass_decorators())
+@pytest.mark.parametrize('decorator2', **dataclass_decorators())
+def test_decorators_in_model_field(decorator1, decorator2):
+    @decorator1
+    class Demo1:
+        int1: int
+
+        @field_validator('int1', mode='before')
+        def set_int_1(cls, v):
+            return v + 100
+
+        @field_serializer('int1')
+        def serialize_int_1(self, v):
+            return v + 10
+
+    @decorator2
+    class Demo2(Demo1):
+        int2: int
+
+        @field_validator('int2', mode='before')
+        def set_int_2(cls, v):
+            return v + 200
+
+        @field_serializer('int2')
+        def serialize_int_2(self, v):
+            return v + 20
+
+    class Model(BaseModel):
+        x: Demo2
+
+    m = Model.model_validate(dict(x=dict(int1=1, int2=2)))
+    assert m.x.int1 == 101
+    assert m.x.int2 == 202
+
+    assert m.model_dump() == {'x': {'int1': 111, 'int2': 222}}
+
+
+@pytest.mark.parametrize('decorator1', **dataclass_decorators())
+@pytest.mark.parametrize('decorator2', **dataclass_decorators())
+def test_vanilla_dataclass_decorators_in_type_adapter(decorator1, decorator2):
+    @decorator1
+    class Demo1:
+        int1: int
+
+        @field_validator('int1', mode='before')
+        def set_int_1(cls, v):
+            return v + 100
+
+        @field_serializer('int1')
+        def serialize_int_1(self, v):
+            return v + 10
+
+    @decorator2
+    class Demo2(Demo1):
+        int2: int
+
+        @field_validator('int2', mode='before')
+        def set_int_2(cls, v):
+            return v + 200
+
+        @field_serializer('int2')
+        def serialize_int_2(self, v):
+            return v + 20
+
+    adapter = TypeAdapter(Demo2)
+
+    m = adapter.validate_python(dict(int1=1, int2=2))
+    assert m.int1 == 101
+    assert m.int2 == 202
+
+    assert adapter.dump_python(m) == {'int1': 111, 'int2': 222}
+
+
+@pytest.mark.parametrize(
+    'dataclass_decorator',
+    [
+        pydantic.dataclasses.dataclass,
+        dataclasses.dataclass,
+    ],
+    ids=['pydantic', 'stdlib'],
+)
+@pytest.mark.skipif(sys.version_info < (3, 10), reason='slots are only supported for dataclasses in Python >= 3.10')
+def test_dataclass_slots(dataclass_decorator):
+    @dataclass_decorator(slots=True)
+    class Model:
+        a: str
+        b: str
+
+    dc = TypeAdapter(Model).validate_python({'a': 'foo', 'b': 'bar'})
+    assert dc.a == 'foo'
+    assert dc.b == 'bar'
+
+
+@pytest.mark.parametrize(
+    'dataclass_decorator',
+    [
+        pydantic.dataclasses.dataclass,
+        dataclasses.dataclass,
+    ],
+    ids=['pydantic', 'stdlib'],
+)
+@pytest.mark.skipif(sys.version_info < (3, 10), reason='slots are only supported for dataclasses in Python >= 3.10')
+def test_dataclass_slots_mixed(dataclass_decorator):
+    @dataclass_decorator(slots=True)
+    class Model:
+        x: int
+        y: dataclasses.InitVar[str]
+        z: ClassVar[str] = 'z-classvar'
+
+    @dataclass_decorator
+    class SubModel(Model):
+        x2: int
+        y2: dataclasses.InitVar[str]
+        z2: ClassVar[str] = 'z2-classvar'
+
+    dc = TypeAdapter(SubModel).validate_python({'x': 1, 'y': 'a', 'x2': 2, 'y2': 'b'})
+    assert dc.x == 1
+    assert dc.x2 == 2
+    assert SubModel.z == 'z-classvar'
+    assert SubModel.z2 == 'z2-classvar'
```

### Comparing `pydantic-2.0a4/tests/test_datetime.py` & `pydantic-2.0b1/tests/test_datetime.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,25 @@
 import re
 from datetime import date, datetime, time, timedelta, timezone
 
 import pytest
 from dirty_equals import HasRepr
 from typing_extensions import Annotated
 
-from pydantic import AwareDatetime, BaseModel, FutureDate, NaiveDatetime, PastDate, ValidationError, condate
+from pydantic import (
+    AwareDatetime,
+    BaseModel,
+    FutureDate,
+    FutureDatetime,
+    NaiveDatetime,
+    PastDate,
+    PastDatetime,
+    ValidationError,
+    condate,
+)
 
 from .conftest import Err
 
 
 def create_tz(minutes):
     return timezone(timedelta(minutes=minutes))
 
@@ -20,14 +30,24 @@
 
 
 @pytest.fixture(scope='module', params=[PastDate, Annotated[date, PastDate()]])
 def past_date_type(request):
     return request.param
 
 
+@pytest.fixture(scope='module', params=[FutureDatetime, Annotated[datetime, FutureDatetime()]])
+def future_datetime_type(request):
+    return request.param
+
+
+@pytest.fixture(scope='module', params=[PastDatetime, Annotated[datetime, PastDatetime()]])
+def past_datetime_type(request):
+    return request.param
+
+
 @pytest.fixture(scope='module', params=[AwareDatetime, Annotated[datetime, AwareDatetime()]])
 def aware_datetime_type(request):
     return request.param
 
 
 @pytest.fixture(scope='module', params=[NaiveDatetime, Annotated[datetime, NaiveDatetime()]])
 def naive_datetime_type(request):
@@ -102,23 +122,23 @@
         # Invalid inputs
         ('4:8:16', Err('Input should be in a valid time format, invalid character in hour [type=time_parsing,')),
         (86400, Err('Input should be in a valid time format, numeric times may not exceed 86,399 seconds')),
         ('xxx', Err('Input should be in a valid time format, input is too short [type=time_parsing,')),
         ('091500', Err('Input should be in a valid time format, invalid time separator, expected `:`')),
         (b'091500', Err('Input should be in a valid time format, invalid time separator, expected `:`')),
         ('09:15:90', Err('Input should be in a valid time format, second value is outside expected range of 0-59')),
-        ('11:05:00Y', Err('Input should be in a valid time format, unexpected extra characters at the end of the inp')),
-        # # https://github.com/pydantic/speedate/issues/10
-        # ('11:05:00-05:30', time(11, 5, 0, tzinfo=create_tz(-330))),
-        # ('11:05:00-0530', time(11, 5, 0, tzinfo=create_tz(-330))),
-        # ('11:05:00Z', time(11, 5, 0, tzinfo=timezone.utc)),
-        # ('11:05:00+00', time(11, 5, 0, tzinfo=timezone.utc)),
-        # ('11:05-06', time(11, 5, 0, tzinfo=create_tz(-360))),
-        # ('11:05+06', time(11, 5, 0, tzinfo=create_tz(360))),
-        # ('11:05:00-25:00', errors.TimeError),
+        ('11:05:00Y', Err('Input should be in a valid time format, invalid timezone sign')),
+        # https://github.com/pydantic/speedate/issues/10
+        ('11:05:00-05:30', time(11, 5, 0, tzinfo=create_tz(-330))),
+        ('11:05:00-0530', time(11, 5, 0, tzinfo=create_tz(-330))),
+        ('11:05:00Z', time(11, 5, 0, tzinfo=timezone.utc)),
+        ('11:05:00+00:00', time(11, 5, 0, tzinfo=timezone.utc)),
+        ('11:05-06:00', time(11, 5, 0, tzinfo=create_tz(-360))),
+        ('11:05+06:00', time(11, 5, 0, tzinfo=create_tz(360))),
+        ('11:05:00-25:00', Err('Input should be in a valid time format, timezone offset must be less than 24 hours')),
     ],
 )
 def test_time_parsing(TimeModel, value, result):
     if isinstance(result, Err):
         with pytest.raises(ValidationError, match=result.message_escaped()):
             TimeModel(d=value)
     else:
@@ -146,20 +166,21 @@
         ('2012-04-23T09:15:00Z', datetime(2012, 4, 23, 9, 15, 0, 0, timezone.utc)),
         ('2012-04-23T10:20:30.400+02:30', datetime(2012, 4, 23, 10, 20, 30, 400_000, create_tz(150))),
         ('2012-04-23T10:20:30.400+02:00', datetime(2012, 4, 23, 10, 20, 30, 400_000, create_tz(120))),
         ('2012-04-23T10:20:30.400-02:00', datetime(2012, 4, 23, 10, 20, 30, 400_000, create_tz(-120))),
         (b'2012-04-23T10:20:30.400-02:00', datetime(2012, 4, 23, 10, 20, 30, 400_000, create_tz(-120))),
         (datetime(2017, 5, 5), datetime(2017, 5, 5)),
         (0, datetime(1970, 1, 1, 0, 0, 0)),
-        # # Invalid inputs
-        ('1494012444.883309', Err('Input should be a valid datetime, invalid date separator')),
-        ('1494012444', Err('Input should be a valid datetime, invalid date separator')),
-        (b'1494012444', Err('Input should be a valid datetime, invalid date separator')),
-        ('1494012444000.883309', Err('Input should be a valid datetime, invalid date separator')),
-        ('-1494012444000.883309', Err('Input should be a valid datetime, invalid character in year')),
+        # Numeric inputs as strings
+        ('1494012444.883309', datetime(2017, 5, 5, 19, 27, 24, 883309)),
+        ('1494012444', datetime(2017, 5, 5, 19, 27, 24)),
+        (b'1494012444', datetime(2017, 5, 5, 19, 27, 24)),
+        ('1494012444000.883309', datetime(2017, 5, 5, 19, 27, 24, 883301)),
+        ('-1494012444000.883309', datetime(1922, 8, 29, 4, 32, 35, 999000)),
+        # Invalid inputs
         ('2012-4-9 4:8:16', Err('Input should be a valid datetime, invalid character in month')),
         ('x20120423091500', Err('Input should be a valid datetime, invalid character in year')),
         ('2012-04-56T09:15:90', Err('Input should be a valid datetime, day value is outside expected range')),
         ('2012-04-23T11:05:00-25:00', Err('Input should be a valid datetime, timezone offset must be less than 24 ho')),
         (19_999_999_999, datetime(2603, 10, 11, 11, 33, 19)),  # just before watershed
         (20_000_000_001, datetime(1970, 8, 20, 11, 33, 20, 1000)),  # just after watershed
         (1_549_316_052, datetime(2019, 2, 4, 21, 34, 12, 0)),  # nowish in s
@@ -197,17 +218,17 @@
     value = datetime.now()
 
     with pytest.raises(ValidationError) as exc_info:
         Model(foo=value)
 
     assert exc_info.value.errors(include_url=False) == [
         {
-            'type': 'datetime_aware',
+            'type': 'timezone_aware',
             'loc': ('foo',),
-            'msg': 'Datetime should have timezone info',
+            'msg': 'Input should have timezone info',
             'input': value,
         }
     ]
 
 
 def test_naive_datetime_validation_success(naive_datetime_type):
     class Model(BaseModel):
@@ -225,17 +246,17 @@
     value = datetime.now(tz=timezone.utc)
 
     with pytest.raises(ValidationError) as exc_info:
         Model(foo=value)
 
     assert exc_info.value.errors(include_url=False) == [
         {
-            'type': 'datetime_naive',
+            'type': 'timezone_naive',
             'loc': ('foo',),
-            'msg': 'Datetime should not have timezone info',
+            'msg': 'Input should not have timezone info',
             'input': value,
         }
     ]
 
 
 @pytest.fixture(scope='module', name='TimedeltaModel')
 def timedelta_model_fixture():
@@ -482,7 +503,95 @@
         {
             'type': 'date_future',
             'loc': ('foo',),
             'msg': 'Date should be in the future',
             'input': value,
         }
     ]
+
+
+@pytest.mark.parametrize(
+    'value,result',
+    (
+        ('1996-01-22T10:20:30', datetime(1996, 1, 22, 10, 20, 30)),
+        (datetime(1996, 1, 22, 10, 20, 30), datetime(1996, 1, 22, 10, 20, 30)),
+    ),
+)
+def test_past_datetime_validation_success(value, result, past_datetime_type):
+    class Model(BaseModel):
+        foo: past_datetime_type
+
+    assert Model(foo=value).foo == result
+
+
+@pytest.mark.parametrize(
+    'value',
+    (
+        datetime.now() + timedelta(1),
+        '2064-06-01T10:20:30',
+    ),
+)
+def test_past_datetime_validation_fails(value, past_datetime_type):
+    class Model(BaseModel):
+        foo: past_datetime_type
+
+    with pytest.raises(ValidationError) as exc_info:
+        Model(foo=value)
+    assert exc_info.value.errors(include_url=False) == [
+        {
+            'type': 'datetime_past',
+            'loc': ('foo',),
+            'msg': 'Input should be in the past',
+            'input': value,
+        }
+    ]
+
+
+def test_future_datetime_validation_success(future_datetime_type):
+    class Model(BaseModel):
+        foo: future_datetime_type
+
+    d = datetime.now() + timedelta(1)
+    assert Model(foo=d).foo == d
+    assert Model(foo='2064-06-01T10:20:30').foo == datetime(2064, 6, 1, 10, 20, 30)
+
+
+@pytest.mark.parametrize(
+    'value',
+    (
+        datetime.now(),
+        datetime.now() - timedelta(1),
+        '1996-01-22T10:20:30',
+    ),
+)
+def test_future_datetime_validation_fails(value, future_datetime_type):
+    class Model(BaseModel):
+        foo: future_datetime_type
+
+    with pytest.raises(ValidationError) as exc_info:
+        Model(foo=value)
+    assert exc_info.value.errors(include_url=False) == [
+        {
+            'type': 'datetime_future',
+            'loc': ('foo',),
+            'msg': 'Input should be in the future',
+            'input': value,
+        }
+    ]
+
+
+@pytest.mark.parametrize(
+    'annotation',
+    (
+        PastDate,
+        PastDatetime,
+        FutureDate,
+        FutureDatetime,
+        NaiveDatetime,
+        AwareDatetime,
+    ),
+)
+def test_invalid_annotated_type(annotation):
+    with pytest.raises(TypeError, match=f"'{annotation.__name__}' cannot annotate 'str'."):
+
+        class Model(BaseModel):
+            foo: Annotated[str, annotation()]
```

### Comparing `pydantic-2.0a4/tests/test_deprecated.py` & `pydantic-2.0b1/tests/test_deprecated.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,20 +5,21 @@
 from pathlib import Path
 from types import SimpleNamespace
 from typing import Any, Dict, List, Type
 
 import pytest
 from typing_extensions import Literal
 
-from pydantic import BaseModel, ConfigDict, Field, PydanticUserError, ValidationError, model_serializer, root_validator
+from pydantic import BaseModel, ConfigDict, Field, PydanticUserError, ValidationError, conlist, root_validator
 from pydantic.config import Extra
 from pydantic.deprecated.decorator import validate_arguments
 from pydantic.deprecated.json import custom_pydantic_encoder, pydantic_encoder, timedelta_isoformat
 from pydantic.deprecated.parse import load_file, load_str_bytes
 from pydantic.deprecated.tools import parse_obj_as, schema_json_of, schema_of
+from pydantic.functional_serializers import model_serializer
 
 if sys.version_info < (3, 11):
     from typing_extensions import get_overloads
 else:
     from typing import get_overloads
 
 
@@ -29,119 +30,80 @@
             'The `from_orm` method is deprecated; set `model_config["from_attributes"]=True` '
             'and use `model_validate` instead.'
         ),
     ):
         return model_type.from_orm(obj)
 
 
-@pytest.mark.xfail(reason='working on V2')
-def test_getdict():
-    class TestCls:
-        a = 1
-        b: int
-
-        def __init__(self):
-            self.c = 3
-
-        @property
-        def d(self):
-            return 4
-
-        def __getattr__(self, key):
-            if key == 'e':
-                return 5
-            else:
-                raise AttributeError()
-
-    t = TestCls()
-    # gd = GetterDict(t)
-    gd = object(t)
-    assert gd.keys() == ['a', 'c', 'd']
-    assert gd.get('a') == 1
-    assert gd['a'] == 1
-    with pytest.raises(KeyError):
-        assert gd['foobar']
-    assert gd.get('b', None) is None
-    assert gd.get('b', 1234) == 1234
-    assert gd.get('c', None) == 3
-    assert gd.get('d', None) == 4
-    assert gd.get('e', None) == 5
-    assert gd.get('f', 'missing') == 'missing'
-    assert list(gd.values()) == [1, 3, 4]
-    assert list(gd.items()) == [('a', 1), ('c', 3), ('d', 4)]
-    assert list(gd) == ['a', 'c', 'd']
-    assert gd == {'a': 1, 'c': 3, 'd': 4}
-    assert 'a' in gd
-    assert len(gd) == 3
-    assert str(gd) == "{'a': 1, 'c': 3, 'd': 4}"
-    assert repr(gd) == "GetterDict[TestCls]({'a': 1, 'c': 3, 'd': 4})"
-
-
 def test_from_attributes_root():
     class PokemonCls:
         def __init__(self, *, en_name: str, jp_name: str):
             self.en_name = en_name
             self.jp_name = jp_name
 
     class Pokemon(BaseModel):
         model_config = ConfigDict(from_attributes=True)
         en_name: str
         jp_name: str
 
-    class PokemonList(BaseModel):
-        root: List[Pokemon]
+    with pytest.warns(DeprecationWarning, match='Pydantic V1 style `@root_validator` validators are deprecated.'):
 
-        @root_validator(pre=True)
-        @classmethod
-        def populate_root(cls, values):
-            return {'root': values}
-
-        @model_serializer(mode='wrap')
-        def _serialize(self, handler, info):
-            data = handler(self)
-            if info.mode == 'json':
-                return data['root']
-            else:
-                return data
+        class PokemonList(BaseModel):
+            root: List[Pokemon]
 
-        @classmethod
-        def model_modify_json_schema(cls, json_schema):
-            return json_schema['properties']['root']
+            @root_validator(pre=True)
+            @classmethod
+            def populate_root(cls, values):
+                return {'root': values}
+
+            @model_serializer(mode='wrap')
+            def _serialize(self, handler, info):
+                data = handler(self)
+                if info.mode == 'json':
+                    return data['root']
+                else:
+                    return data
+
+            @classmethod
+            def model_modify_json_schema(cls, json_schema):
+                return json_schema['properties']['root']
 
-        model_config = ConfigDict(from_attributes=True)
+            model_config = ConfigDict(from_attributes=True)
 
     pika = PokemonCls(en_name='Pikachu', jp_name='ピカチュウ')
     bulbi = PokemonCls(en_name='Bulbasaur', jp_name='フシギダネ')
 
     pokemons = deprecated_from_orm(PokemonList, [pika, bulbi])
     assert pokemons.root == [
         Pokemon(en_name='Pikachu', jp_name='ピカチュウ'),
         Pokemon(en_name='Bulbasaur', jp_name='フシギダネ'),
     ]
 
-    class PokemonDict(BaseModel):
-        root: Dict[str, Pokemon]
-        model_config = ConfigDict(from_attributes=True)
-
-        @root_validator(pre=True)
-        @classmethod
-        def populate_root(cls, values):
-            return {'root': values}
-
-        @model_serializer(mode='wrap')
-        def _serialize(self, handler, info):
-            data = handler(self)
-            if info.mode == 'json':
-                return data['root']
-            else:
-                return data
+    with pytest.warns(DeprecationWarning, match='Pydantic V1 style `@root_validator` validators are deprecated.'):
 
-        @classmethod
-        def model_modify_json_schema(cls, json_schema):
-            return json_schema['properties']['root']
+        class PokemonDict(BaseModel):
+            root: Dict[str, Pokemon]
+            model_config = ConfigDict(from_attributes=True)
+
+            @root_validator(pre=True)
+            @classmethod
+            def populate_root(cls, values):
+                return {'root': values}
+
+            @model_serializer(mode='wrap')
+            def _serialize(self, handler, info):
+                data = handler(self)
+                if info.mode == 'json':
+                    return data['root']
+                else:
+                    return data
+
+            @classmethod
+            def model_modify_json_schema(cls, json_schema):
+                return json_schema['properties']['root']
 
     pokemons = deprecated_from_orm(PokemonDict, {'pika': pika, 'bulbi': bulbi})
     assert pokemons.root == {
         'pika': Pokemon(en_name='Pikachu', jp_name='ピカチュウ'),
         'bulbi': Pokemon(en_name='Bulbasaur', jp_name='フシギダネ'),
     }
 
@@ -247,15 +209,15 @@
         x: int
 
     model = deprecated_from_orm(Model, TestCls())
     assert model.x == 1
     assert not hasattr(model, 'y')
 
 
-@pytest.mark.xfail(reason='working on V2')
+@pytest.mark.filterwarnings('ignore:Pydantic V1 style `@root_validator` validators are deprecated.*:DeprecationWarning')
 def test_root_validator():
     validator_value = None
 
     class TestCls:
         x = 1
         y = 2
 
@@ -265,77 +227,20 @@
         y: int
         z: int
 
         @root_validator(pre=True)
         def change_input_data(cls, value):
             nonlocal validator_value
             validator_value = value
-            return {**value, 'z': value['x'] + value['y']}
+            return {'x': value.x, 'y': value.y, 'z': value.x + value.y}
 
     model = deprecated_from_orm(Model, TestCls())
     assert model.model_dump() == {'x': 1, 'y': 2, 'z': 3}
     # assert isinstance(validator_value, GetterDict)
-    assert validator_value == {'x': 1, 'y': 2}
-
-
-@pytest.mark.xfail(reason='working on V2')
-def test_custom_getter_dict():
-    class TestCls:
-        x = 1
-        y = 2
-
-    def custom_getter_dict(obj):
-        assert isinstance(obj, TestCls)
-        return {'x': 42, 'y': 24}
-
-    class Model(BaseModel):
-        x: int
-        y: int
-
-        class Config:
-            from_attributes = True
-            getter_dict = custom_getter_dict
-
-    model = deprecated_from_orm(Model, TestCls())
-    assert model.model_dump() == {'x': 42, 'y': 24}
-
-
-@pytest.mark.xfail(reason='working on V2')
-def test_recursive_parsing():
-    class Getter:  # GetterDict
-        # try to read the modified property name
-        # either as an attribute or as a key
-        def get(self, key, default):
-            key = key + key
-            try:
-                v = self._obj[key]
-                return Getter(v) if isinstance(v, dict) else v
-            except TypeError:
-                return getattr(self._obj, key, default)
-            except KeyError:
-                return default
-
-    class Model(BaseModel):
-        class Config:
-            from_attributes = True
-            getter_dict = Getter
-
-    class ModelA(Model):
-        a: int
-
-    class ModelB(Model):
-        b: ModelA
-
-    # test recursive parsing with object attributes
-    dct = dict(bb=SimpleNamespace(aa=1))
-    assert deprecated_from_orm(ModelB, dct) == ModelB(b=ModelA(a=1))
-
-    # test recursive parsing with dict keys
-    obj = dict(bb=dict(aa=1))
-    assert deprecated_from_orm(ModelB, obj) == ModelB(b=ModelA(a=1))
+    assert isinstance(validator_value, TestCls)
 
 
 def test_nested_orm():
     class User(BaseModel):
         model_config = ConfigDict(from_attributes=True)
         first_name: str
         last_name: str
@@ -378,14 +283,29 @@
             'loc': ('__root__',),
             'msg': 'Expecting value: line 1 column 1 (char 0)',
             'input': 'invalid',
         }
     ]
 
 
+def test_fields():
+    class Model(BaseModel):
+        x: int
+        y: int = 2
+
+    m = Model(x=1)
+    assert len(Model.model_fields) == 2
+    assert len(m.model_fields) == 2
+    match = '^The `__fields__` attribute is deprecated, use `model_fields` instead.$'
+    with pytest.warns(DeprecationWarning, match=match):
+        assert len(Model.__fields__) == 2
+    with pytest.warns(DeprecationWarning, match=match):
+        assert len(m.__fields__) == 2
+
+
 def test_fields_set():
     class Model(BaseModel):
         x: int
         y: int = 2
 
     m = Model(x=1)
     assert m.model_fields_set == {'x'}
@@ -496,33 +416,45 @@
 def test_unique_items_items():
     with pytest.raises(PydanticUserError, match='`unique_items` is removed. use `Set` instead'):
 
         class Model(BaseModel):
             x: List[int] = Field(None, unique_items=True)
 
 
+def test_unique_items_conlist():
+    with pytest.raises(PydanticUserError, match='`unique_items` is removed. use `Set` instead'):
+
+        class Model(BaseModel):
+            x: conlist(int, unique_items=True)
+
+
 def test_allow_mutation():
     m = '`allow_mutation` is deprecated and will be removed. use `frozen` instead'
     with pytest.warns(DeprecationWarning, match=m):
 
         class Model(BaseModel):
             model_config = ConfigDict(validate_assignment=True)
             x: int = Field(allow_mutation=False)
+            y: int = Field(allow_mutation=True)
+
+    m = Model(x=1, y=2)
 
-    m = Model(x=1)
     assert m.x == 1
     with pytest.raises(ValidationError) as exc_info:
         m.x = 2
     assert exc_info.value.errors(include_url=False) == [
         {'input': 2, 'loc': ('x',), 'msg': 'Field is frozen', 'type': 'frozen_field'}
     ]
 
+    m.y = 3
+    assert m.y == 3
+
 
 def test_field_regex():
-    with pytest.raises(PydanticUserError, match='`regex` is removed. use `Pattern` instead'):
+    with pytest.raises(PydanticUserError, match='`regex` is removed. use `pattern` instead'):
 
         class Model(BaseModel):
             x: str = Field('test', regex=r'^test$')
 
 
 def test_field_extra_arguments():
     m = 'Extra keyword arguments on `Field` is deprecated and will be removed. use `json_schema_extra` instead'
@@ -532,14 +464,26 @@
             x: str = Field('test', test='test')
 
     assert Model.model_json_schema(by_alias=True)['properties'] == {
         'x': {'default': 'test', 'test': 'test', 'title': 'X', 'type': 'string'}
     }
 
 
+def test_field_extra_does_not_rewrite_json_schema_extra():
+    m = 'Extra keyword arguments on `Field` is deprecated and will be removed. use `json_schema_extra` instead'
+    with pytest.warns(DeprecationWarning, match=m):
+
+        class Model(BaseModel):
+            x: str = Field('test', test='test', json_schema_extra={'test': 'json_schema_extra value'})
+
+    assert Model.model_json_schema(by_alias=True)['properties'] == {
+        'x': {'default': 'test', 'test': 'json_schema_extra value', 'title': 'X', 'type': 'string'}
+    }
+
+
 class SimpleModel(BaseModel):
     x: int
 
 
 def test_dict():
     m = SimpleModel(x=1)
     with pytest.warns(DeprecationWarning, match=r'^The `dict` method is deprecated; use `model_dump` instead\.$'):
```

### Comparing `pydantic-2.0a4/tests/test_deprecated_validate_arguments.py` & `pydantic-2.0b1/tests/test_deprecated_validate_arguments.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a4/tests/test_discriminated_union.py` & `pydantic-2.0b1/tests/test_discriminated_union.py`

 * *Files 1% similar despite different names*

```diff
@@ -302,17 +302,15 @@
         literal: Literal['b'] = Field(alias='lit')
 
     class Top(BaseModel):
         sub: Union[A, B] = Field(..., discriminator='literal')
 
     with pytest.raises(ValidationError) as exc_info:
         Top(sub=A(literal='a'))
-    # TODO: Adding this note here that we should make sure the produced error messages for DiscriminatedUnion
-    #   have the same behavior as elsewhere when aliases are involved.
-    #   (I.e., possibly using the alias value as the 'loc')
+
     assert exc_info.value.errors(include_url=False) == [
         {'input': {'literal': 'a'}, 'loc': ('lit',), 'msg': 'Field required', 'type': 'missing'}
     ]
     assert Top(sub=A(lit='a')).sub.literal == 'a'
     assert Top(sub=B(lit='b')).sub.literal == 'b'
     assert Top(sub=B(literal='b')).sub.literal == 'b'
 
@@ -360,17 +358,15 @@
 ]
 if sys.version_info >= (3, 11):
     from enum import StrEnum
 
     ENUM_TEST_CASES.append((StrEnum, {'a': 'v_a', 'b': 'v_b'}))
 
 
-@pytest.mark.xfail(
-    sys.version_info[:2] == (3, 8), reason='https://github.com/python/cpython/issues/103592', strict=False
-)
+@pytest.mark.skipif(sys.version_info[:2] == (3, 8), reason='https://github.com/python/cpython/issues/103592')
 @pytest.mark.parametrize('base_class,choices', ENUM_TEST_CASES)
 def test_discriminated_union_enum(base_class, choices):
     EnumValue = base_class('EnumValue', choices)
 
     class A(BaseModel):
         m: Literal[EnumValue.a]
```

### Comparing `pydantic-2.0a4/tests/test_docs.py` & `pydantic-2.0b1/tests/test_docs.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,49 +88,49 @@
 
     if example.path.name == 'devtools.md':
         pytest.skip('tested below')
 
     eval_example.print_callback = print_callback
 
     prefix_settings = example.prefix_settings()
-    test_settings = prefix_settings.get('test')
-    lint_settings = prefix_settings.get('lint')
-    if test_settings == 'skip' and lint_settings == 'skip':
-        pytest.skip('both test and lint skipped')
+    test_settings = prefix_settings.get('test', '')
+    lint_settings = prefix_settings.get('lint', '')
+    if test_settings.startswith('skip') and lint_settings.startswith('skip'):
+        pytest.skip('both running code and lint skipped')
 
     requires_settings = prefix_settings.get('requires')
     if requires_settings:
         major, minor = map(int, requires_settings.split('.'))
         if sys.version_info < (major, minor):
             pytest.skip(f'requires python {requires_settings}')
 
     group_name = prefix_settings.get('group')
 
     if '# ignore-above' in example.source:
         eval_example.set_config(ruff_ignore=['E402'])
     if group_name:
         eval_example.set_config(ruff_ignore=['F821'])
 
-    if lint_settings != 'skip':
+    if not lint_settings.startswith('skip'):
         if eval_example.update_examples:
             eval_example.format(example)
         else:
             eval_example.lint(example)
 
-    if test_settings == 'skip':
-        return
+    if test_settings.startswith('skip'):
+        pytest.skip(test_settings[4:].lstrip(' -') or 'running code skipped')
 
     group_name = prefix_settings.get('group')
     d = group_globals.get(group_name)
 
     mocker.patch('datetime.datetime', MockedDatetime)
     mocker.patch('random.randint', return_value=3)
 
     xfail = None
-    if test_settings and test_settings.startswith('xfail'):
+    if test_settings.startswith('xfail'):
         xfail = test_settings[5:].lstrip(' -')
 
     rewrite_assertions = prefix_settings.get('rewrite_assert', 'true') == 'true'
 
     try:
         if test_settings == 'no-print-intercept':
             d2 = eval_example.run(example, module_globals=d, rewrite_assertions=rewrite_assertions)
```

### Comparing `pydantic-2.0a4/tests/test_edge_cases.py` & `pydantic-2.0b1/tests/test_edge_cases.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,41 +19,41 @@
     Type,
     TypeVar,
     Union,
 )
 
 import pytest
 from dirty_equals import HasRepr, IsStr
-from pydantic_core import PydanticSerializationError, core_schema
+from pydantic_core import ErrorDetails, InitErrorDetails, PydanticSerializationError, core_schema
 from typing_extensions import Annotated, get_args
 
 from pydantic import (
     BaseModel,
     ConfigDict,
     PydanticInvalidForJsonSchema,
     PydanticSchemaGenerationError,
     TypeAdapter,
     ValidationError,
     constr,
     errors,
-)
-from pydantic.decorators import (
-    field_serializer,
     field_validator,
-    model_serializer,
     model_validator,
     root_validator,
     validator,
 )
 from pydantic.fields import Field, computed_field
+from pydantic.functional_serializers import (
+    field_serializer,
+    model_serializer,
+)
 
 
 def test_str_bytes():
     class Model(BaseModel):
-        v: Union[str, bytes] = ...
+        v: Union[str, bytes]
 
     m = Model(v='s')
     assert m.v == 's'
     assert repr(m.model_fields['v']) == 'FieldInfo(annotation=Union[str, bytes], required=True)'
 
     m = Model(v=b'b')
     assert m.v == b'b'
@@ -595,15 +595,14 @@
     assert m.model_dump(include=['a']) == {'a': 1}
     assert m.model_dump(exclude=['a']) == {'b': 2, 'c': 3, 'd': 4, 'e': 5, 'f': 7}
 
     assert m.model_dump(include=['a'], exclude_unset=True) == {'a': 1}
     assert m.model_dump(exclude=['a'], exclude_unset=True) == {'b': 2, 'e': 5, 'f': 7}
 
 
-@pytest.mark.xfail(reason='pydantic-core include/exclude does not wrap negative ints')
 def test_advanced_exclude():
     class SubSubModel(BaseModel):
         a: str
         b: str
 
     class SubModel(BaseModel):
         c: str
@@ -618,15 +617,14 @@
     assert m.model_dump(exclude={'f': {'c': ..., 'd': {-1: {'a'}}}}) == {
         'e': 'e',
         'f': {'d': [{'a': 'a', 'b': 'b'}, {'b': 'e'}]},
     }
     assert m.model_dump(exclude={'e': ..., 'f': {'d'}}) == {'f': {'c': 'foo'}}
 
 
-@pytest.mark.xfail(reason='pydantic-core include/exclude does not wrap negative ints')
 def test_advanced_exclude_by_alias():
     class SubSubModel(BaseModel):
         a: str
         aliased_b: str = Field(..., alias='b_alias')
 
     class SubModel(BaseModel):
         aliased_c: str = Field(..., alias='c_alias')
@@ -647,15 +645,14 @@
         'f_alias': {'d_alias': [{'a': 'a', 'b_alias': 'b'}, {'b_alias': 'e'}]},
     }
 
     excludes = {'aliased_e': ..., 'aliased_f': {'aliased_d'}}
     assert m.model_dump(exclude=excludes, by_alias=True) == {'f_alias': {'c_alias': 'foo'}}
 
 
-@pytest.mark.xfail(reason='pydantic-core include/exclude does not wrap negative ints')
 def test_advanced_value_include():
     class SubSubModel(BaseModel):
         a: str
         b: str
 
     class SubModel(BaseModel):
         c: str
@@ -668,15 +665,14 @@
     m = Model(e='e', f=SubModel(c='foo', d=[SubSubModel(a='a', b='b'), SubSubModel(a='c', b='e')]))
 
     assert m.model_dump(include={'f'}) == {'f': {'c': 'foo', 'd': [{'a': 'a', 'b': 'b'}, {'a': 'c', 'b': 'e'}]}}
     assert m.model_dump(include={'e'}) == {'e': 'e'}
     assert m.model_dump(include={'f': {'d': {0: ..., -1: {'b'}}}}) == {'f': {'d': [{'a': 'a', 'b': 'b'}, {'b': 'e'}]}}
 
 
-@pytest.mark.xfail(reason='pydantic-core include/exclude does not wrap negative ints')
 def test_advanced_value_exclude_include():
     class SubSubModel(BaseModel):
         a: str
         b: str
 
     class SubModel(BaseModel):
         c: str
@@ -1177,32 +1173,14 @@
     with pytest.raises(ValidationError) as exc_info:
         Model()
     assert exc_info.value.errors(include_url=False) == [
         {'input': {}, 'loc': ('bar',), 'msg': 'Field required', 'type': 'missing'}
     ]
 
 
-@pytest.mark.xfail(reason='items yielded by __get_validators__ are not inspected for valid signatures')
-def test_invalid_validator():
-    class InvalidValidator:
-        @classmethod
-        def __get_validators__(cls):
-            yield cls.has_wrong_arguments
-
-        @classmethod
-        def has_wrong_arguments(cls, value, bar):
-            pass
-
-    with pytest.raises(errors.PydanticUserError, match='Invalid signature for validator'):
-
-        class InvalidValidatorModel(BaseModel):
-            model_config = dict(arbitrary_types_allowed=True)
-            x: InvalidValidator = ...
-
-
 def test_unable_to_infer():
     with pytest.raises(
         errors.PydanticUserError,
         match=re.escape(
             "A non-annotated attribute was detected: `x = None`. All model fields require a type annotation; "
             "if `x` is not meant to be a field, you may be able to resolve this error by annotating it as a "
             "`ClassVar` or updating `model_config['ignored_types']`"
@@ -1233,15 +1211,15 @@
             'msg': 'Input should be a valid number, unable to parse string as an number',
             'input': 'foobar',
         },
         {
             'type': 'decimal_parsing',
             'loc': (
                 'a',
-                'lax-or-strict[lax=function-after[validate(), union[is-instance[Decimal],int,float,constrained-str]],strict=custom-error[function-after[validate(), is-instance[Decimal]]]]',  # noqa: E501
+                'lax-or-strict[lax=function-after[validate(), union[json-or-python[json=function-after[Decimal(), union[int,float,constrained-str]],python=is-instance[Decimal]],int,float,constrained-str]],strict=custom-error[function-after[validate(), json-or-python[json=function-after[Decimal(), union[int,float,constrained-str]],python=is-instance[Decimal]]]]]',  # noqa: E501
             ),
             'msg': 'Input should be a valid decimal',
             'input': 'foobar',
         },
     ]
 
     assert Model(a=1.5).a == 1.5
@@ -1893,15 +1871,14 @@
         'optional3': None,
         'nullable1': 1,
         'nullable2': 'two',
         'nullable3': 'three',
     }
 
 
-@pytest.mark.xfail(reason='need to modify loc of ValidationError')
 def test_custom_generic_validators():
     T1 = TypeVar('T1')
     T2 = TypeVar('T2')
 
     class MyGen(Generic[T1, T2]):
         def __init__(self, t1: T1, t2: T2):
             self.t1 = t1
@@ -1917,20 +1894,35 @@
             args = get_args(source)
             if not args:
                 return schema
 
             t1_f = TypeAdapter(args[0]).validate_python
             t2_f = TypeAdapter(args[1]).validate_python
 
-            def validate(v, info):
+            def convert_to_init_error(e: ErrorDetails, loc: str) -> InitErrorDetails:
+                init_e = {'type': e['type'], 'loc': e['loc'] + (loc,), 'input': e['input']}
+                if 'ctx' in e:
+                    init_e['ctx'] = e['ctx']
+                return init_e
+
+            def validate(v, _info):
                 if not args:
                     return v
-                # TODO: Collect these errors, rather than stopping early, and modify the loc to make the test pass
-                t1_f(v.t1)
-                t2_f(v.t2)
+                try:
+                    v.t1 = t1_f(v.t1)
+                except ValidationError as exc:
+                    raise ValidationError.from_exception_data(
+                        exc.title, [convert_to_init_error(e, 't1') for e in exc.errors()]
+                    ) from exc
+                try:
+                    v.t2 = t2_f(v.t2)
+                except ValidationError as exc:
+                    raise ValidationError.from_exception_data(
+                        exc.title, [convert_to_init_error(e, 't2') for e in exc.errors()]
+                    ) from exc
                 return v
 
             return core_schema.general_after_validator_function(validate, schema)
 
     class Model(BaseModel):
         a: str
         gen: MyGen[str, bool]
@@ -2022,15 +2014,15 @@
     class MyGen(Generic[T1, T2]):
         def __init__(self, t1: T1, t2: T2):
             self.t1 = t1
             self.t2 = t2
 
     match = (
         r'Unable to generate pydantic-core schema for (.*)MyGen\[str, bool\](.*). '
-        r'Setting `arbitrary_types_allowed=True` in the model_config may prevent this error.'
+        r'Set `arbitrary_types_allowed=True` in the model_config to ignore this error'
     )
     with pytest.raises(TypeError, match=match):
 
         class Model(BaseModel):
             a: str
             gen: MyGen[str, bool]
 
@@ -2254,59 +2246,38 @@
 
     class Custom:
         __fields__ = True
 
     assert not issubclass(Custom, BaseModel)
 
 
-@pytest.mark.xfail(reason='"long int", see details below')
 def test_long_int():
     """
     see https://github.com/pydantic/pydantic/issues/1477 and in turn, https://github.com/python/cpython/issues/95778
     """
 
     class Model(BaseModel):
         x: int
 
-    # TODO: The next line now raises the following error:
-    #     E       pydantic_core._pydantic_core.ValidationError: 1 validation error for Model
-    #     E       x
-    #     E         Input should be a finite number [type=finite_number,
-    #     input_value='111111111111111111111111...11111111111111111111111', input_type=str]
-    #   Do we need to resolve this? How hard would that be in pydantic_core? Is it worth it?
-    #   -
-    #   "in pydantic-core we use an i64, which constrains the max and min values. Since that's massively more
-    #   performant, and there are very few real world uses for int > i64:MAX, the error is correct."
-    #   https://github.com/pydantic/pydantic/pull/5151#discussion_r1130693762
-    #   -
-    #   I think before modifying this test and removing the xfail, we should create a new test
-    #   that handles the following line without failure using the is-instance approach described in the comment
-    #   linked above.
     assert Model(x='1' * 4_300).x == int('1' * 4_300)
-    assert Model(x=b'1' * 4_300).x == int('1' * 4_300)
-    assert Model(x=bytearray(b'1' * 4_300)).x == int('1' * 4_300)
 
     too_long = '1' * 4_301
     with pytest.raises(ValidationError) as exc_info:
         Model(x=too_long)
 
+    # insert_assert(exc_info.value.errors(include_url=False))
     assert exc_info.value.errors(include_url=False) == [
         {
+            'type': 'int_parsing_size',
             'loc': ('x',),
-            'msg': 'value is not a valid integer',
-            'type': 'type_error.integer',
-        },
+            'msg': 'Unable to parse input string as an integer, exceeded maximum size',
+            'input': too_long,
+        }
     ]
 
-    too_long_b = too_long.encode('utf-8')
-    with pytest.raises(ValidationError):
-        Model(x=too_long_b)
-    with pytest.raises(ValidationError):
-        Model(x=bytearray(too_long_b))
-
     # this used to hang indefinitely
     with pytest.raises(ValidationError):
         Model(x='1' * (10**7))
 
 
 def test_parent_field_with_default():
     class Parent(BaseModel):
@@ -2342,19 +2313,21 @@
 
         @model_validator(mode='wrap')
         @classmethod
         @abstractmethod
         def my_model_validator(cls, values, handler, info):
             raise NotImplementedError
 
-        @root_validator(skip_on_failure=True)
-        @classmethod
-        @abstractmethod
-        def my_root_validator(cls, values):
-            raise NotImplementedError
+        with pytest.warns(DeprecationWarning):
+
+            @root_validator(skip_on_failure=True)
+            @classmethod
+            @abstractmethod
+            def my_root_validator(cls, values):
+                raise NotImplementedError
 
         with pytest.warns(DeprecationWarning):
 
             @validator('side')
             @classmethod
             @abstractmethod
             def my_validator(cls, value, **kwargs):
@@ -2369,15 +2342,15 @@
         @abstractmethod
         def my_serializer(self, v, _info):
             raise NotImplementedError
 
         @computed_field
         @property
         @abstractmethod
-        def my_computed_field(self):
+        def my_computed_field(self) -> Any:
             raise NotImplementedError
 
     class Square(AbstractSquare):
         pass
 
     with pytest.raises(
         TypeError,
@@ -2396,16 +2369,14 @@
 
 
 @pytest.mark.skipif(sys.version_info < (3, 9), reason='cannot use list.__class_getitem__ before 3.9')
 def test_generic_wrapped_forwardref():
     class Operation(BaseModel):
         callbacks: list['PathItem']
 
-        model_config = {'undefined_types_warning': False}
-
     class PathItem(BaseModel):
         pass
 
     Operation.model_rebuild()
 
     Operation.model_validate({'callbacks': [PathItem()]})
     with pytest.raises(ValidationError) as exc_info:
@@ -2444,37 +2415,34 @@
         kwargs = {
             'match': r'Forward references must evaluate to types\.'
             r' Got FieldInfo\(annotation=NoneType, required=False\)\.'
         }
     with pytest.raises(error, **kwargs):
 
         class M(BaseModel):
-            model_config = {'undefined_types_warning': False}
             B: ForwardRef('B') = Field(default=None)
 
     # The solution:
     class A(BaseModel):
-        model_config = {'undefined_types_warning': False}
-
         B: ForwardRef('__types["B"]') = Field()  # F821
 
     assert A.model_fields['B'].annotation == ForwardRef('__types["B"]')  # F821
     A.model_rebuild(raise_errors=False)
     assert A.model_fields['B'].annotation == ForwardRef('__types["B"]')  # F821
 
     class B(BaseModel):
         pass
 
     class C(BaseModel):
         pass
 
-    assert not A.__pydantic_model_complete__
+    assert not A.__pydantic_complete__
     types = {'B': B}
     A.model_rebuild(_types_namespace={'__types': types})
-    assert A.__pydantic_model_complete__
+    assert A.__pydantic_complete__
 
     assert A(B=B()).B == B()
     with pytest.raises(ValidationError) as exc_info:
         A(B=C())
     assert exc_info.value.errors(include_url=False) == [
         {'input': C(), 'loc': ('B',), 'msg': 'Input should be a valid dictionary', 'type': 'dict_type'}
     ]
```

### Comparing `pydantic-2.0a4/tests/test_fastapi_json_schema.py` & `pydantic-2.0b1/tests/test_fastapi_json_schema.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a4/tests/test_forward_ref.py` & `pydantic-2.0b1/tests/test_forward_ref.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,54 +38,52 @@
 
 
 def test_forward_ref_auto_update_no_model(create_module):
     @create_module
     def module():
         from typing import Optional
 
-        from pydantic import BaseModel
+        import pytest
+
+        from pydantic import BaseModel, PydanticUserError
 
-        class Foo(BaseModel, undefined_types_warning=False):
+        class Foo(BaseModel):
             a: Optional['Bar'] = None
 
+        with pytest.raises(PydanticUserError, match='`Foo` is not fully defined; you should define `Bar`,'):
+            Foo(a={'b': {'a': {}}})
+
         class Bar(BaseModel):
             b: 'Foo'
 
-    assert module.Foo.__pydantic_model_complete__ is False
-    assert module.Bar.__pydantic_model_complete__ is True
+    assert module.Bar.__pydantic_complete__ is True
     assert repr(module.Bar.model_fields['b']) == 'FieldInfo(annotation=Foo, required=True)'
 
     # Bar should be complete and ready to use
     b = module.Bar(b={'a': {'b': {}}})
     assert b.model_dump() == {'b': {'a': {'b': {'a': None}}}}
 
     # model_fields is complete on Foo
     assert repr(module.Foo.model_fields['a']) == (
         "FieldInfo(annotation=Union[ForwardRef('Bar'), NoneType], required=False)"
     )
 
-    # but Foo is not ready to use
-    with pytest.raises(PydanticUserError, match='`Foo` is not fully defined; you should define `Bar`,'):
-        module.Foo(a={'b': {'a': {}}})
-
-    assert module.Foo.model_rebuild() is True
-    assert module.Foo.__pydantic_model_complete__ is True
-
-    # now Foo is ready to use
+    assert module.Foo.__pydantic_complete__ is False
+    # Foo gets auto-rebuilt during the first attempt at validation
     f = module.Foo(a={'b': {'a': {'b': {'a': None}}}})
+    assert module.Foo.__pydantic_complete__ is True
     assert f.model_dump() == {'a': {'b': {'a': {'b': {'a': None}}}}}
 
 
 def test_forward_ref_one_of_fields_not_defined(create_module):
     @create_module
     def module():
-        from pydantic import BaseModel, ConfigDict
+        from pydantic import BaseModel
 
         class Foo(BaseModel):
-            model_config = ConfigDict(undefined_types_warning=False)
             foo: 'Foo'
             bar: 'Bar'
 
     assert {k: repr(v) for k, v in module.Foo.model_fields.items()} == {
         'foo': 'FieldInfo(annotation=Foo, required=True)',
         'bar': "FieldInfo(annotation=ForwardRef('Bar'), required=True)",
     }
@@ -330,16 +328,14 @@
         from typing import List
 
         from pydantic import BaseModel
 
         class Owner(BaseModel):
             account: 'Account'
 
-            model_config = dict(undefined_types_warning=False)
-
         class Account(BaseModel):
             name: str
             owner: 'Owner'
             subaccounts: List['Account'] = []
 
     Account = module.Account
     assert Account.model_json_schema() == {
@@ -377,16 +373,14 @@
 from __future__ import annotations
 from typing import List
 from pydantic import BaseModel
 
 class Owner(BaseModel):
   account: Account
 
-  model_config=dict(undefined_types_warning=False)
-
 class Account(BaseModel):
   name: str
   owner: Owner
   subaccounts: List[Account] = []
 
     """
     )
@@ -421,21 +415,20 @@
 
 def test_forward_ref_with_field(create_module):
     @create_module
     def module():
         from typing import ForwardRef, List
 
         import pytest
-        from pydantic_core import SchemaError
 
         from pydantic import BaseModel, Field
 
         Foo = ForwardRef('Foo')
 
-        with pytest.raises(SchemaError, match=r'Extra inputs are not permitted \[type=extra_forbidden,'):
+        with pytest.raises(TypeError, match=r'The following constraints cannot be applied.*\'gt\''):
 
             class Foo(BaseModel):
                 c: List[Foo] = Field(..., gt=0)
 
 
 def test_forward_ref_optional(create_module):
     module = create_module(
@@ -449,16 +442,14 @@
 class Spec(BaseModel):
     spec_fields: List[str] = Field(..., alias="fields")
     filter: Optional[str] = None
     sort: Optional[str]
 
 
 class PSpec(Spec):
-    model_config = ConfigDict(undefined_types_warning = False)
-    # FIXME investigate why this wasn't causing errors before
     g: Optional[GSpec] = None
 
 
 class GSpec(Spec):
     p: Optional[PSpec]
 
 # PSpec.model_rebuild()
@@ -524,33 +515,31 @@
         from typing_extensions import Literal
 
         from pydantic import BaseModel, Field
 
         class Pet(BaseModel):
             pet: Union['Cat', 'Dog'] = Field(discriminator='type')
 
-            model_config = dict(undefined_types_warning=False)
-
         class Cat(BaseModel):
             type: Literal['cat']
 
         class Dog(BaseModel):
             type: Literal['dog']
 
-    with pytest.raises(PydanticUserError, match='`Pet` is not fully defined; you should define `Cat`'):
-        module.Pet.model_validate({'pet': {'type': 'pika'}})
-
-    module.Pet.model_rebuild()
+    assert module.Pet.__pydantic_complete__ is False
 
     with pytest.raises(
         ValidationError,
         match="Input tag 'pika' found using 'type' does not match any of the expected tags: 'cat', 'dog'",
     ):
         module.Pet.model_validate({'pet': {'type': 'pika'}})
 
+    # Ensure the rebuild has happened automatically despite validation failure
+    assert module.Pet.__pydantic_complete__ is True
+
     assert module.Pet.model_json_schema() == {
         'title': 'Pet',
         'required': ['pet'],
         'type': 'object',
         'properties': {
             'pet': {
                 'title': 'Pet',
@@ -587,68 +576,69 @@
     a: ClassVar[int]
 """
     )
 
     assert module.Model.__class_vars__ == {'a'}
 
 
-@pytest.mark.xfail(reason='json encoder stuff')
 def test_json_encoder_str(create_module):
     module = create_module(
         # language=Python
         """
-from pydantic import BaseModel, ConfigDict
+from pydantic import BaseModel, ConfigDict, field_serializer
 
 
 class User(BaseModel):
     x: str
 
 
 FooUser = User
 
 
 class User(BaseModel):
     y: str
 
 
 class Model(BaseModel):
-    model_config=ConfigDict(json_encoders={'User': lambda v: f'User({v.y})'})
     foo_user: FooUser
     user: User
 
+    @field_serializer('user')
+    def serialize_user(self, v):
+        return f'User({v.y})'
+
 """
     )
 
     m = module.Model(foo_user={'x': 'user1'}, user={'y': 'user2'})
     # TODO: How can we replicate this custom-encoder functionality without affecting the serialization of `User`?
-    assert m.model_dump_json(models_as_dict=False) == '{"foo_user": {"x": "user1"}, "user": "User(user2)"}'
+    assert m.model_dump_json() == '{"foo_user":{"x":"user1"},"user":"User(user2)"}'
 
 
-@pytest.mark.xfail(reason='json encoder stuff')
 def test_json_encoder_forward_ref(create_module):
     # TODO: Replace the use of json_encoders with a root_serializer
     module = create_module(
         # language=Python
         """
-from pydantic import BaseModel, ConfigDict
-from typing import ForwardRef, List, Optional
+from typing import List, Optional
+from typing_extensions import Annotated
+from pydantic import BaseModel, PlainSerializer
+
+def serialize_user(user):
+    return f'User({user.name})'
 
 class User(BaseModel):
     name: str
-    friends: Optional[List['User']] = None
+    friends: Optional[List[Annotated['User', PlainSerializer(serialize_user)]]] = None
 
-    model_config = ConfigDict(
-        json_encoders = {
-            ForwardRef('User'): lambda v: f'User({v.name})',
-        })
 """
     )
 
     m = module.User(name='anne', friends=[{'name': 'ben'}, {'name': 'charlie'}])
-    assert m.model_dump_json(models_as_dict=False) == '{"name": "anne", "friends": ["User(ben)", "User(charlie)"]}'
+    assert m.model_dump_json() == '{"name":"anne","friends":["User(ben)","User(charlie)"]}'
 
 
 skip_pep585 = pytest.mark.skipif(
     sys.version_info < (3, 9), reason='PEP585 generics only supported for python 3.9 and above'
 )
 
 
@@ -678,21 +668,19 @@
 
 @skip_pep585
 def test_pep585_recursive_generics(create_module):
     @create_module
     def module():
         from typing import ForwardRef
 
-        from pydantic import BaseModel, ConfigDict
+        from pydantic import BaseModel
 
         HeroRef = ForwardRef('Hero')
 
         class Team(BaseModel):
-            model_config = ConfigDict(undefined_types_warning=False)
-
             name: str
             heroes: list[HeroRef]
 
         class Hero(BaseModel):
             name: str
             teams: list[Team]
 
@@ -741,26 +729,25 @@
     assert f.y.model_fields_set == {'x'}
 
 
 def test_force_rebuild():
     class Foobar(BaseModel):
         b: int
 
-    assert Foobar.__pydantic_model_complete__ is True
+    assert Foobar.__pydantic_complete__ is True
     assert Foobar.model_rebuild() is None
     assert Foobar.model_rebuild(force=True) is True
 
 
 def test_rebuild_subclass_of_built_model():
     class Model(BaseModel):
         x: int
 
     class FutureReferencingModel(Model):
         y: 'FutureModel'
-        model_config = dict(undefined_types_warning=False)
 
     class FutureModel(BaseModel):
         pass
 
     FutureReferencingModel.model_rebuild()
 
     assert FutureReferencingModel(x=1, y=FutureModel()).model_dump() == {'x': 1, 'y': {}}
@@ -781,39 +768,38 @@
         b: Foo
 
     return Bar
 """
     )
 
     bar_model = module.nested()
-    assert bar_model.__pydantic_model_complete__ is True
+    assert bar_model.__pydantic_complete__ is True
     assert bar_model(b={'a': 1}).model_dump() == {'b': {'a': 1}}
 
 
 def test_nested_more_annotation(create_module):
     @create_module
     def module():
-        from pydantic import BaseModel, ConfigDict
+        from pydantic import BaseModel
 
         def nested():
             class Foo(BaseModel):
                 a: int
 
             def more_nested():
                 class Bar(BaseModel):
-                    model_config = ConfigDict(undefined_types_warning=False)
                     b: 'Foo'
 
                 return Bar
 
             return more_nested()
 
     bar_model = module.nested()
     # this does not work because Foo is in a parent scope
-    assert bar_model.__pydantic_model_complete__ is False
+    assert bar_model.__pydantic_complete__ is False
 
 
 def test_nested_annotation_priority(create_module):
     @create_module
     def module():
         from annotated_types import Gt
         from typing_extensions import Annotated
@@ -836,140 +822,138 @@
     with pytest.raises(ValidationError, match=r'Input should be greater than 10 \[type=greater_than,'):
         bar_model(b=1)
 
 
 def test_nested_model_rebuild(create_module):
     @create_module
     def module():
-        from pydantic import BaseModel, ConfigDict
+        from pydantic import BaseModel
 
         def nested():
             class Bar(BaseModel):
-                model_config = ConfigDict(undefined_types_warning=False)
                 b: 'Foo'
 
             class Foo(BaseModel):
                 a: int
 
-            assert Bar.__pydantic_model_complete__ is False
+            assert Bar.__pydantic_complete__ is False
             Bar.model_rebuild()
             return Bar
 
     bar_model = module.nested()
-    assert bar_model.__pydantic_model_complete__ is True
+    assert bar_model.__pydantic_complete__ is True
     assert bar_model(b={'a': 1}).model_dump() == {'b': {'a': 1}}
 
 
-def pytest_raises_undefined_types_warning(defining_class_name, missing_type_name):
-    """Returns a pytest.raises context manager that checks for the correct undefined types warning message.
-    usage: `with pytest_raises_undefined_types_warning(class_name='Foobar', missing_class_name='UndefinedType'):`
+def pytest_raises_user_error_for_undefined_type(defining_class_name, missing_type_name):
+    """
+    Returns a `pytest.raises` context manager that checks the error message when an undefined type is present.
+
+    usage: `with pytest_raises_user_error_for_undefined_type(class_name='Foobar', missing_class_name='UndefinedType'):`
     """
 
     return pytest.raises(
-        UserWarning,
+        PydanticUserError,
         match=re.escape(
-            f'`{defining_class_name}` has an undefined annotation: `{missing_type_name}`. '
-            'It may be possible to resolve this by setting undefined_types_warning=False '
-            f'in the config for `{defining_class_name}`.'
+            f'`{defining_class_name}` is not fully defined; you should define `{missing_type_name}`, then call'
+            f' `{defining_class_name}.model_rebuild()` before the first `{defining_class_name}` instance is created.'
         ),
     )
 
 
 #   NOTE: the `undefined_types_warning` tests below are "statically parameterized" (i.e. have Duplicate Code).
-#   The initial attempt to refactor them into a single parameterized test was not strateforward, due to the use of the
-#   `create_module` fixture and the need for `from __future__ import annotations` be the first line in a module.
+#   The initial attempt to refactor them into a single parameterized test was not straightforward due to the use of the
+#   `create_module` fixture and the requirement that `from __future__ import annotations` be the first line in a module.
 #
 #   Test Parameters:
 #     1. config setting: (1a) default behavior vs (1b) overriding with Config setting:
 #     2. type checking approach: (2a) `from __future__ import annotations` vs (2b) `ForwardRef`
 #
 #   The parameter tags "1a", "1b", "2a", and "2b" are used in the test names below, to indicate which combination
 #   of conditions the test is covering.
 
 
 def test_undefined_types_warning_1a_raised_by_default_2a_future_annotations(create_module):
-    with pytest_raises_undefined_types_warning(defining_class_name='Foobar', missing_type_name='UndefinedType'):
+    with pytest_raises_user_error_for_undefined_type(defining_class_name='Foobar', missing_type_name='UndefinedType'):
         create_module(
             # language=Python
             """
 from __future__ import annotations
 from pydantic import BaseModel
 
 class Foobar(BaseModel):
     a: UndefinedType
+
+# Trigger the error for an undefined type:
+Foobar(a=1)
 """
         )
 
 
 def test_undefined_types_warning_1a_raised_by_default_2b_forward_ref(create_module):
-    with pytest_raises_undefined_types_warning(defining_class_name='Foobar', missing_type_name='UndefinedType'):
+    with pytest_raises_user_error_for_undefined_type(defining_class_name='Foobar', missing_type_name='UndefinedType'):
 
         @create_module
         def module():
             from typing import ForwardRef
 
             from pydantic import BaseModel
 
             UndefinedType = ForwardRef('UndefinedType')
 
             class Foobar(BaseModel):
                 a: UndefinedType
 
+            # Trigger the error for an undefined type
+            Foobar(a=1)
+
 
 def test_undefined_types_warning_1b_suppressed_via_config_2a_future_annotations(create_module):
     module = create_module(
         # language=Python
         """
 from __future__ import annotations
 from pydantic import BaseModel
 
-# Suppress the undefined_types_warning
-class Foobar(BaseModel, undefined_types_warning=False):
+# Because we don't instantiate the type, no error for an undefined type is raised
+class Foobar(BaseModel):
     a: UndefinedType
 """
     )
-    # Since we're testing the absence of a warning, it's important to confirm pydantic was actually run.
-    # The presence of the `__pydantic_model_complete__` is a good indicator of this.
-    assert module.Foobar.__pydantic_model_complete__ is False
+    # Since we're testing the absence of an error, it's important to confirm pydantic was actually run.
+    # The presence of the `__pydantic_complete__` is a good indicator of this.
+    assert module.Foobar.__pydantic_complete__ is False
 
 
 def test_undefined_types_warning_1b_suppressed_via_config_2b_forward_ref(create_module):
     @create_module
     def module():
         from typing import ForwardRef
 
         from pydantic import BaseModel
 
         UndefinedType = ForwardRef('UndefinedType')
 
-        # Suppress the undefined_types_warning
-        class Foobar(BaseModel, undefined_types_warning=False):
+        # Because we don't instantiate the type, no error for an undefined type is raised
+        class Foobar(BaseModel):
             a: UndefinedType
 
     # Since we're testing the absence of a warning, it's important to confirm pydantic was actually run.
-    # The presence of the `__pydantic_model_complete__` is a good indicator of this.
-    assert module.Foobar.__pydantic_model_complete__ is False
+    # The presence of the `__pydantic_complete__` is a good indicator of this.
+    assert module.Foobar.__pydantic_complete__ is False
 
 
 def test_undefined_types_warning_raised_by_usage(create_module):
-    with pytest.raises(
-        PydanticUserError,
-        match=re.escape(
-            '`Foobar` is not fully defined; you should define `UndefinedType`, '
-            'then call `Foobar.model_rebuild()` before the first `Foobar` instance is created.',
-        ),
-    ):
+    with pytest_raises_user_error_for_undefined_type('Foobar', 'UndefinedType'):
 
         @create_module
         def module():
             from typing import ForwardRef
 
             from pydantic import BaseModel
 
             UndefinedType = ForwardRef('UndefinedType')
 
             class Foobar(BaseModel):
                 a: UndefinedType
 
-                model_config = {'undefined_types_warning': False}
-
             Foobar(a=1)
```

### Comparing `pydantic-2.0a4/tests/test_generics.py` & `pydantic-2.0b1/tests/test_generics.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,41 +25,42 @@
     Tuple,
     Type,
     TypeVar,
     Union,
 )
 
 import pytest
-from dirty_equals import HasRepr
-from pydantic_core import core_schema
-from typing_extensions import Annotated, Literal, OrderedDict, TypeVarTuple, Unpack
+from dirty_equals import HasRepr, IsStr
+from pydantic_core import CoreSchema, core_schema
+from typing_extensions import Annotated, Literal, OrderedDict, TypeVarTuple, Unpack, get_args
 
 from pydantic import (
     BaseModel,
     Field,
+    GetCoreSchemaHandler,
     Json,
     PositiveInt,
     PydanticSchemaGenerationError,
     PydanticUserError,
     ValidationError,
     ValidationInfo,
     computed_field,
-    root_validator,
+    field_validator,
+    model_validator,
 )
 from pydantic._internal._core_utils import collect_invalid_schemas
 from pydantic._internal._generics import (
     _GENERIC_TYPES_CACHE,
     _LIMITED_DICT_SIZE,
     LimitedDict,
     generic_recursion_self_type,
     iter_contained_typevars,
     recursively_defined_type_refs,
     replace_types,
 )
-from pydantic.decorators import field_validator
 
 
 @pytest.fixture()
 def clean_cache():
     # cleans up _GENERIC_TYPES_CACHE for checking item counts in the cache
     _GENERIC_TYPES_CACHE.clear()
     gc.collect(0)
@@ -100,21 +101,21 @@
         @field_validator('data')
         @classmethod
         def validate_value_nonzero(cls, v: Any):
             if any(x == 0 for x in v.values()):
                 raise ValueError('some value is zero')
             return v
 
-        @root_validator(skip_on_failure=True)
+        @model_validator(mode='after')
         @classmethod
-        def validate_sum(cls, values: Dict[str, Any]) -> Dict[str, Any]:
-            data = values.get('data', {})
+        def validate_sum(cls, m):
+            data = m.data
             if sum(data.values()) > 5:
                 raise ValueError('sum too large')
-            return values
+            return m
 
     assert Response[Dict[int, int]](data={1: '4'}).model_dump() == {'data': {1: 4}}
     with pytest.raises(ValidationError) as exc_info:
         Response[Dict[int, int]](data={1: 'a'})
     assert exc_info.value.errors(include_url=False) == [
         {
             'type': 'int_parsing',
@@ -171,18 +172,19 @@
     T = TypeVar('T')
 
     class Model(CustomGenericModel, Generic[T]):
         data: T
 
     instance = Model[int](data=1)
 
-    with pytest.raises(TypeError) as exc_info:
+    with pytest.raises(ValidationError) as exc_info:
         instance.data = 2
-
-    assert str(exc_info.value) == '"Model[int]" is frozen and does not support item assignment'
+    assert exc_info.value.errors(include_url=False) == [
+        {'type': 'frozen_instance', 'loc': ('data',), 'msg': 'Instance is frozen', 'input': 2}
+    ]
 
 
 def test_default_argument():
     T = TypeVar('T')
 
     class Result(BaseModel, Generic[T]):
         data: T
@@ -440,15 +442,15 @@
     data_type = TypeVar('data_type')
 
     class Result(BaseModel, Generic[data_type], frozen=True):
         data: data_type
 
     result = Result[int](data=1)
     assert result.data == 1
-    with pytest.raises(TypeError):
+    with pytest.raises(ValidationError):
         result.data = 2
 
 
 def test_enum_generic():
     T = TypeVar('T')
 
     class MyEnum(IntEnum):
@@ -637,15 +639,15 @@
     class OuterT_SameType(BaseModel, Generic[AT]):
         i: InnerT[AT]
 
     OuterT_SameType[int](i={'a': 8})
     OuterT_SameType[int](i=inner_int)
     OuterT_SameType[str](i=inner_str)
     # TODO: The next line is failing, but passes in v1.
-    #   Might need to do something smart for Any, or re-parse-from-dict if the pydantic_generic_origin is the same..
+    #   Should re-parse-from-dict if the pydantic_generic_origin is the same
     # OuterT_SameType[str](i=inner_int_any)
     OuterT_SameType[int](i=inner_int_any.model_dump())
 
     with pytest.raises(ValidationError) as exc_info:
         OuterT_SameType[int](i=inner_str.model_dump())
     assert exc_info.value.errors(include_url=False) == [
         {
@@ -1098,48 +1100,98 @@
     if sys.version_info >= (3, 10):
         # Check that types.UnionType gets handled properly
         assert replace_types(str | list[T] | float, {T: int}) == str | list[int] | float
 
 
 def test_replace_types_with_user_defined_generic_type_field():
     """Test that using user defined generic types as generic model fields are handled correctly."""
-
     T = TypeVar('T')
     KT = TypeVar('KT')
     VT = TypeVar('VT')
 
     class CustomCounter(Counter[T]):
-        pass
+        @classmethod
+        def __get_pydantic_core_schema__(cls, source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
+            return core_schema.no_info_after_validator_function(
+                cls, handler.generate_schema(Counter[get_args(source_type)[0]])
+            )
 
     class CustomDefaultDict(DefaultDict[KT, VT]):
-        pass
+        @classmethod
+        def __get_pydantic_core_schema__(cls, source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
+            keys_type, values_type = get_args(source_type)
+            return core_schema.no_info_after_validator_function(
+                lambda x: cls(x.default_factory, x), handler.generate_schema(DefaultDict[keys_type, values_type])
+            )
 
     class CustomDeque(Deque[T]):
-        pass
+        @classmethod
+        def __get_pydantic_core_schema__(cls, source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
+            return core_schema.no_info_after_validator_function(
+                cls, handler.generate_schema(Deque[get_args(source_type)[0]])
+            )
 
     class CustomDict(Dict[KT, VT]):
-        pass
+        @classmethod
+        def __get_pydantic_core_schema__(cls, source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
+            keys_type, values_type = get_args(source_type)
+            return core_schema.no_info_after_validator_function(
+                cls, handler.generate_schema(Dict[keys_type, values_type])
+            )
 
     class CustomFrozenset(FrozenSet[T]):
-        pass
+        @classmethod
+        def __get_pydantic_core_schema__(cls, source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
+            return core_schema.no_info_after_validator_function(
+                cls, handler.generate_schema(FrozenSet[get_args(source_type)[0]])
+            )
 
     class CustomIterable(Iterable[T]):
-        pass
+        def __init__(self, iterable):
+            self.iterable = iterable
+
+        def __iter__(self):
+            return self
+
+        def __next__(self):
+            return next(self.iterable)
+
+        @classmethod
+        def __get_pydantic_core_schema__(cls, source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
+            return core_schema.no_info_after_validator_function(
+                cls, handler.generate_schema(Iterable[get_args(source_type)[0]])
+            )
 
     class CustomList(List[T]):
-        pass
+        @classmethod
+        def __get_pydantic_core_schema__(cls, source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
+            return core_schema.no_info_after_validator_function(
+                cls, handler.generate_schema(List[get_args(source_type)[0]])
+            )
 
     class CustomMapping(Mapping[KT, VT]):
-        pass
+        @classmethod
+        def __get_pydantic_core_schema__(cls, source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
+            keys_type, values_type = get_args(source_type)
+            return handler.generate_schema(Mapping[keys_type, values_type])
 
     class CustomOrderedDict(OrderedDict[KT, VT]):
-        pass
+        @classmethod
+        def __get_pydantic_core_schema__(cls, source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
+            keys_type, values_type = get_args(source_type)
+            return core_schema.no_info_after_validator_function(
+                cls, handler.generate_schema(OrderedDict[keys_type, values_type])
+            )
 
     class CustomSet(Set[T]):
-        pass
+        @classmethod
+        def __get_pydantic_core_schema__(cls, source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
+            return core_schema.no_info_after_validator_function(
+                cls, handler.generate_schema(Set[get_args(source_type)[0]])
+            )
 
     class CustomTuple(Tuple[T]):
         pass
 
     class Model(BaseModel, Generic[T, KT, VT]):
         counter_field: CustomCounter[T]
         default_dict_field: CustomDefaultDict[KT, VT]
@@ -1169,36 +1221,33 @@
         ordered_dict_field=OrderedDict([('a', 1)]),
         set_field={True, False},
         tuple_field=(True,),
     )
 
     # The following assertions are just to document the current behavior, and should
     # be updated if/when we do a better job of respecting the exact annotated type
-    assert type(m.counter_field) is Counter.__origin__
-    assert type(m.default_dict_field) is dict
-    assert type(m.deque_field) is deque
-    assert type(m.dict_field) is dict
+    assert type(m.counter_field) is CustomCounter
+    # assert type(m.default_dict_field) is CustomDefaultDict
+    assert type(m.deque_field) is CustomDeque
+    assert type(m.dict_field) is CustomDict
     assert type(m.frozenset_field) is CustomFrozenset
-    assert type(m.iterable_field).__name__ == 'ValidatorIterator'
+    assert type(m.iterable_field) is CustomIterable
     assert type(m.list_field) is CustomList
-    assert type(m.mapping_field) is dict
-    assert type(m.ordered_dict_field) is OrderedDict.__origin__
+    assert type(m.mapping_field) is dict  # this is determined in CustomMapping.__get_pydantic_core_schema__
+    assert type(m.ordered_dict_field) is CustomOrderedDict
     assert type(m.set_field) is CustomSet
     assert type(m.tuple_field) is tuple
 
     assert m.model_dump() == {
         'counter_field': {False: 1, True: 1},
         'default_dict_field': {'a': 1},
         'deque_field': deque([True, False]),
         'dict_field': {'a': 1},
         'frozenset_field': frozenset({False, True}),
-        'iterable_field': HasRepr(
-            'SerializationIterator(index=0, '
-            'iterator=ValidatorIterator(index=0, schema=Some(Bool(BoolValidator { strict: false }))))'
-        ),
+        'iterable_field': HasRepr(IsStr(regex=r'SerializationIterator\(index=0, iterator=.*CustomIterable.*')),
         'list_field': [True, False],
         'mapping_field': {'a': 2},
         'ordered_dict_field': {'a': 1},
         'set_field': {False, True},
         'tuple_field': (True,),
     }
 
@@ -1208,16 +1257,17 @@
 
     class CustomSequence(Sequence[T]):
         pass
 
     with pytest.raises(
         PydanticSchemaGenerationError,
         match=(
-            'Unable to generate pydantic-core schema for custom subclasses of Sequence.'
-            ' Please define `__get_pydantic_core_schema__`.'
+            r'Unable to generate pydantic-core schema for .*'
+            ' Set `arbitrary_types_allowed=True` in the model_config to ignore this error'
+            ' or implement `__get_pydantic_core_schema__` on your type to fully support it'
         ),
     ):
 
         class Model(BaseModel, Generic[T]):
             x: CustomSequence[T]
 
 
@@ -1439,21 +1489,17 @@
         from pydantic import BaseModel
 
         T = TypeVar('T')
 
         class Model1(BaseModel, Generic[T]):
             ref: 'Model2[T]'
 
-            model_config = dict(undefined_types_warning=False)
-
         class Model2(BaseModel, Generic[T]):
             ref: Union[T, Model1[T]]
 
-            model_config = dict(undefined_types_warning=False)
-
         Model1.model_rebuild()
 
     Model1 = module.Model1
     Model2 = module.Model2
 
     with pytest.raises(ValidationError) as exc_info:
         Model1[str].model_validate(dict(ref=dict(ref=dict(ref=dict(ref=123)))))
@@ -1492,23 +1538,19 @@
         from pydantic import BaseModel
 
         T = TypeVar('T')
 
         class Model1(BaseModel, Generic[T]):
             ref: 'Model2[T]'
 
-            model_config = dict(undefined_types_warning=False)
-
         S = TypeVar('S')
 
         class Model2(BaseModel, Generic[S]):
             ref: Union[S, Model1[S]]
 
-            model_config = dict(undefined_types_warning=False)
-
         Model1.model_rebuild()
 
     Model1 = module.Model1
     # Model2 = module.Model2
 
     with pytest.raises(ValidationError) as exc_info:
         Model1[str].model_validate(dict(ref=dict(ref=dict(ref=dict(ref=123)))))
@@ -1557,24 +1599,20 @@
 
         T = TypeVar('T')
 
         class Model1(BaseModel, Generic[T]):
             ref: 'Model2[T]'
             ref2: Union['Model2[T]', None] = None
 
-            model_config = dict(undefined_types_warning=False)
-
         S = TypeVar('S')
 
         class Model2(BaseModel, Generic[S]):
             ref: Union[S, Model1[S]]
             ref2: Union[S, Model1[S], None] = None
 
-            model_config = dict(undefined_types_warning=False)
-
         Model1.model_rebuild()
 
     Model1 = module.Model1
     # Model2 = module.Model2
 
     with pytest.raises(ValidationError) as exc_info:
         Model1[str].model_validate(dict(ref=dict(ref=dict(ref=dict(ref=123)))))
@@ -1616,26 +1654,20 @@
         T1 = TypeVar('T1')
         T2 = TypeVar('T2')
         T3 = TypeVar('T3')
 
         class A1(BaseModel, Generic[T1]):
             a1: 'A2[T1]'
 
-            model_config = dict(undefined_types_warning=False)
-
         class A2(BaseModel, Generic[T2]):
             a2: 'A3[T2]'
 
-            model_config = dict(undefined_types_warning=False)
-
         class A3(BaseModel, Generic[T3]):
             a3: Union['A1[T3]', T3]
 
-            model_config = dict(undefined_types_warning=False)
-
         A1.model_rebuild()
 
     A1 = module.A1
 
     with pytest.raises(ValidationError) as exc_info:
         A1[str].model_validate({'a1': {'a2': {'a3': 1}}})
     assert exc_info.value.errors(include_url=False) == [
@@ -1662,32 +1694,28 @@
         V2 = TypeVar('V2')
         V3 = TypeVar('V3')
 
         class M1(BaseModel, Generic[V1, V2]):
             a: V1
             m: 'M2[V2]'
 
-            model_config = dict(undefined_types_warning=False)
-
         class M2(BaseModel, Generic[V3]):
             m: Union[M1[int, V3], V3]
 
-            model_config = dict(undefined_types_warning=False)
-
         M1.model_rebuild()
 
     M1 = module.M1
 
     # assert M1.__pydantic_core_schema__ == {}
     assert collect_invalid_schemas(M1.__pydantic_core_schema__) == []
 
 
 def test_generic_recursive_models_complicated(create_module):
     """
-    TODO: If we drop the use of LimitedDict and use WeakValueDictionary only, this test will fail if run by itself.
+    Note: If we drop the use of LimitedDict and use WeakValueDictionary only, this test will fail if run by itself.
         This is due to weird behavior with the WeakValueDictionary used for caching.
         As part of the next batch of generics work, we should attempt to fix this if possible.
         In the meantime, if this causes issues, or the test otherwise starts failing, please make it xfail
         with strict=False
     """
 
     @create_module
@@ -1699,59 +1727,45 @@
         T1 = TypeVar('T1')
         T2 = TypeVar('T2')
         T3 = TypeVar('T3')
 
         class A1(BaseModel, Generic[T1]):
             a1: 'A2[T1]'
 
-            model_config = dict(undefined_types_warning=False)
-
         class A2(BaseModel, Generic[T2]):
             a2: 'A3[T2]'
 
-            model_config = dict(undefined_types_warning=False)
-
         class A3(BaseModel, Generic[T3]):
             a3: Union[A1[T3], T3]
 
-            model_config = dict(undefined_types_warning=False)
-
         A1.model_rebuild()
 
         S1 = TypeVar('S1')
         S2 = TypeVar('S2')
 
         class B1(BaseModel, Generic[S1]):
             a1: 'B2[S1]'
 
-            model_config = dict(undefined_types_warning=False)
-
         class B2(BaseModel, Generic[S2]):
             a2: 'B1[S2]'
 
-            model_config = dict(undefined_types_warning=False)
-
         B1.model_rebuild()
 
         V1 = TypeVar('V1')
         V2 = TypeVar('V2')
         V3 = TypeVar('V3')
 
         class M1(BaseModel, Generic[V1, V2]):
             a: int
             b: B1[V2]
             m: 'M2[V1]'
 
-            model_config = dict(undefined_types_warning=False)
-
         class M2(BaseModel, Generic[V3]):
             m: Union[M1[V3, int], V3]
 
-            model_config = dict(undefined_types_warning=False)
-
         M1.model_rebuild()
 
     M1 = module.M1
 
     assert collect_invalid_schemas(M1.__pydantic_core_schema__) == []
 
 
@@ -1826,15 +1840,19 @@
     assert set(Model.model_json_schema()['$defs']) == {'EnumA', 'EnumB', 'GModel_EnumA_', 'GModel_EnumB_'}
 
 
 def test_generic_with_user_defined_generic_field():
     T = TypeVar('T')
 
     class GenericList(List[T]):
-        pass
+        @classmethod
+        def __get_pydantic_core_schema__(cls, source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
+            return core_schema.no_info_after_validator_function(
+                GenericList, handler.generate_schema(List[get_args(source_type)[0]])
+            )
 
     class Model(BaseModel, Generic[T]):
         field: GenericList[T]
 
     model = Model[int](field=[5])
     assert model.field[0] == 5
 
@@ -1983,37 +2001,49 @@
     class C(B[str], Generic[T]):
         c: T
         z: str = 'c'
 
     assert C(a=1, c=...).model_dump() == {'a': 1, 'b': None, 'c': ..., 'x': 'a', 'y': 'b', 'z': 'c'}
 
 
-@pytest.mark.xfail(reason="'Json type's JSON schema; see issue #5072")
 def test_parse_generic_json():
     T = TypeVar('T')
 
     class MessageWrapper(BaseModel, Generic[T]):
         message: Json[T]
 
     class Payload(BaseModel):
         payload_field: str
 
     raw = json.dumps({'payload_field': 'payload'})
     record = MessageWrapper[Payload](message=raw)
     assert isinstance(record.message, Payload)
 
-    schema = record.model_json_schema()
-    # This seems appropriate if the goal is to represent the "serialization" schema, not the validation schema.
-    # We may need a better approach for types with different inputs and outputs; I opened an issue for this in #5072
-    assert schema['properties'] == {'message': {'$ref': '#/definitions/Payload'}}
-    assert schema['definitions']['Payload'] == {
-        'title': 'Payload',
+    validation_schema = record.model_json_schema(mode='validation')
+    assert validation_schema == {
+        'properties': {'message': {'format': 'json-string', 'title': 'Message', 'type': 'string'}},
+        'required': ['message'],
+        'title': 'MessageWrapper[test_parse_generic_json.<locals>.Payload]',
+        'type': 'object',
+    }
+
+    serialization_schema = record.model_json_schema(mode='serialization')
+    assert serialization_schema == {
+        '$defs': {
+            'Payload': {
+                'properties': {'payload_field': {'title': 'Payload Field', 'type': 'string'}},
+                'required': ['payload_field'],
+                'title': 'Payload',
+                'type': 'object',
+            }
+        },
+        'properties': {'message': {'allOf': [{'$ref': '#/$defs/Payload'}], 'title': 'Message'}},
+        'required': ['message'],
+        'title': 'MessageWrapper[test_parse_generic_json.<locals>.Payload]',
         'type': 'object',
-        'properties': {'payload_field': {'title': 'Payload Field', 'type': 'string'}},
-        'required': ['payload_field'],
     }
 
 
 def memray_limit_memory(limit):
     if '--memray' in sys.argv:
         return pytest.mark.limit_memory(limit)
     else:
@@ -2313,15 +2343,18 @@
         'required': ['x'],
         'title': 'Model[test_generic_intenum_bound.<locals>.MyEnum]',
         'type': 'object',
     }
 
 
 @pytest.mark.skipif(sys.version_info < (3, 11), reason='requires python 3.11 or higher')
-@pytest.mark.xfail(reason='TODO: Variadic generic parametrization is not supported yet')
+@pytest.mark.xfail(
+    reason='TODO: Variadic generic parametrization is not supported yet;'
+    ' Issue: https://github.com/pydantic/pydantic/issues/5804'
+)
 def test_variadic_generic_init():
     class ComponentModel(BaseModel):
         pass
 
     class Wrench(ComponentModel):
         pass
 
@@ -2346,15 +2379,17 @@
         main_component=sa, left_component_pocket=[w], right_component_pocket=[sb]
     )
 
     assert my_toolbox.all_components == [sa, w, sb]
 
 
 @pytest.mark.skipif(sys.version_info < (3, 11), reason='requires python 3.11 or higher')
-@pytest.mark.xfail(reason='TODO: Variadic fields are not supported yet')
+@pytest.mark.xfail(
+    reason='TODO: Variadic fields are not supported yet; Issue: https://github.com/pydantic/pydantic/issues/5804'
+)
 def test_variadic_generic_with_variadic_fields():
     class ComponentModel(BaseModel):
         pass
 
     class Wrench(ComponentModel):
         pass
```

### Comparing `pydantic-2.0a4/tests/test_internal.py` & `pydantic-2.0b1/tests/test_internal.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,58 +1,82 @@
 """
 Tests for internal things that are complex enough to warrant their own unit tests.
 """
+from dataclasses import dataclass
+
 import pytest
 from pydantic_core import core_schema as cs
 
-# TODO: rewrite these tests to use the two individual functions
-from pydantic._internal._core_utils import _simplify_schema_references as simplify_schema_references  # type: ignore
+from pydantic._internal._core_utils import flatten_schema_defs, inline_schema_defs
+from pydantic._internal._repr import Representation
 
 
 @pytest.mark.parametrize(
-    'input_schema, expected_output',
+    'input_schema,flattened,inlined',
     [
         # Test case 1: Simple schema with no references
-        (cs.list_schema(cs.int_schema()), cs.list_schema(cs.int_schema())),
+        (cs.list_schema(cs.int_schema()), cs.list_schema(cs.int_schema()), cs.list_schema(cs.int_schema())),
         # Test case 2: Schema with single-level nested references
         (
             cs.definitions_schema(
                 cs.list_schema(cs.definition_reference_schema('list_of_ints')),
                 definitions=[
                     cs.list_schema(cs.definition_reference_schema('int'), ref='list_of_ints'),
                     cs.int_schema(ref='int'),
                 ],
             ),
+            cs.definitions_schema(
+                cs.list_schema(cs.definition_reference_schema('list_of_ints')),
+                definitions=[
+                    cs.list_schema(cs.definition_reference_schema('int'), ref='list_of_ints'),
+                    cs.int_schema(ref='int'),
+                ],
+            ),
             cs.list_schema(cs.list_schema(cs.int_schema())),
         ),
         # Test case 3: Schema with multiple single-level nested references
         (
             cs.list_schema(
                 cs.definitions_schema(cs.definition_reference_schema('int'), definitions=[cs.int_schema(ref='int')])
             ),
+            cs.definitions_schema(
+                cs.list_schema(cs.definition_reference_schema('int')), definitions=[cs.int_schema(ref='int')]
+            ),
             cs.list_schema(cs.int_schema()),
         ),
         # Test case 4: A simple recursive schema
         (
             cs.list_schema(cs.definition_reference_schema(schema_ref='list'), ref='list'),
             cs.definitions_schema(
                 cs.definition_reference_schema(schema_ref='list'),
                 definitions=[cs.list_schema(cs.definition_reference_schema(schema_ref='list'), ref='list')],
             ),
+            cs.definitions_schema(
+                cs.definition_reference_schema(schema_ref='list'),
+                definitions=[cs.list_schema(cs.definition_reference_schema(schema_ref='list'), ref='list')],
+            ),
         ),
         # Test case 5: Deeply nested schema with multiple references
         (
             cs.definitions_schema(
                 cs.list_schema(cs.definition_reference_schema('list_of_lists_of_ints')),
                 definitions=[
                     cs.list_schema(cs.definition_reference_schema('list_of_ints'), ref='list_of_lists_of_ints'),
                     cs.list_schema(cs.definition_reference_schema('int'), ref='list_of_ints'),
                     cs.int_schema(ref='int'),
                 ],
             ),
+            cs.definitions_schema(
+                cs.list_schema(cs.definition_reference_schema('list_of_lists_of_ints')),
+                definitions=[
+                    cs.list_schema(cs.definition_reference_schema('list_of_ints'), ref='list_of_lists_of_ints'),
+                    cs.list_schema(cs.definition_reference_schema('int'), ref='list_of_ints'),
+                    cs.int_schema(ref='int'),
+                ],
+            ),
             cs.list_schema(cs.list_schema(cs.list_schema(cs.int_schema()))),
         ),
         # Test case 6: More complex recursive schema
         (
             cs.definitions_schema(
                 cs.list_schema(cs.definition_reference_schema(schema_ref='list_of_ints_and_lists')),
                 definitions=[
@@ -67,14 +91,28 @@
                             ],
                         ),
                         ref='list_of_ints_and_lists',
                     ),
                     cs.int_schema(ref='int_or_list'),
                 ],
             ),
+            cs.definitions_schema(
+                cs.list_schema(cs.definition_reference_schema(schema_ref='list_of_ints_and_lists')),
+                definitions=[
+                    cs.list_schema(
+                        cs.definition_reference_schema(schema_ref='int_or_list'),
+                        ref='list_of_ints_and_lists',
+                    ),
+                    cs.int_schema(ref='int'),
+                    cs.tuple_variable_schema(
+                        cs.definition_reference_schema(schema_ref='list_of_ints_and_lists'), ref='a tuple'
+                    ),
+                    cs.int_schema(ref='int_or_list'),
+                ],
+            ),
             cs.list_schema(cs.list_schema(cs.int_schema())),
         ),
         # Test case 7: Schema with multiple definitions and nested references, some of which are unused
         (
             cs.definitions_schema(
                 cs.list_schema(cs.definition_reference_schema('list_of_ints')),
                 definitions=[
@@ -82,14 +120,24 @@
                         cs.definitions_schema(
                             cs.definition_reference_schema('int'), definitions=[cs.int_schema(ref='int')]
                         ),
                         ref='list_of_ints',
                     )
                 ],
             ),
+            cs.definitions_schema(
+                cs.list_schema(cs.definition_reference_schema('list_of_ints')),
+                definitions=[
+                    cs.list_schema(
+                        cs.definition_reference_schema('int'),
+                        ref='list_of_ints',
+                    ),
+                    cs.int_schema(ref='int'),
+                ],
+            ),
             cs.list_schema(cs.list_schema(cs.int_schema())),
         ),
         # Test case 8: Reference is used in multiple places
         (
             cs.definitions_schema(
                 cs.union_schema(
                     [
@@ -101,19 +149,50 @@
                     cs.list_schema(cs.definition_reference_schema('int'), ref='list_of_ints'),
                     cs.int_schema(ref='int'),
                 ],
             ),
             cs.definitions_schema(
                 cs.union_schema(
                     [
+                        cs.definition_reference_schema('list_of_ints'),
+                        cs.tuple_variable_schema(cs.definition_reference_schema('int')),
+                    ]
+                ),
+                definitions=[
+                    cs.list_schema(cs.definition_reference_schema('int'), ref='list_of_ints'),
+                    cs.int_schema(ref='int'),
+                ],
+            ),
+            cs.definitions_schema(
+                cs.union_schema(
+                    [
                         cs.list_schema(cs.definition_reference_schema('int')),
                         cs.tuple_variable_schema(cs.definition_reference_schema('int')),
                     ]
                 ),
                 definitions=[cs.int_schema(ref='int')],
             ),
         ),
     ],
 )
-def test_build_definitions_schema(input_schema: cs.CoreSchema, expected_output: cs.CoreSchema):
-    result = simplify_schema_references(input_schema, True)
-    assert result == expected_output
+def test_build_schema_defs(input_schema: cs.CoreSchema, flattened: cs.CoreSchema, inlined: cs.CoreSchema):
+    assert flatten_schema_defs(input_schema) == flattened
+    assert inline_schema_defs(input_schema) == inlined
+
+
+def test_representation_integrations():
+    devtools = pytest.importorskip('devtools')
+
+    @dataclass
+    class Obj(Representation):
+        int_attr: int = 42
+        str_attr: str = 'Marvin'
+
+    obj = Obj()
+
+    assert str(devtools.debug.format(obj)).split('\n')[1:] == [
+        '    Obj(',
+        '        int_attr=42,',
+        "        str_attr='Marvin',",
+        '    ) (Obj)',
+    ]
+    assert list(obj.__rich_repr__()) == [('int_attr', 42), ('str_attr', 'Marvin')]
```

### Comparing `pydantic-2.0a4/tests/test_json.py` & `pydantic-2.0b1/tests/test_json.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,25 +3,30 @@
 import sys
 from dataclasses import dataclass as vanilla_dataclass
 from datetime import date, datetime, time, timedelta, timezone
 from decimal import Decimal
 from enum import Enum
 from ipaddress import IPv4Address, IPv4Interface, IPv4Network, IPv6Address, IPv6Interface, IPv6Network
 from pathlib import Path
-from typing import Generator, Optional, Pattern
+from typing import Any, Generator, Optional, Pattern
 from uuid import UUID
 
 import pytest
-from pydantic_core import SchemaSerializer
+from pydantic_core import CoreSchema, SchemaSerializer, core_schema
 
-from pydantic import BaseModel, ConfigDict, NameEmail, field_serializer
+from pydantic import BaseModel, ConfigDict, GetCoreSchemaHandler, GetJsonSchemaHandler, NameEmail
+from pydantic._internal._config import ConfigWrapper
 from pydantic._internal._generate_schema import GenerateSchema
 from pydantic.color import Color
 from pydantic.dataclasses import dataclass as pydantic_dataclass
 from pydantic.deprecated.json import pydantic_encoder, timedelta_isoformat
+from pydantic.functional_serializers import (
+    field_serializer,
+)
+from pydantic.json_schema import JsonSchemaValue
 from pydantic.types import DirectoryPath, FilePath, SecretBytes, SecretStr, condecimal
 
 try:
     import email_validator
 except ImportError:
     email_validator = None
 
@@ -68,23 +73,25 @@
         (Decimal, lambda: Decimal('12.34'), b'"12.34"'),
         (MyModel, lambda: MyModel(), b'{"a":"b","c":"d"}'),
         (MyEnum, lambda: MyEnum.foo, b'"bar"'),
         (Pattern, lambda: re.compile('^regex$'), b'"^regex$"'),
     ],
 )
 def test_json_serialization(ser_type, gen_value, json_output):
-    gen = GenerateSchema(False, None)
+    config_wrapper = ConfigWrapper({'arbitrary_types_allowed': False})
+    gen = GenerateSchema(config_wrapper, None)
     schema = gen.generate_schema(ser_type)
     serializer = SchemaSerializer(schema)
     assert serializer.to_json(gen_value()) == json_output
 
 
 @pytest.mark.skipif(not email_validator, reason='email_validator not installed')
 def test_json_serialization_email():
-    gen = GenerateSchema(False, None)
+    config_wrapper = ConfigWrapper({'arbitrary_types_allowed': False})
+    gen = GenerateSchema(config_wrapper, None)
     schema = gen.generate_schema(NameEmail)
     serializer = SchemaSerializer(schema)
     assert serializer.to_json(NameEmail('foo bar', 'foobaR@example.com')) == b'"foo bar <foobaR@example.com>"'
 
 
 @pytest.mark.skipif(sys.platform.startswith('win'), reason='paths look different on windows')
 def test_path_encoding(tmpdir):
@@ -118,31 +125,46 @@
     assert m.model_dump() == {'a': 10.2, 'b': b'foobar', 'c': Decimal('10.2'), 'd': {'x': 123, 'y': '123'}}
     assert m.model_dump_json() == '{"a":10.2,"b":"foobar","c":"10.2","d":{"x":123,"y":"123"}}'
     assert m.model_dump_json(exclude={'b'}) == '{"a":10.2,"c":"10.2","d":{"x":123,"y":"123"}}'
 
 
 def test_subclass_encoding():
     class SubDate(datetime):
-        pass
+        @classmethod
+        def __get_pydantic_core_schema__(cls, source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
+            def val(v: datetime) -> SubDate:
+                return SubDate.fromtimestamp(v.timestamp())
+
+            return core_schema.no_info_after_validator_function(val, handler.generate_schema(datetime))
 
     class Model(BaseModel):
         a: datetime
         b: SubDate
 
     m = Model(a=datetime(2032, 1, 1, 1, 1), b=SubDate(2020, 2, 29, 12, 30))
     assert m.model_dump() == {'a': datetime(2032, 1, 1, 1, 1), 'b': SubDate(2020, 2, 29, 12, 30)}
     assert m.model_dump_json() == '{"a":"2032-01-01T01:01:00","b":"2020-02-29T12:30:00"}'
 
 
 def test_subclass_custom_encoding():
     class SubDt(datetime):
-        pass
+        @classmethod
+        def __get_pydantic_core_schema__(cls, source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
+            def val(v: datetime) -> SubDt:
+                return SubDt.fromtimestamp(v.timestamp())
+
+            return core_schema.no_info_after_validator_function(val, handler.generate_schema(datetime))
 
     class SubDelta(timedelta):
-        pass
+        @classmethod
+        def __get_pydantic_core_schema__(cls, source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
+            def val(v: timedelta) -> SubDelta:
+                return cls(seconds=v.total_seconds())
+
+            return core_schema.no_info_after_validator_function(val, handler.generate_schema(timedelta))
 
     class Model(BaseModel):
         a: SubDt
         b: SubDelta
 
         @field_serializer('a', when_used='json')
         def serialize_a(self, v: SubDt, _info):
@@ -331,7 +353,27 @@
     value: int
     nested: Optional[Model] = None
 """
     )
     M = module.Model
 
     assert M(value=1, nested=M(value=2)).model_dump_json(exclude_none=True) == '{"value":1,"nested":{"value":2}}'
+
+
+def test_unresolvable_schema_lookup_error():
+    class Model(BaseModel):
+        mini_me: 'Model'
+
+        @classmethod
+        def __get_pydantic_json_schema__(
+            cls, core_schema: CoreSchema, handler: GetJsonSchemaHandler
+        ) -> JsonSchemaValue:
+            json_schema = super().__get_pydantic_json_schema__(core_schema, handler)
+            return handler.resolve_ref_schema(json_schema)
+
+    with pytest.raises(LookupError) as e:
+        Model.model_json_schema()
+
+    assert e.value.args[0] == (
+        'Could not find a ref for #/$defs/Model.'
+        ' Maybe you tried to call resolve_ref_schema from within a recursive model?'
+    )
```

### Comparing `pydantic-2.0a4/tests/test_json_schema.py` & `pydantic-2.0b1/tests/test_json_schema.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 import math
 import re
+import typing
 from datetime import date, datetime, time, timedelta
 from decimal import Decimal
 from enum import Enum, IntEnum
 from ipaddress import IPv4Address, IPv4Interface, IPv4Network, IPv6Address, IPv6Interface, IPv6Network
 from pathlib import Path
 from typing import (
     Any,
@@ -15,14 +16,15 @@
     Generic,
     Iterable,
     List,
     NamedTuple,
     NewType,
     Optional,
     Pattern,
+    Sequence,
     Set,
     Tuple,
     Type,
     TypeVar,
     Union,
 )
 from uuid import UUID
@@ -30,56 +32,61 @@
 import pytest
 from pydantic_core import CoreSchema, core_schema
 from typing_extensions import Annotated, Literal
 
 from pydantic import (
     BaseModel,
     Field,
+    GetCoreSchemaHandler,
+    GetJsonSchemaHandler,
     ImportString,
+    PydanticUserError,
+    RootModel,
     ValidationError,
+    computed_field,
     field_validator,
 )
-from pydantic._internal._core_metadata import build_metadata_dict
-from pydantic.annotated import GetCoreSchemaHandler
+from pydantic._internal._core_metadata import CoreMetadataHandler, build_metadata_dict
 from pydantic.color import Color
 from pydantic.config import ConfigDict
 from pydantic.dataclasses import dataclass
 from pydantic.errors import PydanticInvalidForJsonSchema
 from pydantic.json_schema import (
     DEFAULT_REF_TEMPLATE,
     GenerateJsonSchema,
-    GetJsonSchemaHandler,
     JsonSchemaValue,
     PydanticJsonSchemaWarning,
     model_json_schema,
     models_json_schema,
 )
-from pydantic.networks import AnyUrl, EmailStr, IPvAnyAddress, IPvAnyInterface, IPvAnyNetwork, NameEmail
+from pydantic.networks import AnyUrl, EmailStr, IPvAnyAddress, IPvAnyInterface, IPvAnyNetwork, MultiHostUrl, NameEmail
 from pydantic.type_adapter import TypeAdapter
 from pydantic.types import (
     UUID1,
     UUID3,
     UUID4,
     UUID5,
     DirectoryPath,
     FilePath,
+    InstanceOf,
     Json,
     NegativeFloat,
     NegativeInt,
     NewPath,
     NonNegativeFloat,
     NonNegativeInt,
     NonPositiveFloat,
     NonPositiveInt,
     PositiveFloat,
     PositiveInt,
     SecretBytes,
     SecretStr,
     StrictBool,
     StrictStr,
+    WithJsonSchema,
     conbytes,
     condate,
     condecimal,
     confloat,
     conint,
     constr,
 )
@@ -417,14 +424,26 @@
         },
         'required': ['enum', 'extra_enum'],
         'title': 'Foo',
         'type': 'object',
     }
 
 
+def test_invalid_json_schema_extra():
+    class MyModel(BaseModel):
+        model_config = ConfigDict(json_schema_extra=1)
+
+        name: str
+
+    with pytest.raises(
+        ValueError, match=re.escape("model_config['json_schema_extra']=1 should be a dict, callable, or None")
+    ):
+        MyModel.model_json_schema()
+
+
 def test_list_enum_schema_extras():
     class FoodChoice(str, Enum):
         spam = 'spam'
         egg = 'egg'
         chips = 'chips'
 
     class Model(BaseModel):
@@ -476,35 +495,38 @@
                 'enum': ['foo', 'bar'],
                 'type': 'string',
             }
         },
     }
 
 
-def test_json_schema():
+def test_decimal_json_schema():
     class Model(BaseModel):
         a: bytes = b'foobar'
         b: Decimal = Decimal('12.34')
 
-    # TODO: What do we want the generated schema to be for Decimal? I'm thinking 'integer', 'number', _or_ 'str'
-    #     Decision: What we have in v1 is not bad enough to be worth changing
-    #     (i.e., keep it as only 'number'; maybe add a comment that other things could be okay)
+    model_json_schema_validation = Model.model_json_schema(mode='validation')
+    model_json_schema_serialization = Model.model_json_schema(mode='serialization')
 
-    with pytest.warns(
-        DeprecationWarning,
-        match=re.escape('The `schema_json` method is deprecated; use `model_json_schema` and json.dumps instead.'),
-    ):
-        schema_json = Model.schema_json(indent=2)
-    assert json.loads(schema_json) == {
+    assert model_json_schema_validation == {
+        'properties': {
+            'a': {'default': 'foobar', 'format': 'binary', 'title': 'A', 'type': 'string'},
+            'b': {'anyOf': [{'type': 'number'}, {'type': 'string'}], 'default': '12.34', 'title': 'B'},
+        },
         'title': 'Model',
         'type': 'object',
+    }
+    assert model_json_schema_serialization == {
         'properties': {
-            'a': {'title': 'A', 'default': 'foobar', 'type': 'string', 'format': 'binary'},
-            'b': {'title': 'B', 'default': '12.34', 'type': 'number'},
+            'a': {'default': 'foobar', 'format': 'binary', 'title': 'A', 'type': 'string'},
+            'b': {'default': '12.34', 'title': 'B', 'type': 'string'},
         },
+        'required': ['a', 'b'],
+        'title': 'Model',
+        'type': 'object',
     }
 
 
 def test_list_sub_model():
     class Foo(BaseModel):
         a: float
 
@@ -535,14 +557,33 @@
         'title': 'Model',
         'type': 'object',
         'properties': {'a': {'anyOf': [{'type': 'string'}, {'type': 'null'}], 'title': 'A'}},
         'required': ['a'],
     }
 
 
+def test_optional_modify_schema():
+    class MyNone(Type[None]):
+        @classmethod
+        def __get_pydantic_core_schema__(
+            cls, source_type: Any, handler: GetCoreSchemaHandler
+        ) -> core_schema.CoreSchema:
+            return core_schema.nullable_schema(core_schema.none_schema())
+
+    class Model(BaseModel):
+        x: MyNone
+
+    assert Model.model_json_schema() == {
+        'properties': {'x': {'title': 'X', 'type': 'null'}},
+        'required': ['x'],
+        'title': 'Model',
+        'type': 'object',
+    }
+
+
 def test_any():
     class Model(BaseModel):
         a: Any
         b: object
 
     assert Model.model_json_schema() == {
         'title': 'Model',
@@ -573,14 +614,15 @@
     }
 
 
 @pytest.mark.parametrize(
     'field_type,extra_props',
     [
         (tuple, {'items': {}}),
+        (Tuple, {'items': {}}),
         (
             Tuple[str, int, Union[str, int, float], float],
             {
                 'prefixItems': [
                     {'type': 'string'},
                     {'type': 'integer'},
                     {'anyOf': [{'type': 'string'}, {'type': 'integer'}, {'type': 'number'}]},
@@ -716,14 +758,18 @@
                 },
                 'properties': {'a': {'anyOf': [{'$ref': '#/$defs/Foo'}, {'type': 'null'}]}},
                 'required': ['a'],
                 'title': 'Model',
                 'type': 'object',
             },
         ),
+        (
+            Union[int, int],
+            {'properties': {'a': {'title': 'A', 'type': 'integer'}}, 'required': ['a']},
+        ),
         (Dict[str, Any], {'properties': {'a': {'title': 'A', 'type': 'object'}}, 'required': ['a']}),
     ],
 )
 def test_list_union_dict(field_type, expected_schema):
     class Model(BaseModel):
         a: field_type
 
@@ -735,15 +781,15 @@
 
 @pytest.mark.parametrize(
     'field_type,expected_schema',
     [
         (datetime, {'type': 'string', 'format': 'date-time'}),
         (date, {'type': 'string', 'format': 'date'}),
         (time, {'type': 'string', 'format': 'time'}),
-        (timedelta, {'type': 'number', 'format': 'time-delta'}),
+        (timedelta, {'type': 'string', 'format': 'duration'}),
     ],
 )
 def test_date_types(field_type, expected_schema):
     class Model(BaseModel):
         a: field_type
 
     attribute_schema = {'title': 'A'}
@@ -859,14 +905,15 @@
     'field_type,expected_schema',
     [
         (AnyUrl, {'title': 'A', 'type': 'string', 'format': 'uri', 'minLength': 1}),
         (
             Annotated[AnyUrl, Field(max_length=2**16)],
             {'title': 'A', 'type': 'string', 'format': 'uri', 'minLength': 1, 'maxLength': 2**16},
         ),
+        (MultiHostUrl, {'title': 'A', 'type': 'string', 'format': 'multi-host-uri', 'minLength': 1}),
     ],
 )
 def test_special_str_types(field_type, expected_schema):
     class Model(BaseModel):
         a: field_type
 
     base_schema = {'title': 'Model', 'type': 'object', 'properties': {'a': {}}, 'required': ['a']}
@@ -934,29 +981,21 @@
 
     assert Model.model_json_schema() == base_schema
 
 
 @pytest.mark.parametrize(
     'field_type,expected_schema',
     [
-        # (ConstrainedFloat, {}),
         (confloat(gt=5, lt=10), {'exclusiveMinimum': 5, 'exclusiveMaximum': 10}),
         (confloat(ge=5, le=10), {'minimum': 5, 'maximum': 10}),
         (confloat(multiple_of=5), {'multipleOf': 5}),
         (PositiveFloat, {'exclusiveMinimum': 0}),
         (NegativeFloat, {'exclusiveMaximum': 0}),
         (NonNegativeFloat, {'minimum': 0}),
         (NonPositiveFloat, {'maximum': 0}),
-        # (ConstrainedDecimal, {}),
-        (
-            condecimal(gt=5, lt=10),
-            {'exclusiveMinimum': 5, 'exclusiveMaximum': 10},
-        ),
-        (condecimal(ge=5, le=10), {'minimum': 5, 'maximum': 10}),
-        (condecimal(multiple_of=5), {'multipleOf': 5}),
     ],
 )
 def test_special_float_types(field_type, expected_schema):
     class Model(BaseModel):
         a: field_type
 
     base_schema = {
@@ -968,14 +1007,37 @@
     base_schema['properties']['a'].update(expected_schema)
 
     assert Model.model_json_schema() == base_schema
 
 
 @pytest.mark.parametrize(
     'field_type,expected_schema',
+    [
+        (condecimal(gt=5, lt=10), {'exclusiveMinimum': 5, 'exclusiveMaximum': 10}),
+        (condecimal(ge=5, le=10), {'minimum': 5, 'maximum': 10}),
+        (condecimal(multiple_of=5), {'multipleOf': 5}),
+    ],
+)
+def test_special_decimal_types(field_type, expected_schema):
+    class Model(BaseModel):
+        a: field_type
+
+    base_schema = {
+        'title': 'Model',
+        'type': 'object',
+        'properties': {'a': {'anyOf': [{'type': 'number'}, {'type': 'string'}], 'title': 'A'}},
+        'required': ['a'],
+    }
+    base_schema['properties']['a']['anyOf'][0].update(expected_schema)
+
+    assert Model.model_json_schema() == base_schema
+
+
+@pytest.mark.parametrize(
+    'field_type,expected_schema',
     [(UUID, 'uuid'), (UUID1, 'uuid1'), (UUID3, 'uuid3'), (UUID4, 'uuid4'), (UUID5, 'uuid5')],
 )
 def test_uuid_types(field_type, expected_schema):
     class Model(BaseModel):
         a: field_type
 
     base_schema = {
@@ -1020,14 +1082,20 @@
         'properties': {
             'a': {'title': 'A', 'type': 'string', 'format': 'json-string'},
             'b': {'title': 'B', 'type': 'string', 'format': 'json-string'},
             'c': {'title': 'C', 'type': 'string', 'format': 'json-string'},
         },
         'required': ['a', 'b', 'c'],
     }
+    assert Model.model_json_schema(mode='serialization') == {
+        'properties': {'a': {'title': 'A'}, 'b': {'title': 'B', 'type': 'integer'}, 'c': {'title': 'C'}},
+        'required': ['a', 'b', 'c'],
+        'title': 'Model',
+        'type': 'object',
+    }
 
 
 def test_ipv4address_type():
     class Model(BaseModel):
         ip_address: IPv4Address
 
     model_schema = Model.model_json_schema()
@@ -1148,32 +1216,54 @@
     (
         (Callable, ...),
         (Callable, lambda x: x),
         (Callable[[int], int], ...),
         (Callable[[int], int], lambda x: x),
     ),
 )
-def test_callable_type(type_, default_value):
-    # TODO: Is this still how we want to handle this?
-    #   With my current changes, it raises
-    #       InvalidForJsonSchema('Cannot generate a JsonSchema for core_schema.CallableSchema')
-    #   We could continue the practice of just not creating such fields,
-    #   but producing a UserWarning when a field is ignored
-    # TODO: If the default value is not JSON encodable, should we just not include it in the schema?
-    #   This seems preferable to me over erroring, but maybe we should also produce a UserWarning for that?
-
-    # Decision: Different user warning depending on if there's a default or not
-
+@pytest.mark.parametrize(
+    'base_json_schema,properties',
+    [
+        (
+            {'a': 'b'},
+            {
+                'callback': {'title': 'Callback', 'a': 'b'},
+                'foo': {'title': 'Foo', 'type': 'integer'},
+            },
+        ),
+        (
+            None,
+            {
+                'foo': {'title': 'Foo', 'type': 'integer'},
+            },
+        ),
+    ],
+)
+def test_callable_type(type_, default_value, base_json_schema, properties):
     class Model(BaseModel):
         callback: type_ = default_value
         foo: int
 
     with pytest.raises(PydanticInvalidForJsonSchema):
-        model_schema = Model.model_json_schema()
-        assert 'callback' not in model_schema['properties']
+        Model.model_json_schema()
+
+    class ModelWithOverride(BaseModel):
+        callback: Annotated[type_, WithJsonSchema(base_json_schema)] = default_value
+        foo: int
+
+    if default_value is Ellipsis or base_json_schema is None:
+        model_schema = ModelWithOverride.model_json_schema()
+    else:
+        with pytest.warns(
+            PydanticJsonSchemaWarning,
+            match='Default value .* is not JSON serializable; excluding'
+            r' default from JSON schema \[non-serializable-default]',
+        ):
+            model_schema = ModelWithOverride.model_json_schema()
+    assert model_schema['properties'] == properties
 
 
 @pytest.mark.parametrize(
     'default_value,properties',
     (
         (Field(...), {'callback': {'title': 'Callback', 'type': 'integer'}}),
         (1, {'callback': {'default': 1, 'title': 'Callback', 'type': 'integer'}}),
@@ -1332,17 +1422,20 @@
     class Ingredient(BaseModel):
         name: str
 
     class Pizza(BaseModel):
         name: str
         ingredients: List[Ingredient]
 
-    model_schema = models_json_schema(
-        [Model, Pizza], title='Multi-model schema', description='Single JSON Schema with multiple definitions'
+    keys_map, model_schema = models_json_schema(
+        [(Model, 'validation'), (Pizza, 'validation')],
+        title='Multi-model schema',
+        description='Single JSON Schema with multiple definitions',
     )
+    assert keys_map == {(Pizza, 'validation'): 'Pizza', (Model, 'validation'): 'Model'}
     assert model_schema == {
         'title': 'Multi-model schema',
         'description': 'Single JSON Schema with multiple definitions',
         '$defs': {
             'Pizza': {
                 'title': 'Pizza',
                 'type': 'object',
@@ -1398,15 +1491,16 @@
 
     class Bar(BaseModel):
         b: Foo
 
     class Baz(BaseModel):
         c: Bar
 
-    model_schema = models_json_schema([Bar, Baz], ref_template=ref_template)
+    keys_map, model_schema = models_json_schema([(Bar, 'validation'), (Baz, 'validation')], ref_template=ref_template)
+    assert keys_map == {(Bar, 'validation'): 'Bar', (Baz, 'validation'): 'Baz'}
     assert model_schema == {
         '$defs': {
             'Baz': {
                 'title': 'Baz',
                 'type': 'object',
                 'properties': {'c': {'$ref': '#/components/schemas/Bar'}},
                 'required': ['c'],
@@ -1433,15 +1527,18 @@
 
     class Bar(BaseModel):
         b: Foo
 
     class Baz(BaseModel):
         c: Bar
 
-    model_schema = models_json_schema([Bar, Baz], ref_template='/schemas/{model}.json#/')
+    keys_map, model_schema = models_json_schema(
+        [(Bar, 'validation'), (Baz, 'validation')], ref_template='/schemas/{model}.json#/'
+    )
+    assert keys_map == {(Bar, 'validation'): 'Bar', (Baz, 'validation'): 'Baz'}
     assert model_schema == {
         '$defs': {
             'Baz': {
                 'title': 'Baz',
                 'type': 'object',
                 'properties': {'c': {'$ref': '/schemas/Bar.json#/'}},
                 'required': ['c'],
@@ -1469,19 +1566,20 @@
     class Bar(BaseModel):
         b: Foo
 
     class Baz(BaseModel):
         c: Bar
 
     with pytest.raises(KeyError):
-        models_json_schema([Bar, Baz], ref_template='/schemas/{bad_name}.json#/')
+        models_json_schema([(Bar, 'validation'), (Baz, 'validation')], ref_template='/schemas/{bad_name}.json#/')
 
 
 def test_schema_no_definitions():
-    model_schema = models_json_schema([], title='Schema without definitions')
+    keys_map, model_schema = models_json_schema([], title='Schema without definitions')
+    assert keys_map == {}
     assert model_schema == {'title': 'Schema without definitions'}
 
 
 def test_list_default():
     class UserModel(BaseModel):
         friends: List[int] = [1]
 
@@ -1578,33 +1676,77 @@
         ({'ge': 2}, float, {'type': 'number', 'minimum': 2}),
         ({'le': 5}, float, {'type': 'number', 'maximum': 5}),
         ({'gt': -math.inf}, float, {'type': 'number'}),
         ({'lt': math.inf}, float, {'type': 'number'}),
         ({'ge': -math.inf}, float, {'type': 'number'}),
         ({'le': math.inf}, float, {'type': 'number'}),
         ({'multiple_of': 5}, float, {'type': 'number', 'multipleOf': 5}),
-        ({'gt': 2}, Decimal, {'type': 'number', 'exclusiveMinimum': 2}),
-        ({'lt': 5}, Decimal, {'type': 'number', 'exclusiveMaximum': 5}),
-        ({'ge': 2}, Decimal, {'type': 'number', 'minimum': 2}),
-        ({'le': 5}, Decimal, {'type': 'number', 'maximum': 5}),
-        ({'multiple_of': 5}, Decimal, {'type': 'number', 'multipleOf': 5}),
+        ({'gt': 2}, Decimal, {'anyOf': [{'exclusiveMinimum': 2.0, 'type': 'number'}, {'type': 'string'}]}),
+        ({'lt': 5}, Decimal, {'anyOf': [{'type': 'number', 'exclusiveMaximum': 5}, {'type': 'string'}]}),
+        ({'ge': 2}, Decimal, {'anyOf': [{'type': 'number', 'minimum': 2}, {'type': 'string'}]}),
+        ({'le': 5}, Decimal, {'anyOf': [{'type': 'number', 'maximum': 5}, {'type': 'string'}]}),
+        ({'multiple_of': 5}, Decimal, {'anyOf': [{'type': 'number', 'multipleOf': 5}, {'type': 'string'}]}),
+    ],
+)
+def test_constraints_schema_validation(kwargs, type_, expected_extra):
+    class Foo(BaseModel):
+        a: type_ = Field('foo', title='A title', description='A description', **kwargs)
+
+    expected_schema = {
+        'title': 'Foo',
+        'type': 'object',
+        'properties': {'a': {'title': 'A title', 'description': 'A description', 'default': 'foo'}},
+    }
+
+    expected_schema['properties']['a'].update(expected_extra)
+    assert Foo.model_json_schema(mode='validation') == expected_schema
+
+
+@pytest.mark.parametrize(
+    'kwargs,type_,expected_extra',
+    [
+        ({'max_length': 5}, str, {'type': 'string', 'maxLength': 5}),
+        ({}, constr(max_length=6), {'type': 'string', 'maxLength': 6}),
+        ({'min_length': 2}, str, {'type': 'string', 'minLength': 2}),
+        ({'max_length': 5}, bytes, {'type': 'string', 'maxLength': 5, 'format': 'binary'}),
+        ({'pattern': '^foo$'}, str, {'type': 'string', 'pattern': '^foo$'}),
+        ({'gt': 2}, int, {'type': 'integer', 'exclusiveMinimum': 2}),
+        ({'lt': 5}, int, {'type': 'integer', 'exclusiveMaximum': 5}),
+        ({'ge': 2}, int, {'type': 'integer', 'minimum': 2}),
+        ({'le': 5}, int, {'type': 'integer', 'maximum': 5}),
+        ({'multiple_of': 5}, int, {'type': 'integer', 'multipleOf': 5}),
+        ({'gt': 2}, float, {'type': 'number', 'exclusiveMinimum': 2}),
+        ({'lt': 5}, float, {'type': 'number', 'exclusiveMaximum': 5}),
+        ({'ge': 2}, float, {'type': 'number', 'minimum': 2}),
+        ({'le': 5}, float, {'type': 'number', 'maximum': 5}),
+        ({'gt': -math.inf}, float, {'type': 'number'}),
+        ({'lt': math.inf}, float, {'type': 'number'}),
+        ({'ge': -math.inf}, float, {'type': 'number'}),
+        ({'le': math.inf}, float, {'type': 'number'}),
+        ({'multiple_of': 5}, float, {'type': 'number', 'multipleOf': 5}),
+        ({'gt': 2}, Decimal, {'type': 'string'}),
+        ({'lt': 5}, Decimal, {'type': 'string'}),
+        ({'ge': 2}, Decimal, {'type': 'string'}),
+        ({'le': 5}, Decimal, {'type': 'string'}),
+        ({'multiple_of': 5}, Decimal, {'type': 'string'}),
     ],
 )
-def test_constraints_schema(kwargs, type_, expected_extra):
+def test_constraints_schema_serialization(kwargs, type_, expected_extra):
     class Foo(BaseModel):
         a: type_ = Field('foo', title='A title', description='A description', **kwargs)
 
     expected_schema = {
         'title': 'Foo',
         'type': 'object',
         'properties': {'a': {'title': 'A title', 'description': 'A description', 'default': 'foo'}},
+        'required': ['a'],
     }
 
     expected_schema['properties']['a'].update(expected_extra)
-    assert Foo.model_json_schema() == expected_schema
+    assert Foo.model_json_schema(mode='serialization') == expected_schema
 
 
 @pytest.mark.parametrize(
     'kwargs,type_,value',
     [
         ({'max_length': 5}, str, 'foo'),
         ({'min_length': 2}, str, 'foo'),
@@ -1631,15 +1773,15 @@
         ({'lt': 5}, Decimal, Decimal(3)),
         ({'ge': 2}, Decimal, Decimal(3)),
         ({'ge': 2}, Decimal, Decimal(2)),
         ({'le': 5}, Decimal, Decimal(3)),
         ({'le': 5}, Decimal, Decimal(5)),
     ],
 )
-def test_constraints_schema_validation(kwargs, type_, value):
+def test_constraints_schema_validation_passes(kwargs, type_, value):
     class Foo(BaseModel):
         a: type_ = Field('foo', title='A title', description='A description', **kwargs)
 
     assert Foo(a=value)
 
 
 @pytest.mark.parametrize(
@@ -2047,24 +2189,27 @@
 
 
 def test_dataclass():
     @dataclass
     class Model:
         a: bool
 
-    assert models_json_schema([Model]) == {
-        '$defs': {
-            'Model': {
-                'title': 'Model',
-                'type': 'object',
-                'properties': {'a': {'title': 'A', 'type': 'boolean'}},
-                'required': ['a'],
+    assert models_json_schema([(Model, 'validation')]) == (
+        {(Model, 'validation'): 'Model'},
+        {
+            '$defs': {
+                'Model': {
+                    'title': 'Model',
+                    'type': 'object',
+                    'properties': {'a': {'title': 'A', 'type': 'boolean'}},
+                    'required': ['a'],
+                }
             }
-        }
-    }
+        },
+    )
 
     assert model_json_schema(Model) == {
         'title': 'Model',
         'type': 'object',
         'properties': {'a': {'title': 'A', 'type': 'boolean'}},
         'required': ['a'],
     }
@@ -2096,17 +2241,48 @@
                 'description': 'This is a test description.',
                 'enum': ['GT', 'LT', 'GE', 'LE', 'ML', 'MO', 'RE'],
             }
         },
     }
 
 
+def test_tuple_with_extra_schema():
+    class MyTuple(Tuple[int, str]):
+        @classmethod
+        def __get_pydantic_core_schema__(cls, _source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
+            return core_schema.tuple_positional_schema(
+                [core_schema.int_schema(), core_schema.str_schema()], extra_schema=core_schema.int_schema()
+            )
+
+    class Model(BaseModel):
+        x: MyTuple
+
+    assert Model.model_json_schema() == {
+        'properties': {
+            'x': {
+                'items': {'type': 'integer'},
+                'minItems': 2,
+                'prefixItems': [{'type': 'integer'}, {'type': 'string'}],
+                'title': 'X',
+                'type': 'array',
+            }
+        },
+        'required': ['x'],
+        'title': 'Model',
+        'type': 'object',
+    }
+
+
 def test_path_modify_schema():
     class MyPath(Path):
         @classmethod
+        def __get_pydantic_core_schema__(cls, _source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
+            return handler.generate_schema(Path)
+
+        @classmethod
         def __get_pydantic_json_schema__(
             cls, core_schema: core_schema.CoreSchema, handler: GetJsonSchemaHandler
         ) -> JsonSchemaValue:
             schema = handler(core_schema)
             schema.update(foobar=123)
             return schema
 
@@ -2201,25 +2377,54 @@
 
 
 class NestedModel(BaseModel):
     c: float
         """
     )
 
-    models = [module.ModelOne, module.ModelTwo, module.NestedModel]
-    model_names = set(models_json_schema(models)['$defs'].keys())
+    # All validation
+    keys_map, schema = models_json_schema(
+        [(module.ModelOne, 'validation'), (module.ModelTwo, 'validation'), (module.NestedModel, 'validation')]
+    )
+    model_names = set(schema['$defs'].keys())
     expected_model_names = {
         'ModelOne',
         'ModelTwo',
         f'{module.__name__}__ModelOne__NestedModel',
         f'{module.__name__}__ModelTwo__NestedModel',
         f'{module.__name__}__NestedModel',
     }
     assert model_names == expected_model_names
 
+    # Validation + serialization
+    keys_map, schema = models_json_schema(
+        [
+            (module.ModelOne, 'validation'),
+            (module.ModelTwo, 'validation'),
+            (module.NestedModel, 'validation'),
+            (module.ModelOne, 'serialization'),
+            (module.ModelTwo, 'serialization'),
+            (module.NestedModel, 'serialization'),
+        ]
+    )
+    model_names = set(schema['$defs'].keys())
+    expected_model_names = {
+        'ModelOneInput',
+        'ModelOneOutput',
+        'ModelTwoInput',
+        'ModelTwoOutput',
+        f'{module.__name__}__ModelOne__NestedModelInput',
+        f'{module.__name__}__ModelOne__NestedModelOutput',
+        f'{module.__name__}__ModelTwo__NestedModelInput',
+        f'{module.__name__}__ModelTwo__NestedModelOutput',
+        f'{module.__name__}__NestedModelInput',
+        f'{module.__name__}__NestedModelOutput',
+    }
+    assert model_names == expected_model_names
+
 
 def test_multiple_enums_with_same_name(create_module):
     module_1 = create_module(
         # language=Python
         """
 from enum import Enum
 
@@ -2284,19 +2489,19 @@
         def validate(cls, v: Any):
             return v
 
         @classmethod
         def __get_pydantic_core_schema__(
             cls,
             source: Any,
-            handler: Callable[[Any], core_schema.CoreSchema],
+            handler: GetCoreSchemaHandler,
         ) -> core_schema.PlainValidatorFunctionSchema:
             source_args = getattr(source, '__args__', [Any])
             param = source_args[0]
-            metadata = build_metadata_dict(js_functions=[lambda _c, h: h(handler(param))])
+            metadata = build_metadata_dict(js_functions=[lambda _c, h: h(handler.generate_schema(param))])
             return core_schema.general_plain_validator_function(
                 GenModel,
                 metadata=metadata,
             )
 
     class Model(BaseModel):
         data: GenModel[str]
@@ -2365,14 +2570,45 @@
                 'minItems': 2,
                 'maxItems': 2,
             }
         },
     }
 
 
+def test_namedtuple_modify_schema():
+    class Coordinates(NamedTuple):
+        x: float
+        y: float
+
+    class CustomCoordinates(Coordinates):
+        @classmethod
+        def __get_pydantic_core_schema__(cls, source: Any, handler: GetCoreSchemaHandler) -> core_schema.CoreSchema:
+            schema = handler(source)
+            schema['arguments_schema']['metadata']['pydantic_js_prefer_positional_arguments'] = False
+            return schema
+
+    class Location(BaseModel):
+        coords: CustomCoordinates = CustomCoordinates(34, 42)
+
+    assert Location.model_json_schema() == {
+        'properties': {
+            'coords': {
+                'additionalProperties': False,
+                'properties': {'x': {'title': 'X', 'type': 'number'}, 'y': {'title': 'Y', 'type': 'number'}},
+                'required': ['x', 'y'],
+                'title': 'Coords',
+                'type': 'object',
+                'default': [34, 42],
+            }
+        },
+        'title': 'Location',
+        'type': 'object',
+    }
+
+
 def test_advanced_generic_schema():  # noqa: C901
     T = TypeVar('T')
     K = TypeVar('K')
 
     class Gen(Generic[T]):
         def __init__(self, data: Any):
             self.data = data
@@ -2382,23 +2618,21 @@
             yield cls.validate
 
         @classmethod
         def validate(cls, v: Any):
             return v
 
         @classmethod
-        def __get_pydantic_core_schema__(
-            cls, source: Any, handler: Callable[[Any], core_schema.CoreSchema]
-        ) -> core_schema.CoreSchema:
+        def __get_pydantic_core_schema__(cls, source: Any, handler: GetCoreSchemaHandler) -> core_schema.CoreSchema:
             if hasattr(source, '__args__'):
                 arg = source.__args__[0]
 
                 def js_func(s, h):
                     # ignore the schema we were given and get a new CoreSchema
-                    s = handler(Optional[arg])
+                    s = handler.generate_schema(Optional[arg])
                     return h(s)
 
                 return core_schema.general_plain_validator_function(
                     Gen,
                     metadata={'pydantic_js_functions': [js_func]},
                 )
             else:
@@ -2654,14 +2888,44 @@
         },
         'required': ['my_field'],
         'title': 'MyModel',
         'type': 'object',
     }
 
 
+def test_remove_anyof_redundancy() -> None:
+    class A:
+        @classmethod
+        def __get_pydantic_json_schema__(
+            cls, core_schema: core_schema.CoreSchema, handler: GetJsonSchemaHandler
+        ) -> JsonSchemaValue:
+            return handler({'type': 'str'})
+
+    class B:
+        @classmethod
+        def __get_pydantic_json_schema__(
+            cls, core_schema: core_schema.CoreSchema, handler: GetJsonSchemaHandler
+        ) -> JsonSchemaValue:
+            return handler({'type': 'str'})
+
+    class MyModel(BaseModel):
+        model_config = ConfigDict(arbitrary_types_allowed=True)
+
+        # Union of two objects should give a JSON with an `anyOf` field, but in this case
+        # since the fields are the same, the `anyOf` is removed.
+        field: Union[A, B]
+
+    assert MyModel.model_json_schema() == {
+        'properties': {'field': {'title': 'Field', 'type': 'string'}},
+        'required': ['field'],
+        'title': 'MyModel',
+        'type': 'object',
+    }
+
+
 def test_discriminated_union():
     class Cat(BaseModel):
         pet_type: Literal['cat']
 
     class Dog(BaseModel):
         pet_type: Literal['dog']
 
@@ -3436,41 +3700,72 @@
         },
         'required': ['password'],
     }
 
 
 def test_override_generate_json_schema():
     class MyGenerateJsonSchema(GenerateJsonSchema):
-        def generate(self, schema):
-            json_schema = super().generate(schema)
+        def generate(self, schema, mode='validation'):
+            json_schema = super().generate(schema, mode=mode)
             json_schema['$schema'] = self.schema_dialect
             return json_schema
 
     class MyBaseModel(BaseModel):
         @classmethod
         def model_json_schema(
             cls,
             by_alias: bool = True,
             ref_template: str = DEFAULT_REF_TEMPLATE,
             schema_generator: Type[GenerateJsonSchema] = MyGenerateJsonSchema,
+            mode='validation',
         ) -> Dict[str, Any]:
-            return super().model_json_schema(by_alias, ref_template, schema_generator)
+            return super().model_json_schema(by_alias, ref_template, schema_generator, mode)
 
     class MyModel(MyBaseModel):
         x: int
 
     assert MyModel.model_json_schema() == {
         '$schema': 'https://json-schema.org/draft/2020-12/schema',
         'properties': {'x': {'title': 'X', 'type': 'integer'}},
         'required': ['x'],
         'title': 'MyModel',
         'type': 'object',
     }
 
 
+def test_generate_json_schema_generate_twice():
+    generator = GenerateJsonSchema()
+
+    class Model(BaseModel):
+        title: str
+
+    generator.generate(Model.__pydantic_core_schema__)
+
+    with pytest.raises(
+        PydanticUserError,
+        match=re.escape(
+            'This JSON schema generator has already been used to generate a JSON schema. '
+            'You must create a new instance of GenerateJsonSchema to generate a new JSON schema.'
+        ),
+    ):
+        generator.generate(Model.__pydantic_core_schema__)
+
+    generator = GenerateJsonSchema()
+    generator.generate_definitions([(Model, 'validation', Model.__pydantic_core_schema__)])
+
+    with pytest.raises(
+        PydanticUserError,
+        match=re.escape(
+            'This JSON schema generator has already been used to generate a JSON schema. '
+            'You must create a new instance of GenerateJsonSchema to generate a new JSON schema.'
+        ),
+    ):
+        generator.generate_definitions([(Model, 'validation', Model.__pydantic_core_schema__)])
+
+
 def test_nested_default_json_schema():
     class InnerModel(BaseModel):
         foo: str = 'bar'
         baz: str = Field(default='foobar', alias='my_alias')
 
     class OuterModel(BaseModel):
         nested_field: InnerModel = InnerModel()
@@ -3632,14 +3927,28 @@
             return json_schema
 
     TypeAdapter(Annotated[CustomType, 123]).json_schema()
 
     assert sum(calls) == 1
 
 
+def test_model_with_strict_mode():
+    class Model(BaseModel):
+        model_config = ConfigDict(strict=True)
+
+        a: str
+
+    assert Model.model_json_schema() == {
+        'properties': {'a': {'title': 'A', 'type': 'string'}},
+        'required': ['a'],
+        'title': 'Model',
+        'type': 'object',
+    }
+
+
 def test_model_with_schema_extra():
     class Model(BaseModel):
         a: str
 
         model_config = dict(json_schema_extra={'examples': [{'a': 'Foo'}]})
 
     assert Model.model_json_schema() == {
@@ -3738,7 +4047,403 @@
             class Config:
                 def json_schema_extra(schema, model_class):
                     schema.pop('properties')
                     schema['type'] = 'override'
                     assert model_class is Model
 
         assert Model.model_json_schema() == {'title': 'Model', 'type': 'override'}
+
+
+def test_serialization_validation_interaction():
+    class Inner(BaseModel):
+        x: Json[int]
+
+    class Outer(BaseModel):
+        inner: Inner
+
+    _, v_schema = models_json_schema([(Outer, 'validation')])
+    assert v_schema == {
+        '$defs': {
+            'Inner': {
+                'properties': {'x': {'format': 'json-string', 'title': 'X', 'type': 'string'}},
+                'required': ['x'],
+                'title': 'Inner',
+                'type': 'object',
+            },
+            'Outer': {
+                'properties': {'inner': {'$ref': '#/$defs/Inner'}},
+                'required': ['inner'],
+                'title': 'Outer',
+                'type': 'object',
+            },
+        }
+    }
+
+    _, s_schema = models_json_schema([(Outer, 'serialization')])
+    assert s_schema == {
+        '$defs': {
+            'Inner': {
+                'properties': {'x': {'title': 'X', 'type': 'integer'}},
+                'required': ['x'],
+                'title': 'Inner',
+                'type': 'object',
+            },
+            'Outer': {
+                'properties': {'inner': {'$ref': '#/$defs/Inner'}},
+                'required': ['inner'],
+                'title': 'Outer',
+                'type': 'object',
+            },
+        }
+    }
+
+    _, vs_schema = models_json_schema([(Outer, 'validation'), (Outer, 'serialization')])
+    assert vs_schema == {
+        '$defs': {
+            'InnerInput': {
+                'properties': {'x': {'format': 'json-string', 'title': 'X', 'type': 'string'}},
+                'required': ['x'],
+                'title': 'Inner',
+                'type': 'object',
+            },
+            'InnerOutput': {
+                'properties': {'x': {'title': 'X', 'type': 'integer'}},
+                'required': ['x'],
+                'title': 'Inner',
+                'type': 'object',
+            },
+            'OuterInput': {
+                'properties': {'inner': {'$ref': '#/$defs/InnerInput'}},
+                'required': ['inner'],
+                'title': 'Outer',
+                'type': 'object',
+            },
+            'OuterOutput': {
+                'properties': {'inner': {'$ref': '#/$defs/InnerOutput'}},
+                'required': ['inner'],
+                'title': 'Outer',
+                'type': 'object',
+            },
+        }
+    }
+
+
+def test_computed_field():
+    class Model(BaseModel):
+        x: int
+
+        @computed_field
+        @property
+        def double_x(self) -> int:
+            return 2 * self.x
+
+    assert Model.model_json_schema(mode='validation') == {
+        'properties': {'x': {'title': 'X', 'type': 'integer'}},
+        'required': ['x'],
+        'title': 'Model',
+        'type': 'object',
+    }
+    assert Model.model_json_schema(mode='serialization') == {
+        'properties': {'double_x': {'title': 'Double X', 'type': 'integer'}, 'x': {'title': 'X', 'type': 'integer'}},
+        'required': ['x', 'double_x'],
+        'title': 'Model',
+        'type': 'object',
+    }
+
+
+def test_serialization_schema_with_exclude():
+    class MyGenerateJsonSchema(GenerateJsonSchema):
+        def field_is_present(self, field) -> bool:
+            # Always include fields in the JSON schema, even if excluded from serialization
+            return True
+
+    class Model(BaseModel):
+        x: int
+        y: int = Field(exclude=True)
+
+    assert Model(x=1, y=1).model_dump() == {'x': 1}
+
+    assert Model.model_json_schema(mode='serialization') == {
+        'properties': {'x': {'title': 'X', 'type': 'integer'}},
+        'required': ['x'],
+        'title': 'Model',
+        'type': 'object',
+    }
+    assert Model.model_json_schema(mode='serialization', schema_generator=MyGenerateJsonSchema) == {
+        'properties': {'x': {'title': 'X', 'type': 'integer'}, 'y': {'title': 'Y', 'type': 'integer'}},
+        'required': ['x'],
+        'title': 'Model',
+        'type': 'object',
+    }
+
+
+@pytest.mark.parametrize('mapping_type', [typing.Dict, typing.Mapping])
+def test_mappings_str_int_json_schema(mapping_type: Any):
+    class Model(BaseModel):
+        str_int_map: mapping_type[str, int]
+
+    assert Model.model_json_schema() == {
+        'title': 'Model',
+        'type': 'object',
+        'properties': {
+            'str_int_map': {
+                'title': 'Str Int Map',
+                'type': 'object',
+                'additionalProperties': {'type': 'integer'},
+            }
+        },
+        'required': ['str_int_map'],
+    }
+
+
+@pytest.mark.parametrize(('sequence_type'), [pytest.param(List), pytest.param(Sequence)])
+def test_sequence_schema(sequence_type):
+    class Model(BaseModel):
+        field: sequence_type[int]
+
+    assert Model.model_json_schema() == {
+        'properties': {
+            'field': {'items': {'type': 'integer'}, 'title': 'Field', 'type': 'array'},
+        },
+        'required': ['field'],
+        'title': 'Model',
+        'type': 'object',
+    }
+
+
+@pytest.mark.parametrize(('sequence_type',), [pytest.param(List), pytest.param(Sequence)])
+def test_sequences_int_json_schema(sequence_type):
+    class Model(BaseModel):
+        int_seq: sequence_type[int]
+
+    assert Model.model_json_schema() == {
+        'title': 'Model',
+        'type': 'object',
+        'properties': {
+            'int_seq': {
+                'title': 'Int Seq',
+                'type': 'array',
+                'items': {'type': 'integer'},
+            },
+        },
+        'required': ['int_seq'],
+    }
+    assert Model.model_validate_json('{"int_seq": [1, 2, 3]}')
+
+
+@pytest.mark.parametrize(
+    'field_schema,model_schema',
+    [
+        (None, {'properties': {}, 'title': 'Model', 'type': 'object'}),
+        (
+            {'a': 'b'},
+            {'properties': {'x': {'a': 'b', 'title': 'X'}}, 'required': ['x'], 'title': 'Model', 'type': 'object'},
+        ),
+    ],
+)
+@pytest.mark.parametrize('instance_of', [True, False])
+def test_arbitrary_type_json_schema(field_schema, model_schema, instance_of):
+    class ArbitraryClass:
+        pass
+
+    if instance_of:
+
+        class Model(BaseModel):
+            x: Annotated[InstanceOf[ArbitraryClass], WithJsonSchema(field_schema)]
+
+    else:
+
+        class Model(BaseModel):
+            model_config = dict(arbitrary_types_allowed=True)
+
+            x: Annotated[ArbitraryClass, WithJsonSchema(field_schema)]
+
+    assert Model.model_json_schema() == model_schema
+
+
+def test_root_model():
+    class A(RootModel[int]):
+        pass
+
+    assert A.model_json_schema() == {'type': 'integer'}
+
+    class B(RootModel[A]):
+        pass
+
+    assert B.model_json_schema() == {'type': 'integer'}
+
+
+def test_get_json_schema_is_passed_the_same_schema_handler_was_called_with() -> None:
+    class CustomInt(int):
+        @classmethod
+        def __get_pydantic_core_schema__(cls, _source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
+            return handler(int)
+
+        @classmethod
+        def __get_pydantic_json_schema__(
+            cls, core_schema: CoreSchema, handler: GetJsonSchemaHandler
+        ) -> JsonSchemaValue:
+            assert core_schema['type'] == 'function-after'
+            inner = core_schema['schema']
+            assert inner['type'] == 'int'
+            inner = inner.copy()
+            inner['gt'] = 0
+            core_schema = {**core_schema, 'schema': inner}
+            return handler(core_schema)
+
+    class Marker:
+        def __get_pydantic_core_schema__(self, source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
+            return core_schema.no_info_after_validator_function(lambda x: x, handler(source_type))
+
+        def __get_pydantic_json_schema__(
+            self, core_schema: CoreSchema, handler: GetJsonSchemaHandler
+        ) -> JsonSchemaValue:
+            return handler(core_schema)
+
+    js_schema = TypeAdapter(Annotated[CustomInt, Marker()]).json_schema()
+
+    # insert_assert(js_schema)
+    assert js_schema == {'type': 'integer', 'exclusiveMinimum': 0}
+
+
+def test_get_json_schema_gets_called_if_schema_is_replaced() -> None:
+    class CustomInt(int):
+        @classmethod
+        def __get_pydantic_core_schema__(cls, _source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
+            return handler(int)
+
+        @classmethod
+        def __get_pydantic_json_schema__(
+            cls, core_schema: CoreSchema, handler: GetJsonSchemaHandler
+        ) -> JsonSchemaValue:
+            assert core_schema['type'] == 'str'
+            core_schema = {**core_schema, 'min_length': 1}
+            return handler(core_schema)
+
+    class Marker:
+        def __get_pydantic_core_schema__(self, source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
+            return core_schema.no_info_after_validator_function(lambda x: x, handler(source_type))
+
+        def __get_pydantic_json_schema__(
+            self, _core_schema: CoreSchema, handler: GetJsonSchemaHandler
+        ) -> JsonSchemaValue:
+            return handler({'type': 'str'})
+
+    js_schema = TypeAdapter(Annotated[CustomInt, Marker()]).json_schema()
+
+    # insert_assert(js_schema)
+    assert js_schema == {'type': 'string', 'minLength': 1}
+
+
+def test_core_metadata_core_schema_metadata():
+    with pytest.raises(TypeError, match=re.escape("CoreSchema metadata should be a dict; got 'test'.")):
+        CoreMetadataHandler({'metadata': 'test'})
+
+    core_metadata_handler = CoreMetadataHandler({})
+    core_metadata_handler._schema = {}
+    assert core_metadata_handler.metadata == {}
+    core_metadata_handler._schema = {'metadata': 'test'}
+    with pytest.raises(TypeError, match=re.escape("CoreSchema metadata should be a dict; got 'test'.")):
+        core_metadata_handler.metadata
+
+
+def test_build_metadata_dict_initial_metadata():
+    assert build_metadata_dict(initial_metadata={'foo': 'bar'}) == {'foo': 'bar', 'pydantic_js_functions': []}
+
+    with pytest.raises(TypeError, match=re.escape("CoreSchema metadata should be a dict; got 'test'.")):
+        build_metadata_dict(initial_metadata='test')
+
+
+def test_core_metadata_get_json_schema():
+    core_metadata_handler = CoreMetadataHandler({})
+    assert core_metadata_handler.get_json_schema({}, lambda c: c) == {}
+
+    core_metadata_handler = CoreMetadataHandler(
+        {'metadata': {'pydantic_js_function': lambda c, h: f'schema = {c}, {h.__name__}'}}
+    )
+    assert core_metadata_handler.get_json_schema({'foo': 'bar'}, lambda c: c) == "schema = {'foo': 'bar'}, <lambda>"
+
+
+def test_type_adapter_json_schemas_title_description():
+    class Model(BaseModel):
+        a: str
+
+    _, json_schema = TypeAdapter.json_schemas([(Model, 'validation', TypeAdapter(Model))])
+    assert 'title' not in json_schema
+    assert 'description' not in json_schema
+
+    _, json_schema = TypeAdapter.json_schemas(
+        [(Model, 'validation', TypeAdapter(Model))],
+        title='test title',
+        description='test description',
+    )
+    assert json_schema['title'] == 'test title'
+    assert json_schema['description'] == 'test description'
+
+
+def test_type_adapter_json_schemas_without_definitions():
+    _, json_schema = TypeAdapter.json_schemas(
+        [(int, 'validation', TypeAdapter(int))],
+        ref_template='#/components/schemas/{model}',
+    )
+
+    assert 'definitions' not in json_schema
+
+
+def test_custom_chain_schema():
+    class MySequence:
+        @classmethod
+        def __get_pydantic_core_schema__(cls, source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
+            list_schema = core_schema.list_schema()
+            return core_schema.chain_schema([list_schema])
+
+    class Model(BaseModel):
+        model_config = ConfigDict(arbitrary_types_allowed=True)
+
+        a: MySequence
+
+    assert Model.model_json_schema() == {
+        'properties': {'a': {'items': {}, 'title': 'A', 'type': 'array'}},
+        'required': ['a'],
+        'title': 'Model',
+        'type': 'object',
+    }
+
+
+def test_json_or_python_schema():
+    class MyJsonOrPython:
+        @classmethod
+        def __get_pydantic_core_schema__(cls, source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
+            int_schema = core_schema.int_schema()
+            return core_schema.json_or_python_schema(json_schema=int_schema, python_schema=int_schema)
+
+    class Model(BaseModel):
+        model_config = ConfigDict(arbitrary_types_allowed=True)
+
+        a: MyJsonOrPython
+
+    assert Model.model_json_schema() == {
+        'properties': {'a': {'title': 'A', 'type': 'integer'}},
+        'required': ['a'],
+        'title': 'Model',
+        'type': 'object',
+    }
+
+
+def test_lax_or_strict_schema():
+    class MyLaxOrStrict:
+        @classmethod
+        def __get_pydantic_core_schema__(cls, source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
+            int_schema = core_schema.int_schema()
+            return core_schema.lax_or_strict_schema(lax_schema=int_schema, strict_schema=int_schema, strict=True)
+
+    class Model(BaseModel):
+        model_config = ConfigDict(arbitrary_types_allowed=True)
+
+        a: MyLaxOrStrict
+
+    assert Model.model_json_schema() == {
+        'properties': {'a': {'title': 'A', 'type': 'integer'}},
+        'required': ['a'],
+        'title': 'Model',
+        'type': 'object',
+    }
```

### Comparing `pydantic-2.0a4/tests/test_main.py` & `pydantic-2.0b1/tests/test_main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 import json
 import platform
 import re
 import sys
-from collections import defaultdict
 from copy import deepcopy
 from enum import Enum
 from typing import (
     Any,
     Callable,
     ClassVar,
-    Counter,
-    DefaultDict,
     Dict,
     Generic,
     List,
     Mapping,
     Optional,
     Set,
     Type,
     TypeVar,
     get_type_hints,
 )
 from uuid import UUID, uuid4
 
 import pytest
+from pydantic_core import CoreSchema
 from typing_extensions import Annotated, Final, Literal
 
 from pydantic import (
     BaseModel,
     ConfigDict,
     Field,
+    GetCoreSchemaHandler,
     PrivateAttr,
     PydanticUndefinedAnnotation,
     PydanticUserError,
     SecretStr,
     ValidationError,
     ValidationInfo,
     constr,
+    field_validator,
 )
-from pydantic.decorators import field_validator
 
 
 def test_success():
     # same as below but defined here so class definition occurs inside the test
     class Model(BaseModel):
         a: float
         b: int = 10
@@ -346,14 +345,39 @@
 
     model = Model(a=1, b='2', c=3.0, d=4)
     assert repr(model) == "Model(a=1, b='2', c=3.0, d=4)"
     assert str(model.model_dump()) == "{'a': 1, 'b': '2', 'c': 3.0, 'd': 4}"
     assert str(model.model_dump_json()) == '{"a":1,"b":"2","c":3.0,"d":4}'
 
 
+def test_extra_broken_via_pydantic_extra_interference():
+    """
+    At the time of writing this test there is `_model_construction.model_extra_getattr` being assigned to model's
+    `__getattr__`. The method then expects `BaseModel.__pydantic_extra__` isn't `None`. Both this actions happen when
+    `model_config.extra` is set to `True`. However, this behavior could be accidentally broken in a subclass of
+    `BaseModel`. In that case `AttributeError` should be thrown when `__getattr__` is being accessed essentially
+    disabling the `extra` functionality.
+    """
+
+    class BrokenExtraBaseModel(BaseModel):
+        def model_post_init(self, __context: Any) -> None:
+            super().model_post_init(__context)
+            object.__setattr__(self, '__pydantic_extra__', None)
+
+    class Model(BrokenExtraBaseModel):
+        model_config = ConfigDict(extra='allow')
+
+    m = Model(extra_field='some extra value')
+
+    with pytest.raises(AttributeError) as e:
+        m.extra_field
+
+    assert e.value.args == ("'Model' object has no attribute 'extra_field'",)
+
+
 def test_set_attr(UltraSimpleModel):
     m = UltraSimpleModel(a=10.2)
     assert m.model_dump() == {'a': 10.2, 'b': 10}
 
     m.b = 20
     assert m.model_dump() == {'a': 10.2, 'b': 20}
 
@@ -439,17 +463,19 @@
         model_config = ConfigDict(extra='forbid', frozen=True)
 
         a: int = 10
 
     m = FrozenModel()
 
     assert m.a == 10
-    with pytest.raises(TypeError) as exc_info:
+    with pytest.raises(ValidationError) as exc_info:
         m.a = 11
-    assert '"FrozenModel" is frozen and does not support item assignment' in exc_info.value.args[0]
+    assert exc_info.value.errors(include_url=False) == [
+        {'type': 'frozen_instance', 'loc': ('a',), 'msg': 'Instance is frozen', 'input': 11}
+    ]
 
 
 def test_not_frozen_are_not_hashable():
     class TestModel(BaseModel):
         a: int = 10
 
     m = TestModel()
@@ -1004,17 +1030,17 @@
             {'foos': {1, '__all__'}},
             {'c': 3, 'foos': []},
             None,
             id='using "__all__" and other items should get merged together, still excluding all list items',
         ),
         pytest.param(
             {'foos': {-1: {'b'}}},
-            {'c': 3, 'foos': [{'a': 1, 'b': 2}, {'a': 3, 'b': 4}]},
+            {'c': 3, 'foos': [{'a': 1, 'b': 2}, {'a': 3}]},
             None,
-            id='negative indexes are ignored',
+            id='negative indexes',
         ),
     ],
 )
 def test_model_export_nested_list(exclude, expected, raises_match):
     class Foo(BaseModel):
         a: int = 1
         b: int = 2
@@ -1375,16 +1401,14 @@
     assert m.model_dump() == {'field': {'field': {'field': None}}}
 
 
 def test_recursive_cycle_with_repeated_field():
     class A(BaseModel):
         b: 'B'
 
-        model_config = {'undefined_types_warning': False}
-
     class B(BaseModel):
         a1: Optional[A] = None
         a2: Optional[A] = None
 
     A.model_rebuild()
 
     assert A.model_validate({'b': {'a1': {'b': {'a1': None}}}}) == A(b=B(a1=A(b=B(a1=None))))
@@ -1583,57 +1607,33 @@
     item = Item(images={image_1, image_2})
     assert image_1 in item.images
 
     assert id(image_1) in {id(image) for image in item.images}
     assert id(image_2) in {id(image) for image in item.images}
 
 
-def test_mapping_retains_type_subclass():
+def test_mapping_subclass_as_input():
     class CustomMap(dict):
         pass
 
     class Model(BaseModel):
-        x: Mapping[str, Mapping[str, int]]
-
-    m = Model(x=CustomMap(outer=CustomMap(inner=42)))
-    assert isinstance(m.x, CustomMap)
-    assert isinstance(m.x['outer'], CustomMap)
-    assert m.x['outer']['inner'] == 42
-
-
-def test_mapping_retains_type_defaultdict():
-    class Model(BaseModel):
-        x: Mapping[str, int]
-
-    d = defaultdict(int)
-    d['foo'] = '2'
-    d['bar']
-
-    m = Model(x=d)
-    assert isinstance(m.x, defaultdict)
-    assert m.x['foo'] == 2
-    assert m.x['bar'] == 0
-
-
-def test_mapping_retains_type_fallback_error():
-    class CustomMap(dict):
-        def __init__(self, *args, **kwargs):
-            if args or kwargs:
-                raise TypeError('test')
-            super().__init__(*args, **kwargs)
-
-    class Model(BaseModel):
         x: Mapping[str, int]
 
     d = CustomMap()
     d['one'] = 1
     d['two'] = 2
 
-    with pytest.raises(TypeError, match='test'):
-        Model(x=d)
+    v = Model(x=d).x
+    # we don't promise that this will or will not be a CustomMap
+    # all we promise is that it _will_ be a mapping
+    assert isinstance(v, Mapping)
+    # but the current behavior is that it will be a dict, not a CustomMap
+    # so document that here
+    assert not isinstance(v, CustomMap)
+    assert v == {'one': 1, 'two': 2}
 
 
 def test_typing_coercion_dict():
     class Model(BaseModel):
         x: Dict[str, int]
 
     m = Model(x={'one': 1, 'two': 2})
@@ -1645,67 +1645,14 @@
 
 
 class MyDict(Dict[KT, VT]):
     def __repr__(self):
         return f'MyDict({super().__repr__()})'
 
 
-def test_dict_subclasses_bare():
-    class Model(BaseModel):
-        a: MyDict
-
-    assert repr(Model(a=MyDict({'a': 1})).a) == "MyDict({'a': 1})"
-    assert repr(Model(a=MyDict({b'x': (1, 2)})).a) == "MyDict({b'x': (1, 2)})"
-
-
-def test_dict_subclasses_typed():
-    class Model(BaseModel):
-        a: MyDict[str, int]
-
-    assert repr(Model(a=MyDict({'a': 1})).a) == "MyDict({'a': 1})"
-
-
-def test_typing_coercion_defaultdict():
-    class Model(BaseModel):
-        x: DefaultDict[int, str]
-
-    d = defaultdict(str)
-    d['1']
-    m = Model(x=d)
-    assert isinstance(m.x, defaultdict)
-    assert repr(m.x) == "defaultdict(<class 'str'>, {1: ''})"
-
-
-def test_typing_coercion_counter():
-    class Model(BaseModel):
-        x: Counter[str]
-
-    m = Model(x={'a': 10})
-    assert isinstance(m.x, Counter)
-    assert repr(m.x) == "Counter({'a': 10})"
-
-
-def test_typing_counter_value_validation():
-    class Model(BaseModel):
-        x: Counter[str]
-
-    with pytest.raises(ValidationError) as exc_info:
-        Model(x={'a': 'a'})
-
-    # insert_assert(exc_info.value.errors(include_url=False))
-    assert exc_info.value.errors(include_url=False) == [
-        {
-            'type': 'int_parsing',
-            'loc': ('x', 'a'),
-            'msg': 'Input should be a valid integer, unable to parse string as an integer',
-            'input': 'a',
-        }
-    ]
-
-
 def test_class_kwargs_config():
     class Base(BaseModel, extra='forbid', alias_generator=str.upper):
         a: int
 
     assert Base.model_config['extra'] == 'forbid'
     assert Base.model_config['alias_generator'] is str.upper
     # assert Base.model_fields['a'].alias == 'A'
@@ -1912,45 +1859,45 @@
         assert calls == ['WithOverrideModel.model_post_init', 'WithOverrideModel.model_post_init']
 
     finally:
         BaseModel.model_post_init = original_base_model_post_init
 
 
 def test_deeper_recursive_model():
-    class A(BaseModel, undefined_types_warning=False):
+    class A(BaseModel):
         b: 'B'
 
-    class B(BaseModel, undefined_types_warning=False):
+    class B(BaseModel):
         c: 'C'
 
-    class C(BaseModel, undefined_types_warning=False):
+    class C(BaseModel):
         a: Optional['A']
 
     A.model_rebuild()
     B.model_rebuild()
     C.model_rebuild()
 
     m = A(b=B(c=C(a=None)))
     assert m.model_dump() == {'b': {'c': {'a': None}}}
 
 
 def test_model_rebuild_localns():
-    class A(BaseModel, undefined_types_warning=False):
+    class A(BaseModel):
         x: int
 
-    class B(BaseModel, undefined_types_warning=False):
+    class B(BaseModel):
         a: 'Model'  # noqa F821
 
     B.model_rebuild(_types_namespace={'Model': A})
 
     m = B(a={'x': 1})
     assert m.model_dump() == {'a': {'x': 1}}
     assert isinstance(m.a, A)
 
-    class C(BaseModel, undefined_types_warning=False):
+    class C(BaseModel):
         a: 'Model'  # noqa F821
 
     with pytest.raises(PydanticUndefinedAnnotation, match="name 'Model' is not defined"):
         C.model_rebuild(_types_namespace={'A': A})
 
 
 @pytest.fixture(scope='session', name='InnerEqualityModel')
@@ -2036,14 +1983,43 @@
     assert m2 == m2_equal
 
     m3_equal = m.model_copy()
     m3_equal._iz = 1
     assert m3 == m3_equal
 
 
+def test_model_copy_extra():
+    class Model(BaseModel, extra='allow'):
+        x: int
+
+    m = Model(x=1, y=2)
+    assert m.model_dump() == {'x': 1, 'y': 2}
+    assert m.model_extra == {'y': 2}
+    m2 = m.model_copy()
+    assert m2.model_dump() == {'x': 1, 'y': 2}
+    assert m2.model_extra == {'y': 2}
+
+    m3 = m.model_copy(update={'x': 4, 'z': 3})
+    assert m3.model_dump() == {'x': 4, 'y': 2, 'z': 3}
+    assert m3.model_extra == {'y': 2, 'z': 3}
+
+    m3.__pydantic_extra__ = None
+    m4 = m.model_copy(update={'x': 4, 'z': 3})
+    assert m4.model_dump() == {'x': 4, 'y': 2, 'z': 3}
+    assert m4.model_extra == {'y': 2, 'z': 3}
+
+
+def test_model_parametrized_name_not_generic():
+    class Model(BaseModel):
+        x: int
+
+    with pytest.raises(TypeError, match='Concrete names should only be generated for generic models.'):
+        Model.model_parametrized_name(())
+
+
 def test_model_equality_generics():
     T = TypeVar('T')
 
     class GenericModel(BaseModel, Generic[T]):
         x: T
 
     class ConcreteModel(BaseModel):
@@ -2083,40 +2059,31 @@
 
         model_config = ConfigDict(strict=True)
 
     assert LaxModel.model_validate({'x': '1'}, strict=None) == LaxModel(x=1)
     assert LaxModel.model_validate({'x': '1'}, strict=False) == LaxModel(x=1)
     with pytest.raises(ValidationError) as exc_info:
         LaxModel.model_validate({'x': '1'}, strict=True)
+    # there's no such thing on the model itself
+    # insert_assert(exc_info.value.errors(include_url=False))
     assert exc_info.value.errors(include_url=False) == [
-        {
-            'type': 'model_class_type',
-            'loc': (),
-            'msg': 'Input should be an instance of LaxModel',
-            'input': {'x': '1'},
-            'ctx': {'class_name': 'LaxModel'},
-        }
+        {'type': 'int_type', 'loc': ('x',), 'msg': 'Input should be a valid integer', 'input': '1'}
     ]
 
     with pytest.raises(ValidationError) as exc_info:
         StrictModel.model_validate({'x': '1'})
     assert exc_info.value.errors(include_url=False) == [
         {'type': 'int_type', 'loc': ('x',), 'msg': 'Input should be a valid integer', 'input': '1'}
     ]
     assert StrictModel.model_validate({'x': '1'}, strict=False) == StrictModel(x=1)
     with pytest.raises(ValidationError) as exc_info:
         LaxModel.model_validate({'x': '1'}, strict=True)
+    # insert_assert(exc_info.value.errors(include_url=False))
     assert exc_info.value.errors(include_url=False) == [
-        {
-            'type': 'model_class_type',
-            'loc': (),
-            'msg': 'Input should be an instance of LaxModel',
-            'input': {'x': '1'},
-            'ctx': {'class_name': 'LaxModel'},
-        }
+        {'type': 'int_type', 'loc': ('x',), 'msg': 'Input should be a valid integer', 'input': '1'}
     ]
 
 
 def test_model_validate_json_strict() -> None:
     class LaxModel(BaseModel):
         x: int
 
@@ -2216,16 +2183,103 @@
         inner: InnerModel
 
     assert OuterModel.model_validate({'inner': {'x': 2}}, context={'multiplier': 1}).inner.x == 2
     assert OuterModel.model_validate({'inner': {'x': 2}}, context={'multiplier': 2}).inner.x == 4
     assert OuterModel.model_validate({'inner': {'x': 2}}, context={'multiplier': 3}).inner.x == 6
 
 
+def test_extra_equality():
+    class MyModel(BaseModel, extra='allow'):
+        pass
+
+    assert MyModel(x=1) != MyModel()
+
+
 def test_equality_delegation():
     from unittest.mock import ANY
 
-    from pydantic import BaseModel
-
     class MyModel(BaseModel):
         foo: str
 
     assert MyModel(foo='bar') == ANY
+
+
+def test_recursion_loop_error():
+    class Model(BaseModel):
+        x: List['Model']
+
+    data = {'x': []}
+    data['x'].append(data)
+    with pytest.raises(ValidationError) as exc_info:
+        Model(**data)
+    assert repr(exc_info.value.errors(include_url=False)[0]) == (
+        "{'type': 'recursion_loop', 'loc': ('x', 0, 'x', 0), 'msg': "
+        "'Recursion error - cyclic reference detected', 'input': {'x': [{...}]}}"
+    )
+
+
+def test_protected_namespace_default():
+    with pytest.raises(NameError, match='Field "model_prefixed_field" has conflict with protected namespace "model_"'):
+
+        class Model(BaseModel):
+            model_prefixed_field: str
+
+
+def test_custom_protected_namespace():
+    with pytest.raises(NameError, match='Field "test_field" has conflict with protected namespace "test_"'):
+
+        class Model(BaseModel):
+            # this field won't raise error because we changed the default value for the
+            # `protected_namespaces` config.
+            model_prefixed_field: str
+            test_field: str
+
+            model_config = ConfigDict(protected_namespaces=('test_',))
+
+
+def test_multiple_protected_namespace():
+    with pytest.raises(
+        NameError, match='Field "also_protect_field" has conflict with protected namespace "also_protect_"'
+    ):
+
+        class Model(BaseModel):
+            also_protect_field: str
+
+            model_config = ConfigDict(protected_namespaces=('protect_me_', 'also_protect_'))
+
+
+def test_model_get_core_schema() -> None:
+    class Model(BaseModel):
+        @classmethod
+        def __get_pydantic_core_schema__(cls, source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
+            assert handler(int) == {'type': 'int'}
+            assert handler.generate_schema(int) == {'type': 'int'}
+            return handler(source_type)
+
+    Model()
+
+
+def test_nested_types_ignored():
+    from pydantic import BaseModel
+
+    class NonNestedType:
+        pass
+
+    # Defining a nested type does not error
+    class GoodModel(BaseModel):
+        class NestedType:
+            pass
+
+        # You can still store such types on the class by annotating as a ClassVar
+        MyType: ClassVar[Type[Any]] = NonNestedType
+
+        # For documentation: you _can_ give multiple names to a nested type and it won't error:
+        # It might be better if it did, but this seems to be rare enough that I'm not concerned
+        x = NestedType
+
+    assert GoodModel.MyType is NonNestedType
+    assert GoodModel.x is GoodModel.NestedType
+
+    with pytest.raises(PydanticUserError, match='A non-annotated attribute was detected'):
+
+        class BadModel(BaseModel):
+            x = NonNestedType
```

### Comparing `pydantic-2.0a4/tests/test_model_signature.py` & `pydantic-2.0b1/tests/test_model_signature.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import sys
 from inspect import Parameter, Signature, signature
-from typing import Any, Iterable, Optional, Union
+from typing import Any, Generic, Iterable, Optional, TypeVar, Union
 
 import pytest
 from typing_extensions import Annotated
 
 from pydantic import BaseModel, ConfigDict, Field, create_model
 from pydantic._internal._typing_extra import is_annotated
 
@@ -28,14 +28,26 @@
 
     sig = signature(Model)
     assert sig != signature(BaseModel)
     assert _equals(map(str, sig.parameters.values()), ('a: float', 'b: int = 10'))
     assert _equals(str(sig), '(*, a: float, b: int = 10) -> None')
 
 
+def test_generic_model_signature():
+    T = TypeVar('T')
+
+    class Model(BaseModel, Generic[T]):
+        a: T
+
+    sig = signature(Model[int])
+    assert sig != signature(BaseModel)
+    assert _equals(map(str, sig.parameters.values()), ('a: int',))
+    assert _equals(str(sig), '(*, a: int) -> None')
+
+
 def test_custom_init_signature():
     class MyModel(BaseModel):
         id: int
         name: str = 'John Doe'
         f__: str = Field(..., alias='foo')
 
         model_config = ConfigDict(extra='allow')
```

### Comparing `pydantic-2.0a4/tests/test_model_validator.py` & `pydantic-2.0b1/tests/test_model_validator.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from __future__ import annotations
 
 from pprint import pprint
-from typing import Any, Dict, cast
+from typing import Any, Dict, Union, cast
 
 import pytest
 
-from pydantic import BaseModel, ValidationInfo
-from pydantic.decorators import model_validator
+from pydantic import BaseModel, ValidationInfo, model_validator
 
 
 def test_model_validator_wrap() -> None:
     class Model(BaseModel):
         x: int
         y: int
 
@@ -40,14 +39,40 @@
                 values['y'] += 1
             else:
                 assert isinstance(values, Model)
                 values.x += 1
                 values.y += 1
             return values
 
+    m = Model(x=1, y=2)
+    assert m.model_dump() == {'x': 2, 'y': 3}
+    # model not changed because we don't revalidate m
+    assert Model.model_validate(m).model_dump() == {'x': 2, 'y': 3}
+
+
+@pytest.mark.parametrize('classmethod_decorator', [classmethod, lambda x: x])
+def test_model_validator_before_revalidate_always(classmethod_decorator: Any) -> None:
+    class Model(BaseModel, revalidate_instances='always'):
+        x: int
+        y: int
+
+        @model_validator(mode='before')
+        @classmethod_decorator
+        def val_model(cls, values: Any, info: ValidationInfo) -> dict[str, Any] | Model:
+            assert not info.context
+            if isinstance(values, dict):
+                values = cast(Dict[str, Any], values)
+                values['x'] += 1
+                values['y'] += 1
+            else:
+                assert isinstance(values, Model)
+                values.x += 1
+                values.y += 1
+            return values
+
     assert Model(x=1, y=2).model_dump() == {'x': 2, 'y': 3}
     assert Model.model_validate(Model(x=1, y=2)).model_dump() == {'x': 3, 'y': 4}
 
 
 def test_model_validator_after() -> None:
     class Model(BaseModel):
         x: int
@@ -72,7 +97,33 @@
             values['age'] *= 2
             return values
 
     class Person(Human):
         age: int
 
     assert Person(age=28).age == 56
+
+
+def test_nested_models() -> None:
+    calls: list[str] = []
+
+    class Model(BaseModel):
+        inner: Union[Model, None]  # noqa
+
+        @model_validator(mode='before')
+        @classmethod
+        def validate_model_before(cls, values: dict[str, Any]) -> dict[str, Any]:
+            calls.append('before')
+            return values
+
+        @model_validator(mode='after')
+        def validate_model_after(self) -> Model:
+            calls.append('after')
+            return self
+
+    Model.model_validate({'inner': None})
+    assert calls == ['before', 'after']
+    calls.clear()
+
+    Model.model_validate({'inner': {'inner': {'inner': None}}})
+    assert calls == ['before'] * 3 + ['after'] * 3
+    calls.clear()
```

### Comparing `pydantic-2.0a4/tests/test_networks.py` & `pydantic-2.0b1/tests/test_networks.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a4/tests/test_networks_ipaddress.py` & `pydantic-2.0b1/tests/test_networks_ipaddress.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a4/tests/test_parse.py` & `pydantic-2.0b1/tests/test_parse.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import List, Tuple
 
 import pytest
 
-from pydantic import BaseModel, ValidationError, model_serializer, parse_obj_as, root_validator
+from pydantic import BaseModel, ValidationError, model_validator, parse_obj_as
+from pydantic.functional_serializers import model_serializer
 
 
 class Model(BaseModel):
     a: float
     b: int = 10
 
 
@@ -43,30 +44,29 @@
     assert exc_info.value.errors(include_url=False) == [
         {'input': {'c': 123}, 'loc': ('a',), 'msg': 'Field required', 'type': 'missing'}
     ]
 
 
 def test_root_model_error():
     with pytest.raises(
-        TypeError,
-        match='__root__ models are no longer supported in v2',
+        TypeError, match="To define root models, use `pydantic.RootModel` rather than a field called '__root__'"
     ):
 
         class MyModel(BaseModel):
             __root__: str
 
 
 def test_model_validate_root():
     class MyModel(BaseModel):
         root: str
 
         # Note that the following three definitions require no changes across all __root__ models
         # I couldn't see a nice way to create a decorator that reduces the boilerplate,
         # but if we want to discourage this pattern, perhaps that's okay?
-        @root_validator(pre=True)
+        @model_validator(mode='before')
         @classmethod
         def populate_root(cls, values):
             return {'root': values}
 
         @model_serializer(mode='wrap')
         def _serialize(self, handler, info):
             data = handler(self)
@@ -81,28 +81,26 @@
             return json_schema['properties']['root']
 
     # Validation
     m = MyModel.model_validate('a')
     assert m.root == 'a'
 
     # Serialization
-    # TODO: Possible concern — `model_dump` is annotated as returning dict[str, Any] — is that okay, given
-    #   model_serializer could change that? Should we try to reflect it in the mypy plugin?
     assert m.model_dump() == {'root': 'a'}
     assert m.model_dump_json() == '"a"'
 
     # JSON schema
     assert m.model_json_schema() == {'title': 'Root', 'type': 'string'}
 
 
 def test_parse_root_list():
     class MyModel(BaseModel):
         root: List[str]
 
-        @root_validator(pre=True)
+        @model_validator(mode='before')
         @classmethod
         def populate_root(cls, values):
             return {'root': values}
 
         @model_serializer(mode='wrap')
         def _serialize(self, handler, info):
             data = handler(self)
@@ -124,15 +122,15 @@
 def test_parse_nested_root_list():
     class NestedData(BaseModel):
         id: str
 
     class NestedModel(BaseModel):
         root: List[NestedData]
 
-        @root_validator(pre=True)
+        @model_validator(mode='before')
         @classmethod
         def populate_root(cls, values):
             return {'root': values}
 
         @model_serializer(mode='wrap')
         def _serialize(self, handler, info):
             data = handler(self)
@@ -157,15 +155,15 @@
 def test_parse_nested_root_tuple():
     class NestedData(BaseModel):
         id: str
 
     class NestedModel(BaseModel):
         root: Tuple[int, NestedData]
 
-        @root_validator(pre=True)
+        @model_validator(mode='before')
         @classmethod
         def populate_root(cls, values):
             return {'root': values}
 
         @model_serializer(mode='wrap')
         def _serialize(self, handler, info):
             data = handler(self)
@@ -190,15 +188,15 @@
     assert isinstance(nested, NestedModel)
 
 
 def test_parse_nested_custom_root():
     class NestedModel(BaseModel):
         root: List[str]
 
-        @root_validator(pre=True)
+        @model_validator(mode='before')
         @classmethod
         def populate_root(cls, values):
             return {'root': values}
 
         @model_serializer(mode='wrap')
         def _serialize(self, handler, info):
             data = handler(self)
@@ -210,15 +208,15 @@
         @classmethod
         def model_modify_json_schema(cls, json_schema):
             return json_schema['properties']['root']
 
     class MyModel(BaseModel):
         root: NestedModel
 
-        @root_validator(pre=True)
+        @model_validator(mode='before')
         @classmethod
         def populate_root(cls, values):
             return {'root': values}
 
         @model_serializer(mode='wrap')
         def _serialize(self, handler, info):
             data = handler(self)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pydantic-2.0a4/tests/test_private_attributes.py` & `pydantic-2.0b1/tests/test_private_attributes.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 import functools
-import platform
 from typing import ClassVar, Generic, TypeVar
 
 import pytest
 
 from pydantic import BaseModel, ConfigDict, PrivateAttr
-from pydantic.fields import Undefined
+from pydantic.fields import _Undefined
 
 
 def test_private_attribute():
     default = {'a': {}}
 
     class Model(BaseModel):
         _foo = PrivateAttr(default)
 
-    assert Model.__slots__ == {'_foo'}
-    if platform.python_implementation() == 'PyPy':
-        repr(Model._foo).startswith('<member_descriptor object at')
-    else:
-        assert repr(Model._foo) == "<member '_foo' of 'Model' objects>"
+    assert set(Model.__private_attributes__) == {'_foo'}
 
     m = Model()
     assert m._foo == default
     assert m._foo is not default
     assert m._foo['a'] is not default['a']
 
     m._foo = None
@@ -50,20 +45,14 @@
 
     def factory():
         return default
 
     class Model(BaseModel):
         _foo = PrivateAttr(default_factory=factory)
 
-    assert Model.__slots__ == {'_foo'}
-    if platform.python_implementation() == 'PyPy':
-        repr(Model._foo).startswith('<member_descriptor object at')
-    else:
-        assert repr(Model._foo) == "<member '_foo' of 'Model' objects>"
-
     assert Model.__private_attributes__ == {'_foo': PrivateAttr(default_factory=factory)}
 
     m = Model()
     assert m._foo == default
     assert m._foo is default
     assert m._foo['a'] is default['a']
 
@@ -76,20 +65,15 @@
 
 def test_private_attribute_annotation():
     class Model(BaseModel):
         """The best model"""
 
         _foo: str
 
-    assert Model.__slots__ == {'_foo'}
-    if platform.python_implementation() == 'PyPy':
-        repr(Model._foo).startswith('<member_descriptor object at')
-    else:
-        assert repr(Model._foo) == "<member '_foo' of 'Model' objects>"
-    assert Model.__private_attributes__ == {'_foo': PrivateAttr(Undefined)}
+    assert Model.__private_attributes__ == {'_foo': PrivateAttr(_Undefined)}
     assert repr(Model.__doc__) == "'The best model'"
 
     m = Model()
     with pytest.raises(AttributeError):
         m._foo
 
     m._foo = '123'
@@ -111,19 +95,14 @@
 
 
 def test_underscore_attrs_are_private():
     class Model(BaseModel):
         _foo: str = 'abc'
         _bar: ClassVar[str] = 'cba'
 
-    assert Model.__slots__ == {'_foo'}
-    if platform.python_implementation() == 'PyPy':
-        repr(Model._foo).startswith('<member_descriptor object at')
-    else:
-        assert repr(Model._foo) == "<member '_foo' of 'Model' objects>"
     assert Model._bar == 'cba'
     assert Model.__private_attributes__ == {'_foo': PrivateAttr('abc')}
 
     m = Model()
     assert m._foo == 'abc'
     m._foo = None
     assert m._foo is None
@@ -140,15 +119,15 @@
 
 def test_private_attribute_intersection_with_extra_field():
     class Model(BaseModel):
         _foo = PrivateAttr('private_attribute')
 
         model_config = ConfigDict(extra='allow')
 
-    assert Model.__slots__ == {'_foo'}
+    assert set(Model.__private_attributes__) == {'_foo'}
     m = Model(_foo='field')
     assert m._foo == 'private_attribute'
     assert m.__dict__ == {}
     assert m.__pydantic_extra__ == {'_foo': 'field'}
     assert m.model_dump() == {'_foo': 'field'}
 
     m._foo = 'still_private'
@@ -241,25 +220,21 @@
 
     class ParentBModel(GrandParentModel):
         _bar = PrivateAttr(default)
 
     class Model(ParentAModel, ParentBModel):
         _baz = PrivateAttr(default)
 
-    assert GrandParentModel.__slots__ == {'_foo'}
-    assert ParentBModel.__slots__ == {'_bar'}
-    assert Model.__slots__ == {'_baz'}
-    if platform.python_implementation() == 'PyPy':
-        assert repr(Model._foo).startswith('<member_descriptor object at')
-        assert repr(Model._bar).startswith('<member_descriptor object at')
-        assert repr(Model._baz).startswith('<member_descriptor object at')
-    else:
-        assert repr(Model._foo) == "<member '_foo' of 'GrandParentModel' objects>"
-        assert repr(Model._bar) == "<member '_bar' of 'ParentBModel' objects>"
-        assert repr(Model._baz) == "<member '_baz' of 'Model' objects>"
+    assert GrandParentModel.__private_attributes__ == {
+        '_foo': PrivateAttr(default),
+    }
+    assert ParentBModel.__private_attributes__ == {
+        '_foo': PrivateAttr(default),
+        '_bar': PrivateAttr(default),
+    }
     assert Model.__private_attributes__ == {
         '_foo': PrivateAttr(default),
         '_bar': PrivateAttr(default),
         '_baz': PrivateAttr(default),
     }
 
     m = Model()
@@ -324,7 +299,43 @@
     """Demonstrate the members of functools are ignore here as with fields."""
 
     class MyModel(BaseModel):
         _a: functools.cached_property
         _b: int
 
     assert set(MyModel.__private_attributes__) == {'_b'}
+
+
+def test_none_as_private_attr():
+    from pydantic import BaseModel
+
+    class A(BaseModel):
+        _x: None
+
+    a = A()
+    a._x = None
+    assert a._x is None
+
+
+def test_layout_compatible_multiple_private_parents():
+    import typing as t
+
+    import pydantic
+
+    class ModelMixin(pydantic.BaseModel):
+        _mixin_private: t.Optional[str] = pydantic.PrivateAttr(None)
+
+    class Model(pydantic.BaseModel):
+        public: str = 'default'
+        _private: t.Optional[str] = pydantic.PrivateAttr(None)
+
+    class NewModel(ModelMixin, Model):
+        pass
+
+    assert set(NewModel.__private_attributes__) == {'_mixin_private', '_private'}
+    m = NewModel()
+    m._mixin_private = 1
+    m._private = 2
+
+    assert m.__pydantic_private__ == {'_mixin_private': 1, '_private': 2}
+    assert m._mixin_private == 1
+    assert m._private == 2
```

### Comparing `pydantic-2.0a4/tests/test_rich_repr.py` & `pydantic-2.0b1/tests/test_rich_repr.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a4/tests/test_serialize.py` & `pydantic-2.0b1/tests/test_serialize.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,39 @@
 """
 New tests for v2 of serialization logic.
 """
 import json
+import re
 from functools import partial, partialmethod
-from typing import Any, Optional
+from typing import Any, Callable, Dict, Iterable, Optional, Pattern, Tuple, Type
 
 import pytest
-from pydantic_core import PydanticSerializationError, core_schema, to_jsonable_python
-from typing_extensions import Annotated
+from pydantic_core import PydanticSerializationError, SchemaSerializer, core_schema, to_jsonable_python
+from typing_extensions import Annotated, TypedDict
 
 from pydantic import (
     BaseModel,
     Field,
     FieldSerializationInfo,
+    GetCoreSchemaHandler,
+    SecretField,
+    SecretStr,
     SerializationInfo,
     SerializerFunctionWrapHandler,
+    TypeAdapter,
+    errors,
     field_serializer,
     model_serializer,
 )
-from pydantic.annotated_arguments import PlainSerializer, WrapSerializer
+from pydantic._internal import _known_annotated_metadata
+from pydantic._internal._config import ConfigWrapper
+from pydantic._internal._generate_schema import GenerateSchema
 from pydantic.config import ConfigDict
+from pydantic.functional_serializers import PlainSerializer, WrapSerializer
+from pydantic.types import _SecretFieldValidator
 
 
 def test_serialize_extra_allow() -> None:
     class Model(BaseModel):
         x: int
         model_config = ConfigDict(extra='allow')
 
@@ -68,54 +78,54 @@
     m = Model(inner=Parent(x=1, y=2))
     assert m.inner.y == 2
     assert m.model_dump() == {'inner': {'x': 1, 'y': 2}}
     assert json.loads(m.model_dump_json()) == {'inner': {'x': 1, 'y': 2}}
 
 
 def test_serializer_annotated_plain_always():
-    FancyInt = Annotated[int, PlainSerializer(lambda x: f'{x:,}', json_return_type='str')]
+    FancyInt = Annotated[int, PlainSerializer(lambda x: f'{x:,}', return_type=str)]
 
     class MyModel(BaseModel):
         x: FancyInt
 
     assert MyModel(x=1234).model_dump() == {'x': '1,234'}
     assert MyModel(x=1234).model_dump(mode='json') == {'x': '1,234'}
     assert MyModel(x=1234).model_dump_json() == '{"x":"1,234"}'
 
 
 def test_serializer_annotated_plain_json():
-    FancyInt = Annotated[int, PlainSerializer(lambda x: f'{x:,}', json_return_type='str', when_used='json')]
+    FancyInt = Annotated[int, PlainSerializer(lambda x: f'{x:,}', return_type=str, when_used='json')]
 
     class MyModel(BaseModel):
         x: FancyInt
 
     assert MyModel(x=1234).model_dump() == {'x': 1234}
     assert MyModel(x=1234).model_dump(mode='json') == {'x': '1,234'}
     assert MyModel(x=1234).model_dump_json() == '{"x":"1,234"}'
 
 
 def test_serializer_annotated_wrap_always():
-    def ser_wrap(v: Any, nxt: SerializerFunctionWrapHandler) -> Any:
+    def ser_wrap(v: Any, nxt: SerializerFunctionWrapHandler) -> str:
         return f'{nxt(v + 1):,}'
 
-    FancyInt = Annotated[int, WrapSerializer(ser_wrap, json_return_type='str')]
+    FancyInt = Annotated[int, WrapSerializer(ser_wrap, return_type=str)]
 
     class MyModel(BaseModel):
         x: FancyInt
 
     assert MyModel(x=1234).model_dump() == {'x': '1,235'}
     assert MyModel(x=1234).model_dump(mode='json') == {'x': '1,235'}
     assert MyModel(x=1234).model_dump_json() == '{"x":"1,235"}'
 
 
 def test_serializer_annotated_wrap_json():
-    def ser_wrap(v: Any, nxt: SerializerFunctionWrapHandler) -> Any:
+    def ser_wrap(v: Any, nxt: SerializerFunctionWrapHandler) -> str:
         return f'{nxt(v + 1):,}'
 
-    FancyInt = Annotated[int, WrapSerializer(ser_wrap, json_return_type='str', when_used='json')]
+    FancyInt = Annotated[int, WrapSerializer(ser_wrap, when_used='json')]
 
     class MyModel(BaseModel):
         x: FancyInt
 
     assert MyModel(x=1234).model_dump() == {'x': 1234}
     assert MyModel(x=1234).model_dump(mode='json') == {'x': '1,235'}
     assert MyModel(x=1234).model_dump_json() == '{"x":"1,235"}'
@@ -137,16 +147,16 @@
     assert FancyIntModel(x=1234).model_dump() == {'x': '1,235'}
 
 
 def test_serialize_decorator_always():
     class MyModel(BaseModel):
         x: Optional[int]
 
-        @field_serializer('x', json_return_type='str')
-        def customise_x_serialisation(v, _info):
+        @field_serializer('x')
+        def customise_x_serialisation(v, _info) -> str:
             return f'{v:,}'
 
     assert MyModel(x=1234).model_dump() == {'x': '1,234'}
     assert MyModel(x=1234).model_dump(mode='json') == {'x': '1,234'}
     assert MyModel(x=1234).model_dump_json() == '{"x":"1,234"}'
     m = MyModel(x=None)
     # can't use v:, on None, hence error
@@ -160,16 +170,16 @@
         m.model_dump_json()
 
 
 def test_serialize_decorator_json():
     class MyModel(BaseModel):
         x: int
 
-        @field_serializer('x', json_return_type='str', when_used='json')
-        def customise_x_serialisation(v):
+        @field_serializer('x', when_used='json')
+        def customise_x_serialisation(v) -> str:
             return f'{v:,}'
 
     assert MyModel(x=1234).model_dump() == {'x': 1234}
     assert MyModel(x=1234).model_dump(mode='json') == {'x': '1,234'}
     assert MyModel(x=1234).model_dump_json() == '{"x":"1,234"}'
 
 
@@ -259,64 +269,64 @@
     with pytest.raises(TypeError, match='Unrecognized field_serializer function signature'):
 
         class _(BaseModel):
             x: int
 
             # caught by type checkers
             @field_serializer('x')
-            def no_args() -> Any:  # pragma: no cover
+            def no_args() -> Any:
                 ...
 
 
 def test_invalid_signature_single_params() -> None:
     with pytest.raises(TypeError, match='Unrecognized field_serializer function signature'):
 
         class _(BaseModel):
             x: int
 
             # not caught by type checkers
             @field_serializer('x')
-            def no_args(self) -> Any:  # pragma: no cover
+            def no_args(self) -> Any:
                 ...
 
 
 def test_invalid_signature_too_many_params_1() -> None:
     with pytest.raises(TypeError, match='Unrecognized field_serializer function signature'):
 
         class _(BaseModel):
             x: int
 
             # caught by type checkers
             @field_serializer('x')
-            def no_args(self, value: Any, nxt: Any, info: Any, extra_param: Any) -> Any:  # pragma: no cover
+            def no_args(self, value: Any, nxt: Any, info: Any, extra_param: Any) -> Any:
                 ...
 
 
 def test_invalid_signature_too_many_params_2() -> None:
     with pytest.raises(TypeError, match='Unrecognized field_serializer function signature'):
 
         class _(BaseModel):
             x: int
 
             # caught by type checkers
             @field_serializer('x')
             @staticmethod
-            def no_args(not_self: Any, value: Any, nxt: Any, info: Any) -> Any:  # pragma: no cover
+            def no_args(not_self: Any, value: Any, nxt: Any, info: Any) -> Any:
                 ...
 
 
 def test_invalid_signature_bad_plain_signature() -> None:
     with pytest.raises(TypeError, match='Unrecognized field_serializer function signature for'):
 
         class _(BaseModel):
             x: int
 
             # caught by type checkers
             @field_serializer('x', mode='plain')
-            def no_args(self, value: Any, nxt: Any, info: Any) -> Any:  # pragma: no cover
+            def no_args(self, value: Any, nxt: Any, info: Any) -> Any:
                 ...
 
 
 def test_serialize_ignore_info_plain():
     class MyModel(BaseModel):
         x: int
 
@@ -338,28 +348,28 @@
     assert MyModel(x=1234).model_dump() == {'x': '1,234'}
 
 
 def test_serialize_decorator_self_info():
     class MyModel(BaseModel):
         x: Optional[int]
 
-        @field_serializer('x', json_return_type='str')
-        def customise_x_serialisation(self, v, info):
+        @field_serializer('x')
+        def customise_x_serialisation(self, v, info) -> str:
             return f'{info.mode}:{v:,}'
 
     assert MyModel(x=1234).model_dump() == {'x': 'python:1,234'}
     assert MyModel(x=1234).model_dump(mode='foobar') == {'x': 'foobar:1,234'}
 
 
 def test_serialize_decorator_self_no_info():
     class MyModel(BaseModel):
         x: Optional[int]
 
-        @field_serializer('x', json_return_type='str')
-        def customise_x_serialisation(self, v):
+        @field_serializer('x')
+        def customise_x_serialisation(self, v) -> str:
             return f'{v:,}'
 
     assert MyModel(x=1234).model_dump() == {'x': '1,234'}
 
 
 def test_model_serializer_plain():
     class MyModel(BaseModel):
@@ -454,34 +464,33 @@
     assert m.model_dump_json(exclude={'a'}) == '{"b":"boom","info":"mode=json exclude={\'a\'}"}'
 
 
 def test_model_serializer_plain_json_return_type():
     class MyModel(BaseModel):
         a: int
 
-        @model_serializer(json_return_type='str_subclass')
-        def _serialize(self):
+        @model_serializer(when_used='json')
+        def _serialize(self) -> str:
             if self.a == 666:
                 return self.a
             else:
                 return f'MyModel(a={self.a!r})'
 
     m = MyModel(a=1)
-    assert m.model_dump() == 'MyModel(a=1)'
+    assert m.model_dump() == {'a': 1}
     assert m.model_dump(mode='json') == 'MyModel(a=1)'
     assert m.model_dump_json() == '"MyModel(a=1)"'
 
     m = MyModel(a=666)
-    assert m.model_dump() == 666
-    with pytest.raises(TypeError, match="^'int' object cannot be converted to 'PyString'$"):
-        m.model_dump(mode='json')
+    assert m.model_dump() == {'a': 666}
+    with pytest.warns(UserWarning, match='Expected `str` but got `int` - serialized value may not be as expected'):
+        assert m.model_dump(mode='json') == 666
 
-    msg = "^Error serializing to JSON: 'int' object cannot be converted to 'PyString'$"
-    with pytest.raises(PydanticSerializationError, match=msg):
-        m.model_dump_json()
+    with pytest.warns(UserWarning, match='Expected `str` but got `int` - serialized value may not be as expected'):
+        assert m.model_dump_json() == '666'
 
 
 def test_model_serializer_wrong_args():
     m = (
         r'Unrecognized model_serializer function signature for '
         r'<.+MyModel._serialize at 0x\w+> with `mode=plain`:\(self, x, y, z\)'
     )
@@ -522,34 +531,34 @@
     m = "Multiple field serializer functions were defined for field 'x', this is not allowed."
     with pytest.raises(TypeError, match=m):
 
         class MyModel(BaseModel):
             x: int
             y: int
 
-            @field_serializer('x', 'y', json_return_type='str')
-            def serializer1(v):
+            @field_serializer('x', 'y')
+            def serializer1(v) -> str:
                 return f'{v:,}'
 
-            @field_serializer('x', json_return_type='str')
-            def serializer2(v):
+            @field_serializer('x')
+            def serializer2(v) -> str:
                 return v
 
 
 def test_field_multiple_serializer_subclass():
     class MyModel(BaseModel):
         x: int
 
-        @field_serializer('x', json_return_type='str')
-        def serializer1(v):
+        @field_serializer('x')
+        def serializer1(v) -> str:
             return f'{v:,}'
 
     class MySubModel(MyModel):
-        @field_serializer('x', json_return_type='str')
-        def serializer1(v):
+        @field_serializer('x')
+        def serializer1(v) -> str:
             return f'{v}'
 
     assert MyModel(x=1234).model_dump() == {'x': '1,234'}
     assert MySubModel(x=1234).model_dump() == {'x': '1234'}
 
 
 def int_ser_func_without_info1(v: int, expected: int) -> str:
@@ -603,15 +612,15 @@
 )
 def test_serialize_partial(
     func: Any,
 ):
     class MyModel(BaseModel):
         x: int
 
-        ser = field_serializer('x', json_return_type='str')(partial(func, expected=1234))
+        ser = field_serializer('x', return_type=str)(partial(func, expected=1234))
 
     assert MyModel(x=1234).model_dump() == {'x': '1,234'}
 
 
 @pytest.mark.parametrize(
     'func',
     [
@@ -627,15 +636,15 @@
 )
 def test_serialize_partialmethod(
     func: Any,
 ):
     class MyModel(BaseModel):
         x: int
 
-        ser = field_serializer('x', json_return_type='str')(partialmethod(func, expected=1234))
+        ser = field_serializer('x', return_type=str)(partialmethod(func, expected=1234))
 
     assert MyModel(x=1234).model_dump() == {'x': '1,234'}
 
 
 def test_serializer_allow_reuse_inheritance_override():
     class Parent(BaseModel):
         x: int
@@ -781,7 +790,150 @@
     class AnyModel(BaseModel):
         x: Any
 
     m = Model(m='test')
     assert m.model_dump() == {'m': 'custom:test'}
     assert to_jsonable_python(AnyModel(x=m)) == {'x': {'m': 'custom:test'}}
     assert AnyModel(x=m).model_dump() == {'x': {'m': 'custom:test'}}
+
+
+def test_invalid_field():
+    msg = (
+        r'Decorators defined with incorrect fields:'
+        r' tests.test_serialize.test_invalid_field.<locals>.Model:\d+.customise_b_serialisation'
+        r" \(use check_fields=False if you're inheriting from the model and intended this\)"
+    )
+    with pytest.raises(errors.PydanticUserError, match=msg):
+
+        class Model(BaseModel):
+            a: str
+
+            @field_serializer('b')
+            def customise_b_serialisation(v):
+                return v
+
+
+def test_serialize_with_extra():
+    class Inner(BaseModel):
+        a: str = 'a'
+
+    class Outer(BaseModel):
+        # this cause the inner model incorrectly dumpped:
+        model_config = ConfigDict(extra='allow')
+        inner: Inner = Field(default_factory=Inner)
+
+    m = Outer.model_validate({})
+
+    assert m.model_dump() == {'inner': {'a': 'a'}}
+
+
+def test_model_serializer_nested_models() -> None:
+    class Model(BaseModel):
+        x: int
+        inner: Optional['Model']
+
+        @model_serializer(mode='wrap')
+        def ser_model(self, handler: Callable[['Model'], Dict[str, Any]]) -> Dict[str, Any]:
+            inner = handler(self)
+            inner['x'] += 1
+            return inner
+
+    assert Model(x=0, inner=None).model_dump() == {'x': 1, 'inner': None}
+
+    assert Model(x=2, inner=Model(x=1, inner=Model(x=0, inner=None))).model_dump() == {
+        'x': 3,
+        'inner': {'x': 2, 'inner': {'x': 1, 'inner': None}},
+    }
+
+
+def test_pattern_serialize():
+    ta = TypeAdapter(Pattern[str])
+    pattern = re.compile('^regex$')
+    assert ta.dump_python(pattern) == pattern
+    assert ta.dump_python(pattern, mode='json') == '^regex$'
+    assert ta.dump_json(pattern) == b'"^regex$"'
+
+
+def test_custom_return_schema():
+    class Model(BaseModel):
+        x: int
+
+        @field_serializer('x', return_type=str)
+        def ser_model(self, v) -> int:
+            return repr(v)
+
+    return_serializer = re.search(r'return_serializer: *\w+', repr(Model.__pydantic_serializer__)).group(0)
+    assert return_serializer == 'return_serializer: Str'
+
+
+def test_clear_return_schema():
+    class Model(BaseModel):
+        x: int
+
+        @field_serializer('x', return_type=Any)
+        def ser_model(self, v) -> int:
+            return repr(v)
+
+    return_serializer = re.search(r'return_serializer: *\w+', repr(Model.__pydantic_serializer__)).group(0)
+    assert return_serializer == 'return_serializer: Any'
+
+
+def test_type_adapter_dump_json():
+    class Model(TypedDict):
+        x: int
+        y: float
+
+        @model_serializer(mode='plain')
+        def ser_model(self) -> Dict[str, Any]:
+            return {'x': self['x'] * 2, 'y': self['y'] * 3}
+
+    ta = TypeAdapter(Model)
+
+    assert ta.dump_json(Model({'x': 1, 'y': 2.5})) == b'{"x":2,"y":7.5}'
+
+
+def test_custom_secret_type_python_serializer():
+    """
+    test for non json serializer in pydantic.types._SecretFieldValidator.serialize.
+    most of the code in this test are just a copy from original implementation.
+    """
+
+    class MySecretFieldValidator(_SecretFieldValidator):
+        def __get_pydantic_core_schema__(
+            self, source: Type[Any], handler: GetCoreSchemaHandler
+        ) -> core_schema.CoreSchema:
+            self.inner_schema = handler(str if self.field_type is SecretStr else bytes)
+            error_kind = 'string_type' if self.field_type is SecretStr else 'bytes_type'
+            return core_schema.general_after_validator_function(
+                self.validate,
+                core_schema.union_schema(
+                    [core_schema.is_instance_schema(self.field_type), self.inner_schema],
+                    strict=True,
+                    custom_error_type=error_kind,
+                ),
+                serialization=core_schema.plain_serializer_function_ser_schema(
+                    self.serialize,
+                    info_arg=True,
+                    return_schema=core_schema.str_schema(),
+                    when_used='always',  # change it to `always` to call `serialize` for python and json
+                ),
+            )
+
+    class MySecretStr(SecretField[str]):
+        @classmethod
+        def __prepare_pydantic_annotations__(
+            cls, source: Type[Any], annotations: Tuple[Any, ...], _config: ConfigDict
+        ) -> Tuple[Any, Iterable[Any]]:
+            metadata, remaining_annotations = _known_annotated_metadata.collect_known_metadata(annotations)
+            _known_annotated_metadata.check_metadata(metadata, {'min_length', 'max_length'}, cls)
+            return (
+                source,
+                (
+                    MySecretFieldValidator(source, **metadata),
+                    *remaining_annotations,
+                ),
+            )
+
+    gen = GenerateSchema(ConfigWrapper({}), None)
+    schema = gen.generate_schema(MySecretStr)
+    serializer = SchemaSerializer(schema)
+    assert serializer.to_python('foo bar') == 'foo bar'
```

### Comparing `pydantic-2.0a4/tests/test_strict.py` & `pydantic-2.0b1/tests/test_strict.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a4/tests/test_structural_pattern_matching.py` & `pydantic-2.0b1/tests/test_structural_pattern_matching.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a4/tests/test_tools.py` & `pydantic-2.0b1/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a4/tests/test_types.py` & `pydantic-2.0b1/tests/test_types.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,50 @@
+import collections
 import itertools
 import json
 import math
 import os
 import re
 import sys
+import typing
 import uuid
-from collections import OrderedDict, deque
+from collections import OrderedDict, defaultdict, deque
 from datetime import date, datetime, time, timedelta, timezone
 from decimal import Decimal
 from enum import Enum, IntEnum
 from pathlib import Path
 from typing import (
     Any,
     Callable,
+    Counter,
+    DefaultDict,
     Deque,
     Dict,
     FrozenSet,
     Iterable,
     List,
-    MutableSet,
     NewType,
     Optional,
     Pattern,
     Sequence,
     Set,
     Tuple,
+    Type,
     TypeVar,
     Union,
 )
 from uuid import UUID
 
 import annotated_types
+import dirty_equals
 import pytest
-from dirty_equals import HasRepr, IsStr
-from pydantic_core import PydanticCustomError, SchemaError, core_schema
+from dirty_equals import HasRepr, IsOneOf, IsStr
+from pydantic_core import CoreSchema, PydanticCustomError, SchemaError, core_schema
 from pydantic_core.core_schema import ValidationInfo
-from typing_extensions import Annotated, Literal, TypedDict
+from typing_extensions import Annotated, Literal, TypedDict, get_args
 
 from pydantic import (
     UUID1,
     UUID3,
     UUID4,
     UUID5,
     AwareDatetime,
@@ -50,25 +55,29 @@
     ConfigDict,
     DirectoryPath,
     EmailStr,
     Field,
     FilePath,
     FiniteFloat,
     FutureDate,
+    FutureDatetime,
+    GetCoreSchemaHandler,
+    GetJsonSchemaHandler,
     Json,
     NaiveDatetime,
     NameEmail,
     NegativeFloat,
     NegativeInt,
     NewPath,
     NonNegativeFloat,
     NonNegativeInt,
     NonPositiveFloat,
     NonPositiveInt,
     PastDate,
+    PastDatetime,
     PositiveFloat,
     PositiveInt,
     PydanticInvalidForJsonSchema,
     SecretBytes,
     SecretStr,
     StrictBool,
     StrictBytes,
@@ -82,18 +91,22 @@
     condecimal,
     confloat,
     confrozenset,
     conint,
     conlist,
     conset,
     constr,
+    field_serializer,
+    field_validator,
+    validate_call,
 )
-from pydantic.decorators import field_validator
-from pydantic.json_schema import GetJsonSchemaHandler, JsonSchemaValue
-from pydantic.types import AllowInfNan, ImportString, SecretField, Strict
+from pydantic.errors import PydanticSchemaGenerationError
+from pydantic.functional_validators import AfterValidator
+from pydantic.json_schema import JsonSchemaValue
+from pydantic.types import AllowInfNan, ImportString, InstanceOf, SecretField, SkipValidation, Strict, TransformSchema
 
 try:
     import email_validator
 except ImportError:
     email_validator = None
 
 # TODO add back tests for Iterator
@@ -795,30 +808,30 @@
     with pytest.raises(ValidationError) as exc_info:
         PyObjectModel(callable='foobar')
     # insert_assert(exc_info.value.errors(include_url=False))
     assert exc_info.value.errors(include_url=False) == [
         {
             'type': 'import_error',
             'loc': ('callable',),
-            'msg': 'Invalid python path: "foobar" doesn\'t look like a module path',
+            'msg': "Invalid python path: No module named 'foobar'",
             'input': 'foobar',
-            'ctx': {'error': '"foobar" doesn\'t look like a module path'},
+            'ctx': {'error': "No module named 'foobar'"},
         }
     ]
 
     with pytest.raises(ValidationError) as exc_info:
         PyObjectModel(callable='os.missing')
     # insert_assert(exc_info.value.errors(include_url=False))
     assert exc_info.value.errors(include_url=False) == [
         {
             'type': 'import_error',
             'loc': ('callable',),
-            'msg': 'Invalid python path: Module "os" does not define a "missing" attribute',
+            'msg': "Invalid python path: No module named 'os.missing'",
             'input': 'os.missing',
-            'ctx': {'error': 'Module "os" does not define a "missing" attribute'},
+            'ctx': {'error': "No module named 'os.missing'"},
         }
     ]
 
     with pytest.raises(ValidationError) as exc_info:
         PyObjectModel(callable='os.path')
     # insert_assert(exc_info.value.errors(include_url=False))
     assert exc_info.value.errors(include_url=False) == [
@@ -829,37 +842,153 @@
         PyObjectModel(callable=[1, 2, 3])
     # insert_assert(exc_info.value.errors(include_url=False))
     assert exc_info.value.errors(include_url=False) == [
         {'type': 'callable_type', 'loc': ('callable',), 'msg': 'Input should be callable', 'input': [1, 2, 3]}
     ]
 
 
-def test_string_import_any():
+@pytest.mark.parametrize(
+    ('value', 'expected', 'mode'),
+    [
+        ('math:cos', 'math.cos', 'json'),
+        ('math:cos', math.cos, 'python'),
+        pytest.param(
+            'os.path', 'posixpath', 'json', marks=pytest.mark.skipif(sys.platform == 'win32', reason='different output')
+        ),
+        pytest.param(
+            'os.path', 'ntpath', 'json', marks=pytest.mark.skipif(sys.platform != 'win32', reason='different output')
+        ),
+        ('os.path', os.path, 'python'),
+        ([1, 2, 3], [1, 2, 3], 'json'),
+        ([1, 2, 3], [1, 2, 3], 'python'),
+        ('math', 'math', 'json'),
+        ('math', math, 'python'),
+        ('builtins.list', 'builtins.list', 'json'),
+        ('builtins.list', list, 'python'),
+        (list, 'builtins.list', 'json'),
+        (list, list, 'python'),
+        (f'{__name__}.pytest', 'pytest', 'json'),
+        (f'{__name__}.pytest', pytest, 'python'),
+    ],
+)
+def test_string_import_any(value: Any, expected: Any, mode: Literal['json', 'python']):
     class PyObjectModel(BaseModel):
         thing: ImportString
 
-    assert PyObjectModel(thing='math.cos').model_dump() == {'thing': math.cos}
-    assert PyObjectModel(thing='os.path').model_dump() == {'thing': os.path}
-    assert PyObjectModel(thing=[1, 2, 3]).model_dump() == {'thing': [1, 2, 3]}
+    assert PyObjectModel(thing=value).model_dump(mode=mode) == {'thing': expected}
+
+
+@pytest.mark.parametrize('value', ['oss', 'os.os', f'{__name__}.x'])
+def test_string_import_any_expected_failure(value: Any):
+    """Ensure importString correctly fails to instantiate when it's supposed to"""
+
+    class PyObjectModel(BaseModel):
+        thing: ImportString
+
+    with pytest.raises(ValidationError, match='type=import_error'):
+        PyObjectModel(thing=value)
 
 
 @pytest.mark.parametrize(
     'annotation',
     [
         ImportString[Annotated[float, annotated_types.Ge(3), annotated_types.Le(4)]],
         Annotated[float, annotated_types.Ge(3), annotated_types.Le(4), ImportString],
     ],
 )
 def test_string_import_constraints(annotation):
     class PyObjectModel(BaseModel):
         thing: annotation
 
-    assert PyObjectModel(thing='math.pi').model_dump() == {'thing': pytest.approx(3.141592654)}
+    assert PyObjectModel(thing='math:pi').model_dump() == {'thing': pytest.approx(3.141592654)}
     with pytest.raises(ValidationError, match='type=greater_than_equal'):
-        PyObjectModel(thing='math.e')
+        PyObjectModel(thing='math:e')
+
+
+def test_string_import_examples():
+    import collections
+
+    adapter = TypeAdapter(ImportString)
+    assert adapter.validate_python('collections') is collections
+    assert adapter.validate_python('collections.abc') is collections.abc
+    assert adapter.validate_python('collections.abc.Mapping') is collections.abc.Mapping
+    assert adapter.validate_python('collections.abc:Mapping') is collections.abc.Mapping
+
+
+@pytest.mark.parametrize(
+    'import_string,errors',
+    [
+        (
+            'collections.abc.def',
+            [
+                {
+                    'ctx': {'error': "No module named 'collections.abc.def'"},
+                    'input': 'collections.abc.def',
+                    'loc': (),
+                    'msg': "Invalid python path: No module named 'collections.abc.def'",
+                    'type': 'import_error',
+                }
+            ],
+        ),
+        (
+            'collections.abc:def',
+            [
+                {
+                    'ctx': {'error': "cannot import name 'def' from 'collections.abc'"},
+                    'input': 'collections.abc:def',
+                    'loc': (),
+                    'msg': "Invalid python path: cannot import name 'def' from 'collections.abc'",
+                    'type': 'import_error',
+                }
+            ],
+        ),
+        (
+            'collections:abc:Mapping',
+            [
+                {
+                    'ctx': {'error': "Import strings should have at most one ':'; received 'collections:abc:Mapping'"},
+                    'input': 'collections:abc:Mapping',
+                    'loc': (),
+                    'msg': "Invalid python path: Import strings should have at most one ':';"
+                    " received 'collections:abc:Mapping'",
+                    'type': 'import_error',
+                }
+            ],
+        ),
+        (
+            '123_collections:Mapping',
+            [
+                {
+                    'ctx': {'error': "No module named '123_collections'"},
+                    'input': '123_collections:Mapping',
+                    'loc': (),
+                    'msg': "Invalid python path: No module named '123_collections'",
+                    'type': 'import_error',
+                }
+            ],
+        ),
+        (
+            ':Mapping',
+            [
+                {
+                    'ctx': {'error': "Import strings should have a nonempty module name; received ':Mapping'"},
+                    'input': ':Mapping',
+                    'loc': (),
+                    'msg': 'Invalid python path: Import strings should have a nonempty module '
+                    "name; received ':Mapping'",
+                    'type': 'import_error',
+                }
+            ],
+        ),
+    ],
+)
+def test_string_import_errors(import_string, errors):
+    with pytest.raises(ValidationError) as exc_info:
+        TypeAdapter(ImportString).validate_python(import_string)
+    assert exc_info.value.errors() == errors
 
 
 def test_decimal():
     class Model(BaseModel):
         v: Decimal
 
     m = Model(v='1.234')
@@ -1028,15 +1157,14 @@
 
 
 class BoolCastable:
     def __bool__(self) -> bool:
         return True
 
 
-@pytest.mark.xfail(sys.platform.startswith('win'), reason='https://github.com/PyO3/pyo3/issues/2913', strict=False)
 @pytest.mark.parametrize(
     'field,value,result',
     [
         ('bool_check', True, True),
         ('bool_check', 1, True),
         ('bool_check', 1.0, True),
         ('bool_check', Decimal(1), True),
@@ -1189,23 +1317,23 @@
         ('timedelta_check', Decimal(123_000.0002), timedelta(days=1, seconds=36600, microseconds=200)),
         ('timedelta_check', '1 10:10', ValidationError),
         ('timedelta_check', b'1 10:10', ValidationError),
         ('list_check', ['1', '2'], ['1', '2']),
         ('list_check', ('1', '2'), ['1', '2']),
         ('list_check', {'1': 1, '2': 2}.keys(), ['1', '2']),
         ('list_check', {'1': '1', '2': '2'}.values(), ['1', '2']),
-        ('list_check', {'1', '2'}, ValidationError),
-        ('list_check', frozenset(['1', '2']), ValidationError),
+        ('list_check', {'1', '2'}, dirty_equals.IsOneOf(['1', '2'], ['2', '1'])),
+        ('list_check', frozenset(['1', '2']), dirty_equals.IsOneOf(['1', '2'], ['2', '1'])),
         ('list_check', {'1': 1, '2': 2}, ValidationError),
         ('tuple_check', ('1', '2'), ('1', '2')),
         ('tuple_check', ['1', '2'], ('1', '2')),
         ('tuple_check', {'1': 1, '2': 2}.keys(), ('1', '2')),
         ('tuple_check', {'1': '1', '2': '2'}.values(), ('1', '2')),
-        ('tuple_check', {'1', '2'}, ValidationError),
-        ('tuple_check', frozenset(['1', '2']), ValidationError),
+        ('tuple_check', {'1', '2'}, dirty_equals.IsOneOf(('1', '2'), ('2', '1'))),
+        ('tuple_check', frozenset(['1', '2']), dirty_equals.IsOneOf(('1', '2'), ('2', '1'))),
         ('tuple_check', {'1': 1, '2': 2}, ValidationError),
         ('set_check', {'1', '2'}, {'1', '2'}),
         ('set_check', ['1', '2', '1', '2'], {'1', '2'}),
         ('set_check', ('1', '2', '1', '2'), {'1', '2'}),
         ('set_check', frozenset(['1', '2']), {'1', '2'}),
         ('set_check', {'1': 1, '2': 2}.keys(), {'1', '2'}),
         ('set_check', {'1': '1', '2': '2'}.values(), {'1', '2'}),
@@ -1310,17 +1438,17 @@
             'msg': 'Input should be in a valid time format, hour value is outside expected range of 0-23',
             'input': '25:20:30.400',
             'ctx': {'error': 'hour value is outside expected range of 0-23'},
         },
         {
             'type': 'time_delta_parsing',
             'loc': ('duration',),
-            'msg': 'Input should be a valid timedelta, unexpected extra characters at the end of the input',
+            'msg': 'Input should be a valid timedelta, invalid timezone sign',
             'input': '15:30.0001broken',
-            'ctx': {'error': 'unexpected extra characters at the end of the input'},
+            'ctx': {'error': 'invalid timezone sign'},
         },
     ]
 
 
 @pytest.fixture(scope='session')
 def cooking_model():
     class FruitEnum(str, Enum):
@@ -1515,30 +1643,25 @@
             }
         ]
 
 
 @pytest.mark.parametrize(
     'kwargs,type_',
     [
-        ({'max_length': 5}, int),
-        ({'min_length': 2}, float),
         ({'pattern': '^foo$'}, int),
-        ({'gt': 2}, str),
-        ({'lt': 5}, bytes),
-        ({'ge': 2}, str),
-        ({'le': 5}, bool),
-        ({'gt': 0}, Callable),
-        ({'gt': 0}, Callable[[int], int]),
         ({'gt': 0}, conlist(int, min_length=4)),
         ({'gt': 0}, conset(int, min_length=4)),
         ({'gt': 0}, confrozenset(int, min_length=4)),
     ],
 )
 def test_invalid_schema_constraints(kwargs, type_):
-    with pytest.raises(SchemaError, match='Invalid Schema:\n.*\n  Extra inputs are not permitted'):
+    match = (
+        r'(:?Invalid Schema:\n.*\n  Extra inputs are not permitted)|(:?The following constraints cannot be applied to)'
+    )
+    with pytest.raises((SchemaError, TypeError), match=match):
 
         class Foo(BaseModel):
             a: type_ = Field('foo', title='A title', description='A description', **kwargs)
 
 
 def test_invalid_decimal_constraint():
     with pytest.raises(
@@ -1554,31 +1677,34 @@
     class MoreStringsModel(BaseModel):
         str_strip_enabled: constr(strip_whitespace=True)
         str_strip_disabled: constr(strip_whitespace=False)
         str_regex: constr(pattern=r'^xxx\d{3}$') = ...
         str_min_length: constr(min_length=5) = ...
         str_email: EmailStr = ...
         name_email: NameEmail = ...
+        str_gt: Annotated[str, annotated_types.Gt('a')]
 
     m = MoreStringsModel(
         str_strip_enabled='   xxx123   ',
         str_strip_disabled='   xxx123   ',
         str_regex='xxx123',
         str_min_length='12345',
         str_email='foobar@example.com  ',
         name_email='foo bar  <foobaR@example.com>',
+        str_gt='b',
     )
     assert m.str_strip_enabled == 'xxx123'
     assert m.str_strip_disabled == '   xxx123   '
     assert m.str_regex == 'xxx123'
     assert m.str_email == 'foobar@example.com'
     assert repr(m.name_email) == "NameEmail(name='foo bar', email='foobaR@example.com')"
     assert str(m.name_email) == 'foo bar <foobaR@example.com>'
     assert m.name_email.name == 'foo bar'
     assert m.name_email.email == 'foobaR@example.com'
+    assert m.str_gt == 'b'
 
 
 @pytest.mark.skipif(not email_validator, reason='email_validator not installed')
 def test_string_fails():
     class MoreStringsModel(BaseModel):
         str_regex: constr(pattern=r'^xxx\d{3}$') = ...
         str_min_length: constr(min_length=5) = ...
@@ -1675,24 +1801,25 @@
 @pytest.mark.parametrize(
     'value,result',
     (
         ([1, 2, '3'], [1, 2, '3']),
         ((1, 2, '3'), [1, 2, '3']),
         ((i**2 for i in range(5)), [0, 1, 4, 9, 16]),
         (deque([1, 2, 3]), [1, 2, 3]),
+        ({1, '2'}, IsOneOf([1, '2'], ['2', 1])),
     ),
 )
 def test_list_success(value, result):
     class Model(BaseModel):
         v: list
 
     assert Model(v=value).v == result
 
 
-@pytest.mark.parametrize('value', (123, '123', {1, 2, '3'}))
+@pytest.mark.parametrize('value', (123, '123'))
 def test_list_fails(value):
     class Model(BaseModel):
         v: list
 
     with pytest.raises(ValidationError) as exc_info:
         Model(v=value)
     # insert_assert(exc_info.value.errors(include_url=False))
@@ -1724,24 +1851,25 @@
 @pytest.mark.parametrize(
     'value,result',
     (
         ([1, 2, '3'], (1, 2, '3')),
         ((1, 2, '3'), (1, 2, '3')),
         ((i**2 for i in range(5)), (0, 1, 4, 9, 16)),
         (deque([1, 2, 3]), (1, 2, 3)),
+        ({1, '2'}, IsOneOf((1, '2'), ('2', 1))),
     ),
 )
 def test_tuple_success(value, result):
     class Model(BaseModel):
         v: tuple
 
     assert Model(v=value).v == result
 
 
-@pytest.mark.parametrize('value', (123, '123', {1, 2, '3'}))
+@pytest.mark.parametrize('value', (123, '123'))
 def test_tuple_fails(value):
     class Model(BaseModel):
         v: tuple
 
     with pytest.raises(ValidationError) as exc_info:
         Model(v=value)
     # insert_assert(exc_info.value.errors(include_url=False))
@@ -1960,14 +2088,32 @@
         Model(it=3)
     # insert_assert(exc_info.value.errors(include_url=False))
     assert exc_info.value.errors(include_url=False) == [
         {'type': 'iterable_type', 'loc': ('it',), 'msg': 'Input should be iterable', 'input': 3}
     ]
 
 
+@pytest.mark.parametrize(
+    'config,input_str',
+    (
+        ({}, 'type=iterable_type, input_value=5, input_type=int'),
+        ({'hide_input_in_errors': False}, 'type=iterable_type, input_value=5, input_type=int'),
+        ({'hide_input_in_errors': True}, 'type=iterable_type'),
+    ),
+)
+def test_iterable_error_hide_input(config, input_str):
+    class Model(BaseModel):
+        it: Iterable[int]
+
+        model_config = ConfigDict(**config)
+
+    with pytest.raises(ValidationError, match=re.escape(f'Input should be iterable [{input_str}]')):
+        Model(it=5)
+
+
 def test_infinite_iterable_validate_first():
     class Model(BaseModel):
         it: Iterable[int]
         b: int
 
         @field_validator('it')
         @classmethod
@@ -2434,20 +2580,28 @@
     with pytest.raises(ValidationError, match=r'Input should be a valid integer \[type=int_type,'):
         Model(v='123456')
 
     with pytest.raises(ValidationError, match=r'Input should be a valid integer \[type=int_type,'):
         Model(v=3.14159)
 
     with pytest.raises(ValidationError, match=r'Input should be a valid integer \[type=int_type,'):
-        Model(v=2**64)
-
-    with pytest.raises(ValidationError, match=r'Input should be a valid integer \[type=int_type,'):
         Model(v=True)
 
 
+def test_int_parsing_size_error():
+    i64_max = 9_223_372_036_854_775_807
+    v = TypeAdapter(int)
+
+    with pytest.raises(
+        ValidationError,
+        match=r'Unable to parse input string as an integer, exceeded maximum size \[type=int_parsing_size,',
+    ):
+        v.validate_json(json.dumps(-i64_max * 2))
+
+
 def test_strict_float():
     class Model(BaseModel):
         v: StrictFloat
 
     assert Model(v=3.14159).v == 3.14159
     assert Model(v=123456).v == 123456
 
@@ -2466,45 +2620,94 @@
         Model(v={})
     assert exc_info.value.errors(include_url=False) == [
         {'type': 'bool_type', 'loc': ('v',), 'msg': 'Input should be a valid boolean', 'input': {}}
     ]
 
 
 def test_uuid_error():
-    class Model(BaseModel):
-        v: UUID
+    v = TypeAdapter(UUID)
+
+    valid = UUID('49fdfa1d856d4003a83e4b9236532ec6')
+
+    # sanity check
+    assert v.validate_python(valid) == valid
+    assert v.validate_python(valid.hex) == valid
 
     with pytest.raises(ValidationError) as exc_info:
-        Model(v='ebcdab58-6eb8-46fb-a190-d07a3')
+        v.validate_python('ebcdab58-6eb8-46fb-a190-d07a3')
     # insert_assert(exc_info.value.errors(include_url=False))
     assert exc_info.value.errors(include_url=False) == [
         {
-            'type': 'uuid_type',
-            'loc': ('v',),
-            'msg': 'Input should be a valid UUID, string, or bytes',
+            'type': 'is_instance_of',
+            'loc': ('is-instance[UUID]',),
+            'msg': 'Input should be an instance of UUID',
             'input': 'ebcdab58-6eb8-46fb-a190-d07a3',
+            'ctx': {'class': 'UUID'},
+        },
+        {
+            'type': 'uuid_parsing',
+            'loc': ('function-after[uuid_validator(), union[str,bytes]]',),
+            'msg': 'Input should be a valid UUID, unable to parse string as an UUID',
+            'input': 'ebcdab58-6eb8-46fb-a190-d07a3',
+        },
+    ]
+
+    not_a_valid_input_type = object()
+    with pytest.raises(ValidationError) as exc_info:
+        v.validate_python(not_a_valid_input_type)
+    # insert_assert(exc_info.value.errors(include_url=False))
+    assert exc_info.value.errors(include_url=False) == [
+        {
+            'type': 'is_instance_of',
+            'loc': ('is-instance[UUID]',),
+            'msg': 'Input should be an instance of UUID',
+            'input': not_a_valid_input_type,
+            'ctx': {'class': 'UUID'},
+        },
+        {
+            'type': 'string_type',
+            'loc': ('function-after[uuid_validator(), union[str,bytes]]', 'str'),
+            'msg': 'Input should be a valid string',
+            'input': not_a_valid_input_type,
+        },
+        {
+            'type': 'bytes_type',
+            'loc': ('function-after[uuid_validator(), union[str,bytes]]', 'bytes'),
+            'msg': 'Input should be a valid bytes',
+            'input': not_a_valid_input_type,
+        },
+    ]
+
+    with pytest.raises(ValidationError) as exc_info:
+        v.validate_python(valid.hex, strict=True)
+    # insert_assert(exc_info.value.errors(include_url=False))
+    assert exc_info.value.errors(include_url=False) == [
+        {
+            'type': 'is_instance_of',
+            'loc': (),
+            'msg': 'Input should be an instance of UUID',
+            'input': '49fdfa1d856d4003a83e4b9236532ec6',
+            'ctx': {'class': 'UUID'},
         }
     ]
 
-    with pytest.raises(ValidationError, match='Input should be a valid UUID, string, or bytes'):
-        Model(v=None)
+    assert v.validate_json(json.dumps(valid.hex), strict=True) == valid
 
 
 def test_uuid_json():
     class Model(BaseModel):
         v: UUID
         v1: UUID1
         v3: UUID3
         v4: UUID4
 
     m = Model(v=uuid.uuid4(), v1=uuid.uuid1(), v3=uuid.uuid3(uuid.NAMESPACE_DNS, 'python.org'), v4=uuid.uuid4())
     assert m.model_dump_json() == f'{{"v":"{m.v}","v1":"{m.v1}","v3":"{m.v3}","v4":"{m.v4}"}}'
 
 
-@pytest.mark.xfail(sys.platform.startswith('win'), reason='https://github.com/PyO3/pyo3/issues/2913', strict=False)
 def test_uuid_validation():
     class UUIDModel(BaseModel):
         a: UUID1
         b: UUID3
         c: UUID4
         d: UUID5
 
@@ -2756,14 +2959,28 @@
                     'ctx': {'whole_digits': 2},
                 }
             ],
         ),
         (dict(max_digits=4, decimal_places=1), Decimal('999'), Decimal('999')),
         (dict(max_digits=20, decimal_places=2), Decimal('742403889818000000'), Decimal('742403889818000000')),
         (dict(max_digits=20, decimal_places=2), Decimal('7.42403889818E+17'), Decimal('7.42403889818E+17')),
+        (dict(max_digits=6, decimal_places=2), Decimal('000000000001111.700000'), Decimal('000000000001111.700000')),
+        (
+            dict(max_digits=6, decimal_places=2),
+            Decimal('0000000000011111.700000'),
+            [
+                {
+                    'type': 'decimal_whole_digits',
+                    'loc': ('foo',),
+                    'msg': 'ensure that there are no more than 4 digits before the decimal point',
+                    'input': Decimal('11111.700000'),
+                    'ctx': {'whole_digits': 4},
+                }
+            ],
+        ),
         (
             dict(max_digits=20, decimal_places=2),
             Decimal('7424742403889818000000'),
             [
                 {
                     'type': 'decimal_max_digits',
                     'loc': ('foo',),
@@ -2787,23 +3004,23 @@
                     'input': Decimal('7.304'),
                     'ctx': {'decimal_places': 2},
                 }
             ],
         ),
         (dict(max_digits=5, decimal_places=5), Decimal('70E-5'), Decimal('70E-5')),
         (
-            dict(max_digits=5, decimal_places=5),
+            dict(max_digits=4, decimal_places=4),
             Decimal('70E-6'),
             [
                 {
                     'loc': ('foo',),
-                    'msg': 'ensure that there are no more than 5 digits in total',
+                    'msg': 'ensure that there are no more than 4 digits in total',
                     'type': 'decimal_max_digits',
-                    'input': Decimal('0.000070'),
-                    'ctx': {'max_digits': 5},
+                    'input': Decimal('0.00007'),
+                    'ctx': {'max_digits': 4},
                 }
             ],
         ),
         *[
             (
                 dict(decimal_places=2, max_digits=10, allow_inf_nan=False),
                 value,
@@ -2920,14 +3137,23 @@
     class Model(BaseModel):
         foo: Path
 
     assert Model(foo=value).foo == result
     assert Model.model_validate_json(json.dumps({'foo': str(value)})).foo == result
 
 
+def test_path_validation_constrained():
+    ta = TypeAdapter(Annotated[Path, Field(min_length=9, max_length=20)])
+    with pytest.raises(ValidationError):
+        ta.validate_python('/short')
+    with pytest.raises(ValidationError):
+        ta.validate_python('/' + 'long' * 100)
+    assert ta.validate_python('/just/right/enough') == Path('/just/right/enough')
+
+
 def test_path_like():
     class Model(BaseModel):
         foo: os.PathLike
 
     assert Model(foo='/foo/bar').foo == Path('/foo/bar')
     assert Model(foo=Path('/foo/bar')).foo == Path('/foo/bar')
     assert Model.model_validate_json('{"foo": "abc"}').foo == Path('abc')
@@ -2963,15 +3189,27 @@
     class Model(BaseModel):
         foo: Path
 
     with pytest.raises(ValidationError) as exc_info:
         Model(foo=123)
     # insert_assert(exc_info.value.errors(include_url=False))
     assert exc_info.value.errors(include_url=False) == [
-        {'type': 'path_type', 'loc': ('foo',), 'msg': 'Input is not a valid path', 'input': 123}
+        {
+            'type': 'is_instance_of',
+            'loc': ('foo', 'json-or-python[json=function-after[path_validator(), str],python=is-instance[Path]]'),
+            'msg': 'Input should be an instance of Path',
+            'input': 123,
+            'ctx': {'class': 'Path'},
+        },
+        {
+            'type': 'string_type',
+            'loc': ('foo', 'function-after[path_validator(), str]'),
+            'msg': 'Input should be a valid string',
+            'input': 123,
+        },
     ]
 
 
 def test_path_validation_strict():
     class Model(BaseModel):
         foo: Path
 
@@ -3044,14 +3282,58 @@
             'loc': ('foo',),
             'msg': 'Path does not point to a directory',
             'input': value,
         }
     ]
 
 
+@pytest.mark.parametrize('value', ('tests/test_types.py', Path('tests/test_types.py')))
+def test_new_path_validation_path_already_exists(value):
+    class Model(BaseModel):
+        foo: NewPath
+
+    with pytest.raises(ValidationError) as exc_info:
+        Model(foo=value)
+    assert exc_info.value.errors(include_url=False) == [
+        {
+            'type': 'path_exists',
+            'loc': ('foo',),
+            'msg': 'Path already exists',
+            'input': value,
+        }
+    ]
+
+
+@pytest.mark.parametrize('value', ('/nonexistentdir/foo.py', Path('/nonexistentdir/foo.py')))
+def test_new_path_validation_parent_does_not_exist(value):
+    class Model(BaseModel):
+        foo: NewPath
+
+    with pytest.raises(ValidationError) as exc_info:
+        Model(foo=value)
+    assert exc_info.value.errors(include_url=False) == [
+        {
+            'type': 'parent_does_not_exist',
+            'loc': ('foo',),
+            'msg': 'Parent directory does not exist',
+            'input': value,
+        }
+    ]
+
+
+@pytest.mark.parametrize(
+    'value,result', (('tests/foo.py', Path('tests/foo.py')), (Path('tests/foo.py'), Path('tests/foo.py')))
+)
+def test_new_path_validation_success(value, result):
+    class Model(BaseModel):
+        foo: NewPath
+
+    assert Model(foo=value).foo == result
+
+
 def test_number_gt():
     class Model(BaseModel):
         a: conint(gt=-1) = 0
 
     assert Model(a=0).model_dump() == {'a': 0}
 
     with pytest.raises(ValidationError) as exc_info:
@@ -3438,53 +3720,112 @@
     assert JsonRequired(json_obj='["x", "y", "z"]').model_dump() == {'json_obj': ['x', 'y', 'z']}
     with pytest.raises(ValidationError, match=r'JSON input should be string, bytes or bytearray \[type=json_type,'):
         JsonRequired(json_obj=None)
     with pytest.raises(ValidationError, match=r'Field required \[type=missing,'):
         JsonRequired()
 
 
-@pytest.mark.parametrize('pattern_type', [re.Pattern, Pattern])
-def test_pattern(pattern_type):
+@pytest.mark.parametrize(
+    ('pattern_type', 'pattern_value', 'matching_value', 'non_matching_value'),
+    [
+        pytest.param(re.Pattern, r'^whatev.r\d$', 'whatever1', ' whatever1', id='re.Pattern'),
+        pytest.param(Pattern, r'^whatev.r\d$', 'whatever1', ' whatever1', id='Pattern'),
+        pytest.param(Pattern[str], r'^whatev.r\d$', 'whatever1', ' whatever1', id='Pattern[str]'),
+        pytest.param(Pattern[bytes], rb'^whatev.r\d$', b'whatever1', b' whatever1', id='Pattern[bytes]'),
+    ],
+)
+def test_pattern(pattern_type, pattern_value, matching_value, non_matching_value):
     class Foobar(BaseModel):
         pattern: pattern_type
 
-    f = Foobar(pattern=r'^whatev.r\d$')
+    f = Foobar(pattern=pattern_value)
     assert f.pattern.__class__.__name__ == 'Pattern'
     # check it's really a proper pattern
-    assert f.pattern.match('whatever1')
-    assert not f.pattern.match(' whatever1')
+    assert f.pattern.match(matching_value)
+    assert not f.pattern.match(non_matching_value)
 
     # Check that pre-compiled patterns are accepted unchanged
-    p = re.compile(r'^whatev.r\d$')
+    p = re.compile(pattern_value)
     f2 = Foobar(pattern=p)
     assert f2.pattern is p
 
     # assert Foobar.model_json_schema() == {
     #     'type': 'object',
     #     'title': 'Foobar',
     #     'properties': {'pattern': {'type': 'string', 'format': 'regex', 'title': 'Pattern'}},
     #     'required': ['pattern'],
     # }
 
 
-@pytest.mark.parametrize('pattern_type', [re.Pattern, Pattern])
-def test_pattern_error(pattern_type):
+@pytest.mark.parametrize(
+    ('pattern_type', 'pattern_value', 'error_type', 'error_msg'),
+    [
+        pytest.param(
+            re.Pattern,
+            '[xx',
+            'pattern_regex',
+            'Input should be a valid regular expression',
+            id='re.Pattern-pattern_regex',
+        ),
+        pytest.param(
+            Pattern, '[xx', 'pattern_regex', 'Input should be a valid regular expression', id='re.Pattern-pattern_regex'
+        ),
+        pytest.param(
+            re.Pattern, (), 'pattern_type', 'Input should be a valid pattern', id='typing.Pattern-pattern_type'
+        ),
+        pytest.param(Pattern, (), 'pattern_type', 'Input should be a valid pattern', id='typing.Pattern-pattern_type'),
+        pytest.param(
+            Pattern[str],
+            re.compile(b''),
+            'pattern_str_type',
+            'Input should be a string pattern',
+            id='typing.Pattern[str]-pattern_str_type-non_str',
+        ),
+        pytest.param(
+            Pattern[str],
+            b'',
+            'pattern_str_type',
+            'Input should be a string pattern',
+            id='typing.Pattern[str]-pattern_str_type-bytes',
+        ),
+        pytest.param(
+            Pattern[str], (), 'pattern_type', 'Input should be a valid pattern', id='typing.Pattern[str]-pattern_type'
+        ),
+        pytest.param(
+            Pattern[bytes],
+            re.compile(''),
+            'pattern_bytes_type',
+            'Input should be a bytes pattern',
+            id='typing.Pattern[bytes]-pattern_bytes_type-non_bytes',
+        ),
+        pytest.param(
+            Pattern[bytes],
+            '',
+            'pattern_bytes_type',
+            'Input should be a bytes pattern',
+            id='typing.Pattern[bytes]-pattern_bytes_type-str',
+        ),
+        pytest.param(
+            Pattern[bytes],
+            (),
+            'pattern_type',
+            'Input should be a valid pattern',
+            id='typing.Pattern[bytes]-pattern_type',
+        ),
+    ],
+)
+def test_pattern_error(pattern_type, pattern_value, error_type, error_msg):
     class Foobar(BaseModel):
         pattern: pattern_type
 
     with pytest.raises(ValidationError) as exc_info:
-        Foobar(pattern='[xx')
+        Foobar(pattern=pattern_value)
     # insert_assert(exc_info.value.errors(include_url=False))
     assert exc_info.value.errors(include_url=False) == [
-        {
-            'type': 'pattern_regex',
-            'loc': ('pattern',),
-            'msg': 'Input should be a valid regular expression',
-            'input': '[xx',
-        }
+        {'type': error_type, 'loc': ('pattern',), 'msg': error_msg, 'input': pattern_value}
     ]
 
 
 def test_secretstr():
     class Foobar(BaseModel):
         password: SecretStr
         empty_password: SecretStr
@@ -3497,14 +3838,16 @@
     assert f.empty_password.__class__.__name__ == 'SecretStr'
 
     # Assert str and repr are correct.
     assert str(f.password) == '**********'
     assert str(f.empty_password) == ''
     assert repr(f.password) == "SecretStr('**********')"
     assert repr(f.empty_password) == "SecretStr('')"
+    assert len(f.password) == 4
+    assert len(f.empty_password) == 0
 
     # Assert retrieval of secret value is correct
     assert f.password.get_secret_value() == '1234'
     assert f.empty_password.get_secret_value() == ''
 
 
 def test_secretstr_is_secret_field():
@@ -3544,14 +3887,15 @@
         NonPositiveFloat,
         NonNegativeFloat,
         StrictFloat,
         FiniteFloat,
         conbytes,
         SecretBytes,
         constr,
+        SecretField,
         StrictStr,
         SecretStr,
         ImportString,
         conset,
         confrozenset,
         conlist,
         condecimal,
@@ -3563,14 +3907,16 @@
         DirectoryPath,
         NewPath,
         Json,
         ByteSize,
         condate,
         PastDate,
         FutureDate,
+        PastDatetime,
+        FutureDatetime,
         AwareDatetime,
         NaiveDatetime,
     ],
 )
 def test_is_hashable(pydantic_type):
     assert type(hash(pydantic_type)) is int
 
@@ -3595,14 +3941,22 @@
             'loc': ('password',),
             'msg': 'Input should be a valid string',
             'input': [6, 23, 'abc'],
         }
     ]
 
 
+def test_secret_str_hashable():
+    assert type(hash(SecretStr('abs'))) is int
+
+
+def test_secret_bytes_hashable():
+    assert type(hash(SecretBytes(b'abs'))) is int
+
+
 def test_secret_str_min_max_length():
     class Foobar(BaseModel):
         password: SecretStr = Field(min_length=6, max_length=10)
 
     with pytest.raises(ValidationError) as exc_info:
         Foobar(password='')
 
@@ -3807,19 +4161,20 @@
             'msg': "Input should be 'a' or 'b'",
             'input': 'c',
             'ctx': {'expected': "'a' or 'b'"},
         }
     ]
 
 
-def test_unsupported_field_type():
-    with pytest.raises(TypeError, match=r'Unable to generate pydantic-core schema MutableSet'):
-
-        class UnsupportedModel(BaseModel):
-            unsupported: MutableSet[int]
+def test_typing_mutable_set():
+    s1 = TypeAdapter(Set[int]).core_schema
+    s1.pop('metadata', None)
+    s2 = TypeAdapter(typing.MutableSet[int]).core_schema
+    s2.pop('metadata', None)
+    assert s1 == s2
 
 
 def test_frozenset_field():
     class FrozenSetModel(BaseModel):
         set: FrozenSet[int]
 
     test_set = frozenset({1, 2, 3})
@@ -3938,14 +4293,24 @@
             deque([10, 20, 30]),
         ),
         (
             Tuple[int, int],
             {1: 10, 2: 20, 3: 30}.items(),
             deque([(1, 10), (2, 20), (3, 30)]),
         ),
+        (
+            float,
+            {1, 2, 3},
+            deque([1, 2, 3]),
+        ),
+        (
+            float,
+            frozenset((1, 2, 3)),
+            deque([1, 2, 3]),
+        ),
     ),
 )
 def test_deque_generic_success(cls, value, result):
     class Model(BaseModel):
         v: Deque[cls]
 
     assert Model(v=value).v == result
@@ -3967,34 +4332,14 @@
     assert Model(v=value).v == result
 
 
 @pytest.mark.parametrize(
     'cls,value,expected_error',
     (
         (
-            float,
-            {1, 2, 3},
-            {
-                'type': 'list_type',
-                'loc': ('v',),
-                'msg': 'Input should be a valid list',
-                'input': {1, 2, 3},
-            },
-        ),
-        (
-            float,
-            frozenset((1, 2, 3)),
-            {
-                'type': 'list_type',
-                'loc': ('v',),
-                'msg': 'Input should be a valid list',
-                'input': frozenset((1, 2, 3)),
-            },
-        ),
-        (
             int,
             [1, 'a', 3],
             {
                 'type': 'int_parsing',
                 'loc': ('v', 1),
                 'msg': 'Input should be a valid integer, unable to parse string as an integer',
                 'input': 'a',
@@ -4104,14 +4449,46 @@
         field: Deque[int] = deque(maxlen=5)
 
     assert DequeModel3().field.maxlen == 5
     assert DequeModel3(field=deque()).field.maxlen is None
     assert DequeModel3(field=deque(maxlen=8)).field.maxlen == 8
 
 
+def test_deque_set_maxlen():
+    class DequeModel1(BaseModel):
+        field: Annotated[Deque[int], Field(max_length=10)]
+
+    assert DequeModel1(field=deque()).field.maxlen == 10
+    assert DequeModel1(field=deque(maxlen=8)).field.maxlen == 8
+    assert DequeModel1(field=deque(maxlen=15)).field.maxlen == 10
+
+    class DequeModel2(BaseModel):
+        field: Annotated[Deque[int], Field(max_length=10)] = deque()
+
+    assert DequeModel2().field.maxlen is None
+    assert DequeModel2(field=deque()).field.maxlen == 10
+    assert DequeModel2(field=deque(maxlen=8)).field.maxlen == 8
+    assert DequeModel2(field=deque(maxlen=15)).field.maxlen == 10
+
+    class DequeModel3(DequeModel2):
+        model_config = ConfigDict(validate_default=True)
+
+    assert DequeModel3().field.maxlen == 10
+
+    class DequeModel4(BaseModel):
+        field: Annotated[Deque[int], Field(max_length=10)] = deque(maxlen=5)
+
+    assert DequeModel4().field.maxlen == 5
+
+    class DequeModel5(DequeModel4):
+        model_config = ConfigDict(validate_default=True)
+
+    assert DequeModel4().field.maxlen == 5
+
+
 @pytest.mark.parametrize('value_type', (None, type(None), None.__class__))
 def test_none(value_type):
     class Model(BaseModel):
         my_none: value_type
         my_none_list: List[value_type]
         my_none_dict: Dict[str, value_type]
         my_json_none: Json[value_type]
@@ -4334,15 +4711,19 @@
     assert M(d=dict(foo='baz')).d == {'foo': 'baz'}
 
 
 def test_custom_generic_containers():
     T = TypeVar('T')
 
     class GenericList(List[T]):
-        pass
+        @classmethod
+        def __get_pydantic_core_schema__(cls, source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
+            return core_schema.no_info_after_validator_function(
+                GenericList, handler.generate_schema(List[get_args(source_type)[0]])
+            )
 
     class Model(BaseModel):
         field: GenericList[int]
 
     model = Model(field=['1', '2'])
     assert model.field == [1, 2]
     assert isinstance(model.field, GenericList)
@@ -4469,17 +4850,17 @@
             """
 
             def validate_from_int(value: int, _validation_info: Optional[ValidationInfo] = None) -> ThirdPartyType:
                 result = ThirdPartyType()
                 result.x = value
                 return result
 
-            instance_validation_schema = core_schema.is_instance_schema(
-                ThirdPartyType,
-                json_function=validate_from_int,
+            instance_validation_schema = core_schema.json_or_python_schema(
+                json_schema=core_schema.no_info_after_validator_function(validate_from_int, core_schema.int_schema()),
+                python_schema=core_schema.is_instance_schema(ThirdPartyType),
             )
             int_validation_schema = core_schema.chain_schema(
                 [core_schema.int_schema(), core_schema.general_plain_validator_function(validate_from_int)]
             )
             return core_schema.union_schema(
                 [instance_validation_schema, int_validation_schema],
                 serialization=core_schema.plain_serializer_function_ser_schema(lambda instance: instance.x),
@@ -4517,27 +4898,657 @@
     assert m_instance.model_dump() == {'third_party_type': 10}
 
     # Demonstrate that validation errors are raised as expected for invalid inputs
     with pytest.raises(ValidationError) as exc_info:
         Model(third_party_type='a')
     assert exc_info.value.errors(include_url=False) == [
         {
-            'ctx': {'class': 'test_third_party_type_integration.<locals>.ThirdPartyType'},
-            'input': 'a',
-            'loc': ('third_party_type', 'is-instance[test_third_party_type_integration.<locals>.ThirdPartyType]'),
-            'msg': 'Input should be an instance of test_third_party_type_integration.<locals>.ThirdPartyType',
             'type': 'is_instance_of',
+            'loc': (
+                'third_party_type',
+                'json-or-python[json=function-after[validate_from_int(), int],python=is-instance[test_third_party_type_integration.<locals>.ThirdPartyType]]',  # noqa: E501
+            ),
+            'msg': 'Input should be an instance of test_third_party_type_integration.<locals>.ThirdPartyType',
+            'input': 'a',
+            'ctx': {'class': 'test_third_party_type_integration.<locals>.ThirdPartyType'},
         },
         {
-            'input': 'a',
-            'loc': ('third_party_type', 'chain[int,function-plain[validate_from_int()]]'),
-            'msg': 'Input should be a valid integer, unable to parse string as an ' 'integer',
             'type': 'int_parsing',
+            'loc': ('third_party_type', 'chain[int,function-plain[validate_from_int()]]'),
+            'msg': 'Input should be a valid integer, unable to parse string as an integer',
+            'input': 'a',
         },
     ]
 
     assert Model.model_json_schema() == {
         'properties': {'third_party_type': {'title': 'Third Party Type', 'type': 'integer'}},
         'required': ['third_party_type'],
         'title': 'Model',
         'type': 'object',
     }
+
+
+def test_sequence_subclass_without_core_schema() -> None:
+    class MyList(List[int]):
+        # The point of this is that subclasses can do arbitrary things
+        # This is the reason why we don't try to handle them automatically
+        # TBD if we introspect `__init__` / `__new__`
+        # (which is the main thing that would mess us up if modified in a subclass)
+        # and automatically handle cases where the subclass doesn't override it.
+        # There's still edge cases (again, arbitrary behavior...)
+        # and it's harder to explain, but could lead to a better user experience in some cases
+        # It will depend on how the complaints (which have and will happen in both directions)
+        # balance out
+        def __init__(self, *args: Any, required: int, **kwargs: Any) -> None:
+            super().__init__(*args, **kwargs)
+
+    with pytest.raises(
+        PydanticSchemaGenerationError, match='implement `__get_pydantic_core_schema__` on your type to fully support it'
+    ):
+
+        class _(BaseModel):
+            x: MyList
+
+
+def test_typing_coercion_defaultdict():
+    class Model(BaseModel):
+        x: DefaultDict[int, str]
+
+    d = defaultdict(str)
+    d['1']
+    m = Model(x=d)
+    assert isinstance(m.x, defaultdict)
+    assert repr(m.x) == "defaultdict(<class 'str'>, {1: ''})"
+
+
+def test_typing_coercion_counter():
+    class Model(BaseModel):
+        x: Counter[str]
+
+    m = Model(x={'a': 10})
+    assert isinstance(m.x, Counter)
+    assert repr(m.x) == "Counter({'a': 10})"
+
+
+def test_typing_counter_value_validation():
+    class Model(BaseModel):
+        x: Counter[str]
+
+    with pytest.raises(ValidationError) as exc_info:
+        Model(x={'a': 'a'})
+
+    # insert_assert(exc_info.value.errors(include_url=False))
+    assert exc_info.value.errors(include_url=False) == [
+        {
+            'type': 'int_parsing',
+            'loc': ('x', 'a'),
+            'msg': 'Input should be a valid integer, unable to parse string as an integer',
+            'input': 'a',
+        }
+    ]
+
+
+def test_mapping_subclass_without_core_schema() -> None:
+    class MyDict(Dict[int, int]):
+        # The point of this is that subclasses can do arbitrary things
+        # This is the reason why we don't try to handle them automatically
+        # TBD if we introspect `__init__` / `__new__`
+        # (which is the main thing that would mess us up if modified in a subclass)
+        # and automatically handle cases where the subclass doesn't override it.
+        # There's still edge cases (again, arbitrary behavior...)
+        # and it's harder to explain, but could lead to a better user experience in some cases
+        # It will depend on how the complaints (which have and will happen in both directions)
+        # balance out
+        def __init__(self, *args: Any, required: int, **kwargs: Any) -> None:
+            super().__init__(*args, **kwargs)
+
+    with pytest.raises(
+        PydanticSchemaGenerationError, match='implement `__get_pydantic_core_schema__` on your type to fully support it'
+    ):
+
+        class _(BaseModel):
+            x: MyDict
+
+
+def test_defaultdict_unknown_default_factory() -> None:
+    """
+    https://github.com/pydantic/pydantic/issues/4687
+    """
+    with pytest.raises(
+        PydanticSchemaGenerationError,
+        match=r'Unable to infer a default factory for with keys of type typing.DefaultDict\[int, int\]',
+    ):
+
+        class Model(BaseModel):
+            d: DefaultDict[int, DefaultDict[int, int]]
+
+
+def test_defaultdict_infer_default_factory() -> None:
+    class Model(BaseModel):
+        a: DefaultDict[int, List[int]]
+        b: DefaultDict[int, int]
+
+    m = Model(a={}, b={})
+    assert m.a.default_factory is not None
+    assert m.a.default_factory() == []
+    assert m.b.default_factory is not None
+    assert m.b.default_factory() == 0
+
+
+def test_defaultdict_explicit_default_factory() -> None:
+    class MyList(List[int]):
+        pass
+
+    class Model(BaseModel):
+        a: DefaultDict[int, Annotated[List[int], Field(default_factory=lambda: MyList())]]
+
+    m = Model(a={})
+    assert m.a.default_factory is not None
+    assert isinstance(m.a.default_factory(), MyList)
+
+
+def test_defaultdict_default_factory_preserved() -> None:
+    class Model(BaseModel):
+        a: DefaultDict[int, List[int]]
+
+    class MyList(List[int]):
+        pass
+
+    m = Model(a=defaultdict(lambda: MyList()))
+    assert m.a.default_factory is not None
+    assert isinstance(m.a.default_factory(), MyList)
+
+
+def test_custom_default_dict() -> None:
+    KT = TypeVar('KT')
+    VT = TypeVar('VT')
+
+    class CustomDefaultDict(DefaultDict[KT, VT]):
+        @classmethod
+        def __get_pydantic_core_schema__(cls, source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
+            keys_type, values_type = get_args(source_type)
+            return core_schema.no_info_after_validator_function(
+                lambda x: cls(x.default_factory, x), handler.generate_schema(DefaultDict[keys_type, values_type])
+            )
+
+    ta = TypeAdapter(CustomDefaultDict[str, int])
+
+    assert ta.validate_python({'a': 1}) == CustomDefaultDict(int, {'a': 1})
+
+
+@pytest.mark.parametrize('field_type', [typing.OrderedDict, collections.OrderedDict])
+def test_ordered_dict_from_ordered_dict(field_type):
+    class Model(BaseModel):
+        od_field: field_type
+
+    od_value = collections.OrderedDict([('a', 1), ('b', 2)])
+
+    m = Model(od_field=od_value)
+
+    assert isinstance(m.od_field, collections.OrderedDict)
+    assert m.od_field == od_value
+    # we don't make any promises about preserving instances
+    # at the moment we always copy them for consistency and predictability
+    # so this is more so documenting the current behavior than a promise
+    # we make to users
+    assert m.od_field is not od_value
+
+    assert m.model_json_schema() == {
+        'properties': {'od_field': {'title': 'Od Field', 'type': 'object'}},
+        'required': ['od_field'],
+        'title': 'Model',
+        'type': 'object',
+    }
+
+
+def test_ordered_dict_from_ordered_dict_typed():
+    class Model(BaseModel):
+        od_field: typing.OrderedDict[str, int]
+
+    od_value = collections.OrderedDict([('a', 1), ('b', 2)])
+
+    m = Model(od_field=od_value)
+
+    assert isinstance(m.od_field, collections.OrderedDict)
+    assert m.od_field == od_value
+
+    assert m.model_json_schema() == {
+        'properties': {
+            'od_field': {
+                'additionalProperties': {'type': 'integer'},
+                'title': 'Od Field',
+                'type': 'object',
+            }
+        },
+        'required': ['od_field'],
+        'title': 'Model',
+        'type': 'object',
+    }
+
+
+@pytest.mark.parametrize('field_type', [typing.OrderedDict, collections.OrderedDict])
+def test_ordered_dict_from_dict(field_type):
+    class Model(BaseModel):
+        od_field: field_type
+
+    od_value = {'a': 1, 'b': 2}
+
+    m = Model(od_field=od_value)
+
+    assert isinstance(m.od_field, collections.OrderedDict)
+    assert m.od_field == collections.OrderedDict(od_value)
+
+    assert m.model_json_schema() == {
+        'properties': {'od_field': {'title': 'Od Field', 'type': 'object'}},
+        'required': ['od_field'],
+        'title': 'Model',
+        'type': 'object',
+    }
+
+
+def test_handle_3rd_party_custom_type_reusing_known_metadata() -> None:
+    class PdDecimal(Decimal):
+        def ___repr__(self) -> str:
+            return f'PdDecimal({super().__repr__()})'
+
+    class PdDecimalMarker:
+        def __get_pydantic_core_schema__(self, source_type: Any, handler: GetCoreSchemaHandler) -> CoreSchema:
+            return core_schema.no_info_after_validator_function(PdDecimal, handler(source_type))
+
+        def __prepare_pydantic_annotations__(
+            self, _source: Any, annotations: Tuple[Any, ...], _config: ConfigDict
+        ) -> Tuple[Any, Iterable[Any]]:
+            return Decimal, [self, *annotations]
+
+    class Model(BaseModel):
+        x: Annotated[PdDecimal, PdDecimalMarker(), annotated_types.Gt(0)]
+
+    assert isinstance(Model(x=1).x, PdDecimal)
+    with pytest.raises(ValidationError) as exc_info:
+        Model(x=-1)
+    assert exc_info.value.errors(include_url=False) == [
+        {'type': 'greater_than', 'loc': ('x',), 'msg': 'Input should be greater than 0', 'input': -1, 'ctx': {'gt': 0}}
+    ]
+
+
+def test_skip_validation():
+    @validate_call
+    def my_function(y: Annotated[int, SkipValidation]):
+        return repr(y)
+
+    assert my_function('2') == "'2'"
+
+
+def test_skip_validation_serialization():
+    class A(BaseModel):
+        x: SkipValidation[int]
+
+        @field_serializer('x')
+        def double_x(self, v):
+            return v * 2
+
+    assert A(x=1).model_dump() == {'x': 2}
+    assert A(x='abc').model_dump() == {'x': 'abcabc'}  # no validation
+    assert A(x='abc').model_dump_json() == '{"x":"abcabc"}'
+
+
+def test_skip_validation_json_schema():
+    class A(BaseModel):
+        x: SkipValidation[int]
+
+    assert A.model_json_schema() == {
+        'properties': {'x': {'title': 'X', 'type': 'integer'}},
+        'required': ['x'],
+        'title': 'A',
+        'type': 'object',
+    }
+
+
+def test_transform_schema_for_first_party_class():
+    # Here, first party means you can define the `__prepare_pydantic_annotations__` method on the class directly.
+    class LowercaseStr(str):
+        @classmethod
+        def __prepare_pydantic_annotations__(
+            cls, _source: Type[Any], annotations: Tuple[Any, ...], _config: ConfigDict
+        ) -> Tuple[Any, Iterable[Any]]:
+            def transform_schema(schema: CoreSchema) -> CoreSchema:
+                return core_schema.no_info_after_validator_function(lambda v: v.lower(), schema)
+
+            return str, (*annotations, TransformSchema(transform_schema))
+
+    class Model(BaseModel):
+        lower: LowercaseStr = Field(min_length=1)
+
+    assert Model(lower='ABC').lower == 'abc'
+
+    with pytest.raises(ValidationError) as exc_info:
+        Model(lower='')
+    assert exc_info.value.errors(include_url=False) == [
+        {
+            'ctx': {'min_length': 1},
+            'input': '',
+            'loc': ('lower',),
+            'msg': 'String should have at least 1 characters',
+            'type': 'string_too_short',
+        }
+    ]
+
+
+def test_transform_schema_for_third_party_class():
+    # Here, third party means you can't define methods on the class directly, so have to use annotations.
+
+    class DatetimeWrapper:
+        # This is pretending to be a third-party class. This example is specifically inspired by pandas.Timestamp,
+        # which can receive an item of type `datetime` as an input to its `__init__`.
+        # The important thing here is we are not defining any custom methods on this type directly.
+        def __init__(self, t: datetime):
+            self.t = t
+
+    class _DatetimeWrapperAnnotation:
+        # This is an auxiliary class that, when used as the first annotation for DatetimeWrapper,
+        # ensures pydantic can produce a valid schema.
+        @classmethod
+        def __prepare_pydantic_annotations__(
+            cls, _source: Type[Any], annotations: Tuple[Any, ...], _config: ConfigDict
+        ) -> Tuple[Any, Iterable[Any]]:
+            def transform(schema: CoreSchema) -> CoreSchema:
+                return core_schema.no_info_after_validator_function(lambda v: DatetimeWrapper(v), schema)
+
+            return datetime, list(annotations) + [TransformSchema(transform)]
+
+    # Giving a name to Annotated[DatetimeWrapper, _DatetimeWrapperAnnotation] makes it easier to use in code
+    # where I want a field of type `DatetimeWrapper` that works as desired with pydantic.
+    PydanticDatetimeWrapper = Annotated[DatetimeWrapper, _DatetimeWrapperAnnotation]
+
+    class Model(BaseModel):
+        # The reason all of the above is necessary is specifically so that we get good behavior
+        timestamp: Annotated[PydanticDatetimeWrapper, annotated_types.Gt(datetime.fromisoformat('2020-01-01 00:00:00'))]
+
+    m = Model(timestamp='2021-01-01 00:00:00')
+    assert isinstance(m.timestamp, DatetimeWrapper)
+    assert repr(m.timestamp.t) == 'datetime.datetime(2021, 1, 1, 0, 0)'
+
+    with pytest.raises(ValidationError) as exc_info:
+        Model(timestamp='2019-01-01 00:00:00')
+    assert exc_info.value.errors(include_url=False) == [
+        {
+            'ctx': {'gt': '2020-01-01T00:00:00'},
+            'input': '2019-01-01 00:00:00',
+            'loc': ('timestamp',),
+            'msg': 'Input should be greater than 2020-01-01T00:00:00',
+            'type': 'greater_than',
+        }
+    ]
+
+
+def test_iterable_arbitrary_type():
+    class CustomIterable(Iterable):
+        def __init__(self, iterable):
+            self.iterable = iterable
+
+        def __iter__(self):
+            return self
+
+        def __next__(self):
+            return next(self.iterable)
+
+    with pytest.raises(
+        PydanticSchemaGenerationError,
+        match='Unable to generate pydantic-core schema for .*CustomIterable.*. Set `arbitrary_types_allowed=True`',
+    ):
+
+        class Model(BaseModel):
+            x: CustomIterable
+
+
+def test_typing_extension_literal_field():
+    from typing_extensions import Literal
+
+    class Model(BaseModel):
+        foo: Literal['foo']
+
+    assert Model(foo='foo').foo == 'foo'
+
+
+@pytest.mark.skipif(sys.version_info < (3, 8), reason='`typing.Literal` is available for python 3.8 and above.')
+def test_typing_literal_field():
+    from typing import Literal
+
+    class Model(BaseModel):
+        foo: Literal['foo']
+
+    assert Model(foo='foo').foo == 'foo'
+
+
+def test_instance_of_annotation():
+    class Model(BaseModel):
+        x: InstanceOf[Sequence[int]]  # Note: the generic parameter gets ignored by runtime validation
+
+    class MyList(list):
+        pass
+
+    assert Model(x='abc').x == 'abc'
+    assert type(Model(x=MyList([1, 2, 3])).x) is MyList
+
+    with pytest.raises(ValidationError) as exc_info:
+        Model(x=1)
+    assert exc_info.value.errors(include_url=False) == [
+        {
+            'ctx': {'class': 'Sequence'},
+            'input': 1,
+            'loc': ('x',),
+            'msg': 'Input should be an instance of Sequence',
+            'type': 'is_instance_of',
+        }
+    ]
+
+    assert Model.model_validate_json('{"x": [1,2,3]}').x == [1, 2, 3]
+    with pytest.raises(ValidationError) as exc_info:
+        Model.model_validate_json('{"x": "abc"}')
+    assert exc_info.value.errors(include_url=False) == [
+        {'input': 'abc', 'loc': ('x',), 'msg': 'Input should be a valid array', 'type': 'list_type'}
+    ]
+
+
+def test_instanceof_invalid_core_schema():
+    class MyClass:
+        pass
+
+    class MyModel(BaseModel):
+        a: InstanceOf[MyClass]
+
+    MyModel(a=MyClass())
+    with pytest.raises(ValidationError) as exc_info:
+        MyModel(a=1)
+    assert exc_info.value.errors(include_url=False) == [
+        {
+            'ctx': {'class': 'test_instanceof_invalid_core_schema.<locals>.MyClass'},
+            'input': 1,
+            'loc': ('a',),
+            'msg': 'Input should be an instance of ' 'test_instanceof_invalid_core_schema.<locals>.MyClass',
+            'type': 'is_instance_of',
+        }
+    ]
+    with pytest.raises(
+        PydanticInvalidForJsonSchema, match='Cannot generate a JsonSchema for core_schema.IsInstanceSchema'
+    ):
+        MyModel.model_json_schema()
+
+
+def test_constraints_arbitrary_type() -> None:
+    class CustomType:
+        def __init__(self, v: Any) -> None:
+            self.v = v
+
+        def __eq__(self, o: object) -> bool:
+            return self.v == o
+
+        def __le__(self, o: object) -> bool:
+            return self.v <= o
+
+        def __lt__(self, o: object) -> bool:
+            return self.v < o
+
+        def __ge__(self, o: object) -> bool:
+            return self.v >= o
+
+        def __gt__(self, o: object) -> bool:
+            return self.v > o
+
+        def __mod__(self, o: Any) -> Any:
+            return self.v % o
+
+        def __len__(self) -> int:
+            return len(self.v)
+
+        def __repr__(self) -> str:
+            return f'CustomType({self.v})'
+
+    class Model(BaseModel):
+        gt: Annotated[CustomType, annotated_types.Gt(CustomType(0))]
+        ge: Annotated[CustomType, annotated_types.Ge(CustomType(0))]
+        lt: Annotated[CustomType, annotated_types.Lt(CustomType(0))]
+        le: Annotated[CustomType, annotated_types.Le(CustomType(0))]
+        multiple_of: Annotated[CustomType, annotated_types.MultipleOf(2)]
+        min_length: Annotated[CustomType, annotated_types.MinLen(1)]
+        max_length: Annotated[CustomType, annotated_types.MaxLen(1)]
+        predicate: Annotated[CustomType, annotated_types.Predicate(lambda x: x > 0)]
+
+        model_config = ConfigDict(arbitrary_types_allowed=True)
+
+    Model(
+        gt=CustomType(1),
+        ge=CustomType(0),
+        lt=CustomType(-1),
+        le=CustomType(0),
+        min_length=CustomType([1, 2]),
+        max_length=CustomType([]),
+        multiple_of=CustomType(4),
+        predicate=CustomType(1),
+    )
+
+    with pytest.raises(ValidationError) as exc_info:
+        Model(
+            gt=CustomType(-1),
+            ge=CustomType(-1),
+            lt=CustomType(1),
+            le=CustomType(1),
+            min_length=CustomType([]),
+            max_length=CustomType([1, 2, 3]),
+            multiple_of=CustomType(3),
+            predicate=CustomType(-1),
+        )
+    # insert_assert(exc_info.value.errors(include_url=False))
+    assert exc_info.value.errors(include_url=False) == [
+        {
+            'type': 'greater_than',
+            'loc': ('gt',),
+            'msg': 'Input should be greater than CustomType(0)',
+            'input': CustomType(-1),
+            'ctx': {'gt': 'CustomType(0)'},
+        },
+        {
+            'type': 'greater_than_equal',
+            'loc': ('ge',),
+            'msg': 'Input should be greater than or equal to CustomType(0)',
+            'input': CustomType(-1),
+            'ctx': {'ge': 'CustomType(0)'},
+        },
+        {
+            'type': 'less_than',
+            'loc': ('lt',),
+            'msg': 'Input should be less than CustomType(0)',
+            'input': CustomType(1),
+            'ctx': {'lt': 'CustomType(0)'},
+        },
+        {
+            'type': 'less_than_equal',
+            'loc': ('le',),
+            'msg': 'Input should be less than or equal to CustomType(0)',
+            'input': CustomType(1),
+            'ctx': {'le': 'CustomType(0)'},
+        },
+        {
+            'type': 'multiple_of',
+            'loc': ('multiple_of',),
+            'msg': 'Input should be a multiple of 2',
+            'input': CustomType(3),
+            'ctx': {'multiple_of': 2},
+        },
+        {
+            'type': 'too_short',
+            'loc': ('min_length',),
+            'msg': 'Value should have at least 1 item after validation, not 0',
+            'input': CustomType([]),
+            'ctx': {'field_type': 'Value', 'min_length': 1, 'actual_length': 0},
+        },
+        {
+            'type': 'too_long',
+            'loc': ('max_length',),
+            'msg': 'Value should have at most 1 item after validation, not 3',
+            'input': CustomType([1, 2, 3]),
+            'ctx': {'field_type': 'Value', 'max_length': 1, 'actual_length': 3},
+        },
+        {
+            'type': 'predicate_failed',
+            'loc': ('predicate',),
+            'msg': 'Predicate test_constraints_arbitrary_type.<locals>.Model.<lambda> failed',
+            'input': CustomType(-1),
+            'ctx': {},
+        },
+    ]
+
+
+def test_annotated_default_value() -> None:
+    t = TypeAdapter(Annotated[List[int], Field(default=['1', '2'])])
+
+    r = t.get_default_value()
+    assert r is not None
+    assert r.value == ['1', '2']
+
+    # insert_assert(t.json_schema())
+    assert t.json_schema() == {'type': 'array', 'items': {'type': 'integer'}, 'default': ['1', '2']}
+
+
+def test_annotated_default_value_validate_default() -> None:
+    t = TypeAdapter(Annotated[List[int], Field(default=['1', '2'])], config=ConfigDict(validate_default=True))
+
+    r = t.get_default_value()
+    assert r is not None
+    assert r.value == [1, 2]
+
+    # insert_assert(t.json_schema())
+    assert t.json_schema() == {'type': 'array', 'items': {'type': 'integer'}, 'default': ['1', '2']}
+
+
+def test_annotated_default_value_functional_validator() -> None:
+    T = TypeVar('T')
+    WithAfterValidator = Annotated[T, AfterValidator(lambda x: [v * 2 for v in x])]
+    WithDefaultValue = Annotated[T, Field(default=['1', '2'])]
+
+    # the order of the args should not matter, we always put the default value on the outside
+    for tp in (WithDefaultValue[WithAfterValidator[List[int]]], WithAfterValidator[WithDefaultValue[List[int]]]):
+        t = TypeAdapter(tp, config=ConfigDict(validate_default=True))
+
+        r = t.get_default_value()
+        assert r is not None
+        assert r.value == [2, 4]
+
+        # insert_assert(t.json_schema())
+        assert t.json_schema() == {'type': 'array', 'items': {'type': 'integer'}, 'default': ['1', '2']}
+
+
+@pytest.mark.parametrize(
+    'pydantic_type,expected',
+    (
+        (Json, 'Json'),
+        (PastDate, 'PastDate'),
+        (FutureDate, 'FutureDate'),
+        (AwareDatetime, 'AwareDatetime'),
+        (NaiveDatetime, 'NaiveDatetime'),
+        (PastDatetime, 'PastDatetime'),
+        (FutureDatetime, 'FutureDatetime'),
+        (ImportString, 'ImportString'),
+    ),
+)
+def test_types_repr(pydantic_type, expected):
+    assert repr(pydantic_type()) == expected
```

### Comparing `pydantic-2.0a4/tests/test_types_namedtuple.py` & `pydantic-2.0b1/tests/test_types_namedtuple.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a4/tests/test_types_payment_card_number.py` & `pydantic-2.0b1/tests/test_types_payment_card_number.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a4/tests/test_types_typeddict.py` & `pydantic-2.0b1/tests/test_types_typeddict.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """
 Tests for TypedDict
 """
-import re
 import sys
 import typing
-from typing import Generic, List, Optional, TypeVar
+from typing import Any, Dict, Generic, List, Optional, TypeVar
 
 import pytest
 import typing_extensions
 from annotated_types import Lt
+from pydantic_core import core_schema
 from typing_extensions import Annotated, TypedDict
 
-from pydantic import BaseModel, Field, PositiveInt, PydanticUserError, ValidationError
+from pydantic import BaseModel, ConfigDict, Field, GetCoreSchemaHandler, PositiveInt, PydanticUserError, ValidationError
+from pydantic.functional_serializers import field_serializer, model_serializer
+from pydantic.functional_validators import field_validator, model_validator
 from pydantic.type_adapter import TypeAdapter
 
 from .conftest import Err
 
 
 @pytest.fixture(
     name='TypedDictAll',
@@ -32,15 +34,15 @@
 
 
 @pytest.fixture(name='TypedDict')
 def fixture_typed_dict(TypedDictAll):
     class TestTypedDict(TypedDictAll):
         foo: str
 
-    if sys.version_info < (3, 11) and TypedDictAll.__module__ == 'typing':
+    if sys.version_info < (3, 12) and TypedDictAll.__module__ == 'typing':
         pytest.skip('typing.TypedDict does not track required keys correctly on Python < 3.11')
 
     if hasattr(TestTypedDict, '__required_keys__'):
         return TypedDictAll
     else:
         pytest.skip('TypedDict does not include __required_keys__')
 
@@ -65,15 +67,15 @@
 
     try:
 
         class M(BaseModel):
             d: MyDict
 
     except PydanticUserError as e:
-        assert e.message == 'Please use `typing_extensions.TypedDict` instead of `typing.TypedDict` on Python < 3.11.'
+        assert e.message == 'Please use `typing_extensions.TypedDict` instead of `typing.TypedDict` on Python < 3.12.'
     else:
         assert M(d=dict(foo='baz')).d == {'foo': 'baz'}
 
 
 def test_typeddict_annotated_simple(TypedDict, req_no_req):
     Required, NotRequired = req_no_req
 
@@ -184,28 +186,84 @@
     ]
 
 
 def test_typeddict_schema(TypedDict):
     class Data(BaseModel):
         a: int
 
-    # TODO: Need to make sure TypedDict's get their own schema
     class DataTD(TypedDict):
         a: int
 
+    class CustomTD(TypedDict):
+        b: int
+
+        @classmethod
+        def __get_pydantic_core_schema__(
+            cls, source_type: Any, handler: GetCoreSchemaHandler
+        ) -> core_schema.CoreSchema:
+            schema = handler(source_type)
+            schema['computed_fields'] = [
+                core_schema.computed_field(property_name='another_b', return_schema=core_schema.int_schema())
+            ]
+            return schema
+
     class Model(BaseModel):
         data: Data
         data_td: DataTD
+        custom_td: CustomTD
 
-    assert Model.model_json_schema() == {
+    assert Model.model_json_schema(mode='validation') == {
         'title': 'Model',
         'type': 'object',
-        'properties': {'data': {'$ref': '#/$defs/Data'}, 'data_td': {'$ref': '#/$defs/DataTD'}},
-        'required': ['data', 'data_td'],
+        'properties': {
+            'custom_td': {'$ref': '#/$defs/CustomTD'},
+            'data': {'$ref': '#/$defs/Data'},
+            'data_td': {'$ref': '#/$defs/DataTD'},
+        },
+        'required': ['data', 'data_td', 'custom_td'],
         '$defs': {
+            'CustomTD': {
+                'type': 'object',
+                'title': 'CustomTD',
+                'properties': {'b': {'title': 'B', 'type': 'integer'}},
+                'required': ['b'],
+            },
+            'Data': {
+                'type': 'object',
+                'title': 'Data',
+                'properties': {'a': {'title': 'A', 'type': 'integer'}},
+                'required': ['a'],
+            },
+            'DataTD': {
+                'type': 'object',
+                'title': 'DataTD',
+                'properties': {'a': {'title': 'A', 'type': 'integer'}},
+                'required': ['a'],
+            },
+        },
+    }
+    assert Model.model_json_schema(mode='serialization') == {
+        'title': 'Model',
+        'type': 'object',
+        'properties': {
+            'custom_td': {'$ref': '#/$defs/CustomTD'},
+            'data': {'$ref': '#/$defs/Data'},
+            'data_td': {'$ref': '#/$defs/DataTD'},
+        },
+        'required': ['data', 'data_td', 'custom_td'],
+        '$defs': {
+            'CustomTD': {
+                'type': 'object',
+                'title': 'CustomTD',
+                'properties': {
+                    'b': {'title': 'B', 'type': 'integer'},
+                    'another_b': {'title': 'Another B', 'type': 'integer'},
+                },
+                'required': ['b', 'another_b'],
+            },
             'Data': {
                 'type': 'object',
                 'title': 'Data',
                 'properties': {'a': {'title': 'A', 'type': 'integer'}},
                 'required': ['a'],
             },
             'DataTD': {
@@ -407,33 +465,30 @@
     if isinstance(expected, Err):
         with pytest.raises(ValidationError, match=expected.message_escaped()):
             Model(d=input_value)
     else:
         assert Model(d=input_value).d == expected
 
 
-def test_recursive_typeddict(create_module):
-    @create_module
-    def module():
-        from typing import Optional
+def test_recursive_typeddict():
+    from typing import Optional
 
-        from typing_extensions import TypedDict
+    from typing_extensions import TypedDict
 
-        from pydantic import BaseModel
+    from pydantic import BaseModel
 
-        class RecursiveTypedDict(TypedDict):
-            # TODO: See if we can get this working if defined in a function (right now, needs to be module-level)
-            foo: Optional['RecursiveTypedDict']
+    class RecursiveTypedDict(TypedDict):
+        foo: Optional['RecursiveTypedDict']
 
-        class RecursiveTypedDictModel(BaseModel):
-            rec: RecursiveTypedDict
+    class RecursiveTypedDictModel(BaseModel):
+        rec: RecursiveTypedDict
 
-    assert module.RecursiveTypedDictModel(rec={'foo': {'foo': None}}).rec == {'foo': {'foo': None}}
+    assert RecursiveTypedDictModel(rec={'foo': {'foo': None}}).rec == {'foo': {'foo': None}}
     with pytest.raises(ValidationError) as exc_info:
-        module.RecursiveTypedDictModel(rec={'foo': {'foo': {'foo': 1}}})
+        RecursiveTypedDictModel(rec={'foo': {'foo': {'foo': 1}}})
     assert exc_info.value.errors(include_url=False) == [
         {
             'input': 1,
             'loc': ('rec', 'foo', 'foo', 'foo'),
             'msg': 'Input should be a valid dictionary',
             'type': 'dict_type',
         }
@@ -496,15 +551,14 @@
 
         from pydantic import BaseModel
 
         T = TypeVar('T')
 
         class RecursiveGenTypedDictModel(BaseModel, Generic[T]):
             rec: 'RecursiveGenTypedDict[T]'
-            model_config = dict(undefined_types_warning=False)
 
         class RecursiveGenTypedDict(TypedDict, Generic[T]):
             foo: Optional['RecursiveGenTypedDict[T]']
             ls: List[T]
 
     int_data: module.RecursiveGenTypedDict[int] = {'foo': {'foo': None, 'ls': [1]}, 'ls': [1]}
     assert module.RecursiveGenTypedDictModel[int](rec=int_data).rec == int_data
@@ -534,15 +588,14 @@
     # First ordering: typed dict first
     class RecursiveGenTypedDict(TypedDict, Generic[T]):
         foo: Optional['RecursiveGenTypedDict[T]']
         ls: List[T]
 
     class RecursiveGenTypedDictModel(BaseModel, Generic[T]):
         rec: 'RecursiveGenTypedDict[T]'
-        model_config = dict(undefined_types_warning=False)
 
     # Note: no model_rebuild() necessary here
     # RecursiveGenTypedDictModel.model_rebuild()
 
     int_data: RecursiveGenTypedDict[int] = {'foo': {'foo': None, 'ls': [1]}, 'ls': [1]}
     assert RecursiveGenTypedDictModel[int](rec=int_data).rec == int_data
 
@@ -567,15 +620,14 @@
 
 def test_recursive_generic_typeddict_in_function_2():
     T = TypeVar('T')
 
     # Second ordering: model first
     class RecursiveGenTypedDictModel(BaseModel, Generic[T]):
         rec: 'RecursiveGenTypedDict[T]'
-        model_config = dict(undefined_types_warning=False)
 
     class RecursiveGenTypedDict(TypedDict, Generic[T]):
         foo: Optional['RecursiveGenTypedDict[T]']
         ls: List[T]
 
     int_data: RecursiveGenTypedDict[int] = {'foo': {'foo': None, 'ls': [1]}, 'ls': [1]}
     assert RecursiveGenTypedDictModel[int](rec=int_data).rec == int_data
@@ -595,54 +647,27 @@
             'loc': ('rec', 'ls', 0),
             'msg': 'Input should be a valid integer, unable to parse string as an ' 'integer',
             'type': 'int_parsing',
         },
     ]
 
 
-def test_recursive_generic_typeddict_in_function_rebuild_error():
-    T = TypeVar('T')
-
-    class RecursiveGenTypedDictModel(BaseModel, Generic[T]):
-        rec: 'RecursiveGenTypedDict[T]'
-        model_config = dict(undefined_types_warning=False)
-
-    IntModel = RecursiveGenTypedDictModel[int]
-
-    class RecursiveGenTypedDict(TypedDict, Generic[T]):
-        foo: Optional['RecursiveGenTypedDict[T]']
-        ls: List[T]
-
-    int_data: RecursiveGenTypedDict[int] = {'foo': {'foo': None, 'ls': [1]}, 'ls': [1]}
-    with pytest.raises(
-        PydanticUserError,
-        match=re.escape(
-            '`RecursiveGenTypedDictModel[int]` is not fully defined; you should define `RecursiveGenTypedDict`,'
-            ' then call `RecursiveGenTypedDictModel[int].model_rebuild()` before the first'
-            ' `RecursiveGenTypedDictModel[int]` instance is created.'
-        ),
-    ):
-        IntModel(rec=int_data).rec
-
-
-def test_recursive_generic_typeddict_in_function_rebuild_pass():
+def test_recursive_generic_typeddict_in_function_3():
     T = TypeVar('T')
 
     class RecursiveGenTypedDictModel(BaseModel, Generic[T]):
         rec: 'RecursiveGenTypedDict[T]'
-        model_config = dict(undefined_types_warning=False)
 
     IntModel = RecursiveGenTypedDictModel[int]
 
     class RecursiveGenTypedDict(TypedDict, Generic[T]):
         foo: Optional['RecursiveGenTypedDict[T]']
         ls: List[T]
 
     int_data: RecursiveGenTypedDict[int] = {'foo': {'foo': None, 'ls': [1]}, 'ls': [1]}
-    IntModel.model_rebuild()
     assert IntModel(rec=int_data).rec == int_data
 
     str_data: RecursiveGenTypedDict[str] = {'foo': {'foo': None, 'ls': ['a']}, 'ls': ['a']}
     with pytest.raises(ValidationError) as exc_info:
         IntModel(rec=str_data)
     assert exc_info.value.errors(include_url=False) == [
         {
@@ -654,7 +679,153 @@
         {
             'input': 'a',
             'loc': ('rec', 'ls', 0),
             'msg': 'Input should be a valid integer, unable to parse string as an ' 'integer',
             'type': 'int_parsing',
         },
     ]
+
+
+@pytest.mark.xfail(reason='Needs https://github.com/pydantic/pydantic/pull/5944')
+def test_typeddict_alias_generator(TypedDict):
+    def alias_generator(name: str) -> str:
+        return 'alias_' + name
+
+    class MyDict(TypedDict):
+        foo: str
+
+    class Model(BaseModel):
+        d: MyDict
+
+    ta = TypeAdapter(MyDict, config=ConfigDict(alias_generator=alias_generator))
+    model = ta.validate_python({'alias_foo': 'bar'})
+
+    assert model['foo'] == 'bar'
+
+    with pytest.raises(ValidationError) as exc_info:
+        ta.validate_python({'foo': 'bar'})
+    assert exc_info.value.errors(include_url=False) == [
+        {'type': 'missing', 'loc': ('alias_foo',), 'msg': 'Field required', 'input': {'foo': 'bar'}},
+        {'input': 'bar', 'loc': ('foo',), 'msg': 'Extra inputs are not permitted', 'type': 'extra_forbidden'},
+    ]
+
+
+def test_typeddict_inheritence(TypedDict: Any) -> None:
+    class Parent(TypedDict):
+        x: int
+
+    class Child(Parent):
+        y: float
+
+    ta = TypeAdapter(Child)
+    assert ta.validate_python({'x': '1', 'y': '1.0'}) == {'x': 1, 'y': 1.0}
+
+
+def test_typeddict_field_validator(TypedDict: Any) -> None:
+    class Parent(TypedDict):
+        a: List[str]
+
+        @field_validator('a')
+        @classmethod
+        def parent_val_before(cls, v: List[str]):
+            v.append('parent before')
+            return v
+
+        @field_validator('a')
+        @classmethod
+        def val(cls, v: List[str]):
+            v.append('parent')
+            return v
+
+        @field_validator('a')
+        @classmethod
+        def parent_val_after(cls, v: List[str]):
+            v.append('parent after')
+            return v
+
+    class Child(Parent):
+        @field_validator('a')
+        @classmethod
+        def child_val_before(cls, v: List[str]):
+            v.append('child before')
+            return v
+
+        @field_validator('a')
+        @classmethod
+        def val(cls, v: List[str]):
+            v.append('child')
+            return v
+
+        @field_validator('a')
+        @classmethod
+        def child_val_after(cls, v: List[str]):
+            v.append('child after')
+            return v
+
+    parent_ta = TypeAdapter(Parent)
+    child_ta = TypeAdapter(Child)
+
+    assert parent_ta.validate_python({'a': []})['a'] == ['parent before', 'parent', 'parent after']
+    assert child_ta.validate_python({'a': []})['a'] == [
+        'parent before',
+        'child',
+        'parent after',
+        'child before',
+        'child after',
+    ]
+
+
+def test_typeddict_model_validator(TypedDict) -> None:
+    class Model(TypedDict):
+        x: int
+        y: float
+
+        @model_validator(mode='before')
+        @classmethod
+        def val_model_before(cls, value: Dict[str, Any]) -> Dict[str, Any]:
+            return dict(x=value['x'] + 1, y=value['y'] + 2)
+
+        @model_validator(mode='after')
+        def val_model_after(self) -> 'Model':
+            return Model(x=self['x'] * 2, y=self['y'] * 3)
+
+    ta = TypeAdapter(Model)
+
+    assert ta.validate_python({'x': 1, 'y': 2.5}) == {'x': 4, 'y': 13.5}
+
+
+def test_typeddict_field_serializer(TypedDict: Any) -> None:
+    class Parent(TypedDict):
+        a: List[str]
+
+        @field_serializer('a')
+        @classmethod
+        def ser(cls, v: List[str]):
+            v.append('parent')
+            return v
+
+    class Child(Parent):
+        @field_serializer('a')
+        @classmethod
+        def ser(cls, v: List[str]):
+            v.append('child')
+            return v
+
+    parent_ta = TypeAdapter(Parent)
+    child_ta = TypeAdapter(Child)
+
+    assert parent_ta.dump_python(Parent({'a': []}))['a'] == ['parent']
+    assert child_ta.dump_python(Child({'a': []}))['a'] == ['child']
+
+
+def test_typeddict_model_serializer(TypedDict) -> None:
+    class Model(TypedDict):
+        x: int
+        y: float
+
+        @model_serializer(mode='plain')
+        def ser_model(self) -> Dict[str, Any]:
+            return {'x': self['x'] * 2, 'y': self['y'] * 3}
+
+    ta = TypeAdapter(Model)
+
+    assert ta.dump_python(Model({'x': 1, 'y': 2.5})) == {'x': 2, 'y': 7.5}
```

### Comparing `pydantic-2.0a4/tests/test_typing.py` & `pydantic-2.0b1/tests/test_typing.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+import sys
 import typing
 from collections import namedtuple
 from typing import Callable, NamedTuple
 
 import pytest
 from typing_extensions import Literal, get_origin
 
 from pydantic import Field  # noqa: F401
-from pydantic._internal._typing_extra import is_namedtuple, is_none_type, origin_is_union
+from pydantic._internal._typing_extra import is_literal_type, is_namedtuple, is_none_type, origin_is_union
 
 try:
     from typing import TypedDict as typing_TypedDict
 except ImportError:
     typing_TypedDict = None
 
 try:
@@ -60,7 +61,22 @@
     try:
         union = union_gen()
     except TypeError:
         pytest.skip('not supported in this python version')
     else:
         origin = get_origin(union)
         assert origin_is_union(origin)
+
+
+def test_is_literal_with_typing_extension_literal():
+    from typing_extensions import Literal
+
+    assert is_literal_type(Literal) is False
+    assert is_literal_type(Literal['foo']) is True
+
+
+@pytest.mark.skipif(sys.version_info < (3, 8), reason='`typing.Literal` is available for python 3.8 and above.')
+def test_is_literal_with_typing_literal():
+    from typing import Literal
+
+    assert is_literal_type(Literal) is False
+    assert is_literal_type(Literal['foo']) is True
```

### Comparing `pydantic-2.0a4/tests/test_utils.py` & `pydantic-2.0b1/tests/test_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,53 +3,54 @@
 import pickle
 import sys
 from copy import copy, deepcopy
 from typing import Callable, Dict, Generic, List, NewType, Tuple, TypeVar, Union
 
 import pytest
 from dirty_equals import IsList
-from pydantic_core import PydanticCustomError
+from pydantic_core import PydanticCustomError, core_schema
 from typing_extensions import Annotated, Literal
 
 from pydantic import BaseModel
 from pydantic._internal import _repr
+from pydantic._internal._core_utils import _WalkCoreSchema
+from pydantic._internal._fields import Undefined
 from pydantic._internal._typing_extra import all_literal_values, get_origin, is_new_type
 from pydantic._internal._utils import (
     BUILTIN_COLLECTIONS,
     ClassAttribute,
     ValueItems,
     all_identical,
     deep_update,
     lenient_issubclass,
     smart_deepcopy,
     unique_list,
 )
 from pydantic._internal._validators import import_string
 from pydantic.alias_generators import to_camel, to_pascal, to_snake
 from pydantic.color import Color
-from pydantic.fields import Undefined
 
 try:
     import devtools
 except ImportError:
     devtools = None
 
 
 def test_import_module():
     assert import_string('os.path') == os.path
 
 
 def test_import_module_invalid():
-    with pytest.raises(PydanticCustomError, match='Invalid python path: "xx" doesn\'t look like a module path'):
+    with pytest.raises(PydanticCustomError, match="Invalid python path: No module named 'xx'"):
         import_string('xx')
 
 
 def test_import_no_attr():
-    with pytest.raises(PydanticCustomError, match='Module "os" does not define a "foobar" attribute'):
-        import_string('os.foobar')
+    with pytest.raises(PydanticCustomError, match="cannot import name 'foobar' from 'os'"):
+        import_string('os:foobar')
 
 
 def foobar(a, b, c=4):
     pass
 
 
 T = TypeVar('T')
@@ -173,14 +174,33 @@
 
     assert sub_vi.is_excluded(2)
     assert [v_ for i, v_ in enumerate(sub_v) if not sub_vi.is_excluded(i)] == ['b']
 
     assert sub_vi.is_included(2)
     assert [v_ for i, v_ in enumerate(sub_v) if sub_vi.is_included(i)] == ['a', 'c']
 
+    vi = ValueItems([], {'__all__': {}})
+    assert vi._items == {}
+
+    with pytest.raises(TypeError, match='Unexpected type of exclude value for index "a" <class \'NoneType\'>'):
+        ValueItems(['a', 'b'], {'a': None})
+
+    m = (
+        'Excluding fields from a sequence of sub-models or dicts must be performed index-wise: '
+        'expected integer keys or keyword "__all__"'
+    )
+    with pytest.raises(TypeError, match=m):
+        ValueItems(['a', 'b'], {'a': {}})
+
+    vi = ValueItems([1, 2, 3, 4], {'__all__': True})
+    assert repr(vi) == 'ValueItems({0: Ellipsis, 1: Ellipsis, 2: Ellipsis, 3: Ellipsis})'
+
+    vi = ValueItems([1, 2], {'__all__': {1, 2}})
+    assert repr(vi) == 'ValueItems({0: {1: Ellipsis, 2: Ellipsis}, 1: {1: Ellipsis, 2: Ellipsis}})'
+
 
 @pytest.mark.parametrize(
     'base,override,intersect,expected',
     [
         # Check in default (union) mode
         (..., ..., False, ...),
         (None, None, False, None),
@@ -516,7 +536,142 @@
         ('camel2', 'camel_2'),
         ('camel2_', 'camel_2_'),
         ('_camel2', '_camel_2'),
     ],
 )
 def test_camel2snake(value: str, result: str) -> None:
     assert to_snake(value) == result
+
+
+@pytest.mark.parametrize(
+    'params,expected_extra_schema',
+    (
+        pytest.param({}, {}, id='Positional tuple without extra_schema'),
+        pytest.param(
+            {'extra_schema': core_schema.float_schema()},
+            {'extra_schema': {'type': 'str'}},
+            id='Positional tuple with extra_schema',
+        ),
+    ),
+)
+def test_handle_tuple_positional_schema(params, expected_extra_schema):
+    schema = core_schema.tuple_positional_schema([core_schema.str_schema()], **params)
+
+    def walk(s, recurse):
+        # change extra_schema['type'] to 'str'
+        if s['type'] == 'float':
+            s['type'] = 'str'
+        return s
+
+    schema = _WalkCoreSchema().handle_tuple_positional_schema(schema, walk)
+    assert schema == {
+        **expected_extra_schema,
+        'items_schema': [{'type': 'str'}],
+        'type': 'tuple-positional',
+    }
+
+
+@pytest.mark.parametrize(
+    'params,expected_extra_schema',
+    (
+        pytest.param({}, {}, id='Model fields without extra_validator'),
+        pytest.param(
+            {'extra_validator': core_schema.float_schema()},
+            {'extra_validator': {'type': 'str'}},
+            id='Model fields with extra_validator',
+        ),
+    ),
+)
+def test_handle_model_fields_schema(params, expected_extra_schema):
+    schema = core_schema.model_fields_schema(
+        {
+            'foo': core_schema.model_field(core_schema.int_schema()),
+        },
+        **params,
+    )
+
+    def walk(s, recurse):
+        # change extra_schema['type'] to 'str'
+        if s['type'] == 'float':
+            s['type'] = 'str'
+        return s
+
+    schema = _WalkCoreSchema().handle_model_fields_schema(schema, walk)
+    assert schema == {
+        **expected_extra_schema,
+        'type': 'model-fields',
+        'fields': {'foo': {'type': 'model-field', 'schema': {'type': 'int'}}},
+    }
+
+
+@pytest.mark.parametrize(
+    'params,expected_extra_schema',
+    (
+        pytest.param({}, {}, id='Typeddict without extra_validator'),
+        pytest.param(
+            {'extra_validator': core_schema.float_schema()},
+            {'extra_validator': {'type': 'str'}},
+            id='Typeddict with extra_validator',
+        ),
+    ),
+)
+def test_handle_typed_dict_schema(params, expected_extra_schema):
+    schema = core_schema.typed_dict_schema(
+        {
+            'foo': core_schema.model_field(core_schema.int_schema()),
+        },
+        **params,
+    )
+
+    def walk(s, recurse):
+        # change extra_validator['type'] to 'str'
+        if s['type'] == 'float':
+            s['type'] = 'str'
+        return s
+
+    schema = _WalkCoreSchema().handle_typed_dict_schema(schema, walk)
+    assert schema == {
+        **expected_extra_schema,
+        'type': 'typed-dict',
+        'fields': {'foo': {'type': 'model-field', 'schema': {'type': 'int'}}},
+    }
+
+
+def test_handle_function_schema():
+    schema = core_schema.field_before_validator_function(function=lambda v, _info: v, schema=core_schema.float_schema())
+
+    def walk(s, recurse):
+        # change type to str
+        if s['type'] == 'float':
+            s['type'] = 'str'
+        return s
+
+    schema = _WalkCoreSchema().handle_function_schema(schema, walk)
+    assert schema['type'] == 'function-before'
+    assert schema['schema'] == {'type': 'str'}
+
+    def walk1(s, recurse):
+        # this is here to make sure this function is not called
+        assert False
+
+    schema = _WalkCoreSchema().handle_function_schema(core_schema.int_schema(), walk1)
+    assert schema['type'] == 'int'
+
+
+def test_handle_call_schema():
+    param_a = core_schema.arguments_parameter(name='a', schema=core_schema.str_schema(), mode='positional_only')
+    args_schema = core_schema.arguments_schema([param_a])
+
+    schema = core_schema.call_schema(
+        arguments=args_schema,
+        function=lambda a: int(a),
+        return_schema=core_schema.str_schema(),
+    )
+
+    def walk(s, recurse):
+        # change return schema
+        if 'return_schema' in schema:
+            schema['return_schema']['type'] = 'int'
+        return s
+
+    schema = _WalkCoreSchema().handle_call_schema(schema, walk)
+    assert schema['return_schema'] == {'type': 'int'}
```

### Comparing `pydantic-2.0a4/tests/test_validate_call.py` & `pydantic-2.0b1/tests/test_validate_call.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import pytest
 from pydantic_core import ArgsKwargs
 from typing_extensions import Annotated
 
 from pydantic import Field, TypeAdapter, ValidationError, validate_call
 
 skip_pre_38 = pytest.mark.skipif(sys.version_info < (3, 8), reason='testing >= 3.8 behaviour only')
+skip_pre_39 = pytest.mark.skipif(sys.version_info < (3, 9), reason='testing >= 3.9 behaviour only')
 
 
 def test_args():
     @validate_call
     def foo(a: int, b: int):
         return f'{a}, {b}'
 
@@ -89,14 +90,15 @@
 
     assert foo_bar.__doc__ == 'This is the foo_bar method.'
     assert foo_bar.__name__ == 'foo_bar'
     assert foo_bar.__module__ == 'tests.test_validate_call'
     assert foo_bar.__qualname__ == 'test_wrap.<locals>.foo_bar'
     assert isinstance(foo_bar.__pydantic_core_schema__, dict)
     assert callable(foo_bar.raw_function)
+    assert repr(foo_bar) == f'ValidateCallWrapper({repr(foo_bar.raw_function)})'
     assert repr(inspect.signature(foo_bar)) == '<Signature (a: int, b: int)>'
 
 
 def test_kwargs():
     @validate_call
     def foo(*, a: int, b: int):
         return a + b
@@ -178,15 +180,15 @@
     def foo2(a: int, b: Annotated[int, Field(default_factory=lambda: 99)], *args: int) -> int:
         """mypy reports Incompatible default for argument "b" if we don't supply ANY as default"""
         return a + b + sum(args)
 
     assert foo2(1) == 100
 
 
-@pytest.mark.skipif(sys.version_info < (3, 8), reason='testing >= 3.8 behaviour only')
+@skip_pre_38
 def test_positional_only(create_module):
     module = create_module(
         # language=Python
         """
 from pydantic import validate_call
 
 @validate_call
@@ -368,15 +370,15 @@
     # insert_assert(exc_info.value.errors(include_url=False))
     assert exc_info.value.errors(include_url=False) == [
         {'type': 'missing_argument', 'loc': ('a',), 'msg': 'Missing required argument', 'input': ArgsKwargs(())},
         {'type': 'missing_argument', 'loc': ('b',), 'msg': 'Missing required argument', 'input': ArgsKwargs(())},
     ]
 
 
-@pytest.mark.skipif(sys.version_info < (3, 9), reason='testing >= 3.9 behaviour only')
+@skip_pre_39
 def test_class_method():
     class X:
         @classmethod
         @validate_call
         def foo(cls, a: int, b: int):
             assert cls == X
             return f'{a}, {b}'
@@ -406,23 +408,70 @@
     assert TypeAdapter(foo).json_schema() == {
         'type': 'object',
         'properties': {'a': {'title': 'A', 'type': 'integer'}, 'b': {'default': None, 'title': 'B', 'type': 'integer'}},
         'required': ['a'],
         'additionalProperties': False,
     }
 
+    # TODO: Uncomment when support for 3.7 is dropped.
+    # @validate_call
+    # def foo(a: int, /, b: int):
+    #     return f'{a}, {b}'
+
+    # assert foo(1, 2) == '1, 2'
+    # assert TypeAdapter(foo).json_schema() == {
+    #     'maxItems': 2,
+    #     'minItems': 2,
+    #     'prefixItems': [{'title': 'A', 'type': 'integer'}, {'title': 'B', 'type': 'integer'}],
+    #     'type': 'array',
+    # }
+
+    # @validate_call
+    # def foo(a: int, /, *, b: int, c: int):
+    #     return f'{a}, {b}, {c}'
+
+    # assert foo(1, b=2, c=3) == '1, 2, 3'
+    # with pytest.raises(
+    #     PydanticInvalidForJsonSchema,
+    #     match=(
+    #       'Unable to generate JSON schema for arguments validator '
+    #       'with positional-only and keyword-only arguments'
+    #     ),
+    # ):
+    #     TypeAdapter(foo).json_schema()
 
-@pytest.mark.xfail(reason='waiting for https://github.com/pydantic/pydantic/issues/5395')
-def test_config_title():
-    @validate_call(config=dict(title='Testing'))
-    def foo(a: int, b: int = None):
-        return f'{a}, {b}'
+    @validate_call
+    def foo(*numbers: int) -> int:
+        return sum(numbers)
+
+    assert foo(1, 2, 3) == 6
+    assert TypeAdapter(foo).json_schema() == {'items': {'type': 'integer'}, 'prefixItems': [], 'type': 'array'}
 
-    js = TypeAdapter(foo).json_schema()
-    assert js['title'] == 'Testing'
+    @validate_call
+    def foo(**scores: int) -> str:
+        return ', '.join(f'{k}={v}' for k, v in sorted(scores.items()))
+
+    assert foo(a=1, b=2) == 'a=1, b=2'
+    assert TypeAdapter(foo).json_schema() == {
+        'additionalProperties': {'type': 'integer'},
+        'properties': {},
+        'type': 'object',
+    }
+
+    @validate_call
+    def foo(a: Annotated[int, Field(..., alias='A')]):
+        return a
+
+    assert foo(1) == 1
+    assert TypeAdapter(foo).json_schema() == {
+        'additionalProperties': False,
+        'properties': {'A': {'title': 'A', 'type': 'integer'}},
+        'required': ['A'],
+        'type': 'object',
+    }
 
 
 def test_alias_generator():
     @validate_call(config=dict(alias_generator=lambda x: x * 2))
     def foo(a: int, b: int):
         return f'{a}, {b}'
 
@@ -508,15 +557,15 @@
     def foo(dt: datetime = Field(default_factory=lambda: 946684800)):
         return dt
 
     assert foo() == datetime(2000, 1, 1)
     assert foo(0) == datetime(1970, 1, 1)
 
 
-@pytest.mark.skipif(sys.version_info < (3, 8), reason='testing >= 3.8 behaviour only')
+@skip_pre_38
 def test_validate_all_positional(create_module):
     module = create_module(
         # language=Python
         """
 from datetime import datetime
 
 from pydantic import Field, validate_call
@@ -547,15 +596,15 @@
 
     assert Foo(1, 2).v == 3
     assert Foo(1, '2').v == 3
     with pytest.raises(ValidationError, match="type=int_parsing, input_value='x', input_type=str"):
         Foo(1, 'x')
 
 
-@pytest.mark.skipif(sys.version_info < (3, 8), reason='testing >= 3.8 behaviour only')
+@skip_pre_38
 def test_positional_and_keyword_with_same_name(create_module):
     module = create_module(
         # language=Python
         """
 from pydantic import validate_call
 
 @validate_call
```

### Comparing `pydantic-2.0a4/tests/test_validator.py` & `pydantic-2.0b1/tests/test_type_adapter.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,16 @@
 import sys
 from typing import Any, Dict, ForwardRef, Generic, List, NamedTuple, Tuple, TypeVar, Union
 
 import pytest
 from pydantic_core import ValidationError
 from typing_extensions import TypeAlias, TypedDict
 
-from pydantic import BaseModel, TypeAdapter, ValidationInfo
+from pydantic import BaseModel, TypeAdapter, ValidationInfo, field_validator
 from pydantic.config import ConfigDict
-from pydantic.decorators import field_validator
 
 ItemType = TypeVar('ItemType')
 
 NestedList = List[List[ItemType]]
 
 
 class PydanticModel(BaseModel):
@@ -66,15 +65,15 @@
 def test_global_namespace_variables():
     v = TypeAdapter(OuterDict).validate_python
     res = v({'foo': [1, '2']})
     assert res == {'foo': [1, 2]}
 
 
 def test_local_namespace_variables():
-    IntList = List[int]
+    IntList = List[int]  # noqa: F841
     OuterDict = Dict[str, 'IntList']
 
     v = TypeAdapter(OuterDict).validate_python
 
     res = v({'foo': [1, '2']})
     assert res == {'foo': [1, 2]}
 
@@ -98,16 +97,19 @@
     assert res == [1, '2']
 
 
 def test_validate_python_strict() -> None:
     class Model(TypedDict):
         x: int
 
-    lax_validator = TypeAdapter(Model, config=ConfigDict(strict=False))
-    strict_validator = TypeAdapter(Model, config=ConfigDict(strict=True))
+    class ModelStrict(Model):
+        __pydantic_config__ = ConfigDict(strict=True)  # type: ignore
+
+    lax_validator = TypeAdapter(Model)
+    strict_validator = TypeAdapter(ModelStrict)
 
     assert lax_validator.validate_python({'x': '1'}, strict=None) == Model(x=1)
     assert lax_validator.validate_python({'x': '1'}, strict=False) == Model(x=1)
     with pytest.raises(ValidationError) as exc_info:
         lax_validator.validate_python({'x': '1'}, strict=True)
     assert exc_info.value.errors(include_url=False) == [
         {'type': 'int_type', 'loc': ('x',), 'msg': 'Input should be a valid integer', 'input': '1'}
@@ -122,20 +124,24 @@
     with pytest.raises(ValidationError) as exc_info:
         strict_validator.validate_python({'x': '1'}, strict=True)
     assert exc_info.value.errors(include_url=False) == [
         {'type': 'int_type', 'loc': ('x',), 'msg': 'Input should be a valid integer', 'input': '1'}
     ]
 
 
+@pytest.mark.xfail(reason='Need to fix this in https://github.com/pydantic/pydantic/pull/5944')
 def test_validate_json_strict() -> None:
     class Model(TypedDict):
         x: int
 
+    class ModelStrict(Model):
+        __pydantic_config__ = ConfigDict(strict=True)  # type: ignore
+
     lax_validator = TypeAdapter(Model, config=ConfigDict(strict=False))
-    strict_validator = TypeAdapter(Model, config=ConfigDict(strict=True))
+    strict_validator = TypeAdapter(ModelStrict)
 
     assert lax_validator.validate_json(json.dumps({'x': '1'}), strict=None) == Model(x=1)
     assert lax_validator.validate_json(json.dumps({'x': '1'}), strict=False) == Model(x=1)
     with pytest.raises(ValidationError) as exc_info:
         lax_validator.validate_json(json.dumps({'x': '1'}), strict=True)
     assert exc_info.value.errors(include_url=False) == [
         {'type': 'int_type', 'loc': ('x',), 'msg': 'Input should be a valid integer', 'input': '1'}
@@ -184,33 +190,7 @@
             return v
 
     validator = TypeAdapter(Model)
     validator.validate_json(json.dumps({'x': 1}))
     validator.validate_json(json.dumps({'x': 1}), context=None)
     validator.validate_json(json.dumps({'x': 1}), context={'foo': 'bar'})
     assert contexts == []
-
-
-def test_merge_config() -> None:
-    class Model(BaseModel):
-        x: int
-        y: str
-
-        model_config = ConfigDict(strict=True, title='FooModel')
-
-    adapted = TypeAdapter(Model, config=ConfigDict(strict=False, str_max_length=20))
-
-    # strict=False gets applied to the outer Model but not to the inner typeddict validator
-    # so we're allowed to validate a dict but `x` still must be an int
-    adapted.validate_python({'x': 1, 'y': '2'})
-    assert adapted.json_schema()['title'] == 'FooModel'
-    with pytest.raises(ValidationError) as exc_info:
-        adapted.validate_python({'x': 1, 'y': 'x' * 21})
-    assert exc_info.value.errors(include_url=False) == [
-        {
-            'type': 'string_too_long',
-            'loc': ('y',),
-            'msg': 'String should have at most 20 characters',
-            'input': 'xxxxxxxxxxxxxxxxxxxxx',
-            'ctx': {'max_length': 20},
-        }
-    ]
```

### Comparing `pydantic-2.0a4/tests/test_validators.py` & `pydantic-2.0b1/tests/test_validators.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,48 +17,50 @@
     ConfigDict,
     Field,
     FieldValidationInfo,
     ValidationError,
     ValidationInfo,
     ValidatorFunctionWrapHandler,
     errors,
+    field_validator,
+    model_validator,
+    root_validator,
     validator,
 )
-from pydantic.annotated_arguments import AfterValidator, BeforeValidator, PlainValidator, WrapValidator
-from pydantic.decorators import field_validator, root_validator
+from pydantic.functional_validators import AfterValidator, BeforeValidator, PlainValidator, WrapValidator
 
 V1_VALIDATOR_DEPRECATION_MATCH = r'Pydantic V1 style `@validator` validators are deprecated'
 
 
 def test_annotated_validator_after() -> None:
-    MyInt = Annotated[int, AfterValidator(lambda x: x if x != -1 else 0)]
+    MyInt = Annotated[int, AfterValidator(lambda x, _info: x if x != -1 else 0)]
 
     class Model(BaseModel):
         x: MyInt
 
     assert Model(x=0).x == 0
     assert Model(x=-1).x == 0
     assert Model(x=-2).x == -2
     assert Model(x=1).x == 1
     assert Model(x='-1').x == 0
 
 
 def test_annotated_validator_before() -> None:
-    FloatMaybeInf = Annotated[float, BeforeValidator(lambda x: x if x != 'zero' else 0.0)]
+    FloatMaybeInf = Annotated[float, BeforeValidator(lambda x, _info: x if x != 'zero' else 0.0)]
 
     class Model(BaseModel):
         x: FloatMaybeInf
 
     assert Model(x='zero').x == 0.0
     assert Model(x=1.0).x == 1.0
     assert Model(x='1.0').x == 1.0
 
 
 def test_annotated_validator_plain() -> None:
-    MyInt = Annotated[int, PlainValidator(lambda x: x if x != -1 else 0)]
+    MyInt = Annotated[int, PlainValidator(lambda x, _info: x if x != -1 else 0)]
 
     class Model(BaseModel):
         x: MyInt
 
     assert Model(x=0).x == 0
     assert Model(x=-1).x == 0
     assert Model(x=-2).x == -2
@@ -206,16 +208,16 @@
             'type': 'int_from_float',
             'loc': ('a',),
             'msg': 'Input should be a valid integer, got a number with a fractional part',
             'input': 4.5,
         }
     ]
 
-    # Doesn't raise ValidationError for number > (2 ^ 63) - 1 and limits them to (2 ^ 63) - 1
-    assert Model(a=(2**63) + 100).a == (2**63) - 1
+    # Doesn't raise ValidationError for number > (2 ^ 63) - 1
+    assert Model(a=(2**63) + 100).a == (2**63) + 100
 
 
 @pytest.mark.parametrize('value', [2.2250738585072011e308, float('nan'), float('inf')])
 def test_int_overflow_validation(value):
     class Model(BaseModel):
         a: int
 
@@ -267,19 +269,16 @@
         {
             'type': 'int_parsing',
             'loc': ('a', 0),
             'msg': 'Input should be a valid integer, unable to parse string as an integer',
             'input': 'a',
         }
     ]
-    with pytest.raises(ValidationError) as exc_info:
-        Model(a={'1'})
-    assert exc_info.value.errors(include_url=False) == [
-        {'type': 'list_type', 'loc': ('a',), 'msg': 'Input should be a valid list', 'input': {'1'}}
-    ]
+
+    assert Model(a={'1'}).a == deque([1])
     assert Model(a=[4, 5]).a == deque([4, 5])
     assert Model(a=(6,)).a == deque([6])
 
 
 def test_validate_whole():
     class Model(BaseModel):
         a: List[int]
@@ -498,28 +497,28 @@
 
     m = Model(a='this is foobar good')
     assert m.a == 'this is foobar good'
     m.check_a('x')
 
 
 def test_use_bare():
-    with pytest.raises(TypeError, match='validators should be used with fields'):
+    with pytest.raises(TypeError, match='`@validator` should be used with fields'):
 
         class Model(BaseModel):
             a: str
 
             with pytest.warns(DeprecationWarning, match=V1_VALIDATOR_DEPRECATION_MATCH):
 
                 @validator
                 def checker(cls, v):
                     return v
 
 
 def test_use_bare_field_validator():
-    with pytest.raises(TypeError, match='field_validators should be used with fields'):
+    with pytest.raises(TypeError, match='`@field_validator` should be used with fields'):
 
         class Model(BaseModel):
             a: str
 
             @field_validator
             def checker(cls, v):
                 return v
@@ -552,15 +551,15 @@
 
 
 def test_validator_bad_fields_throws_configerror():
     """
     Attempts to create a validator with fields set as a list of strings,
     rather than just multiple string args. Expects ConfigError to be raised.
     """
-    with pytest.raises(TypeError, match='validator fields should be passed as separate string args.'):
+    with pytest.raises(TypeError, match='`@validator` fields should be passed as separate string args.'):
 
         class Model(BaseModel):
             a: str
             b: str
 
             with pytest.warns(DeprecationWarning, match=V1_VALIDATOR_DEPRECATION_MATCH):
 
@@ -570,15 +569,15 @@
 
 
 def test_field_validator_bad_fields_throws_configerror():
     """
     Attempts to create a validator with fields set as a list of strings,
     rather than just multiple string args. Expects ConfigError to be raised.
     """
-    with pytest.raises(TypeError, match='field_validator fields should be passed as separate string args.'):
+    with pytest.raises(TypeError, match='`@field_validator` fields should be passed as separate string args.'):
 
         class Model(BaseModel):
             a: str
             b: str
 
             @field_validator(['a', 'b'])
             def check_fields(cls, v):
@@ -762,15 +761,15 @@
         },
         {'type': 'missing', 'loc': ('b',), 'msg': 'Field required', 'input': {'a': 'snap'}},
     ]
 
 
 def test_invalid_field():
     msg = (
-        r'Validators defined with incorrect fields:'
+        r'Decorators defined with incorrect fields:'
         r' tests.test_validators.test_invalid_field.<locals>.Model:\d+.check_b'
         r" \(use check_fields=False if you're inheriting from the model and intended this\)"
     )
     with pytest.raises(errors.PydanticUserError, match=msg):
 
         class Model(BaseModel):
             a: str
@@ -955,47 +954,49 @@
 def test_inheritance_replace_root_validator():
     """
     We promise that if you add a validator
     with the same _function_ name as an existing validator
     it replaces the existing validator and is run instead of it.
     """
 
-    class Parent(BaseModel):
-        a: List[str]
+    with pytest.warns(DeprecationWarning):
 
-        @root_validator(skip_on_failure=True)
-        def parent_val_before(cls, values: Dict[str, Any]):
-            values['a'].append('parent before')
-            return values
+        class Parent(BaseModel):
+            a: List[str]
 
-        @root_validator(skip_on_failure=True)
-        def val(cls, values: Dict[str, Any]):
-            values['a'].append('parent')
-            return values
+            @root_validator(skip_on_failure=True)
+            def parent_val_before(cls, values: Dict[str, Any]):
+                values['a'].append('parent before')
+                return values
 
-        @root_validator(skip_on_failure=True)
-        def parent_val_after(cls, values: Dict[str, Any]):
-            values['a'].append('parent after')
-            return values
+            @root_validator(skip_on_failure=True)
+            def val(cls, values: Dict[str, Any]):
+                values['a'].append('parent')
+                return values
 
-    class Child(Parent):
-        @root_validator(skip_on_failure=True)
-        def child_val_before(cls, values: Dict[str, Any]):
-            values['a'].append('child before')
-            return values
+            @root_validator(skip_on_failure=True)
+            def parent_val_after(cls, values: Dict[str, Any]):
+                values['a'].append('parent after')
+                return values
 
-        @root_validator(skip_on_failure=True)
-        def val(cls, values: Dict[str, Any]):
-            values['a'].append('child')
-            return values
+        class Child(Parent):
+            @root_validator(skip_on_failure=True)
+            def child_val_before(cls, values: Dict[str, Any]):
+                values['a'].append('child before')
+                return values
 
-        @root_validator(skip_on_failure=True)
-        def child_val_after(cls, values: Dict[str, Any]):
-            values['a'].append('child after')
-            return values
+            @root_validator(skip_on_failure=True)
+            def val(cls, values: Dict[str, Any]):
+                values['a'].append('child')
+                return values
+
+            @root_validator(skip_on_failure=True)
+            def child_val_after(cls, values: Dict[str, Any]):
+                values['a'].append('child after')
+                return values
 
     assert Parent(a=[]).a == ['parent before', 'parent', 'parent after']
     assert Child(a=[]).a == ['parent before', 'child', 'parent after', 'child before', 'child after']
 
 
 def test_validation_each_item():
     with pytest.warns(DeprecationWarning, match=V1_VALIDATOR_DEPRECATION_MATCH):
@@ -1286,27 +1287,29 @@
         c: str
 
         @field_validator('b')
         @classmethod
         def repeat_b(cls, v: Any):
             return v * 2
 
-        @root_validator(skip_on_failure=True)
-        def example_root_validator(cls, values: Dict[str, Any]) -> Dict[str, Any]:
-            root_val_values.append(values)
-            if 'snap' in values.get('b', ''):
-                raise ValueError('foobar')
-            return dict(values, b='changed')
+        with pytest.warns(DeprecationWarning):
 
-        @root_validator(skip_on_failure=True)
-        def example_root_validator2(cls, values: Dict[str, Any]) -> Dict[str, Any]:
-            root_val_values.append(values)
-            if 'snap' in values.get('c', ''):
-                raise ValueError('foobar2')
-            return dict(values, c='changed')
+            @root_validator(skip_on_failure=True)
+            def example_root_validator(cls, values: Dict[str, Any]) -> Dict[str, Any]:
+                root_val_values.append(values)
+                if 'snap' in values.get('b', ''):
+                    raise ValueError('foobar')
+                return dict(values, b='changed')
+
+            @root_validator(skip_on_failure=True)
+            def example_root_validator2(cls, values: Dict[str, Any]) -> Dict[str, Any]:
+                root_val_values.append(values)
+                if 'snap' in values.get('c', ''):
+                    raise ValueError('foobar2')
+                return dict(values, c='changed')
 
     assert Model(a='123', b='bar', c='baz').model_dump() == {'a': 123, 'b': 'changed', 'c': 'changed'}
 
     with pytest.raises(ValidationError) as exc_info:
         Model(b='snap dragon', c='snap dragon2')
     assert exc_info.value.errors(include_url=False) == [
         {
@@ -1340,31 +1343,34 @@
     """
     https://github.com/pydantic/pydantic/issues/5388
     """
 
     class Parent(BaseModel):
         x: int
         expected: Any
+        with pytest.warns(DeprecationWarning):
 
-        @root_validator(skip_on_failure=True)
-        @classmethod
-        def root_val(cls, values: Dict[str, Any]) -> Dict[str, Any]:
-            assert cls is values['expected']
-            return values
+            @root_validator(skip_on_failure=True)
+            @classmethod
+            def root_val(cls, values: Dict[str, Any]) -> Dict[str, Any]:
+                assert cls is values['expected']
+                return values
 
     class Child1(Parent):
         pass
 
     class Child2(Parent):
-        @root_validator(skip_on_failure=True)
-        @classmethod
-        def root_val(cls, values: Dict[str, Any]) -> Dict[str, Any]:
-            assert cls is Child2
-            values['x'] = values['x'] * 2
-            return values
+        with pytest.warns(DeprecationWarning):
+
+            @root_validator(skip_on_failure=True)
+            @classmethod
+            def root_val(cls, values: Dict[str, Any]) -> Dict[str, Any]:
+                assert cls is Child2
+                values['x'] = values['x'] * 2
+                return values
 
     class Child3(Parent):
         @classmethod
         def root_val(cls, values: Dict[str, Any]) -> Dict[str, Any]:
             assert cls is Child3
             values['x'] = values['x'] * 3
             return values
@@ -1383,20 +1389,22 @@
         b: str
 
         @field_validator('b')
         @classmethod
         def repeat_b(cls, v: Any):
             return v * 2
 
-        @root_validator(pre=True)
-        def root_validator(cls, values: Dict[str, Any]) -> Dict[str, Any]:
-            root_val_values.append(values)
-            if 'snap' in values.get('b', ''):
-                raise ValueError('foobar')
-            return {'a': 42, 'b': 'changed'}
+        with pytest.warns(DeprecationWarning):
+
+            @root_validator(pre=True)
+            def root_validator(cls, values: Dict[str, Any]) -> Dict[str, Any]:
+                root_val_values.append(values)
+                if 'snap' in values.get('b', ''):
+                    raise ValueError('foobar')
+                return {'a': 42, 'b': 'changed'}
 
     assert Model(a='123', b='bar').model_dump() == {'a': 42, 'b': 'changedchanged'}
 
     with pytest.raises(ValidationError) as exc_info:
         Model(b='snap dragon')
 
     assert root_val_values == [{'a': '123', 'b': 'bar'}, {'b': 'snap dragon'}]
@@ -1414,42 +1422,60 @@
 def test_root_validator_types():
     root_val_values = None
 
     class Model(BaseModel):
         a: int = 1
         b: str
 
-        @root_validator(skip_on_failure=True)
-        def root_validator(cls, values: Dict[str, Any]) -> Dict[str, Any]:
-            nonlocal root_val_values
-            root_val_values = cls, repr(values)
-            return values
+        with pytest.warns(DeprecationWarning):
+
+            @root_validator(skip_on_failure=True)
+            def root_validator(cls, values: Dict[str, Any]) -> Dict[str, Any]:
+                nonlocal root_val_values
+                root_val_values = cls, repr(values)
+                return values
 
         model_config = ConfigDict(extra='allow')
 
     assert Model(b='bar', c='wobble').model_dump() == {'a': 1, 'b': 'bar', 'c': 'wobble'}
 
     assert root_val_values == (Model, "{'a': 1, 'b': 'bar', 'c': 'wobble'}")
 
 
 def test_root_validator_returns_none_exception():
     class Model(BaseModel):
         a: int = 1
 
-        @root_validator(skip_on_failure=True)
-        def root_validator_repeated(cls, values):
-            return None
+        with pytest.warns(DeprecationWarning):
+
+            @root_validator(skip_on_failure=True)
+            def root_validator_repeated(cls, values):
+                return None
 
     with pytest.raises(
         TypeError,
         match=r"(:?__dict__ must be set to a dictionary, not a 'NoneType')|(:?setting dictionary to a non-dict)",
     ):
         Model()
 
 
+def test_model_validator_returns_ignore():
+    # This is weird, and I don't understand entirely why it's happening, but it kind of makes sense
+
+    class Model(BaseModel):
+        a: int = 1
+
+        @model_validator(mode='after')
+        def model_validator_return_none(cls, m):
+            return None
+
+    m = Model(a=2)
+    assert m.model_dump() == {'a': 2}
+
+
 def reusable_validator(num: int) -> int:
     return num * 2
 
 
 def test_reuse_global_validators():
     class Model(BaseModel):
         x: int
@@ -1480,15 +1506,17 @@
             root_val_values.append(values)
             if 'snap' in values.get('b', ''):
                 raise ValueError('foobar')
             return dict(values, b='changed')
 
         if root_validator_classmethod:
             example_root_validator = classmethod(example_root_validator)
-        example_root_validator = root_validator(skip_on_failure=True)(example_root_validator)
+
+        with pytest.warns(DeprecationWarning):
+            example_root_validator = root_validator(skip_on_failure=True)(example_root_validator)
 
     assert Model(a='123', b='bar').model_dump() == {'a': 123, 'b': 'changed'}
 
     with pytest.raises(ValidationError) as exc_info:
         Model(b='snap dragon')
     assert exc_info.value.errors(include_url=False) == [
         {
@@ -1531,17 +1559,15 @@
             return value
 
     m = Model(name='hello')
     m.name = 'goodbye'
     assert validator_calls == 2
 
 
-@pytest.mark.xfail(
-    sys.version_info[:2] == (3, 8), reason='https://github.com/python/cpython/issues/103592', strict=False
-)
+@pytest.mark.skipif(sys.version_info[:2] == (3, 8), reason='https://github.com/python/cpython/issues/103592')
 def test_literal_validator():
     class Model(BaseModel):
         a: Literal['foo']
 
     Model(a='foo')
 
     with pytest.raises(ValidationError) as exc_info:
@@ -1565,26 +1591,24 @@
     class Foo(BaseModel):
         bar: Bar
         barfiz: Literal[Bar.FIZ]
         fizfuz: Literal[Bar.FIZ, Bar.FUZ]
 
     my_foo = Foo.model_validate({'bar': 'fiz', 'barfiz': 'fiz', 'fizfuz': 'fiz'})
     assert my_foo.bar is Bar.FIZ
-    # TODO: this doesn't pass, `my_foo.barfiz == 'fiz'`
-    # Is this an intentional behavior change?
     assert my_foo.barfiz is Bar.FIZ
     assert my_foo.fizfuz is Bar.FIZ
 
     my_foo = Foo.model_validate({'bar': 'fiz', 'barfiz': 'fiz', 'fizfuz': 'fuz'})
     assert my_foo.bar is Bar.FIZ
     assert my_foo.barfiz is Bar.FIZ
     assert my_foo.fizfuz is Bar.FUZ
 
 
-@pytest.mark.xfail(
+@pytest.mark.skipif(
     sys.version_info[:2] == (3, 8), reason='https://github.com/python/cpython/issues/103592', strict=False
 )
 def test_nested_literal_validator():
     L1 = Literal['foo']
     L2 = Literal['bar']
 
     class Model(BaseModel):
@@ -1676,31 +1700,31 @@
 
 def test_overridden_root_validators():
     validate_stub = MagicMock()
 
     class A(BaseModel):
         x: str
 
-        @root_validator(pre=True)
+        @model_validator(mode='before')
         def pre_root(cls, values: Dict[str, Any]) -> Dict[str, Any]:
             validate_stub('A', 'pre')
             return values
 
-        @root_validator(pre=False, skip_on_failure=True)
+        @model_validator(mode='after')
         def post_root(cls, values: Dict[str, Any]) -> Dict[str, Any]:
             validate_stub('A', 'post')
             return values
 
     class B(A):
-        @root_validator(pre=True)
+        @model_validator(mode='before')
         def pre_root(cls, values: Dict[str, Any]) -> Dict[str, Any]:
             validate_stub('B', 'pre')
             return values
 
-        @root_validator(pre=False, skip_on_failure=True)
+        @model_validator(mode='after')
         def post_root(cls, values: Dict[str, Any]) -> Dict[str, Any]:
             validate_stub('B', 'post')
             return values
 
     A(x='pika')
     assert validate_stub.call_args_list == [[('A', 'pre'), {}], [('A', 'post'), {}]]
 
@@ -1712,17 +1736,46 @@
 
 def test_validating_assignment_pre_root_validator_fail():
     class Model(BaseModel):
         current_value: float = Field(..., alias='current')
         max_value: float
 
         model_config = ConfigDict(validate_assignment=True)
+        with pytest.warns(DeprecationWarning):
+
+            @root_validator(pre=True)
+            def values_are_not_string(cls, values: Dict[str, Any]) -> Dict[str, Any]:
+                if any(isinstance(x, str) for x in values.values()):
+                    raise ValueError('values cannot be a string')
+                return values
+
+    m = Model(current=100, max_value=200)
+    with pytest.raises(ValidationError) as exc_info:
+        m.current_value = '100'
+    assert exc_info.value.errors(include_url=False) == [
+        {
+            'type': 'value_error',
+            'loc': (),
+            'msg': 'Value error, values cannot be a string',
+            'input': {'current_value': '100', 'max_value': 200.0},
+            'ctx': {'error': 'values cannot be a string'},
+        }
+    ]
+
+
+def test_validating_assignment_model_validator_before_fail():
+    class Model(BaseModel):
+        current_value: float = Field(..., alias='current')
+        max_value: float
+
+        model_config = ConfigDict(validate_assignment=True)
 
-        @root_validator(pre=True)
+        @model_validator(mode='before')
         def values_are_not_string(cls, values: Dict[str, Any]) -> Dict[str, Any]:
+            assert isinstance(values, dict)
             if any(isinstance(x, str) for x in values.values()):
                 raise ValueError('values cannot be a string')
             return values
 
     m = Model(current=100, max_value=200)
     with pytest.raises(ValidationError) as exc_info:
         m.current_value = '100'
@@ -1743,51 +1796,54 @@
         {'skip_on_failure': False},
         {'skip_on_failure': False, 'pre': False},
         {'pre': False},
     ],
 )
 def test_root_validator_skip_on_failure_invalid(kwargs: Dict[str, Any]):
     with pytest.raises(TypeError, match='MUST specify `skip_on_failure=True`'):
+        with pytest.warns(DeprecationWarning, match='Pydantic V1 style `@root_validator` validators are deprecated.'):
 
-        class Model(BaseModel):
-            @root_validator(**kwargs)
-            def root_val(cls, values: Dict[str, Any]) -> Dict[str, Any]:
-                return values
+            class Model(BaseModel):
+                @root_validator(**kwargs)
+                def root_val(cls, values: Dict[str, Any]) -> Dict[str, Any]:
+                    return values
 
 
 @pytest.mark.parametrize(
     'kwargs',
     [
         {'skip_on_failure': True},
         {'skip_on_failure': True, 'pre': False},
         {'skip_on_failure': False, 'pre': True},
         {'pre': True},
     ],
 )
 def test_root_validator_skip_on_failure_valid(kwargs: Dict[str, Any]):
-    class Model(BaseModel):
-        @root_validator(**kwargs)
-        def root_val(cls, values: Dict[str, Any]) -> Dict[str, Any]:
-            return values
+    with pytest.warns(DeprecationWarning, match='Pydantic V1 style `@root_validator` validators are deprecated.'):
+
+        class Model(BaseModel):
+            @root_validator(**kwargs)
+            def root_val(cls, values: Dict[str, Any]) -> Dict[str, Any]:
+                return values
 
 
-def test_root_validator_many_values_change():
+def test_model_validator_many_values_change():
     """It should run root_validator on assignment and update ALL concerned fields"""
 
     class Rectangle(BaseModel):
         width: float
         height: float
         area: Optional[float] = None
 
         model_config = ConfigDict(validate_assignment=True)
 
-        @root_validator(skip_on_failure=True)
-        def set_area(cls, values: Dict[str, Any]) -> Dict[str, Any]:
-            values['area'] = values['width'] * values['height']
-            return values
+        @model_validator(mode='after')
+        def set_area(cls, m: 'Rectangle') -> 'Rectangle':
+            m.__dict__['area'] = m.width * m.height
+            return m
 
     r = Rectangle(width=1, height=1)
     assert r.area == 1
     r.height = 5
     assert r.area == 5
 
 
@@ -1874,21 +1930,22 @@
     assert Model.val1(1) == 2
     assert Model.val2(1) == 2
     assert Model.val3(1) == 2
 
 
 def test_root_validator_self():
     with pytest.raises(TypeError, match=r'`@root_validator` cannot be applied to instance methods'):
+        with pytest.warns(DeprecationWarning):
 
-        class Model(BaseModel):
-            a: int = 1
+            class Model(BaseModel):
+                a: int = 1
 
-            @root_validator(skip_on_failure=True)
-            def root_validator(self, values: Any) -> Any:
-                return values
+                @root_validator(skip_on_failure=True)
+                def root_validator(self, values: Any) -> Any:
+                    return values
 
 
 def test_validator_self():
     with pytest.warns(DeprecationWarning, match=V1_VALIDATOR_DEPRECATION_MATCH):
         with pytest.raises(TypeError, match=r'`@validator` cannot be applied to instance methods'):
 
             class Model(BaseModel):
@@ -2426,29 +2483,33 @@
                 v['x'] += 2
                 return v
 
         assert Model(x=1).model_dump() == {'x': 3}
 
 
 def test_root_validator_allow_reuse_inheritance():
-    class Parent(BaseModel):
-        x: int
+    with pytest.warns(DeprecationWarning):
 
-        @root_validator(skip_on_failure=True)
-        def root_val(cls, v: Dict[str, Any]) -> Dict[str, Any]:
-            v['x'] += 1
-            return v
+        class Parent(BaseModel):
+            x: int
 
-    class Child(Parent):
-        @root_validator(skip_on_failure=True)
-        def root_val(cls, v: Dict[str, Any]) -> Dict[str, Any]:
-            assert v == {'x': 1}
-            v = super().root_val(v)
-            assert v == {'x': 2}
-            return {'x': 4}
+            @root_validator(skip_on_failure=True)
+            def root_val(cls, v: Dict[str, Any]) -> Dict[str, Any]:
+                v['x'] += 1
+                return v
+
+    with pytest.warns(DeprecationWarning):
+
+        class Child(Parent):
+            @root_validator(skip_on_failure=True)
+            def root_val(cls, v: Dict[str, Any]) -> Dict[str, Any]:
+                assert v == {'x': 1}
+                v = super().root_val(v)
+                assert v == {'x': 2}
+                return {'x': 4}
 
     assert Parent(x=1).model_dump() == {'x': 2}
     assert Child(x=1).model_dump() == {'x': 4}
 
 
 def test_validator_with_underscore_name() -> None:
     """
@@ -2459,7 +2520,36 @@
         return name.lower()
 
     class Model(BaseModel):
         name: str
         _normalize_name = field_validator('name')(f)
 
     assert Model(name='Adrian').name == 'adrian'
+
+
+@pytest.mark.parametrize(
+    'mode,config,input_str',
+    (
+        ('before', {}, "type=value_error, input_value='123', input_type=str"),
+        ('before', {'hide_input_in_errors': False}, "type=value_error, input_value='123', input_type=str"),
+        ('before', {'hide_input_in_errors': True}, 'type=value_error'),
+        ('after', {}, "type=value_error, input_value='123', input_type=str"),
+        ('after', {'hide_input_in_errors': False}, "type=value_error, input_value='123', input_type=str"),
+        ('after', {'hide_input_in_errors': True}, 'type=value_error'),
+        ('plain', {}, "type=value_error, input_value='123', input_type=str"),
+        ('plain', {'hide_input_in_errors': False}, "type=value_error, input_value='123', input_type=str"),
+        ('plain', {'hide_input_in_errors': True}, 'type=value_error'),
+    ),
+)
+def test_validator_function_error_hide_input(mode, config, input_str):
+    class Model(BaseModel):
+        x: str
+
+        model_config = ConfigDict(**config)
+
+        @field_validator('x', mode=mode)
+        @classmethod
+        def check_a1(cls, v: str) -> str:
+            raise ValueError('foo')
+
+    with pytest.raises(ValidationError, match=re.escape(f'Value error, foo [{input_str}]')):
+        Model(x='123')
```

### Comparing `pydantic-2.0a4/tests/test_validators_dataclass.py` & `pydantic-2.0b1/tests/test_validators_dataclass.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from dataclasses import asdict, is_dataclass
 from typing import Any, List
 
 import pytest
 from dirty_equals import HasRepr
 
-from pydantic import ValidationError, root_validator
+from pydantic import ValidationError, field_validator, model_validator
 from pydantic.dataclasses import dataclass
-from pydantic.decorators import field_validator
 
 
 def test_simple():
     @dataclass
     class MyDataclass:
         a: str
 
@@ -146,33 +145,34 @@
         @classmethod
         def add_to_a(cls, v):
             return v + 5
 
     assert Child(a=0).a == 5
 
 
-def test_root_validator():
+def test_model_validator():
     root_val_values = []
 
     @dataclass
     class MyDataclass:
         a: int
         b: str
 
         @field_validator('b')
         @classmethod
         def repeat_b(cls, v):
             return v * 2
 
-        @root_validator(skip_on_failure=True)
-        def root_validator(cls, values):
-            root_val_values.append(values)
-            if 'snap' in values.get('b', ''):
+        @model_validator(mode='after')
+        def root_validator(cls, m):
+            root_val_values.append(asdict(m))
+            if 'snap' in m.b:
                 raise ValueError('foobar')
-            return dict(values, b='changed')
+            m.b = 'changed'
+            return m
 
     assert asdict(MyDataclass(a='123', b='bar')) == {'a': 123, 'b': 'changed'}
 
     with pytest.raises(ValidationError) as exc_info:
         MyDataclass(1, b='snap dragon')
     assert root_val_values == [{'a': 123, 'b': 'barbar'}, {'a': 1, 'b': 'snap dragonsnap dragon'}]
```

### Comparing `pydantic-2.0a4/tests/test_version.py` & `pydantic-2.0b1/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a4/tests/mypy/test_mypy.py` & `pydantic-2.0b1/tests/mypy/test_mypy.py`

 * *Files 4% similar despite different names*

```diff
@@ -207,14 +207,15 @@
         mypy_api.run(command)
 
     assert str(e.value) == 'Configuration value must be a boolean for key: init_forbid_extra'
 
 
 @pytest.mark.parametrize('module', sorted(executable_modules))
 @pytest.mark.filterwarnings('ignore:.*is deprecated.*:DeprecationWarning')
+@pytest.mark.filterwarnings('ignore:.*are deprecated.*:DeprecationWarning')
 def test_success_cases_run(module: str) -> None:
     """
     Ensure the "success" files can actually be executed
     """
     importlib.import_module(f'tests.mypy.modules.{module}')
```

### Comparing `pydantic-2.0a4/tests/mypy/configs/mypy-plugin-strict-no-any.ini` & `pydantic-2.0b1/tests/mypy/configs/mypy-plugin-strict-no-any.ini`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a4/tests/mypy/configs/pyproject-default.toml` & `pydantic-2.0b1/tests/mypy/configs/pyproject-default.toml`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a4/tests/mypy/configs/pyproject-plugin-bad-param.toml` & `pydantic-2.0b1/tests/mypy/configs/pyproject-plugin-bad-param.toml`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a4/tests/mypy/configs/pyproject-plugin-strict.toml` & `pydantic-2.0b1/tests/mypy/configs/pyproject-plugin-strict.toml`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a4/tests/mypy/configs/pyproject-plugin.toml` & `pydantic-2.0b1/tests/mypy/configs/pyproject-plugin.toml`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a4/tests/mypy/modules/computed_fields.py` & `pydantic-2.0b1/tests/mypy/modules/computed_fields.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a4/tests/mypy/modules/fail4.py` & `pydantic-2.0b1/tests/mypy/modules/fail4.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a4/tests/mypy/modules/plugin_default_factory.py` & `pydantic-2.0b1/tests/mypy/modules/plugin_default_factory.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a4/tests/mypy/modules/plugin_fail.py` & `pydantic-2.0b1/tests/mypy/modules/plugin_fail.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a4/tests/mypy/modules/plugin_fail_baseConfig.py` & `pydantic-2.0b1/tests/mypy/modules/plugin_fail_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a4/tests/mypy/modules/plugin_success.py` & `pydantic-2.0b1/tests/mypy/modules/plugin_success.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any, ClassVar, Generic, List, Optional, TypeVar, Union
 
-from pydantic import BaseModel, ConfigDict, Field, create_model, field_validator, validator
+from pydantic import BaseModel, ConfigDict, Field, create_model, field_validator, model_validator, validator
 from pydantic.dataclasses import dataclass
 
 
 # placeholder for removed line
 class Model(BaseModel):
     x: float
     y: str
@@ -21,15 +21,15 @@
 
 
 SelfReferencingModel.model_rebuild()
 
 model = Model(x=1, y='y')
 Model(x=1, y='y', z='z')
 model.x = 2
-model.model_validate(model.__dict__)  # TODO: Change this to .model_validate(model) when possible
+model.model_validate(model)
 
 self_referencing_model = SelfReferencingModel(submodel=SelfReferencingModel(submodel=None))
 
 
 class KwargsModel(BaseModel, from_attributes=True):
     x: float
     y: str
@@ -45,16 +45,14 @@
     z: int = 1
 
 
 InheritingModel.model_validate(model.__dict__)
 
 
 class ForwardReferencingModel(Model):
-    model_config = dict(undefined_types_warning=False)
-
     future: 'FutureModel'
 
 
 class FutureModel(Model):
     pass
 
 
@@ -287,8 +285,13 @@
 
 
 def foo() -> None:
     class MyModel(BaseModel):
         number: int
         custom_validator = get_my_custom_validator('number')  # type: ignore[pydantic-field]
 
+        @model_validator(mode='before')
+        @classmethod
+        def validate_values(cls, values: Any) -> Any:
+            return values
+
     MyModel(number=2)
```

### Comparing `pydantic-2.0a4/tests/mypy/modules/plugin_success_baseConfig.py` & `pydantic-2.0b1/tests/mypy/modules/plugin_success_baseConfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 
 SelfReferencingModel.model_rebuild()
 
 model = Model(x=1, y='y')
 Model(x=1, y='y', z='z')
 model.x = 2
-model.model_validate(model.__dict__)  # TODO: Change to .model_validate(model) when possible
+model.model_validate(model)
 
 self_referencing_model = SelfReferencingModel(submodel=SelfReferencingModel(submodel=None))
 
 
 class KwargsModel(BaseModel, from_attributes=True):
     x: float
     y: str
@@ -53,16 +53,14 @@
 
 InheritingModel.model_validate(model.__dict__)
 
 
 class ForwardReferencingModel(Model):
     future: 'FutureModel'
 
-    model_config = dict(undefined_types_warning=False)
-
 
 class FutureModel(Model):
     pass
 
 
 ForwardReferencingModel.model_rebuild()
 future_model = FutureModel(x=1, y='a')
```

### Comparing `pydantic-2.0a4/tests/mypy/modules/success.py` & `pydantic-2.0b1/tests/mypy/modules/success.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,34 +15,36 @@
     UUID1,
     AwareDatetime,
     BaseModel,
     ConfigDict,
     DirectoryPath,
     FilePath,
     FutureDate,
+    FutureDatetime,
     ImportString,
     Json,
     NaiveDatetime,
     NegativeFloat,
     NegativeInt,
     NonNegativeFloat,
     NonNegativeInt,
     NonPositiveFloat,
     NonPositiveInt,
     PastDate,
+    PastDatetime,
     PositiveFloat,
     PositiveInt,
     StrictBool,
     StrictBytes,
     StrictFloat,
     StrictInt,
     StrictStr,
     UrlConstraints,
+    create_model,
     field_validator,
-    parse_obj_as,
     root_validator,
     validate_call,
 )
 from pydantic.fields import Field, PrivateAttr
 from pydantic.networks import AnyUrl
 
 
@@ -193,15 +195,15 @@
 
 
 class MyPrivateAttr(BaseModel):
     _private_field: str = PrivateAttr()
 
 
 class PydanticTypes(BaseModel):
-    model_config = ConfigDict()  # TODO: add validate_all=True or equivalent if/when possible
+    model_config = ConfigDict(validate_default=True)
 
     # Boolean
     my_strict_bool: StrictBool = True
     # Integer
     my_positive_int: PositiveInt = 1
     my_negative_int: NegativeInt = -1
     my_non_positive_int: NonPositiveInt = -1
@@ -214,32 +216,33 @@
     my_non_negative_float: NonNegativeFloat = 1.1
     my_strict_float: StrictFloat = 1.1
     # Bytes
     my_strict_bytes: StrictBytes = b'pika'
     # String
     my_strict_str: StrictStr = 'pika'
     # ImportString
-    # TODO: Remove the parse_obj_as's below when we get `validate_all` (or similar) working
-    import_string_str: ImportString[Any] = parse_obj_as(ImportString[Any], 'datetime.date')  # type: ignore[misc]
+    import_string_str: ImportString[Any] = 'datetime.date'  # type: ignore[misc]
     import_string_callable: ImportString[Any] = date
     # UUID
     my_uuid1: UUID1 = UUID('a8098c1a-f86e-11da-bd1a-00112444be1e')
-    my_uuid1_str: UUID1 = parse_obj_as(UUID1, 'a8098c1a-f86e-11da-bd1a-00112444be1e')
+    my_uuid1_str: UUID1 = 'a8098c1a-f86e-11da-bd1a-00112444be1e'
     # Path
     my_file_path: FilePath = Path(__file__)
-    my_file_path_str: FilePath = parse_obj_as(Path, __file__)
+    my_file_path_str: FilePath = __file__
     my_dir_path: DirectoryPath = Path('.')
-    my_dir_path_str: DirectoryPath = parse_obj_as(DirectoryPath, '.')
+    my_dir_path_str: DirectoryPath = '.'
     # Json
-    my_json: Json[Dict[str, str]] = parse_obj_as(Json[Dict[str, str]], '{"hello": "world"}')
-    my_json_list: Json[List[str]] = parse_obj_as(Json[List[str]], '["hello", "world"]')
+    my_json: Json[Dict[str, str]] = '{"hello": "world"}'
+    my_json_list: Json[List[str]] = '["hello", "world"]'
     # Date
     my_past_date: PastDate = date.today() - timedelta(1)
     my_future_date: FutureDate = date.today() + timedelta(1)
     # Datetime
+    my_past_datetime: PastDatetime = datetime.now() - timedelta(1)
+    my_future_datetime: FutureDatetime = datetime.now() + timedelta(1)
     my_aware_datetime: AwareDatetime = datetime.now(tz=timezone.utc)
     my_naive_datetime: NaiveDatetime = datetime.now()
 
 
 validated = PydanticTypes()
 validated.import_string_str(2021, 1, 1)
 validated.import_string_callable(2021, 1, 1)
@@ -280,9 +283,8 @@
     def __init__(self, *args: str):
         self.path = os.path.join(*args)
 
     def __fspath__(self) -> str:
         return f'a/custom/{self.path}'
 
 
-# TODO:
-# DynamicModel = create_model('DynamicModel')
+DynamicModel = create_model('DynamicModel')
```

### Comparing `pydantic-2.0a4/tests/mypy/outputs/latest/fail4.txt` & `pydantic-2.0b1/tests/mypy/outputs/latest/fail4.txt`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a4/tests/mypy/outputs/latest/plugin-fail-baseConfig.txt` & `pydantic-2.0b1/tests/mypy/outputs/latest/plugin-fail-baseConfig.txt`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a4/tests/mypy/outputs/latest/plugin-fail-strict-baseConfig.txt` & `pydantic-2.0b1/tests/mypy/outputs/latest/plugin-fail-strict-baseConfig.txt`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a4/tests/mypy/outputs/latest/plugin-fail-strict.txt` & `pydantic-2.0b1/tests/mypy/outputs/latest/plugin-fail-strict.txt`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a4/tests/mypy/outputs/latest/plugin-fail.txt` & `pydantic-2.0b1/tests/mypy/outputs/latest/plugin-fail.txt`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a4/tests/pyright/pyright_example.py` & `pydantic-2.0b1/tests/pyright/pyright_example.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a4/.gitignore` & `pydantic-2.0b1/.gitignore`

 * *Files 22% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 .pytest_cache/
 /.ruff_cache/
 
 # Benchmark and test files
 /benchmarks/*.json
 /htmlcov/
 /codecov.sh
+/coverage.lcov
 .coverage
 test.py
 
 # Documentation files
 /docs/changelog.md
 /site/
 /site.zip
```

### Comparing `pydantic-2.0a4/LICENSE` & `pydantic-2.0b1/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2017 - 2022 Samuel Colvin and other contributors
+Copyright (c) 2017 to present Pydantic Services Inc. and individual contributors.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pydantic-2.0a4/pyproject.toml` & `pydantic-2.0b1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 [build-system]
 requires = ['hatchling', 'hatch-fancy-pypi-readme>=22.5.0']
 build-backend = 'hatchling.build'
 
 [tool.hatch.version]
 path = 'pydantic/version.py'
 
+[tool.hatch.metadata]
+allow-direct-references = true
+
 [tool.hatch.build.targets.sdist]
 # limit which files are included in the sdist (.tar.gz) asset,
 # see https://github.com/pydantic/pydantic/pull/4542
 include = [
     '/README.md',
     '/HISTORY.md',
     '/Makefile',
@@ -52,22 +55,20 @@
     'Framework :: Hypothesis',
     'Framework :: Pydantic',
     'Topic :: Software Development :: Libraries :: Python Modules',
     'Topic :: Internet',
 ]
 requires-python = '>=3.7'
 dependencies = [
-    'typing-extensions>=4.5.0',
+    'typing-extensions>=4.6.1',
     'annotated-types>=0.4.0',
-    "pydantic-core==0.30.0",
+    "pydantic-core==0.38.0",
 ]
 dynamic = ['version', 'readme']
 
-entry-points.hypothesis = {_ = 'pydantic._hypothesis_plugin'}
-
 [project.optional-dependencies]
 email = ['email-validator>=2.0.0']
 
 [tool.pdm.dev-dependencies]
 docs = [
     "autoflake",
     "mkdocs",
@@ -140,49 +141,54 @@
 
 [tool.pytest.ini_options]
 testpaths = 'tests'
 xfail_strict = true
 filterwarnings = [
     'error',
     'ignore:path is deprecated.*:DeprecationWarning:',
+    # Work around https://github.com/pytest-dev/pytest/issues/10977 for Python 3.12
+    'ignore:(ast\.Str|ast\.NameConstant|ast\.Num|Attribute s) is deprecated and will be removed.*:DeprecationWarning:',
 ]
 
 # configuring https://github.com/pydantic/hooky
 [tool.hooky]
-reviewers = ['samuelcolvin', 'adriangb', 'dmontagu', 'hramezani']
+reviewers = ['samuelcolvin', 'adriangb', 'dmontagu', 'hramezani', 'lig', 'Kludex']
 require_change_file = false
 
 [tool.ruff]
 line-length = 120
 extend-select = ['Q', 'RUF100', 'C90', 'UP', 'I']
 flake8-quotes = {inline-quotes = 'single', multiline-quotes = 'double'}
 mccabe = { max-complexity = 14 }
 isort = { known-first-party = ['pydantic', 'tests'] }
 target-version = "py37"
+exclude=['pydantic/v1']
 
 [tool.ruff.per-file-ignores]
 'pydantic/__init__.py' = ['F405', 'F403']
 'tests/test_forward_ref.py' = ['F821']
 
 [tool.coverage.run]
 source = ['pydantic']
-omit = ['pydantic/deprecated/*']
+omit = ['pydantic/deprecated/*', 'pydantic/v1/*']
 branch = true
 context = '${CONTEXT}'
 
 [tool.coverage.report]
 precision = 2
 exclude_lines = [
     'pragma: no cover',
     'raise NotImplementedError',
     'if TYPE_CHECKING:',
     'if typing.TYPE_CHECKING:',
     '@overload',
     '@typing.overload',
     '\(Protocol\):$',
+    'typing.assert_never',
+    'assert_never',
 ]
 
 [tool.coverage.paths]
 source = [
     'pydantic/',
     '/Users/runner/work/pydantic/pydantic/pydantic/',
     'D:\a\pydantic\pydantic\pydantic',
@@ -192,13 +198,13 @@
 color = true
 line-length = 120
 target-version = ['py310']
 skip-string-normalization = true
 
 [tool.pyright]
 include = ['pydantic']
-exclude = ['pydantic/_hypothesis_plugin.py', 'pydantic/mypy.py']
+exclude = ['pydantic/_hypothesis_plugin.py', 'pydantic/mypy.py', 'pydantic/v1']
 
 [tool.codespell]
-skip = '.git,env*'
+skip = '.git,env*,pydantic/v1/*'
 # `ser` - abbreviation for "ser"ialisation
 ignore-words-list = 'gir,ser'
```

### Comparing `pydantic-2.0a4/PKG-INFO` & `pydantic-2.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic
-Version: 2.0a4
+Version: 2.0b1
 Summary: Data validation using Python type hints
 Project-URL: Homepage, https://github.com/pydantic/pydantic
 Project-URL: Documentation, https://docs.pydantic.dev
 Project-URL: Funding, https://github.com/sponsors/samuelcolvin
 Project-URL: Source, https://github.com/pydantic/pydantic
 Project-URL: Changelog, https://docs.pydantic.dev/changelog
 Author-email: Samuel Colvin <s@muelcolvin.com>, Eric Jolibois <em.jolibois@gmail.com>, Hasan Ramezani <hasan.r67@gmail.com>, Adrian Garcia Badaracco <1755071+adriangb@users.noreply.github.com>, Terrence Dorsey <terry@pydantic.dev>, David Montague <david@pydantic.dev>
@@ -31,16 +31,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Requires-Dist: annotated-types>=0.4.0
-Requires-Dist: pydantic-core==0.30.0
-Requires-Dist: typing-extensions>=4.5.0
+Requires-Dist: pydantic-core==0.38.0
+Requires-Dist: typing-extensions>=4.6.1
 Provides-Extra: email
 Requires-Dist: email-validator>=2.0.0; extra == 'email'
 Description-Content-Type: text/markdown
 
 # Pydantic
 
 [![CI](https://github.com/pydantic/pydantic/workflows/CI/badge.svg?event=push)](https://github.com/pydantic/pydantic/actions?query=event%3Apush+branch%3Amain+workflow%3ACI)
@@ -108,14 +108,20 @@
 
 ## Reporting a Security Vulnerability
 
 See our [security policy](https://github.com/pydantic/pydantic/security/policy).
 
 ## Changelog
 
+## v2.0b1 (2023-06-01)
+
+First beta pre-release of Pydantic V2
+
+See the full changelog [here](https://github.com/pydantic/pydantic/releases/tag/v2.0b1)
+
 ## v2.0a4 (2023-05-05)
 
 Fourth pre-release of Pydantic V2
 
 See the full changelog [here](https://github.com/pydantic/pydantic/releases/tag/v2.0a4)
 
 ## v2.0a3 (2023-04-20)
```

