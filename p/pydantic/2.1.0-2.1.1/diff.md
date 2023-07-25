# Comparing `tmp/pydantic-2.1.0.tar.gz` & `tmp/pydantic-2.1.1.tar.gz`

## Comparing `pydantic-2.1.0.tar` & `pydantic-2.1.1.tar`

### file list

```diff
@@ -1,270 +1,270 @@
--rw-r--r--   0        0        0   133183 2020-02-02 00:00:00.000000 pydantic-2.1.0/HISTORY.md
--rw-r--r--   0        0        0     4604 2020-02-02 00:00:00.000000 pydantic-2.1.0/Makefile
--rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 pydantic-2.1.0/README.md
--rw-r--r--   0        0        0     5156 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/__init__.py
--rw-r--r--   0        0        0    11630 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/_migration.py
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/alias_generators.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/class_validators.py
--rw-r--r--   0        0        0    21521 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/color.py
--rw-r--r--   0        0        0     7774 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/config.py
--rw-r--r--   0        0        0    11157 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/dataclasses.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/datetime_parse.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/decorator.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/env_settings.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/error_wrappers.py
--rw-r--r--   0        0        0     4557 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/errors.py
--rw-r--r--   0        0        0    40151 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/fields.py
--rw-r--r--   0        0        0    10830 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/functional_serializers.py
--rw-r--r--   0        0        0    19874 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/functional_validators.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/generics.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/json.py
--rw-r--r--   0        0        0    98393 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/json_schema.py
--rw-r--r--   0        0        0    60009 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/main.py
--rw-r--r--   0        0        0    50600 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/mypy.py
--rw-r--r--   0        0        0    13684 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/networks.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/parse.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/py.typed
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/root_model.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/schema.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/tools.py
--rw-r--r--   0        0        0    15656 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/type_adapter.py
--rw-r--r--   0        0        0    46636 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/types.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/typing.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/utils.py
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/validate_call.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/validators.py
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/version.py
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/warnings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/_internal/__init__.py
--rw-r--r--   0        0        0     4090 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/_internal/_annotated_handlers.py
--rw-r--r--   0        0        0     9830 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/_internal/_config.py
--rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/_internal/_core_metadata.py
--rw-r--r--   0        0        0    23137 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/_internal/_core_utils.py
--rw-r--r--   0        0        0    10840 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/_internal/_dataclasses.py
--rw-r--r--   0        0        0    29738 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/_internal/_decorators.py
--rw-r--r--   0        0        0     6273 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/_internal/_decorators_v1.py
--rw-r--r--   0        0        0    24909 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/_internal/_discriminated_union.py
--rw-r--r--   0        0        0    11141 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/_internal/_fields.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/_internal/_forward_ref.py
--rw-r--r--   0        0        0    89618 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/_internal/_generate_schema.py
--rw-r--r--   0        0        0    22191 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/_internal/_generics.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/_internal/_internal_dataclass.py
--rw-r--r--   0        0        0     9552 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/_internal/_known_annotated_metadata.py
--rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/_internal/_mock_validator.py
--rw-r--r--   0        0        0    26086 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/_internal/_model_construction.py
--rw-r--r--   0        0        0     4210 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/_internal/_repr.py
--rw-r--r--   0        0        0     4740 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/_internal/_schema_generation_shared.py
--rw-r--r--   0        0        0    36148 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/_internal/_std_types_schema.py
--rw-r--r--   0        0        0    16416 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/_internal/_typing_extra.py
--rw-r--r--   0        0        0    12170 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/_internal/_utils.py
--rw-r--r--   0        0        0     5087 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/_internal/_validate_call.py
--rw-r--r--   0        0        0     9936 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/_internal/_validators.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/deprecated/__init__.py
--rw-r--r--   0        0        0     9864 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/deprecated/class_validators.py
--rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/deprecated/config.py
--rw-r--r--   0        0        0     7644 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/deprecated/copy_internals.py
--rw-r--r--   0        0        0    10919 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/deprecated/decorator.py
--rw-r--r--   0        0        0     4465 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/deprecated/json.py
--rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/deprecated/parse.py
--rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/deprecated/tools.py
--rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/v1/__init__.py
--rw-r--r--   0        0        0    14844 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/v1/_hypothesis_plugin.py
--rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/v1/annotated_types.py
--rw-r--r--   0        0        0    14595 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/v1/class_validators.py
--rw-r--r--   0        0        0    16811 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/v1/color.py
--rw-r--r--   0        0        0     6477 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/v1/config.py
--rw-r--r--   0        0        0    17515 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/v1/dataclasses.py
--rw-r--r--   0        0        0     7714 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/v1/datetime_parse.py
--rw-r--r--   0        0        0    10263 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/v1/decorator.py
--rw-r--r--   0        0        0    14039 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/v1/env_settings.py
--rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/v1/error_wrappers.py
--rw-r--r--   0        0        0    17693 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/v1/errors.py
--rw-r--r--   0        0        0    50488 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/v1/fields.py
--rw-r--r--   0        0        0    17805 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/v1/generics.py
--rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/v1/json.py
--rw-r--r--   0        0        0    44378 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/v1/main.py
--rw-r--r--   0        0        0    38641 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/v1/mypy.py
--rw-r--r--   0        0        0    21826 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/v1/networks.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/v1/parse.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/v1/py.typed
--rw-r--r--   0        0        0    47615 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/v1/schema.py
--rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/v1/tools.py
--rw-r--r--   0        0        0    35380 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/v1/types.py
--rw-r--r--   0        0        0    18996 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/v1/typing.py
--rw-r--r--   0        0        0    25809 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/v1/utils.py
--rw-r--r--   0        0        0    21887 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/v1/validators.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 pydantic-2.1.0/pydantic/v1/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/__init__.py
--rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/conftest.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_abc.py
--rw-r--r--   0        0        0    16305 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_aliases.py
--rw-r--r--   0        0        0     9171 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_annotated.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_assert_in_validators.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_callable.py
--rw-r--r--   0        0        0     7751 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_color.py
--rw-r--r--   0        0        0    19678 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_computed_fields.py
--rw-r--r--   0        0        0    23612 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_config.py
--rw-r--r--   0        0        0    13733 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_construction.py
--rw-r--r--   0        0        0    16730 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_create_model.py
--rw-r--r--   0        0        0    68428 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_dataclasses.py
--rw-r--r--   0        0        0    21601 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_datetime.py
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_decorators.py
--rw-r--r--   0        0        0    23108 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_deprecated.py
--rw-r--r--   0        0        0    12237 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_deprecated_validate_arguments.py
--rw-r--r--   0        0        0    48329 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_discriminated_union.py
--rw-r--r--   0        0        0     9781 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_docs.py
--rw-r--r--   0        0        0    79607 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_edge_cases.py
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_errors.py
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_exports.py
--rwxr-xr-x   0        0        0      313 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_fastapi.sh
--rw-r--r--   0        0        0     4980 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_fastapi_json_schema.py
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_fields.py
--rw-r--r--   0        0        0    28393 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_forward_ref.py
--rw-r--r--   0        0        0    75341 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_generics.py
--rw-r--r--   0        0        0    10775 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_internal.py
--rw-r--r--   0        0        0    16346 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_json.py
--rw-r--r--   0        0        0   164674 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_json_schema.py
--rw-r--r--   0        0        0    81311 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_main.py
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_migration.py
--rw-r--r--   0        0        0     5953 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_model_signature.py
--rw-r--r--   0        0        0     4388 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_model_validator.py
--rw-r--r--   0        0        0    29799 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_networks.py
--rw-r--r--   0        0        0    16217 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_networks_ipaddress.py
--rw-r--r--   0        0        0     7462 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_parse.py
--rw-r--r--   0        0        0     8039 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_prepare_annotations.py
--rw-r--r--   0        0        0     9302 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_private_attributes.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_pydantic_extra_types.sh
--rwxr-xr-x   0        0        0      131 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_pydantic_settings.sh
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_rich_repr.py
--rw-r--r--   0        0        0    16611 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_root_model.py
--rw-r--r--   0        0        0    30800 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_serialize.py
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_strict.py
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_structural_pattern_matching.py
--rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_tools.py
--rw-r--r--   0        0        0     8991 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_type_adapter.py
--rw-r--r--   0        0        0    10941 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_type_alias_type.py
--rw-r--r--   0        0        0   179278 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_types.py
--rw-r--r--   0        0        0     5753 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_types_namedtuple.py
--rw-r--r--   0        0        0     5159 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_types_payment_card_number.py
--rw-r--r--   0        0        0    26544 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_types_typeddict.py
--rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_typing.py
--rw-r--r--   0        0        0    21626 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_utils.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_v1.py
--rw-r--r--   0        0        0    21649 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_validate_call.py
--rw-r--r--   0        0        0    74764 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_validators.py
--rwxr-xr-x   0        0        0     4737 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_validators_dataclass.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_version.py
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/test_warnings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/benchmarks/__init__.py
--rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/benchmarks/generate_north_star_data.py
--rw-r--r--   0        0        0     4888 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/benchmarks/test_north_star.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/__init__.py
--rw-r--r--   0        0        0    11030 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/test_mypy.py
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/configs/mypy-default.ini
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/configs/mypy-plugin-strict-no-any.ini
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/configs/mypy-plugin-strict.ini
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/configs/mypy-plugin-very-strict.ini
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/configs/mypy-plugin.ini
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/configs/pyproject-default.toml
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/configs/pyproject-plugin-bad-param.toml
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/configs/pyproject-plugin-strict.toml
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/configs/pyproject-plugin.toml
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/modules/computed_fields.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/modules/custom_constructor.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/modules/dataclass_no_any.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/modules/fail1.py
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/modules/fail2.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/modules/fail3.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/modules/fail4.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/modules/fail_defaults.py
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/modules/generics.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/modules/metaclass_args.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/modules/plugin_default_factory.py
--rw-r--r--   0        0        0     5687 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/modules/plugin_fail.py
--rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/modules/plugin_fail_baseConfig.py
--rw-r--r--   0        0        0     5755 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/modules/plugin_success.py
--rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/modules/plugin_success_baseConfig.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/modules/pydantic_settings.py
--rw-r--r--   0        0        0     7663 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/modules/success.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.0.1/mypy-default_ini/fail1.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.0.1/mypy-default_ini/fail2.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.0.1/mypy-default_ini/fail3.py
--rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.0.1/mypy-default_ini/fail4.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.0.1/mypy-default_ini/metaclass_args.py
--rw-r--r--   0        0        0     6202 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.0.1/mypy-default_ini/plugin_success.py
--rw-r--r--   0        0        0     4625 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.0.1/mypy-default_ini/plugin_success_baseConfig.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.0.1/mypy-default_ini/pydantic_settings.py
--rw-r--r--   0        0        0     8303 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.0.1/mypy-default_ini/success.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.0.1/mypy-plugin-strict-no-any_ini/dataclass_no_any.py
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/fail_defaults.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_default_factory.py
--rw-r--r--   0        0        0    10688 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_fail.py
--rw-r--r--   0        0        0    10463 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_fail_baseConfig.py
--rw-r--r--   0        0        0     5903 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_success.py
--rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_success_baseConfig.py
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.0.1/mypy-plugin-very-strict_ini/metaclass_args.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.0.1/mypy-plugin_ini/custom_constructor.py
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.0.1/mypy-plugin_ini/generics.py
--rw-r--r--   0        0        0     9305 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.0.1/mypy-plugin_ini/plugin_fail.py
--rw-r--r--   0        0        0     9080 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.0.1/mypy-plugin_ini/plugin_fail_baseConfig.py
--rw-r--r--   0        0        0     5755 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.0.1/mypy-plugin_ini/plugin_success.py
--rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.0.1/mypy-plugin_ini/plugin_success_baseConfig.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.0.1/mypy-plugin_ini/pydantic_settings.py
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.0.1/pyproject-default_toml/computed_fields.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.0.1/pyproject-default_toml/fail1.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.0.1/pyproject-default_toml/fail2.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.0.1/pyproject-default_toml/fail3.py
--rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.0.1/pyproject-default_toml/fail4.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.0.1/pyproject-default_toml/pydantic_settings.py
--rw-r--r--   0        0        0     8303 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.0.1/pyproject-default_toml/success.py
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/fail_defaults.py
--rw-r--r--   0        0        0    10688 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/plugin_fail.py
--rw-r--r--   0        0        0    10463 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/plugin_fail_baseConfig.py
--rw-r--r--   0        0        0     5903 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/plugin_success.py
--rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/plugin_success_baseConfig.py
--rw-r--r--   0        0        0     9305 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/plugin_fail.py
--rw-r--r--   0        0        0     9080 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/plugin_fail_baseConfig.py
--rw-r--r--   0        0        0     5755 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/plugin_success.py
--rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/plugin_success_baseConfig.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/pydantic_settings.py
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.1.1/mypy-default_ini/fail1.py
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.1.1/mypy-default_ini/fail2.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.1.1/mypy-default_ini/metaclass_args.py
--rw-r--r--   0        0        0     6263 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.1.1/mypy-default_ini/plugin_success.py
--rw-r--r--   0        0        0     4844 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.1.1/mypy-default_ini/plugin_success_baseConfig.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.1.1/mypy-default_ini/pydantic_settings.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.1.1/mypy-plugin_ini/pydantic_settings.py
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.1.1/pyproject-default_toml/fail1.py
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.1.1/pyproject-default_toml/fail2.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.1.1/pyproject-default_toml/pydantic_settings.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.1.1/pyproject-plugin_toml/pydantic_settings.py
--rw-r--r--   0        0        0     6109 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.2.0/mypy-default_ini/plugin_success.py
--rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.2.0/mypy-default_ini/plugin_success_baseConfig.py
--rw-r--r--   0        0        0    10842 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.2.0/mypy-plugin-strict_ini/plugin_fail.py
--rw-r--r--   0        0        0    10617 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.2.0/mypy-plugin-strict_ini/plugin_fail_baseConfig.py
--rw-r--r--   0        0        0     9459 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.2.0/mypy-plugin_ini/plugin_fail.py
--rw-r--r--   0        0        0     9234 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.2.0/mypy-plugin_ini/plugin_fail_baseConfig.py
--rw-r--r--   0        0        0    10842 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.2.0/pyproject-plugin-strict_toml/plugin_fail.py
--rw-r--r--   0        0        0    10617 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.2.0/pyproject-plugin-strict_toml/plugin_fail_baseConfig.py
--rw-r--r--   0        0        0     9459 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.2.0/pyproject-plugin_toml/plugin_fail.py
--rw-r--r--   0        0        0     9234 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.2.0/pyproject-plugin_toml/plugin_fail_baseConfig.py
--rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.4.1/mypy-default_ini/fail4.py
--rw-r--r--   0        0        0     6126 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.4.1/mypy-default_ini/plugin_success.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.4.1/mypy-plugin-strict_ini/plugin_default_factory.py
--rw-r--r--   0        0        0    10839 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.4.1/mypy-plugin-strict_ini/plugin_fail.py
--rw-r--r--   0        0        0    10614 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.4.1/mypy-plugin-strict_ini/plugin_fail_baseConfig.py
--rw-r--r--   0        0        0     9473 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.4.1/mypy-plugin_ini/plugin_fail.py
--rw-r--r--   0        0        0     9248 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.4.1/mypy-plugin_ini/plugin_fail_baseConfig.py
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.4.1/mypy-plugin_ini/pydantic_settings.py
--rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.4.1/pyproject-default_toml/fail4.py
--rw-r--r--   0        0        0    10839 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.4.1/pyproject-plugin-strict_toml/plugin_fail.py
--rw-r--r--   0        0        0    10614 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.4.1/pyproject-plugin-strict_toml/plugin_fail_baseConfig.py
--rw-r--r--   0        0        0     9473 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.4.1/pyproject-plugin_toml/plugin_fail.py
--rw-r--r--   0        0        0     9248 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.4.1/pyproject-plugin_toml/plugin_fail_baseConfig.py
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/mypy/outputs/1.4.1/pyproject-plugin_toml/pydantic_settings.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/pyright/pyproject.toml
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 pydantic-2.1.0/tests/pyright/pyright_example.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 pydantic-2.1.0/.gitignore
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 pydantic-2.1.0/LICENSE
--rw-r--r--   0        0        0     7082 2020-02-02 00:00:00.000000 pydantic-2.1.0/pyproject.toml
--rw-r--r--   0        0        0   136242 2020-02-02 00:00:00.000000 pydantic-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0   133398 2020-02-02 00:00:00.000000 pydantic-2.1.1/HISTORY.md
+-rw-r--r--   0        0        0     4604 2020-02-02 00:00:00.000000 pydantic-2.1.1/Makefile
+-rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 pydantic-2.1.1/README.md
+-rw-r--r--   0        0        0     5156 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/__init__.py
+-rw-r--r--   0        0        0    11630 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/_migration.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/alias_generators.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/class_validators.py
+-rw-r--r--   0        0        0    21521 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/color.py
+-rw-r--r--   0        0        0     7774 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/config.py
+-rw-r--r--   0        0        0    11157 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/dataclasses.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/datetime_parse.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/decorator.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/env_settings.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/error_wrappers.py
+-rw-r--r--   0        0        0     4557 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/errors.py
+-rw-r--r--   0        0        0    40497 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/fields.py
+-rw-r--r--   0        0        0    10830 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/functional_serializers.py
+-rw-r--r--   0        0        0    19874 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/functional_validators.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/generics.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/json.py
+-rw-r--r--   0        0        0    98393 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/json_schema.py
+-rw-r--r--   0        0        0    60009 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/main.py
+-rw-r--r--   0        0        0    50600 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/mypy.py
+-rw-r--r--   0        0        0    13684 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/networks.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/parse.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/py.typed
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/root_model.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/schema.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/tools.py
+-rw-r--r--   0        0        0    15656 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/type_adapter.py
+-rw-r--r--   0        0        0    46636 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/types.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/typing.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/utils.py
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/validate_call.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/validators.py
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/version.py
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/warnings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/_internal/__init__.py
+-rw-r--r--   0        0        0     4090 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/_internal/_annotated_handlers.py
+-rw-r--r--   0        0        0     9830 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/_internal/_config.py
+-rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/_internal/_core_metadata.py
+-rw-r--r--   0        0        0    23137 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/_internal/_core_utils.py
+-rw-r--r--   0        0        0    10840 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/_internal/_dataclasses.py
+-rw-r--r--   0        0        0    29738 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/_internal/_decorators.py
+-rw-r--r--   0        0        0     6273 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/_internal/_decorators_v1.py
+-rw-r--r--   0        0        0    24909 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/_internal/_discriminated_union.py
+-rw-r--r--   0        0        0    11141 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/_internal/_fields.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/_internal/_forward_ref.py
+-rw-r--r--   0        0        0    89618 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/_internal/_generate_schema.py
+-rw-r--r--   0        0        0    22191 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/_internal/_generics.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/_internal/_internal_dataclass.py
+-rw-r--r--   0        0        0     9552 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/_internal/_known_annotated_metadata.py
+-rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/_internal/_mock_validator.py
+-rw-r--r--   0        0        0    26086 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/_internal/_model_construction.py
+-rw-r--r--   0        0        0     4210 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/_internal/_repr.py
+-rw-r--r--   0        0        0     4740 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/_internal/_schema_generation_shared.py
+-rw-r--r--   0        0        0    36148 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/_internal/_std_types_schema.py
+-rw-r--r--   0        0        0    16416 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/_internal/_typing_extra.py
+-rw-r--r--   0        0        0    12170 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/_internal/_utils.py
+-rw-r--r--   0        0        0     5087 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/_internal/_validate_call.py
+-rw-r--r--   0        0        0     9936 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/_internal/_validators.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/deprecated/__init__.py
+-rw-r--r--   0        0        0     9864 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/deprecated/class_validators.py
+-rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/deprecated/config.py
+-rw-r--r--   0        0        0     7644 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/deprecated/copy_internals.py
+-rw-r--r--   0        0        0    10919 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/deprecated/decorator.py
+-rw-r--r--   0        0        0     4465 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/deprecated/json.py
+-rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/deprecated/parse.py
+-rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/deprecated/tools.py
+-rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/v1/__init__.py
+-rw-r--r--   0        0        0    14844 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/v1/_hypothesis_plugin.py
+-rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/v1/annotated_types.py
+-rw-r--r--   0        0        0    14595 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/v1/class_validators.py
+-rw-r--r--   0        0        0    16811 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/v1/color.py
+-rw-r--r--   0        0        0     6477 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/v1/config.py
+-rw-r--r--   0        0        0    17515 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/v1/dataclasses.py
+-rw-r--r--   0        0        0     7714 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/v1/datetime_parse.py
+-rw-r--r--   0        0        0    10263 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/v1/decorator.py
+-rw-r--r--   0        0        0    14039 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/v1/env_settings.py
+-rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/v1/error_wrappers.py
+-rw-r--r--   0        0        0    17693 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/v1/errors.py
+-rw-r--r--   0        0        0    50488 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/v1/fields.py
+-rw-r--r--   0        0        0    17805 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/v1/generics.py
+-rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/v1/json.py
+-rw-r--r--   0        0        0    44378 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/v1/main.py
+-rw-r--r--   0        0        0    38641 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/v1/mypy.py
+-rw-r--r--   0        0        0    21826 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/v1/networks.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/v1/parse.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/v1/py.typed
+-rw-r--r--   0        0        0    47615 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/v1/schema.py
+-rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/v1/tools.py
+-rw-r--r--   0        0        0    35380 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/v1/types.py
+-rw-r--r--   0        0        0    18996 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/v1/typing.py
+-rw-r--r--   0        0        0    25809 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/v1/utils.py
+-rw-r--r--   0        0        0    21887 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/v1/validators.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 pydantic-2.1.1/pydantic/v1/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/conftest.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_abc.py
+-rw-r--r--   0        0        0    16305 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_aliases.py
+-rw-r--r--   0        0        0     9171 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_annotated.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_assert_in_validators.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_callable.py
+-rw-r--r--   0        0        0     7751 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_color.py
+-rw-r--r--   0        0        0    19678 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_computed_fields.py
+-rw-r--r--   0        0        0    23612 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_config.py
+-rw-r--r--   0        0        0    13733 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_construction.py
+-rw-r--r--   0        0        0    16730 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_create_model.py
+-rw-r--r--   0        0        0    68428 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_dataclasses.py
+-rw-r--r--   0        0        0    21601 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_datetime.py
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_decorators.py
+-rw-r--r--   0        0        0    23108 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_deprecated.py
+-rw-r--r--   0        0        0    12237 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_deprecated_validate_arguments.py
+-rw-r--r--   0        0        0    48329 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_discriminated_union.py
+-rw-r--r--   0        0        0     9781 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_docs.py
+-rw-r--r--   0        0        0    79607 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_edge_cases.py
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_errors.py
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_exports.py
+-rwxr-xr-x   0        0        0      313 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_fastapi.sh
+-rw-r--r--   0        0        0     4980 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_fastapi_json_schema.py
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_fields.py
+-rw-r--r--   0        0        0    28393 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_forward_ref.py
+-rw-r--r--   0        0        0    75341 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_generics.py
+-rw-r--r--   0        0        0    10775 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_internal.py
+-rw-r--r--   0        0        0    16346 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_json.py
+-rw-r--r--   0        0        0   164674 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_json_schema.py
+-rw-r--r--   0        0        0    81311 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_main.py
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_migration.py
+-rw-r--r--   0        0        0     5953 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_model_signature.py
+-rw-r--r--   0        0        0     4388 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_model_validator.py
+-rw-r--r--   0        0        0    29799 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_networks.py
+-rw-r--r--   0        0        0    16217 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_networks_ipaddress.py
+-rw-r--r--   0        0        0     7462 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_parse.py
+-rw-r--r--   0        0        0     8039 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_prepare_annotations.py
+-rw-r--r--   0        0        0     9302 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_private_attributes.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_pydantic_extra_types.sh
+-rwxr-xr-x   0        0        0      131 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_pydantic_settings.sh
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_rich_repr.py
+-rw-r--r--   0        0        0    16611 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_root_model.py
+-rw-r--r--   0        0        0    30800 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_serialize.py
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_strict.py
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_structural_pattern_matching.py
+-rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_tools.py
+-rw-r--r--   0        0        0     8991 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_type_adapter.py
+-rw-r--r--   0        0        0    10941 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_type_alias_type.py
+-rw-r--r--   0        0        0   179278 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_types.py
+-rw-r--r--   0        0        0     5753 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_types_namedtuple.py
+-rw-r--r--   0        0        0     5159 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_types_payment_card_number.py
+-rw-r--r--   0        0        0    26544 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_types_typeddict.py
+-rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_typing.py
+-rw-r--r--   0        0        0    21626 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_utils.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_v1.py
+-rw-r--r--   0        0        0    21649 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_validate_call.py
+-rw-r--r--   0        0        0    74764 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_validators.py
+-rwxr-xr-x   0        0        0     4737 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_validators_dataclass.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_version.py
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/test_warnings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/benchmarks/__init__.py
+-rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/benchmarks/generate_north_star_data.py
+-rw-r--r--   0        0        0     4888 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/benchmarks/test_north_star.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/__init__.py
+-rw-r--r--   0        0        0    11030 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/test_mypy.py
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/configs/mypy-default.ini
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/configs/mypy-plugin-strict-no-any.ini
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/configs/mypy-plugin-strict.ini
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/configs/mypy-plugin-very-strict.ini
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/configs/mypy-plugin.ini
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/configs/pyproject-default.toml
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/configs/pyproject-plugin-bad-param.toml
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/configs/pyproject-plugin-strict.toml
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/configs/pyproject-plugin.toml
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/modules/computed_fields.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/modules/custom_constructor.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/modules/dataclass_no_any.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/modules/fail1.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/modules/fail2.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/modules/fail3.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/modules/fail4.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/modules/fail_defaults.py
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/modules/generics.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/modules/metaclass_args.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/modules/plugin_default_factory.py
+-rw-r--r--   0        0        0     5687 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/modules/plugin_fail.py
+-rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/modules/plugin_fail_baseConfig.py
+-rw-r--r--   0        0        0     5755 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/modules/plugin_success.py
+-rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/modules/plugin_success_baseConfig.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/modules/pydantic_settings.py
+-rw-r--r--   0        0        0     7663 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/modules/success.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.0.1/mypy-default_ini/fail1.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.0.1/mypy-default_ini/fail2.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.0.1/mypy-default_ini/fail3.py
+-rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.0.1/mypy-default_ini/fail4.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.0.1/mypy-default_ini/metaclass_args.py
+-rw-r--r--   0        0        0     6202 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.0.1/mypy-default_ini/plugin_success.py
+-rw-r--r--   0        0        0     4625 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.0.1/mypy-default_ini/plugin_success_baseConfig.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.0.1/mypy-default_ini/pydantic_settings.py
+-rw-r--r--   0        0        0     8303 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.0.1/mypy-default_ini/success.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.0.1/mypy-plugin-strict-no-any_ini/dataclass_no_any.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/fail_defaults.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_default_factory.py
+-rw-r--r--   0        0        0    10688 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_fail.py
+-rw-r--r--   0        0        0    10463 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_fail_baseConfig.py
+-rw-r--r--   0        0        0     5903 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_success.py
+-rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_success_baseConfig.py
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.0.1/mypy-plugin-very-strict_ini/metaclass_args.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.0.1/mypy-plugin_ini/custom_constructor.py
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.0.1/mypy-plugin_ini/generics.py
+-rw-r--r--   0        0        0     9305 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.0.1/mypy-plugin_ini/plugin_fail.py
+-rw-r--r--   0        0        0     9080 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.0.1/mypy-plugin_ini/plugin_fail_baseConfig.py
+-rw-r--r--   0        0        0     5755 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.0.1/mypy-plugin_ini/plugin_success.py
+-rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.0.1/mypy-plugin_ini/plugin_success_baseConfig.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.0.1/mypy-plugin_ini/pydantic_settings.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.0.1/pyproject-default_toml/computed_fields.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.0.1/pyproject-default_toml/fail1.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.0.1/pyproject-default_toml/fail2.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.0.1/pyproject-default_toml/fail3.py
+-rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.0.1/pyproject-default_toml/fail4.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.0.1/pyproject-default_toml/pydantic_settings.py
+-rw-r--r--   0        0        0     8303 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.0.1/pyproject-default_toml/success.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/fail_defaults.py
+-rw-r--r--   0        0        0    10688 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/plugin_fail.py
+-rw-r--r--   0        0        0    10463 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/plugin_fail_baseConfig.py
+-rw-r--r--   0        0        0     5903 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/plugin_success.py
+-rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/plugin_success_baseConfig.py
+-rw-r--r--   0        0        0     9305 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/plugin_fail.py
+-rw-r--r--   0        0        0     9080 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/plugin_fail_baseConfig.py
+-rw-r--r--   0        0        0     5755 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/plugin_success.py
+-rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/plugin_success_baseConfig.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/pydantic_settings.py
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.1.1/mypy-default_ini/fail1.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.1.1/mypy-default_ini/fail2.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.1.1/mypy-default_ini/metaclass_args.py
+-rw-r--r--   0        0        0     6263 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.1.1/mypy-default_ini/plugin_success.py
+-rw-r--r--   0        0        0     4844 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.1.1/mypy-default_ini/plugin_success_baseConfig.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.1.1/mypy-default_ini/pydantic_settings.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.1.1/mypy-plugin_ini/pydantic_settings.py
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.1.1/pyproject-default_toml/fail1.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.1.1/pyproject-default_toml/fail2.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.1.1/pyproject-default_toml/pydantic_settings.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.1.1/pyproject-plugin_toml/pydantic_settings.py
+-rw-r--r--   0        0        0     6109 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.2.0/mypy-default_ini/plugin_success.py
+-rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.2.0/mypy-default_ini/plugin_success_baseConfig.py
+-rw-r--r--   0        0        0    10842 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.2.0/mypy-plugin-strict_ini/plugin_fail.py
+-rw-r--r--   0        0        0    10617 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.2.0/mypy-plugin-strict_ini/plugin_fail_baseConfig.py
+-rw-r--r--   0        0        0     9459 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.2.0/mypy-plugin_ini/plugin_fail.py
+-rw-r--r--   0        0        0     9234 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.2.0/mypy-plugin_ini/plugin_fail_baseConfig.py
+-rw-r--r--   0        0        0    10842 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.2.0/pyproject-plugin-strict_toml/plugin_fail.py
+-rw-r--r--   0        0        0    10617 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.2.0/pyproject-plugin-strict_toml/plugin_fail_baseConfig.py
+-rw-r--r--   0        0        0     9459 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.2.0/pyproject-plugin_toml/plugin_fail.py
+-rw-r--r--   0        0        0     9234 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.2.0/pyproject-plugin_toml/plugin_fail_baseConfig.py
+-rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.4.1/mypy-default_ini/fail4.py
+-rw-r--r--   0        0        0     6126 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.4.1/mypy-default_ini/plugin_success.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.4.1/mypy-plugin-strict_ini/plugin_default_factory.py
+-rw-r--r--   0        0        0    10839 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.4.1/mypy-plugin-strict_ini/plugin_fail.py
+-rw-r--r--   0        0        0    10614 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.4.1/mypy-plugin-strict_ini/plugin_fail_baseConfig.py
+-rw-r--r--   0        0        0     9473 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.4.1/mypy-plugin_ini/plugin_fail.py
+-rw-r--r--   0        0        0     9248 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.4.1/mypy-plugin_ini/plugin_fail_baseConfig.py
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.4.1/mypy-plugin_ini/pydantic_settings.py
+-rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.4.1/pyproject-default_toml/fail4.py
+-rw-r--r--   0        0        0    10839 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.4.1/pyproject-plugin-strict_toml/plugin_fail.py
+-rw-r--r--   0        0        0    10614 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.4.1/pyproject-plugin-strict_toml/plugin_fail_baseConfig.py
+-rw-r--r--   0        0        0     9473 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.4.1/pyproject-plugin_toml/plugin_fail.py
+-rw-r--r--   0        0        0     9248 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.4.1/pyproject-plugin_toml/plugin_fail_baseConfig.py
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/mypy/outputs/1.4.1/pyproject-plugin_toml/pydantic_settings.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/pyright/pyproject.toml
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 pydantic-2.1.1/tests/pyright/pyright_example.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 pydantic-2.1.1/.gitignore
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 pydantic-2.1.1/LICENSE
+-rw-r--r--   0        0        0     7082 2020-02-02 00:00:00.000000 pydantic-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0   136488 2020-02-02 00:00:00.000000 pydantic-2.1.1/PKG-INFO
```

