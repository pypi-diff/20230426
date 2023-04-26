# Comparing `tmp/carculator_utils-1.0.5.tar.gz` & `tmp/carculator_utils-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carculator_utils-1.0.5.tar", last modified: Sun Apr 23 11:18:06 2023, max compression
+gzip compressed data, was "carculator_utils-1.0.6.tar", last modified: Wed Apr 26 07:25:09 2023, max compression
```

## Comparing `carculator_utils-1.0.5.tar` & `carculator_utils-1.0.6.tar`

### file list

```diff
@@ -1,169 +1,169 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:18:06.868886 carculator_utils-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-04-23 11:18:06.864886 carculator_utils-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:18:06.792886 carculator_utils-1.0.5/carculator_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    13413 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/background_systems.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:18:06.792886 carculator_utils-1.0.5/carculator_utils/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:18:06.840886 carculator_utils-1.0.5/carculator_utils/data/IAM/
--rw-r--r--   0 runner    (1001) docker     (123)    82764 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/A_matrix.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614740 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-NPi_2030.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614741 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-NPi_2040.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614739 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-NPi_2050.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614739 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg1150_2030.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614741 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg1150_2040.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614741 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg1150_2050.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614739 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg500_2030.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614741 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg500_2040.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614741 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg500_2050.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-NPi_2005.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-NPi_2010.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-NPi_2020.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg1150_2005.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg1150_2010.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg1150_2020.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg500_2005.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg500_2010.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg500_2020.csv
--rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_static_ 3.8 cutoff.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129388 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-NPi_2030.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129388 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-NPi_2040.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129388 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-NPi_2050.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129388 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg1150_2030.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129389 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg1150_2040.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129389 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg1150_2050.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129389 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg500_2030.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129389 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg500_2040.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129388 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg500_2050.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-NPi_2005.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-NPi_2010.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-NPi_2020.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg1150_2005.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg1150_2010.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg1150_2020.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg500_2005.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg500_2010.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg500_2020.csv
--rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint_static_ 3.8 cutoff.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744503 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-NPi_2030.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744505 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-NPi_2040.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744507 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-NPi_2050.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744503 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg1150_2030.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744508 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg1150_2040.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744510 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg1150_2050.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744503 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg500_2030.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744510 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg500_2040.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744512 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg500_2050.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-NPi_2005.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-NPi_2010.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-NPi_2020.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg1150_2005.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg1150_2010.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg1150_2020.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg500_2005.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg500_2010.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg500_2020.csv
--rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint_static_ 3.8 cutoff.csv
--rw-r--r--   0 runner    (1001) docker     (123)    94289 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/IAM/dict_inputs_A_matrix.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:18:06.844886 carculator_utils-1.0.5/carculator_utils/data/driving cycle/
--rw-r--r--   0 runner    (1001) docker     (123)   623589 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/driving cycle/bus.csv
--rw-r--r--   0 runner    (1001) docker     (123)   102616 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/driving cycle/car.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/driving cycle/dc_specs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)   392181 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/driving cycle/truck.csv
--rw-r--r--   0 runner    (1001) docker     (123)    63435 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/driving cycle/two-wheeler.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:18:06.844886 carculator_utils-1.0.5/carculator_utils/data/efficiency/
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/efficiency/bus.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    12959 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/efficiency/car.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/efficiency/truck.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:18:06.844886 carculator_utils-1.0.5/carculator_utils/data/electricity/
--rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/electricity/cumulative_electricity_losses.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/electricity/elec_tech_map.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    98629 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/electricity/electricity_mixes.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:18:06.844886 carculator_utils-1.0.5/carculator_utils/data/emission_factors/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:18:06.848886 carculator_utils-1.0.5/carculator_utils/data/emission_factors/bus/
--rw-r--r--   0 runner    (1001) docker     (123)    81444 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/bus/EF_HBEFA42_exhaust.csv
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/bus/NMHC_species.csv
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/bus/degradation_EF.csv
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/bus/engine_wear.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/bus/propulsion_noise_coefficients.csv
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/bus/rolling_noise_coefficients.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:18:06.848886 carculator_utils-1.0.5/carculator_utils/data/emission_factors/car/
--rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/car/EF_HBEFA42_exhaust.csv
--rw-r--r--   0 runner    (1001) docker     (123)    28435 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/car/EF_HBEFA42_non_exhaust.csv
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/car/NMHC_species.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/car/degradation_EF.csv
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/car/engine_wear.csv
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/car/propulsion_noise_coefficients.csv
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/car/rolling_noise_coefficients.csv
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/euro_classes.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/exhaust_and_noise_flows.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/exhaust_flows.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/noise_flows.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:18:06.848886 carculator_utils-1.0.5/carculator_utils/data/emission_factors/truck/
--rw-r--r--   0 runner    (1001) docker     (123)    28747 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/truck/EF_HBEFA42_exhaust.csv
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/truck/NMHC_species.csv
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/truck/degradation_EF.csv
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/truck/engine_wear.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/truck/propulsion_noise_coefficients.csv
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/truck/rolling_noise_coefficients.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:18:06.852886 carculator_utils-1.0.5/carculator_utils/data/emission_factors/two-wheeler/
--rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/two-wheeler/EF_HBEFA42_exhaust.csv
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/two-wheeler/NMHC_species.csv
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/two-wheeler/engine_wear.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/emission_factors/two-wheeler/propulsion_noise_coefficients.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:18:06.860886 carculator_utils-1.0.5/carculator_utils/data/export/
--rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/export/ei37_to_ei35.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/export/ei37_to_ei36.csv
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/export/ei38_to_ei37.csv
--rw-r--r--   0 runner    (1001) docker     (123)   154654 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/export/references.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/export/rename_parameters.yml
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/export/rename_powertrains.yml
--rw-r--r--   0 runner    (1001) docker     (123)    57797 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/export/simapro-biosphere.json
--rw-r--r--   0 runner    (1001) docker     (123)  6503006 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/export/simapro-technosphere-3.5.csv
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/export/simapro_blacklist.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/export/simapro_fields.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:18:06.864886 carculator_utils-1.0.5/carculator_utils/data/fuel/
--rw-r--r--   0 runner    (1001) docker     (123)    14496 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/fuel/S_concentration_fuel.csv
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/fuel/default_fuels.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/fuel/fuel_specs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/fuel/share_bio_cng.csv
--rw-r--r--   0 runner    (1001) docker     (123)    14782 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/fuel/share_bio_diesel.csv
--rw-r--r--   0 runner    (1001) docker     (123)    14606 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/fuel/share_bio_gasoline.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:18:06.864886 carculator_utils-1.0.5/carculator_utils/data/gradient/
--rw-r--r--   0 runner    (1001) docker     (123)   751813 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/gradient/bus.csv
--rw-r--r--   0 runner    (1001) docker     (123)    71480 2023-04-23 11:17:52.000000 carculator_utils-1.0.5/carculator_utils/data/gradient/car.csv
--rw-r--r--   0 runner    (1001) docker     (123)   764385 2023-04-23 11:17:53.000000 carculator_utils-1.0.5/carculator_utils/data/gradient/truck.csv
--rw-r--r--   0 runner    (1001) docker     (123)    44045 2023-04-23 11:17:53.000000 carculator_utils-1.0.5/carculator_utils/data/gradient/two-wheeler.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:18:06.864886 carculator_utils-1.0.5/carculator_utils/data/lcia/
--rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-04-23 11:17:53.000000 carculator_utils-1.0.5/carculator_utils/data/lcia/dict_impact_categories.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-23 11:17:53.000000 carculator_utils-1.0.5/carculator_utils/data/lcia/impact_source_categories.yml
--rw-r--r--   0 runner    (1001) docker     (123)     8132 2023-04-23 11:17:53.000000 carculator_utils-1.0.5/carculator_utils/data/monthly_avg_temp.csv
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-23 11:17:53.000000 carculator_utils-1.0.5/carculator_utils/data/purchase_cost_params.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-04-23 11:17:53.000000 carculator_utils-1.0.5/carculator_utils/driving_cycles.py
--rw-r--r--   0 runner    (1001) docker     (123)    20712 2023-04-23 11:17:53.000000 carculator_utils-1.0.5/carculator_utils/energy_consumption.py
--rw-r--r--   0 runner    (1001) docker     (123)    42445 2023-04-23 11:17:53.000000 carculator_utils-1.0.5/carculator_utils/export.py
--rw-r--r--   0 runner    (1001) docker     (123)    17078 2023-04-23 11:17:53.000000 carculator_utils-1.0.5/carculator_utils/hot_emissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    68287 2023-04-23 11:17:53.000000 carculator_utils-1.0.5/carculator_utils/inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)    51632 2023-04-23 11:17:53.000000 carculator_utils-1.0.5/carculator_utils/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9258 2023-04-23 11:17:53.000000 carculator_utils-1.0.5/carculator_utils/noise_emissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-04-23 11:17:53.000000 carculator_utils-1.0.5/carculator_utils/particulates_emissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-23 11:17:53.000000 carculator_utils-1.0.5/carculator_utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-04-23 11:17:53.000000 carculator_utils-1.0.5/carculator_utils/vehicle_input_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:18:06.792886 carculator_utils-1.0.5/carculator_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-04-23 11:18:06.000000 carculator_utils-1.0.5/carculator_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8924 2023-04-23 11:18:06.000000 carculator_utils-1.0.5/carculator_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 11:18:06.000000 carculator_utils-1.0.5/carculator_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-23 11:18:06.000000 carculator_utils-1.0.5/carculator_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-23 11:18:06.000000 carculator_utils-1.0.5/carculator_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-23 11:17:53.000000 carculator_utils-1.0.5/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-23 11:17:53.000000 carculator_utils-1.0.5/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-23 11:17:53.000000 carculator_utils-1.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 11:18:06.868886 carculator_utils-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-23 11:17:53.000000 carculator_utils-1.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 11:18:06.864886 carculator_utils-1.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-23 11:17:53.000000 carculator_utils-1.0.5/tests/test_vehicle_input_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:25:09.223724 carculator_utils-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-04-26 07:25:09.223724 carculator_utils-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:25:09.163723 carculator_utils-1.0.6/carculator_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13413 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/background_systems.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:25:09.163723 carculator_utils-1.0.6/carculator_utils/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:25:09.203723 carculator_utils-1.0.6/carculator_utils/data/IAM/
+-rw-r--r--   0 runner    (1001) docker     (123)    82764 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/A_matrix.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614740 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-NPi_2030.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614741 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-NPi_2040.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614739 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-NPi_2050.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614739 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg1150_2030.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614741 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg1150_2040.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614741 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg1150_2050.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614739 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg500_2030.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614741 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg500_2040.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614741 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg500_2050.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-NPi_2005.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-NPi_2010.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-NPi_2020.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg1150_2005.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg1150_2010.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg1150_2020.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg500_2005.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg500_2010.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg500_2020.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   614757 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_static_ 3.8 cutoff.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129388 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-NPi_2030.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129388 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-NPi_2040.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129388 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-NPi_2050.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129388 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg1150_2030.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129389 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg1150_2040.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129389 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg1150_2050.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129389 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg500_2030.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129389 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg500_2040.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129388 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg500_2050.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-NPi_2005.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-NPi_2010.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-NPi_2020.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg1150_2005.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg1150_2010.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg1150_2020.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg500_2005.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg500_2010.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg500_2020.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   129385 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint_static_ 3.8 cutoff.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744503 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-NPi_2030.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744505 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-NPi_2040.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744507 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-NPi_2050.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744503 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg1150_2030.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744508 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg1150_2040.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744510 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg1150_2050.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744503 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg500_2030.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744510 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg500_2040.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744512 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg500_2050.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-NPi_2005.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-NPi_2010.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-NPi_2020.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg1150_2005.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg1150_2010.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg1150_2020.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg500_2005.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg500_2010.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg500_2020.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   744522 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint_static_ 3.8 cutoff.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    94289 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/IAM/dict_inputs_A_matrix.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:25:09.207723 carculator_utils-1.0.6/carculator_utils/data/driving cycle/
+-rw-r--r--   0 runner    (1001) docker     (123)   623589 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/driving cycle/bus.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   102616 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/driving cycle/car.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/driving cycle/dc_specs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   392181 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/driving cycle/truck.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    63435 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/driving cycle/two-wheeler.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:25:09.207723 carculator_utils-1.0.6/carculator_utils/data/efficiency/
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/efficiency/bus.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    12959 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/efficiency/car.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/efficiency/truck.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:25:09.207723 carculator_utils-1.0.6/carculator_utils/data/electricity/
+-rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/electricity/cumulative_electricity_losses.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/electricity/elec_tech_map.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    98629 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/electricity/electricity_mixes.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:25:09.207723 carculator_utils-1.0.6/carculator_utils/data/emission_factors/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:25:09.207723 carculator_utils-1.0.6/carculator_utils/data/emission_factors/bus/
+-rw-r--r--   0 runner    (1001) docker     (123)    81444 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/bus/EF_HBEFA42_exhaust.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/bus/NMHC_species.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/bus/degradation_EF.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/bus/engine_wear.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/bus/propulsion_noise_coefficients.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/bus/rolling_noise_coefficients.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:25:09.207723 carculator_utils-1.0.6/carculator_utils/data/emission_factors/car/
+-rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/car/EF_HBEFA42_exhaust.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    28435 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/car/EF_HBEFA42_non_exhaust.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/car/NMHC_species.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/car/degradation_EF.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/car/engine_wear.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/car/propulsion_noise_coefficients.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/car/rolling_noise_coefficients.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/euro_classes.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/exhaust_and_noise_flows.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/exhaust_flows.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/noise_flows.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:25:09.211723 carculator_utils-1.0.6/carculator_utils/data/emission_factors/truck/
+-rw-r--r--   0 runner    (1001) docker     (123)    28747 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/truck/EF_HBEFA42_exhaust.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/truck/NMHC_species.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/truck/degradation_EF.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/truck/engine_wear.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/truck/propulsion_noise_coefficients.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/truck/rolling_noise_coefficients.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:25:09.211723 carculator_utils-1.0.6/carculator_utils/data/emission_factors/two-wheeler/
+-rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/two-wheeler/EF_HBEFA42_exhaust.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/two-wheeler/NMHC_species.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/two-wheeler/engine_wear.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/emission_factors/two-wheeler/propulsion_noise_coefficients.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:25:09.219724 carculator_utils-1.0.6/carculator_utils/data/export/
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/export/ei37_to_ei35.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/export/ei37_to_ei36.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/export/ei38_to_ei37.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   154654 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/export/references.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/export/rename_parameters.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/export/rename_powertrains.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    57797 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/export/simapro-biosphere.json
+-rw-r--r--   0 runner    (1001) docker     (123)  6503006 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/export/simapro-technosphere-3.5.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/export/simapro_blacklist.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/export/simapro_fields.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:25:09.219724 carculator_utils-1.0.6/carculator_utils/data/fuel/
+-rw-r--r--   0 runner    (1001) docker     (123)    14496 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/fuel/S_concentration_fuel.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/fuel/default_fuels.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/fuel/fuel_specs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/fuel/share_bio_cng.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    14782 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/fuel/share_bio_diesel.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    14606 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/fuel/share_bio_gasoline.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:25:09.219724 carculator_utils-1.0.6/carculator_utils/data/gradient/
+-rw-r--r--   0 runner    (1001) docker     (123)   751813 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/gradient/bus.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    71480 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/gradient/car.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   764385 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/gradient/truck.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    44045 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/gradient/two-wheeler.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:25:09.219724 carculator_utils-1.0.6/carculator_utils/data/lcia/
+-rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/lcia/dict_impact_categories.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/lcia/impact_source_categories.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     8132 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/monthly_avg_temp.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/data/purchase_cost_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/driving_cycles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23683 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/energy_consumption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42445 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17078 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/hot_emissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68287 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51873 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9258 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/noise_emissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/particulates_emissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/carculator_utils/vehicle_input_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:25:09.163723 carculator_utils-1.0.6/carculator_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-04-26 07:25:09.000000 carculator_utils-1.0.6/carculator_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8924 2023-04-26 07:25:09.000000 carculator_utils-1.0.6/carculator_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 07:25:09.000000 carculator_utils-1.0.6/carculator_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-26 07:25:09.000000 carculator_utils-1.0.6/carculator_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-26 07:25:09.000000 carculator_utils-1.0.6/carculator_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 07:25:09.223724 carculator_utils-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:25:09.219724 carculator_utils-1.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-26 07:25:01.000000 carculator_utils-1.0.6/tests/test_vehicle_input_parameters.py
```

### Comparing `carculator_utils-1.0.5/CODE_OF_CONDUCT.md` & `carculator_utils-1.0.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/CONTRIBUTING.md` & `carculator_utils-1.0.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/LICENSE` & `carculator_utils-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/PKG-INFO` & `carculator_utils-1.0.6/carculator_utils.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: carculator_utils
-Version: 1.0.5
+Name: carculator-utils
+Version: 1.0.6
 Summary: Provides convenience functions for carculator_utils
 Home-page: https://github.com/romainsacchi/carculator_utils
 Author: Romain Sacchi <romain.sacchi@psi.ch>
 License: BSD 3-Clause License
         
         Copyright (c) 2020, Paul Scherrer Institut
         
