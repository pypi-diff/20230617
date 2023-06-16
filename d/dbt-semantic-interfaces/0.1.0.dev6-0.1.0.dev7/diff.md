# Comparing `tmp/dbt_semantic_interfaces-0.1.0.dev6.tar.gz` & `tmp/dbt_semantic_interfaces-0.1.0.dev7.tar.gz`

## Comparing `dbt_semantic_interfaces-0.1.0.dev6.tar` & `dbt_semantic_interfaces-0.1.0.dev7.tar`

### file list

```diff
@@ -1,79 +1,99 @@
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/CHANGELOG.md
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/Makefile
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/mypy.ini
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/__init__.py
--rw-r--r--   0        0        0    18186 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/dataclass_serialization.py
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/enum_extension.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/errors.py
--rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/pretty_print.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/py.typed
--rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/references.py
--rw-r--r--   0        0        0     6161 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/implementations/__init__.py
--rw-r--r--   0        0        0     7622 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/implementations/base.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/implementations/metadata.py
--rw-r--r--   0        0        0     7429 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/implementations/metric.py
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/implementations/semantic_manifest.py
--rw-r--r--   0        0        0     6442 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/implementations/semantic_model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/implementations/elements/__init__.py
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/implementations/elements/dimension.py
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/implementations/elements/entity.py
--rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/implementations/elements/measure.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/implementations/filters/__init__.py
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/implementations/filters/call_parameter_sets.py
--rw-r--r--   0        0        0     5056 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/implementations/filters/where_filter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/parsing/__init__.py
--rw-r--r--   0        0        0    14122 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/parsing/dir_to_model.py
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/parsing/explicit_schema.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/parsing/objects.py
--rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/parsing/schema_validator.py
--rw-r--r--   0        0        0     9628 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/parsing/schemas.py
--rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/parsing/yaml_loader.py
--rw-r--r--   0        0        0    14950 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/parsing/schemas/default_explicit_schema.json
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/protocols/__init__.py
--rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/protocols/dimension.py
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/protocols/entity.py
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/protocols/measure.py
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/protocols/metadata.py
--rw-r--r--   0        0        0     5361 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/protocols/metric.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/protocols/protocol_hint.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/protocols/semantic_manifest.py
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/protocols/semantic_model.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/protocols/where_filter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/transformations/__init__.py
--rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/transformations/add_input_metric_measures.py
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/transformations/agg_time_dimension.py
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/transformations/boolean_measure.py
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/transformations/convert_count.py
--rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/transformations/convert_median.py
--rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/transformations/names.py
--rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/transformations/proxy_measure.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/transformations/pydantic_rule_set.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/transformations/rule_set.py
--rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/transformations/semantic_manifest_transformer.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/transformations/transform_rule.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/type_enums/__init__.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/type_enums/aggregation_type.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/type_enums/dimension_type.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/type_enums/entity_type.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/type_enums/metric_type.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/type_enums/time_granularity.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/__init__.py
--rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/agg_time_dimension.py
--rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/common_entities.py
--rw-r--r--   0        0        0     7487 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/dimension_const.py
--rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/element_const.py
--rw-r--r--   0        0        0     5017 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/entities.py
--rw-r--r--   0        0        0    28360 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/measures.py
--rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/metrics.py
--rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/non_empty.py
--rw-r--r--   0        0        0     6753 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/reserved_keywords.py
--rw-r--r--   0        0        0     5233 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/semantic_manifest_validator.py
--rw-r--r--   0        0        0    10920 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/semantic_models.py
--rw-r--r--   0        0        0     9960 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/unique_valid_name.py
--rw-r--r--   0        0        0    15060 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/validator_helpers.py
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/LICENSE
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/README.md
--rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/pyproject.toml
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev6/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/.tool-versions
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/CHANGELOG.md
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/Makefile
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/mypy.ini
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/__init__.py
+-rw-r--r--   0        0        0    18186 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/dataclass_serialization.py
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/enum_extension.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/errors.py
+-rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/pretty_print.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/py.typed
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/references.py
+-rw-r--r--   0        0        0     6161 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/implementations/__init__.py
+-rw-r--r--   0        0        0     7622 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/implementations/base.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/implementations/metadata.py
+-rw-r--r--   0        0        0     7699 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/implementations/metric.py
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/implementations/semantic_manifest.py
+-rw-r--r--   0        0        0     6442 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/implementations/semantic_model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/implementations/elements/__init__.py
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/implementations/elements/dimension.py
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/implementations/elements/entity.py
+-rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/implementations/elements/measure.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/implementations/filters/__init__.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/implementations/filters/call_parameter_sets.py
+-rw-r--r--   0        0        0     5056 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/implementations/filters/where_filter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/parsing/__init__.py
+-rw-r--r--   0        0        0    14122 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/parsing/dir_to_model.py
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/parsing/explicit_schema.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/parsing/objects.py
+-rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/parsing/schema_validator.py
+-rw-r--r--   0        0        0     9504 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/parsing/schemas.py
+-rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/parsing/yaml_loader.py
+-rw-r--r--   0        0        0    14735 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/parsing/schemas/default_explicit_schema.json
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/protocols/__init__.py
+-rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/protocols/dimension.py
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/protocols/entity.py
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/protocols/measure.py
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/protocols/metadata.py
+-rw-r--r--   0        0        0     5164 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/protocols/metric.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/protocols/protocol_hint.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/protocols/semantic_manifest.py
+-rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/protocols/semantic_model.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/protocols/where_filter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/transformations/__init__.py
+-rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/transformations/add_input_metric_measures.py
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/transformations/agg_time_dimension.py
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/transformations/boolean_measure.py
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/transformations/convert_count.py
+-rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/transformations/convert_median.py
+-rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/transformations/names.py
+-rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/transformations/proxy_measure.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/transformations/pydantic_rule_set.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/transformations/rule_set.py
+-rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/transformations/semantic_manifest_transformer.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/transformations/transform_rule.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/type_enums/__init__.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/type_enums/aggregation_type.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/type_enums/dimension_type.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/type_enums/entity_type.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/type_enums/metric_type.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/type_enums/time_granularity.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/__init__.py
+-rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/agg_time_dimension.py
+-rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/common_entities.py
+-rw-r--r--   0        0        0     7487 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/dimension_const.py
+-rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/element_const.py
+-rw-r--r--   0        0        0     5017 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/entities.py
+-rw-r--r--   0        0        0    28360 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/measures.py
+-rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/metrics.py
+-rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/non_empty.py
+-rw-r--r--   0        0        0     6753 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/reserved_keywords.py
+-rw-r--r--   0        0        0     5233 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/semantic_manifest_validator.py
+-rw-r--r--   0        0        0    10920 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/semantic_models.py
+-rw-r--r--   0        0        0     9960 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/unique_valid_name.py
+-rw-r--r--   0        0        0    15060 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/validator_helpers.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/venv-3.9.16/pyvenv.cfg
+-rw-r--r--   0        0        0     8834 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/venv-3.9.16/bin/Activate.ps1
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/venv-3.9.16/bin/activate
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/venv-3.9.16/bin/activate.csh
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/venv-3.9.16/bin/activate.fish
+-rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/venv-3.9.16/bin/hatch
+-rwxr-xr-x   0        0        0      293 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/venv-3.9.16/bin/hatchling
+-rwxr-xr-x   0        0        0      275 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/venv-3.9.16/bin/httpx
+-rwxr-xr-x   0        0        0      281 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/venv-3.9.16/bin/keyring
+-rwxr-xr-x   0        0        0      291 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/venv-3.9.16/bin/markdown-it
+-rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/venv-3.9.16/bin/pip
+-rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/venv-3.9.16/bin/pip3
+-rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/venv-3.9.16/bin/pip3.9
+-rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/venv-3.9.16/bin/pygmentize
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/venv-3.9.16/bin/python -> /Users/quigleymalcolm/.asdf/installs/python/3.9.16/bin/python
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/venv-3.9.16/bin/python3 -> python
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/venv-3.9.16/bin/python3.9 -> python
+-rwxr-xr-x   0        0        0      290 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/venv-3.9.16/bin/userpath
+-rwxr-xr-x   0        0        0      309 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/venv-3.9.16/bin/virtualenv
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/LICENSE
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/README.md
+-rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/pyproject.toml
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/PKG-INFO
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/Makefile` & `dbt_semantic_interfaces-0.1.0.dev7/Makefile`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/dataclass_serialization.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/dataclass_serialization.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/enum_extension.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/enum_extension.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/errors.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/errors.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/pretty_print.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/pretty_print.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/references.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/references.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/test_utils.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/test_utils.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/implementations/base.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/implementations/base.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/implementations/metric.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/implementations/metric.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from __future__ import annotations
 
