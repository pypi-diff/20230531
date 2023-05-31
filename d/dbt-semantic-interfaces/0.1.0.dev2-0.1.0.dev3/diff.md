# Comparing `tmp/dbt_semantic_interfaces-0.1.0.dev2.tar.gz` & `tmp/dbt_semantic_interfaces-0.1.0.dev3.tar.gz`

## Comparing `dbt_semantic_interfaces-0.1.0.dev2.tar` & `dbt_semantic_interfaces-0.1.0.dev3.tar`

### file list

```diff
@@ -1,99 +1,99 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/.tool-versions
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/CHANGELOG.md
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/Makefile
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/mypy.ini
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/__init__.py
--rw-r--r--   0        0        0    18186 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/dataclass_serialization.py
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/enum_extension.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/errors.py
--rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/model_transformer.py
--rw-r--r--   0        0        0     5126 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/model_validator.py
--rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/pretty_print.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/py.typed
--rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/references.py
--rw-r--r--   0        0        0     6119 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/implementations/__init__.py
--rw-r--r--   0        0        0     7622 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/implementations/base.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/implementations/metadata.py
--rw-r--r--   0        0        0     7556 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/implementations/metric.py
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/implementations/semantic_manifest.py
--rw-r--r--   0        0        0     6502 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/implementations/semantic_model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/implementations/elements/__init__.py
--rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/implementations/elements/dimension.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/implementations/elements/entity.py
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/implementations/elements/measure.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/implementations/filters/__init__.py
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/implementations/filters/call_parameter_sets.py
--rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/implementations/filters/where_filter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/parsing/__init__.py
--rw-r--r--   0        0        0    13861 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/parsing/dir_to_model.py
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/parsing/explicit_schema.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/parsing/objects.py
--rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/parsing/schema_validator.py
--rw-r--r--   0        0        0     9628 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/parsing/schemas.py
--rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/parsing/yaml_loader.py
--rw-r--r--   0        0        0    14950 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/parsing/schemas/default_explicit_schema.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/protocols/__init__.py
--rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/protocols/dimension.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/protocols/entity.py
--rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/protocols/measure.py
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/protocols/metadata.py
--rw-r--r--   0        0        0     5436 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/protocols/metric.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/protocols/protocol_hint.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/protocols/semantic_manifest.py
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/protocols/semantic_model.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/protocols/where_filter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/transformations/__init__.py
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/transformations/add_input_metric_measures.py
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/transformations/agg_time_dimension.py
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/transformations/boolean_measure.py
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/transformations/convert_count.py
--rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/transformations/convert_median.py
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/transformations/names.py
--rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/transformations/proxy_measure.py
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/transformations/pydantic_rule_set.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/transformations/rule_set.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/transformations/transform_rule.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/type_enums/__init__.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/type_enums/aggregation_type.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/type_enums/dimension_type.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/type_enums/entity_type.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/type_enums/metric_type.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/type_enums/time_granularity.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/validations/__init__.py
--rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/validations/agg_time_dimension.py
--rw-r--r--   0        0        0     3891 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/validations/common_entities.py
--rw-r--r--   0        0        0     7681 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/validations/dimension_const.py
--rw-r--r--   0        0        0     4131 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/validations/element_const.py
--rw-r--r--   0        0        0     5107 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/validations/entities.py
--rw-r--r--   0        0        0    28444 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/validations/measures.py
--rw-r--r--   0        0        0     7432 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/validations/metrics.py
--rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/validations/non_empty.py
--rw-r--r--   0        0        0     6791 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/validations/reserved_keywords.py
--rw-r--r--   0        0        0     9051 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/validations/semantic_models.py
--rw-r--r--   0        0        0     9979 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/validations/unique_valid_name.py
--rw-r--r--   0        0        0    14682 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/validations/validator_helpers.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/venv-3.9.16/pyvenv.cfg
--rw-r--r--   0        0        0     8834 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/venv-3.9.16/bin/Activate.ps1
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/venv-3.9.16/bin/activate
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/venv-3.9.16/bin/activate.csh
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/venv-3.9.16/bin/activate.fish
--rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/venv-3.9.16/bin/hatch
--rwxr-xr-x   0        0        0      293 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/venv-3.9.16/bin/hatchling
--rwxr-xr-x   0        0        0      275 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/venv-3.9.16/bin/httpx
--rwxr-xr-x   0        0        0      281 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/venv-3.9.16/bin/keyring
--rwxr-xr-x   0        0        0      291 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/venv-3.9.16/bin/markdown-it
--rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/venv-3.9.16/bin/pip
--rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/venv-3.9.16/bin/pip3
--rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/venv-3.9.16/bin/pip3.9
--rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/venv-3.9.16/bin/pygmentize
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/venv-3.9.16/bin/python -> /Users/quigleymalcolm/.asdf/installs/python/3.9.16/bin/python
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/venv-3.9.16/bin/python3 -> python
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/venv-3.9.16/bin/python3.9 -> python
--rwxr-xr-x   0        0        0      290 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/venv-3.9.16/bin/userpath
--rwxr-xr-x   0        0        0      309 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/venv-3.9.16/bin/virtualenv
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/LICENSE
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/README.md
--rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/pyproject.toml
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/.tool-versions
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/CHANGELOG.md
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/Makefile
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/mypy.ini
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/__init__.py
+-rw-r--r--   0        0        0    18186 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/dataclass_serialization.py
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/enum_extension.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/errors.py
+-rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/pretty_print.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/py.typed
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/references.py
+-rw-r--r--   0        0        0     6119 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/implementations/__init__.py
+-rw-r--r--   0        0        0     7622 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/implementations/base.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/implementations/metadata.py
+-rw-r--r--   0        0        0     7556 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/implementations/metric.py
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/implementations/semantic_manifest.py
+-rw-r--r--   0        0        0     6502 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/implementations/semantic_model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/implementations/elements/__init__.py
+-rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/implementations/elements/dimension.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/implementations/elements/entity.py
+-rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/implementations/elements/measure.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/implementations/filters/__init__.py
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/implementations/filters/call_parameter_sets.py
+-rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/implementations/filters/where_filter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/parsing/__init__.py
+-rw-r--r--   0        0        0    13889 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/parsing/dir_to_model.py
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/parsing/explicit_schema.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/parsing/objects.py
+-rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/parsing/schema_validator.py
+-rw-r--r--   0        0        0     9628 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/parsing/schemas.py
+-rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/parsing/yaml_loader.py
+-rw-r--r--   0        0        0    14950 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/parsing/schemas/default_explicit_schema.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/protocols/__init__.py
+-rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/protocols/dimension.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/protocols/entity.py
+-rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/protocols/measure.py
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/protocols/metadata.py
+-rw-r--r--   0        0        0     5436 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/protocols/metric.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/protocols/protocol_hint.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/protocols/semantic_manifest.py
+-rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/protocols/semantic_model.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/protocols/where_filter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/transformations/__init__.py
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/transformations/add_input_metric_measures.py
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/transformations/agg_time_dimension.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/transformations/boolean_measure.py
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/transformations/convert_count.py
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/transformations/convert_median.py
+-rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/transformations/names.py
+-rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/transformations/proxy_measure.py
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/transformations/pydantic_rule_set.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/transformations/rule_set.py
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/transformations/semantic_manifest_transformer.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/transformations/transform_rule.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/type_enums/__init__.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/type_enums/aggregation_type.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/type_enums/dimension_type.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/type_enums/entity_type.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/type_enums/metric_type.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/type_enums/time_granularity.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/__init__.py
+-rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/agg_time_dimension.py
+-rw-r--r--   0        0        0     3891 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/common_entities.py
+-rw-r--r--   0        0        0     7681 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/dimension_const.py
+-rw-r--r--   0        0        0     4167 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/element_const.py
+-rw-r--r--   0        0        0     5107 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/entities.py
+-rw-r--r--   0        0        0    28504 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/measures.py
+-rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/metrics.py
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/non_empty.py
+-rw-r--r--   0        0        0     6827 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/reserved_keywords.py
+-rw-r--r--   0        0        0     5150 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/semantic_manifest_validator.py
+-rw-r--r--   0        0        0     9051 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/semantic_models.py
+-rw-r--r--   0        0        0    10051 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/unique_valid_name.py
+-rw-r--r--   0        0        0    14682 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/validator_helpers.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/venv-3.9.16/pyvenv.cfg
+-rw-r--r--   0        0        0     8834 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/venv-3.9.16/bin/Activate.ps1
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/venv-3.9.16/bin/activate
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/venv-3.9.16/bin/activate.csh
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/venv-3.9.16/bin/activate.fish
+-rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/venv-3.9.16/bin/hatch
+-rwxr-xr-x   0        0        0      293 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/venv-3.9.16/bin/hatchling
+-rwxr-xr-x   0        0        0      275 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/venv-3.9.16/bin/httpx
+-rwxr-xr-x   0        0        0      281 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/venv-3.9.16/bin/keyring
+-rwxr-xr-x   0        0        0      291 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/venv-3.9.16/bin/markdown-it
+-rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/venv-3.9.16/bin/pip
+-rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/venv-3.9.16/bin/pip3
+-rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/venv-3.9.16/bin/pip3.9
+-rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/venv-3.9.16/bin/pygmentize
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/venv-3.9.16/bin/python -> /Users/quigleymalcolm/.asdf/installs/python/3.9.16/bin/python
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/venv-3.9.16/bin/python3 -> python
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/venv-3.9.16/bin/python3.9 -> python
+-rwxr-xr-x   0        0        0      290 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/venv-3.9.16/bin/userpath
+-rwxr-xr-x   0        0        0      309 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/venv-3.9.16/bin/virtualenv
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/LICENSE
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/README.md
+-rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/pyproject.toml
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev3/PKG-INFO
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/Makefile` & `dbt_semantic_interfaces-0.1.0.dev3/Makefile`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/dataclass_serialization.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/dataclass_serialization.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/enum_extension.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/enum_extension.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/errors.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/errors.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/model_transformer.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/transformations/semantic_manifest_transformer.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/model_validator.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/semantic_manifest_validator.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,13 +109,13 @@
         for future in as_completed(futures):
             res = future.result()
             result = SemanticManifestValidationResults.parse_raw(res)
             results.append(result)
 
         return SemanticManifestValidationResults.merge(results)
 
