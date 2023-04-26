# Comparing `tmp/alchemite_apiclient-0.53.0.tar.gz` & `tmp/alchemite_apiclient-0.54.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alchemite_apiclient-0.53.0.tar", last modified: Wed Mar 29 09:15:51 2023, max compression
+gzip compressed data, was "alchemite_apiclient-0.54.0.tar", last modified: Wed Apr 26 09:34:19 2023, max compression
```

## Comparing `alchemite_apiclient-0.53.0.tar` & `alchemite_apiclient-0.54.0.tar`

### file list

```diff
@@ -1,582 +1,582 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-29 09:15:51.137527 alchemite_apiclient-0.53.0/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       61 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)       25 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4935 2023-03-29 09:15:51.137527 alchemite_apiclient-0.53.0/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4232 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-29 09:15:51.061527 alchemite_apiclient-0.53.0/alchemite_apiclient/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    22492 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-29 09:15:51.061527 alchemite_apiclient-0.53.0/alchemite_apiclient/api/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      224 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/api/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)   112942 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/api/datasets_api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    35604 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/api/default_api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5200 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/api/metrics_api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    58362 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/api/model_dataset_api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)   233750 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/api/models_api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    37770 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/api_client.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-29 09:15:51.065527 alchemite_apiclient-0.53.0/alchemite_apiclient/apis/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      721 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/apis/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    17318 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/configuration.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5079 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/exceptions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13896 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/extensions.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-29 09:15:51.097527 alchemite_apiclient-0.53.0/alchemite_apiclient/model/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      348 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14502 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/additive_sensitivity_request.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15940 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/analyse_validate_request.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12717 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/analyse_validate_request_all_of.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    24816 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/analyse_validate_response.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14439 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/analyse_validate_response_column_analytics.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12124 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/categorical_column.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15273 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/categorical_column_info.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11771 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/categorical_column_info_all_of.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14958 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/categorical_column_info_stats.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    17661 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/categorical_model_column_info.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13506 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/categorical_model_column_info_all_of.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11411 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/categorical_prediction.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11432 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/categorical_result.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11554 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/column_group_batch_request.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11738 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/column_group_patch_request.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11605 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/column_group_request.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13897 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/column_group_response.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11120 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/column_group_response_all_of.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16155 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/column_info.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11587 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/column_value.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11749 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/column_value_nullable.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15595 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/continuous_column_info.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11760 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/continuous_column_info_all_of.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15093 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/continuous_column_info_stats.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16839 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/continuous_model_column_info.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12255 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/continuous_model_column_info_all_of.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11280 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/data.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    27957 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/dataset.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11519 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/dataset1.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12344 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/dataset_chunk.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14079 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/dataset_or_data.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11454 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/dataset_patch.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14432 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/dataset_query_request.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12022 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/dataset_query_request_row_ids.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11619 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/dataset_query_request_sort.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11888 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/dataset_query_response.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11530 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/dataset_query_response_result.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14166 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/dependent_col_fn_arg_col.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14730 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/dependent_col_fn_arg_col_weights.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14585 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/dependent_col_fn_arg_constant_sum.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14493 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/dependent_col_fn_arg_product.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14338 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/dependent_col_fn_arg_ratio.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15173 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/dependent_col_fn_arg_summands_weights.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14716 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/dependent_col_fn_arg_weighted_const_sum.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14627 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/dependent_col_fn_arg_weighted_ratio.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14486 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/dependent_col_fn_arg_zero_if_zero.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11971 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/dependent_col_fn_arg_zero_if_zero_all_of.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12802 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/dependent_columns.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12505 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/dimensionality_reduction_request.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12947 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/dimensionality_reduction_response.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12516 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/dr_dataset_reduction_data.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13100 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/dr_dataset_reduction_metadata.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11332 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/dr_dataset_reduction_metadata_sources.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13072 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/dr_job_reduction_metadata.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11829 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/dr_job_reduction_metadata_sources.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12971 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/dr_model_reduction_data.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11523 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/dr_one_dimension_point.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12103 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/dr_three_dimension_point.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11810 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/dr_two_dimension_point.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11759 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/drpca_reduction_type.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13502 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/drumap_reduction_type.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12701 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/empty_categorical_column.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12903 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/empty_continuous_column.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12586 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/error.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11685 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_all_opt_jobs.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15543 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_optimize_done.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11951 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_optimize_done_all_of.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15300 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_optimize_failed.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11638 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_optimize_failed_all_of.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15422 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_optimize_optimizing.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11784 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_optimize_optimizing_all_of.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15176 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_optimize_pending.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11437 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_optimize_pending_all_of.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16376 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_suggest_additional_done.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11926 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_suggest_additional_done_all_of.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16185 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_suggest_additional_failed.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11665 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_suggest_additional_failed_all_of.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16061 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_suggest_additional_pending.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11464 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_suggest_additional_pending_all_of.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16265 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_suggest_additional_running.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11778 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_suggest_additional_running_all_of.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16322 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_suggest_historic_done.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11906 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_suggest_historic_done_all_of.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16155 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_suggest_historic_failed.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16031 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_suggest_historic_pending.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16235 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_suggest_historic_running.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16295 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_suggest_initial_done.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11896 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_suggest_initial_done_all_of.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16215 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_suggest_initial_failed.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11746 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_suggest_initial_failed_all_of.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16016 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_suggest_initial_pending.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16220 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_suggest_initial_running.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11435 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/historic_categorical_prediction.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12150 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/historic_prediction.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11426 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/historic_scalar_prediction.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10976 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/historic_target_function.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11839 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/historic_value.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12094 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/historic_vector_prediction.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12403 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/historic_vector_value.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12954 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/importance_request.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13832 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/impute_request.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11377 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/int_cat_arr.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11426 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/job_patch.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11133 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/load_request.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    34713 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/model.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    18541 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/model_column_info.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11440 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/model_patch.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11754 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/model_permitted_column_relationships.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10999 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/models_dataset_put_request.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11775 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/models_id_additive_sensitivity_origin.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12259 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/models_id_train_permitted_column_relationships.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14076 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/new_col_fn_arg_col.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11795 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/new_col_fn_arg_col_all_of.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14640 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/new_col_fn_arg_col_weights.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12340 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/new_col_fn_arg_col_weights_all_of.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11409 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/new_col_fn_arg_col_weights_all_of_arguments.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14495 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/new_col_fn_arg_constant_sum.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12142 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/new_col_fn_arg_constant_sum_all_of.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11451 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/new_col_fn_arg_constant_sum_all_of_arguments.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14403 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/new_col_fn_arg_product.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12061 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/new_col_fn_arg_product_all_of.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11607 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/new_col_fn_arg_product_all_of_arguments.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14248 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/new_col_fn_arg_ratio.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11941 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/new_col_fn_arg_ratio_all_of.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15083 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/new_col_fn_arg_summands_weights.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12869 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/new_col_fn_arg_summands_weights_all_of.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11581 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/new_col_fn_arg_summands_weights_all_of_arguments.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14626 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/new_col_fn_arg_weighted_const_sum.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12265 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/new_col_fn_arg_weighted_const_sum_all_of.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11958 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/new_col_fn_arg_weighted_const_sum_all_of_arguments.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14537 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/new_col_fn_arg_weighted_ratio.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12178 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/new_col_fn_arg_weighted_ratio_all_of.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11981 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/new_col_fn_arg_weighted_ratio_all_of_arguments.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14354 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/new_col_fn_arg_zero_if_zero.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11941 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/new_col_fn_arg_zero_if_zero_all_of.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12440 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/new_columns.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12307 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/non_empty_categorical_column.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12381 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/non_empty_continuous_column.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12328 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/non_empty_integer_categorical_column.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    17508 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/optimize_request.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12405 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/ot_sample_def_categorical.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12087 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/ot_sample_def_continuous.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10964 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/ot_sample_definition.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10877 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/ot_set_inputs.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13043 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/outliers_request.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13158 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/output_tolerance_request.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12571 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/output_tolerance_response.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11980 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/output_tolerance_response_fixed_inputs.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11919 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/output_tolerance_response_predicted_outputs.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12010 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/output_tolerance_response_predictions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11857 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/output_tolerance_response_sampled_inputs.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11449 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/part_dependent_columns.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12668 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/part_get_optimize.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11837 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/part_get_optimize_done_result_array.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13493 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/part_get_suggest_additional.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13473 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/part_get_suggest_historic.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13463 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/part_get_suggest_initial.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11353 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/part_new_columns.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11145 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/part_tar_fn_above.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11145 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/part_tar_fn_below.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13513 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/part_tar_fn_between.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11670 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/part_tar_fn_categoricals.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14407 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/part_tar_fn_single_tar.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13421 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/part_tar_fn_sum.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13415 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/part_tar_fn_weighted_sum.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13895 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/predict_request.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12027 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/prediction.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16555 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/query_request.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14001 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/query_response.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12844 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/sample_def_categorical.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10940 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/sample_def_categorical_column_values.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16303 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/sample_def_composition.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14614 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/sample_def_composition_all_of.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12213 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/sample_def_continuous.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14847 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/sample_def_continuous_with_start.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12546 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/sample_def_discrete.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12344 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/sample_def_integer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11515 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/sample_def_start_prop.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12389 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/sample_def_weighted_categorical.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10958 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/sample_definition.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11402 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/scalar_prediction.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11456 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/scalar_result.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13086 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/sensitivity_request.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10871 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/set_inputs.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11163 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/share_group.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12266 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/si_sample_def_categorical.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11045 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/si_sample_def_categorical_column_values.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12135 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/si_sample_def_continuous.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10964 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/si_sample_definition.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11386 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/string_cat_arr.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    23791 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/suggest_additional_parameters.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    19951 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/suggest_additional_parameters_all_of.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    24667 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/suggest_additional_request.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11828 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/suggest_additional_request_all_of.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11688 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/suggest_additional_result.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13065 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/suggest_historic_parameters.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15809 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/suggest_historic_request.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12283 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/suggest_historic_result.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13828 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/suggest_historic_result_samples.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12045 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/suggest_initial_parameters.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15023 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/suggest_initial_request.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11821 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/suggest_initial_request_all_of.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    17283 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/suggest_initial_response.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11679 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/suggest_initial_result.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13582 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/suggest_missing_common.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    19333 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/suggest_missing_data.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11439 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/suggest_missing_data_all_of.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    19913 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/suggest_missing_dataset_id.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12068 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/suggest_missing_dataset_id_all_of.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    21491 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/suggest_missing_imputed_data.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13609 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/suggest_missing_imputed_data_all_of.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    23011 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/suggest_missing_request.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12222 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/suggest_missing_response.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14071 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/suggest_missing_specific.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    17194 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/tar_fn_above.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11445 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/tar_fn_above_all_of.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    17194 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/tar_fn_below.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11445 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/tar_fn_below_all_of.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    17421 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/tar_fn_between.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11507 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/tar_fn_between_all_of.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    17938 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/tar_fn_exclude_categories.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11673 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/tar_fn_exclude_categories_all_of.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    17930 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/tar_fn_include_categories.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11665 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/tar_fn_include_categories_all_of.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16392 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/tar_fn_sum_above.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11562 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/tar_fn_sum_above_all_of.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16392 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/tar_fn_sum_below.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11562 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/tar_fn_sum_below_all_of.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16619 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/tar_fn_sum_between.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11624 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/tar_fn_sum_between_all_of.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16540 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/tar_fn_weighted_sum_above.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11676 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/tar_fn_weighted_sum_above_all_of.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16540 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/tar_fn_weighted_sum_below.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11676 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/tar_fn_weighted_sum_below_all_of.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16767 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/tar_fn_weighted_sum_between.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11738 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/tar_fn_weighted_sum_between_all_of.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10952 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/target_function.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    23224 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/train_request.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11148 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/training_dataset_outliers_request.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13858 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/validate_request.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12755 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/validation_split.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11782 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/value.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12070 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/vector_prediction.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12058 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/vector_result.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12055 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/vector_value.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12328 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model/version_response.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    82086 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/model_utils.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-29 09:15:51.097527 alchemite_apiclient-0.53.0/alchemite_apiclient/models/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    21663 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/models/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14208 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/alchemite_apiclient/rest.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-29 09:15:51.061527 alchemite_apiclient-0.53.0/alchemite_apiclient.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4935 2023-03-29 09:15:51.000000 alchemite_apiclient-0.53.0/alchemite_apiclient.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)    23513 2023-03-29 09:15:51.000000 alchemite_apiclient-0.53.0/alchemite_apiclient.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-03-29 09:15:51.000000 alchemite_apiclient-0.53.0/alchemite_apiclient.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       79 2023-03-29 09:15:51.000000 alchemite_apiclient-0.53.0/alchemite_apiclient.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       20 2023-03-29 09:15:51.000000 alchemite_apiclient-0.53.0/alchemite_apiclient.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-29 09:15:51.129527 alchemite_apiclient-0.53.0/docs/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1757 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/AdditiveSensitivityRequest.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1477 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/AnalyseValidateRequest.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1123 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/AnalyseValidateRequestAllOf.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5720 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/AnalyseValidateResponse.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1616 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/AnalyseValidateResponseColumnAnalytics.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      797 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/CategoricalColumn.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      990 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/CategoricalColumnInfo.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      584 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/CategoricalColumnInfoAllOf.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      959 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/CategoricalColumnInfoStats.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2073 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/CategoricalModelColumnInfo.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1557 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/CategoricalModelColumnInfoAllOf.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      529 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/CategoricalPrediction.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      536 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/CategoricalResult.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      547 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/ColumnGroupBatchRequest.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      720 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/ColumnGroupPatchRequest.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      600 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/ColumnGroupRequest.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      674 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/ColumnGroupResponse.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      545 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/ColumnGroupResponseAllOf.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1582 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/ColumnInfo.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      624 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/ColumnValue.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      701 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/ColumnValueNullable.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1129 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/ContinuousColumnInfo.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      582 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/ContinuousColumnInfoAllOf.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1110 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/ContinuousColumnInfoStats.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1676 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/ContinuousModelColumnInfo.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1020 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/ContinuousModelColumnInfoAllOf.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      802 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/DRDatasetReductionData.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      963 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/DRDatasetReductionMetadata.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      581 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/DRDatasetReductionMetadataSources.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1038 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/DRJobReductionMetadata.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      725 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/DRJobReductionMetadataSources.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1016 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/DRModelReductionData.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      474 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/DROneDimensionPoint.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      546 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/DRPCAReductionType.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      644 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/DRThreeDimensionPoint.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      558 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/DRTwoDimensionPoint.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1155 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/DRUMAPReductionType.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      578 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/Data.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7250 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/Dataset.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      689 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/Dataset1.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      818 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/DatasetChunk.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      842 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/DatasetOrData.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      571 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/DatasetPatch.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1507 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/DatasetQueryRequest.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      866 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/DatasetQueryRequestRowIDs.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      599 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/DatasetQueryRequestSort.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      456 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/DatasetQueryResponse.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      585 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/DatasetQueryResponseResult.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)    61432 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/DatasetsApi.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)    18436 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/DefaultApi.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      791 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/DependentColFnArgCol.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      971 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/DependentColFnArgColWeights.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      748 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/DependentColFnArgConstantSum.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      731 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/DependentColFnArgProduct.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      737 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/DependentColFnArgRatio.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1190 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/DependentColFnArgSummandsWeights.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      772 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/DependentColFnArgWeightedConstSum.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      756 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/DependentColFnArgWeightedRatio.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      767 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/DependentColFnArgZeroIfZero.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      661 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/DependentColFnArgZeroIfZeroAllOf.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      975 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/DependentColumns.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      610 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/DimensionalityReductionRequest.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      699 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/DimensionalityReductionResponse.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      881 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/EmptyCategoricalColumn.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1021 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/EmptyContinuousColumn.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1027 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/Error.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      410 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/GetAllOptJobs.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1025 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/GetOptimizeDone.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      630 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/GetOptimizeDoneAllOf.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      965 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/GetOptimizeFailed.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      580 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/GetOptimizeFailedAllOf.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      988 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/GetOptimizeOptimizing.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      591 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/GetOptimizeOptimizingAllOf.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      940 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/GetOptimizePending.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      552 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/GetOptimizePendingAllOf.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1221 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/GetSuggestAdditionalDone.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      616 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/GetSuggestAdditionalDoneAllOf.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1175 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/GetSuggestAdditionalFailed.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      580 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/GetSuggestAdditionalFailedAllOf.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1150 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/GetSuggestAdditionalPending.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      552 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/GetSuggestAdditionalPendingAllOf.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1192 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/GetSuggestAdditionalRunning.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      585 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/GetSuggestAdditionalRunningAllOf.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1211 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/GetSuggestHistoricDone.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      610 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/GetSuggestHistoricDoneAllOf.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1169 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/GetSuggestHistoricFailed.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1144 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/GetSuggestHistoricPending.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1186 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/GetSuggestHistoricRunning.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1206 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/GetSuggestInitialDone.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      607 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/GetSuggestInitialDoneAllOf.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1210 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/GetSuggestInitialFailed.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      621 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/GetSuggestInitialFailedAllOf.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1141 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/GetSuggestInitialPending.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1183 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/GetSuggestInitialRunning.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      537 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/HistoricCategoricalPrediction.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      598 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/HistoricPrediction.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      534 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/HistoricScalarPrediction.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      700 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/HistoricTargetFunction.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      588 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/HistoricValue.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      609 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/HistoricVectorPrediction.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      766 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/HistoricVectorValue.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1224 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/ImportanceRequest.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1583 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/ImputeRequest.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      316 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/IntCatArr.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      563 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/JobPatch.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      500 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/LoadRequest.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2142 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/MetricsApi.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7976 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/Model.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2665 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/ModelColumnInfo.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)    34357 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/ModelDatasetApi.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      563 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/ModelPatch.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      636 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/ModelPermittedColumnRelationships.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)   138736 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/ModelsApi.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      410 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/ModelsDatasetPutRequest.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      707 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/ModelsIdAdditiveSensitivityOrigin.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      868 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/ModelsIdTrainPermittedColumnRelationships.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      773 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/NewColFnArgCol.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      679 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/NewColFnArgColAllOf.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      953 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/NewColFnArgColWeights.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      859 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/NewColFnArgColWeightsAllOf.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      539 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/NewColFnArgColWeightsAllOfArguments.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      730 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/NewColFnArgConstantSum.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      636 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/NewColFnArgConstantSumAllOf.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      599 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/NewColFnArgConstantSumAllOfArguments.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      713 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/NewColFnArgProduct.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      619 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/NewColFnArgProductAllOf.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      744 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/NewColFnArgProductAllOfArguments.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      719 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/NewColFnArgRatio.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      625 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/NewColFnArgRatioAllOf.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1172 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/NewColFnArgSummandsWeights.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1078 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/NewColFnArgSummandsWeightsAllOf.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      634 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/NewColFnArgSummandsWeightsAllOfArguments.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      754 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/NewColFnArgWeightedConstSum.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      660 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/NewColFnArgWeightedConstSumAllOf.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      698 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/NewColFnArgWeightedConstSumAllOfArguments.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      738 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/NewColFnArgWeightedRatio.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      644 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/NewColFnArgWeightedRatioAllOf.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      852 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/NewColFnArgWeightedRatioAllOfArguments.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      743 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/NewColFnArgZeroIfZero.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      649 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/NewColFnArgZeroIfZeroAllOf.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      799 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/NewColumns.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      770 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/NonEmptyCategoricalColumn.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      843 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/NonEmptyContinuousColumn.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      777 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/NonEmptyIntegerCategoricalColumn.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1254 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/OTSampleDefCategorical.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      815 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/OTSampleDefContinuous.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      604 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/OTSampleDefinition.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      494 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/OTSetInputs.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2953 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/OptimizeRequest.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1255 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/OutliersRequest.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1110 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/OutputToleranceRequest.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      644 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/OutputToleranceResponse.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      809 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/OutputToleranceResponseFixedInputs.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      674 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/OutputToleranceResponsePredictedOutputs.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      776 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/OutputToleranceResponsePredictions.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      741 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/OutputToleranceResponseSampledInputs.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      579 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/PartDependentColumns.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      889 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/PartGetOptimize.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      464 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/PartGetOptimizeDoneResultArray.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1099 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/PartGetSuggestAdditional.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1093 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/PartGetSuggestHistoric.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1090 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/PartGetSuggestInitial.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      561 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/PartNewColumns.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      492 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/PartTarFnAbove.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      492 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/PartTarFnBelow.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      524 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/PartTarFnBetween.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      586 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/PartTarFnCategoricals.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1968 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/PartTarFnSingleTar.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1581 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/PartTarFnSum.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1570 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/PartTarFnWeightedSum.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1614 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/PredictRequest.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      590 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/Prediction.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1716 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/QueryRequest.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      692 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/QueryResponse.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      771 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/SISampleDefCategorical.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      538 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/SISampleDefCategoricalColumnValues.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      859 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/SISampleDefContinuous.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      520 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/SISampleDefinition.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1068 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/SampleDefCategorical.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      536 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/SampleDefCategoricalColumnValues.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1757 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/SampleDefComposition.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1661 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/SampleDefCompositionAllOf.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1022 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/SampleDefContinuous.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1342 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/SampleDefContinuousWithStart.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      962 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/SampleDefDiscrete.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1035 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/SampleDefInteger.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      818 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/SampleDefStartProp.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      784 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/SampleDefWeightedCategorical.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      531 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/SampleDefinition.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      526 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/ScalarPrediction.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      653 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/ScalarResult.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1196 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/SensitivityRequest.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      488 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/SetInputs.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      512 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/ShareGroup.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      319 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/StringCatArr.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4837 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/SuggestAdditionalParameters.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3870 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/SuggestAdditionalParametersAllOf.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5099 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/SuggestAdditionalRequest.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      742 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/SuggestAdditionalRequestAllOf.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      396 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/SuggestAdditionalResult.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1050 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/SuggestHistoricParameters.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1312 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/SuggestHistoricRequest.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      922 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/SuggestHistoricResult.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1358 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/SuggestHistoricResultSamples.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      699 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/SuggestInitialParameters.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      962 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/SuggestInitialRequest.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      740 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/SuggestInitialRequestAllOf.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1470 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/SuggestInitialResponse.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      393 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/SuggestInitialResult.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1440 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/SuggestMissingCommon.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2955 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/SuggestMissingData.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      648 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/SuggestMissingDataAllOf.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3155 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/SuggestMissingDatasetID.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      848 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/SuggestMissingDatasetIDAllOf.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4011 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/SuggestMissingImputedData.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1704 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/SuggestMissingImputedDataAllOf.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4589 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/SuggestMissingRequest.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      909 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/SuggestMissingResponse.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1810 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/SuggestMissingSpecific.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2090 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/TarFnAbove.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      563 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/TarFnAboveAllOf.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2090 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/TarFnBelow.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      563 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/TarFnBelowAllOf.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2164 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/TarFnBetween.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      607 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/TarFnBetweenAllOf.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2226 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/TarFnExcludeCategories.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      612 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/TarFnExcludeCategoriesAllOf.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2222 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/TarFnIncludeCategories.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      608 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/TarFnIncludeCategoriesAllOf.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1754 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/TarFnSumAbove.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      608 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/TarFnSumAboveAllOf.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1754 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/TarFnSumBelow.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      608 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/TarFnSumBelowAllOf.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1828 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/TarFnSumBetween.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      652 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/TarFnSumBetweenAllOf.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1761 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/TarFnWeightedSumAbove.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      634 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/TarFnWeightedSumAboveAllOf.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1761 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/TarFnWeightedSumBelow.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      634 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/TarFnWeightedSumBelowAllOf.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1835 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/TarFnWeightedSumBetween.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      678 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/TarFnWeightedSumBetweenAllOf.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1218 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/TargetFunction.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5666 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/TrainRequest.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      466 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/TrainingDatasetOutliersRequest.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1595 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/ValidateRequest.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1096 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/ValidationSplit.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      580 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/Value.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      601 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/VectorPrediction.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      597 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/VectorResult.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      596 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/VectorValue.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      945 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/docs/VersionResponse.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-29 09:15:51.137527 alchemite_apiclient-0.53.0/example/
--rw-r--r--   0 circleci  (3434) circleci  (3434)   701201 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/example/adrenergic.csv
--rw-r--r--   0 circleci  (3434) circleci  (3434)   243835 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/example/adrenergic_holdout.csv
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1654 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/example/adrenergic_row.csv
--rw-r--r--   0 circleci  (3434) circleci  (3434)      591 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/example/categorical.csv
--rw-r--r--   0 circleci  (3434) circleci  (3434)      140 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/example/credentials_auth_code_SAMPLE.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      179 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/example/credentials_client_SAMPLE.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      167 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/example/credentials_pass_SAMPLE.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      157 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/example/credentials_pass_prompted_SAMPLE.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4566 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/example/example_additive_sensitivity.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4189 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/example/example_basic.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3944 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/example/example_categorical.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2775 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/example/example_chunk.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4120 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/example/example_column_groups.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      490 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/example/example_connect.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5769 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/example/example_custom_validation_splits.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1175 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/example/example_delete.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5634 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/example/example_dimensionality_reduction.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      599 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/example/example_download.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1534 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/example/example_export_import.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4185 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/example/example_hyperopt.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3833 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/example/example_importance.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5574 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/example/example_optimize.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3181 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/example/example_outliers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4318 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/example/example_output_tolerance.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4511 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/example/example_preload.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4053 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/example/example_query.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4504 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/example/example_sensitivity.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5511 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/example/example_suggest_additional.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5547 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/example/example_suggest_historic.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1980 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/example/example_suggest_initial.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4598 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/example/example_suggest_missing.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3419 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/example/example_training_outliers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5099 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/example/example_validate.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5496 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/example/example_vector.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      759 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/example/optimize_args_steel.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      425 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/example/optimize_args_vector.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1290 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/example/optimize_dependentColumns_args_steel.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1189 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/example/steels.csv
--rw-r--r--   0 circleci  (3434) circleci  (3434)      367 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/example/steels_impute.csv
--rw-r--r--   0 circleci  (3434) circleci  (3434)      854 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/example/suggest_additional_args_steel.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      487 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/example/suggest_additional_args_vector.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      247 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/example/suggest_historic_args_steel.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      244 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/example/suggest_historic_args_vector.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      463 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/example/suggest_initial_args.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      503 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/example/vector.csv
--rw-r--r--   0 circleci  (3434) circleci  (3434)      880 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/pyproject.toml
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-03-29 09:15:51.137527 alchemite_apiclient-0.53.0/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1178 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-29 09:15:51.137527 alchemite_apiclient-0.53.0/test/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2255 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/test/test_cornercases.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3919 2023-03-29 09:15:45.000000 alchemite_apiclient-0.53.0/test/test_examples.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-26 09:34:19.358073 alchemite_apiclient-0.54.0/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       61 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       25 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4935 2023-04-26 09:34:19.358073 alchemite_apiclient-0.54.0/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4232 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-26 09:34:19.234071 alchemite_apiclient-0.54.0/alchemite_apiclient/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    22492 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-26 09:34:19.238071 alchemite_apiclient-0.54.0/alchemite_apiclient/api/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      224 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/api/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   112942 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/api/datasets_api.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    35604 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/api/default_api.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5200 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/api/metrics_api.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    58362 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/api/model_dataset_api.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   233750 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/api/models_api.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    37770 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/api_client.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-26 09:34:19.238071 alchemite_apiclient-0.54.0/alchemite_apiclient/apis/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      721 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/apis/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    17318 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/configuration.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5079 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/exceptions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13896 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/extensions.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-26 09:34:19.286072 alchemite_apiclient-0.54.0/alchemite_apiclient/model/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      348 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14502 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/additive_sensitivity_request.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15940 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/analyse_validate_request.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12717 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/analyse_validate_request_all_of.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    24816 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/analyse_validate_response.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14439 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/analyse_validate_response_column_analytics.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12124 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/categorical_column.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15273 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/categorical_column_info.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11771 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/categorical_column_info_all_of.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14958 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/categorical_column_info_stats.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    17661 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/categorical_model_column_info.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13506 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/categorical_model_column_info_all_of.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11411 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/categorical_prediction.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11432 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/categorical_result.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11554 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/column_group_batch_request.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11738 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/column_group_patch_request.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11605 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/column_group_request.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13897 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/column_group_response.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11120 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/column_group_response_all_of.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16155 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/column_info.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11587 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/column_value.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11749 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/column_value_nullable.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15595 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/continuous_column_info.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11760 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/continuous_column_info_all_of.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15093 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/continuous_column_info_stats.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16839 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/continuous_model_column_info.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12255 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/continuous_model_column_info_all_of.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11280 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/data.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    27957 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/dataset.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11519 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/dataset1.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12344 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/dataset_chunk.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14079 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/dataset_or_data.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11454 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/dataset_patch.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14432 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/dataset_query_request.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12022 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/dataset_query_request_row_ids.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11619 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/dataset_query_request_sort.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11888 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/dataset_query_response.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11530 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/dataset_query_response_result.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14166 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/dependent_col_fn_arg_col.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14730 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/dependent_col_fn_arg_col_weights.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14585 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/dependent_col_fn_arg_constant_sum.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14493 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/dependent_col_fn_arg_product.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14338 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/dependent_col_fn_arg_ratio.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15173 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/dependent_col_fn_arg_summands_weights.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14716 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/dependent_col_fn_arg_weighted_const_sum.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14627 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/dependent_col_fn_arg_weighted_ratio.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14486 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/dependent_col_fn_arg_zero_if_zero.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11971 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/dependent_col_fn_arg_zero_if_zero_all_of.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12802 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/dependent_columns.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12505 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/dimensionality_reduction_request.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12947 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/dimensionality_reduction_response.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12516 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/dr_dataset_reduction_data.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13100 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/dr_dataset_reduction_metadata.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11332 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/dr_dataset_reduction_metadata_sources.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13072 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/dr_job_reduction_metadata.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11829 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/dr_job_reduction_metadata_sources.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12971 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/dr_model_reduction_data.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11523 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/dr_one_dimension_point.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12103 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/dr_three_dimension_point.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11810 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/dr_two_dimension_point.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11759 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/drpca_reduction_type.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13502 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/drumap_reduction_type.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12701 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/empty_categorical_column.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12903 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/empty_continuous_column.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12586 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/error.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11685 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_all_opt_jobs.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15543 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_optimize_done.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11951 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_optimize_done_all_of.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15300 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_optimize_failed.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11638 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_optimize_failed_all_of.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15422 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_optimize_optimizing.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11784 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_optimize_optimizing_all_of.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15176 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_optimize_pending.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11437 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_optimize_pending_all_of.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16376 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_suggest_additional_done.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11926 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_suggest_additional_done_all_of.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16185 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_suggest_additional_failed.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11665 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_suggest_additional_failed_all_of.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16061 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_suggest_additional_pending.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11464 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_suggest_additional_pending_all_of.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16265 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_suggest_additional_running.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11778 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_suggest_additional_running_all_of.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16322 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_suggest_historic_done.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11906 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_suggest_historic_done_all_of.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16155 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_suggest_historic_failed.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16031 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_suggest_historic_pending.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16235 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_suggest_historic_running.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16295 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_suggest_initial_done.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11896 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_suggest_initial_done_all_of.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16215 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_suggest_initial_failed.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11746 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_suggest_initial_failed_all_of.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16016 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_suggest_initial_pending.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16220 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_suggest_initial_running.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11435 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/historic_categorical_prediction.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12150 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/historic_prediction.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11426 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/historic_scalar_prediction.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10976 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/historic_target_function.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11839 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/historic_value.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12094 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/historic_vector_prediction.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12403 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/historic_vector_value.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12954 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/importance_request.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13832 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/impute_request.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11377 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/int_cat_arr.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11426 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/job_patch.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11133 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/load_request.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    34713 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/model.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    18541 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/model_column_info.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11440 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/model_patch.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11754 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/model_permitted_column_relationships.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10999 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/models_dataset_put_request.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11775 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/models_id_additive_sensitivity_origin.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12259 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/models_id_train_permitted_column_relationships.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14076 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/new_col_fn_arg_col.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11795 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/new_col_fn_arg_col_all_of.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14640 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/new_col_fn_arg_col_weights.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12340 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/new_col_fn_arg_col_weights_all_of.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11409 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/new_col_fn_arg_col_weights_all_of_arguments.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14495 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/new_col_fn_arg_constant_sum.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12142 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/new_col_fn_arg_constant_sum_all_of.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11451 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/new_col_fn_arg_constant_sum_all_of_arguments.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14403 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/new_col_fn_arg_product.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12061 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/new_col_fn_arg_product_all_of.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11607 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/new_col_fn_arg_product_all_of_arguments.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14248 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/new_col_fn_arg_ratio.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11941 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/new_col_fn_arg_ratio_all_of.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15083 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/new_col_fn_arg_summands_weights.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12869 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/new_col_fn_arg_summands_weights_all_of.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11581 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/new_col_fn_arg_summands_weights_all_of_arguments.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14626 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/new_col_fn_arg_weighted_const_sum.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12265 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/new_col_fn_arg_weighted_const_sum_all_of.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11958 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/new_col_fn_arg_weighted_const_sum_all_of_arguments.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14537 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/new_col_fn_arg_weighted_ratio.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12178 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/new_col_fn_arg_weighted_ratio_all_of.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11981 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/new_col_fn_arg_weighted_ratio_all_of_arguments.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14354 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/new_col_fn_arg_zero_if_zero.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11941 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/new_col_fn_arg_zero_if_zero_all_of.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12440 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/new_columns.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12307 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/non_empty_categorical_column.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12381 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/non_empty_continuous_column.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12328 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/non_empty_integer_categorical_column.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    17508 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/optimize_request.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12405 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/ot_sample_def_categorical.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12087 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/ot_sample_def_continuous.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10964 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/ot_sample_definition.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10877 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/ot_set_inputs.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13043 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/outliers_request.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13158 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/output_tolerance_request.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12571 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/output_tolerance_response.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11980 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/output_tolerance_response_fixed_inputs.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11919 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/output_tolerance_response_predicted_outputs.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12010 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/output_tolerance_response_predictions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11857 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/output_tolerance_response_sampled_inputs.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11449 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/part_dependent_columns.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12668 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/part_get_optimize.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11837 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/part_get_optimize_done_result_array.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13493 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/part_get_suggest_additional.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13473 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/part_get_suggest_historic.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13463 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/part_get_suggest_initial.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11353 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/part_new_columns.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11145 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/part_tar_fn_above.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11145 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/part_tar_fn_below.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13513 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/part_tar_fn_between.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11670 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/part_tar_fn_categoricals.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14407 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/part_tar_fn_single_tar.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13421 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/part_tar_fn_sum.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13415 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/part_tar_fn_weighted_sum.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13895 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/predict_request.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12027 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/prediction.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16555 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/query_request.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14001 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/query_response.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12844 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/sample_def_categorical.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10940 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/sample_def_categorical_column_values.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16961 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/sample_def_composition.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15367 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/sample_def_composition_all_of.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12213 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/sample_def_continuous.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14847 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/sample_def_continuous_with_start.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12546 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/sample_def_discrete.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12344 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/sample_def_integer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11515 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/sample_def_start_prop.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12389 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/sample_def_weighted_categorical.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10958 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/sample_definition.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11402 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/scalar_prediction.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11456 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/scalar_result.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13086 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/sensitivity_request.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10871 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/set_inputs.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11163 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/share_group.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12266 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/si_sample_def_categorical.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11045 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/si_sample_def_categorical_column_values.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12135 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/si_sample_def_continuous.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10964 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/si_sample_definition.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11386 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/string_cat_arr.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    23791 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/suggest_additional_parameters.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    19951 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/suggest_additional_parameters_all_of.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    24667 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/suggest_additional_request.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11828 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/suggest_additional_request_all_of.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11688 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/suggest_additional_result.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13065 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/suggest_historic_parameters.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15809 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/suggest_historic_request.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12283 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/suggest_historic_result.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13828 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/suggest_historic_result_samples.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12045 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/suggest_initial_parameters.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15023 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/suggest_initial_request.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11821 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/suggest_initial_request_all_of.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    17283 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/suggest_initial_response.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11679 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/suggest_initial_result.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13582 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/suggest_missing_common.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    19333 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/suggest_missing_data.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11439 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/suggest_missing_data_all_of.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    19913 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/suggest_missing_dataset_id.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12068 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/suggest_missing_dataset_id_all_of.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    21491 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/suggest_missing_imputed_data.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13609 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/suggest_missing_imputed_data_all_of.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    23011 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/suggest_missing_request.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12222 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/suggest_missing_response.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14071 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/suggest_missing_specific.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    17194 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/tar_fn_above.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11445 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/tar_fn_above_all_of.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    17194 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/tar_fn_below.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11445 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/tar_fn_below_all_of.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    17421 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/tar_fn_between.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11507 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/tar_fn_between_all_of.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    17938 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/tar_fn_exclude_categories.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11673 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/tar_fn_exclude_categories_all_of.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    17930 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/tar_fn_include_categories.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11665 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/tar_fn_include_categories_all_of.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16392 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/tar_fn_sum_above.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11562 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/tar_fn_sum_above_all_of.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16392 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/tar_fn_sum_below.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11562 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/tar_fn_sum_below_all_of.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16619 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/tar_fn_sum_between.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11624 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/tar_fn_sum_between_all_of.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16540 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/tar_fn_weighted_sum_above.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11676 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/tar_fn_weighted_sum_above_all_of.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16540 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/tar_fn_weighted_sum_below.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11676 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/tar_fn_weighted_sum_below_all_of.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16767 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/tar_fn_weighted_sum_between.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11738 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/tar_fn_weighted_sum_between_all_of.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10952 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/target_function.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    23224 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/train_request.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11148 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/training_dataset_outliers_request.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13858 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/validate_request.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12755 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/validation_split.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11782 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/value.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12070 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/vector_prediction.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12058 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/vector_result.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12055 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/vector_value.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12328 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model/version_response.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    82086 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/model_utils.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-26 09:34:19.286072 alchemite_apiclient-0.54.0/alchemite_apiclient/models/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    21663 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/models/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14208 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/alchemite_apiclient/rest.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-26 09:34:19.234071 alchemite_apiclient-0.54.0/alchemite_apiclient.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4935 2023-04-26 09:34:19.000000 alchemite_apiclient-0.54.0/alchemite_apiclient.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    23513 2023-04-26 09:34:19.000000 alchemite_apiclient-0.54.0/alchemite_apiclient.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-26 09:34:19.000000 alchemite_apiclient-0.54.0/alchemite_apiclient.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       79 2023-04-26 09:34:19.000000 alchemite_apiclient-0.54.0/alchemite_apiclient.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       20 2023-04-26 09:34:19.000000 alchemite_apiclient-0.54.0/alchemite_apiclient.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-26 09:34:19.342072 alchemite_apiclient-0.54.0/docs/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1757 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/AdditiveSensitivityRequest.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1477 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/AnalyseValidateRequest.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1123 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/AnalyseValidateRequestAllOf.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5720 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/AnalyseValidateResponse.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1616 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/AnalyseValidateResponseColumnAnalytics.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      797 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/CategoricalColumn.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      990 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/CategoricalColumnInfo.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      584 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/CategoricalColumnInfoAllOf.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      959 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/CategoricalColumnInfoStats.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2073 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/CategoricalModelColumnInfo.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1557 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/CategoricalModelColumnInfoAllOf.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      529 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/CategoricalPrediction.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      536 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/CategoricalResult.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      547 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/ColumnGroupBatchRequest.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      720 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/ColumnGroupPatchRequest.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      600 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/ColumnGroupRequest.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      674 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/ColumnGroupResponse.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      545 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/ColumnGroupResponseAllOf.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1582 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/ColumnInfo.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      624 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/ColumnValue.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      701 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/ColumnValueNullable.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1129 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/ContinuousColumnInfo.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      582 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/ContinuousColumnInfoAllOf.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1110 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/ContinuousColumnInfoStats.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1676 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/ContinuousModelColumnInfo.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1020 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/ContinuousModelColumnInfoAllOf.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      802 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/DRDatasetReductionData.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      963 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/DRDatasetReductionMetadata.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      581 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/DRDatasetReductionMetadataSources.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1038 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/DRJobReductionMetadata.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      725 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/DRJobReductionMetadataSources.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1016 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/DRModelReductionData.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      474 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/DROneDimensionPoint.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      546 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/DRPCAReductionType.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      644 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/DRThreeDimensionPoint.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      558 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/DRTwoDimensionPoint.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1155 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/DRUMAPReductionType.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      578 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/Data.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7250 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/Dataset.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      689 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/Dataset1.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      818 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/DatasetChunk.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      842 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/DatasetOrData.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      571 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/DatasetPatch.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1507 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/DatasetQueryRequest.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      866 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/DatasetQueryRequestRowIDs.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      599 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/DatasetQueryRequestSort.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      456 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/DatasetQueryResponse.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      585 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/DatasetQueryResponseResult.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    61432 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/DatasetsApi.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    18436 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/DefaultApi.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      791 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/DependentColFnArgCol.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      971 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/DependentColFnArgColWeights.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      748 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/DependentColFnArgConstantSum.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      731 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/DependentColFnArgProduct.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      737 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/DependentColFnArgRatio.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1190 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/DependentColFnArgSummandsWeights.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      772 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/DependentColFnArgWeightedConstSum.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      756 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/DependentColFnArgWeightedRatio.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      767 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/DependentColFnArgZeroIfZero.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      661 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/DependentColFnArgZeroIfZeroAllOf.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      975 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/DependentColumns.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      610 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/DimensionalityReductionRequest.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      699 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/DimensionalityReductionResponse.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      881 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/EmptyCategoricalColumn.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1021 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/EmptyContinuousColumn.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1027 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/Error.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      410 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/GetAllOptJobs.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1025 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/GetOptimizeDone.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      630 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/GetOptimizeDoneAllOf.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      965 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/GetOptimizeFailed.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      580 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/GetOptimizeFailedAllOf.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      988 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/GetOptimizeOptimizing.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      591 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/GetOptimizeOptimizingAllOf.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      940 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/GetOptimizePending.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      552 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/GetOptimizePendingAllOf.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1221 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/GetSuggestAdditionalDone.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      616 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/GetSuggestAdditionalDoneAllOf.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1175 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/GetSuggestAdditionalFailed.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      580 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/GetSuggestAdditionalFailedAllOf.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1150 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/GetSuggestAdditionalPending.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      552 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/GetSuggestAdditionalPendingAllOf.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1192 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/GetSuggestAdditionalRunning.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      585 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/GetSuggestAdditionalRunningAllOf.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1211 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/GetSuggestHistoricDone.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      610 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/GetSuggestHistoricDoneAllOf.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1169 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/GetSuggestHistoricFailed.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1144 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/GetSuggestHistoricPending.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1186 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/GetSuggestHistoricRunning.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1206 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/GetSuggestInitialDone.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      607 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/GetSuggestInitialDoneAllOf.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1210 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/GetSuggestInitialFailed.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      621 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/GetSuggestInitialFailedAllOf.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1141 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/GetSuggestInitialPending.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1183 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/GetSuggestInitialRunning.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      537 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/HistoricCategoricalPrediction.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      598 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/HistoricPrediction.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      534 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/HistoricScalarPrediction.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      700 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/HistoricTargetFunction.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      588 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/HistoricValue.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      609 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/HistoricVectorPrediction.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      766 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/HistoricVectorValue.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1224 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/ImportanceRequest.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1583 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/ImputeRequest.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      316 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/IntCatArr.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      563 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/JobPatch.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      500 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/LoadRequest.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2142 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/MetricsApi.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7976 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/Model.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2665 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/ModelColumnInfo.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    34357 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/ModelDatasetApi.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      563 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/ModelPatch.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      636 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/ModelPermittedColumnRelationships.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   138736 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/ModelsApi.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      410 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/ModelsDatasetPutRequest.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      707 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/ModelsIdAdditiveSensitivityOrigin.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      868 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/ModelsIdTrainPermittedColumnRelationships.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      773 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/NewColFnArgCol.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      679 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/NewColFnArgColAllOf.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      953 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/NewColFnArgColWeights.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      859 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/NewColFnArgColWeightsAllOf.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      539 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/NewColFnArgColWeightsAllOfArguments.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      730 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/NewColFnArgConstantSum.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      636 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/NewColFnArgConstantSumAllOf.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      599 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/NewColFnArgConstantSumAllOfArguments.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      713 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/NewColFnArgProduct.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      619 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/NewColFnArgProductAllOf.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      744 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/NewColFnArgProductAllOfArguments.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      719 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/NewColFnArgRatio.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      625 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/NewColFnArgRatioAllOf.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1172 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/NewColFnArgSummandsWeights.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1078 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/NewColFnArgSummandsWeightsAllOf.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      634 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/NewColFnArgSummandsWeightsAllOfArguments.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      754 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/NewColFnArgWeightedConstSum.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      660 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/NewColFnArgWeightedConstSumAllOf.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      698 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/NewColFnArgWeightedConstSumAllOfArguments.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      738 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/NewColFnArgWeightedRatio.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      644 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/NewColFnArgWeightedRatioAllOf.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      852 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/NewColFnArgWeightedRatioAllOfArguments.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      743 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/NewColFnArgZeroIfZero.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      649 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/NewColFnArgZeroIfZeroAllOf.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      799 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/NewColumns.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      770 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/NonEmptyCategoricalColumn.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      843 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/NonEmptyContinuousColumn.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      777 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/NonEmptyIntegerCategoricalColumn.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1254 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/OTSampleDefCategorical.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      815 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/OTSampleDefContinuous.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      604 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/OTSampleDefinition.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      494 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/OTSetInputs.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2953 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/OptimizeRequest.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1255 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/OutliersRequest.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1110 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/OutputToleranceRequest.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      644 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/OutputToleranceResponse.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      809 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/OutputToleranceResponseFixedInputs.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      674 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/OutputToleranceResponsePredictedOutputs.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      776 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/OutputToleranceResponsePredictions.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      741 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/OutputToleranceResponseSampledInputs.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      579 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/PartDependentColumns.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      889 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/PartGetOptimize.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      464 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/PartGetOptimizeDoneResultArray.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1099 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/PartGetSuggestAdditional.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1093 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/PartGetSuggestHistoric.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1090 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/PartGetSuggestInitial.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      561 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/PartNewColumns.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      492 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/PartTarFnAbove.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      492 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/PartTarFnBelow.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      524 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/PartTarFnBetween.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      586 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/PartTarFnCategoricals.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1968 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/PartTarFnSingleTar.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1581 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/PartTarFnSum.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1570 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/PartTarFnWeightedSum.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1614 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/PredictRequest.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      590 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/Prediction.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1716 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/QueryRequest.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      692 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/QueryResponse.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      771 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/SISampleDefCategorical.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      538 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/SISampleDefCategoricalColumnValues.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      859 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/SISampleDefContinuous.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      520 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/SISampleDefinition.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1068 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/SampleDefCategorical.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      536 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/SampleDefCategoricalColumnValues.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2029 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/SampleDefComposition.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1933 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/SampleDefCompositionAllOf.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1022 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/SampleDefContinuous.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1342 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/SampleDefContinuousWithStart.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      962 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/SampleDefDiscrete.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1035 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/SampleDefInteger.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      818 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/SampleDefStartProp.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      784 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/SampleDefWeightedCategorical.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      531 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/SampleDefinition.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      526 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/ScalarPrediction.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      653 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/ScalarResult.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1196 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/SensitivityRequest.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      488 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/SetInputs.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      512 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/ShareGroup.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      319 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/StringCatArr.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4837 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/SuggestAdditionalParameters.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3870 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/SuggestAdditionalParametersAllOf.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5099 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/SuggestAdditionalRequest.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      742 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/SuggestAdditionalRequestAllOf.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      396 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/SuggestAdditionalResult.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1050 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/SuggestHistoricParameters.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1312 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/SuggestHistoricRequest.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      922 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/SuggestHistoricResult.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1358 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/SuggestHistoricResultSamples.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      699 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/SuggestInitialParameters.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      962 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/SuggestInitialRequest.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      740 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/SuggestInitialRequestAllOf.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1470 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/SuggestInitialResponse.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      393 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/SuggestInitialResult.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1440 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/SuggestMissingCommon.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2955 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/SuggestMissingData.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      648 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/SuggestMissingDataAllOf.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3155 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/SuggestMissingDatasetID.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      848 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/SuggestMissingDatasetIDAllOf.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4011 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/SuggestMissingImputedData.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1704 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/SuggestMissingImputedDataAllOf.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4589 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/SuggestMissingRequest.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      909 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/SuggestMissingResponse.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1810 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/SuggestMissingSpecific.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2090 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/TarFnAbove.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      563 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/TarFnAboveAllOf.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2090 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/TarFnBelow.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      563 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/TarFnBelowAllOf.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2164 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/TarFnBetween.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      607 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/TarFnBetweenAllOf.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2226 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/TarFnExcludeCategories.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      612 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/TarFnExcludeCategoriesAllOf.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2222 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/TarFnIncludeCategories.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      608 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/TarFnIncludeCategoriesAllOf.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1754 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/TarFnSumAbove.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      608 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/TarFnSumAboveAllOf.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1754 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/TarFnSumBelow.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      608 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/TarFnSumBelowAllOf.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1828 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/TarFnSumBetween.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      652 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/TarFnSumBetweenAllOf.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1761 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/TarFnWeightedSumAbove.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      634 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/TarFnWeightedSumAboveAllOf.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1761 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/TarFnWeightedSumBelow.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      634 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/TarFnWeightedSumBelowAllOf.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1835 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/TarFnWeightedSumBetween.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      678 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/TarFnWeightedSumBetweenAllOf.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1218 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/TargetFunction.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5666 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/TrainRequest.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      466 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/TrainingDatasetOutliersRequest.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1595 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/ValidateRequest.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1096 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/ValidationSplit.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      580 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/Value.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      601 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/VectorPrediction.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      597 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/VectorResult.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      596 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/VectorValue.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      945 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/docs/VersionResponse.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-26 09:34:19.358073 alchemite_apiclient-0.54.0/example/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   701201 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/example/adrenergic.csv
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   243835 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/example/adrenergic_holdout.csv
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1654 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/example/adrenergic_row.csv
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      591 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/example/categorical.csv
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      140 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/example/credentials_auth_code_SAMPLE.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      179 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/example/credentials_client_SAMPLE.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      167 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/example/credentials_pass_SAMPLE.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      157 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/example/credentials_pass_prompted_SAMPLE.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4566 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/example/example_additive_sensitivity.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4189 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/example/example_basic.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3944 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/example/example_categorical.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2775 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/example/example_chunk.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4120 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/example/example_column_groups.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      490 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/example/example_connect.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5769 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/example/example_custom_validation_splits.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1175 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/example/example_delete.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5634 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/example/example_dimensionality_reduction.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      599 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/example/example_download.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1534 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/example/example_export_import.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4185 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/example/example_hyperopt.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3833 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/example/example_importance.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5574 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/example/example_optimize.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3181 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/example/example_outliers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4318 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/example/example_output_tolerance.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4511 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/example/example_preload.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4053 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/example/example_query.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4504 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/example/example_sensitivity.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5511 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/example/example_suggest_additional.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5547 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/example/example_suggest_historic.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1980 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/example/example_suggest_initial.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4598 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/example/example_suggest_missing.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3419 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/example/example_training_outliers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5099 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/example/example_validate.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5496 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/example/example_vector.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      759 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/example/optimize_args_steel.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      425 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/example/optimize_args_vector.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1290 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/example/optimize_dependentColumns_args_steel.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1189 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/example/steels.csv
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      367 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/example/steels_impute.csv
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      854 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/example/suggest_additional_args_steel.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      487 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/example/suggest_additional_args_vector.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      247 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/example/suggest_historic_args_steel.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      244 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/example/suggest_historic_args_vector.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      463 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/example/suggest_initial_args.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      503 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/example/vector.csv
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      880 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/pyproject.toml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-04-26 09:34:19.358073 alchemite_apiclient-0.54.0/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1178 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-26 09:34:19.358073 alchemite_apiclient-0.54.0/test/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2255 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/test/test_cornercases.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3919 2023-04-26 09:34:13.000000 alchemite_apiclient-0.54.0/test/test_examples.py
```

### Comparing `alchemite_apiclient-0.53.0/PKG-INFO` & `alchemite_apiclient-0.54.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alchemite_apiclient
-Version: 0.53.0
+Version: 0.54.0
 Summary: A python API client for using Alchemite Analytics
 Home-page: 
 Author: Intellegens
 Author-email: Intellegens <support@intellegens.com>
 Project-URL: Homepage, https://intellegens.com
 Project-URL: Docs, https://docs.intellegens.com
 Keywords: Alchemite,Alchemite API,Machine Learning,Artificial Intelligence
