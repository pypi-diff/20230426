# Comparing `tmp/splink-3.7.3.tar.gz` & `tmp/splink-3.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splink-3.7.3.tar", max compression
+gzip compressed data, was "splink-3.8.0.tar", max compression
```

## Comparing `splink-3.7.3.tar` & `splink-3.8.0.tar`

### file list

```diff
@@ -1,111 +1,112 @@
--rw-r--r--   0        0        0     1076 2023-03-30 16:25:57.842546 splink-3.7.3/LICENSE
--rw-r--r--   0        0        0     8426 2023-03-30 16:25:57.842546 splink-3.7.3/README.md
--rw-r--r--   0        0        0     1435 2023-03-30 16:25:57.862546 splink-3.7.3/pyproject.toml
--rw-r--r--   0        0        0       23 2023-03-30 16:25:57.862546 splink-3.7.3/splink/__init__.py
--rw-r--r--   0        0        0    10818 2023-03-30 16:25:57.862546 splink-3.7.3/splink/accuracy.py
--rw-r--r--   0        0        0     4753 2023-03-30 16:25:57.862546 splink-3.7.3/splink/analyse_blocking.py
--rw-r--r--   0        0        0      461 2023-03-30 16:25:57.866546 splink-3.7.3/splink/athena/athena_base.py
--rw-r--r--   0        0        0     1053 2023-03-30 16:25:57.866546 splink-3.7.3/splink/athena/athena_comparison_level_library.py
--rw-r--r--   0        0        0     1628 2023-03-30 16:25:57.866546 splink-3.7.3/splink/athena/athena_comparison_library.py
--rw-r--r--   0        0        0    18735 2023-03-30 16:25:57.866546 splink-3.7.3/splink/athena/athena_linker.py
--rw-r--r--   0        0        0      350 2023-03-30 16:25:57.866546 splink-3.7.3/splink/athena/athena_transforms.py
--rw-r--r--   0        0        0     1276 2023-03-30 16:25:57.866546 splink-3.7.3/splink/athena/athena_utils.py
--rw-r--r--   0        0        0     2866 2023-03-30 16:25:57.866546 splink-3.7.3/splink/block_from_labels.py
--rw-r--r--   0        0        0     5979 2023-03-30 16:25:57.866546 splink-3.7.3/splink/blocking.py
--rw-r--r--   0        0        0    10627 2023-03-30 16:25:57.866546 splink-3.7.3/splink/charts.py
--rw-r--r--   0        0        0     9036 2023-03-30 16:25:57.866546 splink-3.7.3/splink/cluster_studio.py
--rw-r--r--   0        0        0    16881 2023-03-30 16:25:57.866546 splink-3.7.3/splink/comparison.py
--rw-r--r--   0        0        0    25479 2023-03-30 16:25:57.866546 splink-3.7.3/splink/comparison_level.py
--rw-r--r--   0        0        0     9013 2023-03-30 16:25:57.866546 splink-3.7.3/splink/comparison_level_composition.py
--rw-r--r--   0        0        0    15631 2023-03-30 16:25:57.866546 splink-3.7.3/splink/comparison_level_library.py
--rw-r--r--   0        0        0     1237 2023-03-30 16:25:57.866546 splink-3.7.3/splink/comparison_level_sql.py
--rw-r--r--   0        0        0    26398 2023-03-30 16:25:57.866546 splink-3.7.3/splink/comparison_library.py
--rw-r--r--   0        0        0     1878 2023-03-30 16:25:57.866546 splink-3.7.3/splink/comparison_library_utils.py
--rw-r--r--   0        0        0    18523 2023-03-30 16:25:57.866546 splink-3.7.3/splink/comparison_template_library.py
--rw-r--r--   0        0        0      971 2023-03-30 16:25:57.866546 splink-3.7.3/splink/comparison_vector_distribution.py
--rw-r--r--   0        0        0      868 2023-03-30 16:25:57.866546 splink-3.7.3/splink/comparison_vector_values.py
--rw-r--r--   0        0        0    16516 2023-03-30 16:25:57.866546 splink-3.7.3/splink/connected_components.py
--rw-r--r--   0        0        0       67 2023-03-30 16:25:57.866546 splink-3.7.3/splink/constants.py
--rw-r--r--   0        0        0     6089 2023-03-30 16:25:57.866546 splink-3.7.3/splink/convert_v2_to_v3.py
--rw-r--r--   0        0        0     1338 2023-03-30 16:25:57.866546 splink-3.7.3/splink/databricks/enable_splink.py
--rw-r--r--   0        0        0      609 2023-03-30 16:25:57.866546 splink-3.7.3/splink/default_from_jsonschema.py
--rw-r--r--   0        0        0     1269 2023-03-30 16:25:57.866546 splink-3.7.3/splink/dialect_base.py
--rw-r--r--   0        0        0      878 2023-03-30 16:25:57.866546 splink-3.7.3/splink/duckdb/duckdb_base.py
--rw-r--r--   0        0        0     1321 2023-03-30 16:25:57.866546 splink-3.7.3/splink/duckdb/duckdb_comparison_level_library.py
--rw-r--r--   0        0        0     2602 2023-03-30 16:25:57.866546 splink-3.7.3/splink/duckdb/duckdb_comparison_library.py
--rw-r--r--   0        0        0      311 2023-03-30 16:25:57.866546 splink-3.7.3/splink/duckdb/duckdb_comparison_template_library.py
--rw-r--r--   0        0        0     1750 2023-03-30 16:25:57.866546 splink-3.7.3/splink/duckdb/duckdb_helpers.py
--rw-r--r--   0        0        0     9957 2023-03-30 16:25:57.866546 splink-3.7.3/splink/duckdb/duckdb_linker.py
--rw-r--r--   0        0        0    17471 2023-03-30 16:25:57.866546 splink-3.7.3/splink/em_training_session.py
--rw-r--r--   0        0        0     5227 2023-03-30 16:25:57.866546 splink-3.7.3/splink/estimate_u.py
--rw-r--r--   0        0        0      144 2023-03-30 16:25:57.866546 splink-3.7.3/splink/exceptions.py
--rw-r--r--   0        0        0     6062 2023-03-30 16:25:57.866546 splink-3.7.3/splink/expectation_maximisation.py
--rw-r--r--   0        0        0     1558 2023-03-30 16:25:57.866546 splink-3.7.3/splink/files/chart_defs/blocking_rule_generated_comparisons.json
--rw-r--r--   0        0        0     2779 2023-03-30 16:25:57.866546 splink-3.7.3/splink/files/chart_defs/completeness.json
--rw-r--r--   0        0        0     6737 2023-03-30 16:25:57.866546 splink-3.7.3/splink/files/chart_defs/del/bayes_factor_history_chart_def.json
--rw-r--r--   0        0        0     7747 2023-03-30 16:25:57.866546 splink-3.7.3/splink/files/chart_defs/del/bayes_factor_intuition_chart_def.json
--rw-r--r--   0        0        0     6298 2023-03-30 16:25:57.866546 splink-3.7.3/splink/files/chart_defs/del/compare_estimates.json
--rw-r--r--   0        0        0     2155 2023-03-30 16:25:57.866546 splink-3.7.3/splink/files/chart_defs/del/gamma_distribution_chart_def.json
--rw-r--r--   0        0        0      743 2023-03-30 16:25:57.866546 splink-3.7.3/splink/files/chart_defs/del/gamma_histogram.json
--rw-r--r--   0        0        0     1309 2023-03-30 16:25:57.866546 splink-3.7.3/splink/files/chart_defs/del/score_histogram.json
--rw-r--r--   0        0        0     5831 2023-03-30 16:25:57.866546 splink-3.7.3/splink/files/chart_defs/m_u_parameters_interactive_history.json
--rw-r--r--   0        0        0      977 2023-03-30 16:25:57.866546 splink-3.7.3/splink/files/chart_defs/match_weight_histogram.json
--rw-r--r--   0        0        0     5766 2023-03-30 16:25:57.866546 splink-3.7.3/splink/files/chart_defs/match_weights_interactive_history.json
--rw-r--r--   0        0        0     9159 2023-03-30 16:25:57.866546 splink-3.7.3/splink/files/chart_defs/match_weights_waterfall.json
--rw-r--r--   0        0        0     1734 2023-03-30 16:25:57.866546 splink-3.7.3/splink/files/chart_defs/missingness.json
--rw-r--r--   0        0        0     1730 2023-03-30 16:25:57.866546 splink-3.7.3/splink/files/chart_defs/parameter_estimate_comparisons.json
--rw-r--r--   0        0        0     1350 2023-03-30 16:25:57.866546 splink-3.7.3/splink/files/chart_defs/precision_recall.json
--rw-r--r--   0        0        0     1123 2023-03-30 16:25:57.866546 splink-3.7.3/splink/files/chart_defs/probability_two_random_records_match_iteration.json
--rw-r--r--   0        0        0     2326 2023-03-30 16:25:57.866546 splink-3.7.3/splink/files/chart_defs/profile_data.json
--rw-r--r--   0        0        0     1630 2023-03-30 16:25:57.866546 splink-3.7.3/splink/files/chart_defs/roc.json
--rw-r--r--   0        0        0     2645 2023-03-30 16:25:57.866546 splink-3.7.3/splink/files/chart_defs/unlinkables_chart_def.json
--rw-r--r--   0        0        0    66064 2023-03-30 16:25:57.866546 splink-3.7.3/splink/files/external_js/vega-embed@6.20.2
--rw-r--r--   0        0        0   256817 2023-03-30 16:25:57.870546 splink-3.7.3/splink/files/external_js/vega-lite@5.2.0
--rw-r--r--   0        0        0   501599 2023-03-30 16:25:57.874546 splink-3.7.3/splink/files/external_js/vega@5.21.0
--rw-r--r--   0        0        0    12871 2023-03-30 16:25:57.874546 splink-3.7.3/splink/files/settings_jsonschema.json
--rw-r--r--   0        0        0  1228220 2023-03-30 16:25:57.882546 splink-3.7.3/splink/files/spark_jars/scala-udf-similarity-0.1.0_classic.jar
--rw-r--r--   0        0        0   944614 2023-03-30 16:25:57.886546 splink-3.7.3/splink/files/spark_jars/scala-udf-similarity-0.1.0_spark3.3.jar
--rw-r--r--   0        0        0     5486 2023-03-30 16:25:57.886546 splink-3.7.3/splink/files/splink_cluster_studio/cluster_template.j2
--rw-r--r--   0        0        0     2269 2023-03-30 16:25:57.890546 splink-3.7.3/splink/files/splink_cluster_studio/custom.css
--rw-r--r--   0        0        0     2269 2023-03-30 16:25:57.890546 splink-3.7.3/splink/files/splink_comparison_viewer/custom.css
--rw-r--r--   0        0        0     3115 2023-03-30 16:25:57.890546 splink-3.7.3/splink/files/splink_comparison_viewer/template.j2
--rw-r--r--   0        0        0   269522 2023-03-30 16:25:57.890546 splink-3.7.3/splink/files/splink_vis_utils/splink_vis_utils.js
--rw-r--r--   0        0        0      404 2023-03-30 16:25:57.890546 splink-3.7.3/splink/files/templates/single_chart_template.txt
--rw-r--r--   0        0        0      195 2023-03-30 16:25:57.890546 splink-3.7.3/splink/format_sql.py
--rw-r--r--   0        0        0     7955 2023-03-30 16:25:57.890546 splink-3.7.3/splink/input_column.py
--rw-r--r--   0        0        0   114337 2023-03-30 16:25:57.890546 splink-3.7.3/splink/linker.py
--rw-r--r--   0        0        0      300 2023-03-30 16:25:57.890546 splink-3.7.3/splink/logging_messages.py
--rw-r--r--   0        0        0     3132 2023-03-30 16:25:57.890546 splink-3.7.3/splink/lower_id_on_lhs.py
--rw-r--r--   0        0        0     1834 2023-03-30 16:25:57.890546 splink-3.7.3/splink/m_from_labels.py
--rw-r--r--   0        0        0     2465 2023-03-30 16:25:57.890546 splink-3.7.3/splink/m_training.py
--rw-r--r--   0        0        0     2420 2023-03-30 16:25:57.890546 splink-3.7.3/splink/m_u_records_to_parameters.py
--rw-r--r--   0        0        0      623 2023-03-30 16:25:57.890546 splink-3.7.3/splink/match_key_analysis.py
--rw-r--r--   0        0        0     2028 2023-03-30 16:25:57.890546 splink-3.7.3/splink/match_weights_histogram.py
--rw-r--r--   0        0        0     4537 2023-03-30 16:25:57.890546 splink-3.7.3/splink/misc.py
--rw-r--r--   0        0        0     2805 2023-03-30 16:25:57.890546 splink-3.7.3/splink/missingness.py
--rw-r--r--   0        0        0     1221 2023-03-30 16:25:57.890546 splink-3.7.3/splink/parse_sql.py
--rw-r--r--   0        0        0     2909 2023-03-30 16:25:57.890546 splink-3.7.3/splink/pipeline.py
--rw-r--r--   0        0        0     3205 2023-03-30 16:25:57.890546 splink-3.7.3/splink/predict.py
--rw-r--r--   0        0        0     8245 2023-03-30 16:25:57.890546 splink-3.7.3/splink/profile_data.py
--rw-r--r--   0        0        0    18513 2023-03-30 16:25:57.890546 splink-3.7.3/splink/settings.py
--rw-r--r--   0        0        0     1083 2023-03-30 16:25:57.890546 splink-3.7.3/splink/spark/custom_spark_dialect.py
--rw-r--r--   0        0        0      473 2023-03-30 16:25:57.890546 splink-3.7.3/splink/spark/jar_location.py
--rw-r--r--   0        0        0      891 2023-03-30 16:25:57.890546 splink-3.7.3/splink/spark/spark_base.py
--rw-r--r--   0        0        0     1307 2023-03-30 16:25:57.890546 splink-3.7.3/splink/spark/spark_comparison_level_library.py
--rw-r--r--   0        0        0     2589 2023-03-30 16:25:57.890546 splink-3.7.3/splink/spark/spark_comparison_library.py
--rw-r--r--   0        0        0      320 2023-03-30 16:25:57.890546 splink-3.7.3/splink/spark/spark_comparison_template_library.py
--rw-r--r--   0        0        0    21107 2023-03-30 16:25:57.890546 splink-3.7.3/splink/spark/spark_linker.py
--rw-r--r--   0        0        0     4507 2023-03-30 16:25:57.890546 splink-3.7.3/splink/splink_comparison_viewer.py
--rw-r--r--   0        0        0     3220 2023-03-30 16:25:57.890546 splink-3.7.3/splink/splink_dataframe.py
--rw-r--r--   0        0        0     1181 2023-03-30 16:25:57.890546 splink-3.7.3/splink/sql_transform.py
--rw-r--r--   0        0        0      147 2023-03-30 16:25:57.890546 splink-3.7.3/splink/sqlite/sqlite_base.py
--rw-r--r--   0        0        0      750 2023-03-30 16:25:57.890546 splink-3.7.3/splink/sqlite/sqlite_comparison_level_library.py
--rw-r--r--   0        0        0      835 2023-03-30 16:25:57.890546 splink-3.7.3/splink/sqlite/sqlite_comparison_library.py
--rw-r--r--   0        0        0     5542 2023-03-30 16:25:57.890546 splink-3.7.3/splink/sqlite/sqlite_linker.py
--rw-r--r--   0        0        0     4453 2023-03-30 16:25:57.890546 splink-3.7.3/splink/term_frequencies.py
--rw-r--r--   0        0        0     1030 2023-03-30 16:25:57.890546 splink-3.7.3/splink/unique_id_concat.py
--rw-r--r--   0        0        0     1424 2023-03-30 16:25:57.890546 splink-3.7.3/splink/unlinkables.py
--rw-r--r--   0        0        0     2431 2023-03-30 16:25:57.890546 splink-3.7.3/splink/validate_jsonschema.py
--rw-r--r--   0        0        0     2250 2023-03-30 16:25:57.890546 splink-3.7.3/splink/vertically_concatenate.py
--rw-r--r--   0        0        0     5342 2023-03-30 16:25:57.890546 splink-3.7.3/splink/waterfall_chart.py
--rw-r--r--   0        0        0     9352 1970-01-01 00:00:00.000000 splink-3.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-04-25 14:03:55.263020 splink-3.8.0/LICENSE
+-rw-r--r--   0        0        0     8448 2023-04-25 14:03:55.263020 splink-3.8.0/README.md
+-rw-r--r--   0        0        0     1451 2023-04-25 14:03:55.283021 splink-3.8.0/pyproject.toml
+-rw-r--r--   0        0        0       23 2023-04-25 14:03:55.283021 splink-3.8.0/splink/__init__.py
+-rw-r--r--   0        0        0    10852 2023-04-25 14:03:55.283021 splink-3.8.0/splink/accuracy.py
+-rw-r--r--   0        0        0     4753 2023-04-25 14:03:55.283021 splink-3.8.0/splink/analyse_blocking.py
+-rw-r--r--   0        0        0      461 2023-04-25 14:03:55.283021 splink-3.8.0/splink/athena/athena_base.py
+-rw-r--r--   0        0        0     1672 2023-04-25 14:03:55.283021 splink-3.8.0/splink/athena/athena_comparison_level_library.py
+-rw-r--r--   0        0        0     1015 2023-04-25 14:03:55.283021 splink-3.8.0/splink/athena/athena_comparison_library.py
+-rw-r--r--   0        0        0    20569 2023-04-25 14:03:55.283021 splink-3.8.0/splink/athena/athena_linker.py
+-rw-r--r--   0        0        0      350 2023-04-25 14:03:55.283021 splink-3.8.0/splink/athena/athena_transforms.py
+-rw-r--r--   0        0        0     2904 2023-04-25 14:03:55.283021 splink-3.8.0/splink/athena/athena_utils.py
+-rw-r--r--   0        0        0     2867 2023-04-25 14:03:55.283021 splink-3.8.0/splink/block_from_labels.py
+-rw-r--r--   0        0        0     5965 2023-04-25 14:03:55.283021 splink-3.8.0/splink/blocking.py
+-rw-r--r--   0        0        0    10627 2023-04-25 14:03:55.283021 splink-3.8.0/splink/charts.py
+-rw-r--r--   0        0        0     9088 2023-04-25 14:03:55.283021 splink-3.8.0/splink/cluster_studio.py
+-rw-r--r--   0        0        0    16881 2023-04-25 14:03:55.283021 splink-3.8.0/splink/comparison.py
+-rw-r--r--   0        0        0    25479 2023-04-25 14:03:55.283021 splink-3.8.0/splink/comparison_level.py
+-rw-r--r--   0        0        0     9013 2023-04-25 14:03:55.283021 splink-3.8.0/splink/comparison_level_composition.py
+-rw-r--r--   0        0        0    25022 2023-04-25 14:03:55.283021 splink-3.8.0/splink/comparison_level_library.py
+-rw-r--r--   0        0        0     1237 2023-04-25 14:03:55.283021 splink-3.8.0/splink/comparison_level_sql.py
+-rw-r--r--   0        0        0    35793 2023-04-25 14:03:55.287021 splink-3.8.0/splink/comparison_library.py
+-rw-r--r--   0        0        0     4315 2023-04-25 14:03:55.287021 splink-3.8.0/splink/comparison_library_utils.py
+-rw-r--r--   0        0        0    23009 2023-04-25 14:03:55.287021 splink-3.8.0/splink/comparison_template_library.py
+-rw-r--r--   0        0        0      972 2023-04-25 14:03:55.287021 splink-3.8.0/splink/comparison_vector_distribution.py
+-rw-r--r--   0        0        0      868 2023-04-25 14:03:55.287021 splink-3.8.0/splink/comparison_vector_values.py
+-rw-r--r--   0        0        0    16516 2023-04-25 14:03:55.287021 splink-3.8.0/splink/connected_components.py
+-rw-r--r--   0        0        0       67 2023-04-25 14:03:55.287021 splink-3.8.0/splink/constants.py
+-rw-r--r--   0        0        0     6089 2023-04-25 14:03:55.287021 splink-3.8.0/splink/convert_v2_to_v3.py
+-rw-r--r--   0        0        0     1338 2023-04-25 14:03:55.287021 splink-3.8.0/splink/databricks/enable_splink.py
+-rw-r--r--   0        0        0      609 2023-04-25 14:03:55.287021 splink-3.8.0/splink/default_from_jsonschema.py
+-rw-r--r--   0        0        0     1332 2023-04-25 14:03:55.287021 splink-3.8.0/splink/dialect_base.py
+-rw-r--r--   0        0        0     1332 2023-04-25 14:03:55.287021 splink-3.8.0/splink/duckdb/duckdb_base.py
+-rw-r--r--   0        0        0     2369 2023-04-25 14:03:55.287021 splink-3.8.0/splink/duckdb/duckdb_comparison_level_library.py
+-rw-r--r--   0        0        0     1823 2023-04-25 14:03:55.287021 splink-3.8.0/splink/duckdb/duckdb_comparison_library.py
+-rw-r--r--   0        0        0      543 2023-04-25 14:03:55.287021 splink-3.8.0/splink/duckdb/duckdb_comparison_template_library.py
+-rw-r--r--   0        0        0     1750 2023-04-25 14:03:55.287021 splink-3.8.0/splink/duckdb/duckdb_helpers.py
+-rw-r--r--   0        0        0     9974 2023-04-25 14:03:55.287021 splink-3.8.0/splink/duckdb/duckdb_linker.py
+-rw-r--r--   0        0        0    17471 2023-04-25 14:03:55.287021 splink-3.8.0/splink/em_training_session.py
+-rw-r--r--   0        0        0     5244 2023-04-25 14:03:55.287021 splink-3.8.0/splink/estimate_u.py
+-rw-r--r--   0        0        0      144 2023-04-25 14:03:55.287021 splink-3.8.0/splink/exceptions.py
+-rw-r--r--   0        0        0     6062 2023-04-25 14:03:55.287021 splink-3.8.0/splink/expectation_maximisation.py
+-rw-r--r--   0        0        0     1558 2023-04-25 14:03:55.287021 splink-3.8.0/splink/files/chart_defs/blocking_rule_generated_comparisons.json
+-rw-r--r--   0        0        0     2779 2023-04-25 14:03:55.287021 splink-3.8.0/splink/files/chart_defs/completeness.json
+-rw-r--r--   0        0        0     6737 2023-04-25 14:03:55.287021 splink-3.8.0/splink/files/chart_defs/del/bayes_factor_history_chart_def.json
+-rw-r--r--   0        0        0     7747 2023-04-25 14:03:55.287021 splink-3.8.0/splink/files/chart_defs/del/bayes_factor_intuition_chart_def.json
+-rw-r--r--   0        0        0     6298 2023-04-25 14:03:55.287021 splink-3.8.0/splink/files/chart_defs/del/compare_estimates.json
+-rw-r--r--   0        0        0     2155 2023-04-25 14:03:55.287021 splink-3.8.0/splink/files/chart_defs/del/gamma_distribution_chart_def.json
+-rw-r--r--   0        0        0      743 2023-04-25 14:03:55.287021 splink-3.8.0/splink/files/chart_defs/del/gamma_histogram.json
+-rw-r--r--   0        0        0     1309 2023-04-25 14:03:55.287021 splink-3.8.0/splink/files/chart_defs/del/score_histogram.json
+-rw-r--r--   0        0        0     5831 2023-04-25 14:03:55.287021 splink-3.8.0/splink/files/chart_defs/m_u_parameters_interactive_history.json
+-rw-r--r--   0        0        0      977 2023-04-25 14:03:55.287021 splink-3.8.0/splink/files/chart_defs/match_weight_histogram.json
+-rw-r--r--   0        0        0     5766 2023-04-25 14:03:55.287021 splink-3.8.0/splink/files/chart_defs/match_weights_interactive_history.json
+-rw-r--r--   0        0        0     9159 2023-04-25 14:03:55.287021 splink-3.8.0/splink/files/chart_defs/match_weights_waterfall.json
+-rw-r--r--   0        0        0     1734 2023-04-25 14:03:55.287021 splink-3.8.0/splink/files/chart_defs/missingness.json
+-rw-r--r--   0        0        0     1730 2023-04-25 14:03:55.287021 splink-3.8.0/splink/files/chart_defs/parameter_estimate_comparisons.json
+-rw-r--r--   0        0        0     1465 2023-04-25 14:03:55.287021 splink-3.8.0/splink/files/chart_defs/precision_recall.json
+-rw-r--r--   0        0        0     1123 2023-04-25 14:03:55.287021 splink-3.8.0/splink/files/chart_defs/probability_two_random_records_match_iteration.json
+-rw-r--r--   0        0        0     2326 2023-04-25 14:03:55.287021 splink-3.8.0/splink/files/chart_defs/profile_data.json
+-rw-r--r--   0        0        0     1745 2023-04-25 14:03:55.287021 splink-3.8.0/splink/files/chart_defs/roc.json
+-rw-r--r--   0        0        0     2645 2023-04-25 14:03:55.287021 splink-3.8.0/splink/files/chart_defs/unlinkables_chart_def.json
+-rw-r--r--   0        0        0    66064 2023-04-25 14:03:55.287021 splink-3.8.0/splink/files/external_js/vega-embed@6.20.2
+-rw-r--r--   0        0        0   256817 2023-04-25 14:03:55.291021 splink-3.8.0/splink/files/external_js/vega-lite@5.2.0
+-rw-r--r--   0        0        0   501599 2023-04-25 14:03:55.291021 splink-3.8.0/splink/files/external_js/vega@5.21.0
+-rw-r--r--   0        0        0    12871 2023-04-25 14:03:55.291021 splink-3.8.0/splink/files/settings_jsonschema.json
+-rw-r--r--   0        0        0  1228220 2023-04-25 14:03:55.303022 splink-3.8.0/splink/files/spark_jars/scala-udf-similarity-0.1.0_classic.jar
+-rw-r--r--   0        0        0   944614 2023-04-25 14:03:55.307022 splink-3.8.0/splink/files/spark_jars/scala-udf-similarity-0.1.0_spark3.3.jar
+-rw-r--r--   0        0        0   949562 2023-04-25 14:03:55.307022 splink-3.8.0/splink/files/spark_jars/scala-udf-similarity-0.1.1_spark3.x.jar
+-rw-r--r--   0        0        0     5486 2023-04-25 14:03:55.307022 splink-3.8.0/splink/files/splink_cluster_studio/cluster_template.j2
+-rw-r--r--   0        0        0     2269 2023-04-25 14:03:55.307022 splink-3.8.0/splink/files/splink_cluster_studio/custom.css
+-rw-r--r--   0        0        0     2269 2023-04-25 14:03:55.307022 splink-3.8.0/splink/files/splink_comparison_viewer/custom.css
+-rw-r--r--   0        0        0     3115 2023-04-25 14:03:55.307022 splink-3.8.0/splink/files/splink_comparison_viewer/template.j2
+-rw-r--r--   0        0        0   269522 2023-04-25 14:03:55.307022 splink-3.8.0/splink/files/splink_vis_utils/splink_vis_utils.js
+-rw-r--r--   0        0        0      404 2023-04-25 14:03:55.307022 splink-3.8.0/splink/files/templates/single_chart_template.txt
+-rw-r--r--   0        0        0      195 2023-04-25 14:03:55.307022 splink-3.8.0/splink/format_sql.py
+-rw-r--r--   0        0        0     7955 2023-04-25 14:03:55.307022 splink-3.8.0/splink/input_column.py
+-rw-r--r--   0        0        0   119034 2023-04-25 14:03:55.311022 splink-3.8.0/splink/linker.py
+-rw-r--r--   0        0        0      300 2023-04-25 14:03:55.311022 splink-3.8.0/splink/logging_messages.py
+-rw-r--r--   0        0        0     3132 2023-04-25 14:03:55.311022 splink-3.8.0/splink/lower_id_on_lhs.py
+-rw-r--r--   0        0        0     1834 2023-04-25 14:03:55.311022 splink-3.8.0/splink/m_from_labels.py
+-rw-r--r--   0        0        0     2465 2023-04-25 14:03:55.311022 splink-3.8.0/splink/m_training.py
+-rw-r--r--   0        0        0     2420 2023-04-25 14:03:55.311022 splink-3.8.0/splink/m_u_records_to_parameters.py
+-rw-r--r--   0        0        0      623 2023-04-25 14:03:55.311022 splink-3.8.0/splink/match_key_analysis.py
+-rw-r--r--   0        0        0     2028 2023-04-25 14:03:55.311022 splink-3.8.0/splink/match_weights_histogram.py
+-rw-r--r--   0        0        0     4386 2023-04-25 14:03:55.311022 splink-3.8.0/splink/misc.py
+-rw-r--r--   0        0        0     2791 2023-04-25 14:03:55.311022 splink-3.8.0/splink/missingness.py
+-rw-r--r--   0        0        0     1221 2023-04-25 14:03:55.311022 splink-3.8.0/splink/parse_sql.py
+-rw-r--r--   0        0        0     2909 2023-04-25 14:03:55.311022 splink-3.8.0/splink/pipeline.py
+-rw-r--r--   0        0        0     3205 2023-04-25 14:03:55.311022 splink-3.8.0/splink/predict.py
+-rw-r--r--   0        0        0     8245 2023-04-25 14:03:55.311022 splink-3.8.0/splink/profile_data.py
+-rw-r--r--   0        0        0    18517 2023-04-25 14:03:55.311022 splink-3.8.0/splink/settings.py
+-rw-r--r--   0        0        0     1083 2023-04-25 14:03:55.311022 splink-3.8.0/splink/spark/custom_spark_dialect.py
+-rw-r--r--   0        0        0      473 2023-04-25 14:03:55.311022 splink-3.8.0/splink/spark/jar_location.py
+-rw-r--r--   0        0        0     1641 2023-04-25 14:03:55.311022 splink-3.8.0/splink/spark/spark_base.py
+-rw-r--r--   0        0        0     2300 2023-04-25 14:03:55.311022 splink-3.8.0/splink/spark/spark_comparison_level_library.py
+-rw-r--r--   0        0        0     1812 2023-04-25 14:03:55.311022 splink-3.8.0/splink/spark/spark_comparison_library.py
+-rw-r--r--   0        0        0      538 2023-04-25 14:03:55.311022 splink-3.8.0/splink/spark/spark_comparison_template_library.py
+-rw-r--r--   0        0        0    22331 2023-04-25 14:03:55.311022 splink-3.8.0/splink/spark/spark_linker.py
+-rw-r--r--   0        0        0     4507 2023-04-25 14:03:55.311022 splink-3.8.0/splink/splink_comparison_viewer.py
+-rw-r--r--   0        0        0     3220 2023-04-25 14:03:55.311022 splink-3.8.0/splink/splink_dataframe.py
+-rw-r--r--   0        0        0     1181 2023-04-25 14:03:55.311022 splink-3.8.0/splink/sql_transform.py
+-rw-r--r--   0        0        0      147 2023-04-25 14:03:55.311022 splink-3.8.0/splink/sqlite/sqlite_base.py
+-rw-r--r--   0        0        0     1109 2023-04-25 14:03:55.311022 splink-3.8.0/splink/sqlite/sqlite_comparison_level_library.py
+-rw-r--r--   0        0        0      379 2023-04-25 14:03:55.311022 splink-3.8.0/splink/sqlite/sqlite_comparison_library.py
+-rw-r--r--   0        0        0     6052 2023-04-25 14:03:55.311022 splink-3.8.0/splink/sqlite/sqlite_linker.py
+-rw-r--r--   0        0        0     4453 2023-04-25 14:03:55.311022 splink-3.8.0/splink/term_frequencies.py
+-rw-r--r--   0        0        0     1030 2023-04-25 14:03:55.311022 splink-3.8.0/splink/unique_id_concat.py
+-rw-r--r--   0        0        0     1424 2023-04-25 14:03:55.311022 splink-3.8.0/splink/unlinkables.py
+-rw-r--r--   0        0        0     2431 2023-04-25 14:03:55.311022 splink-3.8.0/splink/validate_jsonschema.py
+-rw-r--r--   0        0        0     2326 2023-04-25 14:03:55.311022 splink-3.8.0/splink/vertically_concatenate.py
+-rw-r--r--   0        0        0     5342 2023-04-25 14:03:55.311022 splink-3.8.0/splink/waterfall_chart.py
+-rw-r--r--   0        0        0     9374 1970-01-01 00:00:00.000000 splink-3.8.0/PKG-INFO
```

### Comparing `splink-3.7.3/LICENSE` & `splink-3.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/README.md` & `splink-3.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 
 # Fast, accurate and scalable probabilistic data linkage
 
 Splink is a Python package for probabilistic record linkage (entity resolution) that allows you to deduplicate and link records from datasets without unique identifiers.
 
 ## Key Features
 