-    def checked_validations(self, model: SemanticManifestT) -> None:
+    def checked_validations(self, semantic_manifest: SemanticManifestT) -> None:
         """Similar to validate(), but throws an exception if validation fails."""
-        model_copy = copy.deepcopy(model)
+        model_copy = copy.deepcopy(semantic_manifest)
         model_issues = self.validate_model(model_copy)
         if model_issues.has_blocking_issues:
             raise SemanticManifestValidationException(issues=tuple(model_issues.all_issues))
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/pretty_print.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/pretty_print.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/references.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/references.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/test_utils.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/test_utils.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/implementations/base.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/implementations/base.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/implementations/metric.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/implementations/metric.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/implementations/semantic_manifest.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/implementations/semantic_manifest.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/implementations/semantic_model.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/implementations/semantic_model.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/implementations/elements/dimension.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/implementations/elements/dimension.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/implementations/elements/entity.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/implementations/elements/entity.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/implementations/elements/measure.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/implementations/elements/measure.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/implementations/filters/call_parameter_sets.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/implementations/filters/call_parameter_sets.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/implementations/filters/where_filter.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/implementations/filters/where_filter.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/parsing/dir_to_model.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/parsing/dir_to_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 
 from dbt_semantic_interfaces.errors import ParsingException
 from dbt_semantic_interfaces.implementations.metric import PydanticMetric
 from dbt_semantic_interfaces.implementations.semantic_manifest import (
     PydanticSemanticManifest,
 )
 from dbt_semantic_interfaces.implementations.semantic_model import PydanticSemanticModel
