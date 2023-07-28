# Comparing `tmp/dbt_semantic_interfaces-0.1.0rc1.tar.gz` & `tmp/dbt_semantic_interfaces-0.2.0.tar.gz`

## Comparing `dbt_semantic_interfaces-0.1.0rc1.tar` & `dbt_semantic_interfaces-0.2.0.tar`

### file list

```diff
@@ -1,105 +1,129 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/.tool-versions
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/CHANGELOG.md
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/Makefile
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/mypy.ini
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/__init__.py
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/call_parameter_sets.py
--rw-r--r--   0        0        0    18186 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/dataclass_serialization.py
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/enum_extension.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/errors.py
--rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/pretty_print.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/py.typed
--rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/references.py
--rw-r--r--   0        0        0     6161 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/implementations/__init__.py
--rw-r--r--   0        0        0     7622 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/implementations/base.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/implementations/metadata.py
--rw-r--r--   0        0        0     7699 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/implementations/metric.py
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/implementations/project_configuration.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/implementations/semantic_manifest.py
--rw-r--r--   0        0        0     7269 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/implementations/semantic_model.py
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/implementations/semantic_version.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/implementations/time_spine_table_configuration.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/implementations/elements/__init__.py
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/implementations/elements/dimension.py
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/implementations/elements/entity.py
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/implementations/elements/measure.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/implementations/filters/__init__.py
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/implementations/filters/where_filter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/parsing/__init__.py
--rw-r--r--   0        0        0    15513 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/parsing/dir_to_model.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/parsing/generate_json_schema_file.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/parsing/objects.py
--rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/parsing/schema_validator.py
--rw-r--r--   0        0        0     9860 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/parsing/schemas.py
--rw-r--r--   0        0        0     3878 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/parsing/where_filter_parser.py
--rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/parsing/yaml_loader.py
--rw-r--r--   0        0        0    15414 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/parsing/generated_json_schemas/default_explicit_schema.json
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/protocols/__init__.py
--rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/protocols/dimension.py
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/protocols/entity.py
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/protocols/measure.py
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/protocols/metadata.py
--rw-r--r--   0        0        0     5164 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/protocols/metric.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/protocols/project_configuration.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/protocols/protocol_hint.py
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/protocols/semantic_manifest.py
--rw-r--r--   0        0        0     4260 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/protocols/semantic_model.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/protocols/semantic_version.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/protocols/time_spine_configuration.py
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/protocols/where_filter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/transformations/__init__.py
--rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/transformations/add_input_metric_measures.py
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/transformations/boolean_measure.py
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/transformations/convert_count.py
--rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/transformations/convert_median.py
--rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/transformations/names.py
--rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/transformations/proxy_measure.py
--rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/transformations/pydantic_rule_set.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/transformations/rule_set.py
--rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/transformations/semantic_manifest_transformer.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/transformations/transform_rule.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/type_enums/__init__.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/type_enums/aggregation_type.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/type_enums/dimension_type.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/type_enums/entity_type.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/type_enums/metric_type.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/type_enums/time_granularity.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/validations/__init__.py
--rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/validations/agg_time_dimension.py
--rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/validations/common_entities.py
--rw-r--r--   0        0        0     7487 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/validations/dimension_const.py
--rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/validations/element_const.py
--rw-r--r--   0        0        0     5017 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/validations/entities.py
--rw-r--r--   0        0        0    28374 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/validations/measures.py
--rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/validations/metrics.py
--rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/validations/non_empty.py
--rw-r--r--   0        0        0     6753 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/validations/reserved_keywords.py
--rw-r--r--   0        0        0     5120 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/validations/semantic_manifest_validator.py
--rw-r--r--   0        0        0     9212 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/validations/semantic_models.py
--rw-r--r--   0        0        0     9960 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/validations/unique_valid_name.py
--rw-r--r--   0        0        0    15056 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/validations/validator_helpers.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/venv-3.9.16/pyvenv.cfg
--rw-r--r--   0        0        0     8834 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/venv-3.9.16/bin/Activate.ps1
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/venv-3.9.16/bin/activate
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/venv-3.9.16/bin/activate.csh
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/venv-3.9.16/bin/activate.fish
--rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/venv-3.9.16/bin/hatch
--rwxr-xr-x   0        0        0      293 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/venv-3.9.16/bin/hatchling
--rwxr-xr-x   0        0        0      275 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/venv-3.9.16/bin/httpx
--rwxr-xr-x   0        0        0      281 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/venv-3.9.16/bin/keyring
--rwxr-xr-x   0        0        0      291 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/venv-3.9.16/bin/markdown-it
--rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/venv-3.9.16/bin/pip
--rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/venv-3.9.16/bin/pip3
--rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/venv-3.9.16/bin/pip3.9
--rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/venv-3.9.16/bin/pygmentize
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/venv-3.9.16/bin/python -> /Users/quigleymalcolm/.asdf/installs/python/3.9.16/bin/python
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/venv-3.9.16/bin/python3 -> python
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/venv-3.9.16/bin/python3.9 -> python
--rwxr-xr-x   0        0        0      290 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/venv-3.9.16/bin/userpath
--rwxr-xr-x   0        0        0      309 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/venv-3.9.16/bin/virtualenv
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/LICENSE
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/README.md
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/pyproject.toml
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0rc1/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/.tool-versions
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/Makefile
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/mypy.ini
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/__init__.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/call_parameter_sets.py
+-rw-r--r--   0        0        0    18186 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/dataclass_serialization.py
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/enum_extension.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/errors.py
+-rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/pretty_print.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/py.typed
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/references.py
+-rw-r--r--   0        0        0     6161 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/implementations/__init__.py
+-rw-r--r--   0        0        0     7622 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/implementations/base.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/implementations/metadata.py
+-rw-r--r--   0        0        0     7699 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/implementations/metric.py
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/implementations/project_configuration.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/implementations/semantic_manifest.py
+-rw-r--r--   0        0        0     7568 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/implementations/semantic_model.py
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/implementations/semantic_version.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/implementations/time_spine_table_configuration.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/implementations/elements/__init__.py
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/implementations/elements/dimension.py
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/implementations/elements/entity.py
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/implementations/elements/measure.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/implementations/filters/__init__.py
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/implementations/filters/where_filter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/naming/__init__.py
+-rw-r--r--   0        0        0     5393 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/naming/dundered.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/naming/keywords.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/parsing/__init__.py
+-rw-r--r--   0        0        0    15513 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/parsing/dir_to_model.py
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/parsing/generate_json_schema_file.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/parsing/objects.py
+-rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/parsing/schema_validator.py
+-rw-r--r--   0        0        0     9929 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/parsing/schemas.py
+-rw-r--r--   0        0        0     6588 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/parsing/where_filter_parser.py
+-rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/parsing/yaml_loader.py
+-rw-r--r--   0        0        0    15506 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/parsing/generated_json_schemas/default_explicit_schema.json
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/protocols/__init__.py
+-rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/protocols/dimension.py
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/protocols/entity.py
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/protocols/measure.py
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/protocols/metadata.py
+-rw-r--r--   0        0        0     5164 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/protocols/metric.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/protocols/project_configuration.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/protocols/protocol_hint.py
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/protocols/semantic_manifest.py
+-rw-r--r--   0        0        0     4907 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/protocols/semantic_model.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/protocols/semantic_version.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/protocols/time_spine_configuration.py
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/protocols/where_filter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/transformations/__init__.py
+-rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/transformations/add_input_metric_measures.py
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/transformations/boolean_measure.py
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/transformations/convert_count.py
+-rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/transformations/convert_median.py
+-rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/transformations/names.py
+-rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/transformations/proxy_measure.py
+-rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/transformations/pydantic_rule_set.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/transformations/rule_set.py
+-rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/transformations/semantic_manifest_transformer.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/transformations/transform_rule.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/type_enums/__init__.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/type_enums/aggregation_type.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/type_enums/dimension_type.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/type_enums/entity_type.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/type_enums/metric_type.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/type_enums/time_granularity.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/validations/__init__.py
+-rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/validations/agg_time_dimension.py
+-rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/validations/common_entities.py
+-rw-r--r--   0        0        0     7487 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/validations/dimension_const.py
+-rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/validations/element_const.py
+-rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/validations/entities.py
+-rw-r--r--   0        0        0    28374 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/validations/measures.py
+-rw-r--r--   0        0        0    12665 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/validations/metrics.py
+-rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/validations/non_empty.py
+-rw-r--r--   0        0        0     4596 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/validations/primary_entity.py
+-rw-r--r--   0        0        0     6753 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/validations/reserved_keywords.py
+-rw-r--r--   0        0        0     6150 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/validations/semantic_manifest_validator.py
+-rw-r--r--   0        0        0     9212 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/validations/semantic_models.py
+-rw-r--r--   0        0        0    13043 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/validations/unique_valid_name.py
+-rw-r--r--   0        0        0    15050 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/validations/validator_helpers.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/pkg/__about__.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/venv-3.11.4/pyvenv.cfg
+-rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/venv-3.11.4/bin/Activate.ps1
+-rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/venv-3.11.4/bin/activate
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/venv-3.11.4/bin/activate.csh
+-rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/venv-3.11.4/bin/activate.fish
+-rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/venv-3.11.4/bin/hatch
+-rwxr-xr-x   0        0        0      293 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/venv-3.11.4/bin/hatchling
+-rwxr-xr-x   0        0        0      275 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/venv-3.11.4/bin/httpx
+-rwxr-xr-x   0        0        0      281 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/venv-3.11.4/bin/keyring
+-rwxr-xr-x   0        0        0      291 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/venv-3.11.4/bin/markdown-it
+-rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/venv-3.11.4/bin/pip
+-rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/venv-3.11.4/bin/pip3
+-rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/venv-3.11.4/bin/pip3.11
+-rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/venv-3.11.4/bin/pygmentize
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/venv-3.11.4/bin/python -> /Users/quigleymalcolm/.asdf/installs/python/3.11.4/bin/python
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/venv-3.11.4/bin/python3 -> python
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/venv-3.11.4/bin/python3.11 -> python
+-rwxr-xr-x   0        0        0      290 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/venv-3.11.4/bin/userpath
+-rwxr-xr-x   0        0        0      309 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/venv-3.11.4/bin/virtualenv
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/venv-3.9.16/pyvenv.cfg
+-rw-r--r--   0        0        0     8834 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/venv-3.9.16/bin/Activate.ps1
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/venv-3.9.16/bin/activate
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/venv-3.9.16/bin/activate.csh
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/venv-3.9.16/bin/activate.fish
+-rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/venv-3.9.16/bin/hatch
+-rwxr-xr-x   0        0        0      293 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/venv-3.9.16/bin/hatchling
+-rwxr-xr-x   0        0        0      275 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/venv-3.9.16/bin/httpx
+-rwxr-xr-x   0        0        0      281 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/venv-3.9.16/bin/keyring
+-rwxr-xr-x   0        0        0      291 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/venv-3.9.16/bin/markdown-it
+-rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/venv-3.9.16/bin/pip
+-rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/venv-3.9.16/bin/pip3
+-rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/venv-3.9.16/bin/pip3.9
+-rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/venv-3.9.16/bin/pygmentize
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/venv-3.9.16/bin/python -> /Users/quigleymalcolm/.asdf/installs/python/3.9.16/bin/python
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/venv-3.9.16/bin/python3 -> python
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/venv-3.9.16/bin/python3.9 -> python
+-rwxr-xr-x   0        0        0      290 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/venv-3.9.16/bin/userpath
+-rwxr-xr-x   0        0        0      309 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/venv-3.9.16/bin/virtualenv
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/README.md
+-rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.2.0/PKG-INFO
```