@@ -53,14 +53,20 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ``carculator_utils``
 
 
 Base classes and functions for the carculator package suite.
+Provides base classes to:
+
+* carculator
+* carculator_bus
+* carculator_truck
+* carculator_two-wheeler
 
 ## Support
 
 Do not hesitate to contact the development team at [carculator@psi.ch](mailto:carculator@psi.ch).
 
 ## Maintainers
 
@@ -68,8 +74,8 @@
 
 ## Contributing
 
 See [contributing](https://github.com/romainsacchi/carculator_utils/blob/master/CONTRIBUTING.md).
 
 ## License
 
-[BSD-3-Clause](https://github.com/romainsacchi/carculator_utils/blob/master/LICENSE). Copyright 2020 Paul Scherrer Institut.
+[BSD-3-Clause](https://github.com/romainsacchi/carculator_utils/blob/master/LICENSE). Copyright 2023 Paul Scherrer Institut.
```

### Comparing `carculator_utils-1.0.5/README.md` & `carculator_utils-1.0.6/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # ``carculator_utils``
 
 
 Base classes and functions for the carculator package suite.
+Provides base classes to:
+
+* carculator
+* carculator_bus
+* carculator_truck
+* carculator_two-wheeler
 
 ## Support
 
 Do not hesitate to contact the development team at [carculator@psi.ch](mailto:carculator@psi.ch).
 
 ## Maintainers
 
@@ -13,8 +19,8 @@
 
 ## Contributing
 
 See [contributing](https://github.com/romainsacchi/carculator_utils/blob/master/CONTRIBUTING.md).
 
 ## License
 
-[BSD-3-Clause](https://github.com/romainsacchi/carculator_utils/blob/master/LICENSE). Copyright 2020 Paul Scherrer Institut.
+[BSD-3-Clause](https://github.com/romainsacchi/carculator_utils/blob/master/LICENSE). Copyright 2023 Paul Scherrer Institut.
```

### Comparing `carculator_utils-1.0.5/carculator_utils/__init__.py` & `carculator_utils-1.0.6/carculator_utils/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "NoiseEmissionsModel",
     "HotEmissionsModel",
     "Inventory",
     "BackgroundSystemModel",
     "ExportInventory",
     "VehicleInputParameters",
 )
-__version__ = (1, 0, 5)
+__version__ = (1, 0, 6)
 
 from pathlib import Path
 
 DATA_DIR = Path(__file__).resolve().parent / "data"
 
 from .background_systems import BackgroundSystemModel
 from .driving_cycles import get_standard_driving_cycle_and_gradient
```

### Comparing `carculator_utils-1.0.5/carculator_utils/array.py` & `carculator_utils-1.0.6/carculator_utils/array.py`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/background_systems.py` & `carculator_utils-1.0.6/carculator_utils/background_systems.py`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/A_matrix.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/A_matrix.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-NPi_2030.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-NPi_2030.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-NPi_2040.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-NPi_2040.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-NPi_2050.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-NPi_2050.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg1150_2030.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg1150_2030.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg1150_2040.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg1150_2040.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg1150_2050.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg1150_2050.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg500_2030.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg500_2030.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg500_2040.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg500_2040.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg500_2050.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint__remind_SSP2-PkBudg500_2050.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-NPi_2005.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-NPi_2005.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-NPi_2010.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-NPi_2010.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-NPi_2020.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-NPi_2020.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg1150_2005.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg1150_2005.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg1150_2010.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg1150_2010.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg1150_2020.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg1150_2020.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg500_2005.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg500_2005.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg500_2010.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg500_2010.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg500_2020.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_remind_SSP2-PkBudg500_2020.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_static_ 3.8 cutoff.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_ilcd_midpoint_static_ 3.8 cutoff.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-NPi_2030.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-NPi_2030.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-NPi_2040.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-NPi_2040.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-NPi_2050.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-NPi_2050.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg1150_2030.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg1150_2030.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg1150_2040.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg1150_2040.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg1150_2050.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg1150_2050.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg500_2030.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg500_2030.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg500_2040.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg500_2040.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg500_2050.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint__remind_SSP2-PkBudg500_2050.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-NPi_2005.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-NPi_2005.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-NPi_2010.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-NPi_2010.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-NPi_2020.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-NPi_2020.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg1150_2005.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg1150_2005.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg1150_2010.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg1150_2010.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg1150_2020.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg1150_2020.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg500_2005.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg500_2005.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg500_2010.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg500_2010.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg500_2020.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint_remind_SSP2-PkBudg500_2020.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_endpoint_static_ 3.8 cutoff.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_endpoint_static_ 3.8 cutoff.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-NPi_2030.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-NPi_2030.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-NPi_2040.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-NPi_2040.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-NPi_2050.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-NPi_2050.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg1150_2030.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg1150_2030.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg1150_2040.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg1150_2040.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg1150_2050.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg1150_2050.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg500_2030.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg500_2030.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg500_2040.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg500_2040.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg500_2050.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint__remind_SSP2-PkBudg500_2050.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-NPi_2005.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-NPi_2005.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-NPi_2010.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-NPi_2010.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-NPi_2020.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-NPi_2020.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg1150_2005.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg1150_2005.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg1150_2010.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg1150_2010.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg1150_2020.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg1150_2020.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg500_2005.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg500_2005.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg500_2010.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg500_2010.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg500_2020.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint_remind_SSP2-PkBudg500_2020.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/B_matrix_recipe_midpoint_static_ 3.8 cutoff.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/B_matrix_recipe_midpoint_static_ 3.8 cutoff.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/IAM/dict_inputs_A_matrix.csv` & `carculator_utils-1.0.6/carculator_utils/data/IAM/dict_inputs_A_matrix.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/driving cycle/bus.csv` & `carculator_utils-1.0.6/carculator_utils/data/driving cycle/bus.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/driving cycle/car.csv` & `carculator_utils-1.0.6/carculator_utils/data/driving cycle/car.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/driving cycle/dc_specs.yaml` & `carculator_utils-1.0.6/carculator_utils/data/driving cycle/dc_specs.yaml`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/driving cycle/truck.csv` & `carculator_utils-1.0.6/carculator_utils/data/driving cycle/truck.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/driving cycle/two-wheeler.csv` & `carculator_utils-1.0.6/carculator_utils/data/driving cycle/two-wheeler.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/efficiency/bus.yaml` & `carculator_utils-1.0.6/carculator_utils/data/efficiency/truck.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# engine and transmission efficiency coefficients for the bus model
+# engine and transmission efficiency coefficients for the truck model
 # source: VECTO simulations
 # used to estimate efficiency in relation to the instant power
 # output/max power output
 # also, we do not have coefficient for compressed gas engine
 # so, we use the diesel engine efficiency for this case,
 # and apply a correction factor after
```

### Comparing `carculator_utils-1.0.5/carculator_utils/data/efficiency/car.yaml` & `carculator_utils-1.0.6/carculator_utils/data/efficiency/car.yaml`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/efficiency/truck.yaml` & `carculator_utils-1.0.6/carculator_utils/data/efficiency/bus.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-# engine and transmission efficiency coefficients for the truck model
+# engine and transmission efficiency coefficients for the bus model
 # source: VECTO simulations
 # used to estimate efficiency in relation to the instant power
 # output/max power output
 # also, we do not have coefficient for compressed gas engine
 # so, we use the diesel engine efficiency for this case,
 # and apply a correction factor after
 
 diesel:
   transmission:
     0: 0
     0.025: 0.6
     0.05: 0.75
     0.1: 0.85
     0.2: 0.88
-    0.3: 0.91
-    0.4: 0.91
-    0.5: 0.91
-    0.6: 0.91
-    0.7: 0.91
-    0.8: 0.91
-    0.9: 0.91
+    0.3: 0.9
+    0.4: 0.9
+    0.5: 0.9
+    0.6: 0.9
+    0.7: 0.9
+    0.8: 0.9
+    0.9: 0.9
 
   engine:
     0: 0
     0.025: 0.2
     0.05: 0.25
     0.1: 0.32
     0.2: 0.385
     0.3: 0.41
     0.4: 0.42
     0.5: 0.42
     0.6: 0.42
-    0.7: 0.42
-    0.8: 0.42
-    0.9: 0.4
+    0.7: 0.4
+    0.8: 0.35
+    0.9: 0.25
 
 compressed gas:
   transmission:
     0: 0
     0.025: 0.6
     0.05: 0.75
     0.1: 0.85
```

### Comparing `carculator_utils-1.0.5/carculator_utils/data/electricity/cumulative_electricity_losses.csv` & `carculator_utils-1.0.6/carculator_utils/data/electricity/cumulative_electricity_losses.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/electricity/elec_tech_map.yaml` & `carculator_utils-1.0.6/carculator_utils/data/electricity/elec_tech_map.yaml`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/electricity/electricity_mixes.csv` & `carculator_utils-1.0.6/carculator_utils/data/electricity/electricity_mixes.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/emission_factors/bus/EF_HBEFA42_exhaust.csv` & `carculator_utils-1.0.6/carculator_utils/data/emission_factors/bus/EF_HBEFA42_exhaust.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/emission_factors/bus/propulsion_noise_coefficients.csv` & `carculator_utils-1.0.6/carculator_utils/data/emission_factors/bus/propulsion_noise_coefficients.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/emission_factors/bus/rolling_noise_coefficients.csv` & `carculator_utils-1.0.6/carculator_utils/data/emission_factors/bus/rolling_noise_coefficients.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/emission_factors/car/EF_HBEFA42_exhaust.csv` & `carculator_utils-1.0.6/carculator_utils/data/emission_factors/car/EF_HBEFA42_exhaust.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/emission_factors/car/EF_HBEFA42_non_exhaust.csv` & `carculator_utils-1.0.6/carculator_utils/data/emission_factors/car/EF_HBEFA42_non_exhaust.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/emission_factors/car/NMHC_species.csv` & `carculator_utils-1.0.6/carculator_utils/data/emission_factors/car/NMHC_species.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/emission_factors/car/degradation_EF.csv` & `carculator_utils-1.0.6/carculator_utils/data/emission_factors/car/degradation_EF.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/emission_factors/car/engine_wear.csv` & `carculator_utils-1.0.6/carculator_utils/data/emission_factors/car/engine_wear.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/emission_factors/euro_classes.yaml` & `carculator_utils-1.0.6/carculator_utils/data/emission_factors/euro_classes.yaml`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/emission_factors/exhaust_and_noise_flows.yaml` & `carculator_utils-1.0.6/carculator_utils/data/emission_factors/exhaust_and_noise_flows.yaml`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/emission_factors/exhaust_flows.yaml` & `carculator_utils-1.0.6/carculator_utils/data/emission_factors/exhaust_flows.yaml`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/emission_factors/noise_flows.yaml` & `carculator_utils-1.0.6/carculator_utils/data/emission_factors/noise_flows.yaml`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/emission_factors/truck/EF_HBEFA42_exhaust.csv` & `carculator_utils-1.0.6/carculator_utils/data/emission_factors/truck/EF_HBEFA42_exhaust.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/emission_factors/truck/propulsion_noise_coefficients.csv` & `carculator_utils-1.0.6/carculator_utils/data/emission_factors/truck/propulsion_noise_coefficients.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/emission_factors/truck/rolling_noise_coefficients.csv` & `carculator_utils-1.0.6/carculator_utils/data/emission_factors/truck/rolling_noise_coefficients.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/emission_factors/two-wheeler/EF_HBEFA42_exhaust.csv` & `carculator_utils-1.0.6/carculator_utils/data/emission_factors/two-wheeler/EF_HBEFA42_exhaust.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/emission_factors/two-wheeler/propulsion_noise_coefficients.csv` & `carculator_utils-1.0.6/carculator_utils/data/emission_factors/two-wheeler/propulsion_noise_coefficients.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/export/ei37_to_ei35.csv` & `carculator_utils-1.0.6/carculator_utils/data/export/ei37_to_ei35.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/export/ei37_to_ei36.csv` & `carculator_utils-1.0.6/carculator_utils/data/export/ei37_to_ei36.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/export/ei38_to_ei37.csv` & `carculator_utils-1.0.6/carculator_utils/data/export/ei38_to_ei37.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/export/references.csv` & `carculator_utils-1.0.6/carculator_utils/data/export/references.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/export/rename_parameters.yml` & `carculator_utils-1.0.6/carculator_utils/data/export/rename_parameters.yml`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/export/simapro-biosphere.json` & `carculator_utils-1.0.6/carculator_utils/data/export/simapro-biosphere.json`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/export/simapro-technosphere-3.5.csv` & `carculator_utils-1.0.6/carculator_utils/data/export/simapro-technosphere-3.5.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/export/simapro_fields.yml` & `carculator_utils-1.0.6/carculator_utils/data/export/simapro_fields.yml`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/fuel/S_concentration_fuel.csv` & `carculator_utils-1.0.6/carculator_utils/data/fuel/S_concentration_fuel.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/fuel/default_fuels.yaml` & `carculator_utils-1.0.6/carculator_utils/data/fuel/default_fuels.yaml`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/fuel/fuel_specs.yaml` & `carculator_utils-1.0.6/carculator_utils/data/fuel/fuel_specs.yaml`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/fuel/share_bio_cng.csv` & `carculator_utils-1.0.6/carculator_utils/data/fuel/share_bio_cng.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/fuel/share_bio_diesel.csv` & `carculator_utils-1.0.6/carculator_utils/data/fuel/share_bio_diesel.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/fuel/share_bio_gasoline.csv` & `carculator_utils-1.0.6/carculator_utils/data/fuel/share_bio_gasoline.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/gradient/bus.csv` & `carculator_utils-1.0.6/carculator_utils/data/gradient/bus.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/gradient/car.csv` & `carculator_utils-1.0.6/carculator_utils/data/gradient/car.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/gradient/truck.csv` & `carculator_utils-1.0.6/carculator_utils/data/gradient/truck.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/gradient/two-wheeler.csv` & `carculator_utils-1.0.6/carculator_utils/data/gradient/two-wheeler.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/lcia/dict_impact_categories.csv` & `carculator_utils-1.0.6/carculator_utils/data/lcia/dict_impact_categories.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/lcia/impact_source_categories.yml` & `carculator_utils-1.0.6/carculator_utils/data/lcia/impact_source_categories.yml`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/monthly_avg_temp.csv` & `carculator_utils-1.0.6/carculator_utils/data/monthly_avg_temp.csv`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/data/purchase_cost_params.yaml` & `carculator_utils-1.0.6/carculator_utils/data/purchase_cost_params.yaml`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/driving_cycles.py` & `carculator_utils-1.0.6/carculator_utils/driving_cycles.py`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/energy_consumption.py` & `carculator_utils-1.0.6/carculator_utils/energy_consumption.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from typing import Any, List, Tuple, Union
 
 import numexpr as ne
 import numpy as np
 import pandas as pd
 import xarray as xr
 import yaml
+from numpy import ndarray
 from xarray import DataArray
 
 from . import DATA_DIR
 from .driving_cycles import (
     get_driving_cycle_specs,
     get_standard_driving_cycle_and_gradient,
 )
@@ -99,16 +100,20 @@
                 "air resistance",
                 "gradient resistance",
                 "kinetic energy",
                 "motive energy at wheels",
                 "motive energy",
                 "negative motive energy",
                 "recuperated energy",
-                "power load",
                 "auxiliary energy",
+                "cooling energy",
+                "heating energy",
+                "battery cooling energy",
+                "battery heating energy",
+                "power load",
                 "transmission efficiency",
                 "engine efficiency",
                 "velocity",
             ],
         },
     )
 
@@ -153,14 +158,16 @@
         vehicle_type: str,
         vehicle_size: List[str],
         powertrains: List[str],
         cycle: Union[str, np.ndarray],
         gradient: Union[str, np.ndarray],
         rho_air: float = 1.204,
         country: str = "CH",
+        ambient_temperature: Union[float, np.ndarray] = None,
+        indoor_temperature: Union[float, np.ndarray] = 20,
     ) -> None:
         if not isinstance(vehicle_size, list):
             vehicle_size = [vehicle_size]
 
         self.rho_air = rho_air
 
         if isinstance(cycle, np.ndarray):
@@ -190,93 +197,135 @@
         assert len(self.cycle) == len(
             self.gradient
         ), "The length of the driving cycle and the gradient must be the same."
 
         # Unit conversion km/h to m/s
         self.velocity = np.where(np.isnan(self.cycle), 0, (self.cycle * 1000) / 3600)
         self.velocity = self.velocity[:, None, None, None, :]
+        self.driving_time = self.find_last_driving_second()
 
         # Model acceleration as difference in velocity between
         # time steps (1 second)
         # Zero at first value
         self.acceleration = np.zeros_like(self.velocity)
         self.acceleration[1:-1] = (self.velocity[2:, ...] - self.velocity[:-2, ...]) / 2
 
         self.efficiency_coefficients = get_efficiency_coefficients(vehicle_type)
 
+        self.ambient_temperature = ambient_temperature
+        self.indoor_temperature = indoor_temperature
+
     def calculate_hvac_energy(
         self,
         hvac_power,
         battery_cooling_unit,
         battery_heating_unit,
-        ambient_temp,
-        indoor_temp,
     ) -> tuple[Any, Any, Any, Any]:
-        if ambient_temp is not None:
-            ambient_temp = np.resize(ambient_temp, (12,))
+        if self.ambient_temperature is not None:
+            if isinstance(self.ambient_temperature, (float, int)):
+                self.ambient_temperature = np.resize(self.ambient_temperature, (12,))
+            else:
+                self.ambient_temperature = np.array(self.ambient_temperature)
+                assert (
+                    len(self.ambient_temperature) == 12
+                ), "Ambient temperature must be a 12-month array"
         else:
-            ambient_temp = get_country_temperature(self.country)
+            self.ambient_temperature = np.resize(
+                get_country_temperature(self.country), (12,)
+            )
+
+        if self.indoor_temperature is not None:
+            if isinstance(self.indoor_temperature, (float, int)):
+                self.indoor_temperature = np.resize(self.indoor_temperature, (12,))
+            else:
+                self.indoor_temperature = np.array(self.indoor_temperature)
+                assert (
+                    len(self.indoor_temperature) == 12
+                ), "Indoor temperature must be a 12-month array"
 
         # use ambient temperature if provided, otherwise
         # monthly temperature average (12 values)
         # relation between ambient temperature
         # and HVAC power required
         # from https://doi.org/10.1016/j.energy.2018.12.064
         amb_temp_data_points = np.array([-30, -20, -10, 0, 10, 20, 30, 40])
         pct_power_HVAC = np.array([0.95, 0.54, 0.29, 0.13, 0.04, 0.08, 0.45, 0.7])
 
         # Heating power as long as ambient temperature, in W
         # is below the comfort indoor temperature
         p_heating = (
             np.where(
-                ambient_temp < indoor_temp,
-                np.interp(ambient_temp, amb_temp_data_points, pct_power_HVAC),
+                self.ambient_temperature < self.indoor_temperature,
+                np.interp(
+                    self.ambient_temperature, amb_temp_data_points, pct_power_HVAC
+                ),
                 0,
             ).mean()
             * hvac_power
         ).values
 
         # Cooling power as long as ambient temperature, in W
         # is above the comfort indoor temperature
         p_cooling = (
             np.where(
-                ambient_temp >= indoor_temp,
-                np.interp(ambient_temp, amb_temp_data_points, pct_power_HVAC),
+                self.ambient_temperature >= self.indoor_temperature,
+                np.interp(
+                    self.ambient_temperature, amb_temp_data_points, pct_power_HVAC
+                ),
                 0,
             ).mean()
             * hvac_power
         ).values
 
         # We want to add power draw for battery cooling
         # and battery heating
 
         # battery cooling occurring above 20C, in W
-        p_battery_cooling = np.where(ambient_temp > 20, _(battery_cooling_unit), 0)
+        p_battery_cooling = np.where(
+            self.ambient_temperature > 20, _(battery_cooling_unit), 0
+        )
         p_battery_cooling = p_battery_cooling.mean(-1)
 
         # battery heating occurring below 5C, in W
-        p_battery_heating = np.where(ambient_temp < 5, _(battery_heating_unit), 0)
+        p_battery_heating = np.where(
+            self.ambient_temperature < 5, _(battery_heating_unit), 0
+        )
         p_battery_heating = p_battery_heating.mean(-1)
 
         return p_cooling, p_heating, p_battery_cooling, p_battery_heating
 
+    def find_last_driving_second(self) -> ndarray:
+        """
+        Find the last second of the driving cycle that is not zero.
+        """
+
+        # find last index where velocity is greater than 0
+        # along the last axis of self.velocity
+        # let's iterate through the last axis of self.velocity
+        # and find the last index where velocity is greater than 0
+        driving_time = np.zeros_like(self.velocity)
+
+        for i in range(self.velocity.shape[-1]):
+            last_index = np.where(self.velocity[..., i] > 0)[0][-1]
+            driving_time[:last_index, ..., i] = 1
+
+        return driving_time
+
     def aux_energy_per_km(
         self,
         aux_power: Union[xr.DataArray, np.array],
         efficiency: Union[xr.DataArray, np.array],
         hvac_power: Union[xr.DataArray, np.array] = None,
         battery_cooling_unit: Union[xr.DataArray, np.array] = None,
         battery_heating_unit: Union[xr.DataArray, np.array] = None,
         heat_pump_cop_cooling: Union[xr.DataArray, np.array] = None,
         heat_pump_cop_heating: Union[xr.DataArray, np.array] = None,
         cooling_consumption: Union[xr.DataArray, np.array] = None,
         heating_consumption: Union[xr.DataArray, np.array] = None,
-        ambient_temp: float = None,
-        indoor_temp: float = 20.0,
-    ) -> Union[float, np.ndarray]:
+    ) -> Union[tuple[Any, Any, Any, Any, Any], Any]:
         """
         Calculate energy used other than motive energy per km driven.
 
         :param aux_power: Total power needed for auxiliaries, heating, and cooling (W)
         :param efficiency: Efficiency of electricity generation (dimensionless, between 0.0 and 1.0).
                 Battery electric vehicles should have efficiencies of one here, as we account for
                 battery efficiencies elsewhere.
@@ -292,36 +341,31 @@
                 p_heating,
                 p_battery_cooling,
                 p_battery_heating,
             ) = self.calculate_hvac_energy(
                 hvac_power=hvac_power,
                 battery_cooling_unit=battery_cooling_unit,
                 battery_heating_unit=battery_heating_unit,
-                ambient_temp=ambient_temp,
-                indoor_temp=indoor_temp,
             )
 
-            aux_energy = (
-                aux_power
-                + (p_cooling / _o(heat_pump_cop_cooling) * cooling_consumption)
-                + (p_heating / _o(heat_pump_cop_heating) * heating_consumption)
-                + p_battery_cooling
-                + p_battery_heating
-            ).T.values * np.ones_like(self.velocity)
-
-            return aux_energy
+            return (
+                aux_power.T.values * np.where(self.velocity > 0, 1, 0),
+                (p_cooling / _o(heat_pump_cop_cooling) * cooling_consumption).T.values
+                * self.driving_time,
+                (p_heating / _o(heat_pump_cop_heating) * heating_consumption).T.values
+                * self.driving_time,
+                p_battery_cooling.T * self.driving_time,
+                p_battery_heating.T * self.driving_time,
+            )
 
         _c = lambda x: x.values if isinstance(x, xr.DataArray) else x
 
         # Provide energy in kJ / km (1 J = 1 Ws)
         auxiliary_energy = (
-            _c(aux_power).T[None, ...]  # Watts
-            * np.ones_like(self.velocity)
-            * 1000  # m / km
-            / 1000  # 1 / (J / kJ)
+            _c(aux_power).T[None, ...] * 1000 / 1000  # Watts  # m / km  # 1 / (J / kJ)
         )
 
         efficiency = _c(efficiency)
 
         return auxiliary_energy / _o(efficiency)
 
     def calculate_efficiency(
@@ -393,16 +437,14 @@
         hvac_power: Union[xr.DataArray, np.array] = None,
         battery_cooling_unit: Union[xr.DataArray, np.array] = None,
         battery_heating_unit: Union[xr.DataArray, np.array] = None,
         heat_pump_cop_cooling: Union[xr.DataArray, np.array] = None,
         heat_pump_cop_heating: Union[xr.DataArray, np.array] = None,
         cooling_consumption: Union[xr.DataArray, np.array] = None,
         heating_consumption: Union[xr.DataArray, np.array] = None,
-        ambient_temp: float = None,
-        indoor_temp: float = 20.0,
     ) -> DataArray:
         """
         Calculate energy used and recuperated for a given vehicle per km driven.
 
         :param driving_mass: Mass of vehicle (kg)
         :param rr_coef: Rolling resistance coefficient (dimensionless, between 0.0 and 1.0)
         :param drag_coef: Aerodynamic drag coefficient (dimensionless, between 0.0 and 1.0)