@@ -19,15 +19,15 @@
 
 # alchemite-apiclient
 
 This is a client for interacting with Alchemite Analytics, an applied machine learning platform to accelerate industrial
 R&D and optimise manufacturing by extracting information from sparce or noisy datasets.
 To obtain a licence for this product, please [contact Intellegens](https://intellegens.com/contact-us/) for more information.
 
-API version: 0.53.0
+API version: 0.54.0
 
 ## Requirements.
 
 Python >=3.8
 
 ## Installation & Usage
 ### pip install
```

### Comparing `alchemite_apiclient-0.53.0/README.md` & `alchemite_apiclient-0.54.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # alchemite-apiclient
 
 This is a client for interacting with Alchemite Analytics, an applied machine learning platform to accelerate industrial
 R&D and optimise manufacturing by extracting information from sparce or noisy datasets.
 To obtain a licence for this product, please [contact Intellegens](https://intellegens.com/contact-us/) for more information.
 
-API version: 0.53.0
+API version: 0.54.0
 
 ## Requirements.
 
 Python >=3.8
 
 ## Installation & Usage
 ### pip install
```

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/__init__.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
     Contact: support@intellegens.com
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "0.53.0"
+__version__ = "0.54.0"
 
 # import ApiClient
 from alchemite_apiclient.api_client import ApiClient
 
 # import Configuration
 from alchemite_apiclient.configuration import Configuration
```

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/api/datasets_api.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/api/datasets_api.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/api/default_api.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/api/default_api.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/api/metrics_api.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/api/metrics_api.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/api/model_dataset_api.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/api/model_dataset_api.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/api/models_api.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/api/models_api.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/api_client.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.53.0/python'
+        self.user_agent = 'OpenAPI-Generator/0.54.0/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/apis/__init__.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/configuration.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -403,16 +403,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.53.0\n"\
-               "SDK Package Version: 0.53.0".\
+               "Version of the API: 0.54.0\n"\
+               "SDK Package Version: 0.54.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/exceptions.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/extensions.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/extensions.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/additive_sensitivity_request.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/additive_sensitivity_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/analyse_validate_request.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/analyse_validate_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/analyse_validate_request_all_of.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/analyse_validate_request_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/analyse_validate_response.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/analyse_validate_response.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/analyse_validate_response_column_analytics.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/analyse_validate_response_column_analytics.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/categorical_column.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/categorical_column.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/categorical_column_info.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/categorical_column_info.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/categorical_column_info_all_of.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/categorical_column_info_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/categorical_column_info_stats.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/categorical_column_info_stats.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/categorical_model_column_info.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/categorical_model_column_info.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/categorical_model_column_info_all_of.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/categorical_model_column_info_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/categorical_prediction.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/categorical_prediction.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/categorical_result.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/categorical_result.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/column_group_batch_request.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/column_group_batch_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/column_group_patch_request.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/column_group_patch_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/column_group_request.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/column_group_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/column_group_response.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/column_group_response.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/column_group_response_all_of.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/column_group_response_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/column_info.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/column_info.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/column_value.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/column_value.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/column_value_nullable.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/column_value_nullable.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/continuous_column_info.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/continuous_column_info.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/continuous_column_info_all_of.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/continuous_column_info_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/continuous_column_info_stats.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/continuous_column_info_stats.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/continuous_model_column_info.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/continuous_model_column_info.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/continuous_model_column_info_all_of.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/continuous_model_column_info_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/data.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/data.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/dataset.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/dataset.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/dataset1.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/dataset1.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/dataset_chunk.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/dataset_chunk.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/dataset_or_data.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/dataset_or_data.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/dataset_patch.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/dataset_patch.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/dataset_query_request.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/dataset_query_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/dataset_query_request_row_ids.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/dataset_query_request_row_ids.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/dataset_query_request_sort.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/dataset_query_request_sort.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/dataset_query_response.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/dataset_query_response.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/dataset_query_response_result.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/dataset_query_response_result.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/dependent_col_fn_arg_col.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/dependent_col_fn_arg_col.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/dependent_col_fn_arg_col_weights.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/dependent_col_fn_arg_col_weights.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/dependent_col_fn_arg_constant_sum.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/dependent_col_fn_arg_constant_sum.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/dependent_col_fn_arg_product.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/dependent_col_fn_arg_product.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/dependent_col_fn_arg_ratio.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/dependent_col_fn_arg_ratio.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/dependent_col_fn_arg_summands_weights.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/dependent_col_fn_arg_summands_weights.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/dependent_col_fn_arg_weighted_const_sum.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/dependent_col_fn_arg_weighted_const_sum.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/dependent_col_fn_arg_weighted_ratio.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/dependent_col_fn_arg_weighted_ratio.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/dependent_col_fn_arg_zero_if_zero.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/dependent_col_fn_arg_zero_if_zero.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/dependent_col_fn_arg_zero_if_zero_all_of.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/dependent_col_fn_arg_zero_if_zero_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/dependent_columns.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/dependent_columns.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/dimensionality_reduction_request.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/dimensionality_reduction_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/dimensionality_reduction_response.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/dimensionality_reduction_response.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/dr_dataset_reduction_data.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/dr_dataset_reduction_data.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/dr_dataset_reduction_metadata.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/dr_dataset_reduction_metadata.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/dr_dataset_reduction_metadata_sources.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/dr_dataset_reduction_metadata_sources.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/dr_job_reduction_metadata.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/dr_job_reduction_metadata.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/dr_job_reduction_metadata_sources.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/dr_job_reduction_metadata_sources.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/dr_model_reduction_data.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/dr_model_reduction_data.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/dr_one_dimension_point.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/dr_one_dimension_point.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/dr_three_dimension_point.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/dr_three_dimension_point.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/dr_two_dimension_point.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/dr_two_dimension_point.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/drpca_reduction_type.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/drpca_reduction_type.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/drumap_reduction_type.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/drumap_reduction_type.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/empty_categorical_column.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/empty_categorical_column.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/empty_continuous_column.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/empty_continuous_column.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/error.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/error.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_all_opt_jobs.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_all_opt_jobs.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_optimize_done.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_optimize_done.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_optimize_done_all_of.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_optimize_done_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_optimize_failed.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_optimize_failed.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_optimize_failed_all_of.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_optimize_failed_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_optimize_optimizing.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_optimize_optimizing.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_optimize_optimizing_all_of.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_optimize_optimizing_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_optimize_pending.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_optimize_pending.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_optimize_pending_all_of.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_optimize_pending_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_suggest_additional_done.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_suggest_additional_done.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_suggest_additional_done_all_of.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_suggest_additional_done_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_suggest_additional_failed.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_suggest_additional_failed.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_suggest_additional_failed_all_of.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_suggest_additional_failed_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_suggest_additional_pending.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_suggest_additional_pending.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_suggest_additional_pending_all_of.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_suggest_additional_pending_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_suggest_additional_running.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_suggest_additional_running.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_suggest_additional_running_all_of.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_suggest_additional_running_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_suggest_historic_done.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_suggest_historic_done.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_suggest_historic_done_all_of.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_suggest_historic_done_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_suggest_historic_failed.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_suggest_historic_failed.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_suggest_historic_pending.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_suggest_historic_pending.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_suggest_historic_running.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_suggest_historic_running.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_suggest_initial_done.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_suggest_initial_done.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_suggest_initial_done_all_of.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_suggest_initial_done_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_suggest_initial_failed.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_suggest_initial_failed.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_suggest_initial_failed_all_of.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_suggest_initial_failed_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_suggest_initial_pending.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_suggest_initial_pending.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/get_suggest_initial_running.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/get_suggest_initial_running.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/historic_categorical_prediction.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/historic_categorical_prediction.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/historic_prediction.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/historic_prediction.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/historic_scalar_prediction.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/historic_scalar_prediction.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/historic_target_function.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/historic_target_function.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/historic_value.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/historic_value.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/historic_vector_prediction.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/historic_vector_prediction.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/historic_vector_value.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/historic_vector_value.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/importance_request.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/importance_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/impute_request.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/impute_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/int_cat_arr.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/int_cat_arr.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/job_patch.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/job_patch.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/load_request.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/load_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/model.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/model.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/model_column_info.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/model_column_info.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/model_patch.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/model_patch.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/model_permitted_column_relationships.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/model_permitted_column_relationships.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/models_dataset_put_request.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/models_dataset_put_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/models_id_additive_sensitivity_origin.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/models_id_additive_sensitivity_origin.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/models_id_train_permitted_column_relationships.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/models_id_train_permitted_column_relationships.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/new_col_fn_arg_col.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/new_col_fn_arg_col.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/new_col_fn_arg_col_all_of.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/new_col_fn_arg_col_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/new_col_fn_arg_col_weights.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/new_col_fn_arg_col_weights.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/new_col_fn_arg_col_weights_all_of.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/new_col_fn_arg_col_weights_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/new_col_fn_arg_col_weights_all_of_arguments.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/new_col_fn_arg_col_weights_all_of_arguments.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/new_col_fn_arg_constant_sum.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/new_col_fn_arg_constant_sum.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/new_col_fn_arg_constant_sum_all_of.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/new_col_fn_arg_constant_sum_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/new_col_fn_arg_constant_sum_all_of_arguments.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/new_col_fn_arg_constant_sum_all_of_arguments.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/new_col_fn_arg_product.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/new_col_fn_arg_product.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/new_col_fn_arg_product_all_of.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/new_col_fn_arg_product_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/new_col_fn_arg_product_all_of_arguments.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/new_col_fn_arg_product_all_of_arguments.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/new_col_fn_arg_ratio.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/new_col_fn_arg_ratio.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/new_col_fn_arg_ratio_all_of.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/new_col_fn_arg_ratio_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/new_col_fn_arg_summands_weights.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/new_col_fn_arg_summands_weights.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/new_col_fn_arg_summands_weights_all_of.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/new_col_fn_arg_summands_weights_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/new_col_fn_arg_summands_weights_all_of_arguments.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/new_col_fn_arg_summands_weights_all_of_arguments.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/new_col_fn_arg_weighted_const_sum.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/new_col_fn_arg_weighted_const_sum.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/new_col_fn_arg_weighted_const_sum_all_of.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/new_col_fn_arg_weighted_const_sum_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/new_col_fn_arg_weighted_const_sum_all_of_arguments.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/new_col_fn_arg_weighted_const_sum_all_of_arguments.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/new_col_fn_arg_weighted_ratio.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/new_col_fn_arg_weighted_ratio.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/new_col_fn_arg_weighted_ratio_all_of.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/new_col_fn_arg_weighted_ratio_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/new_col_fn_arg_weighted_ratio_all_of_arguments.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/new_col_fn_arg_weighted_ratio_all_of_arguments.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/new_col_fn_arg_zero_if_zero.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/new_col_fn_arg_zero_if_zero.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/new_col_fn_arg_zero_if_zero_all_of.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/new_col_fn_arg_zero_if_zero_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/new_columns.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/new_columns.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/non_empty_categorical_column.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/non_empty_categorical_column.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/non_empty_continuous_column.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/non_empty_continuous_column.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/non_empty_integer_categorical_column.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/non_empty_integer_categorical_column.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/optimize_request.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/optimize_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/ot_sample_def_categorical.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/ot_sample_def_categorical.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/ot_sample_def_continuous.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/ot_sample_def_continuous.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/ot_sample_definition.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/ot_sample_definition.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/ot_set_inputs.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/ot_set_inputs.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/outliers_request.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/outliers_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/output_tolerance_request.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/output_tolerance_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/output_tolerance_response.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/output_tolerance_response.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/output_tolerance_response_fixed_inputs.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/output_tolerance_response_fixed_inputs.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/output_tolerance_response_predicted_outputs.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/output_tolerance_response_predicted_outputs.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/output_tolerance_response_predictions.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/output_tolerance_response_predictions.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/output_tolerance_response_sampled_inputs.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/output_tolerance_response_sampled_inputs.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/part_dependent_columns.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/part_dependent_columns.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/part_get_optimize.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/part_get_optimize.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/part_get_optimize_done_result_array.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/part_get_optimize_done_result_array.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/part_get_suggest_additional.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/part_get_suggest_additional.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/part_get_suggest_historic.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/part_get_suggest_historic.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/part_get_suggest_initial.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/part_get_suggest_initial.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/part_new_columns.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/part_new_columns.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/part_tar_fn_above.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/part_tar_fn_above.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/part_tar_fn_below.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/part_tar_fn_below.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/part_tar_fn_between.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/part_tar_fn_between.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/part_tar_fn_categoricals.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/part_tar_fn_categoricals.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/part_tar_fn_single_tar.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/part_tar_fn_single_tar.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/part_tar_fn_sum.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/part_tar_fn_sum.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/part_tar_fn_weighted_sum.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/part_tar_fn_weighted_sum.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/predict_request.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/predict_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/prediction.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/prediction.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/query_request.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/query_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/query_response.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/query_response.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/sample_def_categorical.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/sample_def_categorical.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/sample_def_categorical_column_values.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/sample_def_categorical_column_values.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/sample_def_composition.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/sample_def_composition.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,28 +85,30 @@
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'type': (str,),  # noqa: E501
             'values': ({str: (SampleDefContinuous,)},),  # noqa: E501
             'total': (float,),  # noqa: E501
+            'total_range': ([float],),  # noqa: E501
             'min': (int,),  # noqa: E501
             'max': (int,),  # noqa: E501
             'hard_limit': (bool,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():  # noqa
         return None
 
 
     attribute_map = {
         'type': 'type',  # noqa: E501
         'values': 'values',  # noqa: E501
         'total': 'total',  # noqa: E501
+        'total_range': 'totalRange',  # noqa: E501
         'min': 'min',  # noqa: E501
         'max': 'max',  # noqa: E501
         'hard_limit': 'hardLimit',  # noqa: E501
     }
 
     read_only_vars = {
     }
@@ -145,15 +147,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            total (float): The value the columns defined in `values` should sum up to. If not specified, then no total constraint will be applied.. [optional]  # noqa: E501
+            total (float): The value the columns defined in `values` should sum up to. If not specified, then no total constraint will be applied. Cannot be used in conjunction with totalRange.. [optional]  # noqa: E501
+            total_range ([float]): The value the columns defined in `values` should sum between. If not specified, then no totalRange constraint will be applied. Cannot be used in conjunction with total.. [optional]  # noqa: E501
             min (int): The minimum columns defined in `values` to be non-zero.. [optional] if omitted the server will use the default value of 0  # noqa: E501
             max (int): The maximum columns defined in `values` to be non-zero. If not specified, it will default to the number of properties in `values`. [optional]  # noqa: E501
             hard_limit (bool): Whether min/max are strictly enforced. Unused if no min or max set. . [optional] if omitted the server will use the default value of False  # noqa: E501
         """
 
         type = kwargs.get('type', "composition")
         _check_type = kwargs.pop('_check_type', True)
@@ -251,15 +254,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            total (float): The value the columns defined in `values` should sum up to. If not specified, then no total constraint will be applied.. [optional]  # noqa: E501
+            total (float): The value the columns defined in `values` should sum up to. If not specified, then no total constraint will be applied. Cannot be used in conjunction with totalRange.. [optional]  # noqa: E501
+            total_range ([float]): The value the columns defined in `values` should sum between. If not specified, then no totalRange constraint will be applied. Cannot be used in conjunction with total.. [optional]  # noqa: E501
             min (int): The minimum columns defined in `values` to be non-zero.. [optional] if omitted the server will use the default value of 0  # noqa: E501
             max (int): The maximum columns defined in `values` to be non-zero. If not specified, it will default to the number of properties in `values`. [optional]  # noqa: E501
             hard_limit (bool): Whether min/max are strictly enforced. Unused if no min or max set. . [optional] if omitted the server will use the default value of False  # noqa: E501
         """
 
         type = kwargs.get('type', "composition")
         _check_type = kwargs.pop('_check_type', True)
```

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/sample_def_composition_all_of.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/tar_fn_sum_above.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,19 +25,23 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from alchemite_apiclient.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from alchemite_apiclient.model.sample_def_continuous import SampleDefContinuous
-    globals()['SampleDefContinuous'] = SampleDefContinuous
+    from alchemite_apiclient.model.part_tar_fn_above import PartTarFnAbove
+    from alchemite_apiclient.model.part_tar_fn_sum import PartTarFnSum
+    from alchemite_apiclient.model.tar_fn_sum_above_all_of import TarFnSumAboveAllOf
+    globals()['PartTarFnAbove'] = PartTarFnAbove
+    globals()['PartTarFnSum'] = PartTarFnSum
+    globals()['TarFnSumAboveAllOf'] = TarFnSumAboveAllOf
 
 
-class SampleDefCompositionAllOf(ModelNormal):
+class TarFnSumAbove(ModelComposed):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -53,32 +57,17 @@
           that stores validations for max_length, min_length, max_items,
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
-    allowed_values = {
-        ('type',): {
-            'COMPOSITION': "composition",
-        },
-    }
+    allowed_values = {}
 
-    validations = {
-        ('values',): {
-            'min_properties': 2,
-            'min_items': 2,
-        },
-        ('min',): {
-            'inclusive_minimum': 0,
-        },
-        ('max',): {
-            'inclusive_minimum': 0,
-        },
-    }
+    validations = {}
 
     @cached_property
     def additional_properties_type():  # noqa
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
@@ -95,51 +84,44 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
+            'minimum': (float,),  # noqa: E501
+            'targets': ([str],),  # noqa: E501
             'type': (str,),  # noqa: E501
-            'values': ({str: (SampleDefContinuous,)},),  # noqa: E501
-            'total': (float,),  # noqa: E501
-            'min': (int,),  # noqa: E501
-            'max': (int,),  # noqa: E501
-            'hard_limit': (bool,),  # noqa: E501
+            'importance': (float,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():  # noqa
         return None
 
 
     attribute_map = {
+        'minimum': 'minimum',  # noqa: E501
+        'targets': 'targets',  # noqa: E501
         'type': 'type',  # noqa: E501
-        'values': 'values',  # noqa: E501
-        'total': 'total',  # noqa: E501
-        'min': 'min',  # noqa: E501
-        'max': 'max',  # noqa: E501
-        'hard_limit': 'hardLimit',  # noqa: E501
+        'importance': 'importance',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
-    _composed_schemas = {}
-
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, values, *args, **kwargs):  # noqa: E501
-        """SampleDefCompositionAllOf - a model defined in OpenAPI
-
-        Args:
-            values ({str: (SampleDefContinuous,)}): Define the continuous columns and their ranges. Sum of lower bound values must be less than or equal to `total`. Sum of upper bound values must be greater than or equal to `total`. Columns defined here cannot be defined in another sampleDefinition type. 
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """TarFnSumAbove - a model defined in OpenAPI
 
         Keyword Args:
-            type (str): Constrain two or more columns to sum up to `total`. Only supported for global optimization methods. . defaults to "composition", must be one of ["composition", ]  # noqa: E501
+            minimum (float):
+            targets ([str]): Array of columns names to sum
+            type (str): Find a solution where the sum of the given columns is above `\"minimum\"`.. defaults to "sum above", must be one of ["sum above", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -162,21 +144,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            total (float): The value the columns defined in `values` should sum up to. If not specified, then no total constraint will be applied.. [optional]  # noqa: E501
-            min (int): The minimum columns defined in `values` to be non-zero.. [optional] if omitted the server will use the default value of 0  # noqa: E501
-            max (int): The maximum columns defined in `values` to be non-zero. If not specified, it will default to the number of properties in `values`. [optional]  # noqa: E501
-            hard_limit (bool): Whether min/max are strictly enforced. Unused if no min or max set. . [optional] if omitted the server will use the default value of False  # noqa: E501
+            importance (float): The higher the value the higher the importance of this target.  If the importance values all equal 1 then the `probabilityOfSuccess` is a true probability (the probability of all the targets being satisfied, assuming that the probability of any individual target being satisfied is independent of the others).  Note, having many targets or importance numbers > 1 can make the `probabilityOfSuccess` very small, even if most of the targets are individually likely to be met. If there are many targets it may be helpful to make the importance values all add up to 1. This will make the `probabilityOfSuccess` scale with the number of columns so that it becomes a more natural-looking \"score\" of how likely the targets are to be met. For example, the reported `probabilityOfSuccess` of achieving one target with probability 50% is the same as achieving two targets, each with probability 50% and importance 0.5. . [optional] if omitted the server will use the default value of 1  # noqa: E501
         """
 
-        type = kwargs.get('type', "composition")
+        type = kwargs.get('type', "sum above")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         self = super(OpenApiModel, cls).__new__(cls)
@@ -194,44 +173,59 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.type = type
-        self.values = values
+        constant_args = {
+            '_check_type': _check_type,
+            '_path_to_item': _path_to_item,
+            '_spec_property_naming': _spec_property_naming,
+            '_configuration': _configuration,
+            '_visited_composed_classes': self._visited_composed_classes,
+        }
+        composed_info = validate_get_composed_info(
+            constant_args, kwargs, self)
+        self._composed_instances = composed_info[0]
+        self._var_name_to_model_instances = composed_info[1]
+        self._additional_properties_model_instances = composed_info[2]
+        discarded_args = composed_info[3]
+
         for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
+            if var_name in discarded_args and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
+                        self._additional_properties_model_instances:
                 # discard variable.
                 continue
             setattr(self, var_name, var_value)
+
         return self
 
     required_properties = set([
         '_data_store',
         '_check_type',
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
+        '_composed_instances',
+        '_var_name_to_model_instances',
+        '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, values, *args, **kwargs):  # noqa: E501
-        """SampleDefCompositionAllOf - a model defined in OpenAPI
-
-        Args:
-            values ({str: (SampleDefContinuous,)}): Define the continuous columns and their ranges. Sum of lower bound values must be less than or equal to `total`. Sum of upper bound values must be greater than or equal to `total`. Columns defined here cannot be defined in another sampleDefinition type. 
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """TarFnSumAbove - a model defined in OpenAPI
 
         Keyword Args:
-            type (str): Constrain two or more columns to sum up to `total`. Only supported for global optimization methods. . defaults to "composition", must be one of ["composition", ]  # noqa: E501
+            minimum (float):
+            targets ([str]): Array of columns names to sum
+            type (str): Find a solution where the sum of the given columns is above `\"minimum\"`.. defaults to "sum above", must be one of ["sum above", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -254,21 +248,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            total (float): The value the columns defined in `values` should sum up to. If not specified, then no total constraint will be applied.. [optional]  # noqa: E501
-            min (int): The minimum columns defined in `values` to be non-zero.. [optional] if omitted the server will use the default value of 0  # noqa: E501
-            max (int): The maximum columns defined in `values` to be non-zero. If not specified, it will default to the number of properties in `values`. [optional]  # noqa: E501
-            hard_limit (bool): Whether min/max are strictly enforced. Unused if no min or max set. . [optional] if omitted the server will use the default value of False  # noqa: E501
+            importance (float): The higher the value the higher the importance of this target.  If the importance values all equal 1 then the `probabilityOfSuccess` is a true probability (the probability of all the targets being satisfied, assuming that the probability of any individual target being satisfied is independent of the others).  Note, having many targets or importance numbers > 1 can make the `probabilityOfSuccess` very small, even if most of the targets are individually likely to be met. If there are many targets it may be helpful to make the importance values all add up to 1. This will make the `probabilityOfSuccess` scale with the number of columns so that it becomes a more natural-looking \"score\" of how likely the targets are to be met. For example, the reported `probabilityOfSuccess` of achieving one target with probability 50% is the same as achieving two targets, each with probability 50% and importance 0.5. . [optional] if omitted the server will use the default value of 1  # noqa: E501
         """
 
-        type = kwargs.get('type', "composition")
+        type = kwargs.get('type', "sum above")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
@@ -284,20 +275,54 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.type = type
-        self.values = values
+        constant_args = {
+            '_check_type': _check_type,
+            '_path_to_item': _path_to_item,
+            '_spec_property_naming': _spec_property_naming,
+            '_configuration': _configuration,
+            '_visited_composed_classes': self._visited_composed_classes,
+        }
+        composed_info = validate_get_composed_info(
+            constant_args, kwargs, self)
+        self._composed_instances = composed_info[0]
+        self._var_name_to_model_instances = composed_info[1]
+        self._additional_properties_model_instances = composed_info[2]
+        discarded_args = composed_info[3]
+
         for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
+            if var_name in discarded_args and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
+                        self._additional_properties_model_instances:
                 # discard variable.
                 continue
             setattr(self, var_name, var_value)
             if var_name in self.read_only_vars:
                 raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
                                      f"class with read only attributes.")
+
+    @cached_property
+    def _composed_schemas():
+        # we need this here to make our import statements work
+        # we must store _composed_schemas in here so the code is only run
+        # when we invoke this method. If we kept this at the class
+        # level we would get an error because the class level
+        # code would be run when this module is imported, and these composed
+        # classes don't exist yet because their module has not finished
+        # loading
+        lazy_import()
+        return {
+          'anyOf': [
+          ],
+          'allOf': [
+              PartTarFnAbove,
+              PartTarFnSum,
+              TarFnSumAboveAllOf,
+          ],
+          'oneOf': [
+          ],
+        }
```

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/sample_def_continuous.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/sample_def_continuous.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/sample_def_continuous_with_start.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/sample_def_continuous_with_start.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/sample_def_discrete.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/sample_def_discrete.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/sample_def_integer.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/sample_def_integer.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/sample_def_start_prop.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/sample_def_start_prop.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/sample_def_weighted_categorical.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/sample_def_weighted_categorical.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/sample_definition.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/sample_definition.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/scalar_prediction.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/scalar_prediction.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/scalar_result.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/scalar_result.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/sensitivity_request.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/sensitivity_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/set_inputs.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/set_inputs.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/share_group.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/share_group.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/si_sample_def_categorical.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/si_sample_def_categorical.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/si_sample_def_categorical_column_values.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/si_sample_def_categorical_column_values.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/si_sample_def_continuous.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/si_sample_def_continuous.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/si_sample_definition.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/si_sample_definition.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/string_cat_arr.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/string_cat_arr.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/suggest_additional_parameters.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/suggest_additional_parameters.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/suggest_additional_parameters_all_of.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/suggest_additional_parameters_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/suggest_additional_request.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/suggest_additional_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/suggest_additional_request_all_of.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/suggest_additional_request_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/suggest_additional_result.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/suggest_additional_result.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/suggest_historic_parameters.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/suggest_historic_parameters.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/suggest_historic_request.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/suggest_historic_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/suggest_historic_result.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/suggest_historic_result.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/suggest_historic_result_samples.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/suggest_historic_result_samples.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/suggest_initial_parameters.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/suggest_initial_parameters.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/suggest_initial_request.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/suggest_initial_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/suggest_initial_request_all_of.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/suggest_initial_request_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/suggest_initial_response.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/suggest_initial_response.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/suggest_initial_result.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/suggest_initial_result.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/suggest_missing_common.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/suggest_missing_common.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/suggest_missing_data.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/suggest_missing_data.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/suggest_missing_data_all_of.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/suggest_missing_data_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/suggest_missing_dataset_id.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/suggest_missing_dataset_id.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/suggest_missing_dataset_id_all_of.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/suggest_missing_dataset_id_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/suggest_missing_imputed_data.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/suggest_missing_imputed_data.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/suggest_missing_imputed_data_all_of.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/suggest_missing_imputed_data_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/suggest_missing_request.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/suggest_missing_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/suggest_missing_response.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/suggest_missing_response.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/suggest_missing_specific.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/suggest_missing_specific.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/tar_fn_above.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/tar_fn_above.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/tar_fn_above_all_of.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/tar_fn_above_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/tar_fn_below.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/tar_fn_below.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/tar_fn_below_all_of.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/tar_fn_below_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/tar_fn_between.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/tar_fn_between.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/tar_fn_between_all_of.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/tar_fn_between_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/tar_fn_exclude_categories.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/tar_fn_exclude_categories.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/tar_fn_exclude_categories_all_of.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/tar_fn_exclude_categories_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/tar_fn_include_categories.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/tar_fn_include_categories.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/tar_fn_include_categories_all_of.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/tar_fn_include_categories_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/tar_fn_sum_above.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/tar_fn_sum_between.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,23 +25,23 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from alchemite_apiclient.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from alchemite_apiclient.model.part_tar_fn_above import PartTarFnAbove
+    from alchemite_apiclient.model.part_tar_fn_between import PartTarFnBetween
     from alchemite_apiclient.model.part_tar_fn_sum import PartTarFnSum
-    from alchemite_apiclient.model.tar_fn_sum_above_all_of import TarFnSumAboveAllOf
-    globals()['PartTarFnAbove'] = PartTarFnAbove
+    from alchemite_apiclient.model.tar_fn_sum_between_all_of import TarFnSumBetweenAllOf
+    globals()['PartTarFnBetween'] = PartTarFnBetween
     globals()['PartTarFnSum'] = PartTarFnSum
-    globals()['TarFnSumAboveAllOf'] = TarFnSumAboveAllOf
+    globals()['TarFnSumBetweenAllOf'] = TarFnSumBetweenAllOf
 
 
-class TarFnSumAbove(ModelComposed):
+class TarFnSumBetween(ModelComposed):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -84,44 +84,47 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
+            'maximum': (float,),  # noqa: E501
             'minimum': (float,),  # noqa: E501
             'targets': ([str],),  # noqa: E501
             'type': (str,),  # noqa: E501
             'importance': (float,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():  # noqa
         return None
 
 
     attribute_map = {
+        'maximum': 'maximum',  # noqa: E501
         'minimum': 'minimum',  # noqa: E501
         'targets': 'targets',  # noqa: E501
         'type': 'type',  # noqa: E501
         'importance': 'importance',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TarFnSumAbove - a model defined in OpenAPI
+        """TarFnSumBetween - a model defined in OpenAPI
 
         Keyword Args:
+            maximum (float):
             minimum (float):
             targets ([str]): Array of columns names to sum
-            type (str): Find a solution where the sum of the given columns is above `\"minimum\"`.. defaults to "sum above", must be one of ["sum above", ]  # noqa: E501
+            type (str): Find a solution where the sum of the given columns is between `\"minimum\"` and `\"maximum\"`.. defaults to "sum between", must be one of ["sum between", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -147,15 +150,15 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             importance (float): The higher the value the higher the importance of this target.  If the importance values all equal 1 then the `probabilityOfSuccess` is a true probability (the probability of all the targets being satisfied, assuming that the probability of any individual target being satisfied is independent of the others).  Note, having many targets or importance numbers > 1 can make the `probabilityOfSuccess` very small, even if most of the targets are individually likely to be met. If there are many targets it may be helpful to make the importance values all add up to 1. This will make the `probabilityOfSuccess` scale with the number of columns so that it becomes a more natural-looking \"score\" of how likely the targets are to be met. For example, the reported `probabilityOfSuccess` of achieving one target with probability 50% is the same as achieving two targets, each with probability 50% and importance 0.5. . [optional] if omitted the server will use the default value of 1  # noqa: E501
         """
 
-        type = kwargs.get('type', "sum above")
+        type = kwargs.get('type', "sum between")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         self = super(OpenApiModel, cls).__new__(cls)
@@ -212,20 +215,21 @@
         '_composed_instances',
         '_var_name_to_model_instances',
         '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TarFnSumAbove - a model defined in OpenAPI
+        """TarFnSumBetween - a model defined in OpenAPI
 
         Keyword Args:
+            maximum (float):
             minimum (float):
             targets ([str]): Array of columns names to sum
-            type (str): Find a solution where the sum of the given columns is above `\"minimum\"`.. defaults to "sum above", must be one of ["sum above", ]  # noqa: E501
+            type (str): Find a solution where the sum of the given columns is between `\"minimum\"` and `\"maximum\"`.. defaults to "sum between", must be one of ["sum between", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -251,15 +255,15 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             importance (float): The higher the value the higher the importance of this target.  If the importance values all equal 1 then the `probabilityOfSuccess` is a true probability (the probability of all the targets being satisfied, assuming that the probability of any individual target being satisfied is independent of the others).  Note, having many targets or importance numbers > 1 can make the `probabilityOfSuccess` very small, even if most of the targets are individually likely to be met. If there are many targets it may be helpful to make the importance values all add up to 1. This will make the `probabilityOfSuccess` scale with the number of columns so that it becomes a more natural-looking \"score\" of how likely the targets are to be met. For example, the reported `probabilityOfSuccess` of achieving one target with probability 50% is the same as achieving two targets, each with probability 50% and importance 0.5. . [optional] if omitted the server will use the default value of 1  # noqa: E501
         """
 
-        type = kwargs.get('type', "sum above")
+        type = kwargs.get('type', "sum between")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
@@ -315,14 +319,14 @@
         # classes don't exist yet because their module has not finished
         # loading
         lazy_import()
         return {
           'anyOf': [
           ],
           'allOf': [
-              PartTarFnAbove,
+              PartTarFnBetween,
               PartTarFnSum,
-              TarFnSumAboveAllOf,
+              TarFnSumBetweenAllOf,
           ],
           'oneOf': [
           ],
         }
```

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/tar_fn_sum_above_all_of.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/tar_fn_sum_above_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/tar_fn_sum_below.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/tar_fn_sum_below.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/tar_fn_sum_below_all_of.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/tar_fn_sum_below_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/tar_fn_sum_between.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/tar_fn_weighted_sum_below.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,23 +25,23 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from alchemite_apiclient.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from alchemite_apiclient.model.part_tar_fn_between import PartTarFnBetween
-    from alchemite_apiclient.model.part_tar_fn_sum import PartTarFnSum
-    from alchemite_apiclient.model.tar_fn_sum_between_all_of import TarFnSumBetweenAllOf
-    globals()['PartTarFnBetween'] = PartTarFnBetween
-    globals()['PartTarFnSum'] = PartTarFnSum
-    globals()['TarFnSumBetweenAllOf'] = TarFnSumBetweenAllOf
+    from alchemite_apiclient.model.part_tar_fn_below import PartTarFnBelow
+    from alchemite_apiclient.model.part_tar_fn_weighted_sum import PartTarFnWeightedSum
+    from alchemite_apiclient.model.tar_fn_weighted_sum_below_all_of import TarFnWeightedSumBelowAllOf
+    globals()['PartTarFnBelow'] = PartTarFnBelow
+    globals()['PartTarFnWeightedSum'] = PartTarFnWeightedSum
+    globals()['TarFnWeightedSumBelowAllOf'] = TarFnWeightedSumBelowAllOf
 
 
-class TarFnSumBetween(ModelComposed):
+class TarFnWeightedSumBelow(ModelComposed):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -85,46 +85,43 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'maximum': (float,),  # noqa: E501
-            'minimum': (float,),  # noqa: E501
-            'targets': ([str],),  # noqa: E501
+            'targets': ({str: (float,)},),  # noqa: E501
             'type': (str,),  # noqa: E501
             'importance': (float,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():  # noqa
         return None
 
 
     attribute_map = {
         'maximum': 'maximum',  # noqa: E501
-        'minimum': 'minimum',  # noqa: E501
         'targets': 'targets',  # noqa: E501
         'type': 'type',  # noqa: E501
         'importance': 'importance',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TarFnSumBetween - a model defined in OpenAPI
+        """TarFnWeightedSumBelow - a model defined in OpenAPI
 
         Keyword Args:
             maximum (float):
-            minimum (float):
-            targets ([str]): Array of columns names to sum
-            type (str): Find a solution where the sum of the given columns is between `\"minimum\"` and `\"maximum\"`.. defaults to "sum between", must be one of ["sum between", ]  # noqa: E501
+            targets ({str: (float,)}):
+            type (str): Find a solution where the weighted sum of the given columns is below `\"maximum\"`.. defaults to "weighted sum below", must be one of ["weighted sum below", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -150,15 +147,15 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             importance (float): The higher the value the higher the importance of this target.  If the importance values all equal 1 then the `probabilityOfSuccess` is a true probability (the probability of all the targets being satisfied, assuming that the probability of any individual target being satisfied is independent of the others).  Note, having many targets or importance numbers > 1 can make the `probabilityOfSuccess` very small, even if most of the targets are individually likely to be met. If there are many targets it may be helpful to make the importance values all add up to 1. This will make the `probabilityOfSuccess` scale with the number of columns so that it becomes a more natural-looking \"score\" of how likely the targets are to be met. For example, the reported `probabilityOfSuccess` of achieving one target with probability 50% is the same as achieving two targets, each with probability 50% and importance 0.5. . [optional] if omitted the server will use the default value of 1  # noqa: E501
         """
 
-        type = kwargs.get('type', "sum between")
+        type = kwargs.get('type', "weighted sum below")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         self = super(OpenApiModel, cls).__new__(cls)
@@ -215,21 +212,20 @@
         '_composed_instances',
         '_var_name_to_model_instances',
         '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TarFnSumBetween - a model defined in OpenAPI
+        """TarFnWeightedSumBelow - a model defined in OpenAPI
 
         Keyword Args:
             maximum (float):
-            minimum (float):
-            targets ([str]): Array of columns names to sum
-            type (str): Find a solution where the sum of the given columns is between `\"minimum\"` and `\"maximum\"`.. defaults to "sum between", must be one of ["sum between", ]  # noqa: E501
+            targets ({str: (float,)}):
+            type (str): Find a solution where the weighted sum of the given columns is below `\"maximum\"`.. defaults to "weighted sum below", must be one of ["weighted sum below", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -255,15 +251,15 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             importance (float): The higher the value the higher the importance of this target.  If the importance values all equal 1 then the `probabilityOfSuccess` is a true probability (the probability of all the targets being satisfied, assuming that the probability of any individual target being satisfied is independent of the others).  Note, having many targets or importance numbers > 1 can make the `probabilityOfSuccess` very small, even if most of the targets are individually likely to be met. If there are many targets it may be helpful to make the importance values all add up to 1. This will make the `probabilityOfSuccess` scale with the number of columns so that it becomes a more natural-looking \"score\" of how likely the targets are to be met. For example, the reported `probabilityOfSuccess` of achieving one target with probability 50% is the same as achieving two targets, each with probability 50% and importance 0.5. . [optional] if omitted the server will use the default value of 1  # noqa: E501
         """
 
-        type = kwargs.get('type', "sum between")
+        type = kwargs.get('type', "weighted sum below")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
@@ -319,14 +315,14 @@
         # classes don't exist yet because their module has not finished
         # loading
         lazy_import()
         return {
           'anyOf': [
           ],
           'allOf': [
-              PartTarFnBetween,
-              PartTarFnSum,
-              TarFnSumBetweenAllOf,
+              PartTarFnBelow,
+              PartTarFnWeightedSum,
+              TarFnWeightedSumBelowAllOf,
           ],
           'oneOf': [
           ],
         }
```

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/tar_fn_sum_between_all_of.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/tar_fn_sum_between_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/tar_fn_weighted_sum_above.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/tar_fn_weighted_sum_above.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/tar_fn_weighted_sum_above_all_of.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/tar_fn_weighted_sum_above_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/tar_fn_weighted_sum_below.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/tar_fn_weighted_sum_between.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,23 +25,23 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from alchemite_apiclient.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from alchemite_apiclient.model.part_tar_fn_below import PartTarFnBelow
+    from alchemite_apiclient.model.part_tar_fn_between import PartTarFnBetween
     from alchemite_apiclient.model.part_tar_fn_weighted_sum import PartTarFnWeightedSum
-    from alchemite_apiclient.model.tar_fn_weighted_sum_below_all_of import TarFnWeightedSumBelowAllOf
-    globals()['PartTarFnBelow'] = PartTarFnBelow
+    from alchemite_apiclient.model.tar_fn_weighted_sum_between_all_of import TarFnWeightedSumBetweenAllOf
+    globals()['PartTarFnBetween'] = PartTarFnBetween
     globals()['PartTarFnWeightedSum'] = PartTarFnWeightedSum
-    globals()['TarFnWeightedSumBelowAllOf'] = TarFnWeightedSumBelowAllOf
+    globals()['TarFnWeightedSumBetweenAllOf'] = TarFnWeightedSumBetweenAllOf
 
 
-class TarFnWeightedSumBelow(ModelComposed):
+class TarFnWeightedSumBetween(ModelComposed):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -85,43 +85,46 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'maximum': (float,),  # noqa: E501
+            'minimum': (float,),  # noqa: E501
             'targets': ({str: (float,)},),  # noqa: E501
             'type': (str,),  # noqa: E501
             'importance': (float,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():  # noqa
         return None
 
 
     attribute_map = {
         'maximum': 'maximum',  # noqa: E501
+        'minimum': 'minimum',  # noqa: E501
         'targets': 'targets',  # noqa: E501
         'type': 'type',  # noqa: E501
         'importance': 'importance',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TarFnWeightedSumBelow - a model defined in OpenAPI
+        """TarFnWeightedSumBetween - a model defined in OpenAPI
 
         Keyword Args:
             maximum (float):
+            minimum (float):
             targets ({str: (float,)}):
-            type (str): Find a solution where the weighted sum of the given columns is below `\"maximum\"`.. defaults to "weighted sum below", must be one of ["weighted sum below", ]  # noqa: E501
+            type (str): Find a solution where the weighted sum of the given columns is between `\"minimum\"` and `\"maximum\"`.. defaults to "weighted sum between", must be one of ["weighted sum between", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -147,15 +150,15 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             importance (float): The higher the value the higher the importance of this target.  If the importance values all equal 1 then the `probabilityOfSuccess` is a true probability (the probability of all the targets being satisfied, assuming that the probability of any individual target being satisfied is independent of the others).  Note, having many targets or importance numbers > 1 can make the `probabilityOfSuccess` very small, even if most of the targets are individually likely to be met. If there are many targets it may be helpful to make the importance values all add up to 1. This will make the `probabilityOfSuccess` scale with the number of columns so that it becomes a more natural-looking \"score\" of how likely the targets are to be met. For example, the reported `probabilityOfSuccess` of achieving one target with probability 50% is the same as achieving two targets, each with probability 50% and importance 0.5. . [optional] if omitted the server will use the default value of 1  # noqa: E501
         """
 
-        type = kwargs.get('type', "weighted sum below")
+        type = kwargs.get('type', "weighted sum between")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         self = super(OpenApiModel, cls).__new__(cls)
@@ -212,20 +215,21 @@
         '_composed_instances',
         '_var_name_to_model_instances',
         '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TarFnWeightedSumBelow - a model defined in OpenAPI
+        """TarFnWeightedSumBetween - a model defined in OpenAPI
 
         Keyword Args:
             maximum (float):
+            minimum (float):
             targets ({str: (float,)}):
-            type (str): Find a solution where the weighted sum of the given columns is below `\"maximum\"`.. defaults to "weighted sum below", must be one of ["weighted sum below", ]  # noqa: E501
+            type (str): Find a solution where the weighted sum of the given columns is between `\"minimum\"` and `\"maximum\"`.. defaults to "weighted sum between", must be one of ["weighted sum between", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -251,15 +255,15 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             importance (float): The higher the value the higher the importance of this target.  If the importance values all equal 1 then the `probabilityOfSuccess` is a true probability (the probability of all the targets being satisfied, assuming that the probability of any individual target being satisfied is independent of the others).  Note, having many targets or importance numbers > 1 can make the `probabilityOfSuccess` very small, even if most of the targets are individually likely to be met. If there are many targets it may be helpful to make the importance values all add up to 1. This will make the `probabilityOfSuccess` scale with the number of columns so that it becomes a more natural-looking \"score\" of how likely the targets are to be met. For example, the reported `probabilityOfSuccess` of achieving one target with probability 50% is the same as achieving two targets, each with probability 50% and importance 0.5. . [optional] if omitted the server will use the default value of 1  # noqa: E501
         """
 
-        type = kwargs.get('type', "weighted sum below")
+        type = kwargs.get('type', "weighted sum between")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
@@ -315,14 +319,14 @@
         # classes don't exist yet because their module has not finished
         # loading
         lazy_import()
         return {
           'anyOf': [
           ],
           'allOf': [
-              PartTarFnBelow,
+              PartTarFnBetween,
               PartTarFnWeightedSum,
-              TarFnWeightedSumBelowAllOf,
+              TarFnWeightedSumBetweenAllOf,
           ],
           'oneOf': [
           ],
         }
```

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/tar_fn_weighted_sum_below_all_of.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/tar_fn_weighted_sum_below_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/tar_fn_weighted_sum_between.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/validate_request.py`

 * *Files 22% similar despite different names*

```diff
@@ -24,24 +24,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from alchemite_apiclient.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from alchemite_apiclient.model.part_tar_fn_between import PartTarFnBetween
-    from alchemite_apiclient.model.part_tar_fn_weighted_sum import PartTarFnWeightedSum
-    from alchemite_apiclient.model.tar_fn_weighted_sum_between_all_of import TarFnWeightedSumBetweenAllOf
-    globals()['PartTarFnBetween'] = PartTarFnBetween
-    globals()['PartTarFnWeightedSum'] = PartTarFnWeightedSum
-    globals()['TarFnWeightedSumBetweenAllOf'] = TarFnWeightedSumBetweenAllOf
 
-
-class TarFnWeightedSumBetween(ModelComposed):
+class ValidateRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -57,74 +49,66 @@
           that stores validations for max_length, min_length, max_items,
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
-    allowed_values = {}
+    allowed_values = {
+    }
 
-    validations = {}
+    validations = {
+    }
 
-    @cached_property
-    def additional_properties_type():  # noqa
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        lazy_import()
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+    additional_properties_type = None
 
     _nullable = False
 
     @cached_property
     def openapi_types():  # noqa
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'maximum': (float,),  # noqa: E501
-            'minimum': (float,),  # noqa: E501
-            'targets': ({str: (float,)},),  # noqa: E501
-            'type': (str,),  # noqa: E501
-            'importance': (float,),  # noqa: E501
+            'return_probability_distribution': (bool,),  # noqa: E501
+            'dataset_id': (str,),  # noqa: E501
+            'return_row_headers': (bool,),  # noqa: E501
+            'return_column_headers': (bool,),  # noqa: E501
+            'data': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():  # noqa
         return None
 
 
     attribute_map = {
-        'maximum': 'maximum',  # noqa: E501
-        'minimum': 'minimum',  # noqa: E501
-        'targets': 'targets',  # noqa: E501
-        'type': 'type',  # noqa: E501
-        'importance': 'importance',  # noqa: E501
+        'return_probability_distribution': 'returnProbabilityDistribution',  # noqa: E501
+        'dataset_id': 'datasetID',  # noqa: E501
+        'return_row_headers': 'returnRowHeaders',  # noqa: E501
+        'return_column_headers': 'returnColumnHeaders',  # noqa: E501
+        'data': 'data',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
+    _composed_schemas = {}
+
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TarFnWeightedSumBetween - a model defined in OpenAPI
+        """ValidateRequest - a model defined in OpenAPI
 
         Keyword Args:
-            maximum (float):
-            minimum (float):
-            targets ({str: (float,)}):
-            type (str): Find a solution where the weighted sum of the given columns is between `\"minimum\"` and `\"maximum\"`.. defaults to "weighted sum between", must be one of ["weighted sum between", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -147,18 +131,21 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            importance (float): The higher the value the higher the importance of this target.  If the importance values all equal 1 then the `probabilityOfSuccess` is a true probability (the probability of all the targets being satisfied, assuming that the probability of any individual target being satisfied is independent of the others).  Note, having many targets or importance numbers > 1 can make the `probabilityOfSuccess` very small, even if most of the targets are individually likely to be met. If there are many targets it may be helpful to make the importance values all add up to 1. This will make the `probabilityOfSuccess` scale with the number of columns so that it becomes a more natural-looking \"score\" of how likely the targets are to be met. For example, the reported `probabilityOfSuccess` of achieving one target with probability 50% is the same as achieving two targets, each with probability 50% and importance 0.5. . [optional] if omitted the server will use the default value of 1  # noqa: E501
+            return_probability_distribution (bool): If true then the full probability distribution for each prediction will be returned, if false then the predicted value and uncertainty derived from that distribution will be returned instead.. [optional] if omitted the server will use the default value of False  # noqa: E501
+            dataset_id (str): The ID of a dataset to use to make predictions.  The dataset must have the same column headers as the model's training dataset.  Only one of 'datasetID' and 'data' should be provided.. [optional]  # noqa: E501
+            return_row_headers (bool): If true then row headers will be returned in the response csv.  If true and the 'data' property is given then it is required that the first column of csv data are row headers.. [optional] if omitted the server will use the default value of False  # noqa: E501
+            return_column_headers (bool): If true then column headers will be returned in the response csv.. [optional] if omitted the server will use the default value of False  # noqa: E501
+            data (str): An array of CSV data with column headers.  Only one of 'datasetID' and 'data' should be provided.  If returnRowHeaders is true then the first column of the CSV should contain the unique row headers which identify each row.. [optional]  # noqa: E501
         """
 
-        type = kwargs.get('type', "weighted sum between")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         self = super(OpenApiModel, cls).__new__(cls)
@@ -176,60 +163,38 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        constant_args = {
-            '_check_type': _check_type,
-            '_path_to_item': _path_to_item,
-            '_spec_property_naming': _spec_property_naming,
-            '_configuration': _configuration,
-            '_visited_composed_classes': self._visited_composed_classes,
-        }
-        composed_info = validate_get_composed_info(
-            constant_args, kwargs, self)
-        self._composed_instances = composed_info[0]
-        self._var_name_to_model_instances = composed_info[1]
-        self._additional_properties_model_instances = composed_info[2]
-        discarded_args = composed_info[3]
-
         for var_name, var_value in kwargs.items():
-            if var_name in discarded_args and \
+            if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
-                        self._additional_properties_model_instances:
+                        self.additional_properties_type is None:
                 # discard variable.
                 continue
             setattr(self, var_name, var_value)
-
         return self
 
     required_properties = set([
         '_data_store',
         '_check_type',
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
-        '_composed_instances',
-        '_var_name_to_model_instances',
-        '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TarFnWeightedSumBetween - a model defined in OpenAPI
+        """ValidateRequest - a model defined in OpenAPI
 
         Keyword Args:
-            maximum (float):
-            minimum (float):
-            targets ({str: (float,)}):
-            type (str): Find a solution where the weighted sum of the given columns is between `\"minimum\"` and `\"maximum\"`.. defaults to "weighted sum between", must be one of ["weighted sum between", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -252,18 +217,21 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            importance (float): The higher the value the higher the importance of this target.  If the importance values all equal 1 then the `probabilityOfSuccess` is a true probability (the probability of all the targets being satisfied, assuming that the probability of any individual target being satisfied is independent of the others).  Note, having many targets or importance numbers > 1 can make the `probabilityOfSuccess` very small, even if most of the targets are individually likely to be met. If there are many targets it may be helpful to make the importance values all add up to 1. This will make the `probabilityOfSuccess` scale with the number of columns so that it becomes a more natural-looking \"score\" of how likely the targets are to be met. For example, the reported `probabilityOfSuccess` of achieving one target with probability 50% is the same as achieving two targets, each with probability 50% and importance 0.5. . [optional] if omitted the server will use the default value of 1  # noqa: E501
+            return_probability_distribution (bool): If true then the full probability distribution for each prediction will be returned, if false then the predicted value and uncertainty derived from that distribution will be returned instead.. [optional] if omitted the server will use the default value of False  # noqa: E501
+            dataset_id (str): The ID of a dataset to use to make predictions.  The dataset must have the same column headers as the model's training dataset.  Only one of 'datasetID' and 'data' should be provided.. [optional]  # noqa: E501
+            return_row_headers (bool): If true then row headers will be returned in the response csv.  If true and the 'data' property is given then it is required that the first column of csv data are row headers.. [optional] if omitted the server will use the default value of False  # noqa: E501
+            return_column_headers (bool): If true then column headers will be returned in the response csv.. [optional] if omitted the server will use the default value of False  # noqa: E501
+            data (str): An array of CSV data with column headers.  Only one of 'datasetID' and 'data' should be provided.  If returnRowHeaders is true then the first column of the CSV should contain the unique row headers which identify each row.. [optional]  # noqa: E501
         """
 
-        type = kwargs.get('type', "weighted sum between")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
@@ -279,54 +247,18 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        constant_args = {
-            '_check_type': _check_type,
-            '_path_to_item': _path_to_item,
-            '_spec_property_naming': _spec_property_naming,
-            '_configuration': _configuration,
-            '_visited_composed_classes': self._visited_composed_classes,
-        }
-        composed_info = validate_get_composed_info(
-            constant_args, kwargs, self)
-        self._composed_instances = composed_info[0]
-        self._var_name_to_model_instances = composed_info[1]
-        self._additional_properties_model_instances = composed_info[2]
-        discarded_args = composed_info[3]
-
         for var_name, var_value in kwargs.items():
-            if var_name in discarded_args and \
+            if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
-                        self._additional_properties_model_instances:
+                        self.additional_properties_type is None:
                 # discard variable.
                 continue
             setattr(self, var_name, var_value)
             if var_name in self.read_only_vars:
                 raise ApiAttributeError(f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
                                      f"class with read only attributes.")
-
-    @cached_property
-    def _composed_schemas():
-        # we need this here to make our import statements work
-        # we must store _composed_schemas in here so the code is only run
-        # when we invoke this method. If we kept this at the class
-        # level we would get an error because the class level
-        # code would be run when this module is imported, and these composed
-        # classes don't exist yet because their module has not finished
-        # loading
-        lazy_import()
-        return {
-          'anyOf': [
-          ],
-          'allOf': [
-              PartTarFnBetween,
-              PartTarFnWeightedSum,
-              TarFnWeightedSumBetweenAllOf,
-          ],
-          'oneOf': [
-          ],
-        }
```

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/tar_fn_weighted_sum_between_all_of.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/tar_fn_weighted_sum_between_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/target_function.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/target_function.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/train_request.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/train_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/training_dataset_outliers_request.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/training_dataset_outliers_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/validate_request.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/validation_split.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from alchemite_apiclient.exceptions import ApiAttributeError
 
 
 
-class ValidateRequest(ModelNormal):
+class ValidationSplit(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -53,60 +53,71 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
+        ('test_row_ids',): {
+            'min_items': 1,
+        },
+        ('train_row_ids',): {
+            'min_items': 1,
+        },
     }
 
-    additional_properties_type = None
+    @cached_property
+    def additional_properties_type():  # noqa
+        """
+        This must be a method because a model may have properties that are
+        of type self, this must run after the class is loaded
+        """
+        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():  # noqa
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'return_probability_distribution': (bool,),  # noqa: E501
-            'dataset_id': (str,),  # noqa: E501
-            'return_row_headers': (bool,),  # noqa: E501
-            'return_column_headers': (bool,),  # noqa: E501
-            'data': (str,),  # noqa: E501
+            'test_row_ids': ([str],),  # noqa: E501
+            'name': (str,),  # noqa: E501
+            'train_row_ids': ([str],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():  # noqa
         return None
 
 
     attribute_map = {
-        'return_probability_distribution': 'returnProbabilityDistribution',  # noqa: E501
-        'dataset_id': 'datasetID',  # noqa: E501
-        'return_row_headers': 'returnRowHeaders',  # noqa: E501
-        'return_column_headers': 'returnColumnHeaders',  # noqa: E501
-        'data': 'data',  # noqa: E501
+        'test_row_ids': 'testRowIDs',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'train_row_ids': 'trainRowIDs',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ValidateRequest - a model defined in OpenAPI
+    def _from_openapi_data(cls, test_row_ids, *args, **kwargs):  # noqa: E501
+        """ValidationSplit - a model defined in OpenAPI
+
+        Args:
+            test_row_ids ([str]): The row IDs from the training dataset to validate the sub-model against.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -131,19 +142,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            return_probability_distribution (bool): If true then the full probability distribution for each prediction will be returned, if false then the predicted value and uncertainty derived from that distribution will be returned instead.. [optional] if omitted the server will use the default value of False  # noqa: E501
-            dataset_id (str): The ID of a dataset to use to make predictions.  The dataset must have the same column headers as the model's training dataset.  Only one of 'datasetID' and 'data' should be provided.. [optional]  # noqa: E501
-            return_row_headers (bool): If true then row headers will be returned in the response csv.  If true and the 'data' property is given then it is required that the first column of csv data are row headers.. [optional] if omitted the server will use the default value of False  # noqa: E501
-            return_column_headers (bool): If true then column headers will be returned in the response csv.. [optional] if omitted the server will use the default value of False  # noqa: E501
-            data (str): An array of CSV data with column headers.  Only one of 'datasetID' and 'data' should be provided.  If returnRowHeaders is true then the first column of the CSV should contain the unique row headers which identify each row.. [optional]  # noqa: E501
+            name (str): The name of this split, used in `validation-predictions` to identify which set each prediction came from. If not provided the index of the split will be used. If provided, each split's name must be distinct . [optional]  # noqa: E501
+            train_row_ids ([str]): The row IDs from the training dataset to train the validation model on.  If omitted, is the complement of the testRowIDs in respect to the training dataset.  No elements of the test set may be present in the training set. . [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -163,14 +171,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.test_row_ids = test_row_ids
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -183,16 +192,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """ValidateRequest - a model defined in OpenAPI
+    def __init__(self, test_row_ids, *args, **kwargs):  # noqa: E501
+        """ValidationSplit - a model defined in OpenAPI
+
+        Args:
+            test_row_ids ([str]): The row IDs from the training dataset to validate the sub-model against.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -217,19 +229,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            return_probability_distribution (bool): If true then the full probability distribution for each prediction will be returned, if false then the predicted value and uncertainty derived from that distribution will be returned instead.. [optional] if omitted the server will use the default value of False  # noqa: E501
-            dataset_id (str): The ID of a dataset to use to make predictions.  The dataset must have the same column headers as the model's training dataset.  Only one of 'datasetID' and 'data' should be provided.. [optional]  # noqa: E501
-            return_row_headers (bool): If true then row headers will be returned in the response csv.  If true and the 'data' property is given then it is required that the first column of csv data are row headers.. [optional] if omitted the server will use the default value of False  # noqa: E501
-            return_column_headers (bool): If true then column headers will be returned in the response csv.. [optional] if omitted the server will use the default value of False  # noqa: E501
-            data (str): An array of CSV data with column headers.  Only one of 'datasetID' and 'data' should be provided.  If returnRowHeaders is true then the first column of the CSV should contain the unique row headers which identify each row.. [optional]  # noqa: E501
+            name (str): The name of this split, used in `validation-predictions` to identify which set each prediction came from. If not provided the index of the split will be used. If provided, each split's name must be distinct . [optional]  # noqa: E501
+            train_row_ids ([str]): The row IDs from the training dataset to train the validation model on.  If omitted, is the complement of the testRowIDs in respect to the training dataset.  No elements of the test set may be present in the training set. . [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -247,14 +256,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.test_row_ids = test_row_ids
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/validation_split.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/value.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,16 +24,22 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from alchemite_apiclient.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from alchemite_apiclient.model.float_none_type import FloatNoneType
+    from alchemite_apiclient.model.vector_value import VectorValue
+    globals()['VectorValue'] = VectorValue
+    globals()['float, none_type'] = float, none_type
 
-class ValidationSplit(ModelNormal):
+
+class Value(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -53,71 +59,66 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
-        ('test_row_ids',): {
-            'min_items': 1,
-        },
-        ('train_row_ids',): {
-            'min_items': 1,
-        },
     }
 
     @cached_property
     def additional_properties_type():  # noqa
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():  # noqa
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'test_row_ids': ([str],),  # noqa: E501
             'name': (str,),  # noqa: E501
-            'train_row_ids': ([str],),  # noqa: E501
+            'value': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():  # noqa
         return None
 
 
     attribute_map = {
-        'test_row_ids': 'testRowIDs',  # noqa: E501
         'name': 'name',  # noqa: E501
-        'train_row_ids': 'trainRowIDs',  # noqa: E501
+        'value': 'value',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, test_row_ids, *args, **kwargs):  # noqa: E501
-        """ValidationSplit - a model defined in OpenAPI
+    def _from_openapi_data(cls, name, value, *args, **kwargs):  # noqa: E501
+        """Value - a model defined in OpenAPI
 
         Args:
-            test_row_ids ([str]): The row IDs from the training dataset to validate the sub-model against.
+            name (str): Property's name
+            value (bool, date, datetime, dict, float, int, list, str, none_type):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -142,16 +143,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str): The name of this split, used in `validation-predictions` to identify which set each prediction came from. If not provided the index of the split will be used. If provided, each split's name must be distinct . [optional]  # noqa: E501
-            train_row_ids ([str]): The row IDs from the training dataset to train the validation model on.  If omitted, is the complement of the testRowIDs in respect to the training dataset.  No elements of the test set may be present in the training set. . [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -171,15 +170,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.test_row_ids = test_row_ids
+        self.name = name
+        self.value = value
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -192,19 +192,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, test_row_ids, *args, **kwargs):  # noqa: E501
-        """ValidationSplit - a model defined in OpenAPI
+    def __init__(self, name, value, *args, **kwargs):  # noqa: E501
+        """Value - a model defined in OpenAPI
 
         Args:
-            test_row_ids ([str]): The row IDs from the training dataset to validate the sub-model against.
+            name (str): Property's name
+            value (bool, date, datetime, dict, float, int, list, str, none_type):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -229,16 +230,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            name (str): The name of this split, used in `validation-predictions` to identify which set each prediction came from. If not provided the index of the split will be used. If provided, each split's name must be distinct . [optional]  # noqa: E501
-            train_row_ids ([str]): The row IDs from the training dataset to train the validation model on.  If omitted, is the complement of the testRowIDs in respect to the training dataset.  No elements of the test set may be present in the training set. . [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -256,15 +255,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.test_row_ids = test_row_ids
+        self.name = name
+        self.value = value
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/value.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/version_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,22 +24,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from alchemite_apiclient.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from alchemite_apiclient.model.float_none_type import FloatNoneType
-    from alchemite_apiclient.model.vector_value import VectorValue
-    globals()['VectorValue'] = VectorValue
-    globals()['float, none_type'] = float, none_type
 
-
-class Value(ModelNormal):
+class VersionResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -67,58 +61,54 @@
 
     @cached_property
     def additional_properties_type():  # noqa
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():  # noqa
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'name': (str,),  # noqa: E501
-            'value': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'api_definition_version': (str,),  # noqa: E501
+            'api_application_version': (str,),  # noqa: E501
+            'alchemite_version': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():  # noqa
         return None
 
 
     attribute_map = {
-        'name': 'name',  # noqa: E501
-        'value': 'value',  # noqa: E501
+        'api_definition_version': 'APIDefinitionVersion',  # noqa: E501
+        'api_application_version': 'APIApplicationVersion',  # noqa: E501
+        'alchemite_version': 'AlchemiteVersion',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, name, value, *args, **kwargs):  # noqa: E501
-        """Value - a model defined in OpenAPI
-
-        Args:
-            name (str): Property's name
-            value (bool, date, datetime, dict, float, int, list, str, none_type):
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """VersionResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -143,14 +133,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            api_definition_version (str): The version of the API definition in semantic version format (major.minor.patch).. [optional]  # noqa: E501
+            api_application_version (str): The version of the running API application in semantic version format (major.minor.patch).. [optional]  # noqa: E501
+            alchemite_version (str): The current version of Alchemite.  Note that existing models trained on older versions will have to be retrained to take advantage of the latest version.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -170,16 +163,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.name = name
-        self.value = value
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -192,20 +183,16 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, name, value, *args, **kwargs):  # noqa: E501
-        """Value - a model defined in OpenAPI
-
-        Args:
-            name (str): Property's name
-            value (bool, date, datetime, dict, float, int, list, str, none_type):
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """VersionResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -230,14 +217,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            api_definition_version (str): The version of the API definition in semantic version format (major.minor.patch).. [optional]  # noqa: E501
+            api_application_version (str): The version of the running API application in semantic version format (major.minor.patch).. [optional]  # noqa: E501
+            alchemite_version (str): The current version of Alchemite.  Note that existing models trained on older versions will have to be retrained to take advantage of the latest version.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -255,16 +245,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.name = name
-        self.value = value
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/vector_prediction.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/vector_prediction.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/vector_result.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/vector_result.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/vector_value.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/vector_value.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model/version_response.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model/sample_def_composition_all_of.py`

 * *Files 27% similar despite different names*

```diff
@@ -24,16 +24,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from alchemite_apiclient.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from alchemite_apiclient.model.sample_def_continuous import SampleDefContinuous
+    globals()['SampleDefContinuous'] = SampleDefContinuous
 
-class VersionResponse(ModelNormal):
+
+class SampleDefCompositionAllOf(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -50,67 +54,98 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
+        ('type',): {
+            'COMPOSITION': "composition",
+        },
     }
 
     validations = {
+        ('values',): {
+            'min_properties': 2,
+            'min_items': 2,
+        },
+        ('total_range',): {
+            'max_items': 2,
+            'min_items': 2,
+        },
+        ('min',): {
+            'inclusive_minimum': 0,
+        },
+        ('max',): {
+            'inclusive_minimum': 0,
+        },
     }
 
     @cached_property
     def additional_properties_type():  # noqa
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():  # noqa
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'api_definition_version': (str,),  # noqa: E501
-            'api_application_version': (str,),  # noqa: E501
-            'alchemite_version': (str,),  # noqa: E501
+            'type': (str,),  # noqa: E501
+            'values': ({str: (SampleDefContinuous,)},),  # noqa: E501
+            'total': (float,),  # noqa: E501
+            'total_range': ([float],),  # noqa: E501
+            'min': (int,),  # noqa: E501
+            'max': (int,),  # noqa: E501
+            'hard_limit': (bool,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():  # noqa
         return None
 
 
     attribute_map = {
-        'api_definition_version': 'APIDefinitionVersion',  # noqa: E501
-        'api_application_version': 'APIApplicationVersion',  # noqa: E501
-        'alchemite_version': 'AlchemiteVersion',  # noqa: E501
+        'type': 'type',  # noqa: E501
+        'values': 'values',  # noqa: E501
+        'total': 'total',  # noqa: E501
+        'total_range': 'totalRange',  # noqa: E501
+        'min': 'min',  # noqa: E501
+        'max': 'max',  # noqa: E501
+        'hard_limit': 'hardLimit',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """VersionResponse - a model defined in OpenAPI
+    def _from_openapi_data(cls, values, *args, **kwargs):  # noqa: E501
+        """SampleDefCompositionAllOf - a model defined in OpenAPI
+
+        Args:
+            values ({str: (SampleDefContinuous,)}): Define the continuous columns and their ranges. Sum of lower bound values must be less than or equal to `total`. Sum of upper bound values must be greater than or equal to `total`. Columns defined here cannot be defined in another sampleDefinition type. 
 
         Keyword Args:
+            type (str): Constrain two or more columns to sum up to `total`. Only supported for global optimization methods. . defaults to "composition", must be one of ["composition", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -133,19 +168,22 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            api_definition_version (str): The version of the API definition in semantic version format (major.minor.patch).. [optional]  # noqa: E501
-            api_application_version (str): The version of the running API application in semantic version format (major.minor.patch).. [optional]  # noqa: E501
-            alchemite_version (str): The current version of Alchemite.  Note that existing models trained on older versions will have to be retrained to take advantage of the latest version.. [optional]  # noqa: E501
+            total (float): The value the columns defined in `values` should sum up to. If not specified, then no total constraint will be applied. Cannot be used in conjunction with totalRange.. [optional]  # noqa: E501
+            total_range ([float]): The value the columns defined in `values` should sum between. If not specified, then no totalRange constraint will be applied. Cannot be used in conjunction with total.. [optional]  # noqa: E501
+            min (int): The minimum columns defined in `values` to be non-zero.. [optional] if omitted the server will use the default value of 0  # noqa: E501
+            max (int): The maximum columns defined in `values` to be non-zero. If not specified, it will default to the number of properties in `values`. [optional]  # noqa: E501
+            hard_limit (bool): Whether min/max are strictly enforced. Unused if no min or max set. . [optional] if omitted the server will use the default value of False  # noqa: E501
         """
 
+        type = kwargs.get('type', "composition")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         self = super(OpenApiModel, cls).__new__(cls)
@@ -163,14 +201,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.type = type
+        self.values = values
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -183,18 +223,22 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """VersionResponse - a model defined in OpenAPI
+    def __init__(self, values, *args, **kwargs):  # noqa: E501
+        """SampleDefCompositionAllOf - a model defined in OpenAPI
+
+        Args:
+            values ({str: (SampleDefContinuous,)}): Define the continuous columns and their ranges. Sum of lower bound values must be less than or equal to `total`. Sum of upper bound values must be greater than or equal to `total`. Columns defined here cannot be defined in another sampleDefinition type. 
 
         Keyword Args:
+            type (str): Constrain two or more columns to sum up to `total`. Only supported for global optimization methods. . defaults to "composition", must be one of ["composition", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -217,19 +261,22 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            api_definition_version (str): The version of the API definition in semantic version format (major.minor.patch).. [optional]  # noqa: E501
-            api_application_version (str): The version of the running API application in semantic version format (major.minor.patch).. [optional]  # noqa: E501
-            alchemite_version (str): The current version of Alchemite.  Note that existing models trained on older versions will have to be retrained to take advantage of the latest version.. [optional]  # noqa: E501
+            total (float): The value the columns defined in `values` should sum up to. If not specified, then no total constraint will be applied. Cannot be used in conjunction with totalRange.. [optional]  # noqa: E501
+            total_range ([float]): The value the columns defined in `values` should sum between. If not specified, then no totalRange constraint will be applied. Cannot be used in conjunction with total.. [optional]  # noqa: E501
+            min (int): The minimum columns defined in `values` to be non-zero.. [optional] if omitted the server will use the default value of 0  # noqa: E501
+            max (int): The maximum columns defined in `values` to be non-zero. If not specified, it will default to the number of properties in `values`. [optional]  # noqa: E501
+            hard_limit (bool): Whether min/max are strictly enforced. Unused if no min or max set. . [optional] if omitted the server will use the default value of False  # noqa: E501
         """
 
+        type = kwargs.get('type', "composition")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
@@ -245,14 +292,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.type = type
+        self.values = values
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/model_utils.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/model_utils.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/models/__init__.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/models/__init__.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient/rest.py` & `alchemite_apiclient-0.54.0/alchemite_apiclient/rest.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient.egg-info/PKG-INFO` & `alchemite_apiclient-0.54.0/alchemite_apiclient.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alchemite-apiclient
-Version: 0.53.0
+Version: 0.54.0
 Summary: A python API client for using Alchemite Analytics
 Home-page: 
 Author: Intellegens
 Author-email: Intellegens <support@intellegens.com>
 Project-URL: Homepage, https://intellegens.com
 Project-URL: Docs, https://docs.intellegens.com
 Keywords: Alchemite,Alchemite API,Machine Learning,Artificial Intelligence
@@ -19,15 +19,15 @@
 
 # alchemite-apiclient
 
 This is a client for interacting with Alchemite Analytics, an applied machine learning platform to accelerate industrial
 R&D and optimise manufacturing by extracting information from sparce or noisy datasets.
 To obtain a licence for this product, please [contact Intellegens](https://intellegens.com/contact-us/) for more information.
 
-API version: 0.53.0
+API version: 0.54.0
 
 ## Requirements.
 
 Python >=3.8
 
 ## Installation & Usage
 ### pip install
```

### Comparing `alchemite_apiclient-0.53.0/alchemite_apiclient.egg-info/SOURCES.txt` & `alchemite_apiclient-0.54.0/alchemite_apiclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/AdditiveSensitivityRequest.md` & `alchemite_apiclient-0.54.0/docs/AdditiveSensitivityRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/AnalyseValidateRequest.md` & `alchemite_apiclient-0.54.0/docs/AnalyseValidateRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/AnalyseValidateRequestAllOf.md` & `alchemite_apiclient-0.54.0/docs/AnalyseValidateRequestAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/AnalyseValidateResponse.md` & `alchemite_apiclient-0.54.0/docs/AnalyseValidateResponse.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/AnalyseValidateResponseColumnAnalytics.md` & `alchemite_apiclient-0.54.0/docs/AnalyseValidateResponseColumnAnalytics.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/CategoricalColumn.md` & `alchemite_apiclient-0.54.0/docs/CategoricalColumn.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/CategoricalColumnInfo.md` & `alchemite_apiclient-0.54.0/docs/CategoricalColumnInfo.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/CategoricalColumnInfoAllOf.md` & `alchemite_apiclient-0.54.0/docs/CategoricalColumnInfoAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/CategoricalColumnInfoStats.md` & `alchemite_apiclient-0.54.0/docs/CategoricalColumnInfoStats.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/CategoricalModelColumnInfo.md` & `alchemite_apiclient-0.54.0/docs/CategoricalModelColumnInfo.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/CategoricalModelColumnInfoAllOf.md` & `alchemite_apiclient-0.54.0/docs/CategoricalModelColumnInfoAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/CategoricalPrediction.md` & `alchemite_apiclient-0.54.0/docs/CategoricalPrediction.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/CategoricalResult.md` & `alchemite_apiclient-0.54.0/docs/CategoricalResult.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/ColumnGroupBatchRequest.md` & `alchemite_apiclient-0.54.0/docs/ColumnGroupBatchRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/ColumnGroupPatchRequest.md` & `alchemite_apiclient-0.54.0/docs/ColumnGroupPatchRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/ColumnGroupRequest.md` & `alchemite_apiclient-0.54.0/docs/ColumnGroupRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/ColumnGroupResponse.md` & `alchemite_apiclient-0.54.0/docs/ColumnGroupResponse.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/ColumnGroupResponseAllOf.md` & `alchemite_apiclient-0.54.0/docs/ColumnGroupResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/ColumnInfo.md` & `alchemite_apiclient-0.54.0/docs/ColumnInfo.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/ColumnValue.md` & `alchemite_apiclient-0.54.0/docs/ColumnValue.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/ColumnValueNullable.md` & `alchemite_apiclient-0.54.0/docs/ColumnValueNullable.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/ContinuousColumnInfo.md` & `alchemite_apiclient-0.54.0/docs/ContinuousColumnInfo.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/ContinuousColumnInfoAllOf.md` & `alchemite_apiclient-0.54.0/docs/ContinuousColumnInfoAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/ContinuousColumnInfoStats.md` & `alchemite_apiclient-0.54.0/docs/ContinuousColumnInfoStats.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/ContinuousModelColumnInfo.md` & `alchemite_apiclient-0.54.0/docs/ContinuousModelColumnInfo.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/ContinuousModelColumnInfoAllOf.md` & `alchemite_apiclient-0.54.0/docs/ContinuousModelColumnInfoAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/DRDatasetReductionData.md` & `alchemite_apiclient-0.54.0/docs/DRDatasetReductionData.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/DRDatasetReductionMetadata.md` & `alchemite_apiclient-0.54.0/docs/DRDatasetReductionMetadata.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/DRDatasetReductionMetadataSources.md` & `alchemite_apiclient-0.54.0/docs/DRDatasetReductionMetadataSources.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/DRJobReductionMetadata.md` & `alchemite_apiclient-0.54.0/docs/DRJobReductionMetadata.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/DRJobReductionMetadataSources.md` & `alchemite_apiclient-0.54.0/docs/DRJobReductionMetadataSources.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/DRModelReductionData.md` & `alchemite_apiclient-0.54.0/docs/DRModelReductionData.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/DRPCAReductionType.md` & `alchemite_apiclient-0.54.0/docs/DRPCAReductionType.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/DRThreeDimensionPoint.md` & `alchemite_apiclient-0.54.0/docs/DRThreeDimensionPoint.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/DRTwoDimensionPoint.md` & `alchemite_apiclient-0.54.0/docs/DRTwoDimensionPoint.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/DRUMAPReductionType.md` & `alchemite_apiclient-0.54.0/docs/DRUMAPReductionType.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/Data.md` & `alchemite_apiclient-0.54.0/docs/Data.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/Dataset.md` & `alchemite_apiclient-0.54.0/docs/Dataset.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/Dataset1.md` & `alchemite_apiclient-0.54.0/docs/Dataset1.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/DatasetChunk.md` & `alchemite_apiclient-0.54.0/docs/DatasetChunk.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/DatasetOrData.md` & `alchemite_apiclient-0.54.0/docs/DatasetOrData.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/DatasetPatch.md` & `alchemite_apiclient-0.54.0/docs/DatasetPatch.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/DatasetQueryRequest.md` & `alchemite_apiclient-0.54.0/docs/DatasetQueryRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/DatasetQueryRequestRowIDs.md` & `alchemite_apiclient-0.54.0/docs/DatasetQueryRequestRowIDs.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/DatasetQueryRequestSort.md` & `alchemite_apiclient-0.54.0/docs/DatasetQueryRequestSort.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/DatasetQueryResponseResult.md` & `alchemite_apiclient-0.54.0/docs/DatasetQueryResponseResult.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/DatasetsApi.md` & `alchemite_apiclient-0.54.0/docs/DatasetsApi.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/DefaultApi.md` & `alchemite_apiclient-0.54.0/docs/DefaultApi.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/DependentColFnArgCol.md` & `alchemite_apiclient-0.54.0/docs/DependentColFnArgCol.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/DependentColFnArgColWeights.md` & `alchemite_apiclient-0.54.0/docs/DependentColFnArgColWeights.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/DependentColFnArgConstantSum.md` & `alchemite_apiclient-0.54.0/docs/DependentColFnArgConstantSum.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/DependentColFnArgProduct.md` & `alchemite_apiclient-0.54.0/docs/DependentColFnArgProduct.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/DependentColFnArgRatio.md` & `alchemite_apiclient-0.54.0/docs/DependentColFnArgRatio.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/DependentColFnArgSummandsWeights.md` & `alchemite_apiclient-0.54.0/docs/DependentColFnArgSummandsWeights.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/DependentColFnArgWeightedConstSum.md` & `alchemite_apiclient-0.54.0/docs/DependentColFnArgWeightedConstSum.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/DependentColFnArgWeightedRatio.md` & `alchemite_apiclient-0.54.0/docs/DependentColFnArgWeightedRatio.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/DependentColFnArgZeroIfZero.md` & `alchemite_apiclient-0.54.0/docs/DependentColFnArgZeroIfZero.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/DependentColFnArgZeroIfZeroAllOf.md` & `alchemite_apiclient-0.54.0/docs/DependentColFnArgZeroIfZeroAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/DependentColumns.md` & `alchemite_apiclient-0.54.0/docs/DependentColumns.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/DimensionalityReductionRequest.md` & `alchemite_apiclient-0.54.0/docs/DimensionalityReductionRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/DimensionalityReductionResponse.md` & `alchemite_apiclient-0.54.0/docs/DimensionalityReductionResponse.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/EmptyCategoricalColumn.md` & `alchemite_apiclient-0.54.0/docs/EmptyCategoricalColumn.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/EmptyContinuousColumn.md` & `alchemite_apiclient-0.54.0/docs/EmptyContinuousColumn.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/Error.md` & `alchemite_apiclient-0.54.0/docs/Error.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/GetOptimizeDone.md` & `alchemite_apiclient-0.54.0/docs/GetOptimizeDone.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/GetOptimizeDoneAllOf.md` & `alchemite_apiclient-0.54.0/docs/GetOptimizeDoneAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/GetOptimizeFailed.md` & `alchemite_apiclient-0.54.0/docs/GetOptimizeFailed.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/GetOptimizeFailedAllOf.md` & `alchemite_apiclient-0.54.0/docs/GetOptimizeFailedAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/GetOptimizeOptimizing.md` & `alchemite_apiclient-0.54.0/docs/GetOptimizeOptimizing.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/GetOptimizeOptimizingAllOf.md` & `alchemite_apiclient-0.54.0/docs/GetOptimizeOptimizingAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/GetOptimizePending.md` & `alchemite_apiclient-0.54.0/docs/GetOptimizePending.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/GetOptimizePendingAllOf.md` & `alchemite_apiclient-0.54.0/docs/GetOptimizePendingAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/GetSuggestAdditionalDone.md` & `alchemite_apiclient-0.54.0/docs/GetSuggestAdditionalDone.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/GetSuggestAdditionalDoneAllOf.md` & `alchemite_apiclient-0.54.0/docs/GetSuggestAdditionalDoneAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/GetSuggestAdditionalFailed.md` & `alchemite_apiclient-0.54.0/docs/GetSuggestAdditionalFailed.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/GetSuggestAdditionalFailedAllOf.md` & `alchemite_apiclient-0.54.0/docs/GetSuggestAdditionalFailedAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/GetSuggestAdditionalPending.md` & `alchemite_apiclient-0.54.0/docs/GetSuggestAdditionalPending.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/GetSuggestAdditionalPendingAllOf.md` & `alchemite_apiclient-0.54.0/docs/GetSuggestAdditionalPendingAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/GetSuggestAdditionalRunning.md` & `alchemite_apiclient-0.54.0/docs/GetSuggestAdditionalRunning.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/GetSuggestAdditionalRunningAllOf.md` & `alchemite_apiclient-0.54.0/docs/GetSuggestAdditionalRunningAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/GetSuggestHistoricDone.md` & `alchemite_apiclient-0.54.0/docs/GetSuggestHistoricDone.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/GetSuggestHistoricDoneAllOf.md` & `alchemite_apiclient-0.54.0/docs/GetSuggestHistoricDoneAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/GetSuggestHistoricFailed.md` & `alchemite_apiclient-0.54.0/docs/GetSuggestHistoricFailed.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/GetSuggestHistoricPending.md` & `alchemite_apiclient-0.54.0/docs/GetSuggestHistoricPending.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/GetSuggestHistoricRunning.md` & `alchemite_apiclient-0.54.0/docs/GetSuggestHistoricRunning.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/GetSuggestInitialDone.md` & `alchemite_apiclient-0.54.0/docs/GetSuggestInitialDone.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/GetSuggestInitialDoneAllOf.md` & `alchemite_apiclient-0.54.0/docs/GetSuggestInitialDoneAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/GetSuggestInitialFailed.md` & `alchemite_apiclient-0.54.0/docs/GetSuggestInitialFailed.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/GetSuggestInitialFailedAllOf.md` & `alchemite_apiclient-0.54.0/docs/GetSuggestInitialFailedAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/GetSuggestInitialPending.md` & `alchemite_apiclient-0.54.0/docs/GetSuggestInitialPending.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/GetSuggestInitialRunning.md` & `alchemite_apiclient-0.54.0/docs/GetSuggestInitialRunning.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/HistoricCategoricalPrediction.md` & `alchemite_apiclient-0.54.0/docs/HistoricCategoricalPrediction.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/HistoricPrediction.md` & `alchemite_apiclient-0.54.0/docs/HistoricPrediction.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/HistoricScalarPrediction.md` & `alchemite_apiclient-0.54.0/docs/HistoricScalarPrediction.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/HistoricTargetFunction.md` & `alchemite_apiclient-0.54.0/docs/HistoricTargetFunction.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/HistoricValue.md` & `alchemite_apiclient-0.54.0/docs/HistoricValue.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/HistoricVectorPrediction.md` & `alchemite_apiclient-0.54.0/docs/HistoricVectorPrediction.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/HistoricVectorValue.md` & `alchemite_apiclient-0.54.0/docs/HistoricVectorValue.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/ImportanceRequest.md` & `alchemite_apiclient-0.54.0/docs/ImportanceRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/ImputeRequest.md` & `alchemite_apiclient-0.54.0/docs/ImputeRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/JobPatch.md` & `alchemite_apiclient-0.54.0/docs/JobPatch.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/MetricsApi.md` & `alchemite_apiclient-0.54.0/docs/MetricsApi.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/Model.md` & `alchemite_apiclient-0.54.0/docs/Model.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/ModelColumnInfo.md` & `alchemite_apiclient-0.54.0/docs/ModelColumnInfo.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/ModelDatasetApi.md` & `alchemite_apiclient-0.54.0/docs/ModelDatasetApi.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/ModelPatch.md` & `alchemite_apiclient-0.54.0/docs/ModelPatch.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/ModelPermittedColumnRelationships.md` & `alchemite_apiclient-0.54.0/docs/ModelPermittedColumnRelationships.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/ModelsApi.md` & `alchemite_apiclient-0.54.0/docs/ModelsApi.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/ModelsIdAdditiveSensitivityOrigin.md` & `alchemite_apiclient-0.54.0/docs/ModelsIdAdditiveSensitivityOrigin.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/ModelsIdTrainPermittedColumnRelationships.md` & `alchemite_apiclient-0.54.0/docs/ModelsIdTrainPermittedColumnRelationships.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/NewColFnArgCol.md` & `alchemite_apiclient-0.54.0/docs/NewColFnArgCol.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/NewColFnArgColAllOf.md` & `alchemite_apiclient-0.54.0/docs/NewColFnArgColAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/NewColFnArgColWeights.md` & `alchemite_apiclient-0.54.0/docs/NewColFnArgColWeights.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/NewColFnArgColWeightsAllOf.md` & `alchemite_apiclient-0.54.0/docs/NewColFnArgColWeightsAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/NewColFnArgColWeightsAllOfArguments.md` & `alchemite_apiclient-0.54.0/docs/NewColFnArgColWeightsAllOfArguments.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/NewColFnArgConstantSum.md` & `alchemite_apiclient-0.54.0/docs/NewColFnArgConstantSum.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/NewColFnArgConstantSumAllOf.md` & `alchemite_apiclient-0.54.0/docs/NewColFnArgConstantSumAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/NewColFnArgConstantSumAllOfArguments.md` & `alchemite_apiclient-0.54.0/docs/NewColFnArgConstantSumAllOfArguments.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/NewColFnArgProduct.md` & `alchemite_apiclient-0.54.0/docs/NewColFnArgProduct.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/NewColFnArgProductAllOf.md` & `alchemite_apiclient-0.54.0/docs/NewColFnArgProductAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/NewColFnArgProductAllOfArguments.md` & `alchemite_apiclient-0.54.0/docs/NewColFnArgProductAllOfArguments.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/NewColFnArgRatio.md` & `alchemite_apiclient-0.54.0/docs/NewColFnArgRatio.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/NewColFnArgRatioAllOf.md` & `alchemite_apiclient-0.54.0/docs/NewColFnArgRatioAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/NewColFnArgSummandsWeights.md` & `alchemite_apiclient-0.54.0/docs/NewColFnArgSummandsWeights.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/NewColFnArgSummandsWeightsAllOf.md` & `alchemite_apiclient-0.54.0/docs/NewColFnArgSummandsWeightsAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/NewColFnArgSummandsWeightsAllOfArguments.md` & `alchemite_apiclient-0.54.0/docs/NewColFnArgSummandsWeightsAllOfArguments.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/NewColFnArgWeightedConstSum.md` & `alchemite_apiclient-0.54.0/docs/NewColFnArgWeightedConstSum.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/NewColFnArgWeightedConstSumAllOf.md` & `alchemite_apiclient-0.54.0/docs/NewColFnArgWeightedConstSumAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/NewColFnArgWeightedConstSumAllOfArguments.md` & `alchemite_apiclient-0.54.0/docs/NewColFnArgWeightedConstSumAllOfArguments.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/NewColFnArgWeightedRatio.md` & `alchemite_apiclient-0.54.0/docs/NewColFnArgWeightedRatio.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/NewColFnArgWeightedRatioAllOf.md` & `alchemite_apiclient-0.54.0/docs/NewColFnArgWeightedRatioAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/NewColFnArgWeightedRatioAllOfArguments.md` & `alchemite_apiclient-0.54.0/docs/NewColFnArgWeightedRatioAllOfArguments.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/NewColFnArgZeroIfZero.md` & `alchemite_apiclient-0.54.0/docs/NewColFnArgZeroIfZero.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/NewColFnArgZeroIfZeroAllOf.md` & `alchemite_apiclient-0.54.0/docs/NewColFnArgZeroIfZeroAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/NewColumns.md` & `alchemite_apiclient-0.54.0/docs/NewColumns.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/NonEmptyCategoricalColumn.md` & `alchemite_apiclient-0.54.0/docs/NonEmptyCategoricalColumn.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/NonEmptyContinuousColumn.md` & `alchemite_apiclient-0.54.0/docs/NonEmptyContinuousColumn.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/NonEmptyIntegerCategoricalColumn.md` & `alchemite_apiclient-0.54.0/docs/NonEmptyIntegerCategoricalColumn.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/OTSampleDefCategorical.md` & `alchemite_apiclient-0.54.0/docs/OTSampleDefCategorical.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/OTSampleDefContinuous.md` & `alchemite_apiclient-0.54.0/docs/OTSampleDefContinuous.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/OTSampleDefinition.md` & `alchemite_apiclient-0.54.0/docs/OTSampleDefinition.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/OptimizeRequest.md` & `alchemite_apiclient-0.54.0/docs/OptimizeRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/OutliersRequest.md` & `alchemite_apiclient-0.54.0/docs/OutliersRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/OutputToleranceRequest.md` & `alchemite_apiclient-0.54.0/docs/OutputToleranceRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/OutputToleranceResponse.md` & `alchemite_apiclient-0.54.0/docs/OutputToleranceResponse.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/OutputToleranceResponseFixedInputs.md` & `alchemite_apiclient-0.54.0/docs/OutputToleranceResponseFixedInputs.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/OutputToleranceResponsePredictedOutputs.md` & `alchemite_apiclient-0.54.0/docs/OutputToleranceResponsePredictedOutputs.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/OutputToleranceResponsePredictions.md` & `alchemite_apiclient-0.54.0/docs/OutputToleranceResponsePredictions.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/OutputToleranceResponseSampledInputs.md` & `alchemite_apiclient-0.54.0/docs/OutputToleranceResponseSampledInputs.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/PartDependentColumns.md` & `alchemite_apiclient-0.54.0/docs/PartDependentColumns.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/PartGetOptimize.md` & `alchemite_apiclient-0.54.0/docs/PartGetOptimize.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/PartGetSuggestAdditional.md` & `alchemite_apiclient-0.54.0/docs/PartGetSuggestAdditional.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/PartGetSuggestHistoric.md` & `alchemite_apiclient-0.54.0/docs/PartGetSuggestHistoric.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/PartGetSuggestInitial.md` & `alchemite_apiclient-0.54.0/docs/PartGetSuggestInitial.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/PartNewColumns.md` & `alchemite_apiclient-0.54.0/docs/PartNewColumns.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/PartTarFnBetween.md` & `alchemite_apiclient-0.54.0/docs/PartTarFnBetween.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/PartTarFnCategoricals.md` & `alchemite_apiclient-0.54.0/docs/PartTarFnCategoricals.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/PartTarFnSingleTar.md` & `alchemite_apiclient-0.54.0/docs/PartTarFnSingleTar.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/PartTarFnSum.md` & `alchemite_apiclient-0.54.0/docs/PartTarFnSum.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/PartTarFnWeightedSum.md` & `alchemite_apiclient-0.54.0/docs/PartTarFnWeightedSum.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/PredictRequest.md` & `alchemite_apiclient-0.54.0/docs/PredictRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/Prediction.md` & `alchemite_apiclient-0.54.0/docs/Prediction.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/QueryRequest.md` & `alchemite_apiclient-0.54.0/docs/QueryRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/QueryResponse.md` & `alchemite_apiclient-0.54.0/docs/QueryResponse.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/SISampleDefCategorical.md` & `alchemite_apiclient-0.54.0/docs/SISampleDefCategorical.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/SISampleDefCategoricalColumnValues.md` & `alchemite_apiclient-0.54.0/docs/SISampleDefCategoricalColumnValues.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/SISampleDefContinuous.md` & `alchemite_apiclient-0.54.0/docs/SISampleDefContinuous.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/SISampleDefinition.md` & `alchemite_apiclient-0.54.0/docs/SISampleDefinition.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/SampleDefCategorical.md` & `alchemite_apiclient-0.54.0/docs/SampleDefCategorical.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/SampleDefCategoricalColumnValues.md` & `alchemite_apiclient-0.54.0/docs/SampleDefCategoricalColumnValues.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/SampleDefComposition.md` & `alchemite_apiclient-0.54.0/docs/SampleDefCompositionAllOf.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-# SampleDefComposition
+# SampleDefCompositionAllOf
 
-Constrain two or more columns to sum up to `total`. Only supported for global optimization methods. 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
 **values** | [**{str: (SampleDefContinuous,)}**](SampleDefContinuous.md) | Define the continuous columns and their ranges. Sum of lower bound values must be less than or equal to &#x60;total&#x60;. Sum of upper bound values must be greater than or equal to &#x60;total&#x60;. Columns defined here cannot be defined in another sampleDefinition type.  | 
 **type** | **str** | Constrain two or more columns to sum up to &#x60;total&#x60;. Only supported for global optimization methods.  | defaults to "composition"
-**total** | **float** | The value the columns defined in &#x60;values&#x60; should sum up to. If not specified, then no total constraint will be applied. | [optional] 
+**total** | **float** | The value the columns defined in &#x60;values&#x60; should sum up to. If not specified, then no total constraint will be applied. Cannot be used in conjunction with totalRange. | [optional] 
+**total_range** | **[float]** | The value the columns defined in &#x60;values&#x60; should sum between. If not specified, then no totalRange constraint will be applied. Cannot be used in conjunction with total. | [optional] 
 **min** | **int** | The minimum columns defined in &#x60;values&#x60; to be non-zero. | [optional]  if omitted the server will use the default value of 0
 **max** | **int** | The maximum columns defined in &#x60;values&#x60; to be non-zero. If not specified, it will default to the number of properties in &#x60;values&#x60; | [optional] 
 **hard_limit** | **bool** | Whether min/max are strictly enforced. Unused if no min or max set.  | [optional]  if omitted the server will use the default value of False
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `alchemite_apiclient-0.53.0/docs/SampleDefCompositionAllOf.md` & `alchemite_apiclient-0.54.0/docs/SampleDefComposition.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-# SampleDefCompositionAllOf
+# SampleDefComposition
 
+Constrain two or more columns to sum up to `total`. Only supported for global optimization methods. 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
 **values** | [**{str: (SampleDefContinuous,)}**](SampleDefContinuous.md) | Define the continuous columns and their ranges. Sum of lower bound values must be less than or equal to &#x60;total&#x60;. Sum of upper bound values must be greater than or equal to &#x60;total&#x60;. Columns defined here cannot be defined in another sampleDefinition type.  | 
 **type** | **str** | Constrain two or more columns to sum up to &#x60;total&#x60;. Only supported for global optimization methods.  | defaults to "composition"
-**total** | **float** | The value the columns defined in &#x60;values&#x60; should sum up to. If not specified, then no total constraint will be applied. | [optional] 
+**total** | **float** | The value the columns defined in &#x60;values&#x60; should sum up to. If not specified, then no total constraint will be applied. Cannot be used in conjunction with totalRange. | [optional] 
+**total_range** | **[float]** | The value the columns defined in &#x60;values&#x60; should sum between. If not specified, then no totalRange constraint will be applied. Cannot be used in conjunction with total. | [optional] 
 **min** | **int** | The minimum columns defined in &#x60;values&#x60; to be non-zero. | [optional]  if omitted the server will use the default value of 0
 **max** | **int** | The maximum columns defined in &#x60;values&#x60; to be non-zero. If not specified, it will default to the number of properties in &#x60;values&#x60; | [optional] 
 **hard_limit** | **bool** | Whether min/max are strictly enforced. Unused if no min or max set.  | [optional]  if omitted the server will use the default value of False
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `alchemite_apiclient-0.53.0/docs/SampleDefContinuous.md` & `alchemite_apiclient-0.54.0/docs/SampleDefContinuous.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/SampleDefContinuousWithStart.md` & `alchemite_apiclient-0.54.0/docs/SampleDefContinuousWithStart.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/SampleDefDiscrete.md` & `alchemite_apiclient-0.54.0/docs/SampleDefDiscrete.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/SampleDefInteger.md` & `alchemite_apiclient-0.54.0/docs/SampleDefInteger.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/SampleDefStartProp.md` & `alchemite_apiclient-0.54.0/docs/SampleDefStartProp.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/SampleDefWeightedCategorical.md` & `alchemite_apiclient-0.54.0/docs/SampleDefWeightedCategorical.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/SampleDefinition.md` & `alchemite_apiclient-0.54.0/docs/SampleDefinition.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/ScalarPrediction.md` & `alchemite_apiclient-0.54.0/docs/ScalarPrediction.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/ScalarResult.md` & `alchemite_apiclient-0.54.0/docs/ScalarResult.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/SensitivityRequest.md` & `alchemite_apiclient-0.54.0/docs/SensitivityRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/ShareGroup.md` & `alchemite_apiclient-0.54.0/docs/ShareGroup.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/SuggestAdditionalParameters.md` & `alchemite_apiclient-0.54.0/docs/SuggestAdditionalParameters.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/SuggestAdditionalParametersAllOf.md` & `alchemite_apiclient-0.54.0/docs/SuggestAdditionalParametersAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/SuggestAdditionalRequest.md` & `alchemite_apiclient-0.54.0/docs/SuggestAdditionalRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/SuggestAdditionalRequestAllOf.md` & `alchemite_apiclient-0.54.0/docs/SuggestAdditionalRequestAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/SuggestHistoricParameters.md` & `alchemite_apiclient-0.54.0/docs/SuggestHistoricParameters.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/SuggestHistoricRequest.md` & `alchemite_apiclient-0.54.0/docs/SuggestHistoricRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/SuggestHistoricResult.md` & `alchemite_apiclient-0.54.0/docs/SuggestHistoricResult.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/SuggestHistoricResultSamples.md` & `alchemite_apiclient-0.54.0/docs/SuggestHistoricResultSamples.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/SuggestInitialParameters.md` & `alchemite_apiclient-0.54.0/docs/SuggestInitialParameters.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/SuggestInitialRequest.md` & `alchemite_apiclient-0.54.0/docs/SuggestInitialRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/SuggestInitialRequestAllOf.md` & `alchemite_apiclient-0.54.0/docs/SuggestInitialRequestAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/SuggestInitialResponse.md` & `alchemite_apiclient-0.54.0/docs/SuggestInitialResponse.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/SuggestMissingCommon.md` & `alchemite_apiclient-0.54.0/docs/SuggestMissingCommon.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/SuggestMissingData.md` & `alchemite_apiclient-0.54.0/docs/SuggestMissingData.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/SuggestMissingDataAllOf.md` & `alchemite_apiclient-0.54.0/docs/SuggestMissingDataAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/SuggestMissingDatasetID.md` & `alchemite_apiclient-0.54.0/docs/SuggestMissingDatasetID.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/SuggestMissingDatasetIDAllOf.md` & `alchemite_apiclient-0.54.0/docs/SuggestMissingDatasetIDAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/SuggestMissingImputedData.md` & `alchemite_apiclient-0.54.0/docs/SuggestMissingImputedData.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/SuggestMissingImputedDataAllOf.md` & `alchemite_apiclient-0.54.0/docs/SuggestMissingImputedDataAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/SuggestMissingRequest.md` & `alchemite_apiclient-0.54.0/docs/SuggestMissingRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/SuggestMissingResponse.md` & `alchemite_apiclient-0.54.0/docs/SuggestMissingResponse.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/SuggestMissingSpecific.md` & `alchemite_apiclient-0.54.0/docs/SuggestMissingSpecific.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/TarFnAbove.md` & `alchemite_apiclient-0.54.0/docs/TarFnAbove.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/TarFnAboveAllOf.md` & `alchemite_apiclient-0.54.0/docs/TarFnAboveAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/TarFnBelow.md` & `alchemite_apiclient-0.54.0/docs/TarFnBelow.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/TarFnBelowAllOf.md` & `alchemite_apiclient-0.54.0/docs/TarFnBelowAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/TarFnBetween.md` & `alchemite_apiclient-0.54.0/docs/TarFnBetween.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/TarFnBetweenAllOf.md` & `alchemite_apiclient-0.54.0/docs/TarFnBetweenAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/TarFnExcludeCategories.md` & `alchemite_apiclient-0.54.0/docs/TarFnExcludeCategories.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/TarFnExcludeCategoriesAllOf.md` & `alchemite_apiclient-0.54.0/docs/TarFnExcludeCategoriesAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/TarFnIncludeCategories.md` & `alchemite_apiclient-0.54.0/docs/TarFnIncludeCategories.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/TarFnIncludeCategoriesAllOf.md` & `alchemite_apiclient-0.54.0/docs/TarFnIncludeCategoriesAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/TarFnSumAbove.md` & `alchemite_apiclient-0.54.0/docs/TarFnSumAbove.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/TarFnSumAboveAllOf.md` & `alchemite_apiclient-0.54.0/docs/TarFnSumAboveAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/TarFnSumBelow.md` & `alchemite_apiclient-0.54.0/docs/TarFnSumBelow.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/TarFnSumBelowAllOf.md` & `alchemite_apiclient-0.54.0/docs/TarFnSumBelowAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/TarFnSumBetween.md` & `alchemite_apiclient-0.54.0/docs/TarFnSumBetween.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/TarFnSumBetweenAllOf.md` & `alchemite_apiclient-0.54.0/docs/TarFnSumBetweenAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/TarFnWeightedSumAbove.md` & `alchemite_apiclient-0.54.0/docs/TarFnWeightedSumAbove.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/TarFnWeightedSumAboveAllOf.md` & `alchemite_apiclient-0.54.0/docs/TarFnWeightedSumAboveAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/TarFnWeightedSumBelow.md` & `alchemite_apiclient-0.54.0/docs/TarFnWeightedSumBelow.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/TarFnWeightedSumBelowAllOf.md` & `alchemite_apiclient-0.54.0/docs/TarFnWeightedSumBelowAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/TarFnWeightedSumBetween.md` & `alchemite_apiclient-0.54.0/docs/TarFnWeightedSumBetween.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/TarFnWeightedSumBetweenAllOf.md` & `alchemite_apiclient-0.54.0/docs/TarFnWeightedSumBetweenAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/TargetFunction.md` & `alchemite_apiclient-0.54.0/docs/TargetFunction.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/TrainRequest.md` & `alchemite_apiclient-0.54.0/docs/TrainRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/ValidateRequest.md` & `alchemite_apiclient-0.54.0/docs/ValidateRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/ValidationSplit.md` & `alchemite_apiclient-0.54.0/docs/ValidationSplit.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/Value.md` & `alchemite_apiclient-0.54.0/docs/Value.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/VectorPrediction.md` & `alchemite_apiclient-0.54.0/docs/VectorPrediction.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/VectorResult.md` & `alchemite_apiclient-0.54.0/docs/VectorResult.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/VectorValue.md` & `alchemite_apiclient-0.54.0/docs/VectorValue.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/docs/VersionResponse.md` & `alchemite_apiclient-0.54.0/docs/VersionResponse.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/example/adrenergic.csv` & `alchemite_apiclient-0.54.0/example/adrenergic.csv`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/example/adrenergic_holdout.csv` & `alchemite_apiclient-0.54.0/example/adrenergic_holdout.csv`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/example/adrenergic_row.csv` & `alchemite_apiclient-0.54.0/example/adrenergic_row.csv`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/example/categorical.csv` & `alchemite_apiclient-0.54.0/example/categorical.csv`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/example/example_additive_sensitivity.py` & `alchemite_apiclient-0.54.0/example/example_additive_sensitivity.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/example/example_basic.py` & `alchemite_apiclient-0.54.0/example/example_basic.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/example/example_categorical.py` & `alchemite_apiclient-0.54.0/example/example_categorical.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/example/example_chunk.py` & `alchemite_apiclient-0.54.0/example/example_chunk.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/example/example_column_groups.py` & `alchemite_apiclient-0.54.0/example/example_column_groups.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/example/example_custom_validation_splits.py` & `alchemite_apiclient-0.54.0/example/example_custom_validation_splits.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/example/example_delete.py` & `alchemite_apiclient-0.54.0/example/example_delete.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/example/example_dimensionality_reduction.py` & `alchemite_apiclient-0.54.0/example/example_dimensionality_reduction.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/example/example_download.py` & `alchemite_apiclient-0.54.0/example/example_download.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/example/example_export_import.py` & `alchemite_apiclient-0.54.0/example/example_export_import.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/example/example_hyperopt.py` & `alchemite_apiclient-0.54.0/example/example_hyperopt.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/example/example_importance.py` & `alchemite_apiclient-0.54.0/example/example_importance.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/example/example_optimize.py` & `alchemite_apiclient-0.54.0/example/example_optimize.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/example/example_outliers.py` & `alchemite_apiclient-0.54.0/example/example_outliers.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/example/example_output_tolerance.py` & `alchemite_apiclient-0.54.0/example/example_output_tolerance.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/example/example_preload.py` & `alchemite_apiclient-0.54.0/example/example_preload.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/example/example_query.py` & `alchemite_apiclient-0.54.0/example/example_query.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/example/example_sensitivity.py` & `alchemite_apiclient-0.54.0/example/example_sensitivity.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/example/example_suggest_additional.py` & `alchemite_apiclient-0.54.0/example/example_suggest_additional.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/example/example_suggest_historic.py` & `alchemite_apiclient-0.54.0/example/example_suggest_historic.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/example/example_suggest_initial.py` & `alchemite_apiclient-0.54.0/example/example_suggest_initial.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/example/example_suggest_missing.py` & `alchemite_apiclient-0.54.0/example/example_suggest_missing.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/example/example_training_outliers.py` & `alchemite_apiclient-0.54.0/example/example_training_outliers.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/example/example_validate.py` & `alchemite_apiclient-0.54.0/example/example_validate.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/example/example_vector.py` & `alchemite_apiclient-0.54.0/example/example_vector.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/example/optimize_args_steel.json` & `alchemite_apiclient-0.54.0/example/optimize_args_steel.json`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/example/optimize_dependentColumns_args_steel.json` & `alchemite_apiclient-0.54.0/example/optimize_dependentColumns_args_steel.json`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/example/steels.csv` & `alchemite_apiclient-0.54.0/example/steels.csv`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/example/suggest_additional_args_steel.json` & `alchemite_apiclient-0.54.0/example/suggest_additional_args_steel.json`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/pyproject.toml` & `alchemite_apiclient-0.54.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "alchemite_apiclient"
-version = "0.53.0"
+version = "0.54.0"
 authors = [
   { name="Intellegens", email="support@intellegens.com" },
 ]
 description = "A python API client for using Alchemite Analytics"
 keywords = ["Alchemite", "Alchemite API", "Machine Learning", "Artificial Intelligence"]
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `alchemite_apiclient-0.53.0/setup.py` & `alchemite_apiclient-0.54.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "alchemite-apiclient"
-VERSION = "0.53.0"
+VERSION = "0.54.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `alchemite_apiclient-0.53.0/test/test_cornercases.py` & `alchemite_apiclient-0.54.0/test/test_cornercases.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.53.0/test/test_examples.py` & `alchemite_apiclient-0.54.0/test/test_examples.py`

 * *Files identical despite different names*