### Comparing `dbt_semantic_interfaces-0.1.0rc1/Makefile` & `dbt_semantic_interfaces-0.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/call_parameter_sets.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/call_parameter_sets.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/dataclass_serialization.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/dataclass_serialization.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/enum_extension.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/enum_extension.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/errors.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/errors.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/pretty_print.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/pretty_print.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/references.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/references.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/test_utils.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/test_utils.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/implementations/base.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/implementations/base.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/implementations/metric.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/implementations/metric.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/implementations/project_configuration.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/implementations/project_configuration.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/implementations/semantic_manifest.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/implementations/semantic_manifest.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/implementations/semantic_model.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/implementations/semantic_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from dbt_semantic_interfaces.implementations.metadata import PydanticMetadata
 from dbt_semantic_interfaces.protocols import (
     ProtocolHint,
     SemanticModel,
     SemanticModelDefaults,
 )
 from dbt_semantic_interfaces.references import (
+    EntityReference,
     LinkableElementReference,
     MeasureReference,
     SemanticModelReference,
     TimeDimensionReference,
 )
 
 
@@ -83,14 +84,15 @@
         return self
 
     name: str
     defaults: Optional[PydanticSemanticModelDefaults]
     description: Optional[str]
     node_relation: NodeRelation
 
+    primary_entity: Optional[str]
     entities: Sequence[PydanticEntity] = []
     measures: Sequence[PydanticMeasure] = []
     dimensions: Sequence[PydanticDimension] = []
 
     metadata: Optional[PydanticMetadata]
 
     @property