-from dbt_semantic_interfaces.model_transformer import (
-    PydanticSemanticManifestTransformer,
-)
 from dbt_semantic_interfaces.parsing.objects import Version, YamlConfigFile
 from dbt_semantic_interfaces.parsing.schemas import (
     metric_validator,
     semantic_model_validator,
 )
 from dbt_semantic_interfaces.parsing.yaml_loader import (
     PARSING_CONTEXT_KEY,
     ParsingContext,
     YamlConfigLoader,
 )
+from dbt_semantic_interfaces.transformations.semantic_manifest_transformer import (
+    PydanticSemanticManifestTransformer,
+)
 from dbt_semantic_interfaces.validations.validator_helpers import (
     FileContext,
     SemanticManifestValidationException,
     SemanticManifestValidationResults,
     ValidationError,
     ValidationIssue,
 )
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/parsing/explicit_schema.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/parsing/explicit_schema.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/parsing/objects.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/parsing/objects.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/parsing/schema_validator.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/parsing/schema_validator.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/parsing/schemas.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/parsing/schemas.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/parsing/yaml_loader.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/parsing/yaml_loader.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/parsing/schemas/default_explicit_schema.json` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/parsing/schemas/default_explicit_schema.json`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/protocols/dimension.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/protocols/dimension.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/protocols/entity.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/protocols/entity.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/protocols/measure.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/protocols/measure.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/protocols/metadata.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/protocols/metadata.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/protocols/metric.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/protocols/metric.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/protocols/protocol_hint.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/protocols/protocol_hint.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/protocols/semantic_manifest.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/protocols/semantic_manifest.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/protocols/semantic_model.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/protocols/semantic_model.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/transformations/add_input_metric_measures.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/transformations/add_input_metric_measures.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,31 +20,37 @@
     """Add all measures corresponding to the input metrics of the derived metric."""
 
     @override
     def _implements_protocol(self) -> SemanticManifestTransformRule[PydanticSemanticManifest]:  # noqa: D
         return self
 
     @staticmethod
-    def _get_measures_for_metric(model: PydanticSemanticManifest, metric_name: str) -> Set[PydanticMetricInputMeasure]:
+    def _get_measures_for_metric(
+        semantic_manifest: PydanticSemanticManifest, metric_name: str
+    ) -> Set[PydanticMetricInputMeasure]:
         """Returns a unique set of input measures for a given metric."""
         measures = set()
-        matched_metric = next(iter((metric for metric in model.metrics if metric.name == metric_name)), None)
+        matched_metric = next(
+            iter((metric for metric in semantic_manifest.metrics if metric.name == metric_name)), None
+        )
         if matched_metric:
             if matched_metric.type == MetricType.DERIVED:
                 for input_metric in matched_metric.input_metrics:
-                    measures.update(AddInputMetricMeasuresRule._get_measures_for_metric(model, input_metric.name))
+                    measures.update(
+                        AddInputMetricMeasuresRule._get_measures_for_metric(semantic_manifest, input_metric.name)
+                    )
             else:
                 measures.update(set(matched_metric.input_measures))
         else:
             raise ModelTransformError(f"Metric '{metric_name}' is not configured as a metric in the model.")
         return measures
 
     @staticmethod
-    def transform_model(model: PydanticSemanticManifest) -> PydanticSemanticManifest:  # noqa: D
-        for metric in model.metrics:
+    def transform_model(semantic_manifest: PydanticSemanticManifest) -> PydanticSemanticManifest:  # noqa: D
+        for metric in semantic_manifest.metrics:
             if metric.type == MetricType.DERIVED:
-                measures = AddInputMetricMeasuresRule._get_measures_for_metric(model, metric.name)
+                measures = AddInputMetricMeasuresRule._get_measures_for_metric(semantic_manifest, metric.name)
                 assert (
                     metric.type_params.measures is None
                 ), "Derived metric should have no measures predefined in the config"
                 metric.type_params.measures = list(measures)
-        return model
+        return semantic_manifest
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/transformations/agg_time_dimension.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/transformations/agg_time_dimension.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,20 +17,20 @@
     """Sets the aggregation time dimension for measures to the one specified as default."""
 
     @override
     def _implements_protocol(self) -> SemanticManifestTransformRule[PydanticSemanticManifest]:  # noqa: D
         return self
 
     @staticmethod
-    def transform_model(model: PydanticSemanticManifest) -> PydanticSemanticManifest:  # noqa: D
-        for semantic_model in model.semantic_models:
+    def transform_model(semantic_manifest: PydanticSemanticManifest) -> PydanticSemanticManifest:  # noqa: D
+        for semantic_model in semantic_manifest.semantic_models:
             if semantic_model.defaults is None:
                 continue
 
             if semantic_model.defaults.agg_time_dimension is None:
                 continue
 
             for measure in semantic_model.measures:
                 if not measure.agg_time_dimension:
                     measure.agg_time_dimension = semantic_model.defaults.agg_time_dimension
 
-        return model
+        return semantic_manifest
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/transformations/boolean_measure.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/transformations/boolean_measure.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,19 +18,19 @@
     """Converts the expression used in boolean measures so that it can be aggregated."""
 
     @override
     def _implements_protocol(self) -> SemanticManifestTransformRule[PydanticSemanticManifest]:  # noqa: D
         return self
 
     @staticmethod
-    def transform_model(model: PydanticSemanticManifest) -> PydanticSemanticManifest:  # noqa: D
-        for semantic_model in model.semantic_models:
+    def transform_model(semantic_manifest: PydanticSemanticManifest) -> PydanticSemanticManifest:  # noqa: D
+        for semantic_model in semantic_manifest.semantic_models:
             for measure in semantic_model.measures:
                 if measure.agg == AggregationType.SUM_BOOLEAN:
                     if measure.expr:
                         measure.expr = f"CASE WHEN {measure.expr} THEN 1 ELSE 0 END"
                     else:
                         measure.expr = f"CASE WHEN {measure.name} THEN 1 ELSE 0 END"
 
                     measure.agg = AggregationType.SUM
 
-        return model
+        return semantic_manifest
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/transformations/convert_count.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/transformations/convert_count.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,21 +17,21 @@
     """Converts any COUNT measures to SUM equivalent."""
 
     @override
     def _implements_protocol(self) -> SemanticManifestTransformRule[PydanticSemanticManifest]:  # noqa: D
         return self
 
     @staticmethod
-    def transform_model(model: PydanticSemanticManifest) -> PydanticSemanticManifest:  # noqa: D
-        for semantic_model in model.semantic_models:
+    def transform_model(semantic_manifest: PydanticSemanticManifest) -> PydanticSemanticManifest:  # noqa: D
+        for semantic_model in semantic_manifest.semantic_models:
             for measure in semantic_model.measures:
                 if measure.agg == AggregationType.COUNT:
                     if measure.expr is None:
                         raise ModelTransformError(
                             f"Measure '{measure.name}' uses a COUNT aggregation, which requires an expr to be "
                             f"provided. Provide 'expr: 1' if a count of all rows is desired."
                         )
                     if measure.expr != ONE:
                         # Just leave it as SUM(1) if we want to count all
                         measure.expr = f"CASE WHEN {measure.expr} IS NOT NULL THEN 1 ELSE 0 END"
                     measure.agg = AggregationType.SUM
-        return model
+        return semantic_manifest
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/transformations/convert_median.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/transformations/convert_median.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,16 +20,16 @@
     """Converts any MEDIAN measures to percentile equivalent."""
 
     @override
     def _implements_protocol(self) -> SemanticManifestTransformRule[PydanticSemanticManifest]:  # noqa: D
         return self
 
     @staticmethod