-from typing import List, Optional
+from typing import List, Optional, Sequence
 
+from pydantic import Field
+
+from dbt_semantic_interfaces.enum_extension import assert_values_exhausted
 from dbt_semantic_interfaces.errors import ParsingException
 from dbt_semantic_interfaces.implementations.base import (
     HashableBaseModel,
     ModelWithMetadataParsing,
     PydanticCustomInputParser,
     PydanticParseableValueType,
 )
@@ -119,64 +122,62 @@
     offset_to_grain: Optional[TimeGranularity]
 
     @property
     def as_reference(self) -> MetricReference:
         """Property accessor to get the MetricReference associated with this metric input."""
         return MetricReference(element_name=self.name)
 
+    @property
+    def post_aggregation_reference(self) -> MetricReference:
+        """Property accessor to get the MetricReference with the aliased name, if appropriate."""
+        return MetricReference(element_name=self.alias or self.name)
+
 
 class PydanticMetricTypeParams(HashableBaseModel):
     """Type params add additional context to certain metric types (the context depends on the metric type)."""
 
     measure: Optional[PydanticMetricInputMeasure]
-    measures: Optional[List[PydanticMetricInputMeasure]]
-    numerator: Optional[PydanticMetricInputMeasure]
-    denominator: Optional[PydanticMetricInputMeasure]
+    numerator: Optional[PydanticMetricInput]
+    denominator: Optional[PydanticMetricInput]
     expr: Optional[str]
     window: Optional[PydanticMetricTimeWindow]
     grain_to_date: Optional[TimeGranularity]
     metrics: Optional[List[PydanticMetricInput]]
 