@@ -165,19 +167,24 @@
     def get_entity(self, entity_reference: LinkableElementReference) -> PydanticEntity:  # noqa: D
         for entity in self.entities:
             if entity.reference == entity_reference:
                 return entity
 
         raise ValueError(f"No entity with name ({entity_reference}) in semantic_model with name ({self.name})")
 
-    def checked_agg_time_dimension_for_measure(self, measure_reference: MeasureReference):  # noqa: D
+    def checked_agg_time_dimension_for_measure(  # noqa: D
+        self, measure_reference: MeasureReference
+    ) -> TimeDimensionReference:
         measure = self.get_measure(measure_reference=measure_reference)
-        if self.defaults is not None:
-            default_agg_time_dimesion = self.defaults.agg_time_dimension
+        default_agg_time_dimension = self.defaults.agg_time_dimension if self.defaults is not None else None
 
-        agg_time_dimension_name = measure.agg_time_dimension or default_agg_time_dimesion
+        agg_time_dimension_name = measure.agg_time_dimension or default_agg_time_dimension
         assert agg_time_dimension_name is not None, (
             f"Aggregation time dimension for measure {measure.name} is not set! This should either be set directly on "
             f"the measure specification in the model, or else defaulted to the primary time dimension in the data "
             f"source containing the measure."
         )
         return TimeDimensionReference(element_name=agg_time_dimension_name)