@@ -502,71 +544,97 @@
                 / _o(_c(transmission_efficiency))
                 / _o(_c(fuel_cell_system_efficiency)).T[None, ...]
             )
 
             engine_load = np.clip(
                 (motive_energy / (_o(_c(engine_power)).T * 1000)) * self.velocity, 0, 1
             )
+
+            # add a minimum 5% engine load when the vehicle is idling
+            engine_load = np.where(self.velocity == 0, 0.05, engine_load)
+            engine_load *= self.driving_time
             engine_load_iterations.append(engine_load.mean())
 
         negative_motive_energy = xr.where(total_resistance > 0, 0, total_resistance)
         recuperated_energy = (
             negative_motive_energy
             * _c(recuperation_efficiency).T[None, ...]
             * _c(battery_charge_eff).T[None, ...]
             * _c(battery_discharge_eff).T[None, ...]
             * (_c(electric_motor_power).T[None, ...] > 0)
         )
 
-        auxiliary_energy = self.aux_energy_per_km(
-            aux_power,
-            engine_efficiency,
-            hvac_power,
-            battery_cooling_unit,
-            battery_heating_unit,
-            heat_pump_cop_cooling,
-            heat_pump_cop_heating,
-            cooling_consumption,
-            heating_consumption,
-            ambient_temp,
-            indoor_temp,
-        )
+        if hvac_power is None:
+            auxiliary_energy = self.aux_energy_per_km(
+                aux_power,
+                engine_efficiency,
+                hvac_power,
+                battery_cooling_unit,
+                battery_heating_unit,
+                heat_pump_cop_cooling,
+                heat_pump_cop_heating,
+                cooling_consumption,
+                heating_consumption,
+            )
+            cooling_energy, heating_energy, battery_cooling, battery_heating = (
+                np.zeros_like(auxiliary_energy),
+                np.zeros_like(auxiliary_energy),
+                np.zeros_like(auxiliary_energy),
+                np.zeros_like(auxiliary_energy),
+            )
+        else:
+            (
+                auxiliary_energy,
+                cooling_energy,
+                heating_energy,
+                battery_cooling,
+                battery_heating,
+            ) = self.aux_energy_per_km(
+                aux_power,
+                engine_efficiency,
+                hvac_power,
+                battery_cooling_unit,
+                battery_heating_unit,
+                heat_pump_cop_cooling,
+                heat_pump_cop_heating,
+                cooling_consumption,
+                heating_consumption,
+            )
+
         auxiliary_energy *= self.velocity > 0
 
         all_arrays = np.concatenate(
             [
                 _(rolling_resistance),
                 _(air_resistance),
                 _(gradient_resistance),
                 _(inertia),
                 _(motive_energy_at_wheels),
                 _(motive_energy),
                 _(negative_motive_energy),
                 _(recuperated_energy),
-                _(engine_load),
                 _(auxiliary_energy),
+                _(cooling_energy),
+                _(heating_energy),
+                _(battery_cooling),
+                _(battery_heating),
+                _(engine_load),
                 _(transmission_efficiency),
                 _(engine_efficiency),
                 _(self.velocity * np.ones_like(motive_energy)),
             ],
             axis=-1,
         )
 