-    def transform_model(model: PydanticSemanticManifest) -> PydanticSemanticManifest:  # noqa: D
-        for semantic_model in model.semantic_models:
+    def transform_model(semantic_manifest: PydanticSemanticManifest) -> PydanticSemanticManifest:  # noqa: D
+        for semantic_model in semantic_manifest.semantic_models:
             for measure in semantic_model.measures:
                 if measure.agg == AggregationType.MEDIAN:
                     measure.agg = AggregationType.PERCENTILE
 
                     if not measure.agg_params:
                         measure.agg_params = PydanticMeasureAggregationParameters()
                     else:
@@ -42,8 +42,8 @@
                         if measure.agg_params.use_discrete_percentile:
                             raise ModelTransformError(
                                 f"Measure '{measure.name}' uses a MEDIAN aggregation, while use_discrete_percentile"
                                 f"is set to true. Please remove the parameter or set to False."
                             )
                     measure.agg_params.percentile = MEDIAN_PERCENTILE
                     # let's not set use_approximate_percentile to be false due to valid performance reasons
-        return model
+        return semantic_manifest
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/transformations/names.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/transformations/names.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,20 +18,20 @@
     """Lowercases the names of both top level objects and semantic model elements in a model."""
 
     @override
     def _implements_protocol(self) -> SemanticManifestTransformRule[PydanticSemanticManifest]:  # noqa: D
         return self
 
     @staticmethod
-    def transform_model(model: PydanticSemanticManifest) -> PydanticSemanticManifest:  # noqa: D
-        LowerCaseNamesRule._lowercase_top_level_objects(model)
-        for semantic_model in model.semantic_models:
+    def transform_model(semantic_manifest: PydanticSemanticManifest) -> PydanticSemanticManifest:  # noqa: D
+        LowerCaseNamesRule._lowercase_top_level_objects(semantic_manifest)
+        for semantic_model in semantic_manifest.semantic_models:
             LowerCaseNamesRule._lowercase_semantic_model_elements(semantic_model)
 
-        return model
+        return semantic_manifest
 
     @staticmethod
     def _lowercase_semantic_model_elements(semantic_model: PydanticSemanticModel) -> None:
         """Lowercases the names of semantic model elements."""
         if semantic_model.measures:
             for measure in semantic_model.measures:
                 measure.name = measure.name.lower()
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/transformations/proxy_measure.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/transformations/proxy_measure.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,41 +27,41 @@
     """
 
     @override
     def _implements_protocol(self) -> SemanticManifestTransformRule[PydanticSemanticManifest]:  # noqa: D
         return self
 
     @staticmethod
-    def transform_model(model: PydanticSemanticManifest) -> PydanticSemanticManifest:
+    def transform_model(semantic_manifest: PydanticSemanticManifest) -> PydanticSemanticManifest:
         """Creates measure proxy metrics for measures with `create_metric==True`."""
-        for semantic_model in model.semantic_models:
+        for semantic_model in semantic_manifest.semantic_models:
             for measure in semantic_model.measures:
                 if not measure.create_metric:
                     continue
 
                 add_metric = True
-                for metric in model.metrics:
+                for metric in semantic_manifest.metrics:
                     if metric.name == measure.name:
                         if metric.type != MetricType.SIMPLE:
                             raise ModelTransformError(
                                 f"Cannot have metric with the same name as a measure ({measure.name}) that is not a "
                                 f"proxy for that measure"
                             )
                         logger.warning(
                             f"Metric already exists with name ({measure.name}). *Not* adding measure proxy metric for "
                             f"that measure"
                         )
                         add_metric = False
 
                 if add_metric is True:
-                    model.metrics.append(
+                    semantic_manifest.metrics.append(
                         PydanticMetric(
                             name=measure.name,
                             type=MetricType.SIMPLE,
                             type_params=PydanticMetricTypeParams(
                                 measures=[PydanticMetricInputMeasure(name=measure.name)],
                                 expr=measure.name,
                             ),
                         )
                     )
 
-        return model
+        return semantic_manifest
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/transformations/pydantic_rule_set.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/transformations/pydantic_rule_set.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/transformations/rule_set.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/transformations/rule_set.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/transformations/transform_rule.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/transformations/transform_rule.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from dbt_semantic_interfaces.protocols.semantic_manifest import SemanticManifestT
 
 
 class SemanticManifestTransformRule(Protocol[SemanticManifestT]):
     """Encapsulates logic for transforming a model. e.g. add metrics based on measures."""
 
     @abstractmethod
-    def transform_model(self, model: SemanticManifestT) -> SemanticManifestT:
+    def transform_model(self, semantic_manifest: SemanticManifestT) -> SemanticManifestT:
         """Copy and transform the given model into a new model."""
         pass
 
 
 SemanticManifestTransformRuleT = TypeVar("SemanticManifestTransformRuleT", bound=SemanticManifestTransformRule)
 SemanticManifestTransformRuleT_co = TypeVar(
     "SemanticManifestTransformRuleT_co", bound=SemanticManifestTransformRule, covariant=True
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/type_enums/time_granularity.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/type_enums/time_granularity.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/validations/agg_time_dimension.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/agg_time_dimension.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/validations/common_entities.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/common_entities.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/validations/dimension_const.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/dimension_const.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/validations/element_const.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/element_const.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     the SemanticModelMeasuresUniqueRule.
     """
 
     @staticmethod
     @validate_safely(whats_being_done="running model validation ensuring model wide element consistency")
     def validate_manifest(semantic_manifest: PydanticSemanticManifest) -> Sequence[ValidationIssue]:  # noqa: D
         issues = []