+
+    @property
+    def primary_entity_reference(self) -> Optional[EntityReference]:  # noqa: D
+        return EntityReference(element_name=self.primary_entity) if self.primary_entity is not None else None
```

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/implementations/semantic_version.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/implementations/semantic_version.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/implementations/time_spine_table_configuration.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/implementations/time_spine_table_configuration.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/implementations/elements/dimension.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/implementations/elements/dimension.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/implementations/elements/entity.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/implementations/elements/entity.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/implementations/elements/measure.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/implementations/elements/measure.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/implementations/filters/where_filter.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/implementations/filters/where_filter.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/parsing/dir_to_model.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/parsing/dir_to_model.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/parsing/generate_json_schema_file.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/parsing/generate_json_schema_file.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/parsing/objects.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/parsing/objects.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/parsing/schema_validator.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/parsing/schema_validator.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/parsing/schemas.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/parsing/schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -275,14 +275,17 @@
     "properties": {
         "name": {
             "type": "string",
             "pattern": TRANSFORM_OBJECT_NAME_PATTERN,
         },
         "node_relation": {"$ref": "node_relation_schema"},
         "defaults": {"$ref": "semantic_model_defaults_schema"},
+        "primary_entity": {
+            "type": "string",
+        },
         "entities": {"type": "array", "items": {"$ref": "entity_schema"}},
         "measures": {"type": "array", "items": {"$ref": "measure_schema"}},
         "dimensions": {"type": "array", "items": {"$ref": "dimension_schema"}},
         "description": {"type": "string"},
     },
     "additionalProperties": False,
     "required": ["name"],
```

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/parsing/yaml_loader.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/parsing/yaml_loader.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/parsing/generated_json_schemas/default_explicit_schema.json` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/parsing/generated_json_schemas/default_explicit_schema.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999632352941177%*

 * *Differences: {"'definitions'": "{'semantic_model_schema': {'properties': {'primary_entity': "*

 * *                  "OrderedDict([('type', 'string')])}}}"}*

```diff
@@ -432,14 +432,17 @@
                 },
                 "name": {
                     "pattern": "(?!.*__).*^[a-z][a-z0-9_]*[a-z0-9]$",
                     "type": "string"
                 },
                 "node_relation": {
                     "$ref": "#/definitions/node_relation_schema"
+                },
+                "primary_entity": {
+                    "type": "string"
                 }
             },
             "required": [
                 "name"
             ],
             "type": "object"
         },