-        all_arrays[..., :-5] /= 1000
-        all_arrays[..., -4] /= 1000
-        all_arrays[..., :-5] *= _(self.velocity)
-
-        all_arrays[..., 4] = np.where(
-            all_arrays[..., 4] > _(engine_power).T,
-            _(engine_power).T,
-            all_arrays[..., 4],
-        )
+        all_arrays[..., :-4] /= 1000
+        all_arrays[..., :-9] *= _(self.velocity)
+
         all_arrays[..., 5] = np.where(
-            all_arrays[..., 5] > _(engine_power).T,
-            _(engine_power).T,
+            all_arrays[..., 5] > _(engine_power).T * 1.15,
+            _(engine_power).T * 1.15,
             all_arrays[..., 5],
         )
         all_arrays[..., 7] = np.where(
             all_arrays[..., 7] < _(electric_motor_power).T * -1,
             _(electric_motor_power).T * -1,
             all_arrays[..., 7],
         )
```

### Comparing `carculator_utils-1.0.5/carculator_utils/export.py` & `carculator_utils-1.0.6/carculator_utils/export.py`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/hot_emissions.py` & `carculator_utils-1.0.6/carculator_utils/hot_emissions.py`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/inventory.py` & `carculator_utils-1.0.6/carculator_utils/inventory.py`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/model.py` & `carculator_utils-1.0.6/carculator_utils/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,16 @@
         payload=None,
         energy_target=None,
         energy_consumption: dict = None,
         target_range: dict = None,
         target_mass: dict = None,
         power: dict = None,
         fuel_blend: dict = None,
+        ambient_temperature: float = None,
+        indoor_temperature: float = 20,
     ) -> None:
         """
         :param array: multi-dimensional numpy-like array that contains parameters' value(s)
         :param country: country code
         :param cycle: name of a driving cycle, or custom driving cycle
         :param gradient: series of gradients, for each second of the driving cycle
         :param energy_storage: dictionary with selection of battery chemistry, capacity and origin for each powertrain-size-year combination
@@ -99,14 +101,17 @@
         if fuel_blend:
             self.fuel_blend = self.check_fuel_blend(fuel_blend)
         else:
             self.fuel_blend = self.bs.define_fuel_blends(
                 self.array.powertrain.values, self.country, self.array.year.values
             )
 
+        self.ambient_temperature = ambient_temperature
+        self.indoor_temperature = indoor_temperature
+
     def __call__(self, key: Union[str, List]):
         """
         This method fixes a dimension of the `array` attribute given
         a powertrain technology selected.
         Set up this class as a context manager,
         so we can have some nice syntax
 
@@ -644,18 +649,17 @@
         Calculate the share of recuperated energy,
         over the total negative motive energy.
         """
 
         _ = lambda x: np.where(x == 0, 1, x)
 
         self["share recuperated energy"] = (
-            self.energy.sel(parameter="recuperated energy").sum(dim="second")
+            _(self.energy.sel(parameter="recuperated energy").sum(dim="second"))
             / _(self.energy.sel(parameter="negative motive energy").sum(dim="second"))
-            * (self["combustion power share"] < 1)
-        ).T
+        ).T * (self["combustion power share"] < 1)
 
         if "PHEV-d" in self.array.powertrain:
             self.array.loc[
                 dict(powertrain="PHEV-c-d", parameter="share recuperated energy")
             ] = self.array.loc[
                 dict(powertrain="PHEV-e", parameter="share recuperated energy")
             ]
@@ -668,14 +672,15 @@
             ]
 
     def set_electric_utility_factor(self) -> None:
         pass
 
     def create_PHEV(self):
         """
+        Function to create plugin-hybrid vehicles.
         PHEV-p/d is the range-weighted average
         between PHEV-c-p/PHEV-c-d and PHEV-e.
         """
         _ = lambda array: np.where(array == 0, 1, array)
 
         for pwt, pwtc in (("PHEV-d", "PHEV-c-d"), ("PHEV-p", "PHEV-c-p")):
             if pwt in self.array.coords["powertrain"].values:
@@ -1319,15 +1324,15 @@
             yearly_km=self["kilometers per year"],
         )
 
         self.array.loc[
             dict(
                 parameter=list_direct_emissions,
             )
-        ] = hot_emissions
+        ] = hot_emissions.values
 
     def set_particulates_emission(self) -> None:
         """
         Calculate the emission of particulates according to
         https://www.eea.europa.eu/ds_resolveuid/6USNA27I4D
 
         and further disaggregated in:
```

