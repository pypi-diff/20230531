# Comparing `tmp/dbt_semantic_interfaces-0.1.0.dev1.tar.gz` & `tmp/dbt_semantic_interfaces-0.1.0.dev2.tar.gz`

## Comparing `dbt_semantic_interfaces-0.1.0.dev1.tar` & `dbt_semantic_interfaces-0.1.0.dev2.tar`

### file list

```diff
@@ -1,168 +1,99 @@
--rw-r--r--   0        0        0     5669 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.changie.yaml
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.pre-commit-config.yaml
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.tool-versions
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/CHANGELOG.md
--rw-r--r--   0        0        0     4067 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/CONTRIBUTING.md
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/Makefile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.changes/0.0.0.md
--rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.changes/README.md
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.changes/header.tpl.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.changes/unreleased/.gitkeep
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.changes/unreleased/Features-20230515-155013.yaml
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.changes/unreleased/Features-20230515-161320.yaml
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.changes/unreleased/Features-20230516-100539.yaml
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.changes/unreleased/Features-20230516-112250.yaml
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.changes/unreleased/Features-20230516-150352.yaml
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.changes/unreleased/Features-20230516-162909.yaml
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.changes/unreleased/Fixes-20230516-172635.yaml
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.changes/unreleased/Fixes-20230516-175643.yaml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.changes/unreleased/Under the Hood-20230424-152251.yaml
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.changes/unreleased/Under the Hood-20230501-154838.yaml
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.changes/unreleased/Under the Hood-20230501-162818.yaml
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.changes/unreleased/Under the Hood-20230501-164142.yaml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.changes/unreleased/Under the Hood-20230505-120359.yaml
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.changes/unreleased/Under the Hood-20230515-124059.yaml
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.changes/unreleased/Under the Hood-20230515-125335.yaml
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.github/pull_request_template.md
--rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.github/ISSUE_TEMPLATE/feature-request.yml
--rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.github/ISSUE_TEMPLATE/regression-report.yml
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.github/actions/setup-python-env/action.yml
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.github/workflows/bot-changelog.yml
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.github/workflows/changelog-existence.yml
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.github/workflows/ci-pre-commit.yaml
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.github/workflows/ci-pytest.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/__init__.py
--rw-r--r--   0        0        0    17431 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/dataclass_serialization.py
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/enum_extension.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/errors.py
--rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/model_transformer.py
--rw-r--r--   0        0        0     4016 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/model_validator.py
--rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/pretty_print.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/py.typed
--rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/references.py
--rw-r--r--   0        0        0     5744 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/objects/__init__.py
--rw-r--r--   0        0        0     7229 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/objects/base.py
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/objects/metadata.py
--rw-r--r--   0        0        0     7399 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/objects/metric.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/objects/semantic_manifest.py
--rw-r--r--   0        0        0     5699 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/objects/semantic_model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/objects/elements/__init__.py
--rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/objects/elements/dimension.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/objects/elements/entity.py
--rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/objects/elements/measure.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/objects/filters/__init__.py
--rw-r--r--   0        0        0     5443 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/objects/filters/call_parameter_sets.py
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/objects/filters/where_filter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/parsing/__init__.py
--rw-r--r--   0        0        0    13546 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/parsing/dir_to_model.py
--rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/parsing/explicit_schema.py
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/parsing/objects.py
--rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/parsing/schema_validator.py
--rw-r--r--   0        0        0     9300 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/parsing/schemas.py
--rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/parsing/yaml_loader.py
--rw-r--r--   0        0        0    14653 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/parsing/schemas/metricflow.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/protocols/__init__.py
--rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/protocols/dimension.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/protocols/entity.py
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/protocols/measure.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/protocols/metadata.py
--rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/protocols/metric.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/protocols/semantic_manifest.py
--rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/protocols/semantic_model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/transformations/__init__.py
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/transformations/add_input_metric_measures.py
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/transformations/agg_time_dimension.py
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/transformations/boolean_measure.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/transformations/convert_count.py
--rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/transformations/convert_median.py
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/transformations/names.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/transformations/proxy_measure.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/transformations/transform_rule.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/type_enums/__init__.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/type_enums/aggregation_type.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/type_enums/dimension_type.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/type_enums/entity_type.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/type_enums/metric_type.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/type_enums/time_granularity.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/validations/__init__.py
--rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/validations/agg_time_dimension.py
--rw-r--r--   0        0        0     3757 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/validations/common_entities.py
--rw-r--r--   0        0        0     7732 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/validations/dimension_const.py
--rw-r--r--   0        0        0     3889 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/validations/element_const.py
--rw-r--r--   0        0        0     4886 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/validations/entities.py
--rw-r--r--   0        0        0    27760 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/validations/measures.py
--rw-r--r--   0        0        0     6942 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/validations/metrics.py
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/validations/non_empty.py
--rw-r--r--   0        0        0     6649 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/validations/reserved_keywords.py
--rw-r--r--   0        0        0    10060 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/validations/semantic_models.py
--rw-r--r--   0        0        0     9811 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/validations/unique_valid_name.py
--rw-r--r--   0        0        0    13769 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/validations/validator_helpers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/__init__.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/conftest.py
--rw-r--r--   0        0        0     7796 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/test_dataclass_serialization.py
--rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/test_implements_satisfy_protocols.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/test_pretty_print.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/fixtures/__init__.py
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/fixtures/model_fixtures.py
--rw-r--r--   0        0        0    13041 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/fixtures/model_yamls/simple_model/metrics.yaml
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/fixtures/model_yamls/simple_model/semantic_models/accounts_source.yaml
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/fixtures/model_yamls/simple_model/semantic_models/bookings_source.yaml
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/fixtures/model_yamls/simple_model/semantic_models/companies.yaml
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/fixtures/model_yamls/simple_model/semantic_models/id_verifications.yaml
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/fixtures/model_yamls/simple_model/semantic_models/listings_latest.yaml
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/fixtures/model_yamls/simple_model/semantic_models/lux_listing_mapping.yaml
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/fixtures/model_yamls/simple_model/semantic_models/revenue.yaml
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/fixtures/model_yamls/simple_model/semantic_models/user_sm_source.yaml
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/fixtures/model_yamls/simple_model/semantic_models/users_latest.yaml
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/fixtures/model_yamls/simple_model/semantic_models/views_source.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/objects/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/objects/where_filter/__init__.py
--rw-r--r--   0        0        0     2801 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/objects/where_filter/test_parse_calls.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/parsing/__init__.py
--rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/parsing/test_metadata_parsing.py
--rw-r--r--   0        0        0    16598 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/parsing/test_metric_parsing.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/parsing/test_model_deserialization.py
--rw-r--r--   0        0        0    14869 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/parsing/test_semantic_model_parsing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/transformations/__init__.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/transformations/test_configurable_transform_rules.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/validations/__init__.py
--rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/validations/test_agg_time_dimension.py
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/validations/test_common_entities.py
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/validations/test_configurable_rules.py
--rw-r--r--   0        0        0     7407 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/validations/test_dimension_const.py
--rw-r--r--   0        0        0     3655 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/validations/test_element_const.py
--rw-r--r--   0        0        0     4436 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/validations/test_entities.py
--rw-r--r--   0        0        0    25297 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/validations/test_measures.py
--rw-r--r--   0        0        0    11019 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/validations/test_metrics.py
--rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/validations/test_reserved_keywords.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/validations/test_semantic_models.py
--rw-r--r--   0        0        0     7603 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/validations/test_unique_valid_name.py
--rw-r--r--   0        0        0     5818 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/validations/test_validator_helpers.py
--rw-r--r--   0        0        0    14533 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/validations/test_validity_param_definitions.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/venv-3.9.16/pyvenv.cfg
--rw-r--r--   0        0        0     8834 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/venv-3.9.16/bin/Activate.ps1
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/venv-3.9.16/bin/activate
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/venv-3.9.16/bin/activate.csh
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/venv-3.9.16/bin/activate.fish
--rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/venv-3.9.16/bin/hatch
--rwxr-xr-x   0        0        0      293 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/venv-3.9.16/bin/hatchling
--rwxr-xr-x   0        0        0      275 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/venv-3.9.16/bin/httpx
--rwxr-xr-x   0        0        0      281 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/venv-3.9.16/bin/keyring
--rwxr-xr-x   0        0        0      291 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/venv-3.9.16/bin/markdown-it
--rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/venv-3.9.16/bin/pip
--rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/venv-3.9.16/bin/pip3
--rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/venv-3.9.16/bin/pip3.9
--rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/venv-3.9.16/bin/pygmentize
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/venv-3.9.16/bin/python -> /Users/quigleymalcolm/.asdf/installs/python/3.9.16/bin/python
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/venv-3.9.16/bin/python3 -> python
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/venv-3.9.16/bin/python3.9 -> python
--rwxr-xr-x   0        0        0      290 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/venv-3.9.16/bin/userpath
--rwxr-xr-x   0        0        0      309 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/venv-3.9.16/bin/virtualenv
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/LICENSE
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/README.md
--rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/pyproject.toml
--rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/.tool-versions
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/CHANGELOG.md
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/Makefile
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/mypy.ini
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/__init__.py
+-rw-r--r--   0        0        0    18186 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/dataclass_serialization.py
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/enum_extension.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/errors.py
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/model_transformer.py
+-rw-r--r--   0        0        0     5126 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/model_validator.py
+-rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/pretty_print.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/py.typed
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/references.py
+-rw-r--r--   0        0        0     6119 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/implementations/__init__.py
+-rw-r--r--   0        0        0     7622 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/implementations/base.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/implementations/metadata.py
+-rw-r--r--   0        0        0     7556 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/implementations/metric.py
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/implementations/semantic_manifest.py
+-rw-r--r--   0        0        0     6502 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/implementations/semantic_model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/implementations/elements/__init__.py
+-rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/implementations/elements/dimension.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/implementations/elements/entity.py
+-rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/implementations/elements/measure.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/implementations/filters/__init__.py
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/implementations/filters/call_parameter_sets.py
+-rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/implementations/filters/where_filter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/parsing/__init__.py
+-rw-r--r--   0        0        0    13861 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/parsing/dir_to_model.py
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/parsing/explicit_schema.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/parsing/objects.py
+-rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/parsing/schema_validator.py
+-rw-r--r--   0        0        0     9628 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/parsing/schemas.py
+-rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/parsing/yaml_loader.py
+-rw-r--r--   0        0        0    14950 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/parsing/schemas/default_explicit_schema.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/protocols/__init__.py
+-rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/protocols/dimension.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/protocols/entity.py
+-rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/protocols/measure.py
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/protocols/metadata.py
+-rw-r--r--   0        0        0     5436 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/protocols/metric.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/protocols/protocol_hint.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/protocols/semantic_manifest.py
+-rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/protocols/semantic_model.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/protocols/where_filter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/transformations/__init__.py
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/transformations/add_input_metric_measures.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/transformations/agg_time_dimension.py
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/transformations/boolean_measure.py
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/transformations/convert_count.py
+-rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/transformations/convert_median.py
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/transformations/names.py
+-rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/transformations/proxy_measure.py
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/transformations/pydantic_rule_set.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/transformations/rule_set.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/transformations/transform_rule.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/type_enums/__init__.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/type_enums/aggregation_type.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/type_enums/dimension_type.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/type_enums/entity_type.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/type_enums/metric_type.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/type_enums/time_granularity.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/validations/__init__.py
+-rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/validations/agg_time_dimension.py
+-rw-r--r--   0        0        0     3891 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/validations/common_entities.py
+-rw-r--r--   0        0        0     7681 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/validations/dimension_const.py
+-rw-r--r--   0        0        0     4131 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/validations/element_const.py
+-rw-r--r--   0        0        0     5107 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/validations/entities.py
+-rw-r--r--   0        0        0    28444 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/validations/measures.py
+-rw-r--r--   0        0        0     7432 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/validations/metrics.py
+-rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/validations/non_empty.py
+-rw-r--r--   0        0        0     6791 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/validations/reserved_keywords.py
+-rw-r--r--   0        0        0     9051 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/validations/semantic_models.py
+-rw-r--r--   0        0        0     9979 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/validations/unique_valid_name.py
+-rw-r--r--   0        0        0    14682 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/validations/validator_helpers.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/venv-3.9.16/pyvenv.cfg
+-rw-r--r--   0        0        0     8834 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/venv-3.9.16/bin/Activate.ps1
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/venv-3.9.16/bin/activate
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/venv-3.9.16/bin/activate.csh
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/venv-3.9.16/bin/activate.fish
+-rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/venv-3.9.16/bin/hatch
+-rwxr-xr-x   0        0        0      293 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/venv-3.9.16/bin/hatchling
+-rwxr-xr-x   0        0        0      275 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/venv-3.9.16/bin/httpx
+-rwxr-xr-x   0        0        0      281 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/venv-3.9.16/bin/keyring
+-rwxr-xr-x   0        0        0      291 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/venv-3.9.16/bin/markdown-it
+-rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/venv-3.9.16/bin/pip
+-rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/venv-3.9.16/bin/pip3
+-rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/venv-3.9.16/bin/pip3.9
+-rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/venv-3.9.16/bin/pygmentize
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/venv-3.9.16/bin/python -> /Users/quigleymalcolm/.asdf/installs/python/3.9.16/bin/python
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/venv-3.9.16/bin/python3 -> python
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/venv-3.9.16/bin/python3.9 -> python
+-rwxr-xr-x   0        0        0      290 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/venv-3.9.16/bin/userpath
+-rwxr-xr-x   0        0        0      309 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/venv-3.9.16/bin/virtualenv
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/LICENSE
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/README.md
+-rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/pyproject.toml
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev2/PKG-INFO
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/dataclass_serialization.py` & `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/dataclass_serialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,33 +203,40 @@
                 for x in obj
             )
         elif issubclass(object_type, SerializableDataclass):
             if not dataclasses.is_dataclass(object_type):
                 raise RuntimeError(f"{object_type} is not a dataclass")
             if not isinstance(obj, SerializableDataclass):
                 raise RuntimeError(f"{obj} is not a SerializableDataclass")
+
+            # Redundant assertion is needed for mypy to pass.
+            assert issubclass(object_type, SerializableDataclass)
+
             PydanticModel = self._to_pydantic_type_converter.to_pydantic_type(object_type)
 
             field_dict = _get_dataclass_field_definitions(object_type)
             field_values: Dict[str, AnyValueType] = {}
             for field_name, field_definition in field_dict.items():
                 field_values[field_name] = self._convert_dataclass_instance_to_pydantic_model(
                     object_type=field_definition.annotated_field_type,
                     obj=getattr(obj, field_name),
                 )
             return PydanticModel(**field_values)
 
         return obj
 
     def pydantic_serialize(self, obj: SerializableDataclassT) -> str:  # noqa: D
-        assert dataclasses.is_dataclass(obj)
+        # .__class__ seems to be the approach for new classes and there are differences with type(obj)
+        obj_class = obj.__class__
+        assert dataclasses.is_dataclass(obj), f"Got object of type: {obj_class.__name__}"
+        assert isinstance(obj, SerializableDataclass), f"Got object of type: {obj_class.__name__}"
+        assert issubclass(obj_class, SerializableDataclass), f"Got object type: {obj_class.__name__}"
 
         return self._convert_dataclass_instance_to_pydantic_model(
-            # .__class__ seems to be the approach for new classes and there are differences with type(obj)
-            object_type=obj.__class__,
+            object_type=obj_class,
             obj=obj,
         ).json()
 
 
 class DataClassDeserializer:
     """Corresponding deserializer for datclasses that were serialized by DataClassSerializer."""
 
@@ -257,24 +264,27 @@
                 self._convert_field_in_pydantic_object_to_actual_object(
                     field_type=tuple_type_parameter,
                     obj=x,
                 )
                 for x in obj
             )
         elif issubclass(field_type, SerializableDataclass):
-            logger.debug(f"Handling field_type={field_type} object={repr(obj)}")
-            return self._construct_dataclass_from_pydantic_object(
+            logger.error(f"Handling field_type={field_type} object={repr(obj)}")
+            # Redundant assertion is needed for mypy to pass.
+            assert issubclass(field_type, SerializableDataclass), f"Got field type: {field_type.__name__}"
+            assert isinstance(obj, (SerializableDataclass, BaseModel)), f"Got object of type: {obj.__class__.__name__}"
+            return self._construct_dataclass_from_dataclass_like_object(
                 dataclass_type=field_type,
                 obj=obj,
             )
         else:
             return obj
 
-    def _construct_dataclass_from_pydantic_object(
-        self, dataclass_type: Type[SerializableDataclassT], obj: BaseModel
+    def _construct_dataclass_from_dataclass_like_object(
+        self, dataclass_type: Type[SerializableDataclassT], obj: Union[SerializableDataclass, BaseModel]
     ) -> SerializableDataclassT:
         logger.debug(f"Constructing dataclass of type {dataclass_type} from {repr(obj)}")
         object_args = {}
         field_dict = _get_dataclass_field_definitions(dataclass_type)
         for field_name, field_definition in field_dict.items():
             object_args[field_name] = self._convert_field_in_pydantic_object_to_actual_object(
                 field_type=field_definition.annotated_field_type,
@@ -286,15 +296,15 @@
     def pydantic_deserialize(  # noqa: D
         self, dataclass_type: Type[SerializableDataclassT], serialized_obj: str
     ) -> SerializableDataclassT:
         try:
             ClassAsPydantic = self._to_pydantic_type_converter.to_pydantic_type(dataclass_type)
             logger.debug(f"Serialized object for creation of {ClassAsPydantic} is {serialized_obj}")
             pydantic_object = ClassAsPydantic.parse_raw(serialized_obj)
-            return self._construct_dataclass_from_pydantic_object(
+            return self._construct_dataclass_from_dataclass_like_object(
                 dataclass_type=dataclass_type,
                 obj=pydantic_object,
             )
 
         except Exception as e:
             raise DataclassDeserializationError from e
 
@@ -333,15 +343,15 @@
             fields_for_pydantic_model[field_name] = field_definition.as_pydantic_field_tuple()
             logger.debug(f"Adding {field_name} with type {field_definition.annotated_field_type}")
 
         class_name = dataclass_type.__name__ + "AsPydantic"
         logger.debug(
             f"Creating Pydantic model {class_name} with fields:\n{pformat_big_objects(fields_for_pydantic_model)}"
         )
-        pydantic_model = pydantic.create_model(class_name, **fields_for_pydantic_model)
+        pydantic_model = pydantic.create_model(class_name, **fields_for_pydantic_model)  # type: ignore
         logger.debug(f"Finished creating Pydantic model {class_name}")
         logger.debug(f"Finished converting {dataclass_type.__name__} to a pydantic class")
         return pydantic_model
 
     @staticmethod
     def _convert_nested_fields(field_definition: FieldDefinition) -> FieldDefinition:
         """Recursively converts a given field definition into a fully serializable type specification.
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/enum_extension.py` & `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/enum_extension.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/errors.py` & `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/errors.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/pretty_print.py` & `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/pretty_print.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import pprint
 import textwrap
 from collections.abc import Mapping
 from dataclasses import fields, is_dataclass
 
-from dbt_semantic_interfaces.objects.base import HashableBaseModel
+from dbt_semantic_interfaces.implementations.base import HashableBaseModel
 
 
 def is_hashable_base_model(obj):  # type:ignore # noqa: D
     return isinstance(obj, HashableBaseModel)
 
 
 def _to_pretty_printable_object(obj):  # type: ignore
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/references.py` & `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/references.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/test_utils.py` & `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/test_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,49 @@
 import datetime
 import logging
 import textwrap
 from typing import Callable, Optional, Sequence, Tuple
 
 import dateutil.parser
 
-from dbt_semantic_interfaces.objects.elements.dimension import Dimension
-from dbt_semantic_interfaces.objects.elements.entity import Entity
-from dbt_semantic_interfaces.objects.elements.measure import Measure
-from dbt_semantic_interfaces.objects.filters.where_filter import WhereFilter
-from dbt_semantic_interfaces.objects.metadata import FileSlice, Metadata
-from dbt_semantic_interfaces.objects.metric import Metric, MetricType, MetricTypeParams
-from dbt_semantic_interfaces.objects.semantic_manifest import SemanticManifest
-from dbt_semantic_interfaces.objects.semantic_model import NodeRelation, SemanticModel
+from dbt_semantic_interfaces.implementations.elements.dimension import PydanticDimension
+from dbt_semantic_interfaces.implementations.elements.entity import PydanticEntity
+from dbt_semantic_interfaces.implementations.elements.measure import PydanticMeasure
+from dbt_semantic_interfaces.implementations.filters.where_filter import (
+    PydanticWhereFilter,
+)
+from dbt_semantic_interfaces.implementations.metadata import (
+    PydanticFileSlice,
+    PydanticMetadata,
+)
+from dbt_semantic_interfaces.implementations.metric import (
+    MetricType,
+    PydanticMetric,
+    PydanticMetricTypeParams,
+)
+from dbt_semantic_interfaces.implementations.semantic_manifest import (
+    PydanticSemanticManifest,
+)
+from dbt_semantic_interfaces.implementations.semantic_model import (
+    NodeRelation,
+    PydanticSemanticModel,
+)
 from dbt_semantic_interfaces.parsing.objects import YamlConfigFile
 
 logger = logging.getLogger(__name__)
 
 
 def as_datetime(date_string: str) -> datetime.datetime:
     """Helper to convert a string like '2020-01-01' into a datetime object."""
     return dateutil.parser.parse(date_string)
 
 
 def find_semantic_model_with(
-    model: SemanticManifest, function: Callable[[SemanticModel], bool]
-) -> Tuple[SemanticModel, int]:
+    model: PydanticSemanticManifest, function: Callable[[PydanticSemanticModel], bool]
+) -> Tuple[PydanticSemanticModel, int]:
     """Returns a semantic model from the model which matches the criteria defined by the passed in function'.
 
     This is useful because the order of semantic models in the list is non determinant, thus it's impossible to
     hard code which semantic model you want by index. Using semantic model names isn't great for consistency because
     semantic models change and might no longer have the necessary parts to be useful for a given test. This
     allows us to guarantee that a semantic model will be returned which meets the requirements of what a test needs,
     unless none of the semantic models will work.
@@ -37,15 +51,17 @@
     for index, semantic_model in enumerate(model.semantic_models):
         if function(semantic_model):
             return semantic_model, index
 
     raise Exception("Unable to find a semantic_model matching function criteria")
 
 
-def find_metric_with(model: SemanticManifest, function: Callable[[Metric], bool]) -> Tuple[Metric, int]:
+def find_metric_with(
+    model: PydanticSemanticManifest, function: Callable[[PydanticMetric], bool]
+) -> Tuple[PydanticMetric, int]:
     """Returns a metric from the model which matches the criteria defined by the passed in function'.
 
     This is useful because the order of metrics in the list is non-determinant, thus it's impossible to
     hard code which metric you want by index. Using metric names isn't great for consistency because
     metrics change and might no longer have the necessary parts to be useful for a given test. This
     allows us to guarantee that a metric will be returned which meets the requirements of what a test needs,
     unless none of the metrics will work.
@@ -74,83 +90,83 @@
             - name: example_entity
               type: primary
               role: test_role
               expr: example_id
           measures:
             - name: num_sample_rows
               agg: sum
+              agg_time_dimension: ds
               expr: 1
               create_metric: true
           dimensions:
             - name: ds
               type: time
               type_params:
                 time_granularity: day
-                is_primary: true
         """
     )
     return YamlConfigFile(filepath="inline_for_test", contents=yaml_contents)
 
 
-def default_meta() -> Metadata:
+def default_meta() -> PydanticMetadata:
     """Returns a Metadata object with the required information."""
-    return Metadata(
+    return PydanticMetadata(
         repo_file_path="/not/from/a/repo",
-        file_slice=FileSlice(
+        file_slice=PydanticFileSlice(
             filename="not_from_file.py",
             content="N/A",
             start_line_number=0,
             end_line_number=0,
         ),
     )
 
 
 def metric_with_guaranteed_meta(
     name: str,
     type: MetricType,
-    type_params: MetricTypeParams,
-    where_filter: Optional[WhereFilter] = None,
-    metadata: Metadata = default_meta(),
+    type_params: PydanticMetricTypeParams,
+    where_filter: Optional[PydanticWhereFilter] = None,
+    metadata: PydanticMetadata = default_meta(),
     description: str = "adhoc metric",
-) -> Metric:
+) -> PydanticMetric:
     """Creates a metric with the given input.
 
     If a metadata object is not supplied, a default metadata object is used.
     """
-    return Metric(
+    return PydanticMetric(
         name=name,
         description=description,
         type=type,
         type_params=type_params,
         filter=where_filter,
         metadata=metadata,
     )
 
 
 def semantic_model_with_guaranteed_meta(
     name: str,
     description: Optional[str] = None,
     node_relation: Optional[NodeRelation] = None,
-    metadata: Metadata = default_meta(),
-    entities: Sequence[Entity] = (),
-    measures: Sequence[Measure] = (),
-    dimensions: Sequence[Dimension] = (),
-) -> SemanticModel:
+    metadata: PydanticMetadata = default_meta(),
+    entities: Sequence[PydanticEntity] = (),
+    measures: Sequence[PydanticMeasure] = (),
+    dimensions: Sequence[PydanticDimension] = (),
+) -> PydanticSemanticModel:
     """Creates a semantic model with the given input.
 
     If a metadata object is not supplied, a default metadata object is used.
     """
     created_node_relation = node_relation
     if created_node_relation is None:
         created_node_relation = NodeRelation(
             schema_name="schema",
             alias="table",
         )
 
-    return SemanticModel(
+    return PydanticSemanticModel(
         name=name,
         description=description,
         node_relation=created_node_relation,
         entities=entities,
         measures=measures,
         dimensions=dimensions,
         metadata=metadata,
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/objects/base.py` & `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/implementations/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import json
 import os
 from abc import ABC, abstractmethod
-from typing import Any, Callable, ClassVar, Generic, Iterator, TypeVar
+from typing import Any, Callable, ClassVar, Generator, Generic, Type, TypeVar
 
 from pydantic import BaseModel, root_validator
 
 from dbt_semantic_interfaces.errors import ParsingException
 from dbt_semantic_interfaces.parsing.yaml_loader import (
     PARSING_CONTEXT_KEY,
     ParsingContext,
@@ -101,14 +101,16 @@
             },
         }
         return values
 
 
 ModelObjectT_co = TypeVar("ModelObjectT_co", covariant=True, bound=BaseModel)
 
+SelfTypeT = TypeVar("SelfTypeT", bound="PydanticCustomInputParser")
+
 
 class PydanticCustomInputParser(ABC, Generic[ModelObjectT_co]):
     """Implements required methods for enabling custom parsing for Pydantic BaseModel objects.
 
     This abstract class helper is for the specific case where model object classes need to do custom parsing
     prior to object initialization, meaning that the inputs to the initializer itself must be parsed in a
     manner custom to the object, but without updating the input values for the rest of the model hierarchy.
@@ -117,43 +119,49 @@
     processed and validated in the standard Pydantic way. Any subclass needing to mutate the inputs from a dict
     or object type in a subclass-specific way should still be able to do so via the standard Pydantic approach
     of adding a method decorated with @validator or @root_validator, which will work internally to initialization
     and validation of that model object itself.
     """
 
     @classmethod
-    def __get_validators__(cls) -> Iterator[Callable]:
+    def __get_validators__(
+        cls: Type[PydanticCustomInputParser[ModelObjectT_co]],
+    ) -> Generator[Callable[[PydanticParseableValueType], PydanticCustomInputParser[ModelObjectT_co]], None, None]:
         """Pydantic magic method for allowing parsing of arbitrary input on parse_obj invocation.
 
-        This allow for parsing and validation prior to object initialization. Most classes implementing this
+        This allows for parsing and validation prior to object initialization. Most classes implementing this
         interface in our model are doing so because the input value from user-supplied YAML will be a string
         representation rather than the structured object type.
         """
         yield cls.__parse_with_custom_handling
 
     @classmethod
-    def __parse_with_custom_handling(cls: ModelObjectT_co, input: PydanticParseableValueType) -> ModelObjectT_co:
+    def __parse_with_custom_handling(
+        cls: Type[PydanticCustomInputParser[ModelObjectT_co]], input: PydanticParseableValueType
+    ) -> PydanticCustomInputParser[ModelObjectT_co]:
         """Core method for handling common valid - or easily validated - input types.
 
         Pydantic objects can commonly appear as JSON object types (from, e.g., deserializing a Pydantic-serialized
         model) or direct instances of the model object class (from, e.g., initializing an object and passing it in
         to the initializer of a containing model object). This internal wrapper handles both of these cases in the
         standard Pydantic way of either validating the object type input on initialization, or passing the
         already-validated instance along as the output.
 
         Note this will also pass any Pydantic instance initialized via the `construct` method, which means it is
         possible for a caller to thread an unvalidated - and therefore improperly initialized - instance through.
         However, this is part of the contract with `construct` - it is only to be used when the inputs are known
         to the caller to be pre-validated, and so we do not bother guarding against that here.
         """
         if isinstance(input, dict):
-            return cls(**input)
+            return cls(**input)  # type: ignore
         elif isinstance(input, cls):
             return input
         else:
             return cls._from_yaml_value(input)
 
     @classmethod
     @abstractmethod
-    def _from_yaml_value(cls: ModelObjectT_co, input: PydanticParseableValueType) -> ModelObjectT_co:
+    def _from_yaml_value(
+        cls: Type[PydanticCustomInputParser[ModelObjectT_co]], input: PydanticParseableValueType
+    ) -> PydanticCustomInputParser[ModelObjectT_co]:
         """Abstract method for providing object-specific parsing logic."""
         raise NotImplementedError()
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/objects/metric.py` & `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/implementations/metric.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 from __future__ import annotations
 
 from typing import List, Optional
 
 from dbt_semantic_interfaces.errors import ParsingException
-from dbt_semantic_interfaces.objects.base import (
+from dbt_semantic_interfaces.implementations.base import (
     HashableBaseModel,
     ModelWithMetadataParsing,
     PydanticCustomInputParser,
     PydanticParseableValueType,
 )
-from dbt_semantic_interfaces.objects.filters.where_filter import WhereFilter
-from dbt_semantic_interfaces.objects.metadata import Metadata
+from dbt_semantic_interfaces.implementations.filters.where_filter import (
+    PydanticWhereFilter,
+)
+from dbt_semantic_interfaces.implementations.metadata import PydanticMetadata
 from dbt_semantic_interfaces.references import MeasureReference, MetricReference
 from dbt_semantic_interfaces.type_enums.metric_type import MetricType
 from dbt_semantic_interfaces.type_enums.time_granularity import (
     TimeGranularity,
     string_to_time_granularity,
 )
 
 
-class MetricInputMeasure(PydanticCustomInputParser, HashableBaseModel):
+class PydanticMetricInputMeasure(PydanticCustomInputParser, HashableBaseModel):
     """Provides a pointer to a measure along with metric-specific processing directives.
 
     If an alias is set, this will be used as the string name reference for this measure after the aggregation
     phase in the SQL plan.
     """
 
     name: str
-    filter: Optional[WhereFilter]
+    filter: Optional[PydanticWhereFilter]
     alias: Optional[str]
 
     @classmethod
-    def _from_yaml_value(cls, input: PydanticParseableValueType) -> MetricInputMeasure:
+    def _from_yaml_value(cls, input: PydanticParseableValueType) -> PydanticMetricInputMeasure:
         """Parses a MetricInputMeasure from a string (name only) or object (struct spec) input.
 
-        For user input cases, the original YAML spec for a Metric included measure(s) specified as string names
+        For user input cases, the original YAML spec for a PydanticMetric included measure(s) specified as string names
         or lists of string names. As such, configs pre-dating the addition of this model type will only provide the
         base name for this object.
         """
         if isinstance(input, str):
-            return MetricInputMeasure(name=input)
+            return PydanticMetricInputMeasure(name=input)
         else:
             raise ValueError(
                 f"MetricInputMeasure inputs from model configs are expected to be of either type string or "
                 f"object (key/value pairs), but got type {type(input)} with value: {input}"
             )
 
     @property
@@ -53,39 +55,36 @@
 
     @property
     def post_aggregation_measure_reference(self) -> MeasureReference:
         """Property accessor to get the MeasureReference with the aliased name, if appropriate."""
         return MeasureReference(element_name=self.alias or self.name)
 
 
-class MetricTimeWindow(PydanticCustomInputParser, HashableBaseModel):
+class PydanticMetricTimeWindow(PydanticCustomInputParser, HashableBaseModel):
     """Describes the window of time the metric should be accumulated over, e.g., '1 day', '2 weeks', etc."""
 
     count: int
     granularity: TimeGranularity
 
-    def to_string(self) -> str:  # noqa: D
-        return f"{self.count} {self.granularity.value}"
-
     @classmethod
-    def _from_yaml_value(cls, input: PydanticParseableValueType) -> MetricTimeWindow:
+    def _from_yaml_value(cls, input: PydanticParseableValueType) -> PydanticMetricTimeWindow:
         """Parses a MetricTimeWindow from a string input found in a user provided model specification.
 
         The MetricTimeWindow is always expected to be provided as a string in user-defined YAML configs.
         """
         if isinstance(input, str):
-            return MetricTimeWindow.parse(input)
+            return PydanticMetricTimeWindow.parse(input)
         else:
             raise ValueError(
                 f"MetricTimeWindow inputs from model configs are expected to always be of type string, but got "
                 f"type {type(input)} with value: {input}"
             )
 
     @staticmethod
-    def parse(window: str) -> MetricTimeWindow:
+    def parse(window: str) -> PydanticMetricTimeWindow:
         """Returns window values if parsing succeeds, None otherwise.
 
         Output of the form: (<time unit count>, <time granularity>, <error message>) - error message is None if window
         is formatted properly
         """
         parts = window.split(" ")
         if len(parts) != 2:
@@ -104,70 +103,70 @@
                 f"Invalid time granularity {granularity} in cumulative metric window string: ({window})",
             )
 
         count = parts[0]
         if not count.isdigit():
             raise ParsingException(f"Invalid count ({count}) in cumulative metric window string: ({window})")
 
-        return MetricTimeWindow(
+        return PydanticMetricTimeWindow(
             count=int(count),
             granularity=string_to_time_granularity(granularity),
         )
 
 
-class MetricInput(HashableBaseModel):
+class PydanticMetricInput(HashableBaseModel):
     """Provides a pointer to a metric along with the additional properties used on that metric."""
 
     name: str
-    filter: Optional[WhereFilter]
+    filter: Optional[PydanticWhereFilter]
     alias: Optional[str]
-    offset_window: Optional[MetricTimeWindow]
+    offset_window: Optional[PydanticMetricTimeWindow]
     offset_to_grain: Optional[TimeGranularity]
 
     @property
     def as_reference(self) -> MetricReference:
         """Property accessor to get the MetricReference associated with this metric input."""
         return MetricReference(element_name=self.name)
 
 
-class MetricTypeParams(HashableBaseModel):
+class PydanticMetricTypeParams(HashableBaseModel):
     """Type params add additional context to certain metric types (the context depends on the metric type)."""
 
-    measure: Optional[MetricInputMeasure]
-    measures: Optional[List[MetricInputMeasure]]
-    numerator: Optional[MetricInputMeasure]
-    denominator: Optional[MetricInputMeasure]
+    measure: Optional[PydanticMetricInputMeasure]
+    measures: Optional[List[PydanticMetricInputMeasure]]
+    numerator: Optional[PydanticMetricInputMeasure]
+    denominator: Optional[PydanticMetricInputMeasure]
     expr: Optional[str]
-    window: Optional[MetricTimeWindow]
+    window: Optional[PydanticMetricTimeWindow]
     grain_to_date: Optional[TimeGranularity]
-    metrics: Optional[List[MetricInput]]
+    metrics: Optional[List[PydanticMetricInput]]
 
     @property
     def numerator_measure_reference(self) -> Optional[MeasureReference]:
         """Return the measure reference, if any, associated with the metric input measure defined as the numerator."""
         return self.numerator.measure_reference if self.numerator else None
 
     @property
     def denominator_measure_reference(self) -> Optional[MeasureReference]:
         """Return the measure reference, if any, associated with the metric input measure defined as the denominator."""
         return self.denominator.measure_reference if self.denominator else None
 
 
-class Metric(HashableBaseModel, ModelWithMetadataParsing):
+class PydanticMetric(HashableBaseModel, ModelWithMetadataParsing):
     """Describes a metric."""
 
     name: str
     description: Optional[str]
     type: MetricType
-    type_params: MetricTypeParams
-    filter: Optional[WhereFilter]
-    metadata: Optional[Metadata]
+    type_params: PydanticMetricTypeParams
+    filter: Optional[PydanticWhereFilter]
+    metadata: Optional[PydanticMetadata]
 
     @property
-    def input_measures(self) -> List[MetricInputMeasure]:
+    def input_measures(self) -> List[PydanticMetricInputMeasure]:
         """Return the complete list of input measure configurations for this metric."""
         tp = self.type_params
         res = tp.measures or []
         if tp.measure:
             res.append(tp.measure)
         if tp.numerator:
             res.append(tp.numerator)
@@ -178,10 +177,10 @@
 
     @property
     def measure_references(self) -> List[MeasureReference]:
         """Return the measure references associated with all input measure configurations for this metric."""
         return [x.measure_reference for x in self.input_measures]
 
     @property
-    def input_metrics(self) -> List[MetricInput]:
+    def input_metrics(self) -> List[PydanticMetricInput]:
         """Return the associated input metrics for this metric."""
         return self.type_params.metrics or []
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/objects/semantic_model.py` & `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/implementations/semantic_model.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 from __future__ import annotations
 
 from typing import Any, List, Optional, Sequence
 
 from pydantic import validator
+from typing_extensions import override
 
-from dbt_semantic_interfaces.objects.base import (
+from dbt_semantic_interfaces.implementations.base import (
     HashableBaseModel,
     ModelWithMetadataParsing,
 )
-from dbt_semantic_interfaces.objects.elements.dimension import Dimension
-from dbt_semantic_interfaces.objects.elements.entity import Entity
-from dbt_semantic_interfaces.objects.elements.measure import Measure
-from dbt_semantic_interfaces.objects.metadata import Metadata
+from dbt_semantic_interfaces.implementations.elements.dimension import PydanticDimension
+from dbt_semantic_interfaces.implementations.elements.entity import PydanticEntity
+from dbt_semantic_interfaces.implementations.elements.measure import PydanticMeasure
+from dbt_semantic_interfaces.implementations.metadata import PydanticMetadata
+from dbt_semantic_interfaces.protocols.protocol_hint import ProtocolHint
+from dbt_semantic_interfaces.protocols.semantic_model import (
+    SemanticModel,
+    SemanticModelDefaults,
+)
 from dbt_semantic_interfaces.references import (
     LinkableElementReference,
     MeasureReference,
     SemanticModelReference,
 )
 
 
@@ -56,26 +62,39 @@
             return NodeRelation(database=sql_str_split[0], schema_name=sql_str_split[1], alias=sql_str_split[2])
         raise RuntimeError(
             f"Invalid input for a SQL table, expected form '<schema>.<table>' or '<db>.<schema>.<table>' "
             f"but got: {sql_str}"
         )
 
 
-class SemanticModel(HashableBaseModel, ModelWithMetadataParsing):
+class PydanticSemanticModelDefaults(HashableBaseModel, ProtocolHint[SemanticModelDefaults]):  # noqa: D
+    @override
+    def _implements_protocol(self) -> SemanticModelDefaults:  # noqa: D
+        return self
+
+    agg_time_dimension: str
+
+
+class PydanticSemanticModel(HashableBaseModel, ModelWithMetadataParsing, ProtocolHint[SemanticModel]):
     """Describes a semantic model."""
 
+    @override
+    def _implements_protocol(self) -> SemanticModel:
+        return self
+
     name: str
+    defaults: Optional[PydanticSemanticModelDefaults]
     description: Optional[str]
     node_relation: NodeRelation
 
-    entities: Sequence[Entity] = []
-    measures: Sequence[Measure] = []
-    dimensions: Sequence[Dimension] = []
+    entities: Sequence[PydanticEntity] = []
+    measures: Sequence[PydanticMeasure] = []
+    dimensions: Sequence[PydanticDimension] = []
 
-    metadata: Optional[Metadata]
+    metadata: Optional[PydanticMetadata]
 
     @property
     def entity_references(self) -> List[LinkableElementReference]:  # noqa: D
         return [i.reference for i in self.entities]
 
     @property
     def dimension_references(self) -> List[LinkableElementReference]:  # noqa: D
@@ -86,65 +105,65 @@
         return [i.reference for i in self.measures]
 
     @property
     def has_validity_dimensions(self) -> bool:  # noqa: D
         return any([dim.validity_params is not None for dim in self.dimensions])
 
     @property
-    def validity_start_dimension(self) -> Optional[Dimension]:  # noqa: D
+    def validity_start_dimension(self) -> Optional[PydanticDimension]:  # noqa: D
         validity_start_dims = [dim for dim in self.dimensions if dim.validity_params and dim.validity_params.is_start]
         if not validity_start_dims:
             return None
         assert (
             len(validity_start_dims) == 1
         ), "Found more than one validity start dimension. This should have been blocked in validation!"
         return validity_start_dims[0]
 
     @property
-    def validity_end_dimension(self) -> Optional[Dimension]:  # noqa: D
+    def validity_end_dimension(self) -> Optional[PydanticDimension]:  # noqa: D
         validity_end_dims = [dim for dim in self.dimensions if dim.validity_params and dim.validity_params.is_end]
         if not validity_end_dims:
             return None
         assert (
             len(validity_end_dims) == 1
         ), "Found more than one validity end dimension. This should have been blocked in validation!"
         return validity_end_dims[0]
 
     @property
-    def partitions(self) -> List[Dimension]:  # noqa: D
+    def partitions(self) -> List[PydanticDimension]:  # noqa: D
         return [dim for dim in self.dimensions or [] if dim.is_partition]
 
     @property
-    def partition(self) -> Optional[Dimension]:  # noqa: D
+    def partition(self) -> Optional[PydanticDimension]:  # noqa: D
         partitions = self.partitions
         if not partitions:
             return None
         if len(partitions) > 1:
             raise ValueError(f"too many partitions for semantic_model {self.name}")
         return partitions[0]
 
     @property
     def reference(self) -> SemanticModelReference:  # noqa: D
         return SemanticModelReference(semantic_model_name=self.name)
 
-    def get_measure(self, measure_reference: MeasureReference) -> Measure:  # noqa: D
+    def get_measure(self, measure_reference: MeasureReference) -> PydanticMeasure:  # noqa: D
         for measure in self.measures:
             if measure.reference == measure_reference:
                 return measure
 
         raise ValueError(
             f"No dimension with name ({measure_reference.element_name}) in semantic_model with name ({self.name})"
         )
 
-    def get_dimension(self, dimension_reference: LinkableElementReference) -> Dimension:  # noqa: D
+    def get_dimension(self, dimension_reference: LinkableElementReference) -> PydanticDimension:  # noqa: D
         for dim in self.dimensions:
             if dim.reference == dimension_reference:
                 return dim
 
         raise ValueError(f"No dimension with name ({dimension_reference}) in semantic_model with name ({self.name})")
 
-    def get_entity(self, entity_reference: LinkableElementReference) -> Entity:  # noqa: D
+    def get_entity(self, entity_reference: LinkableElementReference) -> PydanticEntity:  # noqa: D
         for entity in self.entities:
             if entity.reference == entity_reference:
                 return entity
 
         raise ValueError(f"No entity with name ({entity_reference}) in semantic_model with name ({self.name})")
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/objects/elements/dimension.py` & `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/implementations/elements/dimension.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,78 +1,70 @@
 from __future__ import annotations
 
 from typing import Optional
 
-from dbt_semantic_interfaces.objects.base import (
+from dbt_semantic_interfaces.implementations.base import (
     HashableBaseModel,
     ModelWithMetadataParsing,
 )
-from dbt_semantic_interfaces.objects.metadata import Metadata
+from dbt_semantic_interfaces.implementations.metadata import PydanticMetadata
 from dbt_semantic_interfaces.references import (
     DimensionReference,
     TimeDimensionReference,
 )
 from dbt_semantic_interfaces.type_enums.dimension_type import DimensionType
 from dbt_semantic_interfaces.type_enums.time_granularity import TimeGranularity
 
 ISO8601_FMT = "YYYY-MM-DD"
 
 
-class DimensionValidityParams(HashableBaseModel):
+class PydanticDimensionValidityParams(HashableBaseModel):
     """Parameters identifying a given dimension as an entity for validity state.
 
     This construct is used for supporting SCD Type II tables, such as might be
     created via dbt's snapshot feature, or generated via periodic loads from external
     dimension semantic models. In either of those cases, there is typically a time dimension
     associated with the SCD semantic model that indicates the start and end times of a
     validity window, where the dimension value is valid for any time within that range.
     """
 
     is_start: bool = False
     is_end: bool = False
 
 
-class DimensionTypeParams(HashableBaseModel):
-    """Dimension type params add additional context to some types (time) of dimensions."""
+class PydanticDimensionTypeParams(HashableBaseModel):
+    """PydanticDimension type params add additional context to some types (time) of dimensions."""
 
-    is_primary: bool = False
     time_granularity: TimeGranularity
-    validity_params: Optional[DimensionValidityParams] = None
+    validity_params: Optional[PydanticDimensionValidityParams] = None
 
 
-class Dimension(HashableBaseModel, ModelWithMetadataParsing):
+class PydanticDimension(HashableBaseModel, ModelWithMetadataParsing):
     """Describes a dimension."""
 
     name: str
     description: Optional[str]
     type: DimensionType
     is_partition: bool = False
-    type_params: Optional[DimensionTypeParams]
+    type_params: Optional[PydanticDimensionTypeParams]
     expr: Optional[str] = None
-    metadata: Optional[Metadata]
-
-    @property
-    def is_primary_time(self) -> bool:  # noqa: D
-        if self.type == DimensionType.TIME and self.type_params is not None:
-            return self.type_params.is_primary
-
-        return False
+    metadata: Optional[PydanticMetadata]
 
     @property
     def reference(self) -> DimensionReference:  # noqa: D
         return DimensionReference(element_name=self.name)
 
     @property
     def time_dimension_reference(self) -> TimeDimensionReference:  # noqa: D
         assert self.type == DimensionType.TIME, f"Got type as {self.type} instead of {DimensionType.TIME}"
         return TimeDimensionReference(element_name=self.name)
 
     @property
-    def validity_params(self) -> Optional[DimensionValidityParams]:
-        """Returns the DimensionValidityParams property, if it exists.
+    def validity_params(self) -> Optional[PydanticDimensionValidityParams]:
+        """Returns the PydanticDimensionValidityParams property, if it exists.
 
         This is to avoid repeatedly checking that type params is not None before doing anything with ValidityParams
         """
         if self.type_params:
             return self.type_params.validity_params
 
         return None
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/objects/elements/entity.py` & `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/implementations/elements/entity.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from __future__ import annotations
 
 from typing import Optional
 
-from dbt_semantic_interfaces.objects.base import (
+from dbt_semantic_interfaces.implementations.base import (
     HashableBaseModel,
     ModelWithMetadataParsing,
 )
-from dbt_semantic_interfaces.objects.metadata import Metadata
+from dbt_semantic_interfaces.implementations.metadata import PydanticMetadata
 from dbt_semantic_interfaces.references import EntityReference
 from dbt_semantic_interfaces.type_enums.entity_type import EntityType
 
 
-class Entity(HashableBaseModel, ModelWithMetadataParsing):
+class PydanticEntity(HashableBaseModel, ModelWithMetadataParsing):
     """Describes a entity."""
 
     name: str
     description: Optional[str]
     type: EntityType
     role: Optional[str]
     expr: Optional[str] = None
-    metadata: Optional[Metadata] = None
+    metadata: Optional[PydanticMetadata] = None
 
     @property
     def reference(self) -> EntityReference:  # noqa: D
         return EntityReference(element_name=self.name)
 
     @property
     def is_linkable_entity_type(self) -> bool:  # noqa: D
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/objects/elements/measure.py` & `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/implementations/elements/measure.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 from __future__ import annotations
 
 from typing import List, Optional
 
-from dbt_semantic_interfaces.objects.base import (
+from dbt_semantic_interfaces.implementations.base import (
     HashableBaseModel,
     ModelWithMetadataParsing,
 )
-from dbt_semantic_interfaces.objects.metadata import Metadata
+from dbt_semantic_interfaces.implementations.metadata import PydanticMetadata
 from dbt_semantic_interfaces.references import MeasureReference, TimeDimensionReference
 from dbt_semantic_interfaces.type_enums.aggregation_type import AggregationType
 
 
-class NonAdditiveDimensionParameters(HashableBaseModel):
+class PydanticNonAdditiveDimensionParameters(HashableBaseModel):
     """Describes the params for specifying non-additive dimensions in a measure.
 
     NOTE: Currently, only TimeDimensions are supported for this filter
     """
 
     name: str
 
     # Optional Fields
     window_choice: AggregationType = AggregationType.MIN
     window_groupings: List[str] = []
 
 
-class MeasureAggregationParameters(HashableBaseModel):
+class PydanticMeasureAggregationParameters(HashableBaseModel):
     """Describes parameters for aggregations."""
 
     percentile: Optional[float] = None
     use_discrete_percentile: bool = False
     use_approximate_percentile: bool = False
 
 
-class Measure(HashableBaseModel, ModelWithMetadataParsing):
+class PydanticMeasure(HashableBaseModel, ModelWithMetadataParsing):
     """Describes a measure."""
 
     name: str
     agg: AggregationType
     description: Optional[str]
     create_metric: Optional[bool]
     expr: Optional[str] = None
-    agg_params: Optional[MeasureAggregationParameters]
-    metadata: Optional[Metadata]
-    non_additive_dimension: Optional[NonAdditiveDimensionParameters] = None
+    agg_params: Optional[PydanticMeasureAggregationParameters]
+    metadata: Optional[PydanticMetadata]
+    non_additive_dimension: Optional[PydanticNonAdditiveDimensionParameters] = None
     agg_time_dimension: Optional[str] = None
 
     @property
     def checked_agg_time_dimension(self) -> TimeDimensionReference:  # noqa: D
         assert self.agg_time_dimension, (
             f"Aggregation time dimension for measure {self.name} is not set! This should either be set directly on "
             f"the measure specification in the model, or else defaulted to the primary time dimension in the data "
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/objects/filters/call_parameter_sets.py` & `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/implementations/filters/where_filter.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,136 +1,111 @@
 from __future__ import annotations
 
-from dataclasses import dataclass
-from typing import List, Sequence, Tuple
+from typing import List, Sequence
 
 import jinja2
 
-from dbt_semantic_interfaces.objects.filters.where_filter import (
-    WhereFilter,
-    WhereFilterTransform,
+from dbt_semantic_interfaces.implementations.base import (
+    HashableBaseModel,
+    PydanticCustomInputParser,
+    PydanticParseableValueType,
+)
+from dbt_semantic_interfaces.implementations.filters.call_parameter_sets import (
+    DimensionCallParameterSet,
+    EntityCallParameterSet,
+    FilterCallParameterSets,
+    ParseWhereFilterException,
+    TimeDimensionCallParameterSet,
 )
 from dbt_semantic_interfaces.references import (
     DimensionReference,
     EntityReference,
     TimeDimensionReference,
 )
 from dbt_semantic_interfaces.type_enums.time_granularity import TimeGranularity
 
 
-@dataclass(frozen=True)
-class DimensionCallParameterSet:
-    """When 'dimension(...)' is used in the Jinja template of the where filter, the parameters to that call."""
-
-    entity_path: Tuple[EntityReference, ...]
-    dimension_reference: DimensionReference
-
-
-@dataclass(frozen=True)
-class TimeDimensionCallParameterSet:
-    """When 'time_dimension(...)' is used in the Jinja template of the where filter, the parameters to that call."""
-
-    entity_path: Tuple[EntityReference, ...]
-    time_dimension_reference: TimeDimensionReference
-    time_granularity: TimeGranularity
-
-
-@dataclass(frozen=True)
-class EntityCallParameterSet:
-    """When 'entity(...)' is used in the Jinja template of the where filter, the parameters to that call."""
-
-    entity_path: Tuple[EntityReference, ...]
-    entity_reference: EntityReference
-
-
-@dataclass(frozen=True)
-class FilterCallParameterSets:
-    """The calls for metric items made in the Jinja template of the where filter."""
+class PydanticWhereFilter(PydanticCustomInputParser, HashableBaseModel):
+    """A filter applied to the data set containing measures, dimensions, identifiers relevant to the query.
 
-    dimension_call_parameter_sets: Tuple[DimensionCallParameterSet, ...] = ()
-    time_dimension_call_parameter_sets: Tuple[TimeDimensionCallParameterSet, ...] = ()
-    entity_call_parameter_sets: Tuple[EntityCallParameterSet, ...] = ()
-
-
-class ParseWhereFilterException(Exception):  # noqa: D
-    pass
-
-
-class ParseToCallParameterSets(WhereFilterTransform[FilterCallParameterSets]):
-    """Parses the where filter and returns the calls used in the template.
-
-    An abbreviated example:
-
-    WhereFilter("{{ dimension('home_state_latest', entity_path=['user']) }} IN ('CA', 'HI', 'WA')")
-
-    ->
-
-    FilterCallParameterSets(
-        dimension_call_parameter_sets=(
-            DimensionCallParameterSet(
-                entity_path=("user",),
-                dimension_reference="home_state_latest",
-            ),
-        )
-        ...
-    )
+    TODO: Clarify whether the filter applies to aggregated or un-aggregated data sets.
 
+    The data set will contain dimensions as required by the query and the dimensions that a referenced in any of the
+    filters that are used in the definition of metrics.
     """
 
-    # To extract the parameters to the calls, we use a function to record the parameters while rendering the Jinja
-    # template. The rendered result is not used, but since Jinja has to render something, using this as a placeholder.
-    _DUMMY_PLACEHOLDER = "DUMMY_PLACEHOLDER"
+    where_sql_template: str
+
+    @classmethod
+    def _from_yaml_value(
+        cls,
+        input: PydanticParseableValueType,
+    ) -> PydanticWhereFilter:
+        """Parses a WhereFilter from a string found in a user-provided model specification.
+
+        User-provided constraint strings are SQL snippets conforming to the expectations of SQL WHERE clauses,
+        and as such we parse them using our standard parse method below.
+        """
+        if isinstance(input, str):
+            return PydanticWhereFilter(where_sql_template=input)
+        else:
+            raise ValueError(f"Expected input to be of type string, but got type {type(input)} with value: {input}")
+
+    @property
+    def call_parameter_sets(self) -> FilterCallParameterSets:
+        """Return the result of extracting the semantic objects referenced in the where SQL template string."""
+        # To extract the parameters to the calls, we use a function to record the parameters while rendering the Jinja
+        # template. The rendered result is not used, but since Jinja has to render something, using this as a
+        # placeholder. An alternative approach would have been to use the Jinja AST API, but this seemed simpler.
+        _DUMMY_PLACEHOLDER = "DUMMY_PLACEHOLDER"
 
-    def transform(self, where_filter: WhereFilter) -> FilterCallParameterSets:  # noqa: D
         dimension_call_parameter_sets: List[DimensionCallParameterSet] = []
         time_dimension_call_parameter_sets: List[TimeDimensionCallParameterSet] = []
         entity_call_parameter_sets: List[EntityCallParameterSet] = []
 
         def _dimension_call(dimension_name: str, entity_path: Sequence[str] = ()) -> str:
             """Gets called by Jinja when rendering {{ dimension(...) }}."""
             dimension_call_parameter_sets.append(
                 DimensionCallParameterSet(
                     dimension_reference=DimensionReference(element_name=dimension_name),
                     entity_path=tuple(EntityReference(element_name=arg) for arg in entity_path),
                 )
             )
-            return ParseToCallParameterSets._DUMMY_PLACEHOLDER
+            return _DUMMY_PLACEHOLDER
 
         def _time_dimension_call(
             time_dimension_name: str, time_granularity_name: str, entity_path: Sequence[str] = ()
         ) -> str:
             """Gets called by Jinja when rendering {{ time_dimension(...) }}."""
             time_dimension_call_parameter_sets.append(
                 TimeDimensionCallParameterSet(
                     time_dimension_reference=TimeDimensionReference(element_name=time_dimension_name),
                     entity_path=tuple(EntityReference(element_name=arg) for arg in entity_path),
                     time_granularity=TimeGranularity(time_granularity_name),
                 )
             )
-            return ParseToCallParameterSets._DUMMY_PLACEHOLDER
+            return _DUMMY_PLACEHOLDER
 
         def _entity_call(entity_name: str, entity_path: Sequence[str] = ()) -> str:
             """Gets called by Jinja when rendering {{ entity(...) }}."""
             entity_call_parameter_sets.append(
                 EntityCallParameterSet(
                     entity_path=tuple(EntityReference(element_name=arg) for arg in entity_path),
                     entity_reference=EntityReference(element_name=entity_name),
                 )
             )
-            return ParseToCallParameterSets._DUMMY_PLACEHOLDER
+            return _DUMMY_PLACEHOLDER
 
         try:
-            jinja2.Template(where_filter.where_sql_template, undefined=jinja2.StrictUndefined).render(
+            jinja2.Template(self.where_sql_template, undefined=jinja2.StrictUndefined).render(
                 dimension=_dimension_call,
                 time_dimension=_time_dimension_call,
                 entity=_entity_call,
             )
         except (jinja2.exceptions.UndefinedError, jinja2.exceptions.TemplateSyntaxError) as e:
-            raise ParseWhereFilterException(
-                f"Error while parsing Jinja template:\n{where_filter.where_sql_template}"
-            ) from e
+            raise ParseWhereFilterException(f"Error while parsing Jinja template:\n{self.where_sql_template}") from e
 
         return FilterCallParameterSets(
             dimension_call_parameter_sets=tuple(dimension_call_parameter_sets),
             time_dimension_call_parameter_sets=tuple(time_dimension_call_parameter_sets),
             entity_call_parameter_sets=tuple(entity_call_parameter_sets),
         )
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/parsing/dir_to_model.py` & `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/parsing/dir_to_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,61 +4,65 @@
 from dataclasses import dataclass
 from string import Template
 from typing import Dict, List, Optional, Type, Union
 
 from jsonschema import exceptions
 
 from dbt_semantic_interfaces.errors import ParsingException
-from dbt_semantic_interfaces.model_transformer import ModelTransformer
-from dbt_semantic_interfaces.objects.metric import Metric
-from dbt_semantic_interfaces.objects.semantic_manifest import SemanticManifest
-from dbt_semantic_interfaces.objects.semantic_model import SemanticModel
+from dbt_semantic_interfaces.implementations.metric import PydanticMetric
+from dbt_semantic_interfaces.implementations.semantic_manifest import (
+    PydanticSemanticManifest,
+)
+from dbt_semantic_interfaces.implementations.semantic_model import PydanticSemanticModel
+from dbt_semantic_interfaces.model_transformer import (
+    PydanticSemanticManifestTransformer,
+)
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
 from dbt_semantic_interfaces.validations.validator_helpers import (
     FileContext,
-    ModelValidationException,
-    ModelValidationResults,
+    SemanticManifestValidationException,
+    SemanticManifestValidationResults,
     ValidationError,
     ValidationIssue,
 )
 
 logger = logging.getLogger(__name__)
 
 VERSION_KEY = "mf_config_schema"
 METRIC_TYPE = "metric"
 SEMANTIC_MODEL_TYPE = "semantic_model"
 DOCUMENT_TYPES = [METRIC_TYPE, SEMANTIC_MODEL_TYPE]
 
 
 @dataclass(frozen=True)
 class ModelBuildResult:  # noqa: D
-    model: SemanticManifest
+    model: PydanticSemanticManifest
     # Issues found in the model.
-    issues: ModelValidationResults = ModelValidationResults()
+    issues: SemanticManifestValidationResults = SemanticManifestValidationResults()
 
 
 @dataclass(frozen=True)
 class FileParsingResult:
     """Results of parsing a config file.
 
     Attributes:
         elements: MetricFlow model elements parsed from the file
         issues: Issues found when trying to parse the file
     """
 
-    elements: List[Union[SemanticModel, Metric]]
+    elements: List[Union[PydanticSemanticModel, PydanticMetric]]
     issues: List[ValidationIssue]
 
 
 def collect_yaml_config_file_paths(directory: str) -> List[str]:
     """Collects a list of file paths for model config files.
 
     Ignores files that are:
@@ -160,29 +164,29 @@
     build_result = parse_yaml_files_to_model(yaml_config_files)
     model = build_result.model
     assert model
 
     build_issues = build_result.issues
     try:
         if apply_transformations:
-            model = ModelTransformer.transform(model)
+            model = PydanticSemanticManifestTransformer.transform(model)
     except Exception as e:
-        transformation_issue_results = ModelValidationResults(errors=[ValidationError(message=str(e))])
-        build_issues = ModelValidationResults.merge([build_issues, transformation_issue_results])
+        transformation_issue_results = SemanticManifestValidationResults(errors=(ValidationError(message=str(e)),))
+        build_issues = SemanticManifestValidationResults.merge([build_issues, transformation_issue_results])
 
     if raise_issues_as_exceptions and build_issues.has_blocking_issues:
-        raise ModelValidationException(build_issues.all_issues)
+        raise SemanticManifestValidationException(build_issues.all_issues)
 
     return ModelBuildResult(model=model, issues=build_issues)
 
 
 def parse_yaml_files_to_model(
     files: List[YamlConfigFile],
-    semantic_model_class: Type[SemanticModel] = SemanticModel,
-    metric_class: Type[Metric] = Metric,
+    semantic_model_class: Type[PydanticSemanticModel] = PydanticSemanticModel,
+    metric_class: Type[PydanticMetric] = PydanticMetric,
 ) -> ModelBuildResult:
     """Builds SemanticManifest from list of config files (as strings).
 
     Persistent storage connection may be passed to write parsed objects=
     to storage and populate object metadata
 
     Note: this function does not finalize the model
@@ -204,36 +208,36 @@
                 semantic_models.append(obj)
             elif isinstance(obj, metric_class):
                 metrics.append(obj)
             else:
                 file_issues.append(
                     ValidationError(
                         context=FileContext(file_name=config_file.filepath),
-                        message=f"Unexpected model object {obj.__name__}. Expected {valid_object_classes}.",
+                        message=f"Unexpected model object {obj.__class__.__name__}. Expected {valid_object_classes}.",
                     )
                 )
 
         issues += file_issues
 
     return ModelBuildResult(
-        model=SemanticManifest(
+        model=PydanticSemanticManifest(
             semantic_models=semantic_models,
             metrics=metrics,
         ),
-        issues=ModelValidationResults.from_issues_sequence(issues),
+        issues=SemanticManifestValidationResults.from_issues_sequence(issues),
     )
 
 
 def parse_config_yaml(
     config_yaml: YamlConfigFile,
-    semantic_model_class: Type[SemanticModel] = SemanticModel,
-    metric_class: Type[Metric] = Metric,
+    semantic_model_class: Type[PydanticSemanticModel] = PydanticSemanticModel,
+    metric_class: Type[PydanticMetric] = PydanticMetric,
 ) -> FileParsingResult:
     """Parses transform config file passed as string - Returns list of model objects."""
-    results: List[Union[SemanticModel, Metric]] = []
+    results: List[Union[PydanticSemanticModel, PydanticMetric]] = []
     ctx: Optional[ParsingContext] = None
     issues: List[ValidationIssue] = []
     try:
         for config_document in YamlConfigLoader.load_all_with_context(
             name=config_yaml.filepath, contents=config_yaml.contents
         ):
             # The config document can be None if there is nothing but white space between two `---`
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/parsing/explicit_schema.py` & `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/parsing/explicit_schema.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 BASE_SCHEMA = {
     "$schema": "http://json-schema.org/draft-07/schema#",
     "type": "object",
     "title": "MetricFlow file schema",
 }
 
 
-def generate_explict_schema(schema_store: Dict) -> Dict:
+def generate_explict_json_schema(schema_store: Dict) -> Dict:
     """Generates a single json schema object from the given schema store."""
     ref_to_definition_mapping = {key: f"#/definitions/{key}" for key in schema_store.keys()}
     definitions = {}
     for schema_name, _schema in schema_store.items():
         schema = deepcopy(_schema)
 
         rewritten_schema = _rewrite_refs(schema, ref_to_definition_mapping)
@@ -61,19 +61,22 @@
         _list = []
         for element in obj:
             _list.append(_rewrite_refs(element, mapping))
         return _list
     return obj
 
 
-def write_schema(schema: Dict, output_dir: str, file_name: str) -> None:
+def write_json_schema(json_schema: Dict, output_dir: str, file_name: str) -> None:
     """Writes the schema from the specified schema store to the given path."""
     path = Path(output_dir).resolve()
     path.mkdir(exist_ok=True)
     with open(path / file_name, "w") as f:
-        json.dump(schema, f, indent=4, sort_keys=True)
+        json.dump(json_schema, f, indent=4, sort_keys=True)
+        f.write("\n")
 
 
 if __name__ == "__main__":
-    schema = generate_explict_schema(schemas.schema_store)
-    output_dir = str(Path(__file__).parent / "schemas")
-    write_schema(schema, output_dir, "metricflow.json")
+    write_json_schema(
+        json_schema=generate_explict_json_schema(schemas.schema_store),
+        output_dir=str(Path(__file__).parent / "schemas"),
+        file_name="default_explicit_schema.json",
+    )
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/parsing/objects.py` & `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/parsing/objects.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import re
 from typing import Optional
 
 from dbt_semantic_interfaces.errors import ParsingException
-from dbt_semantic_interfaces.objects.base import HashableBaseModel
+from dbt_semantic_interfaces.implementations.base import HashableBaseModel
 
 
 class YamlConfigFile(HashableBaseModel):
     """Serializable container for customer model YAML contents.
 
     The serialization support is included here for scenarios where persisting the contents in non-filesystem storage
     services is necessary or desirable.
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/parsing/schema_validator.py` & `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/parsing/schema_validator.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/parsing/schemas.py` & `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/parsing/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from dbt_semantic_interfaces.parsing.schema_validator import SchemaValidator
 
 TRANSFORM_OBJECT_NAME_PATTERN = "(?!.*__).*^[a-z][a-z0-9_]*[a-z0-9]$"
 
 
 # Enums
-metric_types_enum_values = ["MEASURE_PROXY", "RATIO", "EXPR", "CUMULATIVE", "DERIVED"]
+metric_types_enum_values = ["SIMPLE", "RATIO", "EXPR", "CUMULATIVE", "DERIVED"]
 metric_types_enum_values += [x.lower() for x in metric_types_enum_values]
 
 entity_type_enum_values = ["PRIMARY", "UNIQUE", "FOREIGN", "NATURAL"]
 entity_type_enum_values += [x.lower() for x in entity_type_enum_values]
 
 aggregation_type_values = [
     "SUM",
@@ -114,15 +114,14 @@
     "additionalProperties": False,
 }
 
 dimension_type_params_schema = {
     "$id": "dimension_type_params_schema",
     "type": "object",
     "properties": {
-        "is_primary": {"type": "boolean"},
         "time_granularity": {"enum": time_granularity_values},
         "validity_params": {"$ref": "validity_params_schema"},
     },
     "additionalProperties": False,
     "required": ["time_granularity"],
 }
 
@@ -231,23 +230,36 @@
         "database": {"type": "string"},
         "relation_name": {"type": "string"},
     },
     "additionalProperties": False,
     "required": ["alias", "schema_name"],
 }
 
+
+semantic_model_defaults_schema = {
+    "$id": "semantic_model_defaults_schema",
+    "type": "object",
+    "properties": {
+        "agg_time_dimension": {"type": "string"},
+    },
+    "additionalProperties": False,
+    "required": [],
+}
+
+
 semantic_model_schema = {
     "$id": "semantic_model",
     "type": "object",
     "properties": {
         "name": {
             "type": "string",
             "pattern": TRANSFORM_OBJECT_NAME_PATTERN,
         },
         "node_relation": {"$ref": "node_relation_schema"},
+        "defaults": {"$ref": "semantic_model_defaults_schema"},
         "entities": {"type": "array", "items": {"$ref": "entity_schema"}},
         "measures": {"type": "array", "items": {"$ref": "measure_schema"}},
         "dimensions": {"type": "array", "items": {"$ref": "dimension_schema"}},
         "description": {"type": "string"},
     },
     "additionalProperties": False,
     "required": ["name"],
@@ -284,14 +296,15 @@
     dimension_schema["$id"]: dimension_schema,
     validity_params_schema["$id"]: validity_params_schema,
     dimension_type_params_schema["$id"]: dimension_type_params_schema,
     aggregation_type_params_schema["$id"]: aggregation_type_params_schema,
     non_additive_dimension_schema["$id"]: non_additive_dimension_schema,
     metric_input_schema["$id"]: metric_input_schema,
     node_relation_schema["$id"]: node_relation_schema,
+    semantic_model_defaults_schema["$id"]: semantic_model_defaults_schema,
 }
 
 
 resolver = RefResolver.from_schema(schema=metric_schema, store=schema_store)
 semantic_model_validator = SchemaValidator(semantic_model_schema, resolver=resolver)
 derived_group_by_element_validator = SchemaValidator(derived_group_by_element_schema, resolver=resolver)
 metric_validator = SchemaValidator(metric_schema, resolver=resolver)
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/parsing/yaml_loader.py` & `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/parsing/yaml_loader.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/parsing/schemas/metricflow.json` & `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/parsing/schemas/default_explicit_schema.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9935951140873016%*

 * *Differences: {"'definitions'": "{'dimension_type_params_schema': {'properties': {delete: ['is_primary']}}, "*

 * *                  "'measure_schema': {'properties': {'agg': {'enum': {delete: [15, 5]}}}}, "*

 * *                  "'metric': {'properties': {'type': {'enum': {insert: [(0, 'SIMPLE'), (5, "*

 * *                  "'simple')], delete: [5, 0]}}}}, 'semantic_model': {'properties': {'defaults': "*

 * *                  "OrderedDict([('$ref', '#/definitions/semantic_model_defaults_schema')])}}, "*

 * *                  "'semantic_model_ […]*

```diff
@@ -94,17 +94,14 @@
             ],
             "type": "object"
         },
         "dimension_type_params_schema": {
             "$id": "dimension_type_params_schema",
             "additionalProperties": false,
             "properties": {
-                "is_primary": {
-                    "type": "boolean"
-                },
                 "time_granularity": {
                     "enum": [
                         "DAY",
                         "WEEK",
                         "MONTH",
                         "QUARTER",
                         "YEAR",
@@ -183,25 +180,23 @@
                 "agg": {
                     "enum": [
                         "SUM",
                         "MIN",
                         "MAX",
                         "AVERAGE",
                         "COUNT_DISTINCT",
-                        "BOOLEAN",
                         "SUM_BOOLEAN",
                         "COUNT",
                         "PERCENTILE",
                         "MEDIAN",
                         "sum",
                         "min",
                         "max",
                         "average",
                         "count_distinct",
-                        "boolean",
                         "sum_boolean",
                         "count",
                         "percentile",
                         "median"
                     ]
                 },
                 "agg_params": {
@@ -253,20 +248,20 @@
                 },
                 "name": {
                     "pattern": "(?!.*__).*^[a-z][a-z0-9_]*[a-z0-9]$",
                     "type": "string"
                 },
                 "type": {
                     "enum": [
-                        "MEASURE_PROXY",
+                        "SIMPLE",
                         "RATIO",
                         "EXPR",
                         "CUMULATIVE",
                         "DERIVED",
-                        "measure_proxy",
+                        "simple",
                         "ratio",
                         "expr",
                         "cumulative",
                         "derived"
                     ]
                 },
                 "type_params": {
@@ -415,14 +410,17 @@
             ],
             "type": "object"
         },
         "semantic_model": {
             "$id": "semantic_model",
             "additionalProperties": false,
             "properties": {
+                "defaults": {
+                    "$ref": "#/definitions/semantic_model_defaults_schema"
+                },
                 "description": {
                     "type": "string"
                 },
                 "dimensions": {
                     "items": {
                         "$ref": "#/definitions/dimension_schema"
                     },
@@ -449,14 +447,25 @@
                 }
             },
             "required": [
                 "name"
             ],
             "type": "object"
         },
+        "semantic_model_defaults_schema": {
+            "$id": "semantic_model_defaults_schema",
+            "additionalProperties": false,
+            "properties": {
+                "agg_time_dimension": {
+                    "type": "string"
+                }
+            },
+            "required": [],
+            "type": "object"
+        },
         "validity_params_schema": {
             "$id": "validity_params_schema",
             "additionalProperties": false,
             "properties": {
                 "is_end": {
                     "type": "boolean"
                 },
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/protocols/entity.py` & `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/protocols/entity.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,19 +6,38 @@
 from dbt_semantic_interfaces.references import EntityReference
 from dbt_semantic_interfaces.type_enums.entity_type import EntityType
 
 
 class Entity(Protocol):
     """Describes a entity."""
 
-    name: str
-    description: Optional[str]
-    type: EntityType
-    role: Optional[str]
-    expr: Optional[str] = None
+    @property
+    @abstractmethod
+    def name(self) -> str:  # noqa: D
+        pass
+
+    @property
+    @abstractmethod
+    def description(self) -> Optional[str]:  # noqa: D
+        pass
+
+    @property
+    @abstractmethod
+    def type(self) -> EntityType:  # noqa: D
+        pass
+
+    @property
+    @abstractmethod
+    def role(self) -> Optional[str]:  # noqa: D
+        pass
+
+    @property
+    @abstractmethod
+    def expr(self) -> Optional[str]:  # noqa: D
+        pass
 
     @property
     @abstractmethod
     def reference(self) -> EntityReference:
         """Returns a reference to the entity."""
         ...
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/protocols/semantic_model.py` & `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/protocols/semantic_model.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,111 @@
 from __future__ import annotations
 
 from abc import abstractmethod
-from typing import List, Optional, Protocol, Sequence
+from typing import Optional, Protocol, Sequence, TypeVar
 
-from dbt_semantic_interfaces.objects.elements.dimension import Dimension
+from dbt_semantic_interfaces.protocols.dimension import Dimension
 from dbt_semantic_interfaces.protocols.entity import Entity
 from dbt_semantic_interfaces.protocols.measure import Measure
+from dbt_semantic_interfaces.protocols.metadata import Metadata
 from dbt_semantic_interfaces.references import (
     LinkableElementReference,
     MeasureReference,
     SemanticModelReference,
 )
 
 
 class NodeRelation(Protocol):
     """Path object to where the data should be."""
 
-    alias: str
-    schema_name: str
-    database: Optional[str]
-    relation_name: str
+    @property
+    @abstractmethod
+    def alias(self) -> str:  # noqa: D
+        pass
+
+    @property
+    @abstractmethod
+    def schema_name(self) -> str:  # noqa: D
+        pass
+
+    @property
+    @abstractmethod
+    def database(self) -> Optional[str]:  # noqa: D
+        pass
+
+    @property
+    @abstractmethod
+    def relation_name(self) -> str:  # noqa: D
+        pass
+
+
+class SemanticModelDefaults(Protocol):
+    """Path object to where the data should be."""
+
+    @property
+    @abstractmethod
+    def agg_time_dimension(self) -> Optional[str]:
+        """The aggregation time dimension to use for a measure if one was not specified."""
+        pass
 
 
 class SemanticModel(Protocol):
     """Describes a semantic model."""
 
-    name: str
-    description: Optional[str]
-    node_relation: NodeRelation
+    @property
+    @abstractmethod
+    def name(self) -> str:  # noqa: D
+        pass
 
-    entities: Sequence[Entity]
-    measures: Sequence[Measure]
-    dimensions: Sequence[Dimension]
+    @property
+    @abstractmethod
+    def defaults(self) -> Optional[SemanticModelDefaults]:
+        """The defaults to use for fields when parsing this model."""
+        pass
 
     @property
     @abstractmethod
-    def entity_references(self) -> List[LinkableElementReference]:
+    def description(self) -> Optional[str]:  # noqa: D
+        pass
+
+    @property
+    @abstractmethod
+    def node_relation(self) -> NodeRelation:  # noqa: D
+        pass
+
+    @property
+    @abstractmethod
+    def entities(self) -> Sequence[Entity]:  # noqa: D
+        pass
+
+    @property
+    @abstractmethod
+    def measures(self) -> Sequence[Measure]:  # noqa: D
+        pass
+
+    @property
+    @abstractmethod
+    def dimensions(self) -> Sequence[Dimension]:  # noqa: D
+        pass
+
+    @property
+    @abstractmethod
+    def entity_references(self) -> Sequence[LinkableElementReference]:
         """Returns a list of references to all entities in the semantic model."""
         ...
 
     @property
     @abstractmethod
-    def dimension_references(self) -> List[LinkableElementReference]:
+    def dimension_references(self) -> Sequence[LinkableElementReference]:
         """Returns a list of references to all dimensions in the semantic model."""
         ...
 
     @property
     @abstractmethod
-    def measure_references(self) -> List[MeasureReference]:
+    def measure_references(self) -> Sequence[MeasureReference]:
         """Returns a list of references to all measures in the semantic model."""
         ...
 
     @property
     @abstractmethod
     def has_validity_dimensions(self) -> bool:
         """Returns True if there are validity params set on one or more dimensions."""
@@ -67,22 +121,30 @@
     @abstractmethod
     def validity_end_dimension(self) -> Optional[Dimension]:
         """Returns the validity window end dimension, if one is set."""
         ...
 
     @property
     @abstractmethod
-    def partitions(self) -> List[Dimension]:
+    def partitions(self) -> Sequence[Dimension]:
         """Returns a list of all partition dimensions."""
         ...
 
     @property
     @abstractmethod
     def partition(self) -> Optional[Dimension]:
         """Returns the partition dimension, if one is set."""
         ...
 
     @property
     @abstractmethod
     def reference(self) -> SemanticModelReference:
         """Returns a reference to this semantic model."""
         ...
+
+    @property
+    @abstractmethod
+    def metadata(self) -> Optional[Metadata]:  # noqa: D
+        pass
+
+
+SemanticModelT = TypeVar("SemanticModelT", bound=SemanticModel)
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/transformations/add_input_metric_measures.py` & `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/transformations/add_input_metric_measures.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,49 @@
 from typing import Set
 
+from typing_extensions import override
+
 from dbt_semantic_interfaces.errors import ModelTransformError
-from dbt_semantic_interfaces.objects.metric import MetricInputMeasure, MetricType
-from dbt_semantic_interfaces.objects.semantic_manifest import SemanticManifest
-from dbt_semantic_interfaces.transformations.transform_rule import ModelTransformRule
+from dbt_semantic_interfaces.implementations.metric import (
+    MetricType,
+    PydanticMetricInputMeasure,
+)
+from dbt_semantic_interfaces.implementations.semantic_manifest import (
+    PydanticSemanticManifest,
+)
+from dbt_semantic_interfaces.protocols.protocol_hint import ProtocolHint
+from dbt_semantic_interfaces.transformations.transform_rule import (
+    SemanticManifestTransformRule,
+)
 
 
-class AddInputMetricMeasuresRule(ModelTransformRule):
+class AddInputMetricMeasuresRule(ProtocolHint[SemanticManifestTransformRule[PydanticSemanticManifest]]):
     """Add all measures corresponding to the input metrics of the derived metric."""
 
+    @override
+    def _implements_protocol(self) -> SemanticManifestTransformRule[PydanticSemanticManifest]:  # noqa: D
+        return self
+
     @staticmethod
-    def _get_measures_for_metric(model: SemanticManifest, metric_name: str) -> Set[MetricInputMeasure]:
+    def _get_measures_for_metric(model: PydanticSemanticManifest, metric_name: str) -> Set[PydanticMetricInputMeasure]:
         """Returns a unique set of input measures for a given metric."""
         measures = set()
         matched_metric = next(iter((metric for metric in model.metrics if metric.name == metric_name)), None)
         if matched_metric:
             if matched_metric.type == MetricType.DERIVED:
                 for input_metric in matched_metric.input_metrics:
                     measures.update(AddInputMetricMeasuresRule._get_measures_for_metric(model, input_metric.name))
             else:
                 measures.update(set(matched_metric.input_measures))
         else:
             raise ModelTransformError(f"Metric '{metric_name}' is not configured as a metric in the model.")
         return measures
 
     @staticmethod
-    def transform_model(model: SemanticManifest) -> SemanticManifest:  # noqa: D
+    def transform_model(model: PydanticSemanticManifest) -> PydanticSemanticManifest:  # noqa: D
         for metric in model.metrics:
             if metric.type == MetricType.DERIVED:
                 measures = AddInputMetricMeasuresRule._get_measures_for_metric(model, metric.name)
                 assert (
                     metric.type_params.measures is None
                 ), "Derived metric should have no measures predefined in the config"
                 metric.type_params.measures = list(measures)
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/transformations/boolean_measure.py` & `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/transformations/boolean_measure.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,32 @@
 import logging
 
-from dbt_semantic_interfaces.objects.semantic_manifest import SemanticManifest
-from dbt_semantic_interfaces.transformations.transform_rule import ModelTransformRule
+from typing_extensions import override
+
+from dbt_semantic_interfaces.implementations.semantic_manifest import (
+    PydanticSemanticManifest,
+)
+from dbt_semantic_interfaces.protocols.protocol_hint import ProtocolHint
+from dbt_semantic_interfaces.transformations.transform_rule import (
+    SemanticManifestTransformRule,
+)
 from dbt_semantic_interfaces.type_enums.aggregation_type import AggregationType
 
 logger = logging.getLogger(__name__)
 
 
-class BooleanMeasureAggregationRule(ModelTransformRule):
+class BooleanMeasureAggregationRule(ProtocolHint[SemanticManifestTransformRule[PydanticSemanticManifest]]):
     """Converts the expression used in boolean measures so that it can be aggregated."""
 
+    @override
+    def _implements_protocol(self) -> SemanticManifestTransformRule[PydanticSemanticManifest]:  # noqa: D
+        return self
+
     @staticmethod
-    def transform_model(model: SemanticManifest) -> SemanticManifest:  # noqa: D
+    def transform_model(model: PydanticSemanticManifest) -> PydanticSemanticManifest:  # noqa: D
         for semantic_model in model.semantic_models:
             for measure in semantic_model.measures:
                 if measure.agg == AggregationType.SUM_BOOLEAN:
                     if measure.expr:
                         measure.expr = f"CASE WHEN {measure.expr} THEN 1 ELSE 0 END"
                     else:
                         measure.expr = f"CASE WHEN {measure.name} THEN 1 ELSE 0 END"
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/transformations/convert_count.py` & `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/transformations/convert_count.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,31 @@
+from typing_extensions import override
+
 from dbt_semantic_interfaces.errors import ModelTransformError
-from dbt_semantic_interfaces.objects.semantic_manifest import SemanticManifest
-from dbt_semantic_interfaces.transformations.transform_rule import ModelTransformRule
+from dbt_semantic_interfaces.implementations.semantic_manifest import (
+    PydanticSemanticManifest,
+)
+from dbt_semantic_interfaces.protocols.protocol_hint import ProtocolHint
+from dbt_semantic_interfaces.transformations.transform_rule import (
+    SemanticManifestTransformRule,
+)
 from dbt_semantic_interfaces.type_enums.aggregation_type import AggregationType
 
 ONE = "1"
 
 
-class ConvertCountToSumRule(ModelTransformRule):
+class ConvertCountToSumRule(ProtocolHint[SemanticManifestTransformRule[PydanticSemanticManifest]]):
     """Converts any COUNT measures to SUM equivalent."""
 
+    @override
+    def _implements_protocol(self) -> SemanticManifestTransformRule[PydanticSemanticManifest]:  # noqa: D
+        return self
+
     @staticmethod
-    def transform_model(model: SemanticManifest) -> SemanticManifest:  # noqa: D
+    def transform_model(model: PydanticSemanticManifest) -> PydanticSemanticManifest:  # noqa: D
         for semantic_model in model.semantic_models:
             for measure in semantic_model.measures:
                 if measure.agg == AggregationType.COUNT:
                     if measure.expr is None:
                         raise ModelTransformError(
                             f"Measure '{measure.name}' uses a COUNT aggregation, which requires an expr to be "
                             f"provided. Provide 'expr: 1' if a count of all rows is desired."
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/transformations/convert_median.py` & `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/transformations/convert_median.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,41 @@
+from typing_extensions import override
+
 from dbt_semantic_interfaces.errors import ModelTransformError
-from dbt_semantic_interfaces.objects.elements.measure import (
-    MeasureAggregationParameters,
+from dbt_semantic_interfaces.implementations.elements.measure import (
+    PydanticMeasureAggregationParameters,
+)
+from dbt_semantic_interfaces.implementations.semantic_manifest import (
+    PydanticSemanticManifest,
+)
+from dbt_semantic_interfaces.protocols.protocol_hint import ProtocolHint
+from dbt_semantic_interfaces.transformations.transform_rule import (
+    SemanticManifestTransformRule,
 )
-from dbt_semantic_interfaces.objects.semantic_manifest import SemanticManifest
-from dbt_semantic_interfaces.transformations.transform_rule import ModelTransformRule
 from dbt_semantic_interfaces.type_enums.aggregation_type import AggregationType
 
 MEDIAN_PERCENTILE = 0.5
 
 
-class ConvertMedianToPercentileRule(ModelTransformRule):
+class ConvertMedianToPercentileRule(ProtocolHint[SemanticManifestTransformRule[PydanticSemanticManifest]]):
     """Converts any MEDIAN measures to percentile equivalent."""
 
+    @override
+    def _implements_protocol(self) -> SemanticManifestTransformRule[PydanticSemanticManifest]:  # noqa: D
+        return self
+
     @staticmethod
-    def transform_model(model: SemanticManifest) -> SemanticManifest:  # noqa: D
+    def transform_model(model: PydanticSemanticManifest) -> PydanticSemanticManifest:  # noqa: D
         for semantic_model in model.semantic_models:
             for measure in semantic_model.measures:
                 if measure.agg == AggregationType.MEDIAN:
                     measure.agg = AggregationType.PERCENTILE
 
                     if not measure.agg_params:
-                        measure.agg_params = MeasureAggregationParameters()
+                        measure.agg_params = PydanticMeasureAggregationParameters()
                     else:
                         if measure.agg_params.percentile is not None and measure.agg_params.percentile != 0.5:
                             raise ModelTransformError(
                                 f"Measure '{measure.name}' uses a MEDIAN aggregation, while percentile is set to "
                                 f"'{measure.agg_params.percentile}', a conflicting value. Please remove the parameter "
                                 "or set to '0.5'."
                             )
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/transformations/names.py` & `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/transformations/names.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,50 @@
 import logging
 
-from dbt_semantic_interfaces.objects.semantic_manifest import SemanticManifest
-from dbt_semantic_interfaces.objects.semantic_model import SemanticModel
-from dbt_semantic_interfaces.transformations.transform_rule import ModelTransformRule
+from typing_extensions import override
+
+from dbt_semantic_interfaces.implementations.semantic_manifest import (
+    PydanticSemanticManifest,
+)
+from dbt_semantic_interfaces.implementations.semantic_model import PydanticSemanticModel
+from dbt_semantic_interfaces.protocols.protocol_hint import ProtocolHint
+from dbt_semantic_interfaces.transformations.transform_rule import (
+    SemanticManifestTransformRule,
+)
 
 logger = logging.getLogger(__name__)
 
 
-class LowerCaseNamesRule(ModelTransformRule):
+class LowerCaseNamesRule(ProtocolHint[SemanticManifestTransformRule[PydanticSemanticManifest]]):
     """Lowercases the names of both top level objects and semantic model elements in a model."""
 
+    @override
+    def _implements_protocol(self) -> SemanticManifestTransformRule[PydanticSemanticManifest]:  # noqa: D
+        return self
+
     @staticmethod
-    def transform_model(model: SemanticManifest) -> SemanticManifest:  # noqa: D
+    def transform_model(model: PydanticSemanticManifest) -> PydanticSemanticManifest:  # noqa: D
         LowerCaseNamesRule._lowercase_top_level_objects(model)
         for semantic_model in model.semantic_models:
             LowerCaseNamesRule._lowercase_semantic_model_elements(semantic_model)
 
         return model
 
     @staticmethod
-    def _lowercase_semantic_model_elements(semantic_model: SemanticModel) -> None:
+    def _lowercase_semantic_model_elements(semantic_model: PydanticSemanticModel) -> None:
         """Lowercases the names of semantic model elements."""
         if semantic_model.measures:
             for measure in semantic_model.measures:
                 measure.name = measure.name.lower()
         if semantic_model.entities:
             for entity in semantic_model.entities:
                 entity.name = entity.name.lower()
         if semantic_model.dimensions:
             for dimension in semantic_model.dimensions:
                 dimension.name = dimension.name.lower()
 
     @staticmethod
-    def _lowercase_top_level_objects(model: SemanticManifest) -> None:
+    def _lowercase_top_level_objects(model: PydanticSemanticManifest) -> None:
         """Lowercases the names of model objects."""
         if model.semantic_models:
             for semantic_model in model.semantic_models:
                 semantic_model.name = semantic_model.name.lower()
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/transformations/proxy_measure.py` & `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/transformations/proxy_measure.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,67 @@
 import logging
 
+from typing_extensions import override
+
 from dbt_semantic_interfaces.errors import ModelTransformError
-from dbt_semantic_interfaces.objects.metric import (
-    Metric,
-    MetricInputMeasure,
+from dbt_semantic_interfaces.implementations.metric import (
     MetricType,
-    MetricTypeParams,
+    PydanticMetric,
+    PydanticMetricInputMeasure,
+    PydanticMetricTypeParams,
+)
+from dbt_semantic_interfaces.implementations.semantic_manifest import (
+    PydanticSemanticManifest,
+)
+from dbt_semantic_interfaces.protocols.protocol_hint import ProtocolHint
+from dbt_semantic_interfaces.transformations.transform_rule import (
+    SemanticManifestTransformRule,
 )
-from dbt_semantic_interfaces.objects.semantic_manifest import SemanticManifest
-from dbt_semantic_interfaces.transformations.transform_rule import ModelTransformRule
 
 logger = logging.getLogger(__name__)
 
 
-class CreateProxyMeasureRule(ModelTransformRule):
+class CreateProxyMeasureRule(ProtocolHint[SemanticManifestTransformRule[PydanticSemanticManifest]]):
     """Adds a proxy metric for measures that have the create_metric flag set, if it does not already exist.
 
     Also checks that a defined metric with the same name as a measure is a proxy metric.
     """
 
+    @override
+    def _implements_protocol(self) -> SemanticManifestTransformRule[PydanticSemanticManifest]:  # noqa: D
+        return self
+
     @staticmethod
-    def transform_model(model: SemanticManifest) -> SemanticManifest:
+    def transform_model(model: PydanticSemanticManifest) -> PydanticSemanticManifest:
         """Creates measure proxy metrics for measures with `create_metric==True`."""
         for semantic_model in model.semantic_models:
             for measure in semantic_model.measures:
                 if not measure.create_metric:
                     continue
 
                 add_metric = True
                 for metric in model.metrics:
                     if metric.name == measure.name:
-                        if metric.type != MetricType.MEASURE_PROXY:
+                        if metric.type != MetricType.SIMPLE:
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
                     model.metrics.append(
-                        Metric(
+                        PydanticMetric(
                             name=measure.name,
-                            type=MetricType.MEASURE_PROXY,
-                            type_params=MetricTypeParams(
-                                measures=[MetricInputMeasure(name=measure.name)],
+                            type=MetricType.SIMPLE,
+                            type_params=PydanticMetricTypeParams(
+                                measures=[PydanticMetricInputMeasure(name=measure.name)],
                                 expr=measure.name,
                             ),
                         )
                     )
 
         return model
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/type_enums/time_granularity.py` & `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/type_enums/time_granularity.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/validations/agg_time_dimension.py` & `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/validations/agg_time_dimension.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-from typing import List
+from typing import Generic, List, Sequence
 
-from dbt_semantic_interfaces.objects.semantic_manifest import SemanticManifest
-from dbt_semantic_interfaces.objects.semantic_model import SemanticModel
+from dbt_semantic_interfaces.protocols.semantic_manifest import SemanticManifestT
+from dbt_semantic_interfaces.protocols.semantic_model import SemanticModel
 from dbt_semantic_interfaces.references import (
     SemanticModelElementReference,
     TimeDimensionReference,
 )
 from dbt_semantic_interfaces.type_enums.dimension_type import DimensionType
 from dbt_semantic_interfaces.validations.validator_helpers import (
     FileContext,
-    ModelValidationRule,
+    SemanticManifestValidationRule,
     SemanticModelElementContext,
     SemanticModelElementType,
     ValidationError,
     ValidationIssue,
     validate_safely,
 )
 
 
-class AggregationTimeDimensionRule(ModelValidationRule):
+class AggregationTimeDimensionRule(SemanticManifestValidationRule[SemanticManifestT], Generic[SemanticManifestT]):
     """Checks that the agg time dimension for a measure points to a valid time dimension in the semantic model."""
 
     @staticmethod
     @validate_safely(whats_being_done="checking aggregation time dimension for semantic models in the model")
-    def validate_model(model: SemanticManifest) -> List[ValidationIssue]:  # noqa: D
+    def validate_manifest(semantic_manifest: SemanticManifestT) -> Sequence[ValidationIssue]:  # noqa: D
         issues: List[ValidationIssue] = []
-        for semantic_model in model.semantic_models:
+        for semantic_model in semantic_manifest.semantic_models:
             issues.extend(AggregationTimeDimensionRule._validate_semantic_model(semantic_model))
 
         return issues
 
     @staticmethod
     def _time_dimension_in_model(
         time_dimension_reference: TimeDimensionReference, semantic_model: SemanticModel
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/validations/common_entities.py` & `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/validations/common_entities.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-from typing import Dict, List, Set
+from typing import Dict, Generic, List, Sequence, Set
 
-from dbt_semantic_interfaces.objects.elements.entity import Entity
-from dbt_semantic_interfaces.objects.semantic_manifest import SemanticManifest
-from dbt_semantic_interfaces.objects.semantic_model import SemanticModel
+from dbt_semantic_interfaces.protocols.entity import Entity
+from dbt_semantic_interfaces.protocols.semantic_manifest import SemanticManifestT
+from dbt_semantic_interfaces.protocols.semantic_model import SemanticModel
 from dbt_semantic_interfaces.references import (
     EntityReference,
     SemanticModelElementReference,
 )
 from dbt_semantic_interfaces.validations.validator_helpers import (
     FileContext,
-    ModelValidationRule,
+    SemanticManifestValidationRule,
     SemanticModelElementContext,
     SemanticModelElementType,
     ValidationIssue,
     ValidationWarning,
     validate_safely,
 )
 
 
-class CommonEntitysRule(ModelValidationRule):
+class CommonEntitysRule(SemanticManifestValidationRule[SemanticManifestT], Generic[SemanticManifestT]):
     """Checks that entities exist on more than one semantic model."""
 
     @staticmethod
-    def _map_semantic_model_entities(semantic_models: List[SemanticModel]) -> Dict[EntityReference, Set[str]]:
+    def _map_semantic_model_entities(semantic_models: Sequence[SemanticModel]) -> Dict[EntityReference, Set[str]]:
         """Generate mapping of entity names to the set of semantic_models where it is defined."""
         entities_to_semantic_models: Dict[EntityReference, Set[str]] = {}
         for semantic_model in semantic_models or []:
             for entity in semantic_model.entities or []:
                 if entity.reference in entities_to_semantic_models:
                     entities_to_semantic_models[entity.reference].add(semantic_model.name)
                 else:
@@ -61,20 +61,20 @@
                     f"which means it will be unused in joins.",
                 )
             )
         return issues
 
     @staticmethod
     @validate_safely(whats_being_done="running model validation warning if entities are only one one semantic model")
-    def validate_model(model: SemanticManifest) -> List[ValidationIssue]:
+    def validate_manifest(semantic_manifest: SemanticManifestT) -> Sequence[ValidationIssue]:
         """Issues a warning for any entity that is associated with only one semantic_model."""
         issues = []
 
-        entities_to_semantic_models = CommonEntitysRule._map_semantic_model_entities(model.semantic_models)
-        for semantic_model in model.semantic_models or []:
+        entities_to_semantic_models = CommonEntitysRule._map_semantic_model_entities(semantic_manifest.semantic_models)
+        for semantic_model in semantic_manifest.semantic_models or []:
             for entity in semantic_model.entities or []:
                 issues += CommonEntitysRule._check_entity(
                     entity=entity,
                     semantic_model=semantic_model,
                     entities_to_semantic_models=entities_to_semantic_models,
                 )
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/validations/dimension_const.py` & `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/validations/dimension_const.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-from typing import Dict, List
+from typing import Dict, Generic, List, Sequence
 
-from dbt_semantic_interfaces.objects.elements.dimension import Dimension
-from dbt_semantic_interfaces.objects.semantic_manifest import SemanticManifest
-from dbt_semantic_interfaces.objects.semantic_model import SemanticModel
+from dbt_semantic_interfaces.protocols.dimension import Dimension
+from dbt_semantic_interfaces.protocols.semantic_manifest import SemanticManifestT
+from dbt_semantic_interfaces.protocols.semantic_model import SemanticModel
 from dbt_semantic_interfaces.references import (
     DimensionReference,
     SemanticModelElementReference,
 )
 from dbt_semantic_interfaces.type_enums.dimension_type import DimensionType
 from dbt_semantic_interfaces.type_enums.time_granularity import TimeGranularity
 from dbt_semantic_interfaces.validations.validator_helpers import (
     DimensionInvariants,
     FileContext,
-    ModelValidationRule,
+    SemanticManifestValidationRule,
     SemanticModelElementContext,
     SemanticModelElementType,
     ValidationError,
     ValidationIssue,
     validate_safely,
 )
 
 
-class DimensionConsistencyRule(ModelValidationRule):
+class DimensionConsistencyRule(SemanticManifestValidationRule[SemanticManifestT], Generic[SemanticManifestT]):
     """Checks for consistent dimension properties in the semantic models in a model.
 
     * Dimensions with the same name should be of the same type.
     * Dimensions with the same name should be either all partitions or not.
     """
 
     @staticmethod
     @validate_safely(whats_being_done="running model validation ensuring dimension consistency")
-    def validate_model(model: SemanticManifest) -> List[ValidationIssue]:  # noqa: D
+    def validate_manifest(semantic_manifest: SemanticManifestT) -> Sequence[ValidationIssue]:  # noqa: D
         dimension_to_invariant: Dict[DimensionReference, DimensionInvariants] = {}
         time_dims_to_granularity: Dict[DimensionReference, TimeGranularity] = {}
         issues: List[ValidationIssue] = []
 
-        for semantic_model in model.semantic_models:
+        for semantic_model in semantic_manifest.semantic_models:
             issues += DimensionConsistencyRule._validate_semantic_model(
                 semantic_model=semantic_model, dimension_to_invariant=dimension_to_invariant, update_invariant_dict=True
             )
 
             for dimension in semantic_model.dimensions:
                 issues += DimensionConsistencyRule._validate_dimension(
                     dimension=dimension,
@@ -75,18 +75,16 @@
             element_type=SemanticModelElementType.DIMENSION,
         )
 
         if dimension.type == DimensionType.TIME:
             if dimension.reference not in time_dims_to_granularity and dimension.type_params:
                 time_dims_to_granularity[dimension.reference] = dimension.type_params.time_granularity
 
-                # The primary time dimension can be of different time granularities, so don't check for it.
                 if (
                     dimension.type_params is not None
-                    and not dimension.type_params.is_primary
                     and dimension.type_params.time_granularity != time_dims_to_granularity[dimension.reference]
                 ):
                     expected_granularity = time_dims_to_granularity[dimension.reference]
                     issues.append(
                         ValidationError(
                             context=context,
                             message=f"Time granularity must be the same for time dimensions with the same name. "
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/validations/element_const.py` & `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/validations/element_const.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 from collections import defaultdict
-from typing import DefaultDict, List
+from typing import DefaultDict, Generic, List, Sequence
 
-from dbt_semantic_interfaces.objects.semantic_manifest import SemanticManifest
+from dbt_semantic_interfaces.implementations.semantic_manifest import (
+    PydanticSemanticManifest,
+)
+from dbt_semantic_interfaces.protocols.semantic_manifest import SemanticManifestT
 from dbt_semantic_interfaces.references import SemanticModelReference
 from dbt_semantic_interfaces.validations.validator_helpers import (
     FileContext,
-    ModelValidationRule,
+    SemanticManifestValidationRule,
     SemanticModelContext,
     SemanticModelElementType,
     ValidationError,
     ValidationIssue,
     validate_safely,
 )
 
 
-class ElementConsistencyRule(ModelValidationRule):
+class ElementConsistencyRule(SemanticManifestValidationRule[SemanticManifestT], Generic[SemanticManifestT]):
     """Checks that elements in semantic models with the same name are of the same element type across the model.
 
     This reduces the potential confusion that might arise from having an entity named `country` and a dimension
     named `country` while allowing for things like the `user` entity to exist in multiple semantic models. Note not
     all element types allow duplicates, and there are separate validation rules for those cases. See, for example,
     the SemanticModelMeasuresUniqueRule.
     """
 
     @staticmethod
     @validate_safely(whats_being_done="running model validation ensuring model wide element consistency")
-    def validate_model(model: SemanticManifest) -> List[ValidationIssue]:  # noqa: D
+    def validate_manifest(semantic_manifest: PydanticSemanticManifest) -> Sequence[ValidationIssue]:  # noqa: D
         issues = []
-        element_name_to_types = ElementConsistencyRule._get_element_name_to_types(model=model)
+        element_name_to_types = ElementConsistencyRule._get_element_name_to_types(model=semantic_manifest)
         invalid_elements = {
             name: type_mapping for name, type_mapping in element_name_to_types.items() if len(type_mapping) > 1
         }
 
         for element_name, type_to_context in invalid_elements.items():
             # Sort these by value to ensure consistent error messaging
             types_used = [SemanticModelElementType(v) for v in sorted(k.value for k in type_to_context.keys())]
@@ -47,15 +50,15 @@
                     )
                 )
 
         return issues
 
     @staticmethod
     def _get_element_name_to_types(
-        model: SemanticManifest,
+        model: PydanticSemanticManifest,
     ) -> DefaultDict[str, DefaultDict[SemanticModelElementType, List[SemanticModelContext]]]:
         """Create a mapping of element names in the semantic manifest to types with a list of associated contexts."""
         element_types: DefaultDict[
             str, DefaultDict[SemanticModelElementType, List[SemanticModelContext]]
         ] = defaultdict(lambda: defaultdict(list))
         for semantic_model in model.semantic_models:
             semantic_model_context = SemanticModelContext(
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/validations/entities.py` & `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/validations/entities.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import logging
 from datetime import date
-from typing import List, MutableSet
+from typing import Generic, List, MutableSet, Sequence
 
-from dbt_semantic_interfaces.objects.semantic_manifest import SemanticManifest
-from dbt_semantic_interfaces.objects.semantic_model import SemanticModel
+from dbt_semantic_interfaces.protocols.semantic_manifest import SemanticManifestT
+from dbt_semantic_interfaces.protocols.semantic_model import SemanticModel
 from dbt_semantic_interfaces.references import SemanticModelReference
 from dbt_semantic_interfaces.type_enums.entity_type import EntityType
 from dbt_semantic_interfaces.validations.validator_helpers import (
     FileContext,
-    ModelValidationRule,
+    SemanticManifestValidationRule,
     SemanticModelContext,
     ValidationError,
     ValidationFutureError,
     ValidationIssue,
     validate_safely,
 )
 
 logger = logging.getLogger(__name__)
 
 
-class NaturalEntityConfigurationRule(ModelValidationRule):
+class NaturalEntityConfigurationRule(SemanticManifestValidationRule[SemanticManifestT], Generic[SemanticManifestT]):
     """Ensures that entities marked as EntityType.NATURAL are configured correctly."""
 
     @staticmethod
     @validate_safely(
         whats_being_done=(
             "checking that each semantic model has no more than one natural entity, and that "
             "natural entities are used in the appropriate contexts"
@@ -57,26 +57,28 @@
             )
             issues.append(error)
 
         return issues
 
     @staticmethod
     @validate_safely(whats_being_done="checking that entities marked as EntityType.NATURAL are properly configured")
-    def validate_model(model: SemanticManifest) -> List[ValidationIssue]:
+    def validate_manifest(semantic_manifest: SemanticManifestT) -> Sequence[ValidationIssue]:
         """Validate entities marked as EntityType.NATURAL."""
         issues: List[ValidationIssue] = []
-        for semantic_model in model.semantic_models:
+        for semantic_model in semantic_manifest.semantic_models:
             issues += NaturalEntityConfigurationRule._validate_semantic_model_natural_entities(
                 semantic_model=semantic_model
             )
 
         return issues
 
 
-class OnePrimaryEntityPerSemanticModelRule(ModelValidationRule):
+class OnePrimaryEntityPerSemanticModelRule(
+    SemanticManifestValidationRule[SemanticManifestT], Generic[SemanticManifestT]
+):
     """Ensures that each semantic model has only one primary entity."""
 
     @staticmethod
     @validate_safely(whats_being_done="checking semantic model has only one primary entity")
     def _only_one_primary_entity(semantic_model: SemanticModel) -> List[ValidationIssue]:
         primary_entity_names: MutableSet[str] = set()
         for entity in semantic_model.entities or []:
@@ -97,14 +99,14 @@
             ]
         return []
 
     @staticmethod
     @validate_safely(
         whats_being_done="running model validation ensuring each semantic model has only one primary entity"
     )
-    def validate_model(model: SemanticManifest) -> List[ValidationIssue]:  # noqa: D
+    def validate_manifest(semantic_manifest: SemanticManifestT) -> Sequence[ValidationIssue]:  # noqa: D
         issues = []
 
-        for semantic_model in model.semantic_models:
+        for semantic_model in semantic_manifest.semantic_models:
             issues += OnePrimaryEntityPerSemanticModelRule._only_one_primary_entity(semantic_model=semantic_model)
 
         return issues
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/validations/measures.py` & `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/validations/measures.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 from collections import defaultdict
-from typing import DefaultDict, Dict, List, Set
+from typing import DefaultDict, Dict, Generic, List, Sequence, Set
 
 from more_itertools import bucket
 
-from dbt_semantic_interfaces.objects.metric import Metric
-from dbt_semantic_interfaces.objects.semantic_manifest import SemanticManifest
+from dbt_semantic_interfaces.protocols.metric import Metric
+from dbt_semantic_interfaces.protocols.semantic_manifest import (
+    SemanticManifest,
+    SemanticManifestT,
+)
 from dbt_semantic_interfaces.references import MeasureReference, MetricModelReference
 from dbt_semantic_interfaces.type_enums.aggregation_type import AggregationType
 from dbt_semantic_interfaces.type_enums.dimension_type import DimensionType
 from dbt_semantic_interfaces.validations.unique_valid_name import UniqueAndValidNameRule
 from dbt_semantic_interfaces.validations.validator_helpers import (
     FileContext,
     MetricContext,
-    ModelValidationRule,
+    SemanticManifestValidationRule,
     SemanticModelElementContext,
     SemanticModelElementReference,
     SemanticModelElementType,
     ValidationError,
     ValidationIssue,
     ValidationWarning,
     validate_safely,
 )
 
 
-class SemanticModelMeasuresUniqueRule(ModelValidationRule):
+class SemanticModelMeasuresUniqueRule(SemanticManifestValidationRule[SemanticManifestT], Generic[SemanticManifestT]):
     """Asserts all measure names are unique across the model."""
 
     @staticmethod
     @validate_safely(
         whats_being_done="running model validation ensuring measures exist in only one configured semantic model"
     )
-    def validate_model(model: SemanticManifest) -> List[ValidationIssue]:  # noqa: D
+    def validate_manifest(semantic_manifest: SemanticManifestT) -> Sequence[ValidationIssue]:  # noqa: D
         issues: List[ValidationIssue] = []
 
         measure_references_to_semantic_models: Dict[MeasureReference, List] = defaultdict(list)
-        for semantic_model in model.semantic_models:
+        for semantic_model in semantic_manifest.semantic_models:
             for measure in semantic_model.measures:
                 if measure.reference in measure_references_to_semantic_models:
                     issues.append(
                         ValidationError(
                             context=SemanticModelElementContext(
                                 file_context=FileContext.from_metadata(metadata=semantic_model.metadata),
                                 semantic_model_element=SemanticModelElementReference(
@@ -51,18 +54,18 @@
                         )
                     )
                 measure_references_to_semantic_models[measure.reference].append(semantic_model.name)
 
         return issues
 
 
-class MeasureConstraintAliasesRule(ModelValidationRule):
+class MeasureConstraintAliasesRule(SemanticManifestValidationRule[SemanticManifestT], Generic[SemanticManifestT]):
     """Checks that aliases are configured correctly for constrained measure references.
 
-    These are, currently, only applicable for Metric types, since the MetricInputMeasure is only
+    These are, currently, only applicable for PydanticMetric types, since the MetricInputMeasure is only
     """
 
     @staticmethod
     @validate_safely(whats_being_done="ensuring measures aliases are set when required")
     def _validate_required_aliases_are_set(metric: Metric, metric_context: MetricContext) -> List[ValidationIssue]:
         """Checks if valid aliases are set on the input measure references where they are required.
 
@@ -92,52 +95,53 @@
             if len(distinct_input_measures) == 1:
                 # Warn whenever multiple identical references exist - we will consolidate these but it might be
                 # a meaningful oversight if constraints and aliases are specified
                 issues.append(
                     ValidationWarning(
                         context=metric_context,
                         message=(
-                            f"Metric {metric.name} has multiple identical input measures specifications for measure "
-                            f"{name}. This might be hiding a semantic error. Input measure specification: "
+                            f"PydanticMetric {metric.name} has multiple identical input measures specifications for "
+                            f"measure {name}. This might be hiding a semantic error. Input measure specification: "
                             f"{input_measures[0]}."
                         ),
                     )
                 )
                 continue
 
             constrained_measures_without_aliases = [
                 measure for measure in input_measures if measure.filter is not None and measure.alias is None
             ]
             if constrained_measures_without_aliases:
                 issues.append(
                     ValidationError(
                         context=metric_context,
                         message=(
-                            f"Metric {metric.name} depends on multiple different constrained versions of measure "
-                            f"{name}. In such cases, aliases must be provided, but the following input measures have "
-                            f"constraints specified without an alias: {constrained_measures_without_aliases}."
+                            f"PydanticMetric {metric.name} depends on multiple different constrained versions of "
+                            f"measure {name}. In such cases, aliases must be provided, but the following input "
+                            f"measures have constraints specified without an alias: "
+                            f"{constrained_measures_without_aliases}."
                         ),
                     )
                 )
 
         return issues
 
     @staticmethod
     @validate_safely(whats_being_done="checking constrained measures are aliased properly")
-    def validate_model(model: SemanticManifest) -> List[ValidationIssue]:
+    def validate_manifest(semantic_manifest: SemanticManifestT) -> Sequence[ValidationIssue]:
         """Ensures measures that might need an alias have one set, and that the alias is distinct.
 
         We do not allow aliases to collide with other alias or measure names, since that could create
         ambiguity at query time or cause issues if users ever restructure their models.
         """
         issues: List[ValidationIssue] = []
 
-        measure_names = _get_measure_names_from_model(model)
+        measure_names = _get_measure_names_from_model(semantic_manifest)
         measure_alias_to_metrics: DefaultDict[str, List[str]] = defaultdict(list)
-        for metric in model.metrics:
+        for metric in semantic_manifest.metrics:
             metric_context = MetricContext(
                 file_context=FileContext.from_metadata(metadata=metric.metadata),
                 metric=MetricModelReference(metric_name=metric.name),
             )
 
             issues += MeasureConstraintAliasesRule._validate_required_aliases_are_set(
                 metric=metric, metric_context=metric_context
@@ -176,15 +180,15 @@
                     )
 
                 measure_alias_to_metrics[measure.alias].append(metric.name)
 
         return issues
 
 
-class MetricMeasuresRule(ModelValidationRule):
+class MetricMeasuresRule(SemanticManifestValidationRule[SemanticManifestT], Generic[SemanticManifestT]):
     """Checks that the measures referenced in the metrics exist."""
 
     @staticmethod
     @validate_safely(whats_being_done="checking all measures referenced by the metric exist")
     def _validate_metric_measure_references(metric: Metric, valid_measure_names: Set[str]) -> List[ValidationIssue]:
         issues: List[ValidationIssue] = []
 
@@ -202,33 +206,33 @@
                         ),
                     )
                 )
         return issues
 
     @staticmethod
     @validate_safely(whats_being_done="running model validation ensuring metric measures exist")
-    def validate_model(model: SemanticManifest) -> List[ValidationIssue]:  # noqa: D
+    def validate_manifest(semantic_manifest: SemanticManifestT) -> Sequence[ValidationIssue]:  # noqa: D
         issues: List[ValidationIssue] = []
-        valid_measure_names = _get_measure_names_from_model(model)
+        valid_measure_names = _get_measure_names_from_model(semantic_manifest)
 
-        for metric in model.metrics or []:
+        for metric in semantic_manifest.metrics or []:
             issues += MetricMeasuresRule._validate_metric_measure_references(
                 metric=metric, valid_measure_names=valid_measure_names
             )
         return issues
 
 
-class MeasuresNonAdditiveDimensionRule(ModelValidationRule):
+class MeasuresNonAdditiveDimensionRule(SemanticManifestValidationRule[SemanticManifestT], Generic[SemanticManifestT]):
     """Checks that the measure's non_additive_dimensions are properly defined."""
 
     @staticmethod
     @validate_safely(whats_being_done="ensuring that a measure's non_additive_dimensions is valid")
-    def validate_model(model: SemanticManifest) -> List[ValidationIssue]:  # noqa: D
+    def validate_manifest(semantic_manifest: SemanticManifestT) -> Sequence[ValidationIssue]:  # noqa: D
         issues: List[ValidationIssue] = []
-        for semantic_model in model.semantic_models or []:
+        for semantic_model in semantic_manifest.semantic_models or []:
             for measure in semantic_model.measures:
                 non_additive_dimension = measure.non_additive_dimension
                 if non_additive_dimension is None:
                     continue
                 agg_time_dimension = next(
                     (
                         dim
@@ -246,16 +250,16 @@
                                 semantic_model_element=SemanticModelElementReference(
                                     semantic_model_name=semantic_model.name, element_name=measure.name
                                 ),
                                 element_type=SemanticModelElementType.MEASURE,
                             ),
                             message=(
                                 f"Measure '{measure.name}' has a agg_time_dimension of "
-                                f"{measure.checked_agg_time_dimension.element_name} ",
-                                f"that is not defined as a dimension in semantic model '{semantic_model.name}'.",
+                                f"{measure.checked_agg_time_dimension.element_name} "
+                                f"that is not defined as a dimension in semantic model '{semantic_model.name}'."
                             ),
                         )
                     )
                     continue
 
                 # Validates that the non_additive_dimension exists as a time dimension in the semantic model
                 matching_dimension = next(
@@ -368,25 +372,25 @@
                             ),
                         )
                     )
 
         return issues
 
 
-class CountAggregationExprRule(ModelValidationRule):
+class CountAggregationExprRule(SemanticManifestValidationRule[SemanticManifestT], Generic[SemanticManifestT]):
     """Checks that COUNT measures have an expr provided."""
 
     @staticmethod
     @validate_safely(
         whats_being_done="running model validation ensuring expr exist for measures with count aggregation"
     )
-    def validate_model(model: SemanticManifest) -> List[ValidationIssue]:  # noqa: D
+    def validate_manifest(semantic_manifest: SemanticManifestT) -> Sequence[ValidationIssue]:  # noqa: D
         issues: List[ValidationIssue] = []
 
-        for semantic_model in model.semantic_models:
+        for semantic_model in semantic_manifest.semantic_models:
             for measure in semantic_model.measures:
                 context = SemanticModelElementContext(
                     file_context=FileContext.from_metadata(metadata=semantic_model.metadata),
                     semantic_model_element=SemanticModelElementReference(
                         semantic_model_name=semantic_model.name, element_name=measure.name
                     ),
                     element_type=SemanticModelElementType.MEASURE,
@@ -419,26 +423,26 @@
                                 f"incorrect results. Please use the {measure.agg.value}_distinct aggregation type."
                             ),
                         )
                     )
         return issues
 
 
-class PercentileAggregationRule(ModelValidationRule):
+class PercentileAggregationRule(SemanticManifestValidationRule[SemanticManifestT], Generic[SemanticManifestT]):
     """Checks that only PERCENTILE measures have agg_params and valid percentile value provided."""
 
     @staticmethod
     @validate_safely(
         whats_being_done="running model validation ensuring the agg_params.percentile value exist for measures with "
         "percentile aggregation"
     )
-    def validate_model(model: SemanticManifest) -> List[ValidationIssue]:  # noqa: D
+    def validate_manifest(semantic_manifest: SemanticManifestT) -> Sequence[ValidationIssue]:  # noqa: D
         issues: List[ValidationIssue] = []
 
-        for semantic_model in model.semantic_models:
+        for semantic_model in semantic_manifest.semantic_models:
             for measure in semantic_model.measures:
                 context = SemanticModelElementContext(
                     file_context=FileContext.from_metadata(metadata=semantic_model.metadata),
                     semantic_model_element=SemanticModelElementReference(
                         semantic_model_name=semantic_model.name, element_name=measure.name
                     ),
                     element_type=SemanticModelElementType.MEASURE,
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/validations/metrics.py` & `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/validations/metrics.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 import traceback
-from typing import List
+from typing import Generic, List, Sequence
 
 from dbt_semantic_interfaces.errors import ParsingException
-from dbt_semantic_interfaces.objects.metric import Metric, MetricTimeWindow, MetricType
-from dbt_semantic_interfaces.objects.semantic_manifest import SemanticManifest
+from dbt_semantic_interfaces.implementations.metric import PydanticMetricTimeWindow
+from dbt_semantic_interfaces.protocols.metric import Metric, MetricType
+from dbt_semantic_interfaces.protocols.semantic_manifest import (
+    SemanticManifest,
+    SemanticManifestT,
+)
 from dbt_semantic_interfaces.references import MetricModelReference
 from dbt_semantic_interfaces.validations.unique_valid_name import UniqueAndValidNameRule
 from dbt_semantic_interfaces.validations.validator_helpers import (
     FileContext,
     MetricContext,
-    ModelValidationRule,
+    SemanticManifestValidationRule,
     ValidationError,
     ValidationIssue,
     validate_safely,
 )
 
 
-class CumulativeMetricRule(ModelValidationRule):
+class CumulativeMetricRule(SemanticManifestValidationRule[SemanticManifestT], Generic[SemanticManifestT]):
     """Checks that cumulative sum metrics are configured properly."""
 
     @staticmethod
     @validate_safely(whats_being_done="checking that the params of metric are valid if it is a cumulative sum metric")
     def _validate_cumulative_sum_metric_params(metric: Metric) -> List[ValidationIssue]:
         issues: List[ValidationIssue] = []
 
@@ -34,15 +38,17 @@
                         ),
                         message="Both window and grain_to_date set for cumulative metric. Please set one or the other",
                     )
                 )
 
             if metric.type_params.window:
                 try:
-                    MetricTimeWindow.parse(metric.type_params.window.to_string())
+                    window_str = f"{metric.type_params.window.count} {metric.type_params.window.granularity.value}"
+                    # TODO: Should not call an implementation class.
+                    PydanticMetricTimeWindow.parse(window_str)
                 except ParsingException as e:
                     issues.append(
                         ValidationError(
                             context=MetricContext(
                                 file_context=FileContext.from_metadata(metadata=metric.metadata),
                                 metric=MetricModelReference(metric_name=metric.name),
                             ),
@@ -51,24 +57,24 @@
                         )
                     )
 
         return issues
 
     @staticmethod
     @validate_safely(whats_being_done="running model validation ensuring cumulative sum metrics are valid")
-    def validate_model(model: SemanticManifest) -> List[ValidationIssue]:  # noqa: D
+    def validate_manifest(semantic_manifest: SemanticManifestT) -> Sequence[ValidationIssue]:  # noqa: D
         issues: List[ValidationIssue] = []
 
-        for metric in model.metrics or []:
+        for metric in semantic_manifest.metrics or []:
             issues += CumulativeMetricRule._validate_cumulative_sum_metric_params(metric=metric)
 
         return issues
 
 
-class DerivedMetricRule(ModelValidationRule):
+class DerivedMetricRule(SemanticManifestValidationRule[SemanticManifestT], Generic[SemanticManifestT]):
     """Checks that derived metrics are configured properly."""
 
     @staticmethod
     @validate_safely(whats_being_done="checking that the alias set are not unique and distinct")
     def _validate_alias_collision(metric: Metric) -> List[ValidationIssue]:
         issues: List[ValidationIssue] = []
 
@@ -134,15 +140,15 @@
 
         return issues
 
     @staticmethod
     @validate_safely(
         whats_being_done="running model validation ensuring derived metrics properties are configured properly"
     )
-    def validate_model(model: SemanticManifest) -> List[ValidationIssue]:  # noqa: D
+    def validate_manifest(semantic_manifest: SemanticManifestT) -> Sequence[ValidationIssue]:  # noqa: D
         issues: List[ValidationIssue] = []
 
-        issues += DerivedMetricRule._validate_input_metrics_exist(model=model)
-        for metric in model.metrics or []:
+        issues += DerivedMetricRule._validate_input_metrics_exist(model=semantic_manifest)
+        for metric in semantic_manifest.metrics or []:
             issues += DerivedMetricRule._validate_alias_collision(metric=metric)
             issues += DerivedMetricRule._validate_time_offset_params(metric=metric)
         return issues
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/validations/non_empty.py` & `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/validations/non_empty.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,39 @@
-from typing import List
+from typing import Generic, List, Sequence
 
-from dbt_semantic_interfaces.objects.semantic_manifest import SemanticManifest
+from dbt_semantic_interfaces.implementations.semantic_manifest import (
+    PydanticSemanticManifest,
+)
+from dbt_semantic_interfaces.protocols.semantic_manifest import SemanticManifestT
 from dbt_semantic_interfaces.validations.validator_helpers import (
-    ModelValidationRule,
+    SemanticManifestValidationRule,
     ValidationError,
     ValidationIssue,
     validate_safely,
 )
 
 
-class NonEmptyRule(ModelValidationRule):
+class NonEmptyRule(SemanticManifestValidationRule[SemanticManifestT], Generic[SemanticManifestT]):
     """Check if the model contains semantic models and metrics."""
 
     @staticmethod
     @validate_safely(whats_being_done="checking that the model has semantic models")
-    def _check_model_has_semantic_models(model: SemanticManifest) -> List[ValidationIssue]:
+    def _check_model_has_semantic_models(model: PydanticSemanticManifest) -> List[ValidationIssue]:
         issues: List[ValidationIssue] = []
         if not model.semantic_models:
             issues.append(
                 ValidationError(
                     message="No semantic models present in the model.",
                 )
             )
         return issues
 
     @staticmethod
     @validate_safely(whats_being_done="checking that the model has metrics")
-    def _check_model_has_metrics(model: SemanticManifest) -> List[ValidationIssue]:
+    def _check_model_has_metrics(model: PydanticSemanticManifest) -> List[ValidationIssue]:
         issues: List[ValidationIssue] = []
 
         # If we are going to generate measure proxy metrics that is sufficient as well
         create_measure_proxy_metrics = False
         for semantic_model in model.semantic_models:
             for measure in semantic_model.measures:
                 if measure.create_metric is True:
@@ -43,12 +46,12 @@
                     message="No metrics present in the model.",
                 )
             )
         return issues
 
     @staticmethod
     @validate_safely("running model validation rule ensuring metrics and semantic models are defined")
-    def validate_model(model: SemanticManifest) -> List[ValidationIssue]:  # noqa: D
+    def validate_manifest(semantic_manifest: PydanticSemanticManifest) -> Sequence[ValidationIssue]:  # noqa: D
         issues: List[ValidationIssue] = []
-        issues += NonEmptyRule._check_model_has_semantic_models(model=model)
-        issues += NonEmptyRule._check_model_has_metrics(model=model)
+        issues += NonEmptyRule._check_model_has_semantic_models(model=semantic_manifest)
+        issues += NonEmptyRule._check_model_has_metrics(model=semantic_manifest)
         return issues
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/validations/reserved_keywords.py` & `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/validations/reserved_keywords.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,27 @@
-from typing import List
+from typing import Generic, List
 
-from dbt_semantic_interfaces.objects.semantic_manifest import SemanticManifest
-from dbt_semantic_interfaces.objects.semantic_model import SemanticModel
+from dbt_semantic_interfaces.protocols.semantic_manifest import (
+    SemanticManifest,
+    SemanticManifestT,
+)
+from dbt_semantic_interfaces.protocols.semantic_model import SemanticModel
 from dbt_semantic_interfaces.references import SemanticModelElementReference
 from dbt_semantic_interfaces.validations.validator_helpers import (
     FileContext,
-    ModelValidationRule,
+    SemanticManifestValidationRule,
     SemanticModelContext,
     SemanticModelElementContext,
     SemanticModelElementType,
     ValidationError,
     ValidationIssue,
     validate_safely,
 )
 
-# A non-exaustive tuple of reserved keywords
+# A non-exhaustive tuple of reserved keywords
 # This list was created by running an intersection of keywords for redshift,
 # postgres, bigquery, and snowflake
 RESERVED_KEYWORDS = (
     "AND",
     "AS",
     "CREATE",
     "DISTINCT",
@@ -43,15 +46,15 @@
     "UNION",
     "USING",
     "WHERE",
     "WITH",
 )
 
 
-class ReservedKeywordsRule(ModelValidationRule):
+class ReservedKeywordsRule(SemanticManifestValidationRule[SemanticManifestT], Generic[SemanticManifestT]):
     """Check that any element that ends up being selected by name (instead of expr) isn't a commonly reserved keyword.
 
     Note: This rule DOES NOT catch all keywords. That is because keywords are
     engine specific, and semantic validations are not engine specific. I.e. if
     you change your underlying data warehouse engine, semantic validations
     should still pass, but your data warehouse validations might fail. However,
     data warehouse validations are slow in comparison to semantic validation
@@ -149,9 +152,9 @@
         return issues
 
     @classmethod
     @validate_safely(
         whats_being_done="running model validation ensuring elements that aren't selected via a defined expr don't "
         "contain reserved keywords"
     )
-    def validate_model(cls, model: SemanticManifest) -> List[ValidationIssue]:  # noqa: D
-        return cls._validate_semantic_models(model=model)
+    def validate_manifest(cls, semantic_manifest: SemanticManifest) -> List[ValidationIssue]:  # noqa: D
+        return cls._validate_semantic_models(model=semantic_manifest)
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/validations/semantic_models.py` & `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/validations/semantic_models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,97 +1,73 @@
 import logging
-from typing import List
+from typing import Generic, List, Sequence
 
-from dbt_semantic_interfaces.objects.semantic_manifest import SemanticManifest
-from dbt_semantic_interfaces.objects.semantic_model import SemanticModel
+from dbt_semantic_interfaces.protocols.semantic_manifest import SemanticManifestT
+from dbt_semantic_interfaces.protocols.semantic_model import SemanticModel
 from dbt_semantic_interfaces.references import SemanticModelReference
-from dbt_semantic_interfaces.type_enums.dimension_type import DimensionType
 from dbt_semantic_interfaces.type_enums.entity_type import EntityType
 from dbt_semantic_interfaces.validations.validator_helpers import (
     FileContext,
-    ModelValidationRule,
+    SemanticManifestValidationRule,
     SemanticModelContext,
     ValidationError,
     ValidationIssue,
     validate_safely,
 )
 
 logger = logging.getLogger(__name__)
 
 
-class SemanticModelTimeDimensionWarningsRule(ModelValidationRule):
+class SemanticModelTimeDimensionWarningsRule(
+    SemanticManifestValidationRule[SemanticManifestT], Generic[SemanticManifestT]
+):
     """Checks time dimensions in semantic models."""
 
     @staticmethod
     @validate_safely(whats_being_done="running model validation ensuring time dimensions are defined properly")
-    def validate_model(model: SemanticManifest) -> List[ValidationIssue]:  # noqa: D
+    def validate_manifest(semantic_manifest: SemanticManifestT) -> Sequence[ValidationIssue]:  # noqa: D
         issues: List[ValidationIssue] = []
 
-        for semantic_model in model.semantic_models:
+        for semantic_model in semantic_manifest.semantic_models:
             issues.extend(
                 SemanticModelTimeDimensionWarningsRule._validate_semantic_model(semantic_model=semantic_model)
             )
         return issues
 
     @staticmethod
     @validate_safely(whats_being_done="checking validity of the semantic model's time dimensions")
     def _validate_semantic_model(semantic_model: SemanticModel) -> List[ValidationIssue]:
         issues: List[ValidationIssue] = []
 
-        primary_time_dimensions = []
-
-        for dim in semantic_model.dimensions:
-            if dim.type == DimensionType.TIME and dim.type_params is not None and dim.type_params.is_primary:
-                primary_time_dimensions.append(dim)
-
-        # A semantic model must have a primary time dimension if it has
-        # any measures that don't have an `agg_time_dimension` set
-        if (
-            len(primary_time_dimensions) == 0
-            and len(semantic_model.measures) > 0
-            and any(measure.agg_time_dimension is None for measure in semantic_model.measures)
-        ):
-            issues.append(
-                ValidationError(
-                    context=SemanticModelContext(
-                        file_context=FileContext.from_metadata(metadata=semantic_model.metadata),
-                        semantic_model=SemanticModelReference(semantic_model_name=semantic_model.name),
-                    ),
-                    message=f"No primary time dimension in semantic model with name ({semantic_model.name}). "
-                    "Please add one",
-                )
-            )
-
-        if len(primary_time_dimensions) > 1:
-            for primary_time_dimension in primary_time_dimensions:
+        for measure in semantic_model.measures:
+            if measure.agg_time_dimension is None:
                 issues.append(
                     ValidationError(
                         context=SemanticModelContext(
                             file_context=FileContext.from_metadata(metadata=semantic_model.metadata),
                             semantic_model=SemanticModelReference(semantic_model_name=semantic_model.name),
                         ),
-                        message=f"In semantic model {semantic_model.name}, "
-                        f"Primary time dimension with name: {primary_time_dimension.name} "
-                        f"is one of many defined as primary.",
+                        message=f"Aggregation time dimension not specified for measure named '{measure.name}' in the "
+                        f"semantic model named '{semantic_model.name}'. Please add one",
                     )
                 )
 
         return issues
 
 
-class SemanticModelValidityWindowRule(ModelValidationRule):
+class SemanticModelValidityWindowRule(SemanticManifestValidationRule[SemanticManifestT], Generic[SemanticManifestT]):
     """Checks validity windows in semantic models to ensure they comply with runtime requirements."""
 
     @staticmethod
     @validate_safely(whats_being_done="checking correctness of the time dimension validity parameters in the model")
-    def validate_model(model: SemanticManifest) -> List[ValidationIssue]:
+    def validate_manifest(semantic_manifest: SemanticManifestT) -> Sequence[ValidationIssue]:
         """Checks the validity param definitions in every semantic model in the model."""
         issues: List[ValidationIssue] = []
 
-        for semantic_model in model.semantic_models:
+        for semantic_model in semantic_manifest.semantic_models:
             issues.extend(SemanticModelValidityWindowRule._validate_semantic_model(semantic_model=semantic_model))
 
         return issues
 
     @staticmethod
     @validate_safely(
         whats_being_done="checking the semantic model's validity parameters for compatibility with "
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/validations/unique_valid_name.py` & `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/validations/unique_valid_name.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 from __future__ import annotations
 
 import enum
 import re
-from typing import Dict, List, Optional, Tuple
+from typing import Dict, Generic, List, Optional, Sequence, Tuple
 
 from dbt_semantic_interfaces.enum_extension import assert_values_exhausted
-from dbt_semantic_interfaces.objects.semantic_manifest import SemanticManifest
-from dbt_semantic_interfaces.objects.semantic_model import SemanticModel
+from dbt_semantic_interfaces.protocols.semantic_manifest import (
+    SemanticManifest,
+    SemanticManifestT,
+)
+from dbt_semantic_interfaces.protocols.semantic_model import SemanticModel
 from dbt_semantic_interfaces.references import (
     ElementReference,
     MetricModelReference,
     SemanticModelElementReference,
     SemanticModelReference,
 )
 from dbt_semantic_interfaces.type_enums.time_granularity import TimeGranularity
 from dbt_semantic_interfaces.validations.validator_helpers import (
     FileContext,
     MetricContext,
-    ModelValidationRule,
+    SemanticManifestValidationRule,
     SemanticModelContext,
     SemanticModelElementContext,
     SemanticModelElementType,
     ValidationContext,
     ValidationError,
     ValidationIssue,
     validate_safely,
@@ -45,15 +48,15 @@
             )
         elif keyword is MetricFlowReservedKeywords.MF_INTERNAL_UUID:
             return "Used internally to reference a column that has a uuid generated by MetricFlow."
         else:
             assert_values_exhausted(keyword)
 
 
-class UniqueAndValidNameRule(ModelValidationRule):
+class UniqueAndValidNameRule(SemanticManifestValidationRule[SemanticManifestT], Generic[SemanticManifestT]):
     """Check that names are unique and valid.
 
     * Names of elements in semantic models are unique / valid within the semantic model.
     * Names of semantic models, dimension sets and metric sets in the model are unique / valid.
     """
 
     NAME_REGEX = re.compile(r"\A[a-z][a-z0-9_]*[a-z0-9]\Z")
@@ -213,15 +216,15 @@
         for name, _, context in object_info_tuples:
             issues += UniqueAndValidNameRule.check_valid_name(name=name, context=context)
 
         return issues
 
     @staticmethod
     @validate_safely(whats_being_done="running model validation ensuring elements have adequately unique names")
-    def validate_model(model: SemanticManifest) -> List[ValidationIssue]:  # noqa: D
+    def validate_manifest(semantic_manifest: SemanticManifestT) -> Sequence[ValidationIssue]:  # noqa: D
         issues = []
-        issues += UniqueAndValidNameRule._validate_top_level_objects(model=model)
+        issues += UniqueAndValidNameRule._validate_top_level_objects(model=semantic_manifest)
 
-        for semantic_model in model.semantic_models:
+        for semantic_model in semantic_manifest.semantic_models:
             issues += UniqueAndValidNameRule._validate_semantic_model_elements(semantic_model=semantic_model)
 
         return issues
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/validations/validator_helpers.py` & `dbt_semantic_interfaces-0.1.0.dev2/dbt_semantic_interfaces/validations/validator_helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,37 +2,47 @@
 
 import functools
 import traceback
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from datetime import date
 from enum import Enum
-from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple, Union
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    Generic,
+    Iterable,
+    List,
+    Optional,
+    Sequence,
+    Tuple,
+    Union,
+)
 
 import click
 from pydantic import BaseModel, Extra
 
-from dbt_semantic_interfaces.enum_extension import assert_values_exhausted
-from dbt_semantic_interfaces.objects.base import FrozenBaseModel
-from dbt_semantic_interfaces.objects.metadata import Metadata
-from dbt_semantic_interfaces.objects.semantic_manifest import SemanticManifest
+from dbt_semantic_interfaces.implementations.base import FrozenBaseModel
+from dbt_semantic_interfaces.protocols.metadata import Metadata
+from dbt_semantic_interfaces.protocols.semantic_manifest import SemanticManifestT
 from dbt_semantic_interfaces.references import (
     MetricModelReference,
     SemanticModelElementReference,
     SemanticModelReference,
 )
 from dbt_semantic_interfaces.type_enums.dimension_type import DimensionType
 
 VALIDATE_SAFELY_ERROR_STR_TMPLT = ". Issue occurred in method `{method_name}` called with {arguments_str}"
 ValidationContextJSON = Dict[str, Union[str, int, None]]
 ValidationIssueJSON = Dict[str, Union[str, int, ValidationContextJSON]]
 
 
 class ValidationIssueLevel(Enum):
-    """Categorize the issues found while validating a MQL model."""
+    """Categorize the issues found while validating a semantic manifest."""
 
     # Issue should be fixed, but model will still work in MQL
     WARNING = 0
     # Issue doesn't prevent model from working in MQL yet, but will eventually be an error
     FUTURE_ERROR = 1
     # Issue will prevent the model from working in MQL
     ERROR = 2
@@ -66,15 +76,15 @@
 
     class Config:
         """Pydantic class configuration options."""
 
         extra = Extra.forbid
 
     def context_str(self) -> str:
-        """Human readable stringified representation of the context."""
+        """Human-readable stringified representation of the context."""
         context_string = ""
 
         if self.file_name:
             context_string += f"in file `{self.file_name}`"
             if self.line_number:
                 context_string += f" on line #{self.line_number}"
 
@@ -92,38 +102,38 @@
 class MetricContext(BaseModel):
     """The context class for validation issues involving metrics."""
 
     file_context: FileContext
     metric: MetricModelReference
 
     def context_str(self) -> str:
-        """Human readable stringified representation of the context."""
+        """Human-readable stringified representation of the context."""
         return f"with metric `{self.metric.metric_name}` {self.file_context.context_str()}"
 
 
 class SemanticModelContext(BaseModel):
     """The context class for validation issues involving semantic models."""
 
     file_context: FileContext
     semantic_model: SemanticModelReference
 
     def context_str(self) -> str:
-        """Human readable stringified representation of the context."""
+        """Human-readable stringified representation of the context."""
         return f"with semantic model `{self.semantic_model.semantic_model_name}` {self.file_context.context_str()}"
 
 
 class SemanticModelElementContext(BaseModel):
     """The context class for validation issues involving dimensions."""
 
     file_context: FileContext
     semantic_model_element: SemanticModelElementReference
     element_type: SemanticModelElementType
 
     def context_str(self) -> str:
-        """Human readable stringified representation of the context."""
+        """Human-readable stringified representation of the context."""
         return (
             f"with {self.element_type.value} `{self.semantic_model_element.element_name}` in semantic model "
             f"`{self.semantic_model_element.semantic_model_name}` {self.file_context.context_str()}"
         )
 
 
 ValidationContext = Union[
@@ -131,28 +141,28 @@
     MetricContext,
     SemanticModelContext,
     SemanticModelElementContext,
 ]
 
 
 class ValidationIssue(ABC, BaseModel):
-    """The abstract base ValidationIsssue class that the specific ValidationIssue classes are built from."""
+    """The abstract base ValidationIssue class that the specific ValidationIssue classes are built from."""
 
     message: str
     context: Optional[ValidationContext] = None
     extra_detail: Optional[str]
 
     @property
     @abstractmethod
     def level(self) -> ValidationIssueLevel:
-        """The level of of ValidationIssue."""
+        """The level of ValidationIssue."""
         raise NotImplementedError
 
     def as_readable_str(self, verbose: bool = False, prefix: Optional[str] = None) -> str:
-        """Return a easily readable string that can be used to log the issue."""
+        """Return an easily readable string that can be used to log the issue."""
         prefix = prefix or self.level.name
 
         # The following is two lines instead of one line because
         # technically self.context.context_str() can return an empty str
         context_str = self.context.context_str() if self.context else ""
         context_str += " - " if context_str != "" else ""
 
@@ -164,86 +174,122 @@
 
     def as_cli_formatted_str(self, verbose: bool = False) -> str:
         """Returns a color-coded readable string for rendering issues in the CLI."""
         return self.as_readable_str(
             verbose=verbose, prefix=click.style(self.level.name, bold=True, fg=ISSUE_COLOR_MAP[self.level])
         )
 
+    @property
+    @abstractmethod
+    def as_issue_set(self) -> ValidationIssueSet:  # noqa: D
+        raise NotImplementedError
+
+
+@dataclass(frozen=True)
+class ValidationIssueSet:
+    """Groups validation issues by type."""
+
+    warning_issues: Sequence[ValidationWarning] = ()
+    future_error_issues: Sequence[ValidationFutureError] = ()
+    error_issues: Sequence[ValidationError] = ()
+
+    @staticmethod
+    def combine(validation_issue_sets: Iterable[ValidationIssueSet]) -> ValidationIssueSet:
+        """Combine the given issues (no de-duping)."""
+        combined_warning_issues: List[ValidationWarning] = []
+        combined_future_error_issues: List[ValidationFutureError] = []
+        combined_error_issues: List[ValidationError] = []
+
+        for validation_issue_set in validation_issue_sets:
+            combined_warning_issues.extend(validation_issue_set.warning_issues)
+            combined_future_error_issues.extend(validation_issue_set.future_error_issues)
+            combined_error_issues.extend(validation_issue_set.error_issues)
+
+        return ValidationIssueSet(
+            warning_issues=tuple(combined_warning_issues),
+            future_error_issues=tuple(combined_future_error_issues),
+            error_issues=tuple(combined_error_issues),
+        )
+
 
 class ValidationWarning(ValidationIssue, BaseModel):
     """A warning that was found while validating the model."""
 
     @property
     def level(self) -> ValidationIssueLevel:  # noqa: D
         return ValidationIssueLevel.WARNING
 
+    @property
+    def as_issue_set(self) -> ValidationIssueSet:  # noqa: D
+        return ValidationIssueSet(warning_issues=(self,))
+
 
 class ValidationFutureError(ValidationIssue, BaseModel):
     """A future error that was found while validating the model."""
 
     error_date: date
 
     @property
     def level(self) -> ValidationIssueLevel:  # noqa: D
         return ValidationIssueLevel.FUTURE_ERROR
 
     def as_readable_str(self, verbose: bool = False, prefix: Optional[str] = None) -> str:
-        """Return a easily readable string that can be used to log the issue."""
+        """Return an easily readable string that can be used to log the issue."""
         return (
             f"{super().as_readable_str(verbose=verbose, prefix=prefix)}"
             f"IMPORTANT: this error will break your model starting {self.error_date.strftime('%b %d, %Y')}. "
         )
 
+    @property
+    def as_issue_set(self) -> ValidationIssueSet:  # noqa: D
+        return ValidationIssueSet(future_error_issues=(self,))
+
 
 class ValidationError(ValidationIssue, BaseModel):
     """An error that was found while validating the model."""
 
     @property
     def level(self) -> ValidationIssueLevel:  # noqa: D
         return ValidationIssueLevel.ERROR
 
+    @property
+    def as_issue_set(self) -> ValidationIssueSet:  # noqa: D
+        return ValidationIssueSet(error_issues=(self,))
+
 
-class ModelValidationResults(FrozenBaseModel):
-    """Class for organizating the results of running validations."""
+class SemanticManifestValidationResults(FrozenBaseModel):
+    """Class for organizing the results of running validations."""
 
     warnings: Tuple[ValidationWarning, ...] = tuple()
     future_errors: Tuple[ValidationFutureError, ...] = tuple()
     errors: Tuple[ValidationError, ...] = tuple()
 
     @property
     def has_blocking_issues(self) -> bool:
-        """Does the ModelValidationResults have ERROR issues."""
+        """Does the SemanticManifestValidationResults have ERROR issues."""
         return len(self.errors) != 0
 
-    @classmethod
-    def from_issues_sequence(cls, issues: Sequence[ValidationIssue]) -> ModelValidationResults:
-        """Constructs a ModelValidationResults class from a list of ValidationIssues."""
-        warnings: List[ValidationWarning] = []
-        future_errors: List[ValidationFutureError] = []
-        errors: List[ValidationError] = []
-
-        for issue in issues:
-            if issue.level is ValidationIssueLevel.WARNING:
-                warnings.append(issue)
-            elif issue.level is ValidationIssueLevel.FUTURE_ERROR:
-                future_errors.append(issue)
-            elif issue.level is ValidationIssueLevel.ERROR:
-                errors.append(issue)
-            else:
-                assert_values_exhausted(issue.level)
-        return cls(warnings=tuple(warnings), future_errors=tuple(future_errors), errors=tuple(errors))
+    @staticmethod
+    def from_issues_sequence(issues: Sequence[ValidationIssue]) -> SemanticManifestValidationResults:
+        """Constructs a SemanticManifestValidationResults class from a list of ValidationIssues."""
+        combined_issue_set = ValidationIssueSet.combine(tuple(issue.as_issue_set for issue in issues))
+        return SemanticManifestValidationResults(
+            warnings=tuple(combined_issue_set.warning_issues),
+            future_errors=tuple(combined_issue_set.future_error_issues),
+            errors=tuple(combined_issue_set.error_issues),
+        )
 
     @classmethod
-    def merge(cls, results: Sequence[ModelValidationResults]) -> ModelValidationResults:
+    def merge(cls, results: Sequence[SemanticManifestValidationResults]) -> SemanticManifestValidationResults:
         """Creates a new ModelValidatorResults instance from multiple instances.
 
         This is useful when there are multiple validators that are run and the
-        combined results are desireable. For instance there is a ModelValidator
+        combined results are desirable. For instance there is a SemanticManifestValidator
         and a DataWarehouseModelValidator. These both return validation issues.
-        If it's desireable to combine the results, the following makes it easy.
+        If it's desirable to combine the results, the following makes it easy.
         """
         if not isinstance(results, List):
             results = list(results)
 
         # this nested comprehension syntax is a little disorienting
         # basically [element for object in list_of_objects for element in object.list_property]
         # translates to "for each element in an object's list for each object in a list of objects"
@@ -264,35 +310,41 @@
 
     def summary(self) -> str:
         """Returns a stylized summary string for issues."""
         errors = click.style(
             text=f"{ValidationIssueLevel.ERROR.name_plural}: {len(self.errors)}",
             fg=ISSUE_COLOR_MAP[ValidationIssueLevel.ERROR],
         )
-        future_erros = click.style(
+        future_errors = click.style(
             text=f"{ValidationIssueLevel.FUTURE_ERROR.name_plural}: {len(self.future_errors)}",
             fg=ISSUE_COLOR_MAP[ValidationIssueLevel.FUTURE_ERROR],
         )
         warnings = click.style(
             text=f"{ValidationIssueLevel.WARNING.name_plural}: {len(self.warnings)}",
             fg=ISSUE_COLOR_MAP[ValidationIssueLevel.WARNING],
         )
-        return f"{errors}, {future_erros}, {warnings}"
+        return f"{errors}, {future_errors}, {warnings}"
 
 
 def generate_exception_issue(
-    what_was_being_done: str, e: Exception, context: Optional[ValidationContext] = None, extras: Dict[str, str] = {}
+    what_was_being_done: str,
+    e: Exception,
+    context: Optional[ValidationContext] = None,
+    extras: Optional[Dict[str, str]] = None,
 ) -> ValidationIssue:
     """Generates a validation issue for exceptions."""
+    if extras is None:
+        extras = {}
+
     if "stacktrace" not in extras:
         extras["stacktrace"] = "".join(traceback.format_tb(e.__traceback__))
 
     return ValidationError(
         context=context,
-        message=f"An error occured while {what_was_being_done} - "
+        message=f"An error occurred while {what_was_being_done} - "
         f"{''.join(traceback.format_exception_only(etype=type(e), value=e))}",
         extra_detail="\n".join([f"{key}: {value}" for key, value in extras.items()]),
     )
 
 
 def _func_args_to_string(*args: Any, **kwargs: Any) -> str:  # type: ignore
     return f"positional args: {args}, key word args: {kwargs}"
@@ -331,35 +383,23 @@
     All dimensions with a given name in all semantic models should have attributes matching these values.
     """
 
     type: DimensionType
     is_partition: bool
 
 
-class ModelValidationRule(ABC):
-    """Encapsulates logic for checking the values of objects in a model."""
+class SemanticManifestValidationRule(ABC, Generic[SemanticManifestT]):
+    """Encapsulates logic for checking the values of objects in a manifest."""
 
     @classmethod
     @abstractmethod
-    def validate_model(cls, model: SemanticManifest) -> List[ValidationIssue]:
-        """Check the given model and return a list of validation issues."""
+    def validate_manifest(cls, semantic_manifest: SemanticManifestT) -> Sequence[ValidationIssue]:
+        """Check the given manifest and return a list of validation issues."""
         pass
 
-    @classmethod
-    def validate_model_serialized_for_multiprocessing(cls, serialized_model: str) -> str:
-        """Validate a model serialized via Pydantic's .json() method, and return a list of JSON serialized issues.
-
-        This method exists because our validations are forked into parallel processes via
-        multiprocessing.ProcessPoolExecutor, and passing a model or validation results object can result in
-        idiosyncratic behavior and inscrutable errors due to interactions between pickling and pydantic objects.
-        """
-        return ModelValidationResults.from_issues_sequence(
-            cls.validate_model(SemanticManifest.parse_raw(serialized_model))
-        ).json()
-
 
-class ModelValidationException(Exception):
+class SemanticManifestValidationException(Exception):
     """Exception raised when validation of a model fails."""
 
     def __init__(self, issues: Tuple[ValidationIssue, ...]) -> None:  # noqa: D
         issues_str = "\n".join([x.as_readable_str(verbose=True) for x in issues])
         super().__init__(f"Error validating model. Issues:\n{issues_str}")
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev1/venv-3.9.16/bin/Activate.ps1` & `dbt_semantic_interfaces-0.1.0.dev2/venv-3.9.16/bin/Activate.ps1`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev1/venv-3.9.16/bin/activate` & `dbt_semantic_interfaces-0.1.0.dev2/venv-3.9.16/bin/activate`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev1/venv-3.9.16/bin/activate.csh` & `dbt_semantic_interfaces-0.1.0.dev2/venv-3.9.16/bin/activate.csh`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev1/venv-3.9.16/bin/activate.fish` & `dbt_semantic_interfaces-0.1.0.dev2/venv-3.9.16/bin/activate.fish`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev1/.gitignore` & `dbt_semantic_interfaces-0.1.0.dev2/.gitignore`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev1/LICENSE` & `dbt_semantic_interfaces-0.1.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev1/README.md` & `dbt_semantic_interfaces-0.1.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev1/pyproject.toml` & `dbt_semantic_interfaces-0.1.0.dev2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dbt-semantic-interfaces"
-version = "0.1.0.dev1"
+version = "0.1.0.dev2"
 description = 'The shared semantic layer definitions that dbt-core and MetricFlow use'
 readme = "README.md"
 requires-python = ">=3.8"
 license = "Apache-2.0"
 keywords = []
 authors = [
   { name = "dbt Labs", email = "info@dbtlabs.com" },
@@ -16,46 +16,60 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-  "pydantic~=1.9.0",
+  "pydantic~=1.10.8",
   "jsonschema==3.2.0",
   "PyYAML~=6.0",
   "more-itertools==8.10.0",
   "Jinja2==3.1.2",
   "click>=7.1.2",
   "python-dateutil==2.8.2",
+  "importlib_metadata==6.6.0",
+  "typing-extensions~=4.6.1",
 ]
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
-[tool.hatch.envs.pre-commit]
-description = "Env for running pre-commit hooks."
-dependencies = [
-  "pre-commit~=3.2.2",
-  "isort~=5.12.0",
-  "black~=23.3.0",
-  "ruff~=0.0.260",
-  "mypy~=1.1.1",
-  "pytest~=7.3.0",
+[tool.hatch.build.targets.sdist]
+exclude = [
+  "/.github",
+  "/.changes",
+  ".changie.yaml",
+  ".gitignore",
+  ".pre-commit-config.yaml",
+  "CONTRIBUTING.md",
+  "MAKEFILE",
+  "/tests",
 ]
 
-[tool.hatch.envs.pre-commit.scripts]
+[tool.hatch.envs.dev-env.scripts]
 all = ["pre-commit run --all-files"]
 
-[tool.hatch.envs.pytest]
-description = "Env for running pytest."
+[tool.hatch.envs.dev-env]
+description = "Env for running development commands like pytest / pre-commit"
 dependencies = [
   "pytest~=7.3.0",
+  "pytest-xdist~=3.2.1",
   "httpx~=0.24.0",
+  "pre-commit~=3.2.2",
+  "isort~=5.12.0",
+  "black~=23.3.0",
+  "ruff~=0.0.260",
+  "mypy~=1.3.0",
+  "pytest~=7.3.0",
+  "types-Jinja2~=2.11.9",
+  "types-jsonschema~=4.17",
+  "types-python-dateutil~=2.8.19",
+  "types-PyYAML~=6.0.12",
 ]
 
 [tool.ruff]
 line-length = 120
 select = [
   "E", # Pycodestyle
   "F", # Pyflakes
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev1/PKG-INFO` & `dbt_semantic_interfaces-0.1.0.dev2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: dbt-semantic-interfaces
-Version: 0.1.0.dev1
+Version: 0.1.0.dev2
 Summary: The shared semantic layer definitions that dbt-core and MetricFlow use
 Author-email: dbt Labs <info@dbtlabs.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Requires-Dist: click>=7.1.2
+Requires-Dist: importlib-metadata==6.6.0
 Requires-Dist: jinja2==3.1.2
 Requires-Dist: jsonschema==3.2.0
 Requires-Dist: more-itertools==8.10.0
-Requires-Dist: pydantic~=1.9.0
+Requires-Dist: pydantic~=1.10.8
 Requires-Dist: python-dateutil==2.8.2
 Requires-Dist: pyyaml~=6.0
+Requires-Dist: typing-extensions~=4.6.1
 Description-Content-Type: text/markdown
 
 <p align="center">
     <a target="_blank" href="https://twitter.com/dbt_labs">
     <img src="https://img.shields.io/twitter/follow/dbt_labs?labelColor=image.png&color=163B36&logo=twitter&style=flat">
   </a>
     <a target="_blank" href="https://www.getdbt.com/community/">
```

#### html2text {}

```diff
@@ -1,21 +1,22 @@
-Metadata-Version: 2.1 Name: dbt-semantic-interfaces Version: 0.1.0.dev1
+Metadata-Version: 2.1 Name: dbt-semantic-interfaces Version: 0.1.0.dev2
 Summary: The shared semantic layer definitions that dbt-core and MetricFlow use
 Author-email: dbt Labs
 dbtlabs.com> License-Expression: Apache-2.0 License-File: LICENSE Classifier:
 Development Status :: 4 - Beta Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: Implementation :: CPython Classifier: Programming
 Language :: Python :: Implementation :: PyPy Requires-Python: >=3.8 Requires-
-Dist: click>=7.1.2 Requires-Dist: jinja2==3.1.2 Requires-Dist:
-jsonschema==3.2.0 Requires-Dist: more-itertools==8.10.0 Requires-Dist:
-pydantic~=1.9.0 Requires-Dist: python-dateutil==2.8.2 Requires-Dist:
-pyyaml~=6.0 Description-Content-Type: text/markdown
+Dist: click>=7.1.2 Requires-Dist: importlib-metadata==6.6.0 Requires-Dist:
+jinja2==3.1.2 Requires-Dist: jsonschema==3.2.0 Requires-Dist: more-
+itertools==8.10.0 Requires-Dist: pydantic~=1.10.8 Requires-Dist: python-
+dateutil==2.8.2 Requires-Dist: pyyaml~=6.0 Requires-Dist: typing-
+extensions~=4.6.1 Description-Content-Type: text/markdown
                     [https://img.shields.io/twitter/follow/
  dbt_labs?labelColor=image.png&color=163B36&logo=twitter&style=flat] [https://
     img.shields.io/badge/Slack-join-163B36] [https://img.shields.io/badge/
                         code%20style-black-000000.svg]
 # dbt-semantic-interfaces This repo contains the shared semantic classes,
 default validation, and tests designed to be used by both the dbt-core and
 MetricFlow projects. By centralizing these shared resources, we aim to maintain
```

