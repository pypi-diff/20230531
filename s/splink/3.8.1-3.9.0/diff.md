# Comparing `tmp/splink-3.8.1.tar.gz` & `tmp/splink-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splink-3.8.1.tar", max compression
+gzip compressed data, was "splink-3.9.0.tar", max compression
```

## Comparing `splink-3.8.1.tar` & `splink-3.9.0.tar`

### file list

```diff
@@ -1,112 +1,124 @@
--rw-r--r--   0        0        0     1076 2023-04-27 19:35:50.176911 splink-3.8.1/LICENSE
--rw-r--r--   0        0        0     8448 2023-04-27 19:35:50.176911 splink-3.8.1/README.md
--rw-r--r--   0        0        0     1451 2023-04-27 19:35:50.204911 splink-3.8.1/pyproject.toml
--rw-r--r--   0        0        0       23 2023-04-27 19:35:50.204911 splink-3.8.1/splink/__init__.py
--rw-r--r--   0        0        0    10852 2023-04-27 19:35:50.204911 splink-3.8.1/splink/accuracy.py
--rw-r--r--   0        0        0     4759 2023-04-27 19:35:50.204911 splink-3.8.1/splink/analyse_blocking.py
--rw-r--r--   0        0        0      461 2023-04-27 19:35:50.204911 splink-3.8.1/splink/athena/athena_base.py
--rw-r--r--   0        0        0     1672 2023-04-27 19:35:50.204911 splink-3.8.1/splink/athena/athena_comparison_level_library.py
--rw-r--r--   0        0        0     1015 2023-04-27 19:35:50.204911 splink-3.8.1/splink/athena/athena_comparison_library.py
--rw-r--r--   0        0        0    20569 2023-04-27 19:35:50.204911 splink-3.8.1/splink/athena/athena_linker.py
--rw-r--r--   0        0        0      350 2023-04-27 19:35:50.204911 splink-3.8.1/splink/athena/athena_transforms.py
--rw-r--r--   0        0        0     2904 2023-04-27 19:35:50.204911 splink-3.8.1/splink/athena/athena_utils.py
--rw-r--r--   0        0        0     2867 2023-04-27 19:35:50.204911 splink-3.8.1/splink/block_from_labels.py
--rw-r--r--   0        0        0     5965 2023-04-27 19:35:50.204911 splink-3.8.1/splink/blocking.py
--rw-r--r--   0        0        0    10627 2023-04-27 19:35:50.204911 splink-3.8.1/splink/charts.py
--rw-r--r--   0        0        0     9088 2023-04-27 19:35:50.204911 splink-3.8.1/splink/cluster_studio.py
--rw-r--r--   0        0        0    16881 2023-04-27 19:35:50.204911 splink-3.8.1/splink/comparison.py
--rw-r--r--   0        0        0    25479 2023-04-27 19:35:50.204911 splink-3.8.1/splink/comparison_level.py
--rw-r--r--   0        0        0     9013 2023-04-27 19:35:50.204911 splink-3.8.1/splink/comparison_level_composition.py
--rw-r--r--   0        0        0    25022 2023-04-27 19:35:50.204911 splink-3.8.1/splink/comparison_level_library.py
--rw-r--r--   0        0        0     1237 2023-04-27 19:35:50.204911 splink-3.8.1/splink/comparison_level_sql.py
--rw-r--r--   0        0        0    35793 2023-04-27 19:35:50.204911 splink-3.8.1/splink/comparison_library.py
--rw-r--r--   0        0        0     4315 2023-04-27 19:35:50.204911 splink-3.8.1/splink/comparison_library_utils.py
--rw-r--r--   0        0        0    23009 2023-04-27 19:35:50.208911 splink-3.8.1/splink/comparison_template_library.py
--rw-r--r--   0        0        0      972 2023-04-27 19:35:50.208911 splink-3.8.1/splink/comparison_vector_distribution.py
--rw-r--r--   0        0        0      868 2023-04-27 19:35:50.208911 splink-3.8.1/splink/comparison_vector_values.py
--rw-r--r--   0        0        0    16516 2023-04-27 19:35:50.208911 splink-3.8.1/splink/connected_components.py
--rw-r--r--   0        0        0       67 2023-04-27 19:35:50.208911 splink-3.8.1/splink/constants.py
--rw-r--r--   0        0        0     6089 2023-04-27 19:35:50.208911 splink-3.8.1/splink/convert_v2_to_v3.py
--rw-r--r--   0        0        0     1338 2023-04-27 19:35:50.208911 splink-3.8.1/splink/databricks/enable_splink.py
--rw-r--r--   0        0        0      609 2023-04-27 19:35:50.208911 splink-3.8.1/splink/default_from_jsonschema.py
--rw-r--r--   0        0        0     1332 2023-04-27 19:35:50.208911 splink-3.8.1/splink/dialect_base.py
--rw-r--r--   0        0        0     1332 2023-04-27 19:35:50.208911 splink-3.8.1/splink/duckdb/duckdb_base.py
--rw-r--r--   0        0        0     2369 2023-04-27 19:35:50.208911 splink-3.8.1/splink/duckdb/duckdb_comparison_level_library.py
--rw-r--r--   0        0        0     1823 2023-04-27 19:35:50.208911 splink-3.8.1/splink/duckdb/duckdb_comparison_library.py
--rw-r--r--   0        0        0      543 2023-04-27 19:35:50.208911 splink-3.8.1/splink/duckdb/duckdb_comparison_template_library.py
--rw-r--r--   0        0        0     1750 2023-04-27 19:35:50.208911 splink-3.8.1/splink/duckdb/duckdb_helpers.py
--rw-r--r--   0        0        0     9974 2023-04-27 19:35:50.208911 splink-3.8.1/splink/duckdb/duckdb_linker.py
--rw-r--r--   0        0        0    17471 2023-04-27 19:35:50.208911 splink-3.8.1/splink/em_training_session.py
--rw-r--r--   0        0        0     5244 2023-04-27 19:35:50.208911 splink-3.8.1/splink/estimate_u.py
--rw-r--r--   0        0        0      144 2023-04-27 19:35:50.208911 splink-3.8.1/splink/exceptions.py
--rw-r--r--   0        0        0     6062 2023-04-27 19:35:50.208911 splink-3.8.1/splink/expectation_maximisation.py
--rw-r--r--   0        0        0     1558 2023-04-27 19:35:50.208911 splink-3.8.1/splink/files/chart_defs/blocking_rule_generated_comparisons.json
--rw-r--r--   0        0        0     2779 2023-04-27 19:35:50.208911 splink-3.8.1/splink/files/chart_defs/completeness.json
--rw-r--r--   0        0        0     6737 2023-04-27 19:35:50.208911 splink-3.8.1/splink/files/chart_defs/del/bayes_factor_history_chart_def.json
--rw-r--r--   0        0        0     7747 2023-04-27 19:35:50.208911 splink-3.8.1/splink/files/chart_defs/del/bayes_factor_intuition_chart_def.json
--rw-r--r--   0        0        0     6298 2023-04-27 19:35:50.208911 splink-3.8.1/splink/files/chart_defs/del/compare_estimates.json
--rw-r--r--   0        0        0     2155 2023-04-27 19:35:50.208911 splink-3.8.1/splink/files/chart_defs/del/gamma_distribution_chart_def.json
--rw-r--r--   0        0        0      743 2023-04-27 19:35:50.208911 splink-3.8.1/splink/files/chart_defs/del/gamma_histogram.json
--rw-r--r--   0        0        0     1309 2023-04-27 19:35:50.208911 splink-3.8.1/splink/files/chart_defs/del/score_histogram.json
--rw-r--r--   0        0        0     5831 2023-04-27 19:35:50.208911 splink-3.8.1/splink/files/chart_defs/m_u_parameters_interactive_history.json
--rw-r--r--   0        0        0      977 2023-04-27 19:35:50.208911 splink-3.8.1/splink/files/chart_defs/match_weight_histogram.json
--rw-r--r--   0        0        0     5766 2023-04-27 19:35:50.208911 splink-3.8.1/splink/files/chart_defs/match_weights_interactive_history.json
--rw-r--r--   0        0        0     9159 2023-04-27 19:35:50.208911 splink-3.8.1/splink/files/chart_defs/match_weights_waterfall.json
--rw-r--r--   0        0        0     1734 2023-04-27 19:35:50.208911 splink-3.8.1/splink/files/chart_defs/missingness.json
--rw-r--r--   0        0        0     1730 2023-04-27 19:35:50.208911 splink-3.8.1/splink/files/chart_defs/parameter_estimate_comparisons.json
--rw-r--r--   0        0        0     1465 2023-04-27 19:35:50.208911 splink-3.8.1/splink/files/chart_defs/precision_recall.json
--rw-r--r--   0        0        0     1123 2023-04-27 19:35:50.208911 splink-3.8.1/splink/files/chart_defs/probability_two_random_records_match_iteration.json
--rw-r--r--   0        0        0     2326 2023-04-27 19:35:50.208911 splink-3.8.1/splink/files/chart_defs/profile_data.json
--rw-r--r--   0        0        0     1745 2023-04-27 19:35:50.208911 splink-3.8.1/splink/files/chart_defs/roc.json
--rw-r--r--   0        0        0     2645 2023-04-27 19:35:50.208911 splink-3.8.1/splink/files/chart_defs/unlinkables_chart_def.json
--rw-r--r--   0        0        0    66064 2023-04-27 19:35:50.208911 splink-3.8.1/splink/files/external_js/vega-embed@6.20.2
--rw-r--r--   0        0        0   256817 2023-04-27 19:35:50.212911 splink-3.8.1/splink/files/external_js/vega-lite@5.2.0
--rw-r--r--   0        0        0   501599 2023-04-27 19:35:50.212911 splink-3.8.1/splink/files/external_js/vega@5.21.0
--rw-r--r--   0        0        0    12871 2023-04-27 19:35:50.212911 splink-3.8.1/splink/files/settings_jsonschema.json
--rw-r--r--   0        0        0  1228220 2023-04-27 19:35:50.224911 splink-3.8.1/splink/files/spark_jars/scala-udf-similarity-0.1.0_classic.jar
--rw-r--r--   0        0        0   944614 2023-04-27 19:35:50.228911 splink-3.8.1/splink/files/spark_jars/scala-udf-similarity-0.1.0_spark3.3.jar
--rw-r--r--   0        0        0   949562 2023-04-27 19:35:50.228911 splink-3.8.1/splink/files/spark_jars/scala-udf-similarity-0.1.1_spark3.x.jar
--rw-r--r--   0        0        0     5486 2023-04-27 19:35:50.228911 splink-3.8.1/splink/files/splink_cluster_studio/cluster_template.j2
--rw-r--r--   0        0        0     2269 2023-04-27 19:35:50.228911 splink-3.8.1/splink/files/splink_cluster_studio/custom.css
--rw-r--r--   0        0        0     2269 2023-04-27 19:35:50.228911 splink-3.8.1/splink/files/splink_comparison_viewer/custom.css
--rw-r--r--   0        0        0     3115 2023-04-27 19:35:50.228911 splink-3.8.1/splink/files/splink_comparison_viewer/template.j2
--rw-r--r--   0        0        0   269522 2023-04-27 19:35:50.228911 splink-3.8.1/splink/files/splink_vis_utils/splink_vis_utils.js
--rw-r--r--   0        0        0      404 2023-04-27 19:35:50.228911 splink-3.8.1/splink/files/templates/single_chart_template.txt
--rw-r--r--   0        0        0      195 2023-04-27 19:35:50.228911 splink-3.8.1/splink/format_sql.py
--rw-r--r--   0        0        0     7955 2023-04-27 19:35:50.232911 splink-3.8.1/splink/input_column.py
--rw-r--r--   0        0        0   120307 2023-04-27 19:35:50.232911 splink-3.8.1/splink/linker.py
--rw-r--r--   0        0        0      300 2023-04-27 19:35:50.232911 splink-3.8.1/splink/logging_messages.py
--rw-r--r--   0        0        0     3132 2023-04-27 19:35:50.232911 splink-3.8.1/splink/lower_id_on_lhs.py
--rw-r--r--   0        0        0     1834 2023-04-27 19:35:50.232911 splink-3.8.1/splink/m_from_labels.py
--rw-r--r--   0        0        0     2465 2023-04-27 19:35:50.232911 splink-3.8.1/splink/m_training.py
--rw-r--r--   0        0        0     2420 2023-04-27 19:35:50.232911 splink-3.8.1/splink/m_u_records_to_parameters.py
--rw-r--r--   0        0        0      623 2023-04-27 19:35:50.232911 splink-3.8.1/splink/match_key_analysis.py
--rw-r--r--   0        0        0     2028 2023-04-27 19:35:50.232911 splink-3.8.1/splink/match_weights_histogram.py
--rw-r--r--   0        0        0     4548 2023-04-27 19:35:50.232911 splink-3.8.1/splink/misc.py
--rw-r--r--   0        0        0     2791 2023-04-27 19:35:50.232911 splink-3.8.1/splink/missingness.py
--rw-r--r--   0        0        0     1221 2023-04-27 19:35:50.232911 splink-3.8.1/splink/parse_sql.py
--rw-r--r--   0        0        0     2909 2023-04-27 19:35:50.232911 splink-3.8.1/splink/pipeline.py
--rw-r--r--   0        0        0     3205 2023-04-27 19:35:50.232911 splink-3.8.1/splink/predict.py
--rw-r--r--   0        0        0     8245 2023-04-27 19:35:50.232911 splink-3.8.1/splink/profile_data.py
--rw-r--r--   0        0        0    18694 2023-04-27 19:35:50.232911 splink-3.8.1/splink/settings.py
--rw-r--r--   0        0        0     1083 2023-04-27 19:35:50.232911 splink-3.8.1/splink/spark/custom_spark_dialect.py
--rw-r--r--   0        0        0      473 2023-04-27 19:35:50.232911 splink-3.8.1/splink/spark/jar_location.py
--rw-r--r--   0        0        0     1641 2023-04-27 19:35:50.232911 splink-3.8.1/splink/spark/spark_base.py
--rw-r--r--   0        0        0     2300 2023-04-27 19:35:50.232911 splink-3.8.1/splink/spark/spark_comparison_level_library.py
--rw-r--r--   0        0        0     1812 2023-04-27 19:35:50.232911 splink-3.8.1/splink/spark/spark_comparison_library.py
--rw-r--r--   0        0        0      538 2023-04-27 19:35:50.232911 splink-3.8.1/splink/spark/spark_comparison_template_library.py
--rw-r--r--   0        0        0    22331 2023-04-27 19:35:50.232911 splink-3.8.1/splink/spark/spark_linker.py
--rw-r--r--   0        0        0     4507 2023-04-27 19:35:50.232911 splink-3.8.1/splink/splink_comparison_viewer.py
--rw-r--r--   0        0        0     3220 2023-04-27 19:35:50.232911 splink-3.8.1/splink/splink_dataframe.py
--rw-r--r--   0        0        0     1181 2023-04-27 19:35:50.232911 splink-3.8.1/splink/sql_transform.py
--rw-r--r--   0        0        0      147 2023-04-27 19:35:50.232911 splink-3.8.1/splink/sqlite/sqlite_base.py
--rw-r--r--   0        0        0     1109 2023-04-27 19:35:50.232911 splink-3.8.1/splink/sqlite/sqlite_comparison_level_library.py
--rw-r--r--   0        0        0      379 2023-04-27 19:35:50.232911 splink-3.8.1/splink/sqlite/sqlite_comparison_library.py
--rw-r--r--   0        0        0     6052 2023-04-27 19:35:50.232911 splink-3.8.1/splink/sqlite/sqlite_linker.py
--rw-r--r--   0        0        0     4453 2023-04-27 19:35:50.232911 splink-3.8.1/splink/term_frequencies.py
--rw-r--r--   0        0        0     1030 2023-04-27 19:35:50.232911 splink-3.8.1/splink/unique_id_concat.py
--rw-r--r--   0        0        0     1424 2023-04-27 19:35:50.232911 splink-3.8.1/splink/unlinkables.py
--rw-r--r--   0        0        0     2431 2023-04-27 19:35:50.232911 splink-3.8.1/splink/validate_jsonschema.py
--rw-r--r--   0        0        0     2326 2023-04-27 19:35:50.232911 splink-3.8.1/splink/vertically_concatenate.py
--rw-r--r--   0        0        0     5342 2023-04-27 19:35:50.232911 splink-3.8.1/splink/waterfall_chart.py
--rw-r--r--   0        0        0     9374 1970-01-01 00:00:00.000000 splink-3.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-05-31 15:25:25.311725 splink-3.9.0/LICENSE
+-rw-r--r--   0        0        0     8777 2023-05-31 15:25:25.311725 splink-3.9.0/README.md
+-rw-r--r--   0        0        0     1799 2023-05-31 15:25:25.343744 splink-3.9.0/pyproject.toml
+-rw-r--r--   0        0        0       23 2023-05-31 15:25:25.347747 splink-3.9.0/splink/__init__.py
+-rw-r--r--   0        0        0    10852 2023-05-31 15:25:25.347747 splink-3.9.0/splink/accuracy.py
+-rw-r--r--   0        0        0     4759 2023-05-31 15:25:25.347747 splink-3.9.0/splink/analyse_blocking.py
+-rw-r--r--   0        0        0      366 2023-05-31 15:25:25.347747 splink-3.9.0/splink/athena/athena_comparison_level_library.py
+-rw-r--r--   0        0        0      221 2023-05-31 15:25:25.347747 splink-3.9.0/splink/athena/athena_comparison_library.py
+-rw-r--r--   0        0        0      252 2023-05-31 15:25:25.347747 splink-3.9.0/splink/athena/athena_comparison_template_library.py
+-rw-r--r--   0        0        0      661 2023-05-31 15:25:25.347747 splink-3.9.0/splink/athena/athena_helpers/athena_base.py
+-rw-r--r--   0        0        0     3120 2023-05-31 15:25:25.347747 splink-3.9.0/splink/athena/athena_helpers/athena_comparison_imports.py
+-rw-r--r--   0        0        0      350 2023-05-31 15:25:25.347747 splink-3.9.0/splink/athena/athena_helpers/athena_transforms.py
+-rw-r--r--   0        0        0     2903 2023-05-31 15:25:25.347747 splink-3.9.0/splink/athena/athena_helpers/athena_utils.py
+-rw-r--r--   0        0        0    20688 2023-05-31 15:25:25.347747 splink-3.9.0/splink/athena/athena_linker.py
+-rw-r--r--   0        0        0     2867 2023-05-31 15:25:25.347747 splink-3.9.0/splink/block_from_labels.py
+-rw-r--r--   0        0        0     6239 2023-05-31 15:25:25.347747 splink-3.9.0/splink/blocking.py
+-rw-r--r--   0        0        0    11739 2023-05-31 15:25:25.347747 splink-3.9.0/splink/charts.py
+-rw-r--r--   0        0        0     9088 2023-05-31 15:25:25.347747 splink-3.9.0/splink/cluster_studio.py
+-rw-r--r--   0        0        0    16881 2023-05-31 15:25:25.347747 splink-3.9.0/splink/comparison.py
+-rw-r--r--   0        0        0     8766 2023-05-31 15:25:25.347747 splink-3.9.0/splink/comparison_helpers.py
+-rw-r--r--   0        0        0      554 2023-05-31 15:25:25.347747 splink-3.9.0/splink/comparison_helpers_utils.py
+-rw-r--r--   0        0        0    25479 2023-05-31 15:25:25.347747 splink-3.9.0/splink/comparison_level.py
+-rw-r--r--   0        0        0    16492 2023-05-31 15:25:25.347747 splink-3.9.0/splink/comparison_level_composition.py
+-rw-r--r--   0        0        0    46215 2023-05-31 15:25:25.347747 splink-3.9.0/splink/comparison_level_library.py
+-rw-r--r--   0        0        0     1237 2023-05-31 15:25:25.347747 splink-3.9.0/splink/comparison_level_sql.py
+-rw-r--r--   0        0        0    54177 2023-05-31 15:25:25.347747 splink-3.9.0/splink/comparison_library.py
+-rw-r--r--   0        0        0     4727 2023-05-31 15:25:25.347747 splink-3.9.0/splink/comparison_library_utils.py
+-rw-r--r--   0        0        0    59497 2023-05-31 15:25:25.347747 splink-3.9.0/splink/comparison_template_library.py
+-rw-r--r--   0        0        0      972 2023-05-31 15:25:25.347747 splink-3.9.0/splink/comparison_vector_distribution.py
+-rw-r--r--   0        0        0      868 2023-05-31 15:25:25.347747 splink-3.9.0/splink/comparison_vector_values.py
+-rw-r--r--   0        0        0    16886 2023-05-31 15:25:25.347747 splink-3.9.0/splink/connected_components.py
+-rw-r--r--   0        0        0       67 2023-05-31 15:25:25.347747 splink-3.9.0/splink/constants.py
+-rw-r--r--   0        0        0     6089 2023-05-31 15:25:25.347747 splink-3.9.0/splink/convert_v2_to_v3.py
+-rw-r--r--   0        0        0     1338 2023-05-31 15:25:25.347747 splink-3.9.0/splink/databricks/enable_splink.py
+-rw-r--r--   0        0        0      609 2023-05-31 15:25:25.347747 splink-3.9.0/splink/default_from_jsonschema.py
+-rw-r--r--   0        0        0     1608 2023-05-31 15:25:25.347747 splink-3.9.0/splink/dialect_base.py
+-rw-r--r--   0        0        0      476 2023-05-31 15:25:25.347747 splink-3.9.0/splink/duckdb/duckdb_comparison_level_library.py
+-rw-r--r--   0        0        0      371 2023-05-31 15:25:25.347747 splink-3.9.0/splink/duckdb/duckdb_comparison_library.py
+-rw-r--r--   0        0        0      172 2023-05-31 15:25:25.347747 splink-3.9.0/splink/duckdb/duckdb_comparison_template_library.py
+-rw-r--r--   0        0        0     1532 2023-05-31 15:25:25.347747 splink-3.9.0/splink/duckdb/duckdb_helpers/duckdb_base.py
+-rw-r--r--   0        0        0     5597 2023-05-31 15:25:25.347747 splink-3.9.0/splink/duckdb/duckdb_helpers/duckdb_comparison_imports.py
+-rw-r--r--   0        0        0     1750 2023-05-31 15:25:25.347747 splink-3.9.0/splink/duckdb/duckdb_helpers/duckdb_helpers.py
+-rw-r--r--   0        0        0    11482 2023-05-31 15:25:25.347747 splink-3.9.0/splink/duckdb/duckdb_linker.py
+-rw-r--r--   0        0        0    17471 2023-05-31 15:25:25.347747 splink-3.9.0/splink/em_training_session.py
+-rw-r--r--   0        0        0     5244 2023-05-31 15:25:25.347747 splink-3.9.0/splink/estimate_u.py
+-rw-r--r--   0        0        0      144 2023-05-31 15:25:25.347747 splink-3.9.0/splink/exceptions.py
+-rw-r--r--   0        0        0     7333 2023-05-31 15:25:25.347747 splink-3.9.0/splink/expectation_maximisation.py
+-rw-r--r--   0        0        0     1558 2023-05-31 15:25:25.347747 splink-3.9.0/splink/files/chart_defs/blocking_rule_generated_comparisons.json
+-rw-r--r--   0        0        0     5212 2023-05-31 15:25:25.347747 splink-3.9.0/splink/files/chart_defs/comparator_score_chart.json
+-rw-r--r--   0        0        0     1907 2023-05-31 15:25:25.347747 splink-3.9.0/splink/files/chart_defs/comparator_score_threshold_chart.json
+-rw-r--r--   0        0        0     2779 2023-05-31 15:25:25.347747 splink-3.9.0/splink/files/chart_defs/completeness.json
+-rw-r--r--   0        0        0     6737 2023-05-31 15:25:25.347747 splink-3.9.0/splink/files/chart_defs/del/bayes_factor_history_chart_def.json
+-rw-r--r--   0        0        0     7747 2023-05-31 15:25:25.347747 splink-3.9.0/splink/files/chart_defs/del/bayes_factor_intuition_chart_def.json
+-rw-r--r--   0        0        0     6298 2023-05-31 15:25:25.347747 splink-3.9.0/splink/files/chart_defs/del/compare_estimates.json
+-rw-r--r--   0        0        0     2155 2023-05-31 15:25:25.347747 splink-3.9.0/splink/files/chart_defs/del/gamma_distribution_chart_def.json
+-rw-r--r--   0        0        0      743 2023-05-31 15:25:25.347747 splink-3.9.0/splink/files/chart_defs/del/gamma_histogram.json
+-rw-r--r--   0        0        0     1309 2023-05-31 15:25:25.347747 splink-3.9.0/splink/files/chart_defs/del/score_histogram.json
+-rw-r--r--   0        0        0     5831 2023-05-31 15:25:25.347747 splink-3.9.0/splink/files/chart_defs/m_u_parameters_interactive_history.json
+-rw-r--r--   0        0        0      977 2023-05-31 15:25:25.347747 splink-3.9.0/splink/files/chart_defs/match_weight_histogram.json
+-rw-r--r--   0        0        0     5766 2023-05-31 15:25:25.347747 splink-3.9.0/splink/files/chart_defs/match_weights_interactive_history.json
+-rw-r--r--   0        0        0     9159 2023-05-31 15:25:25.347747 splink-3.9.0/splink/files/chart_defs/match_weights_waterfall.json
+-rw-r--r--   0        0        0     1734 2023-05-31 15:25:25.347747 splink-3.9.0/splink/files/chart_defs/missingness.json
+-rw-r--r--   0        0        0     1730 2023-05-31 15:25:25.347747 splink-3.9.0/splink/files/chart_defs/parameter_estimate_comparisons.json
+-rw-r--r--   0        0        0     1962 2023-05-31 15:25:25.347747 splink-3.9.0/splink/files/chart_defs/phonetic_match_chart.json
+-rw-r--r--   0        0        0     1465 2023-05-31 15:25:25.347747 splink-3.9.0/splink/files/chart_defs/precision_recall.json
+-rw-r--r--   0        0        0     1123 2023-05-31 15:25:25.347747 splink-3.9.0/splink/files/chart_defs/probability_two_random_records_match_iteration.json
+-rw-r--r--   0        0        0     2326 2023-05-31 15:25:25.347747 splink-3.9.0/splink/files/chart_defs/profile_data.json
+-rw-r--r--   0        0        0     1745 2023-05-31 15:25:25.347747 splink-3.9.0/splink/files/chart_defs/roc.json
+-rw-r--r--   0        0        0     9924 2023-05-31 15:25:25.347747 splink-3.9.0/splink/files/chart_defs/tf_adjustment_chart.json
+-rw-r--r--   0        0        0     2645 2023-05-31 15:25:25.347747 splink-3.9.0/splink/files/chart_defs/unlinkables_chart_def.json
+-rw-r--r--   0        0        0    66064 2023-05-31 15:25:25.351749 splink-3.9.0/splink/files/external_js/vega-embed@6.20.2
+-rw-r--r--   0        0        0   256817 2023-05-31 15:25:25.351749 splink-3.9.0/splink/files/external_js/vega-lite@5.2.0
+-rw-r--r--   0        0        0   501599 2023-05-31 15:25:25.355752 splink-3.9.0/splink/files/external_js/vega@5.21.0
+-rw-r--r--   0        0        0    12871 2023-05-31 15:25:25.355752 splink-3.9.0/splink/files/settings_jsonschema.json
+-rw-r--r--   0        0        0  1228220 2023-05-31 15:25:25.363757 splink-3.9.0/splink/files/spark_jars/scala-udf-similarity-0.1.0_classic.jar
+-rw-r--r--   0        0        0   944614 2023-05-31 15:25:25.367759 splink-3.9.0/splink/files/spark_jars/scala-udf-similarity-0.1.0_spark3.3.jar
+-rw-r--r--   0        0        0   949562 2023-05-31 15:25:25.367759 splink-3.9.0/splink/files/spark_jars/scala-udf-similarity-0.1.1_spark3.x.jar
+-rw-r--r--   0        0        0     5486 2023-05-31 15:25:25.367759 splink-3.9.0/splink/files/splink_cluster_studio/cluster_template.j2
+-rw-r--r--   0        0        0     2269 2023-05-31 15:25:25.367759 splink-3.9.0/splink/files/splink_cluster_studio/custom.css
+-rw-r--r--   0        0        0     2269 2023-05-31 15:25:25.367759 splink-3.9.0/splink/files/splink_comparison_viewer/custom.css
+-rw-r--r--   0        0        0     3115 2023-05-31 15:25:25.367759 splink-3.9.0/splink/files/splink_comparison_viewer/template.j2
+-rw-r--r--   0        0        0   269522 2023-05-31 15:25:25.367759 splink-3.9.0/splink/files/splink_vis_utils/splink_vis_utils.js
+-rw-r--r--   0        0        0      404 2023-05-31 15:25:25.367759 splink-3.9.0/splink/files/templates/single_chart_template.txt
+-rw-r--r--   0        0        0      195 2023-05-31 15:25:25.367759 splink-3.9.0/splink/format_sql.py
+-rw-r--r--   0        0        0     7955 2023-05-31 15:25:25.367759 splink-3.9.0/splink/input_column.py
+-rw-r--r--   0        0        0   124599 2023-05-31 15:25:25.367759 splink-3.9.0/splink/linker.py
+-rw-r--r--   0        0        0      300 2023-05-31 15:25:25.367759 splink-3.9.0/splink/logging_messages.py
+-rw-r--r--   0        0        0     3132 2023-05-31 15:25:25.367759 splink-3.9.0/splink/lower_id_on_lhs.py
+-rw-r--r--   0        0        0     1834 2023-05-31 15:25:25.367759 splink-3.9.0/splink/m_from_labels.py
+-rw-r--r--   0        0        0     2465 2023-05-31 15:25:25.367759 splink-3.9.0/splink/m_training.py
+-rw-r--r--   0        0        0     2420 2023-05-31 15:25:25.367759 splink-3.9.0/splink/m_u_records_to_parameters.py
+-rw-r--r--   0        0        0      623 2023-05-31 15:25:25.367759 splink-3.9.0/splink/match_key_analysis.py
+-rw-r--r--   0        0        0     2028 2023-05-31 15:25:25.367759 splink-3.9.0/splink/match_weights_histogram.py
+-rw-r--r--   0        0        0     4548 2023-05-31 15:25:25.367759 splink-3.9.0/splink/misc.py
+-rw-r--r--   0        0        0     2791 2023-05-31 15:25:25.367759 splink-3.9.0/splink/missingness.py
+-rw-r--r--   0        0        0     1221 2023-05-31 15:25:25.367759 splink-3.9.0/splink/parse_sql.py
+-rw-r--r--   0        0        0     2909 2023-05-31 15:25:25.367759 splink-3.9.0/splink/pipeline.py
+-rw-r--r--   0        0        0     3205 2023-05-31 15:25:25.367759 splink-3.9.0/splink/predict.py
+-rw-r--r--   0        0        0     8245 2023-05-31 15:25:25.367759 splink-3.9.0/splink/profile_data.py
+-rw-r--r--   0        0        0    18694 2023-05-31 15:25:25.367759 splink-3.9.0/splink/settings.py
+-rw-r--r--   0        0        0      473 2023-05-31 15:25:25.367759 splink-3.9.0/splink/spark/jar_location.py
+-rw-r--r--   0        0        0      474 2023-05-31 15:25:25.367759 splink-3.9.0/splink/spark/spark_comparison_level_library.py
+-rw-r--r--   0        0        0      369 2023-05-31 15:25:25.367759 splink-3.9.0/splink/spark/spark_comparison_library.py
+-rw-r--r--   0        0        0      170 2023-05-31 15:25:25.367759 splink-3.9.0/splink/spark/spark_comparison_template_library.py
+-rw-r--r--   0        0        0     1083 2023-05-31 15:25:25.367759 splink-3.9.0/splink/spark/spark_helpers/custom_spark_dialect.py
+-rw-r--r--   0        0        0     2280 2023-05-31 15:25:25.367759 splink-3.9.0/splink/spark/spark_helpers/spark_base.py
+-rw-r--r--   0        0        0     5565 2023-05-31 15:25:25.367759 splink-3.9.0/splink/spark/spark_helpers/spark_comparison_imports.py
+-rw-r--r--   0        0        0    23101 2023-05-31 15:25:25.367759 splink-3.9.0/splink/spark/spark_linker.py
+-rw-r--r--   0        0        0     4507 2023-05-31 15:25:25.367759 splink-3.9.0/splink/splink_comparison_viewer.py
+-rw-r--r--   0        0        0     3836 2023-05-31 15:25:25.367759 splink-3.9.0/splink/splink_dataframe.py
+-rw-r--r--   0        0        0     1181 2023-05-31 15:25:25.367759 splink-3.9.0/splink/sql_transform.py
+-rw-r--r--   0        0        0      313 2023-05-31 15:25:25.371761 splink-3.9.0/splink/sqlite/sqlite_comparison_level_library.py
+-rw-r--r--   0        0        0      157 2023-05-31 15:25:25.371761 splink-3.9.0/splink/sqlite/sqlite_comparison_library.py
+-rw-r--r--   0        0        0      390 2023-05-31 15:25:25.371761 splink-3.9.0/splink/sqlite/sqlite_comparison_template_library.py
+-rw-r--r--   0        0        0      148 2023-05-31 15:25:25.371761 splink-3.9.0/splink/sqlite/sqlite_helpers/sqlite_base.py
+-rw-r--r--   0        0        0     2061 2023-05-31 15:25:25.371761 splink-3.9.0/splink/sqlite/sqlite_helpers/sqlite_comparison_imports.py
+-rw-r--r--   0        0        0     6159 2023-05-31 15:25:25.371761 splink-3.9.0/splink/sqlite/sqlite_linker.py
+-rw-r--r--   0        0        0    10207 2023-05-31 15:25:25.371761 splink-3.9.0/splink/term_frequencies.py
+-rw-r--r--   0        0        0     1030 2023-05-31 15:25:25.371761 splink-3.9.0/splink/unique_id_concat.py
+-rw-r--r--   0        0        0     1424 2023-05-31 15:25:25.371761 splink-3.9.0/splink/unlinkables.py
+-rw-r--r--   0        0        0     2431 2023-05-31 15:25:25.371761 splink-3.9.0/splink/validate_jsonschema.py
+-rw-r--r--   0        0        0     2326 2023-05-31 15:25:25.371761 splink-3.9.0/splink/vertically_concatenate.py
+-rw-r--r--   0        0        0     5342 2023-05-31 15:25:25.371761 splink-3.9.0/splink/waterfall_chart.py
+-rw-r--r--   0        0        0     9745 1970-01-01 00:00:00.000000 splink-3.9.0/PKG-INFO
```

### Comparing `splink-3.8.1/LICENSE` & `splink-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/README.md` & `splink-3.9.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,35 +8,35 @@
 
 # Fast, accurate and scalable probabilistic data linkage
 
 Splink is a Python package for probabilistic record linkage (entity resolution) that allows you to deduplicate and link records from datasets without unique identifiers.
 
 ## Key Features
 