-        element_name_to_types = ElementConsistencyRule._get_element_name_to_types(model=semantic_manifest)
+        element_name_to_types = ElementConsistencyRule._get_element_name_to_types(semantic_manifest=semantic_manifest)
         invalid_elements = {
             name: type_mapping for name, type_mapping in element_name_to_types.items() if len(type_mapping) > 1
         }
 
         for element_name, type_to_context in invalid_elements.items():
             # Sort these by value to ensure consistent error messaging
             types_used = [SemanticModelElementType(v) for v in sorted(k.value for k in type_to_context.keys())]
@@ -50,21 +50,21 @@
                     )
                 )
 
         return issues
 
     @staticmethod
     def _get_element_name_to_types(
-        model: PydanticSemanticManifest,
+        semantic_manifest: PydanticSemanticManifest,
     ) -> DefaultDict[str, DefaultDict[SemanticModelElementType, List[SemanticModelContext]]]:
         """Create a mapping of element names in the semantic manifest to types with a list of associated contexts."""
         element_types: DefaultDict[
             str, DefaultDict[SemanticModelElementType, List[SemanticModelContext]]
         ] = defaultdict(lambda: defaultdict(list))
-        for semantic_model in model.semantic_models:
+        for semantic_model in semantic_manifest.semantic_models:
             semantic_model_context = SemanticModelContext(
                 file_context=FileContext.from_metadata(metadata=semantic_model.metadata),
                 semantic_model=SemanticModelReference(semantic_model_name=semantic_model.name),
             )
             if semantic_model.measures:
                 for measure in semantic_model.measures:
                     element_types[measure.name][SemanticModelElementType.MEASURE].append(semantic_model_context)
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/validations/entities.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/entities.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/validations/measures.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/measures.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,15 +131,15 @@
         """Ensures measures that might need an alias have one set, and that the alias is distinct.
 
         We do not allow aliases to collide with other alias or measure names, since that could create
         ambiguity at query time or cause issues if users ever restructure their models.
         """
         issues: List[ValidationIssue] = []
 
-        measure_names = _get_measure_names_from_model(semantic_manifest)
+        measure_names = _get_measure_names_from_semantic_manifest(semantic_manifest)
         measure_alias_to_metrics: DefaultDict[str, List[str]] = defaultdict(list)
         for metric in semantic_manifest.metrics:
             metric_context = MetricContext(
                 file_context=FileContext.from_metadata(metadata=metric.metadata),
                 metric=MetricModelReference(metric_name=metric.name),
             )
 
@@ -208,15 +208,15 @@
                 )
         return issues
 
     @staticmethod
     @validate_safely(whats_being_done="running model validation ensuring metric measures exist")
     def validate_manifest(semantic_manifest: SemanticManifestT) -> Sequence[ValidationIssue]:  # noqa: D
         issues: List[ValidationIssue] = []
-        valid_measure_names = _get_measure_names_from_model(semantic_manifest)
+        valid_measure_names = _get_measure_names_from_semantic_manifest(semantic_manifest)
 
         for metric in semantic_manifest.metrics or []:
             issues += MetricMeasuresRule._validate_metric_measure_references(
                 metric=metric, valid_measure_names=valid_measure_names
             )
         return issues
 
@@ -514,15 +514,15 @@
                                 f"({wrong_params_str}) only relevant to Percentile measures."
                             ),
                         )
                     )
         return issues
 
 
-def _get_measure_names_from_model(model: SemanticManifest) -> Set[str]:
+def _get_measure_names_from_semantic_manifest(semantic_manifest: SemanticManifest) -> Set[str]:
     """Return every distinct measure name specified in the model."""
     measure_names = set()
-    for semantic_model in model.semantic_models:
+    for semantic_model in semantic_manifest.semantic_models:
         for measure in semantic_model.measures:
             measure_names.add(measure.reference.element_name)
 
     return measure_names
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/validations/metrics.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,19 +96,19 @@
                             )
                         )
                         used_names.add(input_metric.alias)
         return issues
 
     @staticmethod
     @validate_safely(whats_being_done="checking that the input metrics exist")
-    def _validate_input_metrics_exist(model: SemanticManifest) -> List[ValidationIssue]:
+    def _validate_input_metrics_exist(semantic_manifest: SemanticManifest) -> List[ValidationIssue]:
         issues: List[ValidationIssue] = []
 