```

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/protocols/__init__.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/protocols/dimension.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/protocols/dimension.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/protocols/entity.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/protocols/entity.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     def reference(self) -> EntityReference:
         """Returns a reference to the entity."""
         ...
 
     @property
     @abstractmethod
     def is_linkable_entity_type(self) -> bool:
-        """Indicates whether or not this entity can be used as a linkable entity type for joins.
+        """Indicates whether this entity can be used as a linkable entity type for joins.
 
         That is, can you use the entity as a linkable element in multi-hop dundered syntax. For example,
         the country dimension in the listings data source can be linked via listing__country, because listing
         is the primary key.
 
         At the moment, you may only request things accessible via primary, unique, or natural keys, with natural
         keys reserved for SCD Type II style data sources.
```

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/protocols/measure.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/protocols/measure.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/protocols/metadata.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/protocols/metadata.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/protocols/metric.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/protocols/metric.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/protocols/project_configuration.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/protocols/project_configuration.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/protocols/protocol_hint.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/protocols/protocol_hint.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/protocols/semantic_manifest.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/protocols/semantic_manifest.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/protocols/semantic_model.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/protocols/semantic_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import Optional, Protocol, Sequence, TypeVar
 
 from dbt_semantic_interfaces.protocols.dimension import Dimension
 from dbt_semantic_interfaces.protocols.entity import Entity
 from dbt_semantic_interfaces.protocols.measure import Measure
 from dbt_semantic_interfaces.protocols.metadata import Metadata
 from dbt_semantic_interfaces.references import (
+    EntityReference,
     LinkableElementReference,
     MeasureReference,
     SemanticModelReference,
     TimeDimensionReference,
 )
 
 
@@ -71,14 +72,25 @@
     @property
     @abstractmethod
     def node_relation(self) -> NodeRelation:  # noqa: D
         pass
 
     @property
     @abstractmethod
+    def primary_entity(self) -> Optional[str]:
+        """The primary entity for dimensions listed in this model.
+
+        This is for cases where there are dimensions in the model, but no entity with primary type. This allows those
+        dimensions to be accessed as dimensions need to be qualified by an entity for access. This may be None if there
+        are no dimensions in this model.
+        """
+        pass
+
+    @property
+    @abstractmethod
     def entities(self) -> Sequence[Entity]:  # noqa: D
         pass
 
     @property
     @abstractmethod
     def measures(self) -> Sequence[Measure]:  # noqa: D
         pass
@@ -151,9 +163,15 @@
     def checked_agg_time_dimension_for_measure(self, measure_reference: MeasureReference) -> TimeDimensionReference:
         """Returns the `TimeDimensionReference` what a measure should use for it's `agg_time_dimension`.
 
         Should raise an exception if a TimeDimensionReference cannot be built
         """
         ...
 
+    @property
+    @abstractmethod
+    def primary_entity_reference(self) -> Optional[EntityReference]:
+        """Reference object form of primary_entity."""
+        pass
+
 
 SemanticModelT = TypeVar("SemanticModelT", bound=SemanticModel)
