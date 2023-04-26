# Comparing `tmp/castoredc_api-0.1.7.post1.tar.gz` & `tmp/castoredc_api-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "castoredc_api-0.1.7.post1.tar", last modified: Wed Mar 15 14:44:31 2023, max compression
+gzip compressed data, was "castoredc_api-0.1.8.tar", last modified: Wed Apr 26 07:36:11 2023, max compression
```

## Comparing `castoredc_api-0.1.7.post1.tar` & `castoredc_api-0.1.8.tar`

### file list

```diff
@@ -1,138 +1,138 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 14:44:31.921403 castoredc_api-0.1.7.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    24472 2023-03-15 14:44:31.921403 castoredc_api-0.1.7.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24084 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 14:44:31.901403 castoredc_api-0.1.7.post1/castoredc_api/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 14:44:31.901403 castoredc_api-0.1.7.post1/castoredc_api/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/auth/auth_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 14:44:31.901403 castoredc_api-0.1.7.post1/castoredc_api/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53791 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/client/castoredc_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/client/client_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 14:44:31.901403 castoredc_api-0.1.7.post1/castoredc_api/importer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/importer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9542 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/importer/async_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/importer/async_import.py
--rw-r--r--   0 runner    (1001) docker     (123)    27857 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/importer/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/importer/import_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/importer/sync_import.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 14:44:31.901403 castoredc_api-0.1.7.post1/castoredc_api/study/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/study/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 14:44:31.905403 castoredc_api-0.1.7.post1/castoredc_api/study/castor_objects/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/study/castor_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13811 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/study/castor_objects/castor_data_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/study/castor_objects/castor_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/study/castor_objects/castor_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/study/castor_objects/castor_form_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/study/castor_objects/castor_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/study/castor_objects/castor_report_form_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/study/castor_objects/castor_step.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/study/castor_objects/castor_study_form_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/study/castor_objects/castor_survey_form_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    43302 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/study/castor_study.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 14:44:31.905403 castoredc_api-0.1.7.post1/castoredc_api/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 14:44:31.909403 castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17457 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/data_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/fixtures_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/helpers_api_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_audit_trail_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_country_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)    33404 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_data_point_collection_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_device_token_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_econsent_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_export_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_field_dependency_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_field_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_field_optiongroup_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_field_validation_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_institute_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_metadata_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_metadata_type_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_phase_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_query_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_randomization_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_record_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_record_progress_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)    10351 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_report_data_entry_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_report_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_report_instance_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_report_step_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_role_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_step_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     7794 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_study_data_entry_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)    10233 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_study_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_study_statistics_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_survey_data_entry_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)    25685 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_survey_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_survey_step_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_user_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_verification_endpoints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 14:44:31.913403 castoredc_api-0.1.7.post1/castoredc_api/tests/test_castor_objects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_castor_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17050 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_castor_objects/fixtures_castor_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_castor_objects/helpers_castor_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     6867 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_castor_objects/test_castor_data_point.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_castor_objects/test_castor_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_castor_objects/test_castor_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_castor_objects/test_castor_form_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_castor_objects/test_castor_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_castor_objects/test_castor_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_castor_objects/test_castor_study.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 14:44:31.913403 castoredc_api-0.1.7.post1/castoredc_api/tests/test_import/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_import/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_import/fixtures_import.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 14:44:31.913403 castoredc_api-0.1.7.post1/castoredc_api/tests/test_import/test_async_import/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_import/test_async_import/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_import/test_async_import/test_import_merge_async.py
--rw-r--r--   0 runner    (1001) docker     (123)    15243 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_import/test_async_import/test_import_report_async.py
--rw-r--r--   0 runner    (1001) docker     (123)    13517 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_import/test_async_import/test_import_study_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     9121 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_import/test_async_import/test_import_study_format_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     9261 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_import/test_async_import/test_import_survey_async.py
--rw-r--r--   0 runner    (1001) docker     (123)    12678 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_import/test_async_import/test_import_translation_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_import/test_async_import/test_import_validation_errors_async.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 14:44:31.913403 castoredc_api-0.1.7.post1/castoredc_api/tests/test_import/test_prepare_import/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_import/test_prepare_import/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_import/test_prepare_import/test_column_translation.py
--rw-r--r--   0 runner    (1001) docker     (123)    18400 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_import/test_prepare_import/test_create_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_import/test_prepare_import/test_create_upload_format.py
--rw-r--r--   0 runner    (1001) docker     (123)    21837 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_import/test_prepare_import/test_format_translation.py
--rw-r--r--   0 runner    (1001) docker     (123)    35894 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_import/test_prepare_import/test_label_translation.py
--rw-r--r--   0 runner    (1001) docker     (123)    38852 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_import/test_prepare_import/test_value_translation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 14:44:31.917403 castoredc_api-0.1.7.post1/castoredc_api/tests/test_import/test_sync_import/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_import/test_sync_import/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7632 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_import/test_sync_import/test_import_merge_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)    11945 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_import/test_sync_import/test_import_report_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     9000 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_import/test_sync_import/test_import_study_format_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)    10846 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_import/test_sync_import/test_import_study_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     7880 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_import/test_sync_import/test_import_survey_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)    12478 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_import/test_sync_import/test_import_translation_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_import/test_sync_import/test_import_validation_errors_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 14:44:31.917403 castoredc_api-0.1.7.post1/castoredc_api/tests/test_integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_integration/data_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_integration/fixtures_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_integration/test_data_interpretation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_integration/test_data_interpretation_formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_integration/test_data_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_integration/test_data_structure_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_integration/test_special_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_integration/test_structure_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 14:44:31.917403 castoredc_api-0.1.7.post1/castoredc_api/tests/test_output/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_output/test_csv_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_output/test_csv_output_archived.py
--rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/castoredc_api/tests/test_output/test_csv_output_format.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 14:44:31.901403 castoredc_api-0.1.7.post1/castoredc_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24472 2023-03-15 14:44:31.000000 castoredc_api-0.1.7.post1/castoredc_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7053 2023-03-15 14:44:31.000000 castoredc_api-0.1.7.post1/castoredc_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 14:44:31.000000 castoredc_api-0.1.7.post1/castoredc_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-03-15 14:44:31.000000 castoredc_api-0.1.7.post1/castoredc_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-15 14:44:31.000000 castoredc_api-0.1.7.post1/castoredc_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-15 14:44:31.921403 castoredc_api-0.1.7.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-03-15 14:43:59.000000 castoredc_api-0.1.7.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:36:11.775252 castoredc_api-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    24466 2023-04-26 07:36:11.779252 castoredc_api-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24084 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:36:11.759251 castoredc_api-0.1.8/castoredc_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:36:11.759251 castoredc_api-0.1.8/castoredc_api/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/auth/auth_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:36:11.763251 castoredc_api-0.1.8/castoredc_api/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53662 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/client/castoredc_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/client/client_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:36:11.763251 castoredc_api-0.1.8/castoredc_api/importer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/importer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9989 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/importer/async_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/importer/async_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27909 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/importer/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/importer/import_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/importer/sync_import.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:36:11.763251 castoredc_api-0.1.8/castoredc_api/study/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/study/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:36:11.763251 castoredc_api-0.1.8/castoredc_api/study/castor_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/study/castor_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13811 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/study/castor_objects/castor_data_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/study/castor_objects/castor_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/study/castor_objects/castor_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/study/castor_objects/castor_form_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/study/castor_objects/castor_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/study/castor_objects/castor_report_form_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/study/castor_objects/castor_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/study/castor_objects/castor_study_form_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/study/castor_objects/castor_survey_form_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44398 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/study/castor_study.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:36:11.763251 castoredc_api-0.1.8/castoredc_api/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:36:11.771252 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17457 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/data_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/fixtures_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/helpers_api_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_audit_trail_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_country_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33404 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_data_point_collection_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_device_token_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_econsent_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_export_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_field_dependency_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_field_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_field_optiongroup_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_field_validation_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_institute_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_metadata_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_metadata_type_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_phase_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_query_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_randomization_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_record_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_record_progress_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10351 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_report_data_entry_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_report_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_report_instance_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_report_step_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_role_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_step_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7794 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_study_data_entry_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10233 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_study_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_study_statistics_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_survey_data_entry_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25687 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_survey_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_survey_step_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_user_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_verification_endpoints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:36:11.771252 castoredc_api-0.1.8/castoredc_api/tests/test_castor_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_castor_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17050 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_castor_objects/fixtures_castor_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_castor_objects/helpers_castor_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6867 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_castor_objects/test_castor_data_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_castor_objects/test_castor_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_castor_objects/test_castor_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_castor_objects/test_castor_form_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_castor_objects/test_castor_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_castor_objects/test_castor_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_castor_objects/test_castor_study.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:36:11.771252 castoredc_api-0.1.8/castoredc_api/tests/test_import/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_import/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_import/fixtures_import.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:36:11.771252 castoredc_api-0.1.8/castoredc_api/tests/test_import/test_async_import/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_import/test_async_import/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_import/test_async_import/test_import_merge_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15243 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_import/test_async_import/test_import_report_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13517 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_import/test_async_import/test_import_study_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9121 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_import/test_async_import/test_import_study_format_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9261 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_import/test_async_import/test_import_survey_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12678 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_import/test_async_import/test_import_translation_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_import/test_async_import/test_import_validation_errors_async.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:36:11.775252 castoredc_api-0.1.8/castoredc_api/tests/test_import/test_prepare_import/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_import/test_prepare_import/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_import/test_prepare_import/test_column_translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18400 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_import/test_prepare_import/test_create_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_import/test_prepare_import/test_create_upload_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21837 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_import/test_prepare_import/test_format_translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35894 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_import/test_prepare_import/test_label_translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38852 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_import/test_prepare_import/test_value_translation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:36:11.775252 castoredc_api-0.1.8/castoredc_api/tests/test_import/test_sync_import/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_import/test_sync_import/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11009 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_import/test_sync_import/test_import_merge_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11945 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_import/test_sync_import/test_import_report_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9000 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_import/test_sync_import/test_import_study_format_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10846 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_import/test_sync_import/test_import_study_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7880 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_import/test_sync_import/test_import_survey_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12478 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_import/test_sync_import/test_import_translation_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_import/test_sync_import/test_import_validation_errors_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:36:11.775252 castoredc_api-0.1.8/castoredc_api/tests/test_integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_integration/data_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_integration/fixtures_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_integration/test_data_interpretation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_integration/test_data_interpretation_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_integration/test_data_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_integration/test_data_structure_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_integration/test_special_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_integration/test_structure_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:36:11.775252 castoredc_api-0.1.8/castoredc_api/tests/test_output/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_output/test_csv_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_output/test_csv_output_archived.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/castoredc_api/tests/test_output/test_csv_output_format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:36:11.759251 castoredc_api-0.1.8/castoredc_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24466 2023-04-26 07:36:11.000000 castoredc_api-0.1.8/castoredc_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7053 2023-04-26 07:36:11.000000 castoredc_api-0.1.8/castoredc_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 07:36:11.000000 castoredc_api-0.1.8/castoredc_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-26 07:36:11.000000 castoredc_api-0.1.8/castoredc_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-26 07:36:11.000000 castoredc_api-0.1.8/castoredc_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-26 07:36:11.779252 castoredc_api-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-26 07:35:34.000000 castoredc_api-0.1.8/setup.py
```

### Comparing `castoredc_api-0.1.7.post1/LICENSE.md` & `castoredc_api-0.1.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/PKG-INFO` & `castoredc_api-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: castoredc_api
-Version: 0.1.7.post1
+Version: 0.1.8
 Summary: Python wrapper for the Castor EDC API
 Home-page: https://github.com/reiniervlinschoten/castoredc_api
 Author: Reinier van Linschoten
 Author-email: mail@reiniervl.com
 Maintainer: Reinier van Linschoten
 Maintainer-email: mail@reiniervl.com
 License: MIT