-    @property
-    def numerator_measure_reference(self) -> Optional[MeasureReference]:
-        """Return the measure reference, if any, associated with the metric input measure defined as the numerator."""
-        return self.numerator.measure_reference if self.numerator else None
-
-    @property
-    def denominator_measure_reference(self) -> Optional[MeasureReference]:
-        """Return the measure reference, if any, associated with the metric input measure defined as the denominator."""
-        return self.denominator.measure_reference if self.denominator else None
+    input_measures: List[PydanticMetricInputMeasure] = Field(default_factory=list)
 
 
 class PydanticMetric(HashableBaseModel, ModelWithMetadataParsing):
     """Describes a metric."""
 
     name: str
     description: Optional[str]
     type: MetricType
     type_params: PydanticMetricTypeParams
     filter: Optional[PydanticWhereFilter]
     metadata: Optional[PydanticMetadata]
 
     @property
-    def input_measures(self) -> List[PydanticMetricInputMeasure]:
+    def input_measures(self) -> Sequence[PydanticMetricInputMeasure]:
         """Return the complete list of input measure configurations for this metric."""
-        tp = self.type_params
-        res = tp.measures or []
-        if tp.measure:
-            res.append(tp.measure)
-        if tp.numerator:
-            res.append(tp.numerator)
-        if tp.denominator:
-            res.append(tp.denominator)
-
-        return res
+        return self.type_params.input_measures
 
     @property
     def measure_references(self) -> List[MeasureReference]:
         """Return the measure references associated with all input measure configurations for this metric."""
         return [x.measure_reference for x in self.input_measures]
 
     @property
-    def input_metrics(self) -> List[PydanticMetricInput]:
+    def input_metrics(self) -> Sequence[PydanticMetricInput]:
         """Return the associated input metrics for this metric."""