### Comparing `carculator_utils-1.0.5/carculator_utils/noise_emissions.py` & `carculator_utils-1.0.6/carculator_utils/noise_emissions.py`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/particulates_emissions.py` & `carculator_utils-1.0.6/carculator_utils/particulates_emissions.py`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils/vehicle_input_parameters.py` & `carculator_utils-1.0.6/carculator_utils/vehicle_input_parameters.py`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/carculator_utils.egg-info/PKG-INFO` & `carculator_utils-1.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: carculator-utils
-Version: 1.0.5
+Name: carculator_utils
+Version: 1.0.6
 Summary: Provides convenience functions for carculator_utils
 Home-page: https://github.com/romainsacchi/carculator_utils
 Author: Romain Sacchi <romain.sacchi@psi.ch>
 License: BSD 3-Clause License
         
         Copyright (c) 2020, Paul Scherrer Institut
         
@@ -53,14 +53,20 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ``carculator_utils``
 
 
 Base classes and functions for the carculator package suite.
+Provides base classes to:
+
+* carculator
+* carculator_bus
+* carculator_truck
+* carculator_two-wheeler
 
 ## Support
 
 Do not hesitate to contact the development team at [carculator@psi.ch](mailto:carculator@psi.ch).
 
 ## Maintainers
 