@@ -19,15 +19,15 @@
 [![black](https://github.com/reiniervlinschoten/castoredc_api/actions/workflows/black.yml/badge.svg)](https://github.com/reiniervlinschoten/castoredc_api/actions/workflows/black.yml)
 
 [![pypi](https://img.shields.io/pypi/v/castoredc_api)](https://pypi.org/project/castoredc-api/)
 [![conda](https://img.shields.io/conda/v/reiniervl/castoredc_api)](https://anaconda.org/reiniervl/castoredc_api)
 [![conda-forge](https://img.shields.io/conda/v/conda-forge/castoredc_api)](https://anaconda.org/conda-forge/castoredc_api)
 
 ## Features
-#### Supports CastorEDC Release 2022.5
+#### Supports CastorEDC Release 2023.1
 
 This is a Python package for interacting with the API of Castor Electronic Data Capture (EDC). 
 The package contains functions to interact with all the endpoints defined on https://data.castoredc.com/api#/.
 Within the package are functions for easy export and import of your data through the API.
 
 ### Export
 Supported export formats are
```

### Comparing `castoredc_api-0.1.7.post1/README.md` & `castoredc_api-0.1.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![black](https://github.com/reiniervlinschoten/castoredc_api/actions/workflows/black.yml/badge.svg)](https://github.com/reiniervlinschoten/castoredc_api/actions/workflows/black.yml)
 
 [![pypi](https://img.shields.io/pypi/v/castoredc_api)](https://pypi.org/project/castoredc-api/)
 [![conda](https://img.shields.io/conda/v/reiniervl/castoredc_api)](https://anaconda.org/reiniervl/castoredc_api)
 [![conda-forge](https://img.shields.io/conda/v/conda-forge/castoredc_api)](https://anaconda.org/conda-forge/castoredc_api)
 
 ## Features
-#### Supports CastorEDC Release 2022.5
+#### Supports CastorEDC Release 2023.1
 
 This is a Python package for interacting with the API of Castor Electronic Data Capture (EDC). 
 The package contains functions to interact with all the endpoints defined on https://data.castoredc.com/api#/.
 Within the package are functions for easy export and import of your data through the API.
 
 ### Export
 Supported export formats are
```

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/client/castoredc_api_client.py` & `castoredc_api-0.1.8/castoredc_api/client/castoredc_api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -307,25 +307,25 @@
                 filled_on = datetime.strptime(filled_on, "%Y-%m-%d %H:%M:%S")
             post_data["all_fields_filled_on"] = filled_on.strftime("%Y-%m-%d %H:%M:%S")
         return self.sync_post(url, post_data)
 
     # EXPORT
     @RateLimiter(**client_options.SYNC_OPTIONS)
     def export_study_data(
-        self, exclude_empty_surveys=False, exclude_empty_reports=False
+        self, exclude_empty_surveys=False, exclude_empty_reports=False, archived=False
     ):
         """Returns a list of dicts containing all data in the study (study, surveys, reports)."""
         url = self.study_url + "/export/data"
         return self.sync_get(
             url=url,
             params={
                 "exclude_empty_surveys": exclude_empty_surveys,
                 "exclude_empty_reports": exclude_empty_reports,
+                "archived": archived,
             },
-            timeout=httpx.Timeout(10.0, read=300),
         )["content"]
 
     @RateLimiter(**client_options.SYNC_OPTIONS)
     def export_study_structure(self):
         """Returns a list of dicts containing the structure of the study."""
         url = self.study_url + "/export/structure"
         return self.sync_get(url=url, params={})["content"]
@@ -1260,20 +1260,17 @@
             url = self.study_url + endpoint
         else:
             url = self.base_url + endpoint
         response = self.sync_get(url=url, params={})
         return response["total_items"]
 
     # Synchronous API Interaction
-    def sync_get(self, url: str, params: dict, timeout=None) -> dict:
+    def sync_get(self, url: str, params: dict) -> dict:
         """Synchronous querying of Castor API with a single get requests."""
-        if timeout:
-            response = self.client.get(url=url, params=params, timeout=timeout)
-        else:
-            response = self.client.get(url=url, params=params)
+        response = self.client.get(url=url, params=params)
         return self.handle_response(response)
 
     def sync_post(self, url, body):
         """Helper function to post body to url."""
         response = self.client.post(url=url, json=body)
         response.raise_for_status()
         return response.json()
```

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/client/client_options.py` & `castoredc_api-0.1.8/castoredc_api/client/client_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """File to hold settings for interacting with the Castor EDC API."""
 
 import time
 import httpx
 
 MAX_CONNECTIONS = 15
-TIMEOUT = httpx.Timeout(10.0, read=60)
+TIMEOUT = httpx.Timeout(10.0, read=600)
 LIMITS = httpx.Limits(max_connections=MAX_CONNECTIONS)
 # Rate limit is 600 calls per 10 minutes per api endpoint
 SYNC_LIMIT = 600
 PERIOD_LIMIT = 600
 ASYNC_LIMIT = SYNC_LIMIT / MAX_CONNECTIONS
```

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/importer/async_helpers.py` & `castoredc_api-0.1.8/castoredc_api/importer/async_helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,19 +58,23 @@
         url = (
             study.client.study_url
             + f"/record/{item['row']['record_id']}/data-point-collection/study"
         )
         json = {"common": item["common"], "data": item["body"]}
         feedback = await async_upload_data(client, feedback, json, study, url)
     except httpx.HTTPStatusError as error:
-        feedback["error"] = error.response.json()
+        try:
+            feedback["error"] = error.response.json()
+        except JSONDecodeError:
+            feedback["error"] = (
+                f"JSONDecodeError while handling error for {error.request.url} \n"
+                f"with status code {error.response.status_code}"
+            )
     except httpx.RequestError as error:
         feedback["error"] = f"Request Error for {error.request.url}."
-    except JSONDecodeError:
-        feedback["error"] = "JSONDecodeError while handling Error."
     return feedback
 
 
 async def async_update_survey_data(
     data: list, study: "CastorStudy", change_reason: str
 ) -> list:
     """Updates the Castor EDC database with given survey datapoints."""
@@ -124,19 +128,23 @@
             study.client.study_url
             + f"/record/{item['row']['record_id']}/data-point-collection/"
             f"survey-package-instance/{instance['id']}"
         )
         json = {"data": body, "common": {"change_reason": change_reason}}
         feedback = await async_upload_data(client, feedback, json, study, url)
     except httpx.HTTPStatusError as error:
-        feedback["error"] = error.response.json()
+        try:
+            feedback["error"] = error.response.json()
+        except JSONDecodeError:
+            feedback["error"] = (
+                f"JSONDecodeError while handling error for {error.request.url} \n"
+                f"with status code {error.response.status_code}"
+            )
     except httpx.RequestError as error:
         feedback["error"] = f"Request Error for {error.request.url}."
-    except JSONDecodeError:
-        feedback["error"] = "JSONDecodeError while handling Error."
     return feedback
 
 
 async def async_create_survey_package_instance(
     survey_package_id: str,
     record_id: str,
     email_address: str,
@@ -211,19 +219,23 @@
             study.client.study_url
             + f"/record/{item['row']['record_id']}/data-point-collection/"
             f"report-instance/{instance['id']}"
         )
         json = {"data": body, "common": item["common"]}
         feedback = await async_upload_data(client, feedback, json, study, url)
     except httpx.HTTPStatusError as error:
-        feedback["error"] = error.response.json()
+        try:
+            feedback["error"] = error.response.json()
+        except JSONDecodeError:
+            feedback["error"] = (
+                f"JSONDecodeError while handling error for {error.request.url} \n"
+                f"with status code {error.response.status_code}"
+            )
     except httpx.RequestError as error:
         feedback["error"] = f"Request Error for {error.request.url}."
-    except JSONDecodeError:
-        feedback["error"] = "JSONDecodeError while handling Error."
     return feedback
 
 
 async def async_create_report_instance(
     report_id: str,
     record_id: str,
     report_name_custom: str,
```

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/importer/async_import.py` & `castoredc_api-0.1.8/castoredc_api/importer/async_import.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/importer/helpers.py` & `castoredc_api-0.1.8/castoredc_api/importer/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,25 +161,15 @@
         if target_field.step.form.form_name != target_name:
             return {
                 new_name[0]: [
                     "Error: field is not child of given target" for _ in to_import
                 ]
             }
     elif target == "Survey":
-        # Check for surveys (need to extract all forms in given survey package)
-        # TODO Add survey package structure building to Study object # pylint: disable=fixme
-        # And then remove it here
-        package = next(
-            (
-                item
-                for item in study.client.all_survey_packages()
-                if item["name"] == target_name
-            ),
-            None,
-        )
+        package = study.all_survey_packages.get(target_name, None)
         if package is None:
             return {
                 new_name[0]: ["Error: survey package does not exist" for _ in to_import]
             }
         if target_field.step.form.form_name not in [
             survey["name"] for survey in package["_embedded"]["surveys"]
         ]:
@@ -351,18 +341,19 @@
     options: dict,
     label_data: bool,
     parent_value: typing.Optional[str],
     variable_translation: typing.Optional[dict],
     other_name: str,
 ) -> typing.Optional[list]:
     """Translates a list of values split by ; into Castor Values."""
-    # If the datapoint was None or NaN, return an empty datapoint
-    if not isinstance(values, list):
-        if pd.isnull(values):
-            new_values = None
+    # If the datapoint was Missing, return an empty datapoint
+    if values is None:
+        new_values = None
+    elif values[0] == "MISSING-DATA-POINT":
+        new_values = None
 
     else:
         new_values = []
         translate_dict = get_translation_dict(other_name, variable_translation)
         # If labelled data was provided, translate this to optiongroup values
         # False or parent_value for failures
         if label_data:
@@ -606,15 +597,15 @@
     return new_value
 
 
 def merge_row(row: pd.Series) -> str:
     """Merges multiple columns in a row to a single column."""
     row = row.dropna()
     row = ";".join(row.values.astype(str))
-    row = np.nan if row == "" else row
+    row = "MISSING-DATA-POINT" if row == "" else row
     return row
 
 
 def merge_columns(to_upload: pd.DataFrame, path_to_merge: str) -> pd.DataFrame:
     """Merges multiple columns as defined in path_to_merge to a single column"""
     merge_link = create_merge_translation(path_to_merge)
     # Translate Values
@@ -688,19 +679,29 @@
     }
     return formatted_feedback_row
 
 
 def handle_http_error(error, imported, row):
     """Handles HTTP Errors by outputting imported data and raising an error."""
     if isinstance(error, httpx.HTTPStatusError):
+        try:
+            row["error"] = error.response.json()
+        except JSONDecodeError:
+            row["error"] = (
+                f"JSONDecodeError while handling error for {error.request.url} \n"
+                f"with status code {error.response.status_code}"
+            )
         row["error"] = error.response.json()
     elif isinstance(error, httpx.RequestError):
         row["error"] = f"Request Error for {error.request.url}."
     elif isinstance(error, JSONDecodeError):
-        row["error"] = f"JSONDecodeError while handling Error for {error.request.url}."
+        row["error"] = (
+            f"JSONDecodeError while handling error for {error.request.url} \n"
+            f"with status code {error.response.status_code}"
+        )
     # Add error row to the dataset
     imported.append(row)
     # Output data for error checking
     pd.DataFrame(imported).to_csv(
         pathlib.Path(
             pathlib.Path.cwd(),
             "output",
```

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/importer/import_data.py` & `castoredc_api-0.1.8/castoredc_api/importer/import_data.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/importer/sync_import.py` & `castoredc_api-0.1.8/castoredc_api/importer/sync_import.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/study/castor_objects/castor_data_point.py` & `castoredc_api-0.1.8/castoredc_api/study/castor_objects/castor_data_point.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/study/castor_objects/castor_field.py` & `castoredc_api-0.1.8/castoredc_api/study/castor_objects/castor_field.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/study/castor_objects/castor_form.py` & `castoredc_api-0.1.8/castoredc_api/study/castor_objects/castor_form.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/study/castor_objects/castor_form_instance.py` & `castoredc_api-0.1.8/castoredc_api/study/castor_objects/castor_form_instance.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/study/castor_objects/castor_record.py` & `castoredc_api-0.1.8/castoredc_api/study/castor_objects/castor_record.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/study/castor_objects/castor_report_form_instance.py` & `castoredc_api-0.1.8/castoredc_api/study/castor_objects/castor_report_form_instance.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/study/castor_objects/castor_step.py` & `castoredc_api-0.1.8/castoredc_api/study/castor_objects/castor_step.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/study/castor_objects/castor_study_form_instance.py` & `castoredc_api-0.1.8/castoredc_api/study/castor_objects/castor_study_form_instance.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/study/castor_objects/castor_survey_form_instance.py` & `castoredc_api-0.1.8/castoredc_api/study/castor_objects/castor_survey_form_instance.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/study/castor_study.py` & `castoredc_api-0.1.8/castoredc_api/study/castor_study.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,26 +70,28 @@
         # Dictionary to store the relationship between a form instance and its form ID
         self.form_links = {}
         # List of all records in the study - data
         self.records = {}
         # List of dictionaries of optiongroups
         self.optiongroups = {}
         # Container variables to save time querying the database
-        self.__all_report_instances = {}
+        self.all_report_instances = {}
+        self.all_survey_packages = {}
 
     # STRUCTURE MAPPING
     def map_structure(self) -> None:
         """Maps the structure for the study."""
         # Reset structure & data
         self.forms_on_id = {}
         self.forms_on_name = {}
         self.form_links = {}
         self.records = {}
         self.optiongroups = {}
-        self.__all_report_instances = {}
+        self.all_report_instances = {}
+        self.all_survey_packages = {}
         # Get the structure from the API
         print("Downloading Study Structure.", flush=True, file=sys.stderr)
         data = self.client.export_study_structure()
         # Loop over all fields
         for field in tqdm(data, desc="Mapping Study Structure"):
             # Check if the form for the field exists, if not, create it
             form = self.get_single_form(field["Form Collection ID"])
@@ -124,87 +126,97 @@
         # Augment field data
         self.__load_field_information()
 
         # Map the field dependencies and optiongroups
         self.__map_field_dependencies()
         self.__load_optiongroups()
 
+        # Map the survey packages
+        self.__map_survey_packages()
+
     # DATA MAPPING
-    def map_data(self) -> None:
-        """Maps the data for the study."""
+    def map_data(self, archived: bool = False) -> None:
+        """Maps the data for the study. Archived controls whether archived data is extracted"""
         self.map_structure()
-        self.update_links()
-        self.__link_data()
-        self.__load_record_information()
-        self.__load_survey_information()
+        self.update_links(archived)
+        self.__link_data(archived)
+        self.__load_record_information(archived)
+        self.__load_survey_information(archived)
         self.__load_report_information()
 
-    def update_links(self) -> None:
+    def update_links(self, archived: bool) -> None:
         """Creates the links between form and form instances."""
         # Reset form links
         self.form_links = {}
         # Get the name of the survey forms, as the export data can only be linked on name, not on id
         print("Downloading Surveys.", flush=True, file=sys.stderr)
         surveys = self.client.all_surveys()
         self.form_links["Survey"] = {survey["name"]: survey["id"] for survey in surveys}
         # Get all report instances that need to be linked
         print("Downloading Report Instances.", flush=True, file=sys.stderr)
         # Save this data from the database to save time later
         report_instances = self.client.all_report_instances(archived=0)
-        archived_report_instances = self.client.all_report_instances(archived=1)
+        if archived:
+            archived_report_instances = self.client.all_report_instances(archived=1)
+            report_instances = report_instances + archived_report_instances
         # Create dict with link id: object
-        self.__all_report_instances = {
+        self.all_report_instances = {
             report_instance["id"]: report_instance
-            for report_instance in report_instances + archived_report_instances
+            for report_instance in report_instances
         }
         # Create dict with link instance_id: form_id
         self.form_links["Report"] = {
-            instance_id: self.__all_report_instances[instance_id]["_embedded"][
-                "report"
-            ]["id"]
-            for instance_id in self.__all_report_instances
+            instance_id: self.all_report_instances[instance_id]["_embedded"]["report"][
+                "id"
+            ]
+            for instance_id in self.all_report_instances
         }
 
     # OPTIONGROUPS
     def __load_optiongroups(self) -> None:
         """Loads all optiongroups through the client"""
         # Get the optiongroups
         print("Downloading Optiongroups", flush=True, file=sys.stderr)
         optiongroups = self.client.all_field_optiongroups()
         self.optiongroups = {
             optiongroup["id"]: optiongroup for optiongroup in optiongroups
         }
 
     # AUXILIARY DATA
-    def __load_record_information(self) -> None:
+    def __load_record_information(self, archived: bool) -> None:
         """Adds auxiliary data to records."""
         print("Downloading Record Information.", flush=True, file=sys.stderr)
-        record_data = self.client.all_records()
+        record_data = (
+            self.client.all_records()
+            if archived
+            else self.client.all_records(archived=0)
+        )
         for record_api in tqdm(record_data, desc="Augmenting Record Data"):
             record = self.get_single_record(record_api["id"])
             record.institute = record_api["_embedded"]["institute"]["name"]
             record.randomisation_group = record_api["randomization_group_name"]
             record.randomisation_datetime = self.__get_date_or_none(
                 record_api["randomized_on"]
             )
             record.archived = record_api["archived"]
 
-    def __load_survey_information(self) -> None:
+    def __load_survey_information(self, archived: bool) -> None:
         """Adds auxiliary data to survey forms."""
         print("Downloading Survey Information.", flush=True, file=sys.stderr)
         survey_package_data = self.client.all_survey_package_instances()
         # Create mapping {survey_instance_id: survey_package}
         survey_data = {
             survey["id"]: {
                 "package": package,
                 "record": package["record_id"],
                 "survey": survey,
             }
             for package in survey_package_data
             for survey in package["_embedded"]["survey_instances"]
+            if not package["archived"] or archived
         }
         for survey_instance, values in tqdm(
             survey_data.items(), desc="Augmenting Survey Data"
         ):
             # Test if instance in study
             local_instance = self.get_single_form_instance_on_id(
                 instance_id=survey_instance, record_id=values["record"]
@@ -224,15 +236,15 @@
             local_instance.survey_package_name = values["package"][
                 "survey_package_name"
             ]
 
     def __load_report_information(self) -> None:
         """Adds auxiliary data to report forms."""
         for instance_id, report_instance in tqdm(
-            self.__all_report_instances.items(),
+            self.all_report_instances.items(),
             "Augmenting Report Data",
         ):
             # Test if instance in study
             local_instance = self.get_single_form_instance_on_id(
                 instance_id=instance_id, record_id=report_instance["record_id"]
             )
             local_instance.created_on = datetime.strptime(
@@ -270,14 +282,21 @@
             if dictionary is None
             else datetime.strptime(dictionary["date"], "%Y-%m-%d %H:%M:%S.%f").strftime(
                 self.configuration["datetime_seconds"]
             )
         )
         return date
 
+    # SURVEY PACKAGES
+    def __map_survey_packages(self) -> None:
+        """Maps all survey packages for easier finding."""
+        print("Downloading Survey Packages", flush=True, file=sys.stderr)
+        all_survey_packages = self.client.all_survey_packages()
+        self.all_survey_packages = {item["name"]: item for item in all_survey_packages}
+
     # FIELD DEPENDENCIES
     def __map_field_dependencies(self) -> None:
         """Retrieves all field_dependencies and links them to the right field."""
         print("Downloading Field Dependencies", flush=True, file=sys.stderr)
         dependencies = self.client.all_field_dependencies()
         # Format to dict of {child_id: {"parent_field": parent_field, "parent_value": value}
         dependencies = {
@@ -289,27 +308,29 @@
         }
         for child_id in dependencies:
             self.get_single_field(child_id).field_dependency = dependencies[child_id]
 
     # DATA ANALYSIS
     def export_to_dataframe(self, archived=False) -> dict:
         """Exports all data from a study into a dict of dataframes for statistical analysis."""
-        self.map_data()
+        # TODO: change this to the correct archived, # pylint: disable=fixme
+        #  fails now because the parameter does not seem to be handled correctly server side
+        self.map_data(archived=True)
         dataframes = {
             "Study": self.__export_study_data(archived),
             "Surveys": self.__export_survey_data(archived),
             "Reports": self.__export_report_data(archived),
         }
         return dataframes
 
     def export_to_csv(self, archived=False) -> dict:
         """Exports all data to csv files.
         Returns dict with file locations."""
         now = f"{datetime.now().strftime('%Y%m%d %H%M%S.%f')[:-3]}"
-        dataframes = self.export_to_dataframe(archived)
+        dataframes = self.export_to_dataframe(archived=archived)
         # Instantiate output folder
         pathlib.Path(pathlib.Path.cwd(), "output").mkdir(parents=True, exist_ok=True)
         # Export dataframes
         dataframes["Study"] = self.export_dataframe_to_csv(
             dataframes["Study"], "Study", now
         )
         for survey in dataframes["Surveys"]:
@@ -553,19 +574,19 @@
             form_id = self.form_links[instance_type][instance_id]
             form = self.get_single_form(form_id)
         else:
             raise CastorException(f"{instance_type} is not a form type.")
         return form
 
     # PRIVATE HELPER FUNCTIONS
-    def __link_data(self) -> None:
+    def __link_data(self, archived: bool) -> None:
         """Links the study data"""
         # Get the data from the API
         print("Downloading Study Data.", flush=True, file=sys.stderr)
-        data = self.client.export_study_data()
+        data = self.client.export_study_data(archived=archived)
 
         # Loop over all fields
         for field in tqdm(data, desc="Mapping Data"):
             self.__handle_row(field)
 
     def __handle_row(self, field):
         """Handles a row from the export data."""
```

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/data_models.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/data_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -497,15 +497,15 @@
     ],
     "intro_text": [
         str,
     ],
     "outro_text": [
         str,
     ],
-    "survey_steps": [
+    "survey_forms": [
         list,
     ],
     "_links": [
         dict,
     ],
 }
```

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/fixtures_api.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/fixtures_api.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/helpers_api_endpoints.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/helpers_api_endpoints.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_audit_trail_endpoints.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_audit_trail_endpoints.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             date_to="2022-06-28",
             user_id="B23ABCC4-3A53-FB32-7B78-3960CC907F25",
         )[0]
         assert audit_trail == self.test_audit_trail_model
 
     test_audit_trail_model = {
         "datetime": {
-            "date": "2022-06-28 05:13:49.000000",
+            "date": "2022-06-28 09:13:49.000000",
             "timezone_type": 3,
             "timezone": "Europe/Amsterdam",
         },
         "event_type": "Survey created",
         "user_id": "B23ABCC4-3A53-FB32-7B78-3960CC907F25",
         "user_role": None,
         "user_name": "Reinier van Linschoten",
```

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_country_endpoints.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_country_endpoints.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_data_point_collection_endpoints.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_data_point_collection_endpoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,63 +28,63 @@
     survey_package_data_point_model_keys = survey_package_data_point_model.keys()
 
     test_report_instance_data_points = [
         {
             "field_id": "05353909-4BFB-4547-8700-AD6755FE82DB",
             "field_value": "1",
             "record_id": "000005",
-            "updated_on": "2019-10-28 12:05:28",
+            "updated_on": "2019-10-28 14:05:28",
             "report_instance_id": "124EBE17-8AEF-4A74-BBA7-68DF75693FBD",
             "report_instance_name": "46286061",
         },
         {
             "field_id": "345C89CE-4CF9-4C44-8186-CF813EA7C181",
             "field_value": "1",
             "record_id": "000005",
-            "updated_on": "2019-10-28 12:05:28",
+            "updated_on": "2019-10-28 14:05:28",
             "report_instance_id": "124EBE17-8AEF-4A74-BBA7-68DF75693FBD",
             "report_instance_name": "46286061",
         },
         {
             "field_id": "9E780182-2DF6-423B-A3BE-7934BFED0747",
             "field_value": "1",
             "record_id": "000005",
-            "updated_on": "2019-10-28 12:05:28",
+            "updated_on": "2019-10-28 14:05:28",
             "report_instance_id": "124EBE17-8AEF-4A74-BBA7-68DF75693FBD",
             "report_instance_name": "46286061",
         },
         {
             "field_id": "9F64DFE1-4C5E-4BCC-93B6-3624FA9FC2A4",
             "field_value": "1",
             "record_id": "000005",
-            "updated_on": "2019-10-28 12:05:28",
+            "updated_on": "2019-10-28 14:05:28",
             "report_instance_id": "124EBE17-8AEF-4A74-BBA7-68DF75693FBD",
             "report_instance_name": "46286061",
         },
         {
             "field_id": "C8BD45CE-46C3-43D8-BD2A-DF584A046CF7",
             "field_value": "1",
             "record_id": "000005",
-            "updated_on": "2019-10-28 12:05:28",
+            "updated_on": "2019-10-28 14:05:28",
             "report_instance_id": "124EBE17-8AEF-4A74-BBA7-68DF75693FBD",
             "report_instance_name": "46286061",
         },
         {
             "field_id": "CF963988-E9CE-4CEB-A706-CDFA4916A934",
             "field_value": "1",
             "record_id": "000005",
-            "updated_on": "2019-10-28 12:05:28",
+            "updated_on": "2019-10-28 14:05:28",
             "report_instance_id": "124EBE17-8AEF-4A74-BBA7-68DF75693FBD",
             "report_instance_name": "46286061",
         },
         {
             "field_id": "F610012E-B618-40A7-AA36-6C8BD959A1F1",
             "field_value": "1",
             "record_id": "000005",
-            "updated_on": "2019-10-28 12:05:28",
+            "updated_on": "2019-10-28 14:05:28",
             "report_instance_id": "124EBE17-8AEF-4A74-BBA7-68DF75693FBD",
             "report_instance_name": "46286061",
         },
     ]
     test_survey_instance_data_points = [
         {
             "field_id": "5D3843C7-8341-45DD-A769-8A5D24E6CDA5",
@@ -128,51 +128,51 @@
         },
     ]
     test_survey_package_data_points = [
         {
             "field_id": "5D3843C7-8341-45DD-A769-8A5D24E6CDA5",
             "field_value": "1",
             "record_id": "000002",
-            "updated_on": "2020-05-13 12:17:58",
+            "updated_on": "2020-05-13 16:17:58",
             "survey_instance_id": "F61EF287-9BD1-4047-AB46-88E0F69DD120",
             "survey_name": "QOL Survey",
             "survey_package_instance_id": "23B4FD48-BA41-4C9B-BAEF-D5C3DD5F8E5C",
         },
         {
             "field_id": "6C87B052-1289-4AB2-8D4F-D15AF4DDF950",
             "field_value": "1",
             "record_id": "000002",
-            "updated_on": "2020-05-13 12:17:58",
+            "updated_on": "2020-05-13 16:17:58",
             "survey_instance_id": "F61EF287-9BD1-4047-AB46-88E0F69DD120",
             "survey_name": "QOL Survey",
             "survey_package_instance_id": "23B4FD48-BA41-4C9B-BAEF-D5C3DD5F8E5C",
         },
         {
             "field_id": "A6E8C700-1A2B-4A87-AE1F-E8DC2C2F72C2",
             "field_value": "5",
             "record_id": "000002",
-            "updated_on": "2020-05-13 12:17:58",
+            "updated_on": "2020-05-13 16:17:58",
             "survey_instance_id": "F61EF287-9BD1-4047-AB46-88E0F69DD120",
             "survey_name": "QOL Survey",
             "survey_package_instance_id": "23B4FD48-BA41-4C9B-BAEF-D5C3DD5F8E5C",
         },
         {
             "field_id": "ED12B07E-EDA8-4D64-8268-BE751BD5DB36",
             "field_value": "1",
             "record_id": "000002",
-            "updated_on": "2020-05-13 12:17:58",
+            "updated_on": "2020-05-13 16:17:58",
             "survey_instance_id": "F61EF287-9BD1-4047-AB46-88E0F69DD120",
             "survey_name": "QOL Survey",
             "survey_package_instance_id": "23B4FD48-BA41-4C9B-BAEF-D5C3DD5F8E5C",
         },
         {
             "field_id": "FC4FAA2D-08FD-41F7-B482-444B2B6D3116",
             "field_value": "1",
             "record_id": "000002",
-            "updated_on": "2020-05-13 12:17:58",
+            "updated_on": "2020-05-13 16:17:58",
             "survey_instance_id": "F61EF287-9BD1-4047-AB46-88E0F69DD120",
             "survey_name": "QOL Survey",
             "survey_package_instance_id": "23B4FD48-BA41-4C9B-BAEF-D5C3DD5F8E5C",
         },
     ]
 
     @pytest.fixture(scope="function")
```

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_device_token_endpoints.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_device_token_endpoints.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_econsent_endpoints.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_econsent_endpoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from httpx import HTTPStatusError
 
 from castoredc_api.tests.test_api_endpoints.test_record_endpoints import create_record
 
 
 class TestEconsent:
     @pytest.mark.xfail(
-        reason="Econsent not enable on testing databases",
+        reason="Econsent not enabled on testing databases",
         strict=True,
     )
     def test_econsent_get_success(self, client):
         """Tests if econsent returns the proper data."""
         response = client.get_econsent("000024")
         assert response == {
             "econsent_subject_id": "SUBJECTID",
@@ -29,15 +29,15 @@
     def test_econsent_get_failure(self, client):
         """Tests if single token returns an error."""
         with pytest.raises(HTTPStatusError) as e:
             client.get_econsent("FAKE24")
         assert e.value.response.status_code == 404
 
     @pytest.mark.xfail(
-        reason="Econsent not enable on testing databases",
+        reason="Econsent not enabled on testing databases",
         strict=True,
     )
     def test_econsent_post_success(self, client):
         """Tests if econsent returns the proper data."""
         response = client.create_econsent(
             "000024",
             **{
@@ -49,15 +49,15 @@
         assert response == {
             "econsent_subject_id": "SUBJECTID",
             "econsent_study_id": "STUDYID",
             "econsent_region": "STUDYREGION",
         }
 
     @pytest.mark.xfail(
-        reason="Econsent not enable on testing databases",
+        reason="Econsent not enabled on testing databases",
         strict=True,
     )
     def test_econsent_post_failure(self, client):
         """Tests if single token returns an error."""
         with pytest.raises(HTTPStatusError) as e:
             client.create_econsent(
                 "000024",
@@ -66,15 +66,15 @@
                     "econsent_study_id": "STUDYID",
                     "econsent_region": "STUDYREGION",
                 }
             )
         assert e.value.response.status_code == 404
 
     @pytest.mark.xfail(
-        reason="Econsent not enable on testing databases",
+        reason="Econsent not enabled on testing databases",
         strict=True,
     )
     def test_econsent_patch_success(self, client):
         """Tests if econsent returns the proper data."""
         response = client.update_econsent(
             "000024",
             **{
@@ -86,15 +86,15 @@
         assert response == {
             "econsent_subject_id": "SUBJECTID",
             "econsent_study_id": "STUDYID",
             "econsent_region": "STUDYREGION",
         }
 
     @pytest.mark.xfail(
-        reason="Econsent not enable on testing databases",
+        reason="Econsent not enabled on testing databases",
         strict=True,
     )
     def test_econsent_patch_failure(self, client):
         """Tests if single token returns an error."""
         with pytest.raises(HTTPStatusError) as e:
             client.update_econsent(
                 "000024",
```

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_export_endpoints.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_export_endpoints.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_field_dependency_endpoints.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_field_dependency_endpoints.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_field_endpoints.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_field_endpoints.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_field_optiongroup_endpoints.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_field_optiongroup_endpoints.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_field_validation_endpoints.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_field_validation_endpoints.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_institute_endpoints.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_institute_endpoints.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_metadata_endpoints.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_metadata_endpoints.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_metadata_type_endpoints.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_metadata_type_endpoints.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_phase_endpoints.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_phase_endpoints.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_query_endpoints.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_query_endpoints.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         "created_on": {
             "date": "2019-09-23 12:16:37.000000",
             "timezone_type": 3,
             "timezone": "Europe/Amsterdam",
         },
         "updated_by": "B23ABCC4-3A53-FB32-7B78-3960CC907F25",
         "updated_on": {
-            "date": "2019-09-23 08:16:37.000000",
+            "date": "2019-09-23 12:16:37.000000",
             "timezone_type": 3,
             "timezone": "Europe/Amsterdam",
         },
         "_embedded": {
             "query_remarks": [
                 {
                     "id": "BAF66EE9-DB44-48B5-9247-DBED30EFC553",
```

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_randomization_endpoints.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_randomization_endpoints.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_record_endpoints.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_record_endpoints.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         "created_on": {
             "date": "2019-10-28 15:24:02.000000",
             "timezone_type": 3,
             "timezone": "Europe/Amsterdam",
         },
         "updated_by": "B23ABCC4-3A53-FB32-7B78-3960CC907F25",
         "updated_on": {
-            "date": "2020-07-03 10:13:44.000000",
+            "date": "2020-07-03 14:13:44.000000",
             "timezone_type": 3,
             "timezone": "Europe/Amsterdam",
         },
         "randomized_id": None,
         "randomized_on": None,
         "randomization_group": None,
         "randomization_group_name": None,
```

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_record_progress_endpoints.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_record_progress_endpoints.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_report_data_entry_endpoints.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_report_data_entry_endpoints.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     data_options = data_options
     test_field = {
         "record_id": "000004",
         "field_variable_name": "med_units",
         "field_id": "AFD46D4F-5C17-4B9B-BE19-8A5A702601C1",
         "report_instance_id": "2711B1EF-6118-4EBD-9858-47E4830C4EC5",
         "value": "1",
-        "updated_on": "2020-08-14 10:55:46",
+        "updated_on": "2020-08-14 14:55:46",
         "_embedded": {
             "record": {
                 "id": "000004",
                 "record_id": "000004",
                 "record_status": None,
                 "ccr_patient_id": "",
                 "last_opened_step": "FFF23B2C-AEE6-4304-9CC4-9C7C431D5387",
@@ -43,15 +43,15 @@
                 "created_on": {
                     "date": "2019-10-28 10:54:07.000000",
                     "timezone_type": 3,
                     "timezone": "Europe/Amsterdam",
                 },
                 "updated_by": "B23ABCC4-3A53-FB32-7B78-3960CC907F25",
                 "updated_on": {
-                    "date": "2020-08-14 11:20:27.000000",
+                    "date": "2020-08-14 15:20:27.000000",
                     "timezone_type": 3,
                     "timezone": "Europe/Amsterdam",
                 },
                 "randomized_id": None,
                 "randomized_on": None,
                 "randomization_group": None,
                 "randomization_group_name": None,
@@ -121,15 +121,15 @@
                 "name": "55437058",
                 "status": "open",
                 "parent_id": "",
                 "parent_type": "",
                 "record_id": "000004",
                 "report_name": "Medication",
                 "archived": False,
-                "created_on": "2020-08-14 07:13:54",
+                "created_on": "2020-08-14 11:13:54",
                 "created_by": "B23ABCC4-3A53-FB32-7B78-3960CC907F25",
                 "_embedded": {
                     "report": {
                         "id": "89FF2394-0D41-4D4C-89FE-AA9AB287B31E",
                         "report_id": "89FF2394-0D41-4D4C-89FE-AA9AB287B31E",
                         "name": "Medication",
                         "description": "Alle mogelijke repeated measures zijn hier te bewerken",
```

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_report_endpoints.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_report_endpoints.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_report_instance_endpoints.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_report_instance_endpoints.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         "id": "382AE5BD-E728-4575-B467-142EA83813DE",
         "name": "20412282",
         "status": "open",
         "parent_id": "",
         "parent_type": "",
         "record_id": "110002",
         "report_name": "Unscheduled visit",
-        "created_on": "2019-10-14 12:58:12",
+        "created_on": "2019-10-14 16:58:12",
         "created_by": "B23ABCC4-3A53-FB32-7B78-3960CC907F25",
         "archived": False,
         "_embedded": {
             "report": {
                 "id": "C4ADC387-9BFD-4171-A861-6B973699A6ED",
                 "report_id": "C4ADC387-9BFD-4171-A861-6B973699A6ED",
                 "name": "Unscheduled visit",
```

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_report_step_endpoints.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_report_step_endpoints.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_role_endpoints.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_role_endpoints.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_step_endpoints.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_step_endpoints.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_study_data_entry_endpoints.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_study_data_entry_endpoints.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 class TestStudyDataEntry:
     model_keys = study_data_point_extended_model.keys()
     test_field = {
         "record_id": "000004",
         "field_variable_name": "ic_versions",
         "field_id": "28D1A17B-51C3-4BDC-A604-7B2F6D5D5924",
         "value": "1",
-        "updated_on": "2019-11-04 14:47:38",
+        "updated_on": "2019-11-04 16:47:38",
         "_embedded": {
             "record": {
                 "id": "000004",
                 "record_id": "000004",
                 "record_status": None,
                 "ccr_patient_id": "",
                 "last_opened_step": "FFF23B2C-AEE6-4304-9CC4-9C7C431D5387",
@@ -40,15 +40,15 @@
                 "created_on": {
                     "date": "2019-10-28 10:54:07.000000",
                     "timezone_type": 3,
                     "timezone": "Europe/Amsterdam",
                 },
                 "updated_by": "B23ABCC4-3A53-FB32-7B78-3960CC907F25",
                 "updated_on": {
-                    "date": "2020-08-14 11:20:27.000000",
+                    "date": "2020-08-14 15:20:27.000000",
                     "timezone_type": 3,
                     "timezone": "Europe/Amsterdam",
                 },
                 "randomized_id": None,
                 "randomized_on": None,
                 "randomization_group": None,
                 "randomization_group_name": None,
```

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_study_endpoints.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_study_endpoints.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_study_statistics_endpoints.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_study_statistics_endpoints.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_survey_data_entry_endpoints.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_survey_data_entry_endpoints.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_survey_endpoints.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_survey_endpoints.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     test_survey = {
         "id": "D70C1273-B5D8-45CD-BFE8-A0BA75C44B7E",
         "survey_id": "D70C1273-B5D8-45CD-BFE8-A0BA75C44B7E",
         "name": "QOL Survey",
         "description": "",
         "intro_text": "##### This is the survey intro text. Here you can add some information for the participant that they will see before they start filling in the survey.\n```\n\n\n```\n##### Check the help text in the survey form editor to see how you can format this text or add images and links.\n```\n\n\n```\n### For example, you can use hashtags to make the text bigger or add headings.",
         "outro_text": "",
-        "survey_steps": [],
+        "survey_forms": [],
         "_links": {
             "self": {
                 "href": "https://data.castoredc.com/api/study/D234215B-D956-482D-BF17-71F2BB12A2FD/survey/D70C1273-B5D8-45CD-BFE8-A0BA75C44B7E"
             }
         },
     }
 
@@ -98,15 +98,15 @@
                         }
                     },
                 }
             ]
         },
         "_links": {
             "self": {
-                "href": "https://data.castoredc.com/api/study/D234215B-D956-482D-BF17-71F2BB12A2FD/surveypackage/71C01598-4682-4A4C-90E6-69C0BD38EA47"
+                "href": "https://data.castoredc.com/api/study/D234215B-D956-482D-BF17-71F2BB12A2FD/survey-package/71C01598-4682-4A4C-90E6-69C0BD38EA47"
             }
         },
     }
 
     test_survey_package_instance = {
         "id": "115DF660-A00A-4927-9E5F-A07D030D4A09",
         "survey_package_instance_id": "115DF660-A00A-4927-9E5F-A07D030D4A09",
@@ -161,15 +161,15 @@
                 "created_on": {
                     "date": "2019-10-07 16:16:02.000000",
                     "timezone_type": 3,
                     "timezone": "Europe/Amsterdam",
                 },
                 "updated_by": "B23ABCC4-3A53-FB32-7B78-3960CC907F25",
                 "updated_on": {
-                    "date": "2021-10-20 12:25:16.000000",
+                    "date": "2021-10-20 16:25:16.000000",
                     "timezone_type": 3,
                     "timezone": "Europe/Amsterdam",
                 },
                 "randomized_id": None,
                 "randomization_group": None,
                 "randomization_group_name": None,
                 "randomized_on": None,
@@ -253,15 +253,15 @@
                                 }
                             },
                         }
                     ]
                 },
                 "_links": {
                     "self": {
-                        "href": "https://data.castoredc.com/api/study/D234215B-D956-482D-BF17-71F2BB12A2FD/surveypackage/71C01598-4682-4A4C-90E6-69C0BD38EA47"
+                        "href": "https://data.castoredc.com/api/study/D234215B-D956-482D-BF17-71F2BB12A2FD/survey-package/71C01598-4682-4A4C-90E6-69C0BD38EA47"
                     }
                 },
             },
             "survey_instances": [
                 {
                     "id": "6530D4AB-4705-4864-92AE-B0EC6200E8E5",
                     "progress": 100,
```

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_survey_step_endpoints.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_survey_step_endpoints.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
             "survey": {
                 "id": "D70C1273-B5D8-45CD-BFE8-A0BA75C44B7E",
                 "survey_id": "D70C1273-B5D8-45CD-BFE8-A0BA75C44B7E",
                 "name": "QOL Survey",
                 "description": "",
                 "intro_text": "##### This is the survey intro text. Here you can add some information for the participant that they will see before they start filling in the survey.\n```\n\n\n```\n##### Check the help text in the survey form editor to see how you can format this text or add images and links.\n```\n\n\n```\n### For example, you can use hashtags to make the text bigger or add headings.",
                 "outro_text": "",
-                "survey_steps": [],
+                "survey_forms": [],
                 "_links": {
                     "self": {
                         "href": "https://data.castoredc.com/api/study/D234215B-D956-482D-BF17-71F2BB12A2FD/survey/D70C1273-B5D8-45CD-BFE8-A0BA75C44B7E"
                     }
                 },
             }
         },
```

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_user_endpoints.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_user_endpoints.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_api_endpoints/test_verification_endpoints.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_api_endpoints/test_verification_endpoints.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,15 +39,15 @@
             "id": 2,
             "record_id": "000024",
             "entity_type": "field",
             "entity_id": "BFB50DCE-0563-4963-BAB8-899EE2475961",
             "parent_id": "",
             "verified_by": "B23ABCC4-3A53-FB32-7B78-3960CC907F25",
             "verified_on": {
-                "date": "2021-10-13 13:19:39.000000",
+                "date": "2021-10-13 17:19:39.000000",
                 "timezone_type": 3,
                 "timezone": "Europe/Amsterdam",
             },
             "status": "active",
             "dropped_by": None,
             "dropped_on": None,
             "changed_field": None,
```

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_castor_objects/fixtures_castor_objects.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_castor_objects/fixtures_castor_objects.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_castor_objects/helpers_castor_objects.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_castor_objects/helpers_castor_objects.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_castor_objects/test_castor_data_point.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_castor_objects/test_castor_data_point.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_castor_objects/test_castor_field.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_castor_objects/test_castor_field.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_castor_objects/test_castor_form.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_castor_objects/test_castor_form.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_castor_objects/test_castor_form_instance.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_castor_objects/test_castor_form_instance.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_castor_objects/test_castor_record.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_castor_objects/test_castor_record.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_castor_objects/test_castor_step.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_castor_objects/test_castor_step.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_castor_objects/test_castor_study.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_castor_objects/test_castor_study.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_client.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_import/test_async_import/test_import_merge_async.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_import/test_async_import/test_import_merge_async.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_import/test_async_import/test_import_report_async.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_import/test_async_import/test_import_report_async.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_import/test_async_import/test_import_study_async.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_import/test_async_import/test_import_study_async.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_import/test_async_import/test_import_study_format_async.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_import/test_async_import/test_import_study_format_async.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_import/test_async_import/test_import_survey_async.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_import/test_async_import/test_import_survey_async.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_import/test_async_import/test_import_translation_async.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_import/test_async_import/test_import_translation_async.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_import/test_async_import/test_import_validation_errors_async.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_import/test_async_import/test_import_validation_errors_async.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_import/test_prepare_import/test_column_translation.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_import/test_prepare_import/test_column_translation.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_import/test_prepare_import/test_create_upload.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_import/test_prepare_import/test_create_upload.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_import/test_prepare_import/test_create_upload_format.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_import/test_prepare_import/test_create_upload_format.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_import/test_prepare_import/test_format_translation.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_import/test_prepare_import/test_format_translation.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_import/test_prepare_import/test_label_translation.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_import/test_prepare_import/test_label_translation.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_import/test_prepare_import/test_value_translation.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_import/test_prepare_import/test_value_translation.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_import/test_sync_import/test_import_merge_sync.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_import/test_sync_import/test_import_merge_sync.py`

 * *Files 21% similar despite different names*

```diff
@@ -29,14 +29,27 @@
             label_data=True,
             target="Study",
             merge_path="tests/test_import/translate_files_for_import_tests/study_label_merge_file.xlsx",
         )
 
         assert imported_data == self.study_missing
 
+    def test_import_study_label_merge_empty(self, import_study):
+        """Tests if uploading label data with empty merge columns is successful (so no one has anything)."""
+        imported_data = import_data(
+            data_source_path="tests/test_import/data_files_for_import_tests/data_file_study_labels_merge_empty.xlsx",
+            column_link_path="tests/test_import/link_files_for_import_tests/study_merge_link_file.xlsx",
+            study=import_study,
+            label_data=True,
+            target="Study",
+            merge_path="tests/test_import/translate_files_for_import_tests/study_label_merge_file.xlsx",
+        )
+
+        assert imported_data == self.study_empty
+
     def test_import_study_label_merge_error(self, import_study):
         """Tests if uploading label data with errors is successful"""
         with pytest.raises(CastorException) as e:
             import_data(
                 data_source_path="tests/test_import/data_files_for_import_tests/data_file_study_labels_errors_merge.xlsx",
                 column_link_path="tests/test_import/link_files_for_import_tests/study_merge_link_file.xlsx",
                 study=import_study,
@@ -207,10 +220,93 @@
                 },
                 "failed": {},
                 "error": {},
             }
         ],
     }
 
+    study_empty = {
+        "110001": [
+            {
+                "success": {
+                    "base_bl_date": "16-03-2021",
+                    "base_hb": "8.3",
+                    "fac_V_leiden": "55;16-03-2021",
+                    "onset_stroke": "16-03-2021;07:30",
+                    "onset_trombectomy": "09:25",
+                    "pat_birth_year": "1999",
+                    "pat_sex": "0",
+                    "pat_race": "1",
+                },
+                "failed": {},
+                "error": {},
+            }
+        ],
+        "110002": [
+            {
+                "success": {
+                    "base_bl_date": "17-03-2021",
+                    "base_hb": "7.2",
+                    "fac_V_leiden": "33;17-03-2021",
+                    "onset_stroke": "17-03-2021;15:30",
+                    "onset_trombectomy": "06:33",
+                    "pat_birth_year": "1956",
+                    "pat_sex": "0",
+                    "pat_race": "2",
+                },
+                "failed": {},
+                "error": {},
+            }
+        ],
+        "110003": [
+            {
+                "success": {
+                    "base_bl_date": "16-03-2022",
+                    "base_hb": "9.1",
+                    "fac_V_leiden": "-45;18-03-2022",
+                    "onset_stroke": "18-03-2022;02:00",
+                    "onset_trombectomy": "12:24",
+                    "pat_birth_year": "1945",
+                    "pat_sex": "1",
+                    "pat_race": "3",
+                },
+                "failed": {},
+                "error": {},
+            }
+        ],
+        "110004": [
+            {
+                "success": {
+                    "base_bl_date": "17-03-2022",
+                    "base_hb": "3.2",
+                    "fac_V_leiden": "28;19-03-2022",
+                    "onset_stroke": "17-03-2022;21:43",
+                    "onset_trombectomy": "23:23",
+                    "pat_birth_year": "1933",
+                    "pat_sex": "1",
+                    "pat_race": "4",
+                },
+                "failed": {},
+                "error": {},
+            }
+        ],
+        "110005": [
+            {
+                "success": {
+                    "base_bl_date": "16-03-2023",
+                    "base_hb": "10.3",
+                    "fac_V_leiden": "5;20-03-2023",
+                    "onset_stroke": "16-03-2023;07:22",
+                    "onset_trombectomy": "08:14",
+                    "pat_birth_year": "1921",
+                    "pat_sex": "0",
+                    "pat_race": "5",
+                },
+                "failed": {},
+                "error": {},
+            }
+        ],
+    }
+
     study_error = (
         "Non-viable data found in dataset to be imported. See output folder for details"
     )
```

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_import/test_sync_import/test_import_report_sync.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_import/test_sync_import/test_import_report_sync.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_import/test_sync_import/test_import_study_format_sync.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_import/test_sync_import/test_import_study_format_sync.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_import/test_sync_import/test_import_study_sync.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_import/test_sync_import/test_import_study_sync.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_import/test_sync_import/test_import_survey_sync.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_import/test_sync_import/test_import_survey_sync.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_import/test_sync_import/test_import_translation_sync.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_import/test_sync_import/test_import_translation_sync.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_import/test_sync_import/test_import_validation_errors_sync.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_import/test_sync_import/test_import_validation_errors_sync.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_integration/data_ids.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_integration/data_ids.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_integration/fixtures_integration.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_integration/fixtures_integration.py`

 * *Files 15% similar despite different names*

```diff
@@ -34,10 +34,16 @@
 @pytest.fixture(scope="function")
 def integration_study_mapped(integration_study):
     integration_study.map_data()
     return integration_study
 
 
 @pytest.fixture(scope="function")
+def integration_study_mapped_archived(integration_study):
+    integration_study.map_data(archived=True)
+    return integration_study
+
+
+@pytest.fixture(scope="function")
 def integration_study_format_mapped(integration_study_format):
     integration_study_format.map_data()
     return integration_study_format
```

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_integration/test_data_interpretation.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_integration/test_data_interpretation.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_integration/test_data_interpretation_formatting.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_integration/test_data_interpretation_formatting.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_integration/test_data_mapping.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_integration/test_data_mapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 class TestDataMap:
     """Tests the integration between CastorEDCClient and the CastorObjects that map the study data."""
 
-    def test_records_exist(self, integration_study_mapped):
+    def test_records_exist(self, integration_study_mapped_archived):
         record_ids = [
-            integration_study_mapped.records[record].record_id
-            for record in integration_study_mapped.records
+            integration_study_mapped_archived.records[record].record_id
+            for record in integration_study_mapped_archived.records
         ]
         # Record with leading zeroes
         assert "000001" in record_ids
         # Archived record
         assert "ARCHIVED-110003" in record_ids
         # Normal record
         assert "110009" in record_ids
```

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_integration/test_data_structure_mapping.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_integration/test_data_structure_mapping.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_integration/test_special_cases.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_integration/test_special_cases.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         And where an archived report is the parent of a survey."""
         study = CastorStudy(
             auth_data.client_id,
             auth_data.client_secret,
             auth_data.test_special_study_id,
             "data.castoredc.com",
         )
-        study.map_data()
+        study.map_data(archived=True)
         # Parent is a study phase
         assert (
             study.get_single_form_instance_on_id(
                 "110001", "61AD63FA-9CC9-4F4D-A58C-5FFF6D2A524F"
             ).parent
             == "Baseline"
         )
```

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_integration/test_structure_mapping.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_integration/test_structure_mapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,23 +40,23 @@
         assert "C4ADC387-9BFD-4171-A861-6B973699A6ED" in report_form_ids
         assert "770DB401-6100-4CF5-A95F-3402B55EAC48" in report_form_ids
         assert "8D4F696E-DA2E-4A0E-ACD8-2F1B71718D6E" in report_form_ids
 
     def test_study_form_links_model(self, integration_study):
         """Tests if the links are in the right format."""
         integration_study.map_structure()
-        integration_study.update_links()
+        integration_study.update_links(False)
         assert len(integration_study.form_links.keys()) == 2
         assert type(integration_study.form_links["Report"]) is dict
         assert type(integration_study.form_links["Survey"]) is dict
 
     def test_study_form_links_form(self, integration_study):
         """Tests if the links contain the right forms."""
         integration_study.map_structure()
-        integration_study.update_links()
+        integration_study.update_links(False)
         assert "89FF2394-0D41-4D4C-89FE-AA9AB287B31E" in list(
             integration_study.form_links["Report"].values()
         )
         assert "C4ADC387-9BFD-4171-A861-6B973699A6ED" in list(
             integration_study.form_links["Report"].values()
         )
         assert "770DB401-6100-4CF5-A95F-3402B55EAC48" in list(
@@ -69,15 +69,15 @@
             "D70C1273-B5D8-45CD-BFE8-A0BA75C44B7E"
             in integration_study.form_links["Survey"]["QOL Survey"]
         )
 
     def test_study_form_links_form_instances(self, integration_study):
         """Tests if the links contain the right form instances."""
         integration_study.map_structure()
-        integration_study.update_links()
+        integration_study.update_links(False)
         # Test Reports
         assert (
             "89FF2394-0D41-4D4C-89FE-AA9AB287B31E"
             in integration_study.form_links["Report"][
                 "B68E831D-1347-4237-9F38-F79E86A58D64"
             ]
         )
```

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_output/test_csv_output.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_output/test_csv_output.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_output/test_csv_output_archived.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_output/test_csv_output_archived.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api/tests/test_output/test_csv_output_format.py` & `castoredc_api-0.1.8/castoredc_api/tests/test_output/test_csv_output_format.py`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/castoredc_api.egg-info/PKG-INFO` & `castoredc_api-0.1.8/castoredc_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: castoredc-api
-Version: 0.1.7.post1
+Version: 0.1.8
 Summary: Python wrapper for the Castor EDC API
 Home-page: https://github.com/reiniervlinschoten/castoredc_api
 Author: Reinier van Linschoten
 Author-email: mail@reiniervl.com
 Maintainer: Reinier van Linschoten
 Maintainer-email: mail@reiniervl.com
 License: MIT
@@ -19,15 +19,15 @@
 [![black](https://github.com/reiniervlinschoten/castoredc_api/actions/workflows/black.yml/badge.svg)](https://github.com/reiniervlinschoten/castoredc_api/actions/workflows/black.yml)
 
 [![pypi](https://img.shields.io/pypi/v/castoredc_api)](https://pypi.org/project/castoredc-api/)
 [![conda](https://img.shields.io/conda/v/reiniervl/castoredc_api)](https://anaconda.org/reiniervl/castoredc_api)
 [![conda-forge](https://img.shields.io/conda/v/conda-forge/castoredc_api)](https://anaconda.org/conda-forge/castoredc_api)
 
 ## Features
-#### Supports CastorEDC Release 2022.5
+#### Supports CastorEDC Release 2023.1
 
 This is a Python package for interacting with the API of Castor Electronic Data Capture (EDC). 
 The package contains functions to interact with all the endpoints defined on https://data.castoredc.com/api#/.
 Within the package are functions for easy export and import of your data through the API.
 
 ### Export
 Supported export formats are
```

### Comparing `castoredc_api-0.1.7.post1/castoredc_api.egg-info/SOURCES.txt` & `castoredc_api-0.1.8/castoredc_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `castoredc_api-0.1.7.post1/setup.py` & `castoredc_api-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="castoredc_api",
-    version="0.1.7.post1",
+    version="0.1.8",
     description="Python wrapper for the Castor EDC API",
     author="Reinier van Linschoten",
     author_email="mail@reiniervl.com",
     maintainer="Reinier van Linschoten",
     maintainer_email="mail@reiniervl.com",
     url="https://github.com/reiniervlinschoten/castoredc_api",
     packages=find_packages(include=("castoredc_api", "castoredc_api.*")),
```