### Comparing `pydantic-2.1.0/HISTORY.md` & `pydantic-2.1.1/HISTORY.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## v2.1.1 (2023-07-25)
+
+[GitHub release](https://github.com/pydantic/pydantic/releases/tag/v2.1.1)
+
+* Skip FieldInfo merging when unnecessary by @dmontagu in [#6862](https://github.com/pydantic/pydantic/pull/6862)
+
 ## v2.1.0 (2023-07-25)
 
 [GitHub release](https://github.com/pydantic/pydantic/releases/tag/v2.1.0)
 
 * Add `StringConstraints` for use as Annotated metadata by @adriangb in [#6605](https://github.com/pydantic/pydantic/pull/6605)
 * Try to fix intermittently failing CI by @adriangb in [#6683](https://github.com/pydantic/pydantic/pull/6683)
 * Remove redundant example of optional vs default. by @ehiggs-deliverect in [#6676](https://github.com/pydantic/pydantic/pull/6676)
```

### Comparing `pydantic-2.1.0/Makefile` & `pydantic-2.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/README.md` & `pydantic-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/__init__.py` & `pydantic-2.1.1/pydantic/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/_migration.py` & `pydantic-2.1.1/pydantic/_migration.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/alias_generators.py` & `pydantic-2.1.1/pydantic/alias_generators.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/color.py` & `pydantic-2.1.1/pydantic/color.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/config.py` & `pydantic-2.1.1/pydantic/config.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/dataclasses.py` & `pydantic-2.1.1/pydantic/dataclasses.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/errors.py` & `pydantic-2.1.1/pydantic/errors.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/fields.py` & `pydantic-2.1.1/pydantic/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -376,14 +376,22 @@
             FieldInfo: A merged FieldInfo instance.
         """
         flattened_field_infos: list[FieldInfo] = []
         for field_info in field_infos:
             flattened_field_infos.extend(x for x in field_info.metadata if isinstance(x, FieldInfo))
             flattened_field_infos.append(field_info)
         field_infos = tuple(flattened_field_infos)
+        if len(field_infos) == 1:
+            # No merging necessary, but we still need to make a copy and apply the overrides
+            field_info = copy(field_infos[0])
+            field_info._attributes_set.update(overrides)
+            for k, v in overrides.items():
+                setattr(field_info, k, v)
+            return field_info
+
         new_kwargs: dict[str, Any] = {}
         metadata = {}
         for field_info in field_infos:
             new_kwargs.update(field_info._attributes_set)
             for x in field_info.metadata:
                 if not isinstance(x, FieldInfo):
                     metadata[type(x)] = x
```

### Comparing `pydantic-2.1.0/pydantic/functional_serializers.py` & `pydantic-2.1.1/pydantic/functional_serializers.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/functional_validators.py` & `pydantic-2.1.1/pydantic/functional_validators.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/json_schema.py` & `pydantic-2.1.1/pydantic/json_schema.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/main.py` & `pydantic-2.1.1/pydantic/main.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/mypy.py` & `pydantic-2.1.1/pydantic/mypy.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/networks.py` & `pydantic-2.1.1/pydantic/networks.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/root_model.py` & `pydantic-2.1.1/pydantic/root_model.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/type_adapter.py` & `pydantic-2.1.1/pydantic/type_adapter.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/types.py` & `pydantic-2.1.1/pydantic/types.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/validate_call.py` & `pydantic-2.1.1/pydantic/validate_call.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/version.py` & `pydantic-2.1.1/pydantic/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """The `version` module holds the version information for Pydantic."""
 from typing import Tuple
 
 __all__ = 'VERSION', 'version_info'
 
-VERSION = '2.1.0'
+VERSION = '2.1.1'
 """The version of Pydantic."""
 
 
 def version_info() -> str:
     """Return complete version information for Pydantic and its dependencies."""
     import platform
     import sys
```

### Comparing `pydantic-2.1.0/pydantic/warnings.py` & `pydantic-2.1.1/pydantic/warnings.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/_internal/_annotated_handlers.py` & `pydantic-2.1.1/pydantic/_internal/_annotated_handlers.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/_internal/_config.py` & `pydantic-2.1.1/pydantic/_internal/_config.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/_internal/_core_metadata.py` & `pydantic-2.1.1/pydantic/_internal/_core_metadata.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/_internal/_core_utils.py` & `pydantic-2.1.1/pydantic/_internal/_core_utils.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/_internal/_dataclasses.py` & `pydantic-2.1.1/pydantic/_internal/_dataclasses.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/_internal/_decorators.py` & `pydantic-2.1.1/pydantic/_internal/_decorators.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/_internal/_decorators_v1.py` & `pydantic-2.1.1/pydantic/_internal/_decorators_v1.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/_internal/_discriminated_union.py` & `pydantic-2.1.1/pydantic/_internal/_discriminated_union.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/_internal/_fields.py` & `pydantic-2.1.1/pydantic/_internal/_fields.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/_internal/_generate_schema.py` & `pydantic-2.1.1/pydantic/_internal/_generate_schema.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/_internal/_generics.py` & `pydantic-2.1.1/pydantic/_internal/_generics.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/_internal/_known_annotated_metadata.py` & `pydantic-2.1.1/pydantic/_internal/_known_annotated_metadata.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/_internal/_mock_validator.py` & `pydantic-2.1.1/pydantic/_internal/_mock_validator.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/_internal/_model_construction.py` & `pydantic-2.1.1/pydantic/_internal/_model_construction.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/_internal/_repr.py` & `pydantic-2.1.1/pydantic/_internal/_repr.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/_internal/_schema_generation_shared.py` & `pydantic-2.1.1/pydantic/_internal/_schema_generation_shared.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/_internal/_std_types_schema.py` & `pydantic-2.1.1/pydantic/_internal/_std_types_schema.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/_internal/_typing_extra.py` & `pydantic-2.1.1/pydantic/_internal/_typing_extra.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/_internal/_utils.py` & `pydantic-2.1.1/pydantic/_internal/_utils.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/_internal/_validate_call.py` & `pydantic-2.1.1/pydantic/_internal/_validate_call.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/_internal/_validators.py` & `pydantic-2.1.1/pydantic/_internal/_validators.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/deprecated/class_validators.py` & `pydantic-2.1.1/pydantic/deprecated/class_validators.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/deprecated/config.py` & `pydantic-2.1.1/pydantic/deprecated/config.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/deprecated/copy_internals.py` & `pydantic-2.1.1/pydantic/deprecated/copy_internals.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/deprecated/decorator.py` & `pydantic-2.1.1/pydantic/deprecated/decorator.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/deprecated/json.py` & `pydantic-2.1.1/pydantic/deprecated/json.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/deprecated/parse.py` & `pydantic-2.1.1/pydantic/deprecated/parse.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/deprecated/tools.py` & `pydantic-2.1.1/pydantic/deprecated/tools.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/v1/__init__.py` & `pydantic-2.1.1/pydantic/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/v1/_hypothesis_plugin.py` & `pydantic-2.1.1/pydantic/v1/_hypothesis_plugin.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/v1/annotated_types.py` & `pydantic-2.1.1/pydantic/v1/annotated_types.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/v1/class_validators.py` & `pydantic-2.1.1/pydantic/v1/class_validators.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/v1/color.py` & `pydantic-2.1.1/pydantic/v1/color.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/v1/config.py` & `pydantic-2.1.1/pydantic/v1/config.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/v1/dataclasses.py` & `pydantic-2.1.1/pydantic/v1/dataclasses.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/v1/datetime_parse.py` & `pydantic-2.1.1/pydantic/v1/datetime_parse.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/v1/decorator.py` & `pydantic-2.1.1/pydantic/v1/decorator.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/v1/env_settings.py` & `pydantic-2.1.1/pydantic/v1/env_settings.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/v1/error_wrappers.py` & `pydantic-2.1.1/pydantic/v1/error_wrappers.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/v1/errors.py` & `pydantic-2.1.1/pydantic/v1/errors.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/v1/fields.py` & `pydantic-2.1.1/pydantic/v1/fields.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/v1/generics.py` & `pydantic-2.1.1/pydantic/v1/generics.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/v1/json.py` & `pydantic-2.1.1/pydantic/v1/json.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/v1/main.py` & `pydantic-2.1.1/pydantic/v1/main.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/v1/mypy.py` & `pydantic-2.1.1/pydantic/v1/mypy.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/v1/networks.py` & `pydantic-2.1.1/pydantic/v1/networks.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/v1/parse.py` & `pydantic-2.1.1/pydantic/v1/parse.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/v1/schema.py` & `pydantic-2.1.1/pydantic/v1/schema.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/v1/tools.py` & `pydantic-2.1.1/pydantic/v1/tools.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/v1/types.py` & `pydantic-2.1.1/pydantic/v1/types.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/v1/typing.py` & `pydantic-2.1.1/pydantic/v1/typing.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/v1/utils.py` & `pydantic-2.1.1/pydantic/v1/utils.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/v1/validators.py` & `pydantic-2.1.1/pydantic/v1/validators.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pydantic/v1/version.py` & `pydantic-2.1.1/pydantic/v1/version.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/conftest.py` & `pydantic-2.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_abc.py` & `pydantic-2.1.1/tests/test_abc.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_aliases.py` & `pydantic-2.1.1/tests/test_aliases.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_annotated.py` & `pydantic-2.1.1/tests/test_annotated.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_assert_in_validators.py` & `pydantic-2.1.1/tests/test_assert_in_validators.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_callable.py` & `pydantic-2.1.1/tests/test_callable.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_color.py` & `pydantic-2.1.1/tests/test_color.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_computed_fields.py` & `pydantic-2.1.1/tests/test_computed_fields.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_config.py` & `pydantic-2.1.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_construction.py` & `pydantic-2.1.1/tests/test_construction.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_create_model.py` & `pydantic-2.1.1/tests/test_create_model.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_dataclasses.py` & `pydantic-2.1.1/tests/test_dataclasses.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_datetime.py` & `pydantic-2.1.1/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_decorators.py` & `pydantic-2.1.1/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_deprecated.py` & `pydantic-2.1.1/tests/test_deprecated.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_deprecated_validate_arguments.py` & `pydantic-2.1.1/tests/test_deprecated_validate_arguments.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_discriminated_union.py` & `pydantic-2.1.1/tests/test_discriminated_union.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_docs.py` & `pydantic-2.1.1/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_edge_cases.py` & `pydantic-2.1.1/tests/test_edge_cases.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_errors.py` & `pydantic-2.1.1/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_exports.py` & `pydantic-2.1.1/tests/test_exports.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_fastapi_json_schema.py` & `pydantic-2.1.1/tests/test_fastapi_json_schema.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_fields.py` & `pydantic-2.1.1/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_forward_ref.py` & `pydantic-2.1.1/tests/test_forward_ref.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_generics.py` & `pydantic-2.1.1/tests/test_generics.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_internal.py` & `pydantic-2.1.1/tests/test_internal.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_json.py` & `pydantic-2.1.1/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_json_schema.py` & `pydantic-2.1.1/tests/test_json_schema.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_main.py` & `pydantic-2.1.1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_migration.py` & `pydantic-2.1.1/tests/test_migration.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_model_signature.py` & `pydantic-2.1.1/tests/test_model_signature.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_model_validator.py` & `pydantic-2.1.1/tests/test_model_validator.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_networks.py` & `pydantic-2.1.1/tests/test_networks.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_networks_ipaddress.py` & `pydantic-2.1.1/tests/test_networks_ipaddress.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_parse.py` & `pydantic-2.1.1/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_prepare_annotations.py` & `pydantic-2.1.1/tests/test_prepare_annotations.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_private_attributes.py` & `pydantic-2.1.1/tests/test_private_attributes.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_rich_repr.py` & `pydantic-2.1.1/tests/test_rich_repr.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_root_model.py` & `pydantic-2.1.1/tests/test_root_model.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_serialize.py` & `pydantic-2.1.1/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_strict.py` & `pydantic-2.1.1/tests/test_strict.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_structural_pattern_matching.py` & `pydantic-2.1.1/tests/test_structural_pattern_matching.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_tools.py` & `pydantic-2.1.1/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_type_adapter.py` & `pydantic-2.1.1/tests/test_type_adapter.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_type_alias_type.py` & `pydantic-2.1.1/tests/test_type_alias_type.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_types.py` & `pydantic-2.1.1/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_types_namedtuple.py` & `pydantic-2.1.1/tests/test_types_namedtuple.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_types_payment_card_number.py` & `pydantic-2.1.1/tests/test_types_payment_card_number.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_types_typeddict.py` & `pydantic-2.1.1/tests/test_types_typeddict.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_typing.py` & `pydantic-2.1.1/tests/test_typing.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_utils.py` & `pydantic-2.1.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_v1.py` & `pydantic-2.1.1/tests/test_v1.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_validate_call.py` & `pydantic-2.1.1/tests/test_validate_call.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_validators.py` & `pydantic-2.1.1/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_validators_dataclass.py` & `pydantic-2.1.1/tests/test_validators_dataclass.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_version.py` & `pydantic-2.1.1/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/test_warnings.py` & `pydantic-2.1.1/tests/test_warnings.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/benchmarks/generate_north_star_data.py` & `pydantic-2.1.1/tests/benchmarks/generate_north_star_data.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/benchmarks/test_north_star.py` & `pydantic-2.1.1/tests/benchmarks/test_north_star.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/test_mypy.py` & `pydantic-2.1.1/tests/mypy/test_mypy.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/configs/mypy-plugin-strict-no-any.ini` & `pydantic-2.1.1/tests/mypy/configs/mypy-plugin-strict-no-any.ini`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/configs/pyproject-default.toml` & `pydantic-2.1.1/tests/mypy/configs/pyproject-default.toml`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/configs/pyproject-plugin-bad-param.toml` & `pydantic-2.1.1/tests/mypy/configs/pyproject-plugin-bad-param.toml`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/configs/pyproject-plugin-strict.toml` & `pydantic-2.1.1/tests/mypy/configs/pyproject-plugin-strict.toml`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/configs/pyproject-plugin.toml` & `pydantic-2.1.1/tests/mypy/configs/pyproject-plugin.toml`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/modules/computed_fields.py` & `pydantic-2.1.1/tests/mypy/modules/computed_fields.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/modules/fail4.py` & `pydantic-2.1.1/tests/mypy/modules/fail4.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/modules/generics.py` & `pydantic-2.1.1/tests/mypy/modules/generics.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/modules/metaclass_args.py` & `pydantic-2.1.1/tests/mypy/modules/metaclass_args.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/modules/plugin_default_factory.py` & `pydantic-2.1.1/tests/mypy/modules/plugin_default_factory.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/modules/plugin_fail.py` & `pydantic-2.1.1/tests/mypy/modules/plugin_fail.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/modules/plugin_fail_baseConfig.py` & `pydantic-2.1.1/tests/mypy/modules/plugin_fail_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/modules/plugin_success.py` & `pydantic-2.1.1/tests/mypy/modules/plugin_success.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/modules/plugin_success_baseConfig.py` & `pydantic-2.1.1/tests/mypy/modules/plugin_success_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/modules/success.py` & `pydantic-2.1.1/tests/mypy/modules/success.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.0.1/mypy-default_ini/fail1.py` & `pydantic-2.1.1/tests/mypy/outputs/1.0.1/mypy-default_ini/fail1.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.0.1/mypy-default_ini/fail3.py` & `pydantic-2.1.1/tests/mypy/outputs/1.0.1/mypy-default_ini/fail3.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.0.1/mypy-default_ini/fail4.py` & `pydantic-2.1.1/tests/mypy/outputs/1.0.1/mypy-default_ini/fail4.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.0.1/mypy-default_ini/metaclass_args.py` & `pydantic-2.1.1/tests/mypy/outputs/1.0.1/mypy-default_ini/metaclass_args.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.0.1/mypy-default_ini/plugin_success.py` & `pydantic-2.1.1/tests/mypy/outputs/1.0.1/mypy-default_ini/plugin_success.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.0.1/mypy-default_ini/plugin_success_baseConfig.py` & `pydantic-2.1.1/tests/mypy/outputs/1.0.1/mypy-default_ini/plugin_success_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.0.1/mypy-default_ini/pydantic_settings.py` & `pydantic-2.1.1/tests/mypy/outputs/1.0.1/mypy-default_ini/pydantic_settings.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.0.1/mypy-default_ini/success.py` & `pydantic-2.1.1/tests/mypy/outputs/1.0.1/mypy-default_ini/success.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/fail_defaults.py` & `pydantic-2.1.1/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/fail_defaults.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_default_factory.py` & `pydantic-2.1.1/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_default_factory.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_fail.py` & `pydantic-2.1.1/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_fail.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_fail_baseConfig.py` & `pydantic-2.1.1/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_fail_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_success.py` & `pydantic-2.1.1/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_success.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_success_baseConfig.py` & `pydantic-2.1.1/tests/mypy/outputs/1.0.1/mypy-plugin-strict_ini/plugin_success_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.0.1/mypy-plugin-very-strict_ini/metaclass_args.py` & `pydantic-2.1.1/tests/mypy/outputs/1.0.1/mypy-plugin-very-strict_ini/metaclass_args.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.0.1/mypy-plugin_ini/generics.py` & `pydantic-2.1.1/tests/mypy/outputs/1.0.1/mypy-plugin_ini/generics.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.0.1/mypy-plugin_ini/plugin_fail.py` & `pydantic-2.1.1/tests/mypy/outputs/1.0.1/mypy-plugin_ini/plugin_fail.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.0.1/mypy-plugin_ini/plugin_fail_baseConfig.py` & `pydantic-2.1.1/tests/mypy/outputs/1.0.1/mypy-plugin_ini/plugin_fail_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.0.1/mypy-plugin_ini/plugin_success.py` & `pydantic-2.1.1/tests/mypy/outputs/1.0.1/mypy-plugin_ini/plugin_success.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.0.1/mypy-plugin_ini/plugin_success_baseConfig.py` & `pydantic-2.1.1/tests/mypy/outputs/1.0.1/mypy-plugin_ini/plugin_success_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.0.1/mypy-plugin_ini/pydantic_settings.py` & `pydantic-2.1.1/tests/mypy/outputs/1.0.1/mypy-plugin_ini/pydantic_settings.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.0.1/pyproject-default_toml/computed_fields.py` & `pydantic-2.1.1/tests/mypy/outputs/1.0.1/pyproject-default_toml/computed_fields.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.0.1/pyproject-default_toml/fail1.py` & `pydantic-2.1.1/tests/mypy/outputs/1.0.1/pyproject-default_toml/fail1.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.0.1/pyproject-default_toml/fail3.py` & `pydantic-2.1.1/tests/mypy/outputs/1.0.1/pyproject-default_toml/fail3.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.0.1/pyproject-default_toml/fail4.py` & `pydantic-2.1.1/tests/mypy/outputs/1.0.1/pyproject-default_toml/fail4.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.0.1/pyproject-default_toml/pydantic_settings.py` & `pydantic-2.1.1/tests/mypy/outputs/1.0.1/pyproject-default_toml/pydantic_settings.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.0.1/pyproject-default_toml/success.py` & `pydantic-2.1.1/tests/mypy/outputs/1.0.1/pyproject-default_toml/success.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/fail_defaults.py` & `pydantic-2.1.1/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/fail_defaults.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/plugin_fail.py` & `pydantic-2.1.1/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/plugin_fail.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/plugin_fail_baseConfig.py` & `pydantic-2.1.1/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/plugin_fail_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/plugin_success.py` & `pydantic-2.1.1/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/plugin_success.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/plugin_success_baseConfig.py` & `pydantic-2.1.1/tests/mypy/outputs/1.0.1/pyproject-plugin-strict_toml/plugin_success_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/plugin_fail.py` & `pydantic-2.1.1/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/plugin_fail.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/plugin_fail_baseConfig.py` & `pydantic-2.1.1/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/plugin_fail_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/plugin_success.py` & `pydantic-2.1.1/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/plugin_success.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/plugin_success_baseConfig.py` & `pydantic-2.1.1/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/plugin_success_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/pydantic_settings.py` & `pydantic-2.1.1/tests/mypy/outputs/1.0.1/pyproject-plugin_toml/pydantic_settings.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.1.1/mypy-default_ini/fail1.py` & `pydantic-2.1.1/tests/mypy/outputs/1.1.1/mypy-default_ini/fail1.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.1.1/mypy-default_ini/fail2.py` & `pydantic-2.1.1/tests/mypy/outputs/1.1.1/mypy-default_ini/fail2.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.1.1/mypy-default_ini/metaclass_args.py` & `pydantic-2.1.1/tests/mypy/outputs/1.1.1/mypy-default_ini/metaclass_args.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.1.1/mypy-default_ini/plugin_success.py` & `pydantic-2.1.1/tests/mypy/outputs/1.1.1/mypy-default_ini/plugin_success.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.1.1/mypy-default_ini/plugin_success_baseConfig.py` & `pydantic-2.1.1/tests/mypy/outputs/1.1.1/mypy-default_ini/plugin_success_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.1.1/mypy-default_ini/pydantic_settings.py` & `pydantic-2.1.1/tests/mypy/outputs/1.1.1/mypy-default_ini/pydantic_settings.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.1.1/mypy-plugin_ini/pydantic_settings.py` & `pydantic-2.1.1/tests/mypy/outputs/1.1.1/mypy-plugin_ini/pydantic_settings.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.1.1/pyproject-default_toml/fail1.py` & `pydantic-2.1.1/tests/mypy/outputs/1.1.1/pyproject-default_toml/fail1.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.1.1/pyproject-default_toml/fail2.py` & `pydantic-2.1.1/tests/mypy/outputs/1.1.1/pyproject-default_toml/fail2.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.1.1/pyproject-default_toml/pydantic_settings.py` & `pydantic-2.1.1/tests/mypy/outputs/1.1.1/pyproject-default_toml/pydantic_settings.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.1.1/pyproject-plugin_toml/pydantic_settings.py` & `pydantic-2.1.1/tests/mypy/outputs/1.1.1/pyproject-plugin_toml/pydantic_settings.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.2.0/mypy-default_ini/plugin_success.py` & `pydantic-2.1.1/tests/mypy/outputs/1.2.0/mypy-default_ini/plugin_success.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.2.0/mypy-default_ini/plugin_success_baseConfig.py` & `pydantic-2.1.1/tests/mypy/outputs/1.2.0/mypy-default_ini/plugin_success_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.2.0/mypy-plugin-strict_ini/plugin_fail.py` & `pydantic-2.1.1/tests/mypy/outputs/1.2.0/mypy-plugin-strict_ini/plugin_fail.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.2.0/mypy-plugin-strict_ini/plugin_fail_baseConfig.py` & `pydantic-2.1.1/tests/mypy/outputs/1.2.0/mypy-plugin-strict_ini/plugin_fail_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.2.0/mypy-plugin_ini/plugin_fail.py` & `pydantic-2.1.1/tests/mypy/outputs/1.2.0/mypy-plugin_ini/plugin_fail.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.2.0/mypy-plugin_ini/plugin_fail_baseConfig.py` & `pydantic-2.1.1/tests/mypy/outputs/1.2.0/mypy-plugin_ini/plugin_fail_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.2.0/pyproject-plugin-strict_toml/plugin_fail.py` & `pydantic-2.1.1/tests/mypy/outputs/1.2.0/pyproject-plugin-strict_toml/plugin_fail.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.2.0/pyproject-plugin-strict_toml/plugin_fail_baseConfig.py` & `pydantic-2.1.1/tests/mypy/outputs/1.2.0/pyproject-plugin-strict_toml/plugin_fail_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.2.0/pyproject-plugin_toml/plugin_fail.py` & `pydantic-2.1.1/tests/mypy/outputs/1.2.0/pyproject-plugin_toml/plugin_fail.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.2.0/pyproject-plugin_toml/plugin_fail_baseConfig.py` & `pydantic-2.1.1/tests/mypy/outputs/1.2.0/pyproject-plugin_toml/plugin_fail_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.4.1/mypy-default_ini/fail4.py` & `pydantic-2.1.1/tests/mypy/outputs/1.4.1/mypy-default_ini/fail4.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.4.1/mypy-default_ini/plugin_success.py` & `pydantic-2.1.1/tests/mypy/outputs/1.4.1/mypy-default_ini/plugin_success.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.4.1/mypy-plugin-strict_ini/plugin_default_factory.py` & `pydantic-2.1.1/tests/mypy/outputs/1.4.1/mypy-plugin-strict_ini/plugin_default_factory.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.4.1/mypy-plugin-strict_ini/plugin_fail.py` & `pydantic-2.1.1/tests/mypy/outputs/1.4.1/mypy-plugin-strict_ini/plugin_fail.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.4.1/mypy-plugin-strict_ini/plugin_fail_baseConfig.py` & `pydantic-2.1.1/tests/mypy/outputs/1.4.1/mypy-plugin-strict_ini/plugin_fail_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.4.1/mypy-plugin_ini/plugin_fail.py` & `pydantic-2.1.1/tests/mypy/outputs/1.4.1/mypy-plugin_ini/plugin_fail.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.4.1/mypy-plugin_ini/plugin_fail_baseConfig.py` & `pydantic-2.1.1/tests/mypy/outputs/1.4.1/mypy-plugin_ini/plugin_fail_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.4.1/mypy-plugin_ini/pydantic_settings.py` & `pydantic-2.1.1/tests/mypy/outputs/1.4.1/mypy-plugin_ini/pydantic_settings.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.4.1/pyproject-default_toml/fail4.py` & `pydantic-2.1.1/tests/mypy/outputs/1.4.1/pyproject-default_toml/fail4.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.4.1/pyproject-plugin-strict_toml/plugin_fail.py` & `pydantic-2.1.1/tests/mypy/outputs/1.4.1/pyproject-plugin-strict_toml/plugin_fail.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.4.1/pyproject-plugin-strict_toml/plugin_fail_baseConfig.py` & `pydantic-2.1.1/tests/mypy/outputs/1.4.1/pyproject-plugin-strict_toml/plugin_fail_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.4.1/pyproject-plugin_toml/plugin_fail.py` & `pydantic-2.1.1/tests/mypy/outputs/1.4.1/pyproject-plugin_toml/plugin_fail.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.4.1/pyproject-plugin_toml/plugin_fail_baseConfig.py` & `pydantic-2.1.1/tests/mypy/outputs/1.4.1/pyproject-plugin_toml/plugin_fail_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/mypy/outputs/1.4.1/pyproject-plugin_toml/pydantic_settings.py` & `pydantic-2.1.1/tests/mypy/outputs/1.4.1/pyproject-plugin_toml/pydantic_settings.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/tests/pyright/pyright_example.py` & `pydantic-2.1.1/tests/pyright/pyright_example.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/.gitignore` & `pydantic-2.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/LICENSE` & `pydantic-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/pyproject.toml` & `pydantic-2.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pydantic-2.1.0/PKG-INFO` & `pydantic-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic
-Version: 2.1.0
+Version: 2.1.1
 Summary: Data validation using Python type hints
 Project-URL: Homepage, https://github.com/pydantic/pydantic
 Project-URL: Documentation, https://docs.pydantic.dev
 Project-URL: Funding, https://github.com/sponsors/samuelcolvin
 Project-URL: Source, https://github.com/pydantic/pydantic
 Project-URL: Changelog, https://docs.pydantic.dev/latest/changelog/
 Author-email: Samuel Colvin <s@muelcolvin.com>, Eric Jolibois <em.jolibois@gmail.com>, Hasan Ramezani <hasan.r67@gmail.com>, Adrian Garcia Badaracco <1755071+adriangb@users.noreply.github.com>, Terrence Dorsey <terry@pydantic.dev>, David Montague <david@pydantic.dev>
@@ -109,14 +109,20 @@
 
 ## Reporting a Security Vulnerability
 
 See our [security policy](https://github.com/pydantic/pydantic/security/policy).
 
 ## Changelog
 
+## v2.1.1 (2023-07-25)
+
+[GitHub release](https://github.com/pydantic/pydantic/releases/tag/v2.1.1)
+
+* Skip FieldInfo merging when unnecessary by [@dmontagu](https://github.com/dmontagu) in [#6862](https://github.com/pydantic/pydantic/pull/6862)
+
 ## v2.1.0 (2023-07-25)
 
 [GitHub release](https://github.com/pydantic/pydantic/releases/tag/v2.1.0)
 
 * Add `StringConstraints` for use as Annotated metadata by [@adriangb](https://github.com/adriangb) in [#6605](https://github.com/pydantic/pydantic/pull/6605)
 * Try to fix intermittently failing CI by [@adriangb](https://github.com/adriangb) in [#6683](https://github.com/pydantic/pydantic/pull/6683)
 * Remove redundant example of optional vs default. by [@ehiggs-deliverect](https://github.com/ehiggs-deliverect) in [#6676](https://github.com/pydantic/pydantic/pull/6676)
```