-        return self.type_params.metrics or []
+        if self.type is MetricType.SIMPLE or self.type is MetricType.CUMULATIVE:
+            return ()
+        elif self.type is MetricType.DERIVED:
+            assert self.type_params.metrics is not None, f"{MetricType.DERIVED} should have type_params.metrics set"
+            return self.type_params.metrics
+        elif self.type is MetricType.RATIO:
+            assert (
+                self.type_params.numerator is not None and self.type_params.denominator is not None
+            ), f"{self} is metric type {MetricType.RATIO}, so neither the numerator and denominator should not be None"
+            return (self.type_params.numerator, self.type_params.denominator)
+        else:
+            assert_values_exhausted(self.type)
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/implementations/semantic_manifest.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/implementations/semantic_manifest.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/implementations/semantic_model.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/implementations/semantic_model.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/implementations/elements/dimension.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/implementations/elements/dimension.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/implementations/elements/entity.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/implementations/elements/entity.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/implementations/elements/measure.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/implementations/elements/measure.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/implementations/filters/call_parameter_sets.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/implementations/filters/call_parameter_sets.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/implementations/filters/where_filter.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/implementations/filters/where_filter.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/parsing/dir_to_model.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/parsing/dir_to_model.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/parsing/explicit_schema.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/parsing/explicit_schema.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/parsing/objects.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/parsing/objects.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/parsing/schema_validator.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/parsing/schema_validator.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/parsing/schemas.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/parsing/schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,18 +68,14 @@
 metric_type_params_schema = {
     "$id": "metric_type_params",
     "type": "object",
     "properties": {
         "numerator": {"$ref": "metric_input_measure_schema"},
         "denominator": {"$ref": "metric_input_measure_schema"},
         "measure": {"$ref": "metric_input_measure_schema"},
-        "measures": {
-            "type": "array",
-            "items": {"$ref": "metric_input_measure_schema"},
-        },
         "expr": {"type": ["string", "boolean"]},
         "window": {"type": "string"},
         "grain_to_date": {"type": "string"},
         "metrics": {
             "type": "array",
             "items": {"$ref": "metric_input_schema"},
         },
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/parsing/yaml_loader.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/parsing/yaml_loader.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/parsing/schemas/default_explicit_schema.json` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/parsing/schemas/default_explicit_schema.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999951171875%*

 * *Differences: {"'definitions'": "{'metric_type_params': {'properties': {delete: ['measures']}}}"}*

```diff
@@ -335,20 +335,14 @@
                 },
                 "grain_to_date": {
                     "type": "string"
                 },
                 "measure": {
                     "$ref": "#/definitions/metric_input_measure_schema"
                 },
-                "measures": {
-                    "items": {
-                        "$ref": "#/definitions/metric_input_measure_schema"
-                    },
-                    "type": "array"
-                },
                 "metrics": {
                     "items": {
                         "$ref": "#/definitions/metric_input_schema"
                     },
                     "type": "array"
                 },
                 "numerator": {
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/protocols/__init__.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/protocols/dimension.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/protocols/dimension.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/protocols/entity.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/protocols/entity.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/protocols/measure.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/protocols/measure.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/protocols/metadata.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/protocols/metadata.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/protocols/metric.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/protocols/metric.py`

 * *Files 10% similar despite different names*

```diff
@@ -88,36 +88,43 @@
 
     @property
     @abstractmethod
     def as_reference(self) -> MetricReference:
         """Property accessor to get the MetricReference associated with this metric input."""
         ...
 
+    @property
+    @abstractmethod
+    def post_aggregation_reference(self) -> MetricReference:
+        """Property accessor to get the MetricReference with the aliased name, if appropriate."""
+        pass
+
 
 class MetricTypeParams(Protocol):
     """Type params add additional context to certain metric types (the context depends on the metric type)."""
 
     @property
     @abstractmethod
     def measure(self) -> Optional[MetricInputMeasure]:  # noqa: D
         pass
 
     @property
     @abstractmethod
-    def measures(self) -> Optional[Sequence[MetricInputMeasure]]:  # noqa: D
+    def input_measures(self) -> Sequence[MetricInputMeasure]:
+        """Return measures needed to compute this metric (including measures needed by parent metrics)."""
         pass
 
     @property
     @abstractmethod
-    def numerator(self) -> Optional[MetricInputMeasure]:  # noqa: D
+    def numerator(self) -> Optional[MetricInput]:  # noqa: D
         pass
 
     @property
     @abstractmethod
-    def denominator(self) -> Optional[MetricInputMeasure]:  # noqa: D
+    def denominator(self) -> Optional[MetricInput]:  # noqa: D
         pass
 
     @property
     @abstractmethod
     def expr(self) -> Optional[str]:  # noqa: D
         pass
 
@@ -132,26 +139,14 @@
         pass
 
     @property
     @abstractmethod
     def metrics(self) -> Optional[Sequence[MetricInput]]:  # noqa: D
         pass
 
-    @property
-    @abstractmethod
-    def numerator_measure_reference(self) -> Optional[MeasureReference]:
-        """Return the measure reference, if any, associated with the metric input measure defined as the numerator."""
-        ...
-
-    @property
-    @abstractmethod
-    def denominator_measure_reference(self) -> Optional[MeasureReference]:
-        """Return the measure reference, if any, associated with the metric input measure defined as the denominator."""
-        ...
-
 
 class Metric(Protocol):
     """Describes a metric."""
 
     @property
     @abstractmethod
     def name(self) -> str:  # noqa: D
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/protocols/protocol_hint.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/protocols/protocol_hint.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/protocols/semantic_manifest.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/protocols/semantic_manifest.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/protocols/semantic_model.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/protocols/semantic_model.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/transformations/agg_time_dimension.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/transformations/agg_time_dimension.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/transformations/boolean_measure.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/transformations/boolean_measure.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/transformations/convert_count.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/transformations/convert_count.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/transformations/convert_median.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/transformations/convert_median.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/transformations/names.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/transformations/names.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/transformations/proxy_measure.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/transformations/proxy_measure.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,14 +54,14 @@
 
                 if add_metric is True:
                     semantic_manifest.metrics.append(
                         PydanticMetric(
                             name=measure.name,
                             type=MetricType.SIMPLE,
                             type_params=PydanticMetricTypeParams(
-                                measures=[PydanticMetricInputMeasure(name=measure.name)],
+                                measure=PydanticMetricInputMeasure(name=measure.name),
                                 expr=measure.name,
                             ),
                         )
                     )
 
         return semantic_manifest
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/transformations/pydantic_rule_set.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/transformations/pydantic_rule_set.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/transformations/rule_set.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/transformations/rule_set.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/transformations/semantic_manifest_transformer.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/transformations/semantic_manifest_transformer.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/transformations/transform_rule.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/transformations/transform_rule.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/type_enums/time_granularity.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/type_enums/time_granularity.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/agg_time_dimension.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/agg_time_dimension.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/common_entities.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/common_entities.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/dimension_const.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/dimension_const.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/element_const.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/element_const.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/entities.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/entities.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/measures.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/measures.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/metrics.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/metrics.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/non_empty.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/non_empty.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/reserved_keywords.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/reserved_keywords.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/semantic_manifest_validator.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/semantic_manifest_validator.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/semantic_models.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/semantic_models.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/unique_valid_name.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/unique_valid_name.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/dbt_semantic_interfaces/validations/validator_helpers.py` & `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/validator_helpers.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/.gitignore` & `dbt_semantic_interfaces-0.1.0.dev7/.gitignore`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/LICENSE` & `dbt_semantic_interfaces-0.1.0.dev7/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/README.md` & `dbt_semantic_interfaces-0.1.0.dev7/README.md`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/pyproject.toml` & `dbt_semantic_interfaces-0.1.0.dev7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dbt-semantic-interfaces"
-version = "0.1.0.dev6"
+version = "0.1.0.dev7"
 description = 'The shared semantic layer definitions that dbt-core and MetricFlow use'
 readme = "README.md"
 requires-python = ">=3.8"
 license = "Apache-2.0"
 keywords = []
 authors = [
   { name = "dbt Labs", email = "info@dbtlabs.com" },
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev6/PKG-INFO` & `dbt_semantic_interfaces-0.1.0.dev7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-semantic-interfaces
-Version: 0.1.0.dev6
+Version: 0.1.0.dev7
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
-Metadata-Version: 2.1 Name: dbt-semantic-interfaces Version: 0.1.0.dev6
+Metadata-Version: 2.1 Name: dbt-semantic-interfaces Version: 0.1.0.dev7
 Summary: The shared semantic layer definitions that dbt-core and MetricFlow use
 Author-email: dbt Labs
 dbtlabs.com> License-Expression: Apache-2.0 License-File: LICENSE Classifier:
 Development Status :: 4 - Beta Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
```