```

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/protocols/time_spine_configuration.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/protocols/time_spine_configuration.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/protocols/where_filter.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/protocols/where_filter.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/transformations/add_input_metric_measures.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/transformations/add_input_metric_measures.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/transformations/boolean_measure.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/transformations/boolean_measure.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/transformations/convert_count.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/transformations/convert_count.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/transformations/convert_median.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/transformations/convert_median.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/transformations/names.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/transformations/names.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/transformations/proxy_measure.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/transformations/proxy_measure.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/transformations/pydantic_rule_set.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/transformations/pydantic_rule_set.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/transformations/rule_set.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/transformations/rule_set.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/transformations/semantic_manifest_transformer.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/transformations/semantic_manifest_transformer.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/transformations/transform_rule.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/transformations/transform_rule.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/type_enums/time_granularity.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/type_enums/time_granularity.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/validations/agg_time_dimension.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/validations/agg_time_dimension.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/validations/common_entities.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/validations/common_entities.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/validations/dimension_const.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/validations/dimension_const.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/validations/element_const.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/validations/element_const.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/validations/measures.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/validations/measures.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/validations/non_empty.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/validations/non_empty.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/validations/reserved_keywords.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/validations/reserved_keywords.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/validations/semantic_manifest_validator.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/validations/semantic_manifest_validator.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,37 +5,39 @@
 
 from dbt_semantic_interfaces.protocols import SemanticManifest, SemanticManifestT
 from dbt_semantic_interfaces.validations.agg_time_dimension import (
     AggregationTimeDimensionRule,
 )
 from dbt_semantic_interfaces.validations.dimension_const import DimensionConsistencyRule
 from dbt_semantic_interfaces.validations.element_const import ElementConsistencyRule
-from dbt_semantic_interfaces.validations.entities import (
-    NaturalEntityConfigurationRule,
-    OnePrimaryEntityPerSemanticModelRule,
-)
+from dbt_semantic_interfaces.validations.entities import NaturalEntityConfigurationRule
 from dbt_semantic_interfaces.validations.measures import (
     CountAggregationExprRule,
     MeasureConstraintAliasesRule,
     MeasuresNonAdditiveDimensionRule,
     MetricMeasuresRule,
     PercentileAggregationRule,
     SemanticModelMeasuresUniqueRule,
 )
 from dbt_semantic_interfaces.validations.metrics import (
     CumulativeMetricRule,
     DerivedMetricRule,
+    WhereFiltersAreParseable,
 )
 from dbt_semantic_interfaces.validations.non_empty import NonEmptyRule
+from dbt_semantic_interfaces.validations.primary_entity import PrimaryEntityRule
 from dbt_semantic_interfaces.validations.reserved_keywords import ReservedKeywordsRule
 from dbt_semantic_interfaces.validations.semantic_models import (
     SemanticModelDefaultsRule,
     SemanticModelValidityWindowRule,
 )
-from dbt_semantic_interfaces.validations.unique_valid_name import UniqueAndValidNameRule
+from dbt_semantic_interfaces.validations.unique_valid_name import (
+    PrimaryEntityDimensionPairs,
+    UniqueAndValidNameRule,
+)
 from dbt_semantic_interfaces.validations.validator_helpers import (
     SemanticManifestValidationException,
     SemanticManifestValidationResults,
     SemanticManifestValidationRule,
 )
 
 logger = logging.getLogger(__name__)
@@ -61,24 +63,26 @@
         DerivedMetricRule[SemanticManifestT](),
         CountAggregationExprRule[SemanticManifestT](),
         SemanticModelMeasuresUniqueRule[SemanticManifestT](),
         SemanticModelValidityWindowRule[SemanticManifestT](),
         DimensionConsistencyRule[SemanticManifestT](),
         ElementConsistencyRule[SemanticManifestT](),
         NaturalEntityConfigurationRule[SemanticManifestT](),
-        OnePrimaryEntityPerSemanticModelRule[SemanticManifestT](),
         MeasureConstraintAliasesRule[SemanticManifestT](),
         MetricMeasuresRule[SemanticManifestT](),
         CumulativeMetricRule[SemanticManifestT](),
         NonEmptyRule[SemanticManifestT](),
         UniqueAndValidNameRule[SemanticManifestT](),
         AggregationTimeDimensionRule[SemanticManifestT](),
         ReservedKeywordsRule[SemanticManifestT](),
         MeasuresNonAdditiveDimensionRule[SemanticManifestT](),
         SemanticModelDefaultsRule[SemanticManifestT](),
+        PrimaryEntityRule[SemanticManifestT](),
+        PrimaryEntityDimensionPairs[SemanticManifestT](),
+        WhereFiltersAreParseable[SemanticManifestT](),
     )
 
     def __init__(
         self, rules: Sequence[SemanticManifestValidationRule[SemanticManifestT]] = DEFAULT_RULES, max_workers: int = 1
     ) -> None:
         """Constructor.
 
@@ -91,16 +95,35 @@
             raise ValueError(
                 "SemanticManifestValidator 'rules' must be a sequence with at least one SemanticManifestValidationRule."
             )
 
         self._rules = rules
         self._executor = ProcessPoolExecutor(max_workers=max_workers)
 
-    def validate_semantic_manifest(self, semantic_manifest: SemanticManifestT) -> SemanticManifestValidationResults:
+    def validate_semantic_manifest(
+        self, semantic_manifest: SemanticManifestT, multi_process: bool = False
+    ) -> SemanticManifestValidationResults:
         """Validate a manifest according to configured rules."""
+        if multi_process:
+            return self._validate_multi_process(semantic_manifest=semantic_manifest)
+        else:
+            return self._validate_sync(semantic_manifest=semantic_manifest)
+
+    def _validate_sync(self, semantic_manifest: SemanticManifestT) -> SemanticManifestValidationResults:  # noqa: D
+        results: List[SemanticManifestValidationResults] = []
+
+        for rule in self._rules:
+            issues = rule.validate_manifest(semantic_manifest=semantic_manifest)
+            results.append(SemanticManifestValidationResults.from_issues_sequence(issues))
+
+        return SemanticManifestValidationResults.merge(results)
+
+    def _validate_multi_process(  # noqa: D
+        self, semantic_manifest: SemanticManifestT
+    ) -> SemanticManifestValidationResults:
         results: List[SemanticManifestValidationResults] = []
 
         futures = [
             self._executor.submit(_validate_manifest_with_one_rule, validation_rule, semantic_manifest)
             for validation_rule in self._rules
         ]
         for future in as_completed(futures):
```

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/validations/semantic_models.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/validations/semantic_models.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/validations/unique_valid_name.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/validations/unique_valid_name.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 )
 from dbt_semantic_interfaces.references import (
     ElementReference,
     MetricModelReference,
     SemanticModelElementReference,
     SemanticModelReference,
 )