-- **Speed:** Capable of linking a million records on a laptop in approximately one minute.
-- **Accuracy:** Full support for term frequency adjustments and user-defined fuzzy matching logic.
-- **Scalability:** Execute linkage jobs in Python (using DuckDB) or big-data backends like AWS Athena or Spark for 100+ million records.
-- **Unsupervised Learning:** No training data is required, as models can be trained using an unsupervised approach.
-- **Interactive Outputs:** Provides a wide range of interactive outputs to help users understand their model and diagnose linkage problems.
+⚡ **Speed:** Capable of linking a million records on a laptop in approximately one minute.  
+🎯 **Accuracy:** Full support for term frequency adjustments and user-defined fuzzy matching logic.  
+🌐 **Scalability:** Execute linkage jobs in Python (using DuckDB) or big-data backends like AWS Athena or Spark for 100+ million records.  
+🎓 **Unsupervised Learning:** No training data is required, as models can be trained using an unsupervised approach.  
+📊 **Interactive Outputs:** Provides a wide range of interactive outputs to help users understand their model and diagnose linkage problems.
 
 Splink's core linkage algorithm is based on Fellegi-Sunter's model of record linkage, with various customizations to improve accuracy.
 
 ## What does Splink do?
 
 Consider the following records that lack a unique person identifier:
```

### Comparing `splink-3.7.3/pyproject.toml` & `splink-3.8.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "splink"
-version = "3.7.3"
+version = "3.8.0"
 description = "Fast probabilistic data linkage at scale"
-authors = ["Robin Linacre <robinlinacre@hotmail.com>", "Sam Lindsay", "Theodore Manassis", "Tom Hepworth", "Andy Bond"]
+authors = ["Robin Linacre <robinlinacre@hotmail.com>", "Sam Lindsay", "Theodore Manassis", "Tom Hepworth", "Andy Bond", "Ross Kennedy"]
 license = "MIT"
 homepage = "https://github.com/moj-analytical-services/splink"
 repository = "https://github.com/moj-analytical-services/splink"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.7"
```

### Comparing `splink-3.7.3/splink/accuracy.py` & `splink-3.8.0/splink/accuracy.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,29 +107,29 @@
 
     sql = """
     select
         truth_threshold,
         power(2, truth_threshold) / (1 + power(2, truth_threshold))
             as match_probability,
         row_count,
-        P,
-        N,
-        TP,
-        TN,
-        FP,
-        FN,
+        P as p,
+        N as n,
+        TP as tp,
+        TN as tn,
+        FP as fp,
+        FN as fn,
         P/row_count as P_rate,
         cast(N as float)/row_count as N_rate,
-        cast(TP as float)/P as TP_rate,
-        cast(TN as float)/N as TN_rate,
-        cast(FP as float)/N as FP_rate,
-        cast(FN as float)/P as FN_rate,
+        cast(TP as float)/P as tp_rate,
+        cast(TN as float)/N as tn_rate,
+        cast(FP as float)/N as fp_rate,
+        cast(FN as float)/P as fn_rate,
         cast(TP as float)/(TP+FP) as precision,
         cast(TP as float)/(TP+FN) as recall,
-        cast(TP as float)/(TP + (FP + FN)/2) as F1
+        cast(TP as float)/(TP + (FP + FN)/2) as f1
     from __splink__labels_with_pos_neg_grouped_with_truth_stats
     """
 
     sql = {"sql": sql, "output_table_name": "__splink__truth_space_table"}
     sqls.append(sql)
     return sqls
```

### Comparing `splink-3.7.3/splink/analyse_blocking.py` & `splink-3.8.0/splink/analyse_blocking.py`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/athena/athena_comparison_library.py` & `splink-3.8.0/splink/athena/athena_comparison_level_library.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,22 @@
-from ..comparison_library import (
-    ArrayIntersectAtSizesComparisonBase,
-    DistanceFunctionAtThresholdsComparisonBase,
-    DistanceInKMAtThresholdsComparisonBase,
-    ExactMatchBase,
-    LevenshteinAtThresholdsComparisonBase,
+from ..comparison_level_composition import and_, not_, or_  # noqa: F401
+from ..comparison_level_library import (
+    ArrayIntersectLevelBase,
+    ColumnsReversedLevelBase,
+    DistanceFunctionLevelBase,
+    DistanceInKMLevelBase,
+    ElseLevelBase,
+    ExactMatchLevelBase,
+    LevenshteinLevelBase,
+    NullLevelBase,
+    PercentageDifferenceLevelBase,
 )
 from .athena_base import (
     AthenaBase,
 )
-from .athena_comparison_level_library import (
-    array_intersect_level,
-    distance_function_level,
-    distance_in_km_level,
-    else_level,
-    exact_match_level,
-    levenshtein_level,
-    null_level,
-)
 
 
 class AthenaComparisonProperties(AthenaBase):
     @property
     def _exact_match_level(self):
         return exact_match_level
 
@@ -36,38 +32,50 @@
     def _array_intersect_level(self):
         return array_intersect_level
 
     @property
     def _distance_in_km_level(self):
         return distance_in_km_level
 
+    @property
+    def _distance_function_level(self):
+        return distance_function_level
+
+    @property
+    def _levenshtein_level(self):
+        return levenshtein_level
+
 
-class exact_match(AthenaComparisonProperties, ExactMatchBase):
+class null_level(AthenaBase, NullLevelBase):
     pass
 
 
-class distance_function_at_thresholds(
-    AthenaComparisonProperties, DistanceFunctionAtThresholdsComparisonBase
-):
-    @property
-    def _distance_level(self):
-        return distance_function_level
+class exact_match_level(AthenaBase, ExactMatchLevelBase):
+    pass
 
 
-class levenshtein_at_thresholds(
-    AthenaComparisonProperties, LevenshteinAtThresholdsComparisonBase
-):
-    @property
-    def _distance_level(self):
-        return levenshtein_level
+class else_level(AthenaBase, ElseLevelBase):
+    pass
+
+
+class columns_reversed_level(AthenaBase, ColumnsReversedLevelBase):
+    pass
+
+
+class distance_function_level(AthenaBase, DistanceFunctionLevelBase):
+    pass
+
+
+class levenshtein_level(AthenaBase, LevenshteinLevelBase):
+    pass
+
+
+class array_intersect_level(AthenaBase, ArrayIntersectLevelBase):
+    pass
 
 
-class array_intersect_at_sizes(
-    AthenaComparisonProperties, ArrayIntersectAtSizesComparisonBase
-):
+class percentage_difference_level(AthenaBase, PercentageDifferenceLevelBase):
     pass
 
 
-class distance_in_km_at_thresholds(
-    AthenaComparisonProperties, DistanceInKMAtThresholdsComparisonBase
-):
+class distance_in_km_level(AthenaBase, DistanceInKMLevelBase):
     pass
```

### Comparing `splink-3.7.3/splink/athena/athena_linker.py` & `splink-3.8.0/splink/athena/athena_linker.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,97 +1,74 @@
 from __future__ import annotations
 
 import logging
 import os
-import uuid
 
 import awswrangler as wr
 import boto3
 import numpy as np
 import pandas as pd
 
 from ..athena.athena_transforms import cast_concat_as_varchar
-from ..athena.athena_utils import boto_utils
+from ..athena.athena_utils import (
+    _garbage_collection,
+    _verify_athena_inputs,
+)
 from ..input_column import InputColumn
 from ..linker import Linker
 from ..logging_messages import execute_sql_logging_message_info, log_sql
 from ..misc import ensure_is_list
 from ..splink_dataframe import SplinkDataFrame
 from ..sql_transform import sqlglot_transform_sql
 
 logger = logging.getLogger(__name__)
 
 
-def _verify_athena_inputs(database, bucket, boto3_session):
-    def generic_warning_text():
-        return (
-            f"\nThe supplied {database_bucket_txt} that you have requested to write to "
-            f"{do_does_grammar[0]} not currently exist. \n \nCreate "
-            "{do_does_grammar[1]} either directly from within AWS, or by using "
-            "'awswrangler.athena.create_athena_bucket' for buckets or "
-            "'awswrangler.catalog.create_database' for databases using the "
-            "awswrangler API."
-        )
-
-    errors = []
-
-    if (
-        database
-        not in wr.catalog.databases(limit=None, boto3_session=boto3_session).values
-    ):
-        errors.append(f"database, '{database}'")
-
-    if bucket not in wr.s3.list_buckets(boto3_session=boto3_session):
-        errors.append(f"bucket, '{bucket}'")
-
-    if errors:
-        database_bucket_txt = " and ".join(errors)
-        do_does_grammar = ["does", "it"] if len(errors) == 1 else ["do", "them"]
-        raise Exception(generic_warning_text())
-
-
 class AthenaDataFrame(SplinkDataFrame):
     linker: AthenaLinker
 
     @property
     def columns(self):
-        t = self.get_schema_info(self.physical_name)
+        db, tb = self.linker.get_schema_info(self.physical_name)
         d = wr.catalog.get_table_types(
-            database=t[0],
-            table=t[1],
+            database=db,
+            table=tb,
             boto3_session=self.linker.boto3_session,
         )
 
         cols = list(d.keys())
         return [InputColumn(c, sql_dialect="presto") for c in cols]
 
     def validate(self):
         pass
 
     def drop_table_from_database(self, force_non_splink_table=False):
+        # Check folder and table set for deletion
         self._check_drop_folder_created_by_splink(force_non_splink_table)
         self._check_drop_table_created_by_splink(force_non_splink_table)
-        self.linker.drop_table_from_database_if_exists(self.physical_name)
-        self.linker.delete_table_from_s3(self.physical_name)
+
+        # Delete the table from s3 and your database
+        self.linker._drop_table_from_database_if_exists(self.physical_name)
+        self.linker._delete_table_from_s3(self.physical_name)
 
     def _check_drop_folder_created_by_splink(self, force_non_splink_table=False):