-⚡ **Speed:** Capable of linking a million records on a laptop in approximately one minute.  
-🎯 **Accuracy:** Full support for term frequency adjustments and user-defined fuzzy matching logic.  
-🌐 **Scalability:** Execute linkage jobs in Python (using DuckDB) or big-data backends like AWS Athena or Spark for 100+ million records.  
-🎓 **Unsupervised Learning:** No training data is required, as models can be trained using an unsupervised approach.  
+⚡ **Speed:** Capable of linking a million records on a laptop in approximately one minute.
+🎯 **Accuracy:** Full support for term frequency adjustments and user-defined fuzzy matching logic.
+🌐 **Scalability:** Execute linkage jobs in Python (using DuckDB) or big-data backends like AWS Athena or Spark for 100+ million records.
+🎓 **Unsupervised Learning:** No training data is required, as models can be trained using an unsupervised approach.
 📊 **Interactive Outputs:** Provides a wide range of interactive outputs to help users understand their model and diagnose linkage problems.
 
 Splink's core linkage algorithm is based on Fellegi-Sunter's model of record linkage, with various customizations to improve accuracy.
 
 ## What does Splink do?
 
 Consider the following records that lack a unique person identifier:
 
-![tables showing what splink does](https://raw.githubusercontent.com/moj-analytical-services/splink/master/docs/img/main_readme_what_does_splink_do_1.drawio.png)
+![tables showing what splink does](https://raw.githubusercontent.com/moj-analytical-services/splink/master/docs/img/README/what_does_splink_do_1.drawio.png)
 
 Splink predicts which rows link together:
 
-![tables showing what splink does](https://raw.githubusercontent.com/moj-analytical-services/splink/master/docs/img/main_readme_what_does_splink_do_2.drawio.png)
+![tables showing what splink does](https://raw.githubusercontent.com/moj-analytical-services/splink/master/docs/img/README/what_does_splink_do_2.drawio.png)
 
 and clusters these links to produce an estimated person ID:
 
-![tables showing what splink does](https://raw.githubusercontent.com/moj-analytical-services/splink/master/docs/img/main_readme_what_does_splink_do_3.drawio.png)
+![tables showing what splink does](https://raw.githubusercontent.com/moj-analytical-services/splink/master/docs/img/README/what_does_splink_do_3.drawio.png)
 
 ## What data does Splink work best with?
 
 Before using Splink, input data should be standardized, with consistent column names and formatting (e.g., lowercased, punctuation cleaned up, etc.).
 
 Splink performs best with input data containing **multiple** columns that are **not highly correlated**. For instance, if the entity type is persons, you may have columns for full name, date of birth, and city. If the entity type is companies, you could have columns for name, turnover, sector, and telephone number.
 
@@ -64,43 +64,44 @@
 
 or, if you prefer, you can instead install splink using conda:
 
 ```sh
 conda install -c conda-forge splink
 ```
 
+Should you require a more bare-bones version of Splink **without DuckDB**, please see the following area of the docs:
+> [DuckDBless Splink Installation](https://moj-analytical-services.github.io/splink/installations.html#duckdb-less-installation)
+
 ## Quickstart
 
 The following code demonstrates how to estimate the parameters of a deduplication model, use it to identify duplicate records, and then use clustering to generate an estimated unique person ID.
 
 For more detailed tutorials, please see [here](https://moj-analytical-services.github.io/splink/demos/00_Tutorial_Introduction.html).
 
 ```py
 from splink.duckdb.duckdb_linker import DuckDBLinker
-from splink.duckdb.duckdb_comparison_library import (
-    exact_match,
-    levenshtein_at_thresholds,
-)
+import splink.duckdb.duckdb_comparison_library as cl
+import splink.duckdb.duckdb_comparison_template_library as ctl
 
 import pandas as pd
 
 df = pd.read_csv("./tests/datasets/fake_1000_from_splink_demos.csv")
 
 settings = {
     "link_type": "dedupe_only",
     "blocking_rules_to_generate_predictions": [
         "l.first_name = r.first_name",
         "l.surname = r.surname",
     ],
     "comparisons": [
-        levenshtein_at_thresholds("first_name", 2),
-        exact_match("surname"),
-        exact_match("dob"),
-        exact_match("city", term_frequency_adjustments=True),
-        exact_match("email"),
+        ctl.name_comparison("first_name"),
+        ctl.name_comparison("surname"),
+        ctl.date_comparison("dob", cast_strings_to_date=True),
+        cl.exact_match("city", term_frequency_adjustments=True),
+        cl.levenshtein_at_thresholds("email", 2),
     ],
 }
 
 linker = DuckDBLinker(df, settings)
 linker.estimate_u_using_random_sampling(max_pairs=1e6)
 
 blocking_rule_for_training = "l.first_name = r.first_name and l.surname = r.surname"
@@ -137,15 +138,15 @@
 ## Citation
 
 If you use Splink in your research, we'd be grateful for a citation as follows:
 
 ```BibTeX
 @article{Linacre_Lindsay_Manassis_Slade_Hepworth_2022,
 	title        = {Splink: Free software for probabilistic record linkage at scale.},
-	author       = {Linacre, Robin and Lindsay, Sam and Manassis, Theodore and Slade, Zoe and Hepworth, Tom},
+	author       = {Linacre, Robin and Lindsay, Sam and Manassis, Theodore and Slade, Zoe and Hepworth, Tom and Kennedy, Ross and Bond, Andrew},
 	year         = 2022,
 	month        = {Aug.},
 	journal      = {International Journal of Population Data Science},
 	volume       = 7,
 	number       = 3,
 	doi          = {10.23889/ijpds.v7i3.1794},
 	url          = {https://ijpds.org/article/view/1794},
```

### Comparing `splink-3.8.1/pyproject.toml` & `splink-3.9.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "splink"
-version = "3.8.1"
+version = "3.9.0"
 description = "Fast probabilistic data linkage at scale"
 authors = ["Robin Linacre <robinlinacre@hotmail.com>", "Sam Lindsay", "Theodore Manassis", "Tom Hepworth", "Andy Bond", "Ross Kennedy"]
 license = "MIT"
 homepage = "https://github.com/moj-analytical-services/splink"
 repository = "https://github.com/moj-analytical-services/splink"
 readme = "README.md"
 
@@ -12,14 +12,15 @@
 python = ">=3.7"
 jsonschema = ">=3.2,<5.0"
 pandas = ">=1.0.0"
 duckdb = ">=0.6.0"
 sqlglot = ">=5.1.0"
 altair = ">=4.2.0"
 Jinja2 = ">=3.0.3"
+phonetics = "^1.0.5"
 
 [tool.poetry.group.dev]
 [tool.poetry.group.dev.dependencies]
 tabulate = "0.8.9"
 pyspark = "^3.2.1"
 
 [tool.poetry.group.linting]
@@ -58,7 +59,24 @@
     # bugbear
     "B",
 ]
 ignore = [
     "B905", # `zip()` without an explicit `strict=` parameter
     "B006", # Do not use mutable data structures for argument defaults"
 ]
+
+[tool.pytest.ini_options]
+addopts = ["-m default"]
+markers = [
+# only tests where backend is irrelevant:
+    "core",
+# see tests/decorator.py::dialect_groups for group details:
+    "default",
+    "all",
+# backend-specific sets
+    "duckdb",
+    "duckdb_only",
+    "spark",
+    "spark_only",
+    "sqlite",
+    "sqlite_only",
+]
```

### Comparing `splink-3.8.1/splink/accuracy.py` & `splink-3.9.0/splink/accuracy.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/analyse_blocking.py` & `splink-3.9.0/splink/analyse_blocking.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/athena/athena_linker.py` & `splink-3.9.0/splink/athena/athena_linker.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 import os
 
 import awswrangler as wr
 import boto3
 import numpy as np
 import pandas as pd
 
-from ..athena.athena_transforms import cast_concat_as_varchar
-from ..athena.athena_utils import (
-    _garbage_collection,
-    _verify_athena_inputs,
-)
 from ..input_column import InputColumn
 from ..linker import Linker
 from ..logging_messages import execute_sql_logging_message_info, log_sql
 from ..misc import ensure_is_list
 from ..splink_dataframe import SplinkDataFrame
 from ..sql_transform import sqlglot_transform_sql
+from .athena_helpers.athena_transforms import cast_concat_as_varchar
+from .athena_helpers.athena_utils import (
+    _garbage_collection,
+    _verify_athena_inputs,
+)
 
 logger = logging.getLogger(__name__)
 
 
 class AthenaDataFrame(SplinkDataFrame):
     linker: AthenaLinker
 
@@ -320,24 +320,26 @@
                 raise ValueError(
                     f"Table '{table_name}' already exists in database. "
                     "Please use the 'overwrite' argument if you wish to overwrite"
                 )
             else:
                 self._delete_table_from_database(table_name)
 
+        self._table_registration(input, table_name)
+        return self._table_to_splink_dataframe(table_name, table_name)
+
+    def _table_registration(self, input, table_name):
         if isinstance(input, dict):
             input = pd.DataFrame(input)
         elif isinstance(input, list):
             input = pd.DataFrame.from_records(input)
 
         # Errors if an invalid data type is passed
         self.register_data_on_s3(input, table_name)
 
-        return self._table_to_splink_dataframe(table_name, table_name)
-
     def _random_sample_sql(self, proportion, sample_size, seed=None):
         if proportion == 1.0:
             return ""
         percent = proportion * 100
         return f" TABLESAMPLE BERNOULLI ({percent})"
 
     @property
@@ -393,15 +395,14 @@
                 use_threads=True,
                 boto3_session=self.boto3_session,
             )
 
         self.ctas_query_info.pop(physical_name)
 
     def _delete_table_from_database(self, name):
-
         if name in self.ctas_query_info:
             # Use ctas metadata to delete backing data
             self._delete_table_from_s3(name)
         else:
             # If the location we want to write to already exists,
             # clean this before continuing.
             loc = f"{self.s3_output}{name}"
```

### Comparing `splink-3.8.1/splink/athena/athena_utils.py` & `splink-3.9.0/splink/athena/athena_helpers/athena_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
         "'awswrangler.athena.create_athena_bucket' for buckets or "
         "'awswrangler.catalog.create_database' for databases using the "
         "awswrangler API."
     )
 
 
 def _verify_athena_inputs(database, bucket, boto3_session):
-
     errors = []
 
     if (
         database
         not in wr.catalog.databases(limit=None, boto3_session=boto3_session).values
     ):
         errors.append(f"database '{database}'")
```

### Comparing `splink-3.8.1/splink/block_from_labels.py` & `splink-3.9.0/splink/block_from_labels.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/blocking.py` & `splink-3.9.0/splink/blocking.py`

 * *Files 6% similar despite different names*

```diff
@@ -142,28 +142,36 @@
     # Cover the case where there are no blocking rules
     # This is a bit of a hack where if you do a self-join on 'true'
     # you create a cartesian product, rather than having separate code
     # that generates a cross join for the case of no blocking rules
     if not blocking_rules:
         blocking_rules = [BlockingRule("1=1")]
 
+    # For Blocking rules for deterministic rules, add a match probability
+    # column with all probabilities set to 1.
+    if linker._deterministic_link_mode:
+        probability = ", 1.00 as match_probability"
+    else:
+        probability = ""
+
     sqls = []
     for br in blocking_rules:
         # Apply our salted rules to resolve skew issues. If no salt was
         # selected to be added, then apply the initial blocking rule.
         if apply_salt:
             salted_blocking_rules = br.salted_blocking_rules
         else:
             salted_blocking_rules = [br.blocking_rule]
 
         for salted_br in salted_blocking_rules:
             sql = f"""
             select
             {sql_select_expr}
             , '{br.match_key}' as match_key
+            {probability}
             from {linker._input_tablename_l} as l
             inner join {linker._input_tablename_r} as r
             on
             {salted_br}
             {br.and_not_preceding_rules_sql}
             {where_condition}
             """
```

### Comparing `splink-3.8.1/splink/charts.py` & `splink-3.9.0/splink/charts.py`

 * *Files 4% similar despite different names*

```diff
@@ -346,7 +346,42 @@
 def cumulative_blocking_rule_comparisons_generated(records, as_dict=False):
     chart_path = "blocking_rule_generated_comparisons.json"
     chart = load_chart_definition(chart_path)
 
     chart["data"]["values"] = records
 
     return vegalite_or_json(chart, as_dict=as_dict)
+
+
+def _comparator_score_chart(similarity_records, distance_records, as_dict=False):
+    chart_path = "comparator_score_chart.json"
+    chart = load_chart_definition(chart_path)
+
+    chart["datasets"]["data-similarity"] = similarity_records
+    chart["datasets"]["data-distance"] = distance_records
+
+    return vegalite_or_json(chart, as_dict=as_dict)
+
+
+def _comparator_score_threshold_chart(
+    records, similarity_threshold, distance_threshold, as_dict=False
+):
+    chart_path = "comparator_score_threshold_chart.json"
+    chart = load_chart_definition(chart_path)
+
+    chart["layer"][0]["title"] = (
+        f"Heatmap of Matches for "
+        f"distance_threshold = {distance_threshold}, "
+        f"similarity_threshold = {similarity_threshold}"
+    )
+    chart["datasets"]["data-with-thresholds"] = records
+
+    return vegalite_or_json(chart, as_dict=as_dict)
+
+
+def _phonetic_match_chart(records, as_dict=False):
+    chart_path = "phonetic_match_chart.json"
+    chart = load_chart_definition(chart_path)
+
+    chart["datasets"]["data-phonetic"] = records
+
+    return vegalite_or_json(chart, as_dict=as_dict)
```

### Comparing `splink-3.8.1/splink/cluster_studio.py` & `splink-3.9.0/splink/cluster_studio.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/comparison.py` & `splink-3.9.0/splink/comparison.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/comparison_level.py` & `splink-3.9.0/splink/comparison_level.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/comparison_level_sql.py` & `splink-3.9.0/splink/comparison_level_sql.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/comparison_library_utils.py` & `splink-3.9.0/splink/comparison_library_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,15 +63,17 @@
 
 
 def distance_threshold_comparison_levels(
     self,
     col_name: str,
     distance_function_name: str,
     distance_threshold_or_thresholds,
+    regex_extract: str = None,
     higher_is_more_similar: bool = True,
+    include_colname_in_charts_label=False,
     m_probability_or_probabilities_thres: list = None,
 ):
     thresholds = ensure_is_iterable(distance_threshold_or_thresholds)
     threshold_comparison_levels = []
 
     if m_probability_or_probabilities_thres is None:
         m_probability_or_probabilities_thres = [None] * len(thresholds)
@@ -79,26 +81,35 @@
         m_probability_or_probabilities_thres
     )
 
     for thres, m_prob in zip(thresholds, m_probability_or_probabilities_thres):
         if distance_function_name == "levenshtein":
             distance_function_name = self._levenshtein_name
             higher_is_more_similar = False
+        elif distance_function_name == "damerau-levenshtein":
+            distance_function_name = self._damerau_levenshtein_name
+            higher_is_more_similar = False
         elif distance_function_name == "jaro":
             distance_function_name = self._jaro_name
             higher_is_more_similar = True
         elif distance_function_name == "jaro-winkler":
             distance_function_name = self._jaro_winkler_name
             higher_is_more_similar = True
         elif distance_function_name == "jaccard":
             distance_function_name = self._jaccard_name
             higher_is_more_similar = True
 
         # these function arguments hold for all cases.
-        kwargs = dict(col_name=col_name, distance_threshold=thres, m_probability=m_prob)
+        kwargs = dict(
+            col_name=col_name,
+            distance_threshold=thres,
+            include_colname_in_charts_label=include_colname_in_charts_label,
+            regex_extract=regex_extract,
+            m_probability=m_prob,
+        )
         # separate out the two that are only used
         # when we have a user-supplied function, rather than a predefined subclass
         # feels a bit hacky, but will do at least for time being
         if not self._is_distance_subclass:
             kwargs["distance_function_name"] = distance_function_name
             kwargs["higher_is_more_similar"] = higher_is_more_similar
```

### Comparing `splink-3.8.1/splink/comparison_vector_distribution.py` & `splink-3.9.0/splink/comparison_vector_distribution.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/comparison_vector_values.py` & `splink-3.9.0/splink/comparison_vector_values.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/connected_components.py` & `splink-3.9.0/splink/connected_components.py`

 * *Files 4% similar despite different names*

```diff
@@ -291,15 +291,18 @@
             where rep_match
         """
 
     return sql
 
 
 def _cc_create_unique_id_cols(
-    linker: "Linker", concat_with_tf: str, df_predict: str, match_probability_threshold
+    linker: "Linker",
+    concat_with_tf: str,
+    df_predict: str,
+    match_probability_threshold: float,
 ):
     """Create SQL to pull unique ID columns for connected components.
 
     Takes the output of linker.predict() and either creates unique IDs for
     our linked dataframes, if we are performing a link job, or pulls out
     the unique ID columns if deduping.
 
@@ -313,27 +316,36 @@
             and connected in our algorithm.
 
     Returns:
         SplinkDataFrame: A dataframe containing two sets of unique IDs,
         unique_id_l and unique_id_r.
 
     """
+    # Set probability threshold
+    if linker._deterministic_link_mode:
+        match_probability_condition = ""
+    elif match_probability_threshold is None:
+        raise TypeError("Parameter 'match_probability_threshold' is missing or None")
+    else:
+        match_probability_condition = (
+            f"where match_probability >= {match_probability_threshold}"
+        )
 
     uid_cols = linker._settings_obj._unique_id_input_columns
     uid_concat_edges_l = _composite_unique_id_from_edges_sql(uid_cols, "l")
     uid_concat_edges_r = _composite_unique_id_from_edges_sql(uid_cols, "r")
     uid_concat_edges = _composite_unique_id_from_edges_sql(uid_cols, None)
 
     # Generate new unique IDs for our linked dataframes.
     sql = f"""
         select
         {uid_concat_edges_l} as unique_id_l,
         {uid_concat_edges_r} as unique_id_r
         from {df_predict}
-        where match_probability >= {match_probability_threshold}
+        {match_probability_condition}
 
         UNION
 
         select
         {uid_concat_edges} as unique_id_l,
         {uid_concat_edges} as unique_id_r
         from {concat_with_tf}
```

### Comparing `splink-3.8.1/splink/convert_v2_to_v3.py` & `splink-3.9.0/splink/convert_v2_to_v3.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/databricks/enable_splink.py` & `splink-3.9.0/splink/databricks/enable_splink.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/default_from_jsonschema.py` & `splink-3.9.0/splink/default_from_jsonschema.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/dialect_base.py` & `splink-3.9.0/splink/dialect_base.py`

 * *Files 25% similar despite different names*

```diff
@@ -23,18 +23,28 @@
             f"Datediff function not defined for "
             f"object of type {type(self)}.  "
             f"Have you remembered to use dialect-specific "
             f"comparisons/comparison levels?"
         )
 
     @property
+    def _regex_extract_function(self):
+        raise NotImplementedError(
+            "Regex extract option not defined for " "the SQL backend being used.  "
+        )
+
+    @property
     def _levenshtein_name(self):
         return "levenshtein"
 
     @property
+    def _damerau_levenshtein_name(self):
+        return "damerau_levenshtein"
+
+    @property
     def _jaro_name(self):
         return "jaro"
 
     @property
     def _jaro_winkler_name(self):
         return "jaro_winkler"
```

### Comparing `splink-3.8.1/splink/duckdb/duckdb_base.py` & `splink-3.9.0/splink/duckdb/duckdb_helpers/duckdb_base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..dialect_base import (
+from ...dialect_base import (
     DialectBase,
 )
 
 
 def size_array_intersect_sql(col_name_l, col_name_r):
     # sum of individual (unique) array sizes, minus the (unique) union
     return (
@@ -31,27 +31,37 @@
     else:
         return f"""
             abs(date_diff('{date_metric}', {col_name_l},
               {col_name_r})) <= {date_threshold}
         """
 
 
+def regex_extract_sql(col_name, regex):
+    return f"""
+        regexp_extract({col_name}, '{regex}')
+    """
+
+
 class DuckDBBase(DialectBase):
     @property
     def _sql_dialect(self):
         return "duckdb"
 
     @property
     def _size_array_intersect_function(self):
         return size_array_intersect_sql
 
     @property
     def _datediff_function(self):
         return datediff_sql
 
     @property
+    def _regex_extract_function(self):
+        return regex_extract_sql
+
+    @property
     def _jaro_name(self):
         return "jaro_similarity"
 
     @property
     def _jaro_winkler_name(self):
         return "jaro_winkler_similarity"
```

### Comparing `splink-3.8.1/splink/duckdb/duckdb_comparison_level_library.py` & `splink-3.9.0/splink/sqlite/sqlite_helpers/sqlite_comparison_imports.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,118 +1,96 @@
-from ..comparison_level_composition import and_, not_, or_  # noqa: F401
-from ..comparison_level_library import (
-    ArrayIntersectLevelBase,
+from ...comparison_level_library import (
     ColumnsReversedLevelBase,
-    DateDiffLevelBase,
     DistanceFunctionLevelBase,
-    DistanceInKMLevelBase,
     ElseLevelBase,
     ExactMatchLevelBase,
-    JaccardLevelBase,
-    JaroLevelBase,
-    JaroWinklerLevelBase,
     LevenshteinLevelBase,
     NullLevelBase,
     PercentageDifferenceLevelBase,
 )
-from .duckdb_base import (
-    DuckDBBase,
+from ...comparison_library import (
+    DistanceFunctionAtThresholdsComparisonBase,
+    ExactMatchBase,
+    LevenshteinAtThresholdsComparisonBase,
+)
+from .sqlite_base import (
+    SqliteBase,
 )
 
 
 # Class used to feed our comparison_library classes
-class DuckDBComparisonProperties(DuckDBBase):
+class SqliteComparisonProperties(SqliteBase):
     @property
     def _exact_match_level(self):
         return exact_match_level
 
     @property
     def _null_level(self):
         return null_level
 
     @property
     def _else_level(self):
         return else_level
 
     @property
-    def _datediff_level(self):
-        return datediff_level
-
-    @property
-    def _array_intersect_level(self):
-        return array_intersect_level
-
-    @property
-    def _distance_in_km_level(self):
-        return distance_in_km_level
-
-    @property
     def _distance_function_level(self):
         return distance_function_level
 
     @property
     def _levenshtein_level(self):
         return levenshtein_level
 
     @property
-    def _jaro_level(self):
-        return jaro_level
-
-    @property
-    def _jaro_winkler_level(self):
-        return jaro_winkler_level
-
-    @property
-    def _jaccard_level(self):
-        return jaccard_level
+    def _columns_reversed_level(self):
+        return columns_reversed_level
 
 
-class null_level(DuckDBBase, NullLevelBase):
+#########################
+### COMPARISON LEVELS ###
+#########################
+class null_level(SqliteBase, NullLevelBase):
     pass
 
 
-class exact_match_level(DuckDBBase, ExactMatchLevelBase):
+class exact_match_level(SqliteBase, ExactMatchLevelBase):
     pass
 
 
-class else_level(DuckDBBase, ElseLevelBase):
+class else_level(SqliteBase, ElseLevelBase):
     pass
 
 
-class columns_reversed_level(DuckDBBase, ColumnsReversedLevelBase):
+class levenshtein_level(SqliteBase, LevenshteinLevelBase):
     pass
 
 
-class distance_function_level(DuckDBBase, DistanceFunctionLevelBase):
+class columns_reversed_level(SqliteBase, ColumnsReversedLevelBase):
     pass
 
 
-class levenshtein_level(DuckDBBase, LevenshteinLevelBase):
+class distance_function_level(SqliteBase, DistanceFunctionLevelBase):
     pass
 
 
-class jaro_level(DuckDBBase, JaroLevelBase):
+class percentage_difference_level(SqliteBase, PercentageDifferenceLevelBase):
     pass
 
 
-class jaro_winkler_level(DuckDBBase, JaroWinklerLevelBase):
+##########################
+### COMPARISON LIBRARY ###
+##########################
+class exact_match(SqliteComparisonProperties, ExactMatchBase):
     pass
 
 
-class jaccard_level(DuckDBBase, JaccardLevelBase):
+class distance_function_at_thresholds(
+    SqliteComparisonProperties, DistanceFunctionAtThresholdsComparisonBase
+):
     pass
 
 
-class array_intersect_level(DuckDBBase, ArrayIntersectLevelBase):
-    pass
-
-
-class percentage_difference_level(DuckDBBase, PercentageDifferenceLevelBase):
-    pass
-
-
-class distance_in_km_level(DuckDBBase, DistanceInKMLevelBase):
-    pass
-
-
-class datediff_level(DuckDBBase, DateDiffLevelBase):
-    pass
+class levenshtein_at_thresholds(
+    SqliteComparisonProperties, LevenshteinAtThresholdsComparisonBase
+):
+    @property
+    def _distance_level(self):
+        return self._levenshtein_level
```

### Comparing `splink-3.8.1/splink/duckdb/duckdb_helpers.py` & `splink-3.9.0/splink/duckdb/duckdb_helpers/duckdb_helpers.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/duckdb/duckdb_linker.py` & `splink-3.9.0/splink/duckdb/duckdb_linker.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from __future__ import annotations
 
 import logging
+import os
 from tempfile import TemporaryDirectory
 
 import duckdb
 import pandas as pd
 from duckdb import DuckDBPyConnection
 
 from ..input_column import InputColumn
 from ..linker import Linker
 from ..misc import (
     ensure_is_list,
 )
 from ..splink_dataframe import SplinkDataFrame
-from .duckdb_helpers import (
+from .duckdb_helpers.duckdb_helpers import (
     create_temporary_duckdb_connection,
     duckdb_load_from_file,
     validate_duckdb_connection,
 )
 
 logger = logging.getLogger(__name__)
 
@@ -50,14 +51,52 @@
     def as_pandas_dataframe(self, limit=None):
         sql = f"select * from {self.physical_name}"
         if limit:
             sql += f" limit {limit}"
 
         return self.linker._con.query(sql).to_df()
 
+    def to_parquet(self, filepath, overwrite=False):
+        if not overwrite:
+            self.check_file_exists(filepath)
+
+        if not filepath.endswith(".parquet"):
+            raise SyntaxError(
+                f"The filepath you've entered to '{filepath}' is "
+                "not a parquet file. Please ensure that the filepath "
+                "ends with `.parquet` before retrying."
+            )
+
+        # create the directories recursively if they don't exist
+        path = os.path.dirname(filepath)
+        if path:
+            os.makedirs(path, exist_ok=True)
+
+        sql = f"COPY {self.physical_name} TO '{filepath}' (FORMAT PARQUET);"
+        self.linker._con.query(sql)
+
+    def to_csv(self, filepath, overwrite=False):
+        if not overwrite:
+            self.check_file_exists(filepath)
+
+        if not filepath.endswith(".csv"):
+            raise SyntaxError(
+                f"The filepath you've entered '{filepath}' is "
+                "not a csv file. Please ensure that the filepath "
+                "ends with `.csv` before retrying."
+            )
+
+        # create the directories recursively if they don't exist
+        path = os.path.dirname(filepath)
+        if path:
+            os.makedirs(path, exist_ok=True)
+
+        sql = f"COPY {self.physical_name} TO '{filepath}' (HEADER, DELIMITER ',');"
+        self.linker._con.query(sql)
+
 
 class DuckDBLinker(Linker):
     """Manages the data linkage process and holds the data linkage model."""
 
     def __init__(
         self,
         input_table_or_tables: str | list,
@@ -192,23 +231,26 @@
                 raise ValueError(
                     f"Table '{table_name}' already exists in database. "
                     "Please use the 'overwrite' argument if you wish to overwrite"
                 )
             else:
                 self._con.unregister(table_name)
 
+        self._table_registration(input, table_name)
+        return self._table_to_splink_dataframe(table_name, table_name)
+
+    def _table_registration(self, input, table_name):
         if isinstance(input, dict):
             input = pd.DataFrame(input)
         elif isinstance(input, list):
             input = pd.DataFrame.from_records(input)
 
         # Registration errors will automatically
         # occur if an invalid data type is passed as an argument
         self._con.register(table_name, input)
-        return self._table_to_splink_dataframe(table_name, table_name)
 
     def _random_sample_sql(self, proportion, sample_size, seed=None):
         if proportion == 1.0:
             return ""
         percent = proportion * 100
         if seed:
             return f"USING SAMPLE bernoulli({percent}%) REPEATABLE({seed})"
```

### Comparing `splink-3.8.1/splink/em_training_session.py` & `splink-3.9.0/splink/em_training_session.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/estimate_u.py` & `splink-3.9.0/splink/estimate_u.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/expectation_maximisation.py` & `splink-3.9.0/splink/expectation_maximisation.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import logging
 import time
 from typing import TYPE_CHECKING
 
-import duckdb
+import pandas as pd
 
 from .comparison_level import ComparisonLevel
 from .constants import LEVEL_NOT_OBSERVED_TEXT
 from .m_u_records_to_parameters import m_u_records_to_lookup_dict
 from .predict import predict_from_comparison_vectors_sqls
 from .settings import Settings
 from .splink_dataframe import SplinkDataFrame
@@ -52,44 +52,84 @@
     union_sqls.append(sql)
 
     sql = " union all ".join(union_sqls)
 
     return sql
 
 
-def compute_proportions_for_new_parameters(m_u_df):
+def compute_proportions_for_new_parameters_sql(table_name):
     """Using the results from compute_new_parameters_sql, compute
     m and u
     """
 
-    sql = """
+    sql = f"""
     select
         comparison_vector_value,
         output_column_name,
         m_count/sum(m_count) over (PARTITION BY output_column_name)
             as m_probability,
         u_count/sum(u_count) over (PARTITION BY output_column_name)
             as u_probability
-    from m_u_df
+    from {table_name}
     where comparison_vector_value != -1
     and output_column_name != '_probability_two_random_records_match'
 
     union all
 
     select
         comparison_vector_value,
         output_column_name,
         m_count as m_probability,
         u_count as u_probability
-    from m_u_df
+    from {table_name}
     where output_column_name = '_probability_two_random_records_match'
     order by output_column_name, comparison_vector_value asc
     """
 
-    return duckdb.query(sql).to_df().to_dict("records")
+    return sql
+
+
+def compute_proportions_for_new_parameters_pandas(m_u_df):
+    data = m_u_df.copy()
+    m_prob = "m_probability"
+    u_prob = "u_probability"
+    data.rename(columns={"m_count": m_prob, "u_count": u_prob}, inplace=True)
+
+    random_records = data[
+        data.output_column_name == "_probability_two_random_records_match"
+    ]
+    data = data[data.output_column_name != "_probability_two_random_records_match"]
+
+    data = data[data.comparison_vector_value != -1]
+    index = data.index.tolist()
+
+    m_probs = data.loc[index, m_prob] / data.groupby("output_column_name")[
+        m_prob
+    ].transform("sum")
+    u_probs = data.loc[index, u_prob] / data.groupby("output_column_name")[
+        u_prob
+    ].transform("sum")
+
+    data.loc[index, m_prob] = m_probs
+    data.loc[index, u_prob] = u_probs
+
+    data = pd.concat([random_records, data])
+
+    return data.to_dict("records")
+
+
+def compute_proportions_for_new_parameters(m_u_df):
+    # Execute with duckdb if installed, otherwise default to pandas
+    try:
+        import duckdb
+
+        sql = compute_proportions_for_new_parameters_sql("m_u_df")
+        return duckdb.query(sql).to_df().to_dict("records")
+    except (ImportError, ModuleNotFoundError):
+        return compute_proportions_for_new_parameters_pandas(m_u_df)
 
 
 def populate_m_u_from_lookup(
     em_training_session, comparison_level: ComparisonLevel, m_u_records_lookup
 ):
     cl = comparison_level
     c = comparison_level.comparison
```

### Comparing `splink-3.8.1/splink/files/chart_defs/blocking_rule_generated_comparisons.json` & `splink-3.9.0/splink/files/chart_defs/blocking_rule_generated_comparisons.json`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/files/chart_defs/completeness.json` & `splink-3.9.0/splink/files/chart_defs/completeness.json`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/files/chart_defs/del/bayes_factor_history_chart_def.json` & `splink-3.9.0/splink/files/chart_defs/del/bayes_factor_history_chart_def.json`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/files/chart_defs/del/bayes_factor_intuition_chart_def.json` & `splink-3.9.0/splink/files/chart_defs/del/bayes_factor_intuition_chart_def.json`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/files/chart_defs/del/compare_estimates.json` & `splink-3.9.0/splink/files/chart_defs/del/compare_estimates.json`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/files/chart_defs/del/gamma_distribution_chart_def.json` & `splink-3.9.0/splink/files/chart_defs/del/gamma_distribution_chart_def.json`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/files/chart_defs/del/gamma_histogram.json` & `splink-3.9.0/splink/files/chart_defs/del/gamma_histogram.json`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/files/chart_defs/del/score_histogram.json` & `splink-3.9.0/splink/files/chart_defs/del/score_histogram.json`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/files/chart_defs/m_u_parameters_interactive_history.json` & `splink-3.9.0/splink/files/chart_defs/m_u_parameters_interactive_history.json`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/files/chart_defs/match_weight_histogram.json` & `splink-3.9.0/splink/files/chart_defs/match_weight_histogram.json`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/files/chart_defs/match_weights_interactive_history.json` & `splink-3.9.0/splink/files/chart_defs/match_weights_interactive_history.json`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/files/chart_defs/match_weights_waterfall.json` & `splink-3.9.0/splink/files/chart_defs/match_weights_waterfall.json`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/files/chart_defs/missingness.json` & `splink-3.9.0/splink/files/chart_defs/missingness.json`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/files/chart_defs/parameter_estimate_comparisons.json` & `splink-3.9.0/splink/files/chart_defs/parameter_estimate_comparisons.json`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/files/chart_defs/precision_recall.json` & `splink-3.9.0/splink/files/chart_defs/precision_recall.json`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/files/chart_defs/probability_two_random_records_match_iteration.json` & `splink-3.9.0/splink/files/chart_defs/probability_two_random_records_match_iteration.json`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/files/chart_defs/profile_data.json` & `splink-3.9.0/splink/files/chart_defs/profile_data.json`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/files/chart_defs/roc.json` & `splink-3.9.0/splink/files/chart_defs/roc.json`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/files/chart_defs/unlinkables_chart_def.json` & `splink-3.9.0/splink/files/chart_defs/unlinkables_chart_def.json`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/files/external_js/vega-embed@6.20.2` & `splink-3.9.0/splink/files/external_js/vega-embed@6.20.2`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/files/external_js/vega-lite@5.2.0` & `splink-3.9.0/splink/files/external_js/vega-lite@5.2.0`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/files/external_js/vega@5.21.0` & `splink-3.9.0/splink/files/external_js/vega@5.21.0`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/files/settings_jsonschema.json` & `splink-3.9.0/splink/files/settings_jsonschema.json`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/files/spark_jars/scala-udf-similarity-0.1.0_classic.jar` & `splink-3.9.0/splink/files/spark_jars/scala-udf-similarity-0.1.0_classic.jar`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/files/spark_jars/scala-udf-similarity-0.1.0_spark3.3.jar` & `splink-3.9.0/splink/files/spark_jars/scala-udf-similarity-0.1.0_spark3.3.jar`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/files/spark_jars/scala-udf-similarity-0.1.1_spark3.x.jar` & `splink-3.9.0/splink/files/spark_jars/scala-udf-similarity-0.1.1_spark3.x.jar`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/files/splink_cluster_studio/cluster_template.j2` & `splink-3.9.0/splink/files/splink_cluster_studio/cluster_template.j2`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/files/splink_cluster_studio/custom.css` & `splink-3.9.0/splink/files/splink_cluster_studio/custom.css`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/files/splink_comparison_viewer/custom.css` & `splink-3.9.0/splink/files/splink_comparison_viewer/custom.css`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/files/splink_comparison_viewer/template.j2` & `splink-3.9.0/splink/files/splink_comparison_viewer/template.j2`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/files/splink_vis_utils/splink_vis_utils.js` & `splink-3.9.0/splink/files/splink_vis_utils/splink_vis_utils.js`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/input_column.py` & `splink-3.9.0/splink/input_column.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/linker.py` & `splink-3.9.0/splink/linker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from __future__ import annotations
 
 import hashlib
 import json
 import logging
 import os
+import re
 import warnings
 from collections import UserDict
 from copy import copy, deepcopy
 from pathlib import Path
 from statistics import median
 
+import sqlglot
+
 from splink.input_column import InputColumn, remove_quotes_from_identifiers
 
 from .accuracy import (
     prediction_errors_from_label_column,
     prediction_errors_from_labels_table,
     truth_space_table_from_labels_column,
     truth_space_table_from_labels_table,
@@ -76,14 +79,15 @@
 from .term_frequencies import (
     _join_tf_to_input_df_sql,
     colname_to_tf_tablename,
     compute_all_term_frequencies_sqls,
     compute_term_frequencies_from_concat_with_tf,
     term_frequencies_for_single_column_sql,
     term_frequencies_from_concat_with_tf,
+    tf_adjustment_chart,
 )
 from .unique_id_concat import (
     _composite_unique_id_from_edges_sql,
 )
 from .unlinkables import unlinkables_data
 from .vertically_concatenate import vertically_concatenate_sql
 
@@ -183,15 +187,16 @@
         self._pipeline = SQLPipeline()
 
         self._names_of_tables_created_by_splink: set = set()
         self._intermediate_table_cache: dict = CacheDictWithLogging()
 
         if not isinstance(settings_dict, (dict, type(None))):
             # Run if you've entered a filepath
-            self._setup_settings_objs(None)  # feed it a blank settings dictionary
+            # feed it a blank settings dictionary
+            self._setup_settings_objs(None)
             self.load_settings(settings_dict)
         else:
             settings_dict = deepcopy(settings_dict)
             self._setup_settings_objs(settings_dict)
 
         homogenised_tables, homogenised_aliases = self._register_input_tables(
             input_table_or_tables,
@@ -207,14 +212,15 @@
         self._em_training_sessions = []
 
         self._find_new_matches_mode = False
         self._train_u_using_random_sample_mode = False
         self._compare_two_records_mode = False
         self._self_link_mode = False
         self._analyse_blocking_mode = False
+        self._deterministic_link_mode = False
 
         self.debug_mode = False
 
     @property
     def _cache_uid(self):
         if self._settings_dict:
             return self._settings_obj._cache_uid
@@ -338,15 +344,14 @@
     def _infinity_expression(self):
         raise NotImplementedError(
             f"infinity sql expression not available for {type(self)}"
         )
 
     @property
     def _verify_link_only_job(self):
-
         cache = self._intermediate_table_cache
         if "__splink__df_concat_with_tf" not in cache:
             return
 
         if self._settings_obj._link_type == "link_only":
             # if input datasets > 1 then skip
             if len(self._input_tables_dict) > 1:
@@ -371,20 +376,36 @@
 
     def _register_input_tables(self, input_tables, input_aliases, accepted_df_dtypes):
         # 'homogenised' means all entries are strings representing tables
         homogenised_tables = []
         homogenised_aliases = []
         accepted_df_dtypes = ensure_is_tuple(accepted_df_dtypes)
 
+        existing_tables = []
+        for alias in input_aliases:
+            # Check if alias is a string (indicating a table name) and that it is not
+            # a file path.
+            if not isinstance(alias, str) or re.match(pattern=r".*", string=alias):
+                continue
+            exists = self._table_exists_in_database(alias)
+            if exists:
+                existing_tables.append(f"'{alias}'")
+        if existing_tables:
+            input_tables = ", ".join(existing_tables)
+            raise ValueError(
+                f"Table(s): {input_tables} already exists in database. "
+                "Please remove or rename it/them before retrying"
+            )
+
         for i, (table, alias) in enumerate(zip(input_tables, input_aliases)):
             if isinstance(alias, accepted_df_dtypes):
                 alias = f"__splink__input_table_{i}"
 
             if isinstance(table, accepted_df_dtypes):
-                self.register_table(table, alias)
+                self._table_registration(table, alias)
                 table = alias
 
             homogenised_tables.append(table)
             homogenised_aliases.append(alias)
 
         return homogenised_tables, homogenised_aliases
 
@@ -576,17 +597,27 @@
     ) -> SplinkDataFrame:
         """Log the sql, then call _run_sql_execution(), wrapping any errors"""
         logger.debug(execute_sql_logging_message_info(templated_name, physical_name))
         logger.log(5, log_sql(final_sql))
         try:
             return self._run_sql_execution(final_sql, templated_name, physical_name)
         except Exception as e:
+            # Parse our SQL through sqlglot to pretty print
+            try:
+                final_sql = sqlglot.parse_one(
+                    final_sql,
+                    read=self._sql_dialect,
+                ).sql(pretty=True)
+                # if sqlglot produces any errors, just report the raw SQL
+            except Exception:
+                pass
+
             raise SplinkException(
                 f"Error executing the following sql for table "
-                f"`{templated_name}`({physical_name}):\n{final_sql}"
+                f"`{templated_name}` ({physical_name}):\n{final_sql}"
             ) from e
 
     def register_table(self, input, table_name, overwrite=False):
         """
         Register a table to your backend database, to be used in one of the
         splink methods, or simply to allow querying.
 
@@ -608,14 +639,38 @@
         Returns:
             SplinkDataFrame: An abstraction representing the table created by the sql
                 pipeline
         """
 
         raise NotImplementedError(f"register_table not implemented for {type(self)}")
 
+    def _table_registration(self, input, table_name):
+        """
+        Register a table to your backend database, to be used in one of the
+        splink methods, or simply to allow querying.
+
+        Tables can be of type: dictionary, record level dictionary,
+        pandas dataframe, pyarrow table and in the spark case, a spark df.
+
+        This function is contains no overwrite functionality, so it can be used
+        where we don't want to allow for overwriting.
+
+        Args:
+            input: The data you wish to register. This can be either a dictionary,
+                pandas dataframe, pyarrow table or a spark dataframe.
+            table_name (str): The name you wish to assign to the table.
+
+        Returns:
+            None
+        """
+
+        raise NotImplementedError(
+            f"_table_registration not implemented for {type(self)}"
+        )
+
     def query_sql(self, sql, output_type="pandas"):
         """
         Run a SQL query against your backend database and return
         the resulting output.
 
         Examples:
             >>> linker = DuckDBLinker(df, settings)
@@ -951,15 +1006,15 @@
             settings_dict (dict | str | Path): A Splink settings dictionary or
                 the path to your settings json file.
         """
 
         if not isinstance(settings_dict, dict):
             p = Path(settings_dict)
             if not p.is_file():  # check if it's a valid file/filepath
-                raise ValueError(
+                raise FileNotFoundError(
                     "The filepath you have provided is either not a valid file "
                     "or doesn't exist along the path provided."
                 )
             settings_dict = json.loads(p.read_text())
 
         # Store the cache ID so it can be reloaded after cache invalidation
         cache_id = self._cache_uid
@@ -1132,14 +1187,20 @@
             >>> df = linker.deterministic_link()
 
         Returns:
             SplinkDataFrame: A SplinkDataFrame of the pairwise comparisons.  This
                 represents a table materialised in the database. Methods on the
                 SplinkDataFrame allow you to access the underlying data.
         """
+
+        # Allows clustering during a deterministic linkage.
+        # This is used in `cluster_pairwise_predictions_at_threshold`
+        # to set the cluster threshold to 1
+        self._deterministic_link_mode = True
+
         concat_with_tf = self._initialise_df_concat_with_tf()
         sql = block_using_rules_sql(self)
         self._enqueue_sql(sql, "__splink__df_blocked")
         return self._execute_sql_pipeline([concat_with_tf])
 
     def estimate_u_using_random_sampling(
         self, max_pairs: int = None, seed: int = None, *, target_rows=None
@@ -1719,15 +1780,15 @@
         self._self_link_mode = False
 
         return predictions
 
     def cluster_pairwise_predictions_at_threshold(
         self,
         df_predict: SplinkDataFrame,
-        threshold_match_probability: float,
+        threshold_match_probability: float = None,
         pairwise_formatting: bool = False,
         filter_pairwise_format_for_clusters: bool = True,
     ) -> SplinkDataFrame:
         """Clusters the pairwise match predictions that result from `linker.predict()`
         into groups of connected record using the connected components graph clustering
         algorithm
 
@@ -2598,14 +2659,68 @@
         Returns:
             VegaLite: A VegaLite chart object. See altair.vegalite.v4.display.VegaLite.
                 The vegalite spec is available as a dictionary using the `spec`
                 attribute.
         """
         return self._settings_obj.match_weights_chart()
 
+    def tf_adjustment_chart(
+        self,
+        output_column_name: str,
+        n_most_freq: int = 10,
+        n_least_freq: int = 10,
+        vals_to_include: str | list = None,
+        as_dict: bool = False,
+    ):
+        """Display a chart showing the impact of term frequency adjustments on a
+        specific comparison level.
+        Each value
+
+        Args:
+            output_column_name (str): Name of an output column for which term frequency
+                 adjustment has been applied.
+            n_most_freq (int, optional): Number of most frequent values to show. If this
+                 or `n_least_freq` set to None, all values will be shown.
+                Default to 10.
+            n_least_freq (int, optional): Number of least frequent values to show. If
+                this or `n_most_freq` set to None, all values will be shown.
+                Default to 10.
+            vals_to_include (list, optional): Specific values for which to show term
+                sfrequency adjustments.
+                Defaults to None.
+
+        Returns:
+            VegaLite: A VegaLite chart object. See altair.vegalite.v4.display.VegaLite.
+                The vegalite spec is available as a dictionary using the `spec`
+                attribute.
+        """
+
+        # Comparisons with TF adjustments
+        tf_comparisons = [
+            c._output_column_name
+            for c in self._settings_obj.comparisons
+            if any([cl._has_tf_adjustments for cl in c.comparison_levels])
+        ]
+        if output_column_name not in tf_comparisons:
+            raise ValueError(
+                f"{output_column_name} is not a valid comparison column, or does not"
+                f" have term frequency adjustment activated"
+            )
+
+        vals_to_include = ensure_is_list(vals_to_include)
+
+        return tf_adjustment_chart(
+            self,
+            output_column_name,
+            n_most_freq,
+            n_least_freq,
+            vals_to_include,
+            as_dict,
+        )
+
     def m_u_parameters_chart(self):
         """Display a chart of the m and u parameters of the linkage model
 
         Examples:
             >>> linker.m_u_parameters_chart()
             >>>
             >>> # To view offline (if you don't have an internet connection):
```

### Comparing `splink-3.8.1/splink/lower_id_on_lhs.py` & `splink-3.9.0/splink/lower_id_on_lhs.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/m_from_labels.py` & `splink-3.9.0/splink/m_from_labels.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/m_training.py` & `splink-3.9.0/splink/m_training.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/m_u_records_to_parameters.py` & `splink-3.9.0/splink/m_u_records_to_parameters.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/match_key_analysis.py` & `splink-3.9.0/splink/match_key_analysis.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/match_weights_histogram.py` & `splink-3.9.0/splink/match_weights_histogram.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/misc.py` & `splink-3.9.0/splink/misc.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/missingness.py` & `splink-3.9.0/splink/missingness.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/parse_sql.py` & `splink-3.9.0/splink/parse_sql.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/pipeline.py` & `splink-3.9.0/splink/pipeline.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/predict.py` & `splink-3.9.0/splink/predict.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/profile_data.py` & `splink-3.9.0/splink/profile_data.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/settings.py` & `splink-3.9.0/splink/settings.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/spark/custom_spark_dialect.py` & `splink-3.9.0/splink/spark/spark_helpers/custom_spark_dialect.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/spark/spark_linker.py` & `splink-3.9.0/splink/spark/spark_linker.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from ..databricks.enable_splink import enable_splink
 from ..input_column import InputColumn
 from ..linker import Linker
 from ..misc import ensure_is_list, major_minor_version_greater_equal_than
 from ..splink_dataframe import SplinkDataFrame
 from ..term_frequencies import colname_to_tf_tablename
-from .custom_spark_dialect import Dialect
+from .spark_helpers.custom_spark_dialect import Dialect
 
 logger = logging.getLogger(__name__)
 
 Dialect["customspark"]
 
 
 class SparkDataframe(SplinkDataFrame):
@@ -58,14 +58,28 @@
             sql += f" limit {limit}"
 
         return self.linker.spark.sql(sql).toPandas()
 
     def as_spark_dataframe(self):
         return self.linker.spark.table(self.physical_name)
 
+    def to_parquet(self, filepath, overwrite=False):
+        if not overwrite:
+            self.check_file_exists(filepath)
+
+        spark_df = self.as_spark_dataframe()
+        spark_df.write.mode("overwrite").format("parquet").save(filepath)
+
+    def to_csv(self, filepath, overwrite=False):
+        if not overwrite:
+            self.check_file_exists(filepath)
+
+        spark_df = self.as_spark_dataframe()
+        spark_df.write.format("csv").option("header", "true").save(filepath)
+
 
 class SparkLinker(Linker):
     def __init__(
         self,
         input_table_or_tables,
         settings_dict=None,
         break_lineage_method=None,
@@ -252,14 +266,19 @@
             (
                 "jaro_winkler",
                 "uk.gov.moj.dash.linkage.JaroWinklerSimilarity",
                 DoubleType(),
             ),
             ("jaccard", "uk.gov.moj.dash.linkage.JaccardSimilarity", DoubleType()),
             ("cosine_distance", "uk.gov.moj.dash.linkage.CosineDistance", DoubleType()),
+            (
+                "damerau_levenshtein",
+                "uk.gov.moj.dash.linkage.LevDamerauDistance",
+                DoubleType(),
+            ),
             ("Dmetaphone", "uk.gov.moj.dash.linkage.DoubleMetaphone", StringType()),
             (
                 "DmetaphoneAlt",
                 "uk.gov.moj.dash.linkage.DoubleMetaphoneAlt",
                 StringType(),
             ),
             ("QgramTokeniser", "uk.gov.moj.dash.linkage.QgramTokeniser", StringType()),
@@ -339,15 +358,15 @@
         spark_df = self._repartition_if_needed(spark_df, templated_name)
 
         regex_to_persist = [
             r"__splink__df_comparison_vectors",
             r"__splink__df_concat_with_tf",
             r"__splink__df_predict",
             r"__splink__df_tf_.+",
-            r"__splink__df_representatives.+",
+            r"__splink__df_representatives.*",
             r"__splink__df_neighbours",
             r"__splink__df_connected_components_df",
         ]
 
         if re.fullmatch(r"|".join(regex_to_persist), templated_name):
             if self.break_lineage_method == "persist":
                 spark_df = spark_df.persist()
@@ -436,25 +455,28 @@
         if exists:
             if not overwrite:
                 raise ValueError(
                     f"Table '{table_name}' already exists in database. "
                     "Please use the 'overwrite' argument if you wish to overwrite"
                 )
 
+        self._table_registration(input, table_name)
+        return self._table_to_splink_dataframe(table_name, table_name)
+
+    def _table_registration(self, input, table_name):
         if isinstance(input, dict):
             input = pd.DataFrame(input)
             input = self.spark.createDataFrame(input)
         elif isinstance(input, list):
             input = pd.DataFrame.from_records(input)
             input = self.spark.createDataFrame(input)
         elif isinstance(input, pd.DataFrame):
             input = self.spark.createDataFrame(input)
 
         input.createOrReplaceTempView(table_name)
-        return self._table_to_splink_dataframe(table_name, table_name)
 
     def _random_sample_sql(self, proportion, sample_size, seed=None):
         if proportion == 1.0:
             return ""
         percent = proportion * 100
         if seed:
             return f" ORDER BY rand({seed}) LIMIT {round(sample_size)}"
```

### Comparing `splink-3.8.1/splink/splink_comparison_viewer.py` & `splink-3.9.0/splink/splink_comparison_viewer.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/splink_dataframe.py` & `splink-3.9.0/splink/splink_dataframe.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import logging
+from pathlib import Path
 from typing import TYPE_CHECKING
 
 logger = logging.getLogger(__name__)
 
 # https://stackoverflow.com/questions/39740632/python-type-hinting-without-cyclic-imports
 if TYPE_CHECKING:
     from .linker import Linker
@@ -86,7 +87,22 @@
             "\n`.as_record_dict(limit=5)` or "
             "`.as_pandas_dataframe(limit=5)`.\n"
             "\nYou may omit the `limit` argument to return all records."
             "\n\nThis table represents the following splink entity: "
             f"{self.templated_name}"
         )
         p.text(msg)
+
+    def to_parquet(self, filepath, overwrite=False):
+        raise NotImplementedError("`to_parquet` not implemented for this linker")
+
+    def to_csv(self, filepath, overwrite=False):
+        raise NotImplementedError("`to_csv` not implemented for this linker")
+
+    def check_file_exists(self, filepath):
+        p = Path(filepath)
+        if p.exists():
+            raise FileExistsError(
+                "The filepath you've supplied already exists. Please use "
+                "either `overwrite = True` or manually move or delete the "
+                "existing file."
+            )
```

### Comparing `splink-3.8.1/splink/sql_transform.py` & `splink-3.9.0/splink/sql_transform.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/sqlite/sqlite_linker.py` & `splink-3.9.0/splink/sqlite/sqlite_linker.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,22 +143,25 @@
                 raise ValueError(
                     f"Table '{table_name}' already exists in database. "
                     "Please use the 'overwrite' argument if you wish to overwrite"
                 )
             else:
                 self._delete_table_from_database(table_name)
 
+        self._table_registration(input, table_name)
+        return self._table_to_splink_dataframe(table_name, table_name)
+
+    def _table_registration(self, input, table_name):
         if isinstance(input, dict):
             input = pd.DataFrame(input)
         elif isinstance(input, list):
             input = pd.DataFrame.from_records(input)
 
         # Will error if an invalid data type is passed
         input.to_sql(table_name, self.con, index=False)
-        return self._table_to_splink_dataframe(table_name, table_name)
 
     def _random_sample_sql(self, proportion, sample_size, seed=None):
         if proportion == 1.0:
             return ""
         if seed:
             raise NotImplementedError(
                 "SQLite does not support seeds in random ",
```

### Comparing `splink-3.8.1/splink/unique_id_concat.py` & `splink-3.9.0/splink/unique_id_concat.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/unlinkables.py` & `splink-3.9.0/splink/unlinkables.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/validate_jsonschema.py` & `splink-3.9.0/splink/validate_jsonschema.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/vertically_concatenate.py` & `splink-3.9.0/splink/vertically_concatenate.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/splink/waterfall_chart.py` & `splink-3.9.0/splink/waterfall_chart.py`

 * *Files identical despite different names*

### Comparing `splink-3.8.1/PKG-INFO` & `splink-3.9.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splink
-Version: 3.8.1
+Version: 3.9.0
 Summary: Fast probabilistic data linkage at scale
 Home-page: https://github.com/moj-analytical-services/splink
 License: MIT
 Author: Robin Linacre
 Author-email: robinlinacre@hotmail.com
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Jinja2 (>=3.0.3)
 Requires-Dist: altair (>=4.2.0)
 Requires-Dist: duckdb (>=0.6.0)
 Requires-Dist: jsonschema (>=3.2,<5.0)
 Requires-Dist: pandas (>=1.0.0)
+Requires-Dist: phonetics (>=1.0.5,<2.0.0)
 Requires-Dist: sqlglot (>=5.1.0)
 Project-URL: Repository, https://github.com/moj-analytical-services/splink
 Description-Content-Type: text/markdown
 
 <p align="center">
 <img src="https://user-images.githubusercontent.com/7570107/85285114-3969ac00-b488-11ea-88ff-5fca1b34af1f.png" alt="Splink Logo" height="150px">
 </p>
@@ -33,35 +34,35 @@
 
 # Fast, accurate and scalable probabilistic data linkage
 
 Splink is a Python package for probabilistic record linkage (entity resolution) that allows you to deduplicate and link records from datasets without unique identifiers.
 
 ## Key Features
 
-⚡ **Speed:** Capable of linking a million records on a laptop in approximately one minute.  
-🎯 **Accuracy:** Full support for term frequency adjustments and user-defined fuzzy matching logic.  
-🌐 **Scalability:** Execute linkage jobs in Python (using DuckDB) or big-data backends like AWS Athena or Spark for 100+ million records.  
-🎓 **Unsupervised Learning:** No training data is required, as models can be trained using an unsupervised approach.  
+⚡ **Speed:** Capable of linking a million records on a laptop in approximately one minute.
+🎯 **Accuracy:** Full support for term frequency adjustments and user-defined fuzzy matching logic.
+🌐 **Scalability:** Execute linkage jobs in Python (using DuckDB) or big-data backends like AWS Athena or Spark for 100+ million records.
+🎓 **Unsupervised Learning:** No training data is required, as models can be trained using an unsupervised approach.
 📊 **Interactive Outputs:** Provides a wide range of interactive outputs to help users understand their model and diagnose linkage problems.
 
 Splink's core linkage algorithm is based on Fellegi-Sunter's model of record linkage, with various customizations to improve accuracy.
 
 ## What does Splink do?
 
 Consider the following records that lack a unique person identifier:
 
-![tables showing what splink does](https://raw.githubusercontent.com/moj-analytical-services/splink/master/docs/img/main_readme_what_does_splink_do_1.drawio.png)
+![tables showing what splink does](https://raw.githubusercontent.com/moj-analytical-services/splink/master/docs/img/README/what_does_splink_do_1.drawio.png)
 
 Splink predicts which rows link together:
 
-![tables showing what splink does](https://raw.githubusercontent.com/moj-analytical-services/splink/master/docs/img/main_readme_what_does_splink_do_2.drawio.png)
+![tables showing what splink does](https://raw.githubusercontent.com/moj-analytical-services/splink/master/docs/img/README/what_does_splink_do_2.drawio.png)
 
 and clusters these links to produce an estimated person ID:
 
-![tables showing what splink does](https://raw.githubusercontent.com/moj-analytical-services/splink/master/docs/img/main_readme_what_does_splink_do_3.drawio.png)
+![tables showing what splink does](https://raw.githubusercontent.com/moj-analytical-services/splink/master/docs/img/README/what_does_splink_do_3.drawio.png)
 
 ## What data does Splink work best with?
 
 Before using Splink, input data should be standardized, with consistent column names and formatting (e.g., lowercased, punctuation cleaned up, etc.).
 
 Splink performs best with input data containing **multiple** columns that are **not highly correlated**. For instance, if the entity type is persons, you may have columns for full name, date of birth, and city. If the entity type is companies, you could have columns for name, turnover, sector, and telephone number.
 
@@ -89,43 +90,44 @@
 
 or, if you prefer, you can instead install splink using conda:
 
 ```sh
 conda install -c conda-forge splink
 ```
 
+Should you require a more bare-bones version of Splink **without DuckDB**, please see the following area of the docs:
+> [DuckDBless Splink Installation](https://moj-analytical-services.github.io/splink/installations.html#duckdb-less-installation)
+
 ## Quickstart
 
 The following code demonstrates how to estimate the parameters of a deduplication model, use it to identify duplicate records, and then use clustering to generate an estimated unique person ID.
 
 For more detailed tutorials, please see [here](https://moj-analytical-services.github.io/splink/demos/00_Tutorial_Introduction.html).
 
 ```py
 from splink.duckdb.duckdb_linker import DuckDBLinker
-from splink.duckdb.duckdb_comparison_library import (
-    exact_match,
-    levenshtein_at_thresholds,
-)
+import splink.duckdb.duckdb_comparison_library as cl
+import splink.duckdb.duckdb_comparison_template_library as ctl
 
 import pandas as pd
 
 df = pd.read_csv("./tests/datasets/fake_1000_from_splink_demos.csv")
 
 settings = {
     "link_type": "dedupe_only",
     "blocking_rules_to_generate_predictions": [
         "l.first_name = r.first_name",
         "l.surname = r.surname",
     ],
     "comparisons": [
-        levenshtein_at_thresholds("first_name", 2),
-        exact_match("surname"),
-        exact_match("dob"),
-        exact_match("city", term_frequency_adjustments=True),
-        exact_match("email"),
+        ctl.name_comparison("first_name"),
+        ctl.name_comparison("surname"),
+        ctl.date_comparison("dob", cast_strings_to_date=True),
+        cl.exact_match("city", term_frequency_adjustments=True),
+        cl.levenshtein_at_thresholds("email", 2),
     ],
 }
 
 linker = DuckDBLinker(df, settings)
 linker.estimate_u_using_random_sampling(max_pairs=1e6)
 
 blocking_rule_for_training = "l.first_name = r.first_name and l.surname = r.surname"
@@ -162,15 +164,15 @@
 ## Citation
 
 If you use Splink in your research, we'd be grateful for a citation as follows:
 
 ```BibTeX
 @article{Linacre_Lindsay_Manassis_Slade_Hepworth_2022,
 	title        = {Splink: Free software for probabilistic record linkage at scale.},
-	author       = {Linacre, Robin and Lindsay, Sam and Manassis, Theodore and Slade, Zoe and Hepworth, Tom},
+	author       = {Linacre, Robin and Lindsay, Sam and Manassis, Theodore and Slade, Zoe and Hepworth, Tom and Kennedy, Ross and Bond, Andrew},
 	year         = 2022,
 	month        = {Aug.},
 	journal      = {International Journal of Population Data Science},
 	volume       = 7,
 	number       = 3,
 	doi          = {10.23889/ijpds.v7i3.1794},
 	url          = {https://ijpds.org/article/view/1794},
```