-        all_metrics = {m.name for m in model.metrics}
-        for metric in model.metrics:
+        all_metrics = {m.name for m in semantic_manifest.metrics}
+        for metric in semantic_manifest.metrics:
             if metric.type == MetricType.DERIVED:
                 for input_metric in metric.input_metrics:
                     if input_metric.name not in all_metrics:
                         issues.append(
                             ValidationError(
                                 context=MetricContext(
                                     file_context=FileContext.from_metadata(metadata=metric.metadata),
@@ -143,12 +143,12 @@
     @staticmethod
     @validate_safely(
         whats_being_done="running model validation ensuring derived metrics properties are configured properly"
     )
     def validate_manifest(semantic_manifest: SemanticManifestT) -> Sequence[ValidationIssue]:  # noqa: D
         issues: List[ValidationIssue] = []
 
-        issues += DerivedMetricRule._validate_input_metrics_exist(model=semantic_manifest)
+        issues += DerivedMetricRule._validate_input_metrics_exist(semantic_manifest=semantic_manifest)
         for metric in semantic_manifest.metrics or []:
             issues += DerivedMetricRule._validate_alias_collision(metric=metric)
             issues += DerivedMetricRule._validate_time_offset_params(metric=metric)
         return issues
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/validations/non_empty.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/non_empty.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,45 +13,45 @@
 
 
 class NonEmptyRule(SemanticManifestValidationRule[SemanticManifestT], Generic[SemanticManifestT]):
     """Check if the model contains semantic models and metrics."""
 
     @staticmethod
     @validate_safely(whats_being_done="checking that the model has semantic models")
-    def _check_model_has_semantic_models(model: PydanticSemanticManifest) -> List[ValidationIssue]:
+    def _check_model_has_semantic_models(semantic_manifest: PydanticSemanticManifest) -> List[ValidationIssue]:
         issues: List[ValidationIssue] = []
-        if not model.semantic_models:
+        if not semantic_manifest.semantic_models:
             issues.append(
                 ValidationError(
                     message="No semantic models present in the model.",
                 )
             )
         return issues
 
     @staticmethod
     @validate_safely(whats_being_done="checking that the model has metrics")
-    def _check_model_has_metrics(model: PydanticSemanticManifest) -> List[ValidationIssue]:
+    def _check_model_has_metrics(semantic_manifest: PydanticSemanticManifest) -> List[ValidationIssue]:
         issues: List[ValidationIssue] = []
 
         # If we are going to generate measure proxy metrics that is sufficient as well
         create_measure_proxy_metrics = False
-        for semantic_model in model.semantic_models:
+        for semantic_model in semantic_manifest.semantic_models:
             for measure in semantic_model.measures:
                 if measure.create_metric is True:
                     create_measure_proxy_metrics = True
                     break
 
-        if not model.metrics and not create_measure_proxy_metrics:
+        if not semantic_manifest.metrics and not create_measure_proxy_metrics:
             issues.append(
                 ValidationError(
                     message="No metrics present in the model.",
                 )
             )
         return issues
 
     @staticmethod
     @validate_safely("running model validation rule ensuring metrics and semantic models are defined")
     def validate_manifest(semantic_manifest: PydanticSemanticManifest) -> Sequence[ValidationIssue]:  # noqa: D
         issues: List[ValidationIssue] = []
-        issues += NonEmptyRule._check_model_has_semantic_models(model=semantic_manifest)
-        issues += NonEmptyRule._check_model_has_metrics(model=semantic_manifest)
+        issues += NonEmptyRule._check_model_has_semantic_models(semantic_manifest=semantic_manifest)
+        issues += NonEmptyRule._check_model_has_metrics(semantic_manifest=semantic_manifest)
         return issues
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/validations/reserved_keywords.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/reserved_keywords.py`

 * *Files 6% similar despite different names*

```diff
@@ -121,20 +121,20 @@
                     )
                 )
 
         return issues
 
     @classmethod
     @validate_safely(whats_being_done="checking that semantic_model node_relations are not sql reserved keywords")
-    def _validate_semantic_models(cls, model: SemanticManifest) -> List[ValidationIssue]:
+    def _validate_semantic_models(cls, semantic_manifest: SemanticManifest) -> List[ValidationIssue]:
         """Checks names of objects that are not nested."""
         issues: List[ValidationIssue] = []
         set_keywords = set(RESERVED_KEYWORDS)
 
-        for semantic_model in model.semantic_models:
+        for semantic_model in semantic_manifest.semantic_models:
             set_sql_table_path_parts = set(
                 [part.upper() for part in semantic_model.node_relation.relation_name.split(".")]
             )
             keyword_intersection = set_keywords.intersection(set_sql_table_path_parts)
 
             if len(keyword_intersection) > 0:
                 issues.append(
@@ -153,8 +153,8 @@
 
     @classmethod
     @validate_safely(
         whats_being_done="running model validation ensuring elements that aren't selected via a defined expr don't "
         "contain reserved keywords"
     )
     def validate_manifest(cls, semantic_manifest: SemanticManifest) -> List[ValidationIssue]:  # noqa: D
-        return cls._validate_semantic_models(model=semantic_manifest)
+        return cls._validate_semantic_models(semantic_manifest=semantic_manifest)
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/validations/semantic_models.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/semantic_models.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/validations/unique_valid_name.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/unique_valid_name.py`

 * *Files 4% similar despite different names*

```diff
@@ -160,19 +160,19 @@
         for name, _, context in element_info_tuples:
             issues += UniqueAndValidNameRule.check_valid_name(name=name.element_name, context=context)
 
         return issues
 
     @staticmethod
     @validate_safely(whats_being_done="checking model top level element names are sufficiently unique")
-    def _validate_top_level_objects(model: SemanticManifest) -> List[ValidationIssue]:
+    def _validate_top_level_objects(semantic_manifest: SemanticManifest) -> List[ValidationIssue]:
         """Checks names of objects that are not nested."""
         object_info_tuples = []
-        if model.semantic_models:
-            for semantic_model in model.semantic_models:
+        if semantic_manifest.semantic_models:
+            for semantic_model in semantic_manifest.semantic_models:
                 object_info_tuples.append(
                     (
                         semantic_model.name,
                         "semantic model",
                         SemanticModelContext(
                             file_context=FileContext.from_metadata(metadata=semantic_model.metadata),
                             semantic_model=SemanticModelReference(semantic_model_name=semantic_model.name),
@@ -192,17 +192,17 @@
                         message=f"Can't use name `{name}` for a {type_} when it was already used for a "
                         f"{name_to_type[name]}",
                     )
                 )
             else:
                 name_to_type[name] = type_
 
-        if model.metrics:
+        if semantic_manifest.metrics:
             metric_names = set()
-            for metric in model.metrics:
+            for metric in semantic_manifest.metrics:
                 if metric.name in metric_names:
                     issues.append(
                         ValidationError(
                             context=MetricContext(
                                 file_context=FileContext.from_metadata(metadata=metric.metadata),
                                 metric=MetricModelReference(metric_name=metric.name),
                             ),
@@ -218,13 +218,13 @@
 
         return issues
 
     @staticmethod
     @validate_safely(whats_being_done="running model validation ensuring elements have adequately unique names")
     def validate_manifest(semantic_manifest: SemanticManifestT) -> Sequence[ValidationIssue]:  # noqa: D
         issues = []
-        issues += UniqueAndValidNameRule._validate_top_level_objects(model=semantic_manifest)
+        issues += UniqueAndValidNameRule._validate_top_level_objects(semantic_manifest=semantic_manifest)
 
         for semantic_model in semantic_manifest.semantic_models:
             issues += UniqueAndValidNameRule._validate_semantic_model_elements(semantic_model=semantic_model)
 
         return issues
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/validations/validator_helpers.py` & `dbt_semantic_interfaces-0.1.0.dev3/dbt_semantic_interfaces/validations/validator_helpers.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/venv-3.9.16/bin/Activate.ps1` & `dbt_semantic_interfaces-0.1.0.dev3/venv-3.9.16/bin/Activate.ps1`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/venv-3.9.16/bin/activate` & `dbt_semantic_interfaces-0.1.0.dev3/venv-3.9.16/bin/activate`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/venv-3.9.16/bin/activate.csh` & `dbt_semantic_interfaces-0.1.0.dev3/venv-3.9.16/bin/activate.csh`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/venv-3.9.16/bin/activate.fish` & `dbt_semantic_interfaces-0.1.0.dev3/venv-3.9.16/bin/activate.fish`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/.gitignore` & `dbt_semantic_interfaces-0.1.0.dev3/.gitignore`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/LICENSE` & `dbt_semantic_interfaces-0.1.0.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/README.md` & `dbt_semantic_interfaces-0.1.0.dev3/README.md`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/pyproject.toml` & `dbt_semantic_interfaces-0.1.0.dev3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dbt-semantic-interfaces"
-version = "0.1.0.dev2"
+version = "0.1.0.dev3"
 description = 'The shared semantic layer definitions that dbt-core and MetricFlow use'
 readme = "README.md"
 requires-python = ">=3.8"
 license = "Apache-2.0"
 keywords = []
 authors = [
   { name = "dbt Labs", email = "info@dbtlabs.com" },
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev2/PKG-INFO` & `dbt_semantic_interfaces-0.1.0.dev3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-semantic-interfaces
-Version: 0.1.0.dev2
+Version: 0.1.0.dev3
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
-Metadata-Version: 2.1 Name: dbt-semantic-interfaces Version: 0.1.0.dev2
+Metadata-Version: 2.1 Name: dbt-semantic-interfaces Version: 0.1.0.dev3
 Summary: The shared semantic layer definitions that dbt-core and MetricFlow use
 Author-email: dbt Labs
 dbtlabs.com> License-Expression: Apache-2.0 License-File: LICENSE Classifier:
 Development Status :: 4 - Beta Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
```