-        filepath = self.linker.boto_utils.s3_output
+        filepath = self.linker.s3_output
         filename = self.physical_name
         # Validate that the folder is a splink generated folder...
         files = wr.s3.list_objects(
             path=os.path.join(filepath, filename),
             boto3_session=self.linker.boto3_session,
             ignore_empty=True,
         )
 
         if len(files) == 0:
             if not force_non_splink_table:
                 raise ValueError(
                     f"You've asked to drop data housed under the filepath "
-                    f"{self.linker.boto_utils.s3_output} from your "
+                    f"{self.linker.s3_output} from your "
                     "s3 output bucket, which is not a folder created by "
                     "Splink. If you really want to delete this data, you "
                     "can do so by setting force_non_splink_table=True."
                 )
 
         # validate that the ctas_query_info is for the given table
         # we're interacting with
@@ -114,44 +91,39 @@
         """
         if limit:
             sql += f" limit {limit}"
 
         out_df = wr.athena.read_sql_query(
             sql=sql,
             database=self.linker.output_schema,
-            s3_output=self.linker.boto_utils.s3_output,
+            s3_output=self.linker.s3_output,
             keep_files=False,
             ctas_approach=True,
             use_threads=True,
             boto3_session=self.linker.boto3_session,
         )
         return out_df
 
     def as_record_dict(self, limit=None):
         out_df = self.as_pandas_dataframe(limit)
         out_df = out_df.fillna(np.nan).replace([np.nan], [None])
         return out_df.to_dict(orient="records")
 
-    def get_schema_info(self, input_table):
-        t = input_table.split(".")
-        return t if len(t) > 1 else [self.linker.output_schema, self.physical_name]
-
 
 class AthenaLinker(Linker):
     def __init__(
         self,
         input_table_or_tables,
         boto3_session: boto3.session.Session,
         output_database: str,
         output_bucket: str,
         settings_dict: dict = None,
         input_table_aliases: str | list = None,
         set_up_basic_logging=True,
         output_filepath: str = "",
-        garbage_collection_level: int = 1,
     ):
         """An athena backend for our main linker class. This funnels our generated SQL
         through athena using awswrangler.
         See linker.py for more information on the main linker class.
         Attributes:
             input_table_or_tables (Union[str, list]): Input data into the linkage model.
                 Either a single string (the name of a table in a database) for
@@ -171,26 +143,14 @@
                 saves your tables under a custom name: '__splink__input_table_{n}';
                 where n is the list index.
             set_up_basic_logging (bool, optional): If true, sets ups up basic logging
                 so that Splink sends messages at INFO level to stdout. Defaults to True.
             output_filepath (str, optional): Inside of your selected output bucket,
                 where to write output files to.
                 Defaults to "splink_warehouse/{unique_id}".
-            garbage_collection_level (int, optional): Garbage collection cleans up both
-                your database and s3 bucket, deleting or unlinking any tables previously
-                generated by splink. 0, 1 and 2 are the accepted levels. Defaults to 1.
-
-                0 performs no cleaning. Existing tables will not be unlinked or deleted.
-                1 will unlink any tables with the '__splink_df' prefix within the
-                database you've specified for linking, but leaves the underlying
-                s3 files intact.
-                2 scans your specified output database for any tables with the
-                '__splink_df' prefix and both unlinks the database table and deletes
-                the backing data on s3.
-
         Examples:
             >>> # Creating a database in athena and writing to it
             >>> import awswrangler as wr
             >>> wr.catalog.create_database("splink_awswrangler_test", exist_ok=True)
             >>>
             >>> from splink.athena.athena_linker import AthenaLinker
             >>> import boto3
@@ -223,102 +183,131 @@
             >>>     input_table_or_tables="splink_awswrangler_test.synthetic_data_all",
             >>>     boto3_session=my_session,
             >>>     output_bucket="alpha-splink-db-testing",
             >>>     output_database="splink_awswrangler_test2",
             >>> )
         """
 
+        if not type(boto3_session) == boto3.session.Session:
+            raise ValueError("Please enter a valid boto3 session object.")
+
         self._sql_dialect_ = "presto"
 
+        _verify_athena_inputs(output_database, output_bucket, boto3_session)
         self.boto3_session = boto3_session
         self.output_schema = output_database
-        self.boto_utils = boto_utils(
-            boto3_session,
-            output_bucket,
-            output_filepath,
-        )
+        self.output_bucket = output_bucket
+
+        # If the default folder is blank, name it `splink_warehouse`
+        if output_filepath:
+            self.output_filepath = output_filepath
+        else:
+            self.output_filepath = "splink_warehouse"
+
+        # This query info dictionary is used to circumvent the need to run
+        # `wr.catalog.get_table_location` every time we want to delete
+        # the backing data from s3.
         self.ctas_query_info = {}
 
         # If user has provided pandas dataframes, need to register
         # them with the database, using user-provided aliases
         # if provided or a created alias if not
-
         input_tables = ensure_is_list(input_table_or_tables)
 
         input_aliases = self._ensure_aliases_populated_and_is_list(
             input_table_or_tables, input_table_aliases
         )
+        accepted_df_dtypes = pd.DataFrame
 
-        # 'homogenised' means all entries are strings representing tables
-        homogenised_tables = []
-        homogenised_aliases = []
-
-        for table, alias in zip(input_tables, input_aliases):
-            if type(table).__name__ == "DataFrame":
-                if type(alias).__name__ == "DataFrame":
-                    df_id = uuid.uuid4().hex[:7]
-                    alias = f"__splink__input_table_{df_id}"
-
-                self.register_data_on_s3(table, alias)
-
-            homogenised_tables.append(alias)
-            homogenised_aliases.append(alias)
+        # Run a quick check against our inputs to check if they
+        # exist in the database
+        for table in input_tables:
+            if not isinstance(table, accepted_df_dtypes):
+                db, tb = self.get_schema_info(table)
+                self.check_table_exists(db, tb)
 
         super().__init__(
-            homogenised_tables,
+            input_tables,
             settings_dict,
+            accepted_df_dtypes,
             set_up_basic_logging,
-            input_table_aliases=homogenised_aliases,
-        )
-
-        self._drop_all_tables_created_by_splink(
-            garbage_collection_level,
-            homogenised_aliases,
+            input_table_aliases=input_aliases,
         )
 
     def _table_to_splink_dataframe(self, templated_name, physical_name):
         return AthenaDataFrame(templated_name, physical_name, self)
 
     def change_output_filepath(self, new_filepath):
-        self.boto_utils = boto_utils(
-            self.boto3_session,
-            self.boto_utils.bucket,
-            new_filepath,
-        )
+        self.output_filepath = new_filepath
+
+    def get_schema_info(self, input_table):
+        t = input_table.split(".")
+        return t if len(t) > 1 else [self.output_schema, input_table]
+
+    @property
+    def s3_output(self):
+        out_path = os.path.join(
+            "s3://",
+            self.output_bucket,
+            self.output_filepath,
+            self._cache_uid,  # added in the super() step
+        )
+        if out_path[-1] != "/":
+            out_path += "/"
+
+        return out_path
+
+    def check_table_exists(self, db, tb):
+        # A quick function to check if a table exists
+        # and spit out a warning if it is not found.
+        table_exists = wr.catalog.does_table_exist(
+            database=db,
+            table=tb,
+        )
+        if not table_exists:
+            raise wr.exceptions.InvalidTable(
+                f"Table '{tb}' was not found within your selected "
+                f"database '{db}'. Please verify your input table "
+                "exists."
+            )
 
     def register_data_on_s3(self, table, alias):
+        out_loc = f"{self.s3_output}{alias}"
+
         wr.s3.to_parquet(
             df=table,
-            path=f"{self.boto_utils.s3_output}{alias}",
+            path=out_loc,
             dataset=True,
             mode="overwrite",
             database=self.output_schema,
             table=alias,
             boto3_session=self.boto3_session,
             compression="snappy",
             use_threads=True,
         )
+        # Construct the ctas metadata that we require
+        ctas_metadata = {
+            "ctas_database": self.output_schema,
+            "ctas_table": alias,
+        }
+        self.ctas_query_info.update({alias: ctas_metadata})
 
     def _execute_sql_against_backend(self, sql, templated_name, physical_name):
-        # Deletes the table in the db, but not the object on s3.
-        # This needs to be removed manually (full s3 path provided)
-        self.drop_table_from_database_if_exists(physical_name)
+        self._delete_table_from_database(physical_name)
         sql = sqlglot_transform_sql(sql, cast_concat_as_varchar)
         sql = sql.replace("FLOAT", "double").replace("float", "double")
 
         logger.debug(execute_sql_logging_message_info(templated_name, physical_name))
         logger.log(5, log_sql(sql))
 
         # create our table on athena and extract the metadata information
         query_metadata = self.create_table(sql, physical_name=physical_name)
         # append our metadata locations
-        self.ctas_query_info = {
-            **self.ctas_query_info,
-            **{physical_name: query_metadata},
-        }
+        query_metadata = self._extract_ctas_metadata(query_metadata)
+        self.ctas_query_info.update({physical_name: query_metadata})
 
         output_obj = self._table_to_splink_dataframe(templated_name, physical_name)
         return output_obj
 
     def register_table(self, input, table_name, overwrite=False):
         # If the user has provided a table name, return it as a SplinkDataframe
         if isinstance(input, str):
@@ -329,26 +318,27 @@
         if exists:
             if not overwrite:
                 raise ValueError(
                     f"Table '{table_name}' already exists in database. "
                     "Please use the 'overwrite' argument if you wish to overwrite"
                 )
             else:
-                self.drop_table_from_database_if_exists(table_name)
+                self._delete_table_from_database(table_name)
 
         if isinstance(input, dict):
             input = pd.DataFrame(input)
         elif isinstance(input, list):
             input = pd.DataFrame.from_records(input)
 
-        # Will error if an invalid data type is passed
+        # Errors if an invalid data type is passed
         self.register_data_on_s3(input, table_name)
+
         return self._table_to_splink_dataframe(table_name, table_name)
 
-    def _random_sample_sql(self, proportion, sample_size):
+    def _random_sample_sql(self, proportion, sample_size, seed=None):
         if proportion == 1.0:
             return ""
         percent = proportion * 100
         return f" TABLESAMPLE BERNOULLI ({percent})"
 
     @property
     def _infinity_expression(self):
@@ -366,99 +356,167 @@
         ctas_metadata = wr.athena.create_ctas_table(
             sql=sql,
             database=database,
             ctas_table=physical_name,
             storage_format="parquet",
             write_compression="snappy",
             boto3_session=self.boto3_session,
-            s3_output=self.boto_utils.s3_output,
+            s3_output=self.s3_output,
             wait=True,
         )
         return ctas_metadata
 
-    def drop_table_from_database_if_exists(self, table):
-        wr.catalog.delete_table_if_exists(
+    def _drop_table_from_database_if_exists(self, table):
+        return wr.catalog.delete_table_if_exists(
             database=self.output_schema, table=table, boto3_session=self.boto3_session
         )
 
-    def delete_table_from_s3(self, physical_name):
-        path = f"{self.boto_utils.s3_output}{physical_name}/"
-        metadata = self.ctas_query_info[physical_name]
-        metadata_urls = [
-            # metadata output location
-            f'{metadata["ctas_query_metadata"].output_location}.metadata',
-            # manifest location
-            metadata["ctas_query_metadata"].manifest_location,
-        ]
+    def _delete_table_from_s3(self, physical_name):
+        path = f"{self.s3_output}{physical_name}/"
         # delete our folder
         wr.s3.delete_objects(
             path=path,
             use_threads=True,
             boto3_session=self.boto3_session,
         )
-        # delete our metadata
-        wr.s3.delete_objects(
-            path=metadata_urls,
-            use_threads=True,
-            boto3_session=self.boto3_session,
-        )
+
+        metadata = self.ctas_query_info[physical_name]
+        if "output_location" in metadata:
+            metadata_urls = [
+                # metadata output location
+                f"{metadata['output_location']}.metadata",
+                # manifest location
+                metadata["manifest_location"],
+            ]
+            # delete our metadata
+            wr.s3.delete_objects(
+                path=metadata_urls,
+                use_threads=True,
+                boto3_session=self.boto3_session,
+            )
 
         self.ctas_query_info.pop(physical_name)
 
-    def _drop_all_tables_created_by_splink(
-        self, garbage_collection_level=1, input_tables=[]
-    ):
-        """A method that runs a cleanup process for the tables created by splink and
-        currently contained in your designated database.
+    def _delete_table_from_database(self, name):
 
-        Historic tables will not be wiped by this process, only those currently
-        contained on the database selected by the user.
+        if name in self.ctas_query_info:
+            # Use ctas metadata to delete backing data
+            self._delete_table_from_s3(name)
+        else:
+            # If the location we want to write to already exists,
+            # clean this before continuing.
+            loc = f"{self.s3_output}{name}"
+            folder_exists = wr.s3.list_directories(
+                loc,
+                boto3_session=self.boto3_session,
+            )
+            if folder_exists:
+                # This will only delete objects we are required to delete
+                wr.s3.delete_objects(
+                    path=loc,
+                    use_threads=True,
+                    boto3_session=self.boto3_session,
+                )
 
+        self._drop_table_from_database_if_exists(name)
+
+    def _extract_ctas_metadata(self, ctas_metadata):
+        query_meta = ctas_metadata.pop("ctas_query_metadata")
+        out_locs = {
+            "output_location": query_meta.output_location,
+            "manifest_location": query_meta.manifest_location,
+        }
+        ctas_metadata.update(out_locs)
+        return ctas_metadata
+
+    def drop_all_tables_created_by_splink(
+        self,
+        delete_s3_folders=True,
+        tables_to_exclude=[],
+    ):
+        """Run a cleanup process for the tables created by splink and
+        currently contained in your output database.
+        Only those tables currently contained within your database
+        will be permanently deleted. Anything existing on s3 that
+        isn't connected to your database will not be removed.
         Attributes:
-            garbage_collection_level (int): The amount of cleaning you wish to be
-            performed.
-                0 performs no cleaning. Existing tables will not be unlinked or deleted.
-                1 will unlink any tables with the '__splink_df' prefix within the
-                database you've specified for linking, but leaves the underlying
-                s3 files intact.
-                2 scans your specified output database for any tables with the
-                '__splink_df' prefix and both unlinks the database table and deletes
-                the backing data on s3.
-            input_tables (list): A list of input tables you wish to add to an ignore
-                list. These will not be removed during garbage collection.
+            delete_s3_folders (bool, optional): Whether to delete the
+                backing data contained on s3. If False, the tables created
+                by splink will be removed from your database, but the parquet
+                outputs will remain on s3. Defaults to True.
+            tables_to_exclude (list, optional): A list of input tables you wish to
+                add to an ignore list. These will not be removed during garbage
+                collection.
         """