@@ -68,8 +74,8 @@
 
 ## Contributing
 
 See [contributing](https://github.com/romainsacchi/carculator_utils/blob/master/CONTRIBUTING.md).
 
 ## License
 
-[BSD-3-Clause](https://github.com/romainsacchi/carculator_utils/blob/master/LICENSE). Copyright 2020 Paul Scherrer Institut.
+[BSD-3-Clause](https://github.com/romainsacchi/carculator_utils/blob/master/LICENSE). Copyright 2023 Paul Scherrer Institut.
```

### Comparing `carculator_utils-1.0.5/carculator_utils.egg-info/SOURCES.txt` & `carculator_utils-1.0.6/carculator_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/readthedocs.yml` & `carculator_utils-1.0.6/readthedocs.yml`

 * *Files identical despite different names*

### Comparing `carculator_utils-1.0.5/setup.py` & `carculator_utils-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="carculator_utils",
-    version="1.0.5",
+    version="1.0.6",
     packages=packages,
     author="Romain Sacchi <romain.sacchi@psi.ch>",
     python_requires=">=3.9",
     license=open("LICENSE").read(),
     package_data={
         "carculator_utils": package_files(os.path.join("carculator_utils", "data"))
     },
```

### Comparing `carculator_utils-1.0.5/tests/test_vehicle_input_parameters.py` & `carculator_utils-1.0.6/tests/test_vehicle_input_parameters.py`

 * *Files identical despite different names*