-from dbt_semantic_interfaces.type_enums import TimeGranularity
+from dbt_semantic_interfaces.type_enums import EntityType, TimeGranularity
 from dbt_semantic_interfaces.validations.validator_helpers import (
     FileContext,
     MetricContext,
     SemanticManifestValidationRule,
     SemanticModelContext,
     SemanticModelElementContext,
     SemanticModelElementType,
@@ -224,7 +224,72 @@
         issues = []
         issues += UniqueAndValidNameRule._validate_top_level_objects(semantic_manifest=semantic_manifest)
 
         for semantic_model in semantic_manifest.semantic_models:
             issues += UniqueAndValidNameRule._validate_semantic_model_elements(semantic_model=semantic_model)
 
         return issues
+
+
+class PrimaryEntityDimensionPairs(SemanticManifestValidationRule[SemanticManifestT], Generic[SemanticManifestT]):
+    """All dimension + primary entity pairs across the semantic manifest are unique."""
+
+    @staticmethod
+    @validate_safely(
+        whats_being_done="validating the semantic model doesn't have dimension + primary entity pair conflicts"
+    )
+    def _check_semantic_model(  # noqa: D
+        semantic_model: SemanticModel, known_pairings: Dict[str, Dict[str, str]]
+    ) -> Sequence[ValidationIssue]:
+        issues: List[ValidationIssue] = []
+
+        primary_entity = semantic_model.primary_entity
+        if primary_entity is None:
+            for entity in semantic_model.entities:
+                if entity.type is EntityType.PRIMARY:
+                    primary_entity = entity.name
+                    break
+
+        # If primary entity is still none, return early. It's an issue,
+        # but not the subject of this validation. This is handled by
+        # PrimaryEntityRule
+        if primary_entity is None:
+            return issues
+
+        safe = False
+        if known_pairings.get(primary_entity) is None:
+            known_pairings[primary_entity] = {}
+            safe = True
+
+        for dimension in semantic_model.dimensions:
+            if safe or known_pairings[primary_entity].get(dimension.name) is None:
+                known_pairings[primary_entity][dimension.name] = semantic_model.name
+            else:
+                issues.append(
+                    ValidationError(
+                        context=SemanticModelElementContext(
+                            file_context=FileContext.from_metadata(metadata=semantic_model.metadata),
+                            semantic_model_element=SemanticModelElementReference(
+                                semantic_model_name=semantic_model.name, element_name=dimension.name
+                            ),
+                            element_type=SemanticModelElementType.DIMENSION,
+                        ),
+                        message="Duplicate dimension + primary entity pairing detected, dimension + primary entity "
+                        f"pairings must be unique. Semantic model `{semantic_model.name}` has a primary entity of "
+                        f"`{primary_entity}` and dimension `{dimension.name}`, but this pairing is already in use on "
+                        f"semantic model `{known_pairings[primary_entity][dimension.name]}`.",
+                    )
+                )
+
+        return issues
+
+    @staticmethod
+    @validate_safely(whats_being_done="validating there are no duplicate dimension primary entity pairs")
+    def validate_manifest(semantic_manifest: SemanticManifestT) -> Sequence[ValidationIssue]:  # noqa: D
+        issues = []
+        known_pairings: Dict[str, Dict[str, str]] = {}
+        for semantic_model in semantic_manifest.semantic_models:
+            issues += PrimaryEntityDimensionPairs._check_semantic_model(
+                semantic_model=semantic_model, known_pairings=known_pairings
+            )
+
+        return issues
```

### Comparing `dbt_semantic_interfaces-0.1.0rc1/dbt_semantic_interfaces/validations/validator_helpers.py` & `dbt_semantic_interfaces-0.2.0/dbt_semantic_interfaces/validations/validator_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -336,15 +336,15 @@
 
     if "stacktrace" not in extras:
         extras["stacktrace"] = "".join(traceback.format_tb(e.__traceback__))
 
     return ValidationError(
         context=context,
         message=f"An error occurred while {what_was_being_done} - "
-        f"{''.join(traceback.format_exception_only(etype=type(e), value=e))}",
+        f"{''.join(traceback.format_exception_only(type(e), value=e))}",
         extra_detail="\n".join([f"{key}: {value}" for key, value in extras.items()]),
     )
 
 
 def _func_args_to_string(*args: Any, **kwargs: Any) -> str:  # type: ignore
     return f"positional args: {args}, key word args: {kwargs}"
```

### Comparing `dbt_semantic_interfaces-0.1.0rc1/venv-3.9.16/bin/Activate.ps1` & `dbt_semantic_interfaces-0.2.0/venv-3.9.16/bin/Activate.ps1`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/venv-3.9.16/bin/activate` & `dbt_semantic_interfaces-0.2.0/venv-3.9.16/bin/activate`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/venv-3.9.16/bin/activate.csh` & `dbt_semantic_interfaces-0.2.0/venv-3.9.16/bin/activate.csh`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/venv-3.9.16/bin/activate.fish` & `dbt_semantic_interfaces-0.2.0/venv-3.9.16/bin/activate.fish`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/.gitignore` & `dbt_semantic_interfaces-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/LICENSE` & `dbt_semantic_interfaces-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/README.md` & `dbt_semantic_interfaces-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0rc1/pyproject.toml` & `dbt_semantic_interfaces-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dbt-semantic-interfaces"
-version = "0.1.0rc1"
+version = "0.2.0"
 description = 'The shared semantic layer definitions that dbt-core and MetricFlow use'
 readme = "README.md"
 requires-python = ">=3.8"
 license = "Apache-2.0"
 keywords = []
 authors = [
   { name = "dbt Labs", email = "info@dbtlabs.com" },
```

### Comparing `dbt_semantic_interfaces-0.1.0rc1/PKG-INFO` & `dbt_semantic_interfaces-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-semantic-interfaces
-Version: 0.1.0rc1
+Version: 0.2.0
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
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: dbt-semantic-interfaces Version: 0.1.0rc1 Summary:
-The shared semantic layer definitions that dbt-core and MetricFlow use Author-
+Metadata-Version: 2.1 Name: dbt-semantic-interfaces Version: 0.2.0 Summary: The
+shared semantic layer definitions that dbt-core and MetricFlow use Author-
 email: dbt Labs
 dbtlabs.com> License-Expression: Apache-2.0 License-File: LICENSE Classifier:
 Development Status :: 4 - Beta Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: Implementation :: CPython Classifier: Programming
```