-        # No collection requested
-        if garbage_collection_level == 0:
-            return
-
-        # This will only delete tables created within the splink process. These are
-        # tables containing the specific prefix: "__splink"
-        tables = wr.catalog.get_tables(
-            database=self.output_schema,
-            name_prefix="__splink",
-            boto3_session=self.boto3_session,
+        _garbage_collection(
+            self.output_schema,
+            self.boto3_session,
+            delete_s3_folders,
+            tables_to_exclude,
         )
-        delete_metadata_loc = []
-        for t in tables:
-            # Don't overwrite input tables if they have been
-            # given the __splink prefix.
-            if t["Name"] not in input_tables:
-                wr.catalog.delete_table_if_exists(
-                    database=t["DatabaseName"],
-                    table=t["Name"],
-                    boto3_session=self.boto3_session,
-                )
-                if garbage_collection_level == 2:
-                    path = t["StorageDescriptor"]["Location"]
-                    wr.s3.delete_objects(
-                        path=path,
-                        use_threads=True,
-                        boto3_session=self.boto3_session,
-                    )
-                    metadata_loc = f"{path.split('/__splink')[0]}/tables/"
-                    if metadata_loc not in delete_metadata_loc:
-                        wr.s3.delete_objects(
-                            path=metadata_loc,
-                            use_threads=True,
-                            boto3_session=self.boto3_session,
-                        )
-                        delete_metadata_loc.append(metadata_loc)
+
+    def drop_splink_tables_from_database(
+        self,
+        database_name: str,
+        delete_s3_folders: bool = True,
+        tables_to_exclude: list = [],
+    ):
+        """Run a cleanup process for the tables created by splink
+        in a specified database.
+        Only those tables currently contained within your database
+        will be permanently deleted. Anything existing on s3 that
+        isn't connected to your database will not be removed.
+        Attributes:
+            database_name (str): The name of the database to delete splink tables from.
+            delete_s3_folders (bool, optional): Whether to delete the
+                backing data contained on s3. If False, the tables created
+                by splink will be removed from your database, but the parquet
+                outputs will remain on s3. Defaults to True.
+            tables_to_exclude (list, optional): A list of input tables you wish to
+                add to an ignore list. These will not be removed during garbage
+                collection.
+        """
+        _garbage_collection(
+            database_name,
+            self.boto3_session,
+            delete_s3_folders,
+            tables_to_exclude,
+        )
+
+    def drop_tables_in_current_splink_run(
+        self,
+        delete_s3_folders: bool = True,
+        tables_to_exclude: list = [],
+    ):
+        """Run a cleanup process for the tables created
+        by the current splink linker.
+        This leaves tables from previous runs untouched.
+        Only those tables currently contained within your database
+        will be permanently deleted. Anything existing on s3 that
+        isn't connected to your database will not be removed.
+        Attributes:
+            delete_s3_folders (bool, optional): Whether to delete the
+                backing data contained on s3. If False, the tables created
+                by splink will be removed from your database, but the parquet
+                outputs will remain on s3. Defaults to True.
+            tables_to_exclude (list, optional): A list of input tables you wish to
+                add to an ignore list. These will not be removed during garbage
+                collection.
+        """
+        tables_to_exclude = ensure_is_list(tables_to_exclude)
+        tables_to_exclude = [
+            df.physical_name if isinstance(df, SplinkDataFrame) else df
+            for df in tables_to_exclude
+        ]
+        # Exclude tables that the user doesn't want to delete
+        tables = self._names_of_tables_created_by_splink.copy()
+        tables = [t for t in tables if t not in tables_to_exclude]
+
+        for table in tables:
+            _garbage_collection(
+                self.output_schema,
+                self.boto3_session,
+                delete_s3_folders,
+                name_prefix=table,
+            )
+            # pop from our tables created by splink list
+            self._names_of_tables_created_by_splink.remove(table)
```

### Comparing `splink-3.7.3/splink/block_from_labels.py` & `splink-3.8.0/splink/block_from_labels.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     `linker` object.
     """
 
     df = linker._table_to_splink_dataframe(labels_table_name, labels_table_name)
 
     unique_id_col = linker._settings_obj._unique_id_column_name
 
-    source_dataset_col = linker._settings_obj._source_dataset_column_name
+    source_dataset_col = linker._settings_obj._source_dataset_input_column
 
     sql = lower_id_to_left_hand_side(df, source_dataset_col, unique_id_col)
 
     sqls = []
     sql = {
         "sql": sql,
         "output_table_name": "__splink__labels_prepared_for_joining",
```

### Comparing `splink-3.7.3/splink/blocking.py` & `splink-3.8.0/splink/blocking.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
         )
 
     if (
         linker._two_dataset_link_only
         and not linker._find_new_matches_mode
         and not linker._compare_two_records_mode
     ):
-        source_dataset_col = linker._settings_obj._source_dataset_column_name
+        source_dataset_col = linker._source_dataset_column_name
         # Need df_l to be the one with the lowest id to preeserve the property
         # that the left dataset is the one with the lowest concatenated id
         keys = linker._input_tables_dict.keys()
         keys = list(sorted(keys))
         df_l = linker._input_tables_dict[keys[0]]
         df_r = linker._input_tables_dict[keys[1]]
```

### Comparing `splink-3.7.3/splink/charts.py` & `splink-3.8.0/splink/charts.py`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/cluster_studio.py` & `splink-3.8.0/splink/cluster_studio.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
     df_edges = linker._sql_to_splink_dataframe_checking_cache(
         sql, "__splink__scs_edges"
     )
     return df_edges.as_record_dict()
 
 
 def _get_random_cluster_ids(
-    linker: "Linker", connected_components: SplinkDataFrame, sample_size: int
+    linker: "Linker", connected_components: SplinkDataFrame, sample_size: int, seed=None
 ):
     sql = f"""
     select count(distinct cluster_id) as count
     from {connected_components.physical_name}
     """
     df_cluster_count = linker._sql_to_splink_dataframe_checking_cache(
         sql, "__splink__cluster_count"
@@ -133,15 +133,15 @@
 
     sql = f"""
     with distinct_clusters as (
     select distinct(cluster_id)
     from {connected_components.physical_name}
     )
     select cluster_id from distinct_clusters
-    {linker._random_sample_sql(proportion, sample_size)}
+    {linker._random_sample_sql(proportion, sample_size, seed)}
     """
 
     df_sample = linker._sql_to_splink_dataframe_checking_cache(
         sql,
         "__splink__df_concat_with_tf_sample",
     )
     return [r["cluster_id"] for r in df_sample.as_record_dict()]
@@ -184,29 +184,30 @@
 def render_splink_cluster_studio_html(
     linker: "Linker",
     df_predicted_edges: SplinkDataFrame,
     df_clustered_nodes: SplinkDataFrame,
     out_path: str,
     sampling_method="random",
     sample_size=10,
+    sample_seed=None,
     cluster_ids: list = None,
     cluster_names: list = None,
     overwrite: bool = False,
 ):
     bundle_observable_notebook = True
 
     svu_options = {
         "cluster_colname": "cluster_id",
         "prob_colname": "match_probability",
     }
     named_clusters_dict = None
     if cluster_ids is None:
         if sampling_method == "random":
             cluster_ids = _get_random_cluster_ids(
-                linker, df_clustered_nodes, sample_size
+                linker, df_clustered_nodes, sample_size, sample_seed
             )
         if sampling_method == "by_cluster_size":
             cluster_ids = _get_cluster_id_of_each_size(linker, df_clustered_nodes, 1)
             if len(cluster_ids) > sample_size:
                 cluster_ids = random.sample(cluster_ids, k=sample_size)
             cluster_names = [
                 f"Cluster ID: {c['cluster_id']}, size  {c['cluster_size']}"
```

### Comparing `splink-3.7.3/splink/comparison.py` & `splink-3.8.0/splink/comparison.py`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/comparison_level.py` & `splink-3.8.0/splink/comparison_level.py`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/comparison_level_composition.py` & `splink-3.8.0/splink/comparison_level_composition.py`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/comparison_level_sql.py` & `splink-3.8.0/splink/comparison_level_sql.py`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/comparison_library.py` & `splink-3.8.0/splink/comparison_library.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from __future__ import annotations
 
 from .comparison import Comparison
 from .comparison_library_utils import (
     comparison_at_thresholds_error_logger,
     datediff_error_logger,
+    distance_threshold_comparison_levels,
+    distance_threshold_description,
 )
 from .misc import ensure_is_iterable
 
 
 class ExactMatchBase(Comparison):
     def __init__(
         self,
         col_name,
         term_frequency_adjustments=False,
         m_probability_exact_match=None,
         m_probability_else=None,
         include_colname_in_charts_label=False,
-    ):
+    ) -> Comparison:
         """A comparison of the data in `col_name` with two levels:
         - Exact match
         - Anything else
 
         Args:
             col_name (str): The name of the column to compare
             term_frequency_adjustments (bool, optional): If True, term frequency
@@ -28,17 +30,26 @@
             m_probability_exact_match (_type_, optional): If provided, overrides the
                 default m probability for the exact match level. Defaults to None.
             m_probability_else (_type_, optional): If provided, overrides the
                 default m probability for the 'anything else' level. Defaults to None.
             include_colname_in_charts_label: If true, append col name to label for
                 charts.  Defaults to False.
 
+        Examples:
+            >>> # Simple DuckDB exact_match comparison
+            >>> import splink.duckdb.duckdb_comparison_library as cl
+            >>> cl.exact_match("first_name")
+
+            >>> # Simple Spark exact_match comparison
+            >>> import splink.spark.spark_comparison_library as cl
+            >>> cl.exact_match("first_name")
+
         Returns:
-            Comparison: A comparison that can be inclued in the Splink settings
-                dictionary
+            Comparison: A comparison for exact match that can be included in the Splink
+                settings dictionary
         """
 
         comparison_dict = {
             "comparison_description": "Exact match vs. anything else",
             "comparison_levels": [
                 self._null_level(col_name),
                 self._exact_match_level(
@@ -54,35 +65,39 @@
 
 
 class DistanceFunctionAtThresholdsComparisonBase(Comparison):
     def __init__(
         self,
         col_name: str,
         distance_function_name: str,
-        distance_threshold_or_thresholds: int | list,
+        distance_threshold_or_thresholds: float | list,
         higher_is_more_similar: bool = True,
         include_exact_match_level=True,
         term_frequency_adjustments=False,
         m_probability_exact_match=None,
-        m_probability_or_probabilities_lev: float | list = None,
+        m_probability_or_probabilities_thres: float | list = None,
         m_probability_else=None,
-    ):
+    ) -> Comparison:
         """A comparison of the data in `col_name` with a user-provided distance
         function used to assess middle similarity levels.
 
         The user-provided distance function must exist in the SQL backend.
 
         An example of the output with default arguments and setting
         `distance_function_name` to `jaccard` and
         `distance_threshold_or_thresholds = [0.9,0.7]` would be
+
         - Exact match
         - Jaccard distance <= 0.9
         - Jaccard distance <= 0.7
         - Anything else
 
+        Note: distance_function_at_thresholds() is primarily used in the
+        backend to create the out-of-the-box cl.XXX_at_thresholds() functions
+
         Args:
             col_name (str): The name of the column to compare
             distance_function_name (str): The name of the distance function.
             distance_threshold_or_thresholds (Union[int, list], optional): The
                 threshold(s) to use for the middle similarity level(s).
                 Defaults to [1, 2].
             higher_is_more_similar (bool): If True, a higher value of the distance
@@ -91,72 +106,83 @@
                 (e.g. levenshtein).
             include_exact_match_level (bool, optional): If True, include an exact match
                 level. Defaults to True.
             term_frequency_adjustments (bool, optional): If True, apply term frequency
                 adjustments to the exact match level. Defaults to False.
             m_probability_exact_match (_type_, optional): If provided, overrides the
                 default m probability for the exact match level. Defaults to None.
-            m_probability_or_probabilities_lev (Union[float, list], optional):
-                _description_. If provided, overrides the default m probabilities
+            m_probability_or_probabilities_thres (Union[float, list], optional):
+                If provided, overrides the default m probabilities
                 for the thresholds specified. Defaults to None.
             m_probability_else (_type_, optional): If provided, overrides the
                 default m probability for the 'anything else' level. Defaults to None.
 
+        Examples:
+            >>> # DuckDB Jaccard Comparison at thresholds 0.9 and 0.7
+            >>> import splink.duckdb.duckdb_comparison_library as cl
+            >>> cl.distance_function_at_thresholds("name",
+            >>>                    distance_function_name = 'jaccard',
+            >>>                    distance_threshold_or_thresholds = [0.9, 0.7]
+            >>>                    )
+
+            >>> # Spark Jaccard Comparison at thresholds 0.9 and 0.7
+            >>> import splink.spark.spark_comparison_library as cl
+            >>> cl.distance_function_at_thresholds("name",
+            >>>                    distance_function_name = 'jaccard',
+            >>>                    distance_threshold_or_thresholds = [0.9, 0.7]
+            >>>                    )
+
+
         Returns:
-            Comparison:
+            Comparison: A comparison for a chosen distance function similarity that
+                can be included in the Splink settings dictionary.
         """
+        # Validate user inputs
 
-        distance_thresholds = ensure_is_iterable(distance_threshold_or_thresholds)
-
-        if m_probability_or_probabilities_lev is None:
-            m_probability_or_probabilities_lev = [None] * len(distance_thresholds)
-        m_probabilities = ensure_is_iterable(m_probability_or_probabilities_lev)
+        distance_threshold_or_thresholds = ensure_is_iterable(
+            distance_threshold_or_thresholds
+        )
 
-        # Validate user inputs
-        comparison_at_thresholds_error_logger("distance_function", distance_thresholds)
+        comparison_at_thresholds_error_logger(
+            distance_function_name, distance_threshold_or_thresholds
+        )
 
         comparison_levels = []
         comparison_levels.append(self._null_level(col_name))
         if include_exact_match_level:
             level = self._exact_match_level(
                 col_name,
                 term_frequency_adjustments=term_frequency_adjustments,
                 m_probability=m_probability_exact_match,
             )
             comparison_levels.append(level)
 
-        for thres, m_prob in zip(distance_thresholds, m_probabilities):
-            # these function arguments hold for all cases.
-            kwargs = dict(
-                col_name=col_name,
-                distance_threshold=thres,
-                m_probability=m_prob,
-            )
-            # separate out the two that are only used
-            # when we have a user-supplied function, rather than a predefined subclass
-            # feels a bit hacky, but will do at least for time being
-            if not self._is_distance_subclass:
-                kwargs["distance_function_name"] = distance_function_name
-                kwargs["higher_is_more_similar"] = higher_is_more_similar
-            level = self._distance_level(**kwargs)
-            comparison_levels.append(level)
+        threshold_comparison_levels = distance_threshold_comparison_levels(
+            self,
+            col_name,
+            distance_function_name,
+            distance_threshold_or_thresholds,
+            m_probability_or_probabilities_thres,
+        )
+        comparison_levels = comparison_levels + threshold_comparison_levels
 
         comparison_levels.append(
             self._else_level(m_probability=m_probability_else),
         )
 
+        # Construct comparison description
         comparison_desc = ""
         if include_exact_match_level:
             comparison_desc += "Exact match vs. "
 
-        thres_desc = ", ".join([str(d) for d in distance_thresholds])
-        plural = "" if len(distance_thresholds) == 1 else "s"
-        comparison_desc += (
-            f"{distance_function_name} at threshold{plural} {thres_desc} vs. "
+        threshold_desc = distance_threshold_description(
+            col_name, distance_function_name, distance_threshold_or_thresholds
         )
+        comparison_desc += threshold_desc
+
         comparison_desc += "anything else"
 
         comparison_dict = {
             "comparison_description": comparison_desc,
             "comparison_levels": comparison_levels,
         }
         super().__init__(comparison_dict)
@@ -172,15 +198,15 @@
         col_name: str,
         distance_threshold_or_thresholds: int | list = [1, 2],
         include_exact_match_level=True,
         term_frequency_adjustments=False,
         m_probability_exact_match=None,
         m_probability_or_probabilities_lev: float | list = None,
         m_probability_else=None,
-    ):
+    ) -> Comparison:
         """A comparison of the data in `col_name` with the levenshtein distance used to
         assess middle similarity levels.
 
         An example of the output with default arguments and setting
         `distance_threshold_or_thresholds = [1,2]` would be
         - Exact match
         - levenshtein distance <= 1
@@ -195,21 +221,30 @@
             include_exact_match_level (bool, optional): If True, include an exact match
                 level. Defaults to True.
             term_frequency_adjustments (bool, optional): If True, apply term frequency
                 adjustments to the exact match level. Defaults to False.
             m_probability_exact_match (_type_, optional): If provided, overrides the
                 default m probability for the exact match level. Defaults to None.
             m_probability_or_probabilities_lev (Union[float, list], optional):
-                _description_. If provided, overrides the default m probabilities
+                If provided, overrides the default m probabilities
                 for the thresholds specified for given function. Defaults to None.
             m_probability_else (_type_, optional): If provided, overrides the
                 default m probability for the 'anything else' level. Defaults to None.
+        Examples:
+            >>> # DuckDB Levenshtein comparison at thresholds 1 and 2
+            >>> import splink.duckdb.duckdb_comparison_library as cl
+            >>> cl.levenshtein_at_thresholds("first_name", [1,2])
+
+            >>> # Spark Levenshtein comparison at thresholds 1 and 2
+            >>> import splink.spark.spark_comparison_library as cl
+            >>> cl.levenshtein_at_thresholds("first_name", [1,2])
 
         Returns:
-            Comparison:
+            Comparison: A comparison for Levenshtein similarity that can be included
+                in the Splink settings dictionary.
         """
 
         super().__init__(
             col_name,
             self._levenshtein_name,
             distance_threshold_or_thresholds,
             False,
@@ -229,22 +264,22 @@
     def __init__(
         self,
         col_name: str,
         distance_threshold_or_thresholds: int | list = [0.9, 0.7],
         include_exact_match_level=True,
         term_frequency_adjustments=False,
         m_probability_exact_match=None,
-        m_probability_or_probabilities_lev: float | list = None,
+        m_probability_or_probabilities_jac: float | list = None,
         m_probability_else=None,
-    ):
+    ) -> Comparison:
         """A comparison of the data in `col_name` with the jaccard distance used to
         assess middle similarity levels.
 
         An example of the output with default arguments and setting
-        `distance_threshold_or_thresholds = [1,2]` would be
+        `distance_threshold_or_thresholds = [0.9,0.7]` would be
         - Exact match
         - Jaccard distance <= 0.9
         - Jaccard distance <= 0.7
         - Anything else
 
         Args:
             col_name (str): The name of the column to compare
@@ -253,33 +288,111 @@
                 Defaults to [0.9, 0.7].
             include_exact_match_level (bool, optional): If True, include an exact match
                 level. Defaults to True.
             term_frequency_adjustments (bool, optional): If True, apply term frequency
                 adjustments to the exact match level. Defaults to False.
             m_probability_exact_match (_type_, optional): If provided, overrides the
                 default m probability for the exact match level. Defaults to None.
-            m_probability_or_probabilities_lev (Union[float, list], optional):
-                _description_. If provided, overrides the default m probabilities
+            m_probability_or_probabilities_jac (Union[float, list], optional):
+                If provided, overrides the default m probabilities
                 for the thresholds specified for given function. Defaults to None.
             m_probability_else (_type_, optional): If provided, overrides the
                 default m probability for the 'anything else' level. Defaults to None.
 
+        Examples:
+            >>> # DuckDB Jaccard comparison at thresholds 0.9 and 0.7
+            >>> import splink.duckdb.duckdb_comparison_library as cl
+            >>> cl.jaccard_at_thresholds("first_name", [0.9, 0.7])
+
+            >>> # Spark Jaccard comparison at thresholds 0.9 and 0.7
+            >>> import splink.spark.spark_comparison_library as cl
+            >>> cl.jaccard_at_thresholds("first_name", [0.9, 0.7])
+
         Returns:
-            Comparison:
+            Comparison: A comparison for Jaccard similarity that can be included
+                in the Splink settings dictionary.
         """
 
         super().__init__(
             col_name,
             self._jaccard_name,
             distance_threshold_or_thresholds,
             True,
             include_exact_match_level,
             term_frequency_adjustments,
             m_probability_exact_match,
-            m_probability_or_probabilities_lev,
+            m_probability_or_probabilities_jac,
+            m_probability_else,
+        )
+
+    @property
+    def _is_distance_subclass(self):
+        return True
+
+
+class JaroAtThresholdsComparisonBase(DistanceFunctionAtThresholdsComparisonBase):
+    def __init__(
+        self,
+        col_name: str,
+        distance_threshold_or_thresholds: int | list = [0.9, 0.7],
+        include_exact_match_level=True,
+        term_frequency_adjustments=False,
+        m_probability_exact_match=None,
+        m_probability_or_probabilities_jar: float | list = None,
+        m_probability_else=None,
+    ) -> Comparison:
+        """A comparison of the data in `col_name` with the jaro distance used to
+        assess middle similarity levels.
+
+        An example of the output with default arguments and setting
+        `distance_threshold_or_thresholds = [0.9, 0.7]` would be
+        - Exact match
+        - jaro distance <= 0.9
+        - jaro distance <= 0.7
+        - Anything else
+
+        Args:
+            col_name (str): The name of the column to compare
+            distance_threshold_or_thresholds (Union[int, list], optional): The
+                threshold(s) to use for the middle similarity level(s).
+                Defaults to [0.9, 0.7].
+            include_exact_match_level (bool, optional): If True, include an exact match
+                level. Defaults to True.
+            term_frequency_adjustments (bool, optional): If True, apply term frequency
+                adjustments to the exact match level. Defaults to False.
+            m_probability_exact_match (_type_, optional): If provided, overrides the
+                default m probability for the exact match level. Defaults to None.
+            m_probability_or_probabilities_jar (Union[float, list], optional):
+                If provided, overrides the default m probabilities
+                for the thresholds specified for given function. Defaults to None.
+            m_probability_else (_type_, optional): If provided, overrides the
+                default m probability for the 'anything else' level. Defaults to None.
+
+        Examples:
+            >>> # DuckDB Jaro comparison at thresholds 0.9 and 0.7
+            >>> import splink.duckdb.duckdb_comparison_library as cl
+            >>> cl.jaro_at_thresholds("first_name", [0.9, 0.7])
+
+            >>> # Spark Jaccard comparison at thresholds 0.9 and 0.7
+            >>> import splink.spark.spark_comparison_library as cl
+            >>> cl.jaro_at_thresholds("first_name", [0.9, 0.7])
+
+        Returns:
+            Comparison:
+        """
+
+        super().__init__(
+            col_name,
+            self._jaro_name,
+            distance_threshold_or_thresholds,
+            True,
+            include_exact_match_level,
+            term_frequency_adjustments,
+            m_probability_exact_match,
+            m_probability_or_probabilities_jar,
             m_probability_else,
         )
 
     @property
     def _is_distance_subclass(self):
         return True
 
@@ -288,22 +401,22 @@
     def __init__(
         self,
         col_name: str,
         distance_threshold_or_thresholds: int | list = [0.9, 0.7],
         include_exact_match_level=True,
         term_frequency_adjustments=False,
         m_probability_exact_match=None,
-        m_probability_or_probabilities_lev: float | list = None,
+        m_probability_or_probabilities_jw: float | list = None,
         m_probability_else=None,
-    ):
+    ) -> Comparison:
         """A comparison of the data in `col_name` with the jaro_winkler distance used to
         assess middle similarity levels.
 
         An example of the output with default arguments and setting
-        `distance_threshold_or_thresholds = [1,2]` would be
+        `distance_threshold_or_thresholds = [0.9, 0.7]` would be
         - Exact match
         - jaro_winkler distance <= 0.9
         - jaro_winkler distance <= 0.7
         - Anything else
 
         Args:
             col_name (str): The name of the column to compare
@@ -312,33 +425,43 @@
                 Defaults to [0.9, 0.7].
             include_exact_match_level (bool, optional): If True, include an exact match
                 level. Defaults to True.
             term_frequency_adjustments (bool, optional): If True, apply term frequency
                 adjustments to the exact match level. Defaults to False.
             m_probability_exact_match (_type_, optional): If provided, overrides the
                 default m probability for the exact match level. Defaults to None.
-            m_probability_or_probabilities_lev (Union[float, list], optional):
-                _description_. If provided, overrides the default m probabilities
+            m_probability_or_probabilities_jw (Union[float, list], optional):
+                If provided, overrides the default m probabilities
                 for the thresholds specified for given function. Defaults to None.
             m_probability_else (_type_, optional): If provided, overrides the
                 default m probability for the 'anything else' level. Defaults to None.
 
+        Examples:
+            >>> # DuckDB Jaro-winkler comparison at thresholds 0.9 and 0.7
+            >>> import splink.duckdb.duckdb_comparison_library as cl
+            >>> cl.jaro_winkler_at_thresholds("first_name", [0.9, 0.7])
+
+            >>> # Spark Jaro-winkler comparison at thresholds 0.9 and 0.7
+            >>> import splink.spark.saprk_comparison_library as cl
+            >>> cl.jaro_winkler_at_thresholds("first_name", [0.9, 0.7])
+
         Returns:
-            Comparison:
+            Comparison: A comparison for Jaro Winkler similarity that can be included
+                in the Splink settings dictionary.
         """
 
         super().__init__(
             col_name,
             self._jaro_winkler_name,
             distance_threshold_or_thresholds,
             True,
             include_exact_match_level,
             term_frequency_adjustments,
             m_probability_exact_match,
-            m_probability_or_probabilities_lev,
+            m_probability_or_probabilities_jw,
             m_probability_else,
         )
 
     @property
     def _is_distance_subclass(self):
         return True
 
@@ -346,15 +469,15 @@
 class ArrayIntersectAtSizesComparisonBase(Comparison):
     def __init__(
         self,
         col_name: str,
         size_or_sizes: int | list = [1],
         m_probability_or_probabilities_sizes: float | list = None,
         m_probability_else=None,
-    ):
+    ) -> Comparison:
         """A comparison of the data in array column `col_name` with various
         intersection sizes to assess similarity levels.
 
         An example of the output with default arguments and setting
         `size_or_sizes = [3, 1]` would be
         - Intersection has at least 3 elements
         - Intersection has at least 1 element (i.e. 1 or 2)
@@ -362,21 +485,31 @@
 
         Args:
             col_name (str): The name of the column to compare
             size_or_sizes (Union[int, list], optional): The size(s) of intersection
                 to use for the non-'else' similarity level(s). Should be in
                 descending order. Defaults to [1].
             m_probability_or_probabilities_sizes (Union[float, list], optional):
-                _description_. If provided, overrides the default m probabilities
+                If provided, overrides the default m probabilities
                 for the sizes specified. Defaults to None.
             m_probability_else (_type_, optional): If provided, overrides the
                 default m probability for the 'anything else' level. Defaults to None.
 
+        Examples:
+            >>> # DuckDB Array intersect comparison at sizes 3 and 1
+            >>> import splink.duckdb.duckdb_comparison_library as cl
+            >>> cl.array_intersect_at_sizes("first_name", [3, 1])
+
+            >>> # Spark Array intersect comparison at sizes 3 and 1
+            >>> import splink.spark.spark_comparison_library as cl
+            >>> cl.array_intersect_at_sizes("first_name", [3, 1])
+
         Returns:
-            Comparison:
+            Comparison: A comparison for the intersection of arrays that can be included
+                in the Splink settings dictionary.
         """
 
         sizes = ensure_is_iterable(size_or_sizes)
         if len(sizes) == 0:
             raise ValueError(
                 "`size_or_sizes` must have at least one element, so that Comparison "
                 "has more than just an 'else' level"
@@ -426,17 +559,19 @@
         self,
         col_name: str,
         date_thresholds: int | list = [1],
         date_metrics: str | list = ["year"],
         include_exact_match_level=True,
         term_frequency_adjustments=False,
         m_probability_exact_match=None,
-        m_probability_or_probabilities_sizes: float | list = None,
+        m_probability_or_probabilities_dat: float | list = None,
         m_probability_else=None,
-    ):
+        cast_strings_to_date=False,
+        date_format=None,
+    ) -> Comparison:
         """A comparison of the data in the date column `col_name` with various
         date thresholds and metrics to assess similarity levels.
 
         An example of the output with default arguments and settings
         `date_thresholds = [1]` and `date_metrics = ['day']` would be
         - The two input dates are within 1 day of one another
         - Anything else (i.e. all other dates lie outside this range)
@@ -461,35 +596,79 @@
                 Metrics should be one of `day`, `month` or `year`.
             include_exact_match_level (bool, optional): If True, include an exact match
                 level. Defaults to True.
             term_frequency_adjustments (bool, optional): If True, apply term frequency
                 adjustments to the exact match level. Defaults to False.
             m_probability_exact_match (_type_, optional): If provided, overrides the
                 default m probability for the exact match level. Defaults to None.
-            m_probability_or_probabilities_sizes (Union[float, list], optional):
-                _description_. If provided, overrides the default m probabilities
+            m_probability_or_probabilities_dat (Union[float, list], optional):
+                If provided, overrides the default m probabilities
                 for the sizes specified. Defaults to None.
             m_probability_else (_type_, optional): If provided, overrides the
                 default m probability for the 'anything else' level. Defaults to None.
+            cast_strings_to_date (bool, optional): Set to True to
+                enable date-casting when input dates are strings. Also adjust
+                date_format if date-strings are not in (yyyy-mm-dd) format.
+                Defaults to False.
+            date_format(str, optional): Format of input dates if date-strings
+                are given. Must be consistent across record pairs. If None
+                (the default), downstream functions for each backend assign
+                date_format to ISO 8601 format (yyyy-mm-dd).
+
+        Examples:
+            >>> # DuckDB Date Difference comparison at thresholds 10 days, 12 months
+            >>> # and 15 years
+            >>> import splink.duckdb.duckdb_comparison_library as cl
+            >>> cl.datediff_at_thresholds("date",
+            >>>                             date_thresholds = [10, 12, 15],
+            >>>                             date_metrics = ['day', 'month', 'year']
+            >>>                             )
+
+            >>> # Spark Date Difference comparison at thresholds 10 days, 12 months
+            >>> # and 15 years
+            >>> import splink.spark.spark_comparison_library as cl
+            >>> cl.datediff_at_thresholds("date",
+            >>>                             date_thresholds = [10, 12, 15],
+            >>>                             date_metrics = ['day', 'month', 'year']
+            >>>                             )
+
+            >>> # DuckDB datediff comparison with date-casting and unspecified
+            >>> # (default = %Y-%m-%d) date_format
+            >>> import splink.duckdb.duckdb_comparison_library as cl
+            >>> cl.datediff_at_thresholds("dob",
+                                            date_thresholds=[1,5],
+                                            date_metrics = ["day", "year"],
+                                            cast_strings_to_date=True
+                                            )
+
+            >>> # DuckDB datediff comparison with date-casting and specified
+            >>> # (non-default) date_format
+            >>> import splink.duckdb.duckdb_comparison_library as cl
+            >>> cl.datediff_at_thresholds("dob",
+                                            date_thresholds=[1,5],
+                                            date_metrics = ["day", "year"],
+                                            cast_strings_to_date=True,
+                                            date_format='%d/%m/%Y'
+                                            )
 
         Returns:
-            Comparison: A comparison that can be inclued in the Splink settings
-                dictionary.
+            Comparison: A comparison for Datediff that can be included in the Splink
+                settings dictionary.
         """
 
         thresholds = ensure_is_iterable(date_thresholds)
         metrics = ensure_is_iterable(date_metrics)
 
         # Validate user inputs
         comparison_at_thresholds_error_logger("datediff", date_thresholds)
         datediff_error_logger(thresholds, metrics)
 
-        if m_probability_or_probabilities_sizes is None:
-            m_probability_or_probabilities_sizes = [None] * len(thresholds)
-        m_probabilities = ensure_is_iterable(m_probability_or_probabilities_sizes)
+        if m_probability_or_probabilities_dat is None:
+            m_probability_or_probabilities_dat = [None] * len(thresholds)
+        m_probabilities = ensure_is_iterable(m_probability_or_probabilities_dat)
 
         comparison_levels = []
         comparison_levels.append(self._null_level(col_name))
         if include_exact_match_level:
             level = self._exact_match_level(
                 col_name,
                 term_frequency_adjustments=term_frequency_adjustments,
@@ -499,14 +678,16 @@
 
         for date_thres, date_metr, m_prob in zip(thresholds, metrics, m_probabilities):
             level = self._datediff_level(
                 col_name,
                 date_threshold=date_thres,
                 date_metric=date_metr,
                 m_probability=m_prob,
+                cast_strings_to_date=cast_strings_to_date,
+                date_format=date_format,
             )
             comparison_levels.append(level)
 
         comparison_levels.append(
             self._else_level(m_probability=m_probability_else),
         )
 
@@ -538,17 +719,17 @@
     def __init__(
         self,
         lat_col: str,
         long_col: str,
         km_thresholds: int | list = [0.1, 1],
         include_exact_match_level=False,
         m_probability_exact_match=None,
-        m_probability_or_probabilities_lev: float | list = None,
+        m_probability_or_probabilities_km: float | list = None,
         m_probability_else=None,
-    ):
+    ) -> Comparison:
         """A comparison of the coordinates defined in 'lat_col' and
         'long col' giving the haversine distance between them in km.
 
         An example of the output with default arguments and settings
         `km_thresholds = [1]` would be
         - The two coordinates within 1 km of one another
         - Anything else (i.e.  the distance between all coordinate lie outside
@@ -563,43 +744,57 @@
             km_thresholds (Union[int, list], optional): The size(s) of given date
                 thresholds, to assess whether two coordinates fall within a given
                 distance.
             include_exact_match_level (bool, optional): If True, include an exact match
                 level. Defaults to True.
             m_probability_exact_match (_type_, optional): If provided, overrides the
                 default m probability for the exact match level. Defaults to None.
-            m_probability_or_probabilities_lev (Union[float, list], optional):
-                _description_. If provided, overrides the default m probabilities
+            m_probability_or_probabilities_km (Union[float, list], optional):
+                If provided, overrides the default m probabilities
                 for the sizes specified. Defaults to None.
             m_probability_else (_type_, optional): If provided, overrides the
                 default m probability for the 'anything else' level. Defaults to None.
 
+        Examples:
+            >>> # DuckDB KM Distance comparison at thresholds 0.1, 1, 10 kilometres
+            >>> import splink.duckdb.duckdb_comparison_library as cl
+            >>> cl.datediff_at_thresholds("lat_col",
+            >>>                            "long_col",
+            >>>                            km_thresholds = [0.1, 1, 10]
+            >>>                            )
+
+            >>> # Spark KM Distance comparison at thresholds 0.1, 1, 10 kilometres
+            >>> import splink.spark.spark_comparison_library as cl
+            >>> cl.datediff_at_thresholds("lat_col",
+            >>>                            "long_col",
+            >>>                            km_thresholds = [0.1, 1, 10]
+            >>>                            )
+
         Returns:
-            Comparison: A comparison that can be inclued in the Splink settings
-                dictionary.
+            Comparison: A comparison for Distance in KM that can be included in the
+                Splink settings dictionary.
         """
 
         thresholds = ensure_is_iterable(km_thresholds)
 
-        if m_probability_or_probabilities_lev is None:
-            m_probability_or_probabilities_sizes = [None] * len(thresholds)
-        m_probabilities = ensure_is_iterable(m_probability_or_probabilities_sizes)
+        if m_probability_or_probabilities_km is None:
+            m_probability_or_probabilities_km = [None] * len(thresholds)
+        m_probabilities = ensure_is_iterable(m_probability_or_probabilities_km)
 
         comparison_levels = []
 
         null_level = {
             "sql_condition": f"({lat_col}_l IS NULL OR {lat_col}_r IS NULL) \n"
             f"OR ({long_col}_l IS NULL OR {long_col}_r IS NULL)",
             "label_for_charts": "Null",
             "is_null_level": True,
         }
         comparison_levels.append(null_level)
 
         if include_exact_match_level:
-
             label_suffix = f" {lat_col}, {long_col}"
             level = {
                 "sql_condition": f"({lat_col}_l = {lat_col}_r) \n"
                 f"AND ({long_col}_l = {long_col}_r)",
                 "label_for_charts": f"Exact match{label_suffix}",
             }
```

### Comparing `splink-3.7.3/splink/comparison_template_library.py` & `splink-3.8.0/splink/comparison_template_library.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,38 +3,46 @@
 # it simpler to use splink out-of-the-box
 
 from __future__ import annotations
 
 import logging
 
 from .comparison import Comparison  # change to self
-from .comparison_library_utils import datediff_error_logger
+from .comparison_library_utils import (
+    datediff_error_logger,
+    distance_threshold_comparison_levels,
+    distance_threshold_description,
+)
 from .misc import ensure_is_iterable
 
 logger = logging.getLogger(__name__)
 
 
 class DateComparisonBase(Comparison):
     def __init__(
         self,
-        col_name,
-        include_exact_match_level=True,
-        term_frequency_adjustments=False,
-        separate_1st_january=False,
-        levenshtein_thresholds=[1, 2],
-        jaro_winkler_thresholds=[],
+        col_name: str,
+        include_exact_match_level: bool = True,
+        term_frequency_adjustments: bool = False,
+        separate_1st_january: bool = False,
+        levenshtein_thresholds: int | list = [1, 2],
+        jaro_thresholds: int | list = [],
+        jaro_winkler_thresholds: int | list = [],
         datediff_thresholds: int | list = [1, 10],
         datediff_metrics: str | list = ["year", "year"],
-        m_probability_exact_match=None,
-        m_probability_1st_january=None,
+        m_probability_exact_match: float = None,
+        m_probability_1st_january: float = None,
         m_probability_or_probabilities_lev: float | list = None,
+        m_probability_or_probabilities_jar: float | list = None,
         m_probability_or_probabilities_jw: float | list = None,
         m_probability_or_probabilities_datediff: float | list = None,
-        m_probability_else=None,
-    ):
+        m_probability_else: float = None,
+        cast_strings_to_date: bool = False,
+        date_format: str = None,
+    ) -> Comparison:
         """A wrapper to generate a comparison for a date column the data in
         `col_name` with preselected defaults.
 
         The default arguments will give a comparison with comparison levels:\n
         - Exact match (1st of January only)\n
         - Exact match (all other dates)\n
         - Levenshtein distance <= 2\n
@@ -48,41 +56,85 @@
                 level. Defaults to True.
             term_frequency_adjustments (bool, optional): If True, apply term frequency
                 adjustments to the exact match level. Defaults to False.
             separate_1st_january (bool, optional): If True, include a separate
                 exact match comparison level when date is 1st January.
             levenshtein_thresholds (Union[int, list], optional): The thresholds to use
                 for levenshtein similarity level(s).
-                We recommend use of either levenshtein or jaro_winkler for fuzzy
-                matching, but not both.
+                We recommend using one of either levenshtein, jaro or jaro_winkler for
+                fuzzy matching, but not multiple.
                 Defaults to [2]
+            jaro_thresholds (Union[int, list], optional): The thresholds to use
+                for jaro similarity level(s).
+                We recommend using one of either levenshtein, jaro or jaro_winkler for
+                fuzzy matching, but not multiple.
+                Defaults to []
             jaro_winkler_thresholds (Union[int, list], optional): The thresholds to use
                 for jaro_winkler similarity level(s).
-                We recommend use of either levenshtein or jaro_winkler for fuzzy
-                matching, but not both.
+                We recommend using one of either levenshtein, jaro or jaro_winkler for
+                fuzzy matching, but not multiple.
                 Defaults to []
             datediff_thresholds (Union[int, list], optional): The thresholds to use
                 for datediff similarity level(s).
                 Defaults to [1, 1].
             datediff_metrics (Union[str, list], optional): The metrics to apply
                 thresholds to for datediff similarity level(s).
                 Defaults to ["month", "year"].
             m_probability_exact_match (_type_, optional): If provided, overrides the
                 default m probability for the exact match level. Defaults to None.
             m_probability_or_probabilities_lev (Union[float, list], optional):
-                _description_. If provided, overrides the default m probabilities
+                If provided, overrides the default m probabilities
                 for the levenshtein thresholds specified. Defaults to None.
+            m_probability_or_probabilities_jar (Union[float, list], optional):
+                If provided, overrides the default m probabilities
+                for the jaro thresholds specified. Defaults to None.
             m_probability_or_probabilities_jw (Union[float, list], optional):
-                _description_. If provided, overrides the default m probabilities
+                If provided, overrides the default m probabilities
                 for the jaro winkler thresholds specified. Defaults to None.
             m_probability_or_probabilities_datediff (Union[float, list], optional):
-                _description_. If provided, overrides the default m probabilities
+                If provided, overrides the default m probabilities
                 for the datediff thresholds specified. Defaults to None.
             m_probability_else (_type_, optional): If provided, overrides the
                 default m probability for the 'anything else' level. Defaults to None.
+            cast_strings_to_date (bool, optional): Set to True to
+                enable date-casting when input dates are strings. Also adjust
+                date_format if date-strings are not in (yyyy-mm-dd) format.
+                Defaults to False.
+            date_format(str, optional): Format of input dates if date-strings
+                are given. Must be consistent across record pairs. If None
+                (the default), downstream functions for each backend assign
+                date_format to ISO 8601 format (yyyy-mm-dd).
+
+
+        Examples:
+            >>> # DuckDB Basic Date Comparison
+            >>> import splink.duckdb.duckdb_comparison_template_library as ctl
+            >>> clt.date_comparison("date_of_birth")
+
+            >>> # DuckDB Bespoke Date Comparison
+            >>> import splink.duckdb.duckdb_comparison_template_library as ctl
+            >>> clt.date_comparison(
+            >>>                     "date_of_birth",
+            >>>                     levenshtein_thresholds=[],
+            >>>                     jaro_winkler_thresholds=[0.88],
+            >>>                     datediff_thresholds=[1, 1],
+            >>>                     datediff_metrics=["month", "year"])
+
+            >>> # Spark Basic Date Comparison
+            >>> import splink.spark.spark_comparison_template_library as ctl
+            >>> clt.date_comparison("date_of_birth")
+
+            >>> # Spark Bespoke Date Comparison
+            >>> import splink.spark.spark_comparison_template_library as ctl
+            >>> clt.date_comparison(
+            >>>                     "date_of_birth",
+            >>>                     levenshtein_thresholds=[],
+            >>>                     jaro_winkler_thresholds=[0.88],
+            >>>                     datediff_thresholds=[1, 1],
+            >>>                     datediff_metrics=["month", "year"])
 
         Returns:
             Comparison: A comparison that can be inclued in the Splink settings
                 dictionary.
         """
         # Construct Comparison
         comparison_levels = []
@@ -107,66 +159,62 @@
             comparison_level = self._exact_match_level(
                 col_name,
                 term_frequency_adjustments=term_frequency_adjustments,
                 m_probability=m_probability_exact_match,
             )
             comparison_levels.append(comparison_level)
 
+        levenshtein_thresholds = ensure_is_iterable(levenshtein_thresholds)
         if len(levenshtein_thresholds) > 0:
-            levenshtein_thresholds = ensure_is_iterable(levenshtein_thresholds)
-
-            if m_probability_or_probabilities_lev is None:
-                m_probability_or_probabilities_lev = [None] * len(
-                    levenshtein_thresholds
-                )
-            m_probability_or_probabilities_lev = ensure_is_iterable(
-                m_probability_or_probabilities_lev
+            threshold_comparison_levels = distance_threshold_comparison_levels(
+                self,
+                col_name,
+                "levenshtein",
+                levenshtein_thresholds,
+                m_probability_or_probabilities_lev,
+            )
+            comparison_levels = comparison_levels + threshold_comparison_levels
+
+        jaro_thresholds = ensure_is_iterable(jaro_thresholds)
+        if len(jaro_thresholds) > 0:
+            threshold_comparison_levels = distance_threshold_comparison_levels(
+                self,
+                col_name,
+                "jaro",
+                jaro_thresholds,
+                m_probability_or_probabilities_jar,
             )
+            comparison_levels = comparison_levels + threshold_comparison_levels
 
-            for thres, m_prob in zip(
-                levenshtein_thresholds, m_probability_or_probabilities_lev
-            ):
-                comparison_level = self._levenshtein_level(
-                    col_name,
-                    distance_threshold=thres,
-                    m_probability=m_prob,
-                )
-                comparison_levels.append(comparison_level)
-
+        jaro_winkler_thresholds = ensure_is_iterable(jaro_winkler_thresholds)
         if len(jaro_winkler_thresholds) > 0:
-            jaro_winkler_thresholds = ensure_is_iterable(jaro_winkler_thresholds)
-
-            if m_probability_or_probabilities_jw is None:
-                m_probability_or_probabilities_jw = [None] * len(
-                    jaro_winkler_thresholds
-                )
-            m_probability_or_probabilities_jw = ensure_is_iterable(
-                m_probability_or_probabilities_jw
-            )
-
-            for thres, m_prob in zip(
-                jaro_winkler_thresholds, m_probability_or_probabilities_jw
-            ):
-                comparison_level = self._jaro_winkler_level(
-                    col_name,
-                    distance_threshold=thres,
-                    m_probability=m_prob,
-                )
-                comparison_levels.append(comparison_level)
-
-        if len(levenshtein_thresholds) > 0 and len(jaro_winkler_thresholds) > 0:
+            threshold_comparison_levels = distance_threshold_comparison_levels(
+                self,
+                col_name,
+                "jaro-winkler",
+                jaro_winkler_thresholds,
+                m_probability_or_probabilities_jw,
+            )
+            comparison_levels = comparison_levels + threshold_comparison_levels
+
+        count_string_match_functions_used = (
+            (len(levenshtein_thresholds) > 0)
+            + (len(jaro_thresholds) > 0)
+            + (len(jaro_winkler_thresholds) > 0)
+        )
+        if count_string_match_functions_used > 1:
             logger.warning(
-                "You have included a comparison level for both Levenshtein and "
-                "Jaro-Winkler similarity. We recommend choosing one or the other."
+                "You have included a comparison level for more than one of "
+                "Levenshtein, Jaro and Jaro-Winkler similarity. We recommend "
+                "choosing one of the three."
             )
 
+        datediff_thresholds = ensure_is_iterable(datediff_thresholds)
+        datediff_metrics = ensure_is_iterable(datediff_metrics)
         if len(datediff_thresholds) > 0:
-            datediff_thresholds = ensure_is_iterable(datediff_thresholds)
-            datediff_metrics = ensure_is_iterable(datediff_metrics)
-
             if m_probability_or_probabilities_datediff is None:
                 m_probability_or_probabilities_datediff = [None] * len(
                     datediff_thresholds
                 )
             m_probability_or_probabilities_datediff = ensure_is_iterable(
                 m_probability_or_probabilities_datediff
             )
@@ -177,39 +225,43 @@
                 m_probability_or_probabilities_datediff,
             ):
                 comparison_level = self._datediff_level(
                     col_name,
                     date_threshold=thres,
                     date_metric=metric,
                     m_probability=m_prob,
+                    cast_strings_to_date=cast_strings_to_date,
+                    date_format=date_format,
                 )
                 comparison_levels.append(comparison_level)
 
             comparison_levels.append(
                 self._else_level(m_probability=m_probability_else),
             )
 
         # Construct Description
         comparison_desc = ""
         if include_exact_match_level:
             comparison_desc += "Exact match vs. "
 
         if len(levenshtein_thresholds) > 0:
-            lev_desc = ", ".join([str(d) for d in levenshtein_thresholds])
-            plural = "" if len(levenshtein_thresholds) == 1 else "s"
-            comparison_desc += (
-                f"Dates within levenshtein threshold{plural} {lev_desc} vs. "
+            desc = distance_threshold_description(
+                col_name, "levenshtein", levenshtein_thresholds
             )
+            comparison_desc += desc
+
+        if len(jaro_thresholds) > 0:
+            desc = distance_threshold_description(col_name, "jaro", jaro_thresholds)
+            comparison_desc += desc
 
         if len(jaro_winkler_thresholds) > 0:
-            lev_desc = ", ".join([str(d) for d in jaro_winkler_thresholds])
-            plural = "" if len(jaro_winkler_thresholds) == 1 else "s"
-            comparison_desc += (
-                f"Dates within jaro_winkler threshold{plural} {lev_desc} vs. "
+            desc = distance_threshold_description(
+                col_name, "jaro_winkler", jaro_winkler_thresholds
             )
+            comparison_desc += desc
 
         if len(datediff_thresholds) > 0:
             datediff_desc = ", ".join(
                 [
                     f"{m.title()}(s): {v}"
                     for v, m in zip(datediff_thresholds, datediff_metrics)
                 ]
@@ -223,33 +275,39 @@
 
         comparison_dict = {
             "comparison_description": comparison_desc,
             "comparison_levels": comparison_levels,
         }
         super().__init__(comparison_dict)
 
+    @property
+    def _is_distance_subclass(self):
+        return False
+
 
 class NameComparisonBase(Comparison):
     def __init__(
         self,
-        col_name,
-        include_exact_match_level=True,
-        phonetic_col_name=None,
-        term_frequency_adjustments_name=False,
-        term_frequency_adjustments_phonetic_name=False,
-        levenshtein_thresholds=[],
-        jaro_winkler_thresholds=[0.95, 0.88],
-        jaccard_thresholds=[],
-        m_probability_exact_match_name=None,
-        m_probability_exact_match_phonetic_name=None,
+        col_name: str,
+        include_exact_match_level: bool = True,
+        phonetic_col_name: str = None,
+        term_frequency_adjustments_name: bool = False,
+        term_frequency_adjustments_phonetic_name: bool = False,
+        levenshtein_thresholds: int | list = [],
+        jaro_thresholds: float | list = [],
+        jaro_winkler_thresholds: float | list = [0.95, 0.88],
+        jaccard_thresholds: float | list = [],
+        m_probability_exact_match_name: bool = None,
+        m_probability_exact_match_phonetic_name: bool = None,
         m_probability_or_probabilities_lev: float | list = None,
+        m_probability_or_probabilities_jar: float | list = None,
         m_probability_or_probabilities_jw: float | list = None,
         m_probability_or_probabilities_jac: float | list = None,
-        m_probability_else=None,
-    ):
+        m_probability_else: float = None,
+    ) -> Comparison:
         """A wrapper to generate a comparison for a name column the data in
         `col_name` with preselected defaults.
 
         The default arguments will give a comparison with comparison levels:\n
         - Exact match \n
         - Jaro Winkler similarity >= 0.95\n
         - Jaro Winkler similarity >= 0.88\n
@@ -270,39 +328,80 @@
             term_frequency_adjustments_phonetic_name (bool, optional): If True, apply
                 term frequency adjustments to the exact match level for
                 "phonetic_col_name".
                 Defaults to False.
             levenshtein_thresholds (Union[int, list], optional): The thresholds to use
                 for levenshtein similarity level(s).
                 Defaults to []
+            jaro_thresholds (Union[int, list], optional): The thresholds to use
+                for jaro similarity level(s).
+                We recommend using one of either levenshtein, jaro or jaro_winkler for
+                fuzzy matching, but not multiple.
+                Defaults to []
             jaro_winkler_thresholds (Union[int, list], optional): The thresholds to use
                 for jaro_winkler similarity level(s).
                 Defaults to [0.88]
             jaccard_thresholds (Union[int, list], optional): The thresholds to use
                 for jaccard similarity level(s).
                 Defaults to []
             m_probability_exact_match_name (_type_, optional): If provided, overrides
                 the default m probability for the exact match level for col_name.
                 Defaults to None.
             m_probability_exact_match_phonetic_name (_type_, optional): If provided,
                 overrides the default m probability for the exact match level for
                 phonetic_col_name. Defaults to None.
             m_probability_or_probabilities_lev (Union[float, list], optional):
-                _description_. If provided, overrides the default m probabilities
-                for the thresholds specified. Defaults to None.
-            m_probability_or_probabilities_datediff (Union[float, list], optional):
-                _description_. If provided, overrides the default m probabilities
+                If provided, overrides the default m probabilities
                 for the thresholds specified. Defaults to None.
+            m_probability_or_probabilities_jar (Union[float, list], optional):
+                If provided, overrides the default m probabilities
+                for the jaro thresholds specified. Defaults to None.
+            m_probability_or_probabilities_jw (Union[float, list], optional):
+                If provided, overrides the default m probabilities
+                for the jaro winkler thresholds specified. Defaults to None.
+            m_probability_or_probabilities_jac (Union[float, list], optional):
+                If provided, overrides the default m probabilities
+                for the jaccard thresholds specified. Defaults to None.
             m_probability_else (_type_, optional): If provided, overrides the
                 default m probability for the 'anything else' level. Defaults to None.
 
+        Examples:
+            >>> # DuckDB Basic Name Comparison
+            >>> import splink.duckdb.duckdb_comparison_template_library as ctl
+            >>> clt.name_comparison("name")
+
+            >>> # DuckDB Bespoke Name Comparison
+            >>> import splink.duckdb.duckdb_comparison_template_library as ctl
+            >>> clt.name_comparison("name",
+            >>>                     phonetic_col_name = "name_dm",
+            >>>                     term_frequency_adjustments_name = True,
+            >>>                     levenshtein_thresholds=[2],
+            >>>                     jaro_winkler_thresholds=[],
+            >>>                     jaccard_thresholds=[1]
+            >>>                     )
+
+            >>> # Spark Basic Name Comparison
+            >>> import splink.spark.spark_comparison_template_library as ctl
+            >>> clt.name_comparison("name")
+
+            >>> # Spark Bespoke Date Comparison
+            >>> import splink.spark.spark_comparison_template_library as ctl
+            >>> clt.name_comparison("name",
+            >>>                     phonetic_col_name = "name_dm",
+            >>>                     term_frequency_adjustments_name = True,
+            >>>                     levenshtein_thresholds=[2],
+            >>>                     jaro_winkler_thresholds=[],
+            >>>                     jaccard_thresholds=[1]
+            >>>                     )
+
         Returns:
             Comparison: A comparison that can be included in the Splink settings
                 dictionary.
         """
+
         # Construct Comparison
         comparison_levels = []
         comparison_levels.append(self._null_level(col_name))
 
         if include_exact_match_level:
             comparison_level = self._exact_match_level(
                 col_name,
@@ -317,106 +416,96 @@
                     phonetic_col_name,
                     term_frequency_adjustments=term_frequency_adjustments_phonetic_name,
                     m_probability=m_probability_exact_match_phonetic_name,
                     include_colname_in_charts_label=True,
                 )
                 comparison_levels.append(comparison_level)
 
+        levenshtein_thresholds = ensure_is_iterable(levenshtein_thresholds)
         if len(levenshtein_thresholds) > 0:
-            levenshtein_thresholds = ensure_is_iterable(levenshtein_thresholds)
-
-            if m_probability_or_probabilities_lev is None:
-                m_probability_or_probabilities_lev = [None] * len(
-                    levenshtein_thresholds
-                )
-            m_probability_or_probabilities_lev = ensure_is_iterable(
-                m_probability_or_probabilities_lev
+            threshold_comparison_levels = distance_threshold_comparison_levels(
+                self,
+                col_name,
+                "levenshtein",
+                levenshtein_thresholds,
+                m_probability_or_probabilities_lev,
+            )
+            comparison_levels = comparison_levels + threshold_comparison_levels
+
+        jaro_thresholds = ensure_is_iterable(jaro_thresholds)
+        if len(jaro_thresholds) > 0:
+            threshold_comparison_levels = distance_threshold_comparison_levels(
+                self,
+                col_name,
+                "jaro",
+                jaro_thresholds,
+                m_probability_or_probabilities_jar,
             )
+            comparison_levels = comparison_levels + threshold_comparison_levels
 
-            for thres, m_prob in zip(
-                levenshtein_thresholds, m_probability_or_probabilities_lev
-            ):
-                comparison_level = self._levenshtein_level(
-                    col_name,
-                    distance_threshold=thres,
-                    m_probability=m_prob,
-                )
-                comparison_levels.append(comparison_level)
-
+        jaro_winkler_thresholds = ensure_is_iterable(jaro_winkler_thresholds)
         if len(jaro_winkler_thresholds) > 0:
-            jaro_winkler_thresholds = ensure_is_iterable(jaro_winkler_thresholds)
-
-            if m_probability_or_probabilities_jw is None:
-                m_probability_or_probabilities_jw = [None] * len(
-                    jaro_winkler_thresholds
-                )
-            m_probability_or_probabilities_jw = ensure_is_iterable(
-                m_probability_or_probabilities_jw
+            threshold_comparison_levels = distance_threshold_comparison_levels(
+                self,
+                col_name,
+                "jaro-winkler",
+                jaro_winkler_thresholds,
+                m_probability_or_probabilities_jw,
             )
+            comparison_levels = comparison_levels + threshold_comparison_levels
 
-            for thres, m_prob in zip(
-                jaro_winkler_thresholds, m_probability_or_probabilities_jw
-            ):
-                comparison_level = self._jaro_winkler_level(
-                    col_name,
-                    distance_threshold=thres,
-                    m_probability=m_prob,
-                )
-                comparison_levels.append(comparison_level)
-
+        jaccard_thresholds = ensure_is_iterable(jaccard_thresholds)
         if len(jaccard_thresholds) > 0:
-            jaccard_thresholds = ensure_is_iterable(jaccard_thresholds)
-
-            if m_probability_or_probabilities_jac is None:
-                m_probability_or_probabilities_jac = [None] * len(jaccard_thresholds)
-            m_probability_or_probabilities_jac = ensure_is_iterable(
-                m_probability_or_probabilities_jac
+            threshold_comparison_levels = distance_threshold_comparison_levels(
+                self,
+                col_name,
+                "jaccard",
+                jaccard_thresholds,
+                m_probability_or_probabilities_jar,
             )
-
-            for thres, m_prob in zip(
-                jaccard_thresholds, m_probability_or_probabilities_jac
-            ):
-                comparison_level = self._jaccard_level(
-                    col_name,
-                    distance_threshold=thres,
-                    m_probability=m_prob,
-                )
-                comparison_levels.append(comparison_level)
+            comparison_levels = comparison_levels + threshold_comparison_levels
 
         comparison_levels.append(
             self._else_level(m_probability=m_probability_else),
         )
 
         # Construct Description
         comparison_desc = ""
         if include_exact_match_level:
             comparison_desc += "Exact match vs. "
 
         if phonetic_col_name is not None:
             comparison_desc += "Names with phonetic exact match vs. "
 
         if len(levenshtein_thresholds) > 0:
-            lev_desc = ", ".join([str(d) for d in levenshtein_thresholds])
-            plural = "" if len(levenshtein_thresholds) == 1 else "s"
-            comparison_desc += (
-                f"Dates within levenshtein threshold{plural} {lev_desc} vs. "
+            desc = distance_threshold_description(
+                col_name, "levenshtein", levenshtein_thresholds
             )
+            comparison_desc += desc
+
+        if len(jaro_thresholds) > 0:
+            desc = distance_threshold_description(col_name, "jaro", jaro_thresholds)
+            comparison_desc += desc
 
         if len(jaro_winkler_thresholds) > 0:
-            lev_desc = ", ".join([str(d) for d in jaro_winkler_thresholds])
-            plural = "" if len(jaro_winkler_thresholds) == 1 else "s"
-            comparison_desc += (
-                f"Names within jaro_winkler threshold{plural} {lev_desc} vs. "
+            desc = distance_threshold_description(
+                col_name, "jaro_winkler", jaro_winkler_thresholds
             )
+            comparison_desc += desc
 
         if len(jaccard_thresholds) > 0:
-            lev_desc = ", ".join([str(d) for d in jaccard_thresholds])
-            plural = "" if len(jaccard_thresholds) == 1 else "s"
-            comparison_desc += f"Names within jaccard threshold{plural} {lev_desc} vs. "
+            desc = distance_threshold_description(
+                col_name, "jaccard", jaccard_thresholds
+            )
+            comparison_desc += desc
 
         comparison_desc += "anything else"
 
         comparison_dict = {
             "comparison_description": comparison_desc,
             "comparison_levels": comparison_levels,
         }
         super().__init__(comparison_dict)
+
+    @property
+    def _is_distance_subclass(self):
+        return False
```

### Comparing `splink-3.7.3/splink/comparison_vector_distribution.py` & `splink-3.8.0/splink/comparison_vector_distribution.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 # https://stackoverflow.com/questions/39740632/python-type-hinting-without-cyclic-imports
 if TYPE_CHECKING:
-    from .linker import Linker
+    from ..linker import Linker
 
 
 def comparison_vector_distribution_sql(linker: Linker):
     gamma_columns = [c._gamma_column_name for c in linker._settings_obj.comparisons]
     groupby_cols = " , ".join(gamma_columns)
     gam_concat = " || ',' || ".join(gamma_columns)
```

### Comparing `splink-3.7.3/splink/comparison_vector_values.py` & `splink-3.8.0/splink/comparison_vector_values.py`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/connected_components.py` & `splink-3.8.0/splink/connected_components.py`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/convert_v2_to_v3.py` & `splink-3.8.0/splink/convert_v2_to_v3.py`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/databricks/enable_splink.py` & `splink-3.8.0/splink/databricks/enable_splink.py`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/default_from_jsonschema.py` & `splink-3.8.0/splink/default_from_jsonschema.py`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/dialect_base.py` & `splink-3.8.0/splink/dialect_base.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,13 +27,17 @@
         )
 
     @property
     def _levenshtein_name(self):
         return "levenshtein"
 
     @property
+    def _jaro_name(self):
+        return "jaro"
+
+    @property
     def _jaro_winkler_name(self):
         return "jaro_winkler"
 
     @property
     def _jaccard_name(self):
         return "jaccard"
```

### Comparing `splink-3.7.3/splink/duckdb/duckdb_comparison_level_library.py` & `splink-3.8.0/splink/duckdb/duckdb_comparison_level_library.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,24 +4,72 @@
     ColumnsReversedLevelBase,
     DateDiffLevelBase,
     DistanceFunctionLevelBase,
     DistanceInKMLevelBase,
     ElseLevelBase,
     ExactMatchLevelBase,
     JaccardLevelBase,
+    JaroLevelBase,
     JaroWinklerLevelBase,
     LevenshteinLevelBase,
     NullLevelBase,
     PercentageDifferenceLevelBase,
 )
 from .duckdb_base import (
     DuckDBBase,
 )
 
 
+# Class used to feed our comparison_library classes
+class DuckDBComparisonProperties(DuckDBBase):
+    @property
+    def _exact_match_level(self):
+        return exact_match_level
+
+    @property
+    def _null_level(self):
+        return null_level
+
+    @property
+    def _else_level(self):
+        return else_level
+
+    @property
+    def _datediff_level(self):
+        return datediff_level
+
+    @property
+    def _array_intersect_level(self):
+        return array_intersect_level
+
+    @property
+    def _distance_in_km_level(self):
+        return distance_in_km_level
+
+    @property
+    def _distance_function_level(self):
+        return distance_function_level
+
+    @property
+    def _levenshtein_level(self):
+        return levenshtein_level
+
+    @property
+    def _jaro_level(self):
+        return jaro_level
+
+    @property
+    def _jaro_winkler_level(self):
+        return jaro_winkler_level
+
+    @property
+    def _jaccard_level(self):
+        return jaccard_level
+
+
 class null_level(DuckDBBase, NullLevelBase):
     pass
 
 
 class exact_match_level(DuckDBBase, ExactMatchLevelBase):
     pass
 
@@ -38,14 +86,18 @@
     pass
 
 
 class levenshtein_level(DuckDBBase, LevenshteinLevelBase):
     pass
 
 
+class jaro_level(DuckDBBase, JaroLevelBase):
+    pass
+
+
 class jaro_winkler_level(DuckDBBase, JaroWinklerLevelBase):
     pass
 
 
 class jaccard_level(DuckDBBase, JaccardLevelBase):
     pass
```

### Comparing `splink-3.7.3/splink/duckdb/duckdb_helpers.py` & `splink-3.8.0/splink/duckdb/duckdb_helpers.py`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/duckdb/duckdb_linker.py` & `splink-3.8.0/splink/duckdb/duckdb_linker.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,17 +5,15 @@
 
 import duckdb
 import pandas as pd
 from duckdb import DuckDBPyConnection
 
 from ..input_column import InputColumn
 from ..linker import Linker
-from ..logging_messages import execute_sql_logging_message_info, log_sql
 from ..misc import (
-    all_letter_combos,
     ensure_is_list,
 )
 from ..splink_dataframe import SplinkDataFrame
 from .duckdb_helpers import (
     create_temporary_duckdb_connection,
     duckdb_load_from_file,
     validate_duckdb_connection,
@@ -114,49 +112,48 @@
             con = duckdb.connect(database=connection)
 
         self._con = con
 
         # If user has provided pandas dataframes, need to register
         # them with the database, using user-provided aliases
         # if provided or a created alias if not
-
         input_tables = ensure_is_list(input_table_or_tables)
+        input_tables = [
+            duckdb_load_from_file(t) if isinstance(t, str) else t for t in input_tables
+        ]
 
         input_aliases = self._ensure_aliases_populated_and_is_list(
             input_table_or_tables, input_table_aliases
         )
 
-        # 'homogenised' means all entries are strings representing tables
-        homogenised_tables = []
-        homogenised_aliases = []
-
-        default_aliases = all_letter_combos(len(input_tables))
-
-        for table, alias, default_alias in zip(
-            input_tables, input_aliases, default_aliases
-        ):
-            if type(alias).__name__ in ["DataFrame", "Table"]:
-                alias = f"_{default_alias}"
-
-            if type(table).__name__ in ["DataFrame", "Table"]:
-                con.register(alias, table)
-                if isinstance(table, pd.DataFrame):
-                    self._check_cast_error(alias)
-                table = alias
-
-            homogenised_tables.append(duckdb_load_from_file(table))
-            homogenised_aliases.append(alias)
+        accepted_df_dtypes = [pd.DataFrame]
+        try:
+            # If pyarrow is installed, add to the accepted list
+            import pyarrow as pa
+
+            accepted_df_dtypes.append(pa.lib.Table)
+        except ImportError:
+            pass
 
         super().__init__(
-            homogenised_tables,
+            input_tables,
             settings_dict,
+            accepted_df_dtypes,
             set_up_basic_logging,
-            input_table_aliases=homogenised_aliases,
+            input_table_aliases=input_aliases,
         )
 
+        # Quickly check for casting error in duckdb/pandas
+        for i, (table, alias) in enumerate(zip(input_tables, input_aliases)):
+            if isinstance(table, pd.DataFrame):
+                if isinstance(alias, pd.DataFrame):
+                    alias = f"__splink__input_table_{i}"
+
+                self._check_cast_error(alias)
+
         if output_schema:
             self._con.execute(
                 f"""
                     CREATE SCHEMA IF NOT EXISTS {output_schema};
                     SET schema '{output_schema}';
                 """
             )
@@ -167,26 +164,26 @@
         return DuckDBLinkerDataFrame(templated_name, physical_name, self)
 
     def _execute_sql_against_backend(self, sql, templated_name, physical_name):
         # In the case of a table already existing in the database,
         # execute sql is only reached if the user has explicitly turned off the cache
         self._delete_table_from_database(physical_name)
 
-        logger.debug(execute_sql_logging_message_info(templated_name, physical_name))
-        logger.log(5, log_sql(sql))
-
         sql = f"""
         CREATE TABLE {physical_name}
         AS
         ({sql})
         """
-        self._con.execute(sql)
+        self._log_and_run_sql_execution(sql, templated_name, physical_name)
 
         return DuckDBLinkerDataFrame(templated_name, physical_name, self)
 
+    def _run_sql_execution(self, final_sql, templated_name, physical_name):
+        self._con.execute(final_sql)
+
     def register_table(self, input, table_name, overwrite=False):
         # If the user has provided a table name, return it as a SplinkDataframe
         if isinstance(input, str):
             return self._table_to_splink_dataframe(table_name, input)
 
         # Check if table name is already in use
         exists = self._table_exists_in_database(table_name)
@@ -205,19 +202,22 @@
             input = pd.DataFrame.from_records(input)
 
         # Registration errors will automatically
         # occur if an invalid data type is passed as an argument
         self._con.register(table_name, input)
         return self._table_to_splink_dataframe(table_name, table_name)
 
-    def _random_sample_sql(self, proportion, sample_size):
+    def _random_sample_sql(self, proportion, sample_size, seed=None):
         if proportion == 1.0:
             return ""
         percent = proportion * 100
-        return f"USING SAMPLE {percent}% (bernoulli)"
+        if seed:
+            return f"USING SAMPLE bernoulli({percent}%) REPEATABLE({seed})"
+        else:
+            return f"USING SAMPLE {percent}% (bernoulli)"
 
     @property
     def _infinity_expression(self):
         return "cast('infinity' as double)"
 
     def _table_exists_in_database(self, table_name):
         sql = f"PRAGMA table_info('{table_name}');"
```

### Comparing `splink-3.7.3/splink/em_training_session.py` & `splink-3.8.0/splink/em_training_session.py`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/estimate_u.py` & `splink-3.8.0/splink/estimate_u.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     # p(r) = r(r-1)/2, where r is input rows
     # Solve this for r
     # https://www.wolframalpha.com/input?i=Solve%5Bp%3Dr+*+%28r+-+1%29+%2F+2%2C+r%5D
     sample_rows = 0.5 * ((8 * n_pairs + 1) ** 0.5 + 1)
     return sample_rows
 
 
-def estimate_u_values(linker: Linker, max_pairs):
+def estimate_u_values(linker: Linker, max_pairs, seed=None):
     logger.info("----- Estimating u probabilities using random sampling -----")
 
     nodes_with_tf = linker._initialise_df_concat_with_tf()
 
     original_settings_obj = linker._settings_obj
 
     training_linker = deepcopy(linker)
@@ -89,15 +89,15 @@
 
     if sample_size > count_rows:
         sample_size = count_rows
 
     sql = f"""
     select *
     from __splink__df_concat_with_tf
-    {training_linker._random_sample_sql(proportion, sample_size)}
+    {training_linker._random_sample_sql(proportion, sample_size, seed)}
     """
     training_linker._enqueue_sql(sql, "__splink__df_concat_with_tf_sample")
     df_sample = training_linker._execute_sql_pipeline([nodes_with_tf])
 
     settings_obj._blocking_rules_to_generate_predictions = []
 
     sql = block_using_rules_sql(training_linker)
```

### Comparing `splink-3.7.3/splink/expectation_maximisation.py` & `splink-3.8.0/splink/expectation_maximisation.py`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/files/chart_defs/blocking_rule_generated_comparisons.json` & `splink-3.8.0/splink/files/chart_defs/blocking_rule_generated_comparisons.json`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/files/chart_defs/completeness.json` & `splink-3.8.0/splink/files/chart_defs/completeness.json`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/files/chart_defs/del/bayes_factor_history_chart_def.json` & `splink-3.8.0/splink/files/chart_defs/del/bayes_factor_history_chart_def.json`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/files/chart_defs/del/bayes_factor_intuition_chart_def.json` & `splink-3.8.0/splink/files/chart_defs/del/bayes_factor_intuition_chart_def.json`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/files/chart_defs/del/compare_estimates.json` & `splink-3.8.0/splink/files/chart_defs/del/compare_estimates.json`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/files/chart_defs/del/gamma_distribution_chart_def.json` & `splink-3.8.0/splink/files/chart_defs/del/gamma_distribution_chart_def.json`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/files/chart_defs/del/gamma_histogram.json` & `splink-3.8.0/splink/files/chart_defs/del/gamma_histogram.json`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/files/chart_defs/del/score_histogram.json` & `splink-3.8.0/splink/files/chart_defs/del/score_histogram.json`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/files/chart_defs/m_u_parameters_interactive_history.json` & `splink-3.8.0/splink/files/chart_defs/m_u_parameters_interactive_history.json`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/files/chart_defs/match_weight_histogram.json` & `splink-3.8.0/splink/files/chart_defs/match_weight_histogram.json`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/files/chart_defs/match_weights_interactive_history.json` & `splink-3.8.0/splink/files/chart_defs/match_weights_interactive_history.json`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/files/chart_defs/match_weights_waterfall.json` & `splink-3.8.0/splink/files/chart_defs/match_weights_waterfall.json`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/files/chart_defs/missingness.json` & `splink-3.8.0/splink/files/chart_defs/missingness.json`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/files/chart_defs/parameter_estimate_comparisons.json` & `splink-3.8.0/splink/files/chart_defs/parameter_estimate_comparisons.json`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/files/chart_defs/probability_two_random_records_match_iteration.json` & `splink-3.8.0/splink/files/chart_defs/probability_two_random_records_match_iteration.json`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/files/chart_defs/profile_data.json` & `splink-3.8.0/splink/files/chart_defs/profile_data.json`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/files/chart_defs/roc.json` & `splink-3.8.0/splink/files/chart_defs/precision_recall.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5547762784090909%*

 * *Differences: {"'encoding'": "{'tooltip': {2: {'field': 'fp_rate', 'title': 'FP_rate'}, 3: {'field': 'tp_rate', "*

 * *               "'title': 'TP_rate'}, 4: {'field': 'tp', 'title': 'TP'}, 5: {'field': 'tn', "*

 * *               "'title': 'TN'}, 6: {'field': 'fp', 'title': 'FP'}, 7: {'field': 'fn', 'title': "*

 * *               "'FN'}, 10: {'field': 'f1', 'title': 'F1'}}, 'x': {'field': 'recall', 'sort': "*

 * *               "['-recall'], 'title': 'Recall'}, 'y': {'field': 'precision', 'sort': "*

 * *               "['-precision'], 'title': […]*

```diff
@@ -16,87 +16,83 @@
             },
             {
                 "field": "match_probability",
                 "format": ".4%",
                 "type": "quantitative"
             },
             {
-                "field": "FP_rate",
+                "field": "fp_rate",
                 "format": ".4f",
+                "title": "FP_rate",
                 "type": "quantitative"
             },
             {
-                "field": "TP_rate",
+                "field": "tp_rate",
                 "format": ".4f",
+                "title": "TP_rate",
                 "type": "quantitative"
             },
             {
-                "field": "TP",
+                "field": "tp",
                 "format": ",.0f",
+                "title": "TP",
                 "type": "quantitative"
             },
             {
-                "field": "TN",
+                "field": "tn",
                 "format": ",.0f",
+                "title": "TN",
                 "type": "quantitative"
             },
             {
-                "field": "FP",
+                "field": "fp",
                 "format": ",.0f",
+                "title": "FP",
                 "type": "quantitative"
             },
             {
-                "field": "FN",
+                "field": "fn",
                 "format": ",.0f",
+                "title": "FN",
                 "type": "quantitative"
             },
             {
                 "field": "precision",
                 "format": ".4f",
                 "type": "quantitative"
             },
             {
                 "field": "recall",
                 "format": ".4f",
                 "type": "quantitative"
             },
             {
-                "field": "F1",
+                "field": "f1",
                 "format": ".4f",
+                "title": "F1",
                 "type": "quantitative"
             }
         ],
         "x": {
-            "field": "FP_rate",
+            "field": "recall",
             "sort": [
-                "truth_threshold"
+                "-recall"
             ],
-            "title": "False Positive Rate amongst clerically reviewed records",
+            "title": "Recall",
             "type": "quantitative"
         },
         "y": {
-            "field": "TP_rate",
+            "field": "precision",
             "sort": [
-                "truth_threshold"
+                "-precision"
             ],
-            "title": "True Positive Rate amongst clerically reviewed records",
+            "title": "Precision",
             "type": "quantitative"
         }
     },
-    "height": 600,
     "mark": {
         "clip": true,
         "point": true,
         "type": "line"
     },
-    "selection": {
-        "selector076": {
-            "bind": "scales",
-            "encodings": [
-                "x"
-            ],
-            "type": "interval"
-        }
-    },
-    "title": "Receiver operating characteristic curve",
-    "width": 600
+    "title": "Precision-recall curve"
 }
```

### Comparing `splink-3.7.3/splink/files/chart_defs/unlinkables_chart_def.json` & `splink-3.8.0/splink/files/chart_defs/unlinkables_chart_def.json`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/files/external_js/vega-embed@6.20.2` & `splink-3.8.0/splink/files/external_js/vega-embed@6.20.2`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/files/external_js/vega-lite@5.2.0` & `splink-3.8.0/splink/files/external_js/vega-lite@5.2.0`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/files/external_js/vega@5.21.0` & `splink-3.8.0/splink/files/external_js/vega@5.21.0`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/files/settings_jsonschema.json` & `splink-3.8.0/splink/files/settings_jsonschema.json`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/files/spark_jars/scala-udf-similarity-0.1.0_classic.jar` & `splink-3.8.0/splink/files/spark_jars/scala-udf-similarity-0.1.0_classic.jar`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/files/spark_jars/scala-udf-similarity-0.1.0_spark3.3.jar` & `splink-3.8.0/splink/files/spark_jars/scala-udf-similarity-0.1.0_spark3.3.jar`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/files/splink_cluster_studio/cluster_template.j2` & `splink-3.8.0/splink/files/splink_cluster_studio/cluster_template.j2`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/files/splink_cluster_studio/custom.css` & `splink-3.8.0/splink/files/splink_cluster_studio/custom.css`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/files/splink_comparison_viewer/custom.css` & `splink-3.8.0/splink/files/splink_comparison_viewer/custom.css`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/files/splink_comparison_viewer/template.j2` & `splink-3.8.0/splink/files/splink_comparison_viewer/template.j2`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/files/splink_vis_utils/splink_vis_utils.js` & `splink-3.8.0/splink/files/splink_vis_utils/splink_vis_utils.js`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/input_column.py` & `splink-3.8.0/splink/input_column.py`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/linker.py` & `splink-3.8.0/splink/linker.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,29 +33,39 @@
     roc_chart,
     unlinkables_chart,
     waterfall_chart,
 )
 from .cluster_studio import render_splink_cluster_studio_html
 from .comparison import Comparison
 from .comparison_level import ComparisonLevel
-from .comparison_vector_distribution import comparison_vector_distribution_sql
+from .comparison_vector_distribution import (
+    comparison_vector_distribution_sql,
+)
 from .comparison_vector_values import compute_comparison_vector_values_sql
 from .connected_components import (
     _cc_create_unique_id_cols,
     solve_connected_components,
 )
 from .em_training_session import EMTrainingSession
 from .estimate_u import estimate_u_values
+from .exceptions import SplinkException
+from .logging_messages import execute_sql_logging_message_info, log_sql
 from .m_from_labels import estimate_m_from_pairwise_labels
 from .m_training import estimate_m_values_from_label_column
 from .match_key_analysis import (
     count_num_comparisons_from_blocking_rules_for_prediction_sql,
 )
 from .match_weights_histogram import histogram_data
-from .misc import ascii_uid, bayes_factor_to_prob, ensure_is_list, prob_to_bayes_factor
+from .misc import (
+    ascii_uid,
+    bayes_factor_to_prob,
+    ensure_is_list,
+    ensure_is_tuple,
+    prob_to_bayes_factor,
+)
 from .missingness import completeness_data, missingness_data
 from .pipeline import SQLPipeline
 from .predict import predict_from_comparison_vectors_sqls
 from .profile_data import profile_columns
 from .settings import Settings
 from .splink_comparison_viewer import (
     comparison_viewer_table_sqls,
@@ -118,14 +128,15 @@
     a `DuckDBLinker`.
     """
 
     def __init__(
         self,
         input_table_or_tables: str | list,
         settings_dict: dict,
+        accepted_df_dtypes,
         set_up_basic_logging: bool = True,
         input_table_aliases: str | list = None,
     ):
         """Initialise the linker object, which manages the data linkage process and
         holds the data linkage model.
 
         Examples:
@@ -166,31 +177,38 @@
                 format="%(message)s",
             )
             splink_logger = logging.getLogger("splink")
             splink_logger.setLevel(logging.INFO)
 
         self._pipeline = SQLPipeline()
 
-        self._input_tables_dict = self._get_input_tables_dict(
-            input_table_or_tables, input_table_aliases
-        )
+        self._names_of_tables_created_by_splink: set = set()
+        self._intermediate_table_cache: dict = CacheDictWithLogging()
 
         if not isinstance(settings_dict, (dict, type(None))):
+            # Run if you've entered a filepath
             self._setup_settings_objs(None)  # feed it a blank settings dictionary
             self.load_settings(settings_dict)
         else:
             settings_dict = deepcopy(settings_dict)
             self._setup_settings_objs(settings_dict)
 
+        homogenised_tables, homogenised_aliases = self._register_input_tables(
+            input_table_or_tables,
+            input_table_aliases,
+            accepted_df_dtypes,
+        )
+
+        self._input_tables_dict = self._get_input_tables_dict(
+            homogenised_tables, homogenised_aliases
+        )
+
         self._validate_input_dfs()
         self._em_training_sessions = []
 
-        self._names_of_tables_created_by_splink: set = set()
-        self._intermediate_table_cache: dict = CacheDictWithLogging()
-
         self._find_new_matches_mode = False
         self._train_u_using_random_sample_mode = False
         self._compare_two_records_mode = False
         self._self_link_mode = False
         self._analyse_blocking_mode = False
 
         self.debug_mode = False
@@ -260,14 +278,30 @@
             return "__splink__df_concat"
 
         if self._two_dataset_link_only:
             return "__splink_df_concat_with_tf_right"
         return "__splink__df_concat_with_tf"
 
     @property
+    def _source_dataset_column_name(self):
+        if self._settings_obj_ is None:
+            return None
+
+        # Used throughout the scripts to feed our SQL
+        if self._settings_obj._source_dataset_column_name_is_required:
+            df_obj = next(iter(self._input_tables_dict.values()))
+            columns = df_obj.columns_escaped
+
+            input_column = self._settings_obj._source_dataset_input_column
+            src_ds_col = InputColumn(input_column, self).name()
+            return "__splink_source_dataset" if src_ds_col in columns else input_column
+        else:
+            return None
+
+    @property
     def _two_dataset_link_only(self):
         # Two dataset link only join is a special case where an inner join of the
         # two datasets is much more efficient than self-joining the vertically
         # concatenation of all input datasets
         if self._find_new_matches_mode:
             return True
 
@@ -302,14 +336,33 @@
 
     @property
     def _infinity_expression(self):
         raise NotImplementedError(
             f"infinity sql expression not available for {type(self)}"
         )
 
+    def _register_input_tables(self, input_tables, input_aliases, accepted_df_dtypes):
+        # 'homogenised' means all entries are strings representing tables
+        homogenised_tables = []
+        homogenised_aliases = []
+        accepted_df_dtypes = ensure_is_tuple(accepted_df_dtypes)
+
+        for i, (table, alias) in enumerate(zip(input_tables, input_aliases)):
+            if isinstance(alias, accepted_df_dtypes):
+                alias = f"__splink__input_table_{i}"
+
+            if isinstance(table, accepted_df_dtypes):
+                self.register_table(table, alias)
+                table = alias
+
+            homogenised_tables.append(table)
+            homogenised_aliases.append(alias)
+
+        return homogenised_tables, homogenised_aliases
+
     def _setup_settings_objs(self, settings_dict):
         # Setup the linker class's required settings
         self._settings_dict = settings_dict
 
         # if settings_dict is passed, set sql_dialect on it if missing, and make sure
         # incompatible dialect not passed
         if settings_dict is not None and settings_dict.get("sql_dialect", None) is None:
@@ -453,19 +506,56 @@
                     output_tablename,
                     materialise_as_hash=False,
                     use_cache=False,
                 )
             self._pipeline.reset()
             return dataframe
 
-    def _execute_sql_against_backend(self, sql, templated_name, physical_name):
+    def _execute_sql_against_backend(
+        self, sql: str, templated_name: str, physical_name: str
+    ) -> SplinkDataFrame:
+        """Execute a single sql SELECT statement, returning a SplinkDataFrame.
+
+        Subclasses should implement this, using _log_and_run_sql_execution() within
+        their implementation, maybe doing some SQL translation or other prep/cleanup
+        work before/after.
+        """
         raise NotImplementedError(
             f"_execute_sql_against_backend not implemented for {type(self)}"
         )
 
+    def _run_sql_execution(
+        self, final_sql: str, templated_name: str, physical_name: str
+    ) -> SplinkDataFrame:
+        """**Actually** execute the sql against the backend database.
+
+        This is intended to be implemented by a subclass, but not actually called
+        directly. Instead, call _log_and_run_sql_execution, and that will call
+        this method.
+
+        This could return something, or not. It's up to the Linker subclass to decide.
+        """
+        raise NotImplementedError(
+            f"_run_sql_execution not implemented for {type(self)}"
+        )
+
+    def _log_and_run_sql_execution(
+        self, final_sql: str, templated_name: str, physical_name: str
+    ) -> SplinkDataFrame:
+        """Log the sql, then call _run_sql_execution(), wrapping any errors"""
+        logger.debug(execute_sql_logging_message_info(templated_name, physical_name))
+        logger.log(5, log_sql(final_sql))
+        try:
+            return self._run_sql_execution(final_sql, templated_name, physical_name)
+        except Exception as e:
+            raise SplinkException(
+                f"Error executing the following sql for table "
+                f"`{templated_name}`({physical_name}):\n{final_sql}"
+            ) from e
+
     def register_table(self, input, table_name, overwrite=False):
         """
         Register a table to your backend database, to be used in one of the
         splink methods, or simply to allow querying.
 
         Tables can be of type: dictionary, record level dictionary,
         pandas dataframe, pyarrow table and in the spark case, a spark df.
@@ -649,14 +739,19 @@
 
     def _table_exists_in_database(self, table_name):
         raise NotImplementedError(
             f"table_exists_in_database not implemented for {type(self)}"
         )
 
     def _validate_input_dfs(self):
+        if not hasattr(self, "_input_tables_dict"):
+            # This is only triggered where a user loads a settings dict from a
+            # given file path.
+            return
+
         for df in self._input_tables_dict.values():
             df.validate()
 
         if self._settings_obj_ is not None:
             if self._settings_obj._link_type == "dedupe_only":
                 if len(self._input_tables_dict) > 1:
                     raise ValueError(
@@ -829,16 +924,30 @@
             if not p.is_file():  # check if it's a valid file/filepath
                 raise ValueError(
                     "The filepath you have provided is either not a valid file "
                     "or doesn't exist along the path provided."
                 )
             settings_dict = json.loads(p.read_text())
 
+        # Store the cache ID so it can be reloaded after cache invalidation
+        cache_id = self._cache_uid
+        # So we don't run into any issues with generated tables having
+        # invalid columns as settings have been tweaked, invalidate
+        # the cache and allow these tables to be recomputed.
+
+        # This is less efficient, but triggers infrequently and ensures we don't
+        # run into issues where the defaults used conflict with the actual values
+        # supplied in settings.
+
+        # This is particularly relevant with `source_dataset`, which appears within
+        # concat_with_tf.
+        self.invalidate_cache()
+
         # If a uid already exists in your settings object, prioritise this
-        settings_dict["linker_uid"] = settings_dict.get("linker_uid", self._cache_uid)
+        settings_dict["linker_uid"] = settings_dict.get("linker_uid", cache_id)
         settings_dict["sql_dialect"] = settings_dict.get(
             "sql_dialect", self._sql_dialect
         )
         self._settings_dict = settings_dict
         self._settings_obj_ = Settings(settings_dict)
         self._validate_input_dfs()
         self._validate_dialect()
@@ -996,34 +1105,41 @@
         """
         concat_with_tf = self._initialise_df_concat_with_tf()
         sql = block_using_rules_sql(self)
         self._enqueue_sql(sql, "__splink__df_blocked")
         return self._execute_sql_pipeline([concat_with_tf])
 
     def estimate_u_using_random_sampling(
-        self, max_pairs: int = None, *, target_rows=None
+        self, max_pairs: int = None, seed: int = None, *, target_rows=None
     ):
         """Estimate the u parameters of the linkage model using random sampling.
 
         The u parameters represent the proportion of record comparisons that fall
         into each comparison level amongst truly non-matching records.
 
         This procedure takes a sample of the data and generates the cartesian
         product of pairwise record comparisons amongst the sampled records.
         The validity of the u values rests on the assumption that the resultant
         pairwise comparisons are non-matches (or at least, they are very unlikely to be
         matches). For large datasets, this is typically true.
 
+        The results of estimate_u_using_random_sampling, and therefore an entire splink
+        model, can be made reproducible by setting the seed parameter. Setting the seed
+        will have performance implications as additional processing is required.
+
         Args:
             max_pairs (int): The maximum number of pairwise record comparisons to
             sample. Larger will give more accurate estimates
             but lead to longer runtimes.  In our experience at least 1e9 (one billion)
             gives best results but can take a long time to compute. 1e7 (ten million)
             is often adequate whilst testing different model specifications, before
             the final model is estimated.
+            seed (int): Seed for random sampling. Assign to get reproducible u
+            probabilities. Note, seed for random sampling is only supported for
+            DuckDB and Spark, for Athena and SQLite set to None.
 
         Examples:
             >>> linker.estimate_u_using_random_sampling(1e8)
 
         Returns:
             None: Updates the estimated u parameters within the linker object
             and returns nothing.
@@ -1043,15 +1159,15 @@
                 DeprecationWarning,
                 stacklevel=2,
             )
             max_pairs = target_rows
         else:
             raise TypeError("Missing argument max_pairs")
 
-        estimate_u_values(self, max_pairs)
+        estimate_u_values(self, max_pairs, seed)
         self._populate_m_u_from_trained_values()
 
         self._settings_obj._columns_without_estimated_parameters_message()
 
     def estimate_m_from_label_column(self, label_colname: str):
         """Estimate the m parameters of the linkage model from a label (ground truth)
         column in the input dataframe(s).
@@ -2236,15 +2352,15 @@
             >>>
             >>> # View resultant html file in Jupyter (or just load it in your browser)
             >>> from IPython.display import IFrame
             >>> IFrame(src="./test_chart.html", width=1000, height=500
 
         """
         records = missingness_data(self, input_dataset)
-        return missingness_chart(records, input_dataset)
+        return missingness_chart(records)
 
     def completeness_chart(self, input_dataset: str = None, cols: list[str] = None):
         """Generate a summary chart of the completeness (proportion of non-nulls) of
         columns in each of the input datasets. By default, completeness is assessed for
         all column in the input data.
 
         Args:
@@ -2264,15 +2380,15 @@
             >>>
             >>> # View resultant html file in Jupyter (or just load it in your browser)
             >>> from IPython.display import IFrame
             >>> IFrame(src="./test_chart.html", width=1000, height=500
 
         """
         records = completeness_data(self, input_dataset, cols)
-        return completeness_chart(records, input_dataset)
+        return completeness_chart(records)
 
     def count_num_comparisons_from_blocking_rule(
         self,
         blocking_rule: str,
     ) -> int:
         """Compute the number of pairwise record comparisons that would be generated by
         a blocking rule
```

### Comparing `splink-3.7.3/splink/lower_id_on_lhs.py` & `splink-3.8.0/splink/lower_id_on_lhs.py`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/m_from_labels.py` & `splink-3.8.0/splink/m_from_labels.py`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/m_training.py` & `splink-3.8.0/splink/m_training.py`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/m_u_records_to_parameters.py` & `splink-3.8.0/splink/m_u_records_to_parameters.py`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/match_key_analysis.py` & `splink-3.8.0/splink/match_key_analysis.py`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/match_weights_histogram.py` & `splink-3.8.0/splink/match_weights_histogram.py`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/misc.py` & `splink-3.8.0/splink/misc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import itertools
 import json
 import random
 import string
 from math import inf, log2
 from typing import Iterable
 
 import numpy as np
@@ -44,14 +43,23 @@
     return a if isinstance(a, Iterable) else [a]
 
 
 def ensure_is_list(a):
     return a if isinstance(a, list) else [a]
 
 
+def ensure_is_tuple(a):
+    if isinstance(a, tuple):
+        return a
+    elif isinstance(a, list):
+        return tuple(a)
+    else:
+        return (a,)
+
+
 def join_list_with_commas_final_and(lst):
     if len(lst) == 1:
         return lst[0]
     return ", ".join(lst[:-1]) + " and " + lst[-1]
 
 
 class EverythingEncoder(json.JSONEncoder):
@@ -77,25 +85,14 @@
             return obj.tolist()
         try:
             return json.JSONEncoder.default(self, obj)
         except TypeError:
             return obj.__str__()
 
 
-def all_letter_combos(n):
-    """a,b,....,z,aa,ab,...,aaa"""
-
-    combos = []
-    for size in itertools.count(1):
-        for s in itertools.product(string.ascii_lowercase, repeat=size):
-            combos.append("".join(s))
-            if len(combos) >= n:
-                return combos
-
-
 def calculate_cartesian(df_rows, link_type):
     """
     Calculates the cartesian product for the input df(s).
     """
     n = df_rows
 
     if link_type == "link_only":
```

### Comparing `splink-3.7.3/splink/missingness.py` & `splink-3.8.0/splink/missingness.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     if input_tablename is None:
         df_concat = linker._initialise_df_concat(materialise=True)
         input_tablename = df_concat.physical_name
 
     columns = linker._settings_obj._columns_used_by_comparisons
 
     if linker._settings_obj._source_dataset_column_name_is_required:
-        source_name = linker._settings_obj._source_dataset_column_name
+        source_name = linker._source_dataset_column_name
     else:
         # Set source dataset to a literal string if dedupe_only
         source_name = "'_a'"
 
     for col in columns:
         sql = f"""
         (select
```

### Comparing `splink-3.7.3/splink/parse_sql.py` & `splink-3.8.0/splink/parse_sql.py`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/pipeline.py` & `splink-3.8.0/splink/pipeline.py`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/predict.py` & `splink-3.8.0/splink/predict.py`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/profile_data.py` & `splink-3.8.0/splink/profile_data.py`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/settings.py` & `splink-3.8.0/splink/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,28 +149,28 @@
     def _source_dataset_column_name_is_required(self):
         return self._link_type not in [
             "dedupe_only",
             "link_only_find_matches_to_new_records",
         ]
 
     @property
-    def _source_dataset_column_name(self):
+    def _source_dataset_input_column(self):
         if self._source_dataset_column_name_is_required:
             s_else_d = self._from_settings_dict_else_default
             return s_else_d("source_dataset_column_name")
         else:
             return None
 
     @property
     def _unique_id_input_columns(self) -> list[InputColumn]:
         cols = []
 
         if self._source_dataset_column_name_is_required:
             col = InputColumn(
-                self._source_dataset_column_name,
+                self._source_dataset_input_column,
                 settings_obj=self,
             )
             cols.append(col)
 
         col = InputColumn(self._unique_id_column_name, settings_obj=self)
         cols.append(col)
 
@@ -194,15 +194,15 @@
 
         return len(self._blocking_rules_to_generate_predictions) > 1
 
     @property
     def _columns_used_by_comparisons(self):
         cols_used = []
         if self._source_dataset_column_name_is_required:
-            cols_used.append(self._source_dataset_column_name)
+            cols_used.append(self._source_dataset_input_column)
         cols_used.append(self._unique_id_column_name)
         for cc in self.comparisons:
             cols = cc._input_columns_used_by_case_statement
             cols = [c.name() for c in cols]
 
             cols_used.extend(cols)
         return dedupe_preserving_order(cols_used)
@@ -424,15 +424,15 @@
 
     def _as_completed_dict(self):
         rr_match = self._probability_two_random_records_match
         current_settings = {
             "comparisons": [cc._as_completed_dict() for cc in self.comparisons],
             "probability_two_random_records_match": rr_match,
             "unique_id_column_name": self._unique_id_column_name,
-            "source_dataset_column_name": self._source_dataset_column_name,
+            "source_dataset_column_name": self._source_dataset_input_column,
         }
         return {**self._settings_dict, **current_settings}
 
     def match_weights_chart(self, as_dict=False):
         records = self._parameters_as_detailed_records
 
         return match_weights_chart(records, as_dict=as_dict)
```

### Comparing `splink-3.7.3/splink/spark/custom_spark_dialect.py` & `splink-3.8.0/splink/spark/custom_spark_dialect.py`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/spark/spark_base.py` & `splink-3.8.0/splink/duckdb/duckdb_base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,57 @@
 from ..dialect_base import (
     DialectBase,
 )
 
 
 def size_array_intersect_sql(col_name_l, col_name_r):
-    return f"size(array_intersect({col_name_l}, {col_name_r}))"
+    # sum of individual (unique) array sizes, minus the (unique) union
+    return (
+        f"list_unique({col_name_l}) + list_unique({col_name_r})"
+        f" - list_unique(list_concat({col_name_l}, {col_name_r}))"
+    )
+
+
+def datediff_sql(
+    col_name_l,
+    col_name_r,
+    date_threshold,
+    date_metric,
+    cast_str=False,
+    date_format=None,
+):
+    if date_format is None:
+        date_format = "%Y-%m-%d"
+
+    if cast_str:
+        return f"""
+            abs(date_diff('{date_metric}',strptime({col_name_l},
+              '{date_format}'),strptime({col_name_r},
+              '{date_format}'))) <= {date_threshold}
+        """
+    else:
+        return f"""
+            abs(date_diff('{date_metric}', {col_name_l},
+              {col_name_r})) <= {date_threshold}
+        """
 
 
-def datediff_sql(col_name_l, col_name_r, date_threshold, date_metric):
-    if date_metric == "day":
-        date_f = f"abs(datediff({col_name_l}, {col_name_r}))"
-    elif date_metric in ["month", "year"]:
-        date_f = f"ceil(abs(months_between({col_name_l}, {col_name_r})"
-        if date_metric == "year":
-            date_f += " / 12))"
-        else:
-            date_f += "))"
-
-    return f"""
-        {date_f} <= {date_threshold}
-    """
-
-
-class SparkBase(DialectBase):
+class DuckDBBase(DialectBase):
     @property
     def _sql_dialect(self):
-        return "spark"
+        return "duckdb"
+
+    @property
+    def _size_array_intersect_function(self):
+        return size_array_intersect_sql
 
     @property
     def _datediff_function(self):
         return datediff_sql
 
     @property
-    def _size_array_intersect_function(self):
-        return size_array_intersect_sql
+    def _jaro_name(self):
+        return "jaro_similarity"
+
+    @property
+    def _jaro_winkler_name(self):
+        return "jaro_winkler_similarity"
```

### Comparing `splink-3.7.3/splink/spark/spark_linker.py` & `splink-3.8.0/splink/spark/spark_linker.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from pyspark.sql.dataframe import DataFrame as spark_df
 from pyspark.sql.types import DoubleType, StringType
 from pyspark.sql.utils import AnalysisException
 
 from ..databricks.enable_splink import enable_splink
 from ..input_column import InputColumn
 from ..linker import Linker
-from ..logging_messages import execute_sql_logging_message_info, log_sql
 from ..misc import ensure_is_list, major_minor_version_greater_equal_than
 from ..splink_dataframe import SplinkDataFrame
 from ..term_frequencies import colname_to_tf_tablename
 from .custom_spark_dialect import Dialect
 
 logger = logging.getLogger(__name__)
 
@@ -120,14 +119,16 @@
 
         input_tables = ensure_is_list(input_table_or_tables)
 
         input_aliases = self._ensure_aliases_populated_and_is_list(
             input_table_or_tables, input_table_aliases
         )
 
+        accepted_df_dtypes = (pd.DataFrame, spark_df)
+
         self._get_spark_from_input_tables_if_not_provided(spark, input_tables)
 
         if num_partitions_on_repartition is None:
             parallelism_value = 200
             try:
                 parallelism_value = self.spark.conf.get("spark.default.parallelism")
                 parallelism_value = int(parallelism_value)
@@ -145,34 +146,22 @@
         else:
             self.num_partitions_on_repartition = num_partitions_on_repartition
 
         self._set_catalog_and_database_if_not_provided(catalog, database)
 
         self._drop_splink_cached_tables()
 
-        homogenised_tables = []
-        homogenised_aliases = []
-
-        for i, (table, alias) in enumerate(zip(input_tables, input_aliases)):
-            if type(alias).__name__ == "DataFrame":
-                alias = f"__splink__input_table_{i}"
-
-            if type(table).__name__ == "DataFrame":
-                self.register_table(table, alias)
-                table = alias
-
-            homogenised_tables.append(table)
-            homogenised_aliases.append(alias)
-
         super().__init__(
-            homogenised_tables,
+            input_tables,
             settings_dict,
+            accepted_df_dtypes,
             set_up_basic_logging,
-            input_table_aliases=homogenised_aliases,
+            input_table_aliases=input_aliases,
         )
+        self._check_ansi_enabled_if_converting_dates()
 
         self.in_databricks = "DATABRICKS_RUNTIME_VERSION" in os.environ
         if self.in_databricks:
             enable_splink(spark)
 
         self._set_default_break_lineage_method()
 
@@ -255,14 +244,15 @@
             self.break_lineage_method = "parquet"
 
     def _register_udfs_from_jar(self):
         # register udf functions
         # will for loop through this list to register UDFs.
         # List is a tuple of structure (UDF Name, class path, spark return type)
         udfs_register = [
+            ("jaro_sim", "uk.gov.moj.dash.linkage.JaroSimilarity", DoubleType()),
             (
                 "jaro_winkler",
                 "uk.gov.moj.dash.linkage.JaroWinklerSimilarity",
                 DoubleType(),
             ),
             ("jaccard", "uk.gov.moj.dash.linkage.JaccardSimilarity", DoubleType()),
             ("cosine_distance", "uk.gov.moj.dash.linkage.CosineDistance", DoubleType()),
@@ -389,30 +379,29 @@
                 raise ValueError(
                     f"Unknown break_lineage_method: {self.break_lineage_method}"
                 )
         return spark_df
 
     def _execute_sql_against_backend(self, sql, templated_name, physical_name):
         sql = sqlglot.transpile(sql, read="spark", write="customspark", pretty=True)[0]
-
-        logger.debug(execute_sql_logging_message_info(templated_name, physical_name))
-        logger.log(5, log_sql(sql))
-        spark_df = self.spark.sql(sql)
-
+        spark_df = self._log_and_run_sql_execution(sql, templated_name, physical_name)
         spark_df = self._break_lineage_and_repartition(
             spark_df, templated_name, physical_name
         )
 
         # After blocking, want to repartition
         # if templated
         spark_df.createOrReplaceTempView(physical_name)
 
         output_df = self._table_to_splink_dataframe(templated_name, physical_name)
         return output_df
 
+    def _run_sql_execution(self, final_sql, templated_name, physical_name):
+        return self.spark.sql(final_sql)
+
     @property
     def _infinity_expression(self):
         return "'infinity'"
 
     def register_table(self, input, table_name, overwrite=False):
         """
         Register a table to your backend database, to be used in one of the
@@ -459,19 +448,22 @@
             input = self.spark.createDataFrame(input)
         elif isinstance(input, pd.DataFrame):
             input = self.spark.createDataFrame(input)
 
         input.createOrReplaceTempView(table_name)
         return self._table_to_splink_dataframe(table_name, table_name)
 
-    def _random_sample_sql(self, proportion, sample_size):
+    def _random_sample_sql(self, proportion, sample_size, seed=None):
         if proportion == 1.0:
             return ""
         percent = proportion * 100
-        return f" TABLESAMPLE ({percent} PERCENT) "
+        if seed:
+            return f" ORDER BY rand({seed}) LIMIT {round(sample_size)}"
+        else:
+            return f" TABLESAMPLE ({percent} PERCENT) "
 
     def _table_exists_in_database(self, table_name):
         query_result = self.spark.sql(
             f"show tables from {self.splink_data_store} like '{table_name}'"
         ).collect()
         if len(query_result) > 1:
             # this clause accounts for temp tables which can have the same name as
@@ -489,7 +481,37 @@
         elif len(query_result) == 1:
             return True
         elif len(query_result) == 0:
             return False
 
     def register_tf_table(self, df, col_name, overwrite=False):
         self.register_table(df, colname_to_tf_tablename(col_name), overwrite)
+
+    def _check_ansi_enabled_if_converting_dates(self):
+        # because have this code in the init- need to first check if settings dict exits
+        try:
+            comparisons_as_list = self._settings_obj._settings_dict["comparisons"]
+            settings_obj = True
+        except ValueError:
+            settings_obj = False
+
+        if settings_obj is True:
+            # see if any of the comparisons contain 'to_timestamp',
+            #  the spark SQL used to convert date to str if date-to-str cast is used
+            if any(
+                [
+                    "to_timestamp" in str(comparisons_as_list[x].values())
+                    for x in range(0, len(comparisons_as_list))
+                ]
+            ):
+                # now check if ansi is enabled:
+                bool_ansi = self.spark.sparkContext.getConf().get(
+                    "spark.sql.ansi.enabled"
+                )
+                if bool_ansi == "False" or bool_ansi is None:
+                    logger.warning(
+                        """--WARN-- \n You are using datediff comparison
+                        with str-casting and ANSI is not enabled. Bad dates
+                        e.g. 1999-13-54 will not trigger an exception but will
+                        classed as comparison level = "ELSE". Ensure date strings
+                        are cleaned to remove bad dates \n"""
+                    )
```

### Comparing `splink-3.7.3/splink/splink_comparison_viewer.py` & `splink-3.8.0/splink/splink_comparison_viewer.py`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/splink_dataframe.py` & `splink-3.8.0/splink/splink_dataframe.py`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/sql_transform.py` & `splink-3.8.0/splink/sql_transform.py`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/sqlite/sqlite_linker.py` & `splink-3.8.0/splink/sqlite/sqlite_linker.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import logging
 from math import log2, pow
 
 import pandas as pd
 
 from ..input_column import InputColumn
 from ..linker import Linker
-from ..logging_messages import execute_sql_logging_message_info, log_sql
+from ..misc import ensure_is_list
 from ..splink_dataframe import SplinkDataFrame
 
 logger = logging.getLogger(__name__)
 
 
 def dict_factory(cursor, row):
     d = {}
@@ -90,42 +90,51 @@
         self._sql_dialect_ = "sqlite"
 
         self.con = connection
         self.con.row_factory = dict_factory
         self.con.create_function("log2", 1, log2)
         self.con.create_function("pow", 2, pow)
 
+        input_tables = ensure_is_list(input_table_or_tables)
+        input_aliases = self._ensure_aliases_populated_and_is_list(
+            input_table_or_tables, input_table_aliases
+        )
+        accepted_df_dtypes = pd.DataFrame
+
         super().__init__(
-            input_table_or_tables,
+            input_tables,
             settings_dict,
+            accepted_df_dtypes,
             set_up_basic_logging,
-            input_table_aliases=input_table_aliases,
+            input_table_aliases=input_aliases,
         )
 
     def _table_to_splink_dataframe(self, templated_name, physical_name):
         return SQLiteDataFrame(templated_name, physical_name, self)
 
     def _execute_sql_against_backend(self, sql, templated_name, physical_name):
         # In the case of a table already existing in the database,
         # execute sql is only reached if the user has explicitly turned off the cache
         self._delete_table_from_database(physical_name)
 
-        logger.debug(execute_sql_logging_message_info(templated_name, physical_name))
-        logger.log(5, log_sql(sql))
-
         sql = f"""
         create table {physical_name}
         as
         {sql}
         """
-        self.con.execute(sql)
+        self._log_and_run_sql_execution(sql, templated_name, physical_name)
 
         output_obj = self._table_to_splink_dataframe(templated_name, physical_name)
         return output_obj
 
+    def _run_sql_execution(
+        self, final_sql: str, templated_name: str, physical_name: str
+    ) -> SplinkDataFrame:
+        return self.con.execute(final_sql)
+
     def register_table(self, input, table_name, overwrite=False):
         # If the user has provided a table name, return it as a SplinkDataframe
         if isinstance(input, str):
             return self._table_to_splink_dataframe(table_name, input)
 
         # Check if table name is already in use
         exists = self._table_exists_in_database(table_name)
@@ -143,20 +152,24 @@
         elif isinstance(input, list):
             input = pd.DataFrame.from_records(input)
 
         # Will error if an invalid data type is passed
         input.to_sql(table_name, self.con, index=False)
         return self._table_to_splink_dataframe(table_name, table_name)
 
-    def _random_sample_sql(self, proportion, sample_size):
+    def _random_sample_sql(self, proportion, sample_size, seed=None):
         if proportion == 1.0:
             return ""
+        if seed:
+            raise NotImplementedError(
+                "SQLite does not support seeds in random ",
+                "samples. Please remove the `seed` parameter.",
+            )
 
         sample_size = int(sample_size)
-
         return (
             "where unique_id IN (SELECT unique_id FROM __splink__df_concat_with_tf"
             f" ORDER BY RANDOM() LIMIT {sample_size})"
         )
 
     @property
     def _infinity_expression(self):
```

### Comparing `splink-3.7.3/splink/term_frequencies.py` & `splink-3.8.0/splink/term_frequencies.py`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/unique_id_concat.py` & `splink-3.8.0/splink/unique_id_concat.py`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/unlinkables.py` & `splink-3.8.0/splink/unlinkables.py`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/validate_jsonschema.py` & `splink-3.8.0/splink/validate_jsonschema.py`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/splink/vertically_concatenate.py` & `splink-3.8.0/splink/vertically_concatenate.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,16 +47,18 @@
         salt_sql = ", random() as __splink_salt"
     else:
         salt_sql = ""
 
     if source_dataset_col_req:
         sqls_to_union = []
         for df_obj in linker._input_tables_dict.values():
+            source_ds_col = linker._source_dataset_column_name
             sql = f"""
-            select '{df_obj.templated_name}' as source_dataset, {select_columns_sql}
+            select '{df_obj.templated_name}' as {source_ds_col},
+            {select_columns_sql}
             {salt_sql}
             from {df_obj.physical_name}
             """
             sqls_to_union.append(sql)
         sql = " UNION ALL ".join(sqls_to_union)
     else:
         sql = f"""
```

### Comparing `splink-3.7.3/splink/waterfall_chart.py` & `splink-3.8.0/splink/waterfall_chart.py`

 * *Files identical despite different names*

### Comparing `splink-3.7.3/PKG-INFO` & `splink-3.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splink
-Version: 3.7.3
+Version: 3.8.0
 Summary: Fast probabilistic data linkage at scale
 Home-page: https://github.com/moj-analytical-services/splink
 License: MIT
 Author: Robin Linacre
 Author-email: robinlinacre@hotmail.com
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
@@ -33,19 +33,19 @@
 
 # Fast, accurate and scalable probabilistic data linkage
 
 Splink is a Python package for probabilistic record linkage (entity resolution) that allows you to deduplicate and link records from datasets without unique identifiers.
 
 ## Key Features
 
-- **Speed:** Capable of linking a million records on a laptop in approximately one minute.
-- **Accuracy:** Full support for term frequency adjustments and user-defined fuzzy matching logic.
-- **Scalability:** Execute linkage jobs in Python (using DuckDB) or big-data backends like AWS Athena or Spark for 100+ million records.
-- **Unsupervised Learning:** No training data is required, as models can be trained using an unsupervised approach.
-- **Interactive Outputs:** Provides a wide range of interactive outputs to help users understand their model and diagnose linkage problems.
+⚡ **Speed:** Capable of linking a million records on a laptop in approximately one minute.  
+🎯 **Accuracy:** Full support for term frequency adjustments and user-defined fuzzy matching logic.  
+🌐 **Scalability:** Execute linkage jobs in Python (using DuckDB) or big-data backends like AWS Athena or Spark for 100+ million records.  
+🎓 **Unsupervised Learning:** No training data is required, as models can be trained using an unsupervised approach.  
+📊 **Interactive Outputs:** Provides a wide range of interactive outputs to help users understand their model and diagnose linkage problems.
 
 Splink's core linkage algorithm is based on Fellegi-Sunter's model of record linkage, with various customizations to improve accuracy.
 
 ## What does Splink do?
 
 Consider the following records that lack a unique person identifier:
```

