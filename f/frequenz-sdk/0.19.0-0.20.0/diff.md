# Comparing `tmp/frequenz-sdk-0.19.0.tar.gz` & `tmp/frequenz-sdk-0.20.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frequenz-sdk-0.19.0.tar", last modified: Wed Mar 15 15:48:28 2023, max compression
+gzip compressed data, was "frequenz-sdk-0.20.0.tar", last modified: Tue Apr 25 14:15:54 2023, max compression
```

## Comparing `frequenz-sdk-0.19.0.tar` & `frequenz-sdk-0.20.0.tar`

### file list

```diff
@@ -1,117 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 15:48:28.741970 frequenz-sdk-0.19.0/
--rw-r--r--   0 runner    (1001) docker     (122)     4430 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)     1090 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      225 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2111 2023-03-15 15:48:28.741970 frequenz-sdk-0.19.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      830 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     2046 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/RELEASE_NOTES.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 15:48:28.713970 frequenz-sdk-0.19.0/docs/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/docs/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)       82 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/docs/SUMMARY.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 15:48:28.713970 frequenz-sdk-0.19.0/docs/css/
--rw-r--r--   0 runner    (1001) docker     (122)     1340 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/docs/css/mkdocstrings.css
--rw-r--r--   0 runner    (1001) docker     (122)     1131 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/docs/css/style.css
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (122)    57278 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/docs/logo.png
--rw-r--r--   0 runner    (1001) docker     (122)     1737 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/docs/mkdocstrings_autoapi.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 15:48:28.713970 frequenz-sdk-0.19.0/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (122)      222 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (122)     2542 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (122)     4253 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-15 15:48:28.741970 frequenz-sdk-0.19.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 15:48:28.709970 frequenz-sdk-0.19.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 15:48:28.701970 frequenz-sdk-0.19.0/src/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 15:48:28.717970 frequenz-sdk-0.19.0/src/frequenz/sdk/
--rw-r--r--   0 runner    (1001) docker     (122)       97 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 15:48:28.717970 frequenz-sdk-0.19.0/src/frequenz/sdk/_api_client/
--rw-r--r--   0 runner    (1001) docker     (122)      214 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/_api_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1201 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/_api_client/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 15:48:28.717970 frequenz-sdk-0.19.0/src/frequenz/sdk/_internal/
--rw-r--r--   0 runner    (1001) docker     (122)      231 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      648 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/_internal/_constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     1158 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/_internal/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (122)      842 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/_internal/singleton_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 15:48:28.721970 frequenz-sdk-0.19.0/src/frequenz/sdk/actor/
--rw-r--r--   0 runner    (1001) docker     (122)      670 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/actor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2024 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/actor/_channel_registry.py
--rw-r--r--   0 runner    (1001) docker     (122)     2653 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/actor/_config_managing.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 15:48:28.721970 frequenz-sdk-0.19.0/src/frequenz/sdk/actor/_data_sourcing/
--rw-r--r--   0 runner    (1001) docker     (122)      272 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/actor/_data_sourcing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/actor/_data_sourcing/data_sourcing.py
--rw-r--r--   0 runner    (1001) docker     (122)    15571 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/actor/_data_sourcing/microgrid_api_source.py
--rw-r--r--   0 runner    (1001) docker     (122)     6903 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/actor/_decorator.py
--rw-r--r--   0 runner    (1001) docker     (122)     6983 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/actor/_resampling.py
--rw-r--r--   0 runner    (1001) docker     (122)     1810 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/actor/_run_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 15:48:28.721970 frequenz-sdk-0.19.0/src/frequenz/sdk/actor/power_distributing/
--rw-r--r--   0 runner    (1001) docker     (122)      868 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/actor/power_distributing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7708 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/actor/power_distributing/_battery_pool_status.py
--rw-r--r--   0 runner    (1001) docker     (122)    16522 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/actor/power_distributing/_battery_status.py
--rw-r--r--   0 runner    (1001) docker     (122)    28171 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/actor/power_distributing/power_distributing.py
--rw-r--r--   0 runner    (1001) docker     (122)      784 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/actor/power_distributing/request.py
--rw-r--r--   0 runner    (1001) docker     (122)     4080 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/actor/power_distributing/result.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 15:48:28.725970 frequenz-sdk-0.19.0/src/frequenz/sdk/config/
--rw-r--r--   0 runner    (1001) docker     (122)      189 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5008 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/config/_config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 15:48:28.725970 frequenz-sdk-0.19.0/src/frequenz/sdk/microgrid/
--rw-r--r--   0 runner    (1001) docker     (122)      499 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/microgrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    21890 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/microgrid/_graph.py
--rw-r--r--   0 runner    (1001) docker     (122)     5339 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/microgrid/_microgrid.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 15:48:28.725970 frequenz-sdk-0.19.0/src/frequenz/sdk/microgrid/client/
--rw-r--r--   0 runner    (1001) docker     (122)      488 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/microgrid/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    23726 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/microgrid/client/_client.py
--rw-r--r--   0 runner    (1001) docker     (122)      583 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/microgrid/client/_connection.py
--rw-r--r--   0 runner    (1001) docker     (122)     4873 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/microgrid/client/_retry.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 15:48:28.729970 frequenz-sdk-0.19.0/src/frequenz/sdk/microgrid/component/
--rw-r--r--   0 runner    (1001) docker     (122)      721 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/microgrid/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4789 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/microgrid/component/_component.py
--rw-r--r--   0 runner    (1001) docker     (122)    10579 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/microgrid/component/_component_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     2632 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/microgrid/component/_component_states.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 15:48:28.729970 frequenz-sdk-0.19.0/src/frequenz/sdk/power/
--rw-r--r--   0 runner    (1001) docker     (122)      315 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/power/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    18075 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/power/_distribution_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 15:48:28.729970 frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/
--rw-r--r--   0 runner    (1001) docker     (122)      298 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1722 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/_base_types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 15:48:28.733970 frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/_formula_engine/
--rw-r--r--   0 runner    (1001) docker     (122)      630 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/_formula_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      225 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/_formula_engine/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    28125 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_engine.py
--rw-r--r--   0 runner    (1001) docker     (122)     4005 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_engine_pool.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 15:48:28.737970 frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/
--rw-r--r--   0 runner    (1001) docker     (122)     1022 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2663 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_battery_power_formula.py
--rw-r--r--   0 runner    (1001) docker     (122)     3043 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_ev_charger_current_formula.py
--rw-r--r--   0 runner    (1001) docker     (122)     1800 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_ev_charger_power_formula.py
--rw-r--r--   0 runner    (1001) docker     (122)     2465 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_formula_generator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3414 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_grid_current_formula.py
--rw-r--r--   0 runner    (1001) docker     (122)     2540 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_grid_power_formula.py
--rw-r--r--   0 runner    (1001) docker     (122)     2173 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_pv_power_formula.py
--rw-r--r--   0 runner    (1001) docker     (122)     7495 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_steps.py
--rw-r--r--   0 runner    (1001) docker     (122)     4292 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/_formula_engine/_resampled_formula_builder.py
--rw-r--r--   0 runner    (1001) docker     (122)     4573 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/_formula_engine/_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (122)     7943 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/_moving_window.py
--rw-r--r--   0 runner    (1001) docker     (122)    27273 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/_resampling.py
--rw-r--r--   0 runner    (1001) docker     (122)    17417 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/_ringbuffer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3220 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/_serializable_ringbuffer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 15:48:28.737970 frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/battery_pool/
--rw-r--r--   0 runner    (1001) docker     (122)      327 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/battery_pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8394 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/battery_pool/_component_metric_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     2137 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/battery_pool/_component_metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)     9089 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/battery_pool/_methods.py
--rw-r--r--   0 runner    (1001) docker     (122)    16450 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/battery_pool/_metric_calculator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3709 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/battery_pool/_result_types.py
--rw-r--r--   0 runner    (1001) docker     (122)     7355 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/battery_pool/battery_pool.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 15:48:28.741970 frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/ev_charger_pool/
--rw-r--r--   0 runner    (1001) docker     (122)      188 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/ev_charger_pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5444 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/ev_charger_pool/_ev_charger_pool.py
--rw-r--r--   0 runner    (1001) docker     (122)     6023 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/ev_charger_pool/_state_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 15:48:28.741970 frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/logical_meter/
--rw-r--r--   0 runner    (1001) docker     (122)      214 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/logical_meter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7248 2023-03-15 15:48:18.000000 frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/logical_meter/_logical_meter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-15 15:48:28.741970 frequenz-sdk-0.19.0/src/frequenz_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2111 2023-03-15 15:48:28.000000 frequenz-sdk-0.19.0/src/frequenz_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4300 2023-03-15 15:48:28.000000 frequenz-sdk-0.19.0/src/frequenz_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-15 15:48:28.000000 frequenz-sdk-0.19.0/src/frequenz_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1004 2023-03-15 15:48:28.000000 frequenz-sdk-0.19.0/src/frequenz_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-03-15 15:48:28.000000 frequenz-sdk-0.19.0/src/frequenz_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:54.955660 frequenz-sdk-0.20.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     4430 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1090 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      225 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2111 2023-04-25 14:15:54.955660 frequenz-sdk-0.20.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      830 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     4101 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/RELEASE_NOTES.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:54.943659 frequenz-sdk-0.20.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/docs/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)       82 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/docs/SUMMARY.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:54.943659 frequenz-sdk-0.20.0/docs/css/
+-rw-r--r--   0 runner    (1001) docker     (122)     1340 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/docs/css/mkdocstrings.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1131 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/docs/css/style.css
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (122)    57278 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/docs/logo.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1737 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/docs/mkdocstrings_autoapi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:54.943659 frequenz-sdk-0.20.0/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (122)      222 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2542 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3881 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-25 14:15:54.955660 frequenz-sdk-0.20.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:54.939659 frequenz-sdk-0.20.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:54.939659 frequenz-sdk-0.20.0/src/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:54.943659 frequenz-sdk-0.20.0/src/frequenz/sdk/
+-rw-r--r--   0 runner    (1001) docker     (122)       97 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:54.943659 frequenz-sdk-0.20.0/src/frequenz/sdk/_api_client/
+-rw-r--r--   0 runner    (1001) docker     (122)      214 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/_api_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1201 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/_api_client/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:54.943659 frequenz-sdk-0.20.0/src/frequenz/sdk/_internal/
+-rw-r--r--   0 runner    (1001) docker     (122)      231 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      648 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/_internal/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/_internal/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (122)      842 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/_internal/singleton_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:54.943659 frequenz-sdk-0.20.0/src/frequenz/sdk/actor/
+-rw-r--r--   0 runner    (1001) docker     (122)      670 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/actor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2024 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/actor/_channel_registry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2656 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/actor/_config_managing.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:54.943659 frequenz-sdk-0.20.0/src/frequenz/sdk/actor/_data_sourcing/
+-rw-r--r--   0 runner    (1001) docker     (122)      272 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/actor/_data_sourcing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/actor/_data_sourcing/data_sourcing.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15634 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/actor/_data_sourcing/microgrid_api_source.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6865 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/actor/_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6890 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/actor/_resampling.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1810 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/actor/_run_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:54.947659 frequenz-sdk-0.20.0/src/frequenz/sdk/actor/power_distributing/
+-rw-r--r--   0 runner    (1001) docker     (122)      868 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/actor/power_distributing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7708 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/actor/power_distributing/_battery_pool_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17217 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/actor/power_distributing/_battery_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29122 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/actor/power_distributing/power_distributing.py
+-rw-r--r--   0 runner    (1001) docker     (122)      887 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/actor/power_distributing/request.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3070 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/actor/power_distributing/result.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:54.947659 frequenz-sdk-0.20.0/src/frequenz/sdk/config/
+-rw-r--r--   0 runner    (1001) docker     (122)      189 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5012 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/config/_config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:54.947659 frequenz-sdk-0.20.0/src/frequenz/sdk/microgrid/
+-rw-r--r--   0 runner    (1001) docker     (122)     1058 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/microgrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12697 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/microgrid/_data_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21892 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/microgrid/_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:54.947659 frequenz-sdk-0.20.0/src/frequenz/sdk/microgrid/client/
+-rw-r--r--   0 runner    (1001) docker     (122)      488 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/microgrid/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23732 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/microgrid/client/_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)      583 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/microgrid/client/_connection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4873 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/microgrid/client/_retry.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:54.947659 frequenz-sdk-0.20.0/src/frequenz/sdk/microgrid/component/
+-rw-r--r--   0 runner    (1001) docker     (122)      721 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/microgrid/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4789 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/microgrid/component/_component.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10579 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/microgrid/component/_component_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2632 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/microgrid/component/_component_states.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5360 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/microgrid/connection_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:54.947659 frequenz-sdk-0.20.0/src/frequenz/sdk/power/
+-rw-r--r--   0 runner    (1001) docker     (122)      315 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/power/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18075 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/power/_distribution_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:54.947659 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (122)     1556 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4493 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_base_types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:54.951660 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/
+-rw-r--r--   0 runner    (1001) docker     (122)      415 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      225 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24805 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_engine.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3837 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_engine_pool.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:54.951660 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/
+-rw-r--r--   0 runner    (1001) docker     (122)     1022 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2789 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_battery_power_formula.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2945 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_ev_charger_current_formula.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1784 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_ev_charger_power_formula.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2480 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_formula_generator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3212 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_grid_current_formula.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2551 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_grid_power_formula.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2180 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_pv_power_formula.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7495 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_steps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4575 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_resampled_formula_builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4573 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10633 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_moving_window.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28722 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_resampling.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:54.951660 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_ringbuffer/
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_ringbuffer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17660 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_ringbuffer/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_ringbuffer/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:54.951660 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/battery_pool/
+-rw-r--r--   0 runner    (1001) docker     (122)      327 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/battery_pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8410 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/battery_pool/_component_metric_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2137 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/battery_pool/_component_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9089 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/battery_pool/_methods.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16477 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/battery_pool/_metric_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3709 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/battery_pool/_result_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9017 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/battery_pool/battery_pool.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:54.951660 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/ev_charger_pool/
+-rw-r--r--   0 runner    (1001) docker     (122)      419 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/ev_charger_pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10536 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/ev_charger_pool/_ev_charger_pool.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4676 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/ev_charger_pool/_set_current_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4106 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/ev_charger_pool/_state_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:54.951660 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/logical_meter/
+-rw-r--r--   0 runner    (1001) docker     (122)      214 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/logical_meter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6910 2023-04-25 14:15:40.000000 frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/logical_meter/_logical_meter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 14:15:54.955660 frequenz-sdk-0.20.0/src/frequenz_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2111 2023-04-25 14:15:54.000000 frequenz-sdk-0.20.0/src/frequenz_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4480 2023-04-25 14:15:54.000000 frequenz-sdk-0.20.0/src/frequenz_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 14:15:54.000000 frequenz-sdk-0.20.0/src/frequenz_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      925 2023-04-25 14:15:54.000000 frequenz-sdk-0.20.0/src/frequenz_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-25 14:15:54.000000 frequenz-sdk-0.20.0/src/frequenz_sdk.egg-info/top_level.txt
```

### Comparing `frequenz-sdk-0.19.0/CONTRIBUTING.md` & `frequenz-sdk-0.20.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.19.0/LICENSE` & `frequenz-sdk-0.20.0/LICENSE`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.19.0/PKG-INFO` & `frequenz-sdk-0.20.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequenz-sdk
-Version: 0.19.0
+Version: 0.20.0
 Summary: Frequenz Python SDK
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-sdk-python/releases
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-sdk-python
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-sdk-python/issues
 Project-URL: Support, https://github.com/frequenz-floss/frequenz-sdk-python/discussions/categories/support
```

### Comparing `frequenz-sdk-0.19.0/README.md` & `frequenz-sdk-0.20.0/README.md`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.19.0/docs/css/mkdocstrings.css` & `frequenz-sdk-0.20.0/docs/css/mkdocstrings.css`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.19.0/docs/css/style.css` & `frequenz-sdk-0.20.0/docs/css/style.css`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.19.0/docs/logo.png` & `frequenz-sdk-0.20.0/docs/logo.png`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.19.0/docs/mkdocstrings_autoapi.py` & `frequenz-sdk-0.20.0/docs/mkdocstrings_autoapi.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.19.0/mkdocs.yml` & `frequenz-sdk-0.20.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.19.0/pyproject.toml` & `frequenz-sdk-0.20.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -22,19 +22,19 @@
    "Programming Language :: Python :: 3.9",
    "Programming Language :: Python :: 3.10",
    "Topic :: Software Development :: Libraries",
 ]
 requires-python = ">= 3.8, < 4"
 dependencies = [
     "frequenz-api-microgrid >= 0.11.0, < 0.12.0",
-    "frequenz-channels >= 0.13.0, < 0.14.0",
+    "frequenz-channels >= 0.14.0, < 0.15.0",
     "google-api-python-client >= 2.71, < 3",
     "grpcio >= 1.51.1, < 2",
     "grpcio-tools >= 1.51.1, < 2",
-    "networkx >= 2.8, < 3",
+    "networkx >= 2.8, < 4",
     "numpy >= 1.24.2, < 2",
     "protobuf >= 4.21.6, < 5",
     "pydantic >= 1.9",
     "sympy >= 1.10.1, < 2",
     "toml >= 0.10",
     "tqdm >= 4.38.0, < 5",
     "typing_extensions >= 4.4.0, < 5",
@@ -44,50 +44,50 @@
 
 [[project.authors]]
 name ="Frequenz Energy-as-a-Service GmbH"
 email = "floss@frequenz.com"
 
 [project.optional-dependencies]
 docs-gen = [
-    "mike >= 1.1.2, < 2",
-    "mkdocs-gen-files >= 0.4.0, < 0.5.0",
-    "mkdocs-literate-nav >= 0.4.0, < 0.5.0",
-    "mkdocs-material >= 8.5.7, < 9",
-    "mkdocs-section-index >= 0.3.4, < 0.4.0",
-    "mkdocstrings[python] >= 0.19.0, < 0.20.0",
+    "mike == 1.1.2",
+    "mkdocs-gen-files == 0.4.0",
+    "mkdocs-literate-nav == 0.6.0",
+    "mkdocs-material == 9.1.8",
+    "mkdocs-section-index == 0.3.5",
+    "mkdocstrings[python] == 0.21.2",
 ]
 docs-lint = [
-    "pydocstyle >= 6.3.0, < 7",
-    "darglint >= 1.8.1, < 2",
-    "tomli >= 2.0.1, < 3",  # Needed by pydocstyle to read pyproject.toml
+    "pydocstyle == 6.3.0",
+    "darglint == 1.8.1",
+    "tomli == 2.0.1",  # Needed by pydocstyle to read pyproject.toml
 ]
 format = [
-    "black >= 23.1.0, < 24",
-    "isort >= 5.12.0, < 6",
+    "black == 23.3.0",
+    "isort == 5.12.0",
 ]
 nox = [
-    "nox == 2022.11.21",
-    "toml >= 0.10.2, < 1",
+    "nox == 2023.4.22",
+    "toml == 0.10.2",
 ]
 pytest = [
-    "pytest >= 7.2.1, < 8",
-    "pytest-cov >= 4.0.0, < 5",
-    "pytest-mock >= 3.10.0, < 4",
-    "pytest-asyncio >= 0.20.3, < 1",
-    "time-machine >= 2.9.0, < 3",
-    "async-solipsism >= 0.5, < 1",
+    "pytest == 7.3.1",
+    "pytest-cov == 4.0.0",
+    "pytest-mock == 3.10.0",
+    "pytest-asyncio == 0.21.0",
+    "time-machine == 2.9.0",
+    "async-solipsism == 0.5",
 ]
 mypy = [
-    "mypy >= 1.0.1, < 2",
+    "mypy == 1.2.0",
     "grpc-stubs == 1.24.12",  # This dependency introduces breaking changes in patch releases
     # For checking the noxfile, docs/ script, and tests
     "frequenz-sdk[docs-gen,nox,pytest]",
 ]
 pylint = [
-    "pylint >= 2.17.0, < 3",
+    "pylint == 2.17.3",
     # For checking the noxfile, docs/ script, and tests
     "frequenz-sdk[docs-gen,nox,pytest]",
 ]
 dev = [
     "frequenz-sdk[docs-gen,docs-lint,format,nox,pytest,mypy,pylint]",
 ]
 
@@ -130,20 +130,14 @@
 line_length = 88
 src_paths = ["src", "examples", "tests"]
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 required_plugins = [ "pytest-asyncio", "pytest-mock" ]
 
-[tool.mypy]
-# This is a temporary hack, for details see:
-# * https://github.com/frequenz-floss/frequenz-sdk-python/pull/219
-# * https://github.com/frequenz-floss/frequenz-sdk-python/issues/226
-exclude = ["src/frequenz/sdk/timeseries/_formula_engine/"]
-
 [[tool.mypy.overrides]]
 module = [
     "grpc.aio",
     "grpc.aio.*",
     # There is a stubs package available, but it's not working:
     # https://github.com/eggplants/networkx-stubs/issues/1
     "networkx",
```

### Comparing `frequenz-sdk-0.19.0/src/frequenz/sdk/_api_client/api_client.py` & `frequenz-sdk-0.20.0/src/frequenz/sdk/_api_client/api_client.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.19.0/src/frequenz/sdk/_internal/_constants.py` & `frequenz-sdk-0.20.0/src/frequenz/sdk/_internal/_constants.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.19.0/src/frequenz/sdk/_internal/asyncio.py` & `frequenz-sdk-0.20.0/src/frequenz/sdk/_internal/asyncio.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,19 +9,23 @@
 from abc import ABC
 from typing import Any
 
 
 async def cancel_and_await(task: asyncio.Task[Any]) -> None:
     """Cancel a task and wait for it to finish.
 
+    Exits immediately if the task is already done.
+
     The `CancelledError` is suppresed, but any other exception will be propagated.
 
     Args:
         task: The task to be cancelled and waited for.
     """
+    if task.done():
+        return
     task.cancel()
     try:
         await task
     except asyncio.CancelledError:
         pass
```

### Comparing `frequenz-sdk-0.19.0/src/frequenz/sdk/_internal/singleton_meta.py` & `frequenz-sdk-0.20.0/src/frequenz/sdk/_internal/singleton_meta.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.19.0/src/frequenz/sdk/actor/__init__.py` & `frequenz-sdk-0.20.0/src/frequenz/sdk/actor/__init__.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.19.0/src/frequenz/sdk/actor/_channel_registry.py` & `frequenz-sdk-0.20.0/src/frequenz/sdk/actor/_channel_registry.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.19.0/src/frequenz/sdk/actor/_config_managing.py` & `frequenz-sdk-0.20.0/src/frequenz/sdk/actor/_config_managing.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import toml
 from frequenz.channels import Sender
 from frequenz.channels.util import FileWatcher
 
 from ..actor._decorator import actor
 from ..config import Config
 
-logger = logging.getLogger(__name__)
+_logger = logging.getLogger(__name__)
 
 
 @actor
 class ConfigManagingActor:
     """
     Manages config variables.
 
@@ -76,14 +76,14 @@
         can be cache in the Broadcast channel and served to receivers even if
         there hasn't been any change to the config file itself.
         """
         await self.send_config()
 
         async for path in self._file_watcher:
             if str(path) == self._conf_file:
-                logger.info(
+                _logger.info(
                     "Update configs, because file %s was modified.",
                     self._conf_file,
                 )
                 await self.send_config()
 
-        logger.debug("ConfigManager stopped.")
+        _logger.debug("ConfigManager stopped.")
```

### Comparing `frequenz-sdk-0.19.0/src/frequenz/sdk/actor/_data_sourcing/data_sourcing.py` & `frequenz-sdk-0.20.0/src/frequenz/sdk/actor/_data_sourcing/data_sourcing.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.19.0/src/frequenz/sdk/actor/_data_sourcing/microgrid_api_source.py` & `frequenz-sdk-0.20.0/src/frequenz/sdk/actor/_data_sourcing/microgrid_api_source.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import logging
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Any, Callable, Dict, List, Optional, Tuple
 
 from frequenz.channels import Receiver, Sender
 
-from ... import microgrid
+from ...microgrid import connection_manager
 from ...microgrid.component import (
     BatteryData,
     ComponentCategory,
     ComponentMetricId,
     EVChargerData,
     InverterData,
     MeterData,
@@ -134,15 +134,15 @@
         Returns:
             The category of the given component, if it is a valid component, or None
                 otherwise.
         """
         if comp_id in self._comp_categories_cache:
             return self._comp_categories_cache[comp_id]
 
-        api = microgrid.get().api_client
+        api = connection_manager.get().api_client
         for comp in await api.components():
             self._comp_categories_cache[comp.component_id] = comp.category
 
         if comp_id in self._comp_categories_cache:
             return self._comp_categories_cache[comp_id]
 
         return None
@@ -164,15 +164,15 @@
         """
         for metric in requests:
             if metric not in _BatteryDataMethods:
                 raise ValueError(f"Unknown metric {metric} for Battery id {comp_id}")
         if comp_id not in self.comp_data_receivers:
             self.comp_data_receivers[
                 comp_id
-            ] = await microgrid.get().api_client.battery_data(comp_id)
+            ] = await connection_manager.get().api_client.battery_data(comp_id)
 
     async def _check_ev_charger_request(
         self,
         comp_id: int,
         requests: Dict[ComponentMetricId, List[ComponentMetricRequest]],
     ) -> None:
         """Check if the requests are valid EV Charger metrics.
@@ -187,15 +187,15 @@
         """
         for metric in requests:
             if metric not in _EVChargerDataMethods:
                 raise ValueError(f"Unknown metric {metric} for EvCharger id {comp_id}")
         if comp_id not in self.comp_data_receivers:
             self.comp_data_receivers[
                 comp_id
-            ] = await microgrid.get().api_client.ev_charger_data(comp_id)
+            ] = await connection_manager.get().api_client.ev_charger_data(comp_id)
 
     async def _check_inverter_request(
         self,
         comp_id: int,
         requests: Dict[ComponentMetricId, List[ComponentMetricRequest]],
     ) -> None:
         """Check if the requests are valid Inverter metrics.
@@ -210,15 +210,15 @@
         """
         for metric in requests:
             if metric not in _InverterDataMethods:
                 raise ValueError(f"Unknown metric {metric} for Inverter id {comp_id}")
         if comp_id not in self.comp_data_receivers:
             self.comp_data_receivers[
                 comp_id
-            ] = await microgrid.get().api_client.inverter_data(comp_id)
+            ] = await connection_manager.get().api_client.inverter_data(comp_id)
 
     async def _check_meter_request(
         self,
         comp_id: int,
         requests: Dict[ComponentMetricId, List[ComponentMetricRequest]],
     ) -> None:
         """Check if the requests are valid Meter metrics.
@@ -233,15 +233,15 @@
         """
         for metric in requests:
             if metric not in _MeterDataMethods:
                 raise ValueError(f"Unknown metric {metric} for Meter id {comp_id}")
         if comp_id not in self.comp_data_receivers:
             self.comp_data_receivers[
                 comp_id
-            ] = await microgrid.get().api_client.meter_data(comp_id)
+            ] = await connection_manager.get().api_client.meter_data(comp_id)
 
     async def _check_requested_component_and_metrics(
         self,
         comp_id: int,
         category: ComponentCategory,
         requests: Dict[ComponentMetricId, List[ComponentMetricRequest]],
     ) -> None:
```

### Comparing `frequenz-sdk-0.19.0/src/frequenz/sdk/actor/_decorator.py` & `frequenz-sdk-0.20.0/src/frequenz/sdk/actor/_decorator.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 """
 
 import asyncio
 import inspect
 import logging
 from typing import Any, Generic, Optional, Type, TypeVar
 
-logger = logging.getLogger(__name__)
+from frequenz.sdk._internal.asyncio import cancel_and_await
+
+_logger = logging.getLogger(__name__)
 
 OT = TypeVar("OT")
 
 
 def _check_run_method_exists(cls: Type[Any]) -> None:
     """Check if a run method exists in the given class.
 
@@ -195,40 +197,36 @@
 
         async def _start_actor(self) -> None:
             """Run the main logic of the actor as a coroutine.
 
             Raises:
                 asyncio.CancelledError: when the actor's task gets cancelled.
             """
-            logger.debug("Starting actor: %s", cls.__name__)
+            _logger.debug("Starting actor: %s", cls.__name__)
             number_of_restarts = 0
             while (
                 self.restart_limit is None or number_of_restarts <= self.restart_limit
             ):
                 if number_of_restarts > 0:
-                    logger.info("Restarting actor: %s", cls.__name__)
+                    _logger.info("Restarting actor: %s", cls.__name__)
 
                 try:
                     await super().run()
                 except asyncio.CancelledError:
-                    logger.debug("Cancelling actor: %s", cls.__name__)
+                    _logger.debug("Cancelling actor: %s", cls.__name__)
                     raise
                 except Exception:  # pylint: disable=broad-except
-                    logger.exception("Actor (%s) crashed", cls.__name__)
+                    _logger.exception("Actor (%s) crashed", cls.__name__)
                 finally:
                     number_of_restarts += 1
 
-            logger.info("Shutting down actor: %s", cls.__name__)
+            _logger.info("Shutting down actor: %s", cls.__name__)
 
         async def _stop(self) -> None:
             """Stop an running actor."""
-            self._actor_task.cancel()
-            try:
-                await self._actor_task
-            except asyncio.CancelledError:
-                pass
+            await cancel_and_await(self._actor_task)
 
         async def join(self) -> None:
             """Await the actor's task, and return when the task completes."""
             await self._actor_task
 
     return ActorClass
```

### Comparing `frequenz-sdk-0.19.0/src/frequenz/sdk/actor/_resampling.py` & `frequenz-sdk-0.20.0/src/frequenz/sdk/actor/_resampling.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from .._internal.asyncio import cancel_and_await
 from ..timeseries import Sample
 from ..timeseries._resampling import Resampler, ResamplerConfig, ResamplingError
 from ._channel_registry import ChannelRegistry
 from ._data_sourcing import ComponentMetricRequest
 from ._decorator import actor
 
-logger = logging.getLogger(__name__)
+_logger = logging.getLogger(__name__)
 
 
 @actor
 class ComponentMetricsResamplingActor:
     """An actor to resample microgrid component metrics."""
 
     def __init__(  # pylint: disable=too-many-arguments
@@ -77,16 +77,15 @@
         receiver = self._channel_registry.new_receiver(data_source_channel_name)
 
         # This is a temporary hack until the Sender implementation uses
         # exceptions to report errors.
         sender = self._channel_registry.new_sender(request.get_channel_name())
 
         async def sink_adapter(sample: Sample) -> None:
-            if not await sender.send(sample):
-                raise RuntimeError(f"Error while sending with sender {sender}", sender)
+            await sender.send(sample)
 
         self._resampler.add_timeseries(request_channel_name, receiver, sink_adapter)
 
     async def _process_resampling_requests(self) -> None:
         """Process resampling data requests."""
         async for request in self._resampling_request_receiver:
             await self._subscribe(request)
@@ -136,20 +135,20 @@
 
                     # We don't know what to do with something other than
                     # ResamplingError, so propagate the exception if that is the
                     # case.
                     if not isinstance(error, ResamplingError):
                         raise error
                     for source, source_error in error.exceptions.items():
-                        logger.error(
+                        _logger.error(
                             "Error resampling source %s, removing source...", source
                         )
                         removed = self._resampler.remove_timeseries(source)
                         if not removed:
-                            logger.warning(
+                            _logger.warning(
                                 "Got an exception from an unknown source: "
                                 "source=%r, exception=%r",
                                 source,
                                 source_error,
                             )
                     # The resampling_task will be re-created if we reached this point
         finally:
```

### Comparing `frequenz-sdk-0.19.0/src/frequenz/sdk/actor/_run_utils.py` & `frequenz-sdk-0.20.0/src/frequenz/sdk/actor/_run_utils.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.19.0/src/frequenz/sdk/actor/power_distributing/__init__.py` & `frequenz-sdk-0.20.0/src/frequenz/sdk/actor/power_distributing/__init__.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.19.0/src/frequenz/sdk/actor/power_distributing/_battery_pool_status.py` & `frequenz-sdk-0.20.0/src/frequenz/sdk/actor/power_distributing/_battery_pool_status.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.19.0/src/frequenz/sdk/actor/power_distributing/_battery_status.py` & `frequenz-sdk-0.20.0/src/frequenz/sdk/actor/power_distributing/_battery_status.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,28 +2,29 @@
 # Copyright © 2022 Frequenz Energy-as-a-Service GmbH
 """Class to return battery status."""
 
 from __future__ import annotations
 
 import asyncio
 import logging
+import math
 from dataclasses import dataclass
 from datetime import datetime, timedelta, timezone
 from enum import Enum
 from typing import Iterable, Optional, Set, TypeVar, Union
 
 from frequenz.api.microgrid.battery_pb2 import ComponentState as BatteryComponentState
 from frequenz.api.microgrid.battery_pb2 import RelayState as BatteryRelayState
 from frequenz.api.microgrid.common_pb2 import ErrorLevel
 from frequenz.api.microgrid.inverter_pb2 import ComponentState as InverterComponentState
 from frequenz.channels import Receiver, Sender
 from frequenz.channels.util import Select, Timer
 
 from frequenz.sdk._internal.asyncio import cancel_and_await
-from frequenz.sdk.microgrid import get as get_microgrid
+from frequenz.sdk.microgrid import connection_manager
 from frequenz.sdk.microgrid.component import (
     BatteryData,
     ComponentCategory,
     ComponentData,
     InverterData,
 )
 
@@ -235,15 +236,15 @@
         New status is send only when it change.
 
         Args:
             status_sender: Channel to send status updates.
             set_power_result_receiver: Channel to receive results of the requests to the
                 components.
         """
-        api_client = get_microgrid().api_client
+        api_client = connection_manager.get().api_client
 
         battery_receiver = await api_client.battery_data(self._battery.component_id)
         inverter_receiver = await api_client.inverter_data(self._inverter.component_id)
 
         self._select = Select(
             battery=battery_receiver,
             battery_timer=self._battery.data_recv_timer,
@@ -265,14 +266,15 @@
 
     def _update_status(self, select: Select) -> Optional[Status]:
         if msg := select.battery:
             self._battery.last_msg_correct = (
                 self._is_message_reliable(msg.inner)
                 and self._is_battery_state_correct(msg.inner)
                 and self._no_critical_error(msg.inner)
+                and self._is_capacity_present(msg.inner)
             )
             self._battery.last_msg_timestamp = msg.inner.timestamp
             self._battery.data_recv_timer.reset()
 
         elif msg := select.inverter:
             self._inverter.last_msg_correct = (
                 self._is_message_reliable(msg.inner)
@@ -348,14 +350,34 @@
             self._blocking_status.unblock()
             return Status.WORKING
         if self._blocking_status.is_blocked():
             return Status.UNCERTAIN
 
         return Status.WORKING
 
+    def _is_capacity_present(self, msg: BatteryData) -> bool:
+        """Check whether the battery capacity is NaN or not.
+
+        If battery capacity is missing, then we can't work with it.
+
+        Args:
+            msg: battery message
+
+        Returns:
+            True if battery capacity is present, false otherwise.
+        """
+        if math.isnan(msg.capacity):
+            if self._last_status == Status.WORKING:
+                _logger.warning(
+                    "Battery %d capacity is NaN",
+                    msg.component_id,
+                )
+            return False
+        return True
+
     def _no_critical_error(self, msg: Union[BatteryData, InverterData]) -> bool:
         """Check if battery or inverter message has any critical error.
 
         Args:
             msg: message.
 
         Returns:
@@ -468,15 +490,15 @@
 
         Args:
             battery_id: battery id adjacent to the wanted inverter
 
         Returns:
             Id of the inverter. If battery hasn't adjacent inverter, then return None.
         """
-        graph = get_microgrid().component_graph
+        graph = connection_manager.get().component_graph
         return next(
             (
                 comp.component_id
                 for comp in graph.predecessors(battery_id)
                 if comp.category == ComponentCategory.INVERTER
             ),
             None,
```

### Comparing `frequenz-sdk-0.19.0/src/frequenz/sdk/actor/power_distributing/power_distributing.py` & `frequenz-sdk-0.20.0/src/frequenz/sdk/actor/power_distributing/power_distributing.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,18 +28,17 @@
     Tuple,
 )
 
 import grpc
 from frequenz.channels import Bidirectional, Peekable, Receiver, Sender
 from google.protobuf.empty_pb2 import Empty  # pylint: disable=no-name-in-module
 
-from ... import microgrid
 from ..._internal.asyncio import cancel_and_await
 from ...actor._decorator import actor
-from ...microgrid import ComponentGraph
+from ...microgrid import ComponentGraph, connection_manager
 from ...microgrid.client import MicrogridApiClient
 from ...microgrid.component import (
     BatteryData,
     Component,
     ComponentCategory,
     InverterData,
 )
@@ -62,22 +61,25 @@
     channel: Bidirectional.Handle[Result, Request]
     """The bidirectional channel to communicate with the user."""
 
 
 @actor
 class PowerDistributingActor:
     # pylint: disable=too-many-instance-attributes
-    """Tool to distribute power between batteries in microgrid.
+    """Actor to distribute the power between batteries in a microgrid.
 
-    The purpose of this tool is to keep equal SoC level in the batteries.
-    PowerDistributor can have many users. Each user should first register in order
-    to get its id, channel for sending request, and channel for receiving response.
+    The purpose of this tool is to keep an equal SoC level in all batteries.
+    The PowerDistributingActor can have many concurrent users which at this time
+    need to be known at construction time.
 
-    It is recommended to wait for PowerDistributor output with timeout. Otherwise if
-    the processing function fail then the response will never come.
+    For each user a bidirectional channel needs to be created through which
+    they can send and receive requests and responses.
+
+    It is recommended to wait for PowerDistributingActor output with timeout. Otherwise if
+    the processing function fails then the response will never come.
     The timeout should be Result:request_timeout_sec + time for processing the request.
 
     Edge cases:
     * If there are 2 requests to be processed for the same subset of batteries, then
     only the latest request will be processed. Older request will be ignored. User with
     older request will get response with Result.Status.IGNORED.
 
@@ -88,16 +90,16 @@
 
     Example:
         ``` python
         import grpc.aio as grpcaio
 
         from frequenz.sdk.microgrid.graph import _MicrogridComponentGraph
         from frequenz.sdk.microgrid.component import ComponentCategory
-        from frequenz.sdk.actor.power_distribution import (
-            PowerDistributor,
+        from frequenz.sdk.actor.power_distributing import (
+            PowerDistributingActor,
             Request,
             Result,
             Success,
             Error,
             PartialFailure,
             Ignored,
         )
@@ -110,15 +112,15 @@
         graph = _MicrogridComponentGraph()
         await graph.refresh_from_api(api)
 
         batteries = graph.components(component_category={ComponentCategory.BATTERY})
         batteries_ids = {c.component_id for c in batteries}
 
         channel = Bidirectional[Request, Result]("user1", "power_distributor")
-        power_distributor = PowerDistributor(
+        power_distributor = PowerDistributingActor(
             mock_api, component_graph, {"user1": channel.service_handle}
         )
 
         client_handle = channel.client_handle
 
         # Set power 1200W to given batteries.
         request = Request(power=1200, batteries=batteries_ids, request_timeout_sec=10.0)
@@ -161,22 +163,22 @@
         # NOTE: power_distributor_exponent should be received from ConfigManager
         self.power_distributor_exponent: float = 1.0
         self.distribution_algorithm = DistributionAlgorithm(
             self.power_distributor_exponent
         )
 
         self._bat_inv_map, self._inv_bat_map = self._get_components_pairs(
-            microgrid.get().component_graph
+            connection_manager.get().component_graph
         )
         self._battery_receivers: Dict[int, Peekable[BatteryData]] = {}
         self._inverter_receivers: Dict[int, Peekable[InverterData]] = {}
 
         # The components in different requests be for the same components, or for
         # completely different components. They should not overlap.
-        # Otherwise the PowerDistributor has no way to decide what request is more
+        # Otherwise the PowerDistributingActor has no way to decide what request is more
         # important. It will execute both. And later request will override the previous
         # one.
         # That is why the queue of maxsize = total number of batteries should be enough.
         self._request_queue: asyncio.Queue[Tuple[Request, _User]] = asyncio.Queue(
             maxsize=len(self._bat_inv_map)
         )
 
@@ -251,43 +253,43 @@
         `set_power` request with distributed power.
         The output of the `set_power` method is processed.
         Every battery and inverter that failed or didn't respond in time will be marked
         as broken for some time.
         """
         await self._create_channels()
 
-        api = microgrid.get().api_client
+        api = connection_manager.get().api_client
 
         # Wait few seconds to get data from the channels created above.
         await asyncio.sleep(self._wait_for_data_sec)
 
         self._started.set()
         while True:
             request, user = await self._request_queue.get()
 
             try:
                 pairs_data: List[InvBatPair] = self._get_components_data(
                     request.batteries
                 )
             except KeyError as err:
-                await user.channel.send(Error(request, str(err)))
+                await user.channel.send(Error(request=request, msg=str(err)))
                 continue
 
             if len(pairs_data) == 0:
                 error_msg = f"No data for the given batteries {str(request.batteries)}"
-                await user.channel.send(Error(request, str(error_msg)))
+                await user.channel.send(Error(request=request, msg=str(error_msg)))
                 continue
 
             try:
                 distribution = self.distribution_algorithm.distribute_power(
                     request.power, pairs_data
                 )
             except ValueError as err:
                 error_msg = f"Couldn't distribute power, error: {str(err)}"
-                await user.channel.send(Error(request, str(error_msg)))
+                await user.channel.send(Error(request=request, msg=str(error_msg)))
                 continue
 
             distributed_power_value = request.power - distribution.remaining_power
             battery_distribution = {
                 self._inv_bat_map[bat_id]: dist
                 for bat_id, dist in distribution.distribution.items()
             }
@@ -303,26 +305,26 @@
             )
 
             response: Success | PartialFailure
             if len(failed_batteries) > 0:
                 succeed_batteries = set(battery_distribution.keys()) - failed_batteries
                 response = PartialFailure(
                     request=request,
-                    succeed_power=distributed_power_value,
-                    succeed_batteries=succeed_batteries,
+                    succeeded_power=distributed_power_value,
+                    succeeded_batteries=succeed_batteries,
                     failed_power=failed_power,
                     failed_batteries=failed_batteries,
                     excess_power=distribution.remaining_power,
                 )
             else:
                 succeed_batteries = set(battery_distribution.keys())
                 response = Success(
                     request=request,
-                    succeed_power=distributed_power_value,
-                    used_batteries=succeed_batteries,
+                    succeeded_power=distributed_power_value,
+                    succeeded_batteries=succeed_batteries,
                     excess_power=distribution.remaining_power,
                 )
 
             asyncio.gather(
                 *[
                     self._all_battery_status.update_status(
                         succeed_batteries, failed_batteries
@@ -374,31 +376,31 @@
         """
         for battery in request.batteries:
             if battery not in self._battery_receivers:
                 msg = (
                     f"No battery {battery}, available batteries: "
                     f"{list(self._battery_receivers.keys())}"
                 )
-                return Error(request, msg)
+                return Error(request=request, msg=msg)
 
         if not request.adjust_power:
             if request.power < 0:
                 bound = self._get_lower_bound(request.batteries)
                 if request.power < bound:
-                    return OutOfBound(request, bound)
+                    return OutOfBound(request=request, bound=bound)
             else:
                 bound = self._get_upper_bound(request.batteries)
                 if request.power > bound:
-                    return OutOfBound(request, bound)
+                    return OutOfBound(request=request, bound=bound)
 
         return None
 
     def _remove_duplicated_requests(
         self, request: Request, user: _User
-    ) -> List[asyncio.Task[bool]]:
+    ) -> List[asyncio.Task[None]]:
         """Remove duplicated requests from the queue.
 
         Remove old requests in which set of batteries are the same as in new request.
         If batteries in new request overlap with batteries in old request but are not
         equal, then log error and process both messages.
 
         Args:
@@ -407,27 +409,27 @@
 
         Returns:
             Tasks with result sent to the users which requests were duplicated.
         """
         batteries = request.batteries
 
         good_requests: List[Tuple[Request, _User]] = []
-        to_ignore: List[asyncio.Task[bool]] = []
+        to_ignore: List[asyncio.Task[None]] = []
 
         while not self._request_queue.empty():
             prev_request, prev_user = self._request_queue.get_nowait()
             # Generators seems to be the fastest
             if prev_request.batteries == batteries:
                 task = asyncio.create_task(
-                    prev_user.channel.send(Ignored(prev_request))
+                    prev_user.channel.send(Ignored(request=prev_request))
                 )
                 to_ignore.append(task)
             # Use generators as generators seems to be the fastest.
             elif any(battery_id in prev_request.batteries for battery_id in batteries):
-                # If that happen PowerDistributor has no way to distinguish what
+                # If that happen PowerDistributingActor has no way to distinguish what
                 # request is more important. This should not happen
                 _logger.error(
                     "Batteries in two requests overlap! Actor: %s requested %s "
                     "and Actor: %s requested %s",
                     user.user_id,
                     str(request),
                     prev_user.user_id,
@@ -444,55 +446,55 @@
     async def _wait_for_request(self, user: _User) -> None:
         """Wait for the request from user.
 
         Check if request is correct. If request is not correct send ERROR response
         to the user. If request is correct, then add it to the main queue to be
         process.
 
-        If main queue has request for the same subset of batteries, then remove older
-        request, and send its user response with Result.Status.IGNORED.
+        Already existing requests for the same subset of batteries will be
+        removed and their users will be notified with a Result.Status.IGNORED response.
         Only new request will re processed.
-        If set of batteries are not the same but have common elements, then both
-        batteries will be processed.
+        If the sets of batteries are not the same but they have common elements,
+        then both batteries will be processed.
 
         Args:
             user: User that sends the requests.
         """
         while True:
             request: Optional[Request] = await user.channel.receive()
             if request is None:
                 _logger.info(
                     "Send channel for user %s was closed. User will be unregistered.",
                     user.user_id,
                 )
 
                 self._users_channels.pop(user.user_id)
                 if len(self._users_channels) == 0:
-                    _logger.error("No users in PowerDistributor!")
+                    _logger.error("No users in PowerDistributingActor!")
                 return
 
-            # Wait for PowerDistributor to start.
+            # Wait for PowerDistributingActor to start.
             if not self._started.is_set():
                 await self._started.wait()
 
             # We should discover as fast as possible that request is wrong.
-            check_result = self._check_request(request)
-            if check_result is not None:
-                await user.channel.send(check_result)
+            error = self._check_request(request)
+            if error is not None:
+                await user.channel.send(error)
                 continue
 
             tasks = self._remove_duplicated_requests(request, user)
             if self._request_queue.full():
                 q_size = (self._request_queue.qsize(),)
                 msg = (
                     f"Request queue is full {q_size}, can't process this request. "
                     "Consider increasing size of the queue."
                 )
                 _logger.error(msg)
-                await user.channel.send(Error(request, str(msg)))
+                await user.channel.send(Error(request=request, msg=str(msg)))
             else:
                 self._request_queue.put_nowait((request, user))
                 await asyncio.gather(*tasks)
 
     def _get_components_pairs(
         self, component_graph: ComponentGraph
     ) -> Tuple[Dict[int, int], Dict[int, int]]:
@@ -531,28 +533,47 @@
                 )
 
             bat_inv_map[battery.component_id] = inverters[0].component_id
             inv_bat_map[inverters[0].component_id] = battery.component_id
 
         return bat_inv_map, inv_bat_map
 
+    def _get_working_batteries(self, batteries: Set[int]) -> Set[int]:
+        """Get subset with working batteries.
+
+        If none of the given batteries are working, then treat all of them
+        as working.
+
+        Args:
+            batteries: requested batteries
+
+        Returns:
+            Subset with working batteries or input set if none of the given batteries
+                are working.
+        """
+        working_batteries = self._all_battery_status.get_working_batteries(batteries)
+        if len(working_batteries) == 0:
+            return batteries
+        return working_batteries
+
     def _get_components_data(self, batteries: Set[int]) -> List[InvBatPair]:
         """Get data for the given batteries and adjacent inverters.
 
         Args:
             batteries: Batteries that needs data.
 
         Raises:
             KeyError: If any battery in the given list doesn't exists in microgrid.
 
         Returns:
             Pairs of battery and adjacent inverter data.
         """
         pairs_data: List[InvBatPair] = []
-        working_batteries = self._all_battery_status.get_working_batteries(batteries)
+        working_batteries = self._get_working_batteries(batteries)
+
         for battery_id in working_batteries:
             if battery_id not in self._battery_receivers:
                 raise KeyError(
                     f"No battery {battery_id}, "
                     f"available batteries: {list(self._battery_receivers.keys())}"
                 )
 
@@ -585,15 +606,15 @@
 
         Args:
             battery_id: battery id
             inverter_id: inverter id
 
         Returns:
             Data for the battery and adjacent inverter without NaN values.
-            Return None if we could not replace NaN values.
+                Return None if we could not replace NaN values.
         """
         battery_data = self._battery_receivers[battery_id].peek()
         inverter_data = self._inverter_receivers[inverter_id].peek()
 
         # It means that nothing has been send on this channels, yet.
         # This should be handled by BatteryStatus. BatteryStatus should not return
         # this batteries as working.
@@ -651,44 +672,44 @@
         return InvBatPair(
             replace(battery_data, **battery_new_metrics),
             replace(inverter_data, **inverter_new_metrics),
         )
 
     async def _create_channels(self) -> None:
         """Create channels to get data of components in microgrid."""
-        api = microgrid.get().api_client
+        api = connection_manager.get().api_client
         for battery_id, inverter_id in self._bat_inv_map.items():
             bat_recv: Receiver[BatteryData] = await api.battery_data(battery_id)
             self._battery_receivers[battery_id] = bat_recv.into_peekable()
 
             inv_recv: Receiver[InverterData] = await api.inverter_data(inverter_id)
             self._inverter_receivers[inverter_id] = inv_recv.into_peekable()
 
     def _parse_result(
         self,
         # type comment to quiet pylint and mypy `unused-import` error
         tasks,  # type: Dict[int, asyncio.Task[Empty]]
         distribution: Dict[int, int],
         request_timeout_sec: float,
     ) -> Tuple[int, Set[int]]:
-        """Parse result of `set_power` requests.
+        """Parse the results of `set_power` requests.
 
-        Check if any task failed and why. If any task didn't success, then corresponding
-        battery is marked as broken.
+        Check if any task has failed and determine the reason for failure.
+        If any task did not succeed, then the corresponding battery is marked as broken.
 
         Args:
-            tasks: Dictionary where key is inverter id and value is task that set power
-                for this inverter. Each tasks should be finished or cancelled.
-            distribution: Dictionary where key is inverter id and value is how much
+            tasks: A dictionary where the key is the inverter ID and the value is the task that
+                set the power for this inverter. Each task should be finished or cancelled.
+            distribution: A dictionary where the key is the inverter ID and the value is how much
                 power was set to the corresponding inverter.
-            request_timeout_sec: timeout which has been used for request.
+            request_timeout_sec: The timeout that was used for the request.
 
         Returns:
-            Tuple where first element is total failed power, and the second element
-            set of batteries that failed.
+            A tuple where the first element is the total failed power, and the second element is
+            the set of batteries that failed.
         """
         failed_power: int = 0
         failed_batteries: Set[int] = set()
 
         for inverter_id, aws in tasks.items():
             battery_id = self._inv_bat_map[inverter_id]
             try:
```

### Comparing `frequenz-sdk-0.19.0/src/frequenz/sdk/config/_config.py` & `frequenz-sdk-0.20.0/src/frequenz/sdk/config/_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """Read and update config variables."""
 
 import logging
 from typing import Any, Dict, Optional, TypeVar
 
 from pydantic import ValidationError, parse_raw_as
 
-log = logging.getLogger(__name__)
+_logger = logging.getLogger(__name__)
 
 T = TypeVar("T")
 
 
 class Config:
     """
     Stores config variables.
```

### Comparing `frequenz-sdk-0.19.0/src/frequenz/sdk/microgrid/_graph.py` & `frequenz-sdk-0.20.0/src/frequenz/sdk/microgrid/_graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from typing import Callable, Iterable, List, Optional, Set
 
 import networkx as nx
 
 from .client import Connection, MicrogridApiClient
 from .component import Component, ComponentCategory
 
-logger = logging.getLogger(__name__)
+_logger = logging.getLogger(__name__)
 
 
 class InvalidGraphError(Exception):
     """Exception type that will be thrown if graph data is not valid."""
 
 
 class ComponentGraph(ABC):
@@ -305,15 +305,15 @@
         # from the new NetworkX graph data
         _provisional = _MicrogridComponentGraph()
         _provisional._graph = new_graph  # pylint: disable=protected-access
         if correct_errors is not None:
             try:
                 _provisional.validate()
             except InvalidGraphError as err:
-                logger.warning("Attempting to fix invalid component data: %s", err)
+                _logger.warning("Attempting to fix invalid component data: %s", err)
                 correct_errors(_provisional)
 
         try:
             _provisional.validate()
         except Exception as err:
             raise InvalidGraphError(
                 "Cannot populate component graph from provided input!"
```

### Comparing `frequenz-sdk-0.19.0/src/frequenz/sdk/microgrid/_microgrid.py` & `frequenz-sdk-0.20.0/src/frequenz/sdk/microgrid/connection_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -133,43 +133,43 @@
         self._api = MicrogridGrpcClient(grpc_channel, target)
         await self._graph.refresh_from_api(self._api)
 
     async def _initialize(self) -> None:
         await self._graph.refresh_from_api(self._api)
 
 
-_MICROGRID: Optional[ConnectionManager] = None
+_CONNECTION_MANAGER: Optional[ConnectionManager] = None
 
 
 async def initialize(host: str, port: int) -> None:
     """Initialize the MicrogridApi. This function should be called only once.
 
     Args:
         host: Microgrid host
         port: Microgrid port
 
     Raises:
         AssertionError: If method was called more then once.
     """
     # From Doc: pylint just try to discourage this usage.
     # That doesn't mean you cannot use it.
-    global _MICROGRID  # pylint: disable=global-statement
+    global _CONNECTION_MANAGER  # pylint: disable=global-statement
 
-    if _MICROGRID is not None:
+    if _CONNECTION_MANAGER is not None:
         raise AssertionError("MicrogridApi was already initialized.")
 
     microgrid_api = _InsecureConnectionManager(host, port)
     await microgrid_api._initialize()  # pylint: disable=protected-access
 
     # Check again that _MICROGRID_API is None in case somebody had the great idea of
     # calling initialize() twice and in parallel.
-    if _MICROGRID is not None:
+    if _CONNECTION_MANAGER is not None:
         raise AssertionError("MicrogridApi was already initialized.")
 
-    _MICROGRID = microgrid_api
+    _CONNECTION_MANAGER = microgrid_api
 
 
 def get() -> ConnectionManager:
     """Get the MicrogridApi instance created by initialize().
 
     This function should be only called after initialize().
 
@@ -178,14 +178,14 @@
             * If `initialize()` method was not called before this call.
             * If `initialize()` methods was called but was not awaited and instance was
                 not created yet.
 
     Returns:
         MicrogridApi instance.
     """
-    if _MICROGRID is None:
+    if _CONNECTION_MANAGER is None:
         raise RuntimeError(
-            "MicrogridApi is not initialized (or the initialization didn't "
-            "finished yet). Call and/or await for initialize() to finish."
+            "ConnectionManager is not initialized. "
+            "Call `await microgrid.initialize()` first."
         )
 
-    return _MICROGRID
+    return _CONNECTION_MANAGER
```

### Comparing `frequenz-sdk-0.19.0/src/frequenz/sdk/microgrid/client/_client.py` & `frequenz-sdk-0.20.0/src/frequenz/sdk/microgrid/client/_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     "_GenericComponentData",
     MeterData,
     BatteryData,
     InverterData,
     EVChargerData,
 )
 
-logger = logging.getLogger(__name__)
+_logger = logging.getLogger(__name__)
 
 
 class MicrogridApiClient(ABC):
     """Base interface for microgrid API clients to implement."""
 
     @abstractmethod
     async def components(self) -> Iterable[Component]:
@@ -337,45 +337,45 @@
             sender: A channel sender, to send the component data to.
 
         Raises:
             AioRpcError: if connection to Microgrid API cannot be established
         """
         retry_spec: RetryStrategy = self._retry_spec.copy()
         while True:
-            logger.debug(
+            _logger.debug(
                 "Making call to `GetComponentData`, for component_id=%d", component_id
             )
             try:
                 call = self.api.GetComponentData(
                     microgrid_pb.ComponentIdParam(id=component_id),
                 )
                 # grpc.aio is missing types and mypy thinks this is not
                 # async iterable, but it is
                 async for msg in call:  # type: ignore[attr-defined]
                     await sender.send(transform(msg))
             except grpc.aio.AioRpcError as err:
                 api_details = f"Microgrid API: {self.target}."
-                logger.exception(
+                _logger.exception(
                     "`GetComponentData`, for component_id=%d: exception: %s api: %s",
                     component_id,
                     err,
                     api_details,
                 )
 
             if interval := retry_spec.next_interval():
-                logger.warning(
+                _logger.warning(
                     "`GetComponentData`, for component_id=%d: connection ended, "
                     "retrying %s in %0.3f seconds.",
                     component_id,
                     retry_spec.get_progress(),
                     interval,
                 )
                 await asyncio.sleep(interval)
             else:
-                logger.warning(
+                _logger.warning(
                     "`GetComponentData`, for component_id=%d: connection ended, "
                     "retry limit exceeded %s.",
                     component_id,
                     retry_spec.get_progress(),
                 )
                 break
 
@@ -654,15 +654,15 @@
                     component_id=component_id,
                     # pylint: disable=no-member,line-too-long
                     target_metric=microgrid_pb.SetBoundsParam.TargetMetric.TARGET_METRIC_POWER_ACTIVE,
                     bounds=common_pb.Bounds(lower=lower, upper=upper),
                 ),
             )
         except grpc.aio.AioRpcError as err:
-            logger.error(
+            _logger.error(
                 "set_bounds write failed: %s, for message: %s, api: %s. Err: %s",
                 err,
                 next,
                 api_details,
                 err.details(),
             )
             raise
```

### Comparing `frequenz-sdk-0.19.0/src/frequenz/sdk/microgrid/client/_connection.py` & `frequenz-sdk-0.20.0/src/frequenz/sdk/microgrid/client/_connection.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.19.0/src/frequenz/sdk/microgrid/client/_retry.py` & `frequenz-sdk-0.20.0/src/frequenz/sdk/microgrid/client/_retry.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.19.0/src/frequenz/sdk/microgrid/component/__init__.py` & `frequenz-sdk-0.20.0/src/frequenz/sdk/microgrid/component/__init__.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.19.0/src/frequenz/sdk/microgrid/component/_component.py` & `frequenz-sdk-0.20.0/src/frequenz/sdk/microgrid/component/_component.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.19.0/src/frequenz/sdk/microgrid/component/_component_data.py` & `frequenz-sdk-0.20.0/src/frequenz/sdk/microgrid/component/_component_data.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.19.0/src/frequenz/sdk/microgrid/component/_component_states.py` & `frequenz-sdk-0.20.0/src/frequenz/sdk/microgrid/component/_component_states.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.19.0/src/frequenz/sdk/power/_distribution_algorithm.py` & `frequenz-sdk-0.20.0/src/frequenz/sdk/power/_distribution_algorithm.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_engine.py` & `frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_engine.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,24 +3,32 @@
 
 """A formula engine that can apply formulas on streaming data."""
 
 from __future__ import annotations
 
 import asyncio
 import logging
-import weakref
 from abc import ABC
 from collections import deque
 from datetime import datetime
 from math import isinf, isnan
-from typing import Dict, Generic, List, Optional, Set, Tuple, Type, TypeVar
-from uuid import UUID, uuid4
+from typing import (
+    Dict,
+    Generic,
+    List,
+    Optional,
+    Set,
+    Tuple,
+    Type,
+    TypeVar,
+    Union,
+    overload,
+)
 
 from frequenz.channels import Broadcast, Receiver
-from frequenz.channels._broadcast import Receiver as BroadcastReceiver
 
 from ..._internal.asyncio import cancel_and_await
 from .. import Sample, Sample3Phase
 from ._formula_steps import (
     Adder,
     Averager,
     Divider,
@@ -28,15 +36,15 @@
     MetricFetcher,
     Multiplier,
     OpenParen,
     Subtractor,
 )
 from ._tokenizer import TokenType
 
-logger = logging.Logger(__name__)
+_logger = logging.Logger(__name__)
 
 _operator_precedence = {
     "(": 0,
     "/": 1,
     "*": 2,
     "-": 3,
     "+": 4,
@@ -155,63 +163,160 @@
         res = eval_stack.pop()
         if isnan(res) or isinf(res):
             return Sample(metric_ts, None)
 
         return Sample(metric_ts, res)
 
 
-class FormulaEngine:
+_CompositionType = Union[
+    "FormulaEngine",
+    "HigherOrderFormulaBuilder",
+    "FormulaEngine3Phase",
+    "HigherOrderFormulaBuilder3Phase",
+]
+
+_CompositionType1Phase = Union[
+    "FormulaEngine",
+    "HigherOrderFormulaBuilder",
+]
+
+_CompositionType3Phase = Union[
+    "FormulaEngine3Phase",
+    "HigherOrderFormulaBuilder3Phase",
+]
+
+_GenericEngine = TypeVar("_GenericEngine", "FormulaEngine", "FormulaEngine3Phase")
+_GenericHigherOrderBuilder = TypeVar(
+    "_GenericHigherOrderBuilder",
+    "HigherOrderFormulaBuilder",
+    "HigherOrderFormulaBuilder3Phase",
+)
+
+
+class _ComposableFormulaEngine(
+    ABC, Generic[_GenericEngine, _GenericHigherOrderBuilder]
+):
+    """A base class for formula engines."""
+
+    _higher_order_builder: Type[_GenericHigherOrderBuilder]
+    _task: asyncio.Task[None] | None = None
+
+    async def _stop(self) -> None:
+        """Stop a running formula engine."""
+        if self._task is None:
+            return
+        await cancel_and_await(self._task)
+
+    def __add__(
+        self,
+        other: _GenericEngine | _GenericHigherOrderBuilder,
+    ) -> _GenericHigherOrderBuilder:
+        """Return a formula builder that adds (data in) `other` to `self`.
+
+        Args:
+            other: A formula receiver, or a formula builder instance corresponding to a
+                sub-expression.
+
+        Returns:
+            A formula builder that can take further expressions, or can be built
+                into a formula engine.
+        """
+        return self._higher_order_builder(self) + other  # type: ignore
+
+    def __sub__(
+        self, other: _GenericEngine | _GenericHigherOrderBuilder
+    ) -> _GenericHigherOrderBuilder:
+        """Return a formula builder that subtracts (data in) `other` from `self`.
+
+        Args:
+            other: A formula receiver, or a formula builder instance corresponding to a
+                sub-expression.
+
+        Returns:
+            A formula builder that can take further expressions, or can be built
+                into a formula engine.
+        """
+        return self._higher_order_builder(self) - other  # type: ignore
+
+    def __mul__(
+        self, other: _GenericEngine | _GenericHigherOrderBuilder
+    ) -> _GenericHigherOrderBuilder:
+        """Return a formula builder that multiplies (data in) `self` with `other`.
+
+        Args:
+            other: A formula receiver, or a formula builder instance corresponding to a
+                sub-expression.
+
+        Returns:
+            A formula builder that can take further expressions, or can be built
+                into a formula engine.
+        """
+        return self._higher_order_builder(self) * other  # type: ignore
+
+    def __truediv__(
+        self, other: _GenericEngine | _GenericHigherOrderBuilder
+    ) -> _GenericHigherOrderBuilder:
+        """Return a formula builder that divides (data in) `self` by `other`.
+
+        Args:
+            other: A formula receiver, or a formula builder instance corresponding to a
+                sub-expression.
+
+        Returns:
+            A formula builder that can take further expressions, or can be built
+                into a formula engine.
+        """
+        return self._higher_order_builder(self) / other  # type: ignore
+
+
+class FormulaEngine(
+    _ComposableFormulaEngine["FormulaEngine", "HigherOrderFormulaBuilder"]
+):
     """
     The FormulaEngine evaluates formulas and streams the results.
 
     Use the `FormulaBuilder` to create `FormulaEngine` instances.
     """
 
     def __init__(
         self,
-        name: str,
-        steps: List[FormulaStep],
-        metric_fetchers: Dict[str, MetricFetcher],
+        builder: FormulaBuilder,
     ) -> None:
         """Create a `FormulaEngine` instance.
 
         Args:
-            name: A name for the formula.
-            steps: Steps for the engine to execute, in post-fix order.
-            metric_fetchers: Fetchers for each metric stream the formula depends on.
+            builder: A `FormulaBuilder` instance to get the formula steps and metric
+                fetchers from.
         """
-        self._name: str = name
-        self._channel: FormulaChannel = FormulaChannel(self._name, self)
-        self._task: asyncio.Task[None] | None = None
-        self._evaluator = FormulaEvaluator(name, steps, metric_fetchers)
+        self._higher_order_builder = HigherOrderFormulaBuilder
+        self._name: str = builder.name
+        self._builder = builder
+        self._channel = Broadcast[Sample](self._name)
 
     async def _run(self) -> None:
+        await self._builder.subscribe()
+        steps, metric_fetchers = self._builder.finalize()
+        evaluator = FormulaEvaluator(self._name, steps, metric_fetchers)
         sender = self._channel.new_sender()
         while True:
             try:
-                msg = await self._evaluator.apply()
+                msg = await evaluator.apply()
             except asyncio.CancelledError:
-                logger.exception("FormulaEngine task cancelled: %s", self._name)
-                break
+                _logger.exception("FormulaEngine task cancelled: %s", self._name)
+                raise
             except Exception as err:  # pylint: disable=broad-except
-                logger.warning(
+                _logger.warning(
                     "Formula application failed: %s. Error: %s", self._name, err
                 )
             else:
                 await sender.send(msg)
 
-    async def _stop(self) -> None:
-        """Stop a running formula engine."""
-        if self._task is None:
-            return
-        await cancel_and_await(self._task)
-
     def new_receiver(
         self, name: Optional[str] = None, max_size: int = 50
-    ) -> FormulaReceiver:
+    ) -> Receiver[Sample]:
         """Create a new receiver that streams the output of the formula engine.
 
         Args:
             name: An optional name for the receiver.
             max_size: The size of the receiver's buffer.
 
         Returns:
@@ -219,67 +324,68 @@
         """
         if self._task is None:
             self._task = asyncio.create_task(self._run())
 
         return self._channel.new_receiver(name, max_size)
 
 
-class FormulaEngine3Phase:
+class FormulaEngine3Phase(
+    _ComposableFormulaEngine["FormulaEngine3Phase", "HigherOrderFormulaBuilder3Phase"]
+):
     """
     The FormulaEngine evaluates formulas and streams the results.
 
     Use the `FormulaBuilder` to create `FormulaEngine` instances.
     """
 
     def __init__(
         self,
         name: str,
-        phase_streams: Tuple[FormulaReceiver, FormulaReceiver, FormulaReceiver],
+        phase_streams: Tuple[FormulaEngine, FormulaEngine, FormulaEngine],
     ) -> None:
-        """Create a `FormulaEngine` instance.
+        """Create a `FormulaEngine3Phase` instance.
 
         Args:
             name: A name for the formula.
             phase_streams: output streams of formula engines running per-phase formulas.
         """
+        self._higher_order_builder = HigherOrderFormulaBuilder3Phase
         self._name: str = name
-        self._channel: FormulaChannel3Phase = FormulaChannel3Phase(self._name, self)
+        self._channel = Broadcast[Sample3Phase](self._name)
         self._task: asyncio.Task[None] | None = None
         self._streams: tuple[
-            FormulaReceiver, FormulaReceiver, FormulaReceiver
+            FormulaEngine, FormulaEngine, FormulaEngine
         ] = phase_streams
 
     async def _run(self) -> None:
         sender = self._channel.new_sender()
+        phase_1_rx = self._streams[0].new_receiver()
+        phase_2_rx = self._streams[1].new_receiver()
+        phase_3_rx = self._streams[2].new_receiver()
+
         while True:
             try:
-                phase_1 = await self._streams[0].receive()
-                phase_2 = await self._streams[1].receive()
-                phase_3 = await self._streams[2].receive()
+                phase_1 = await phase_1_rx.receive()
+                phase_2 = await phase_2_rx.receive()
+                phase_3 = await phase_3_rx.receive()
                 msg = Sample3Phase(
                     phase_1.timestamp,
                     phase_1.value,
                     phase_2.value,
                     phase_3.value,
                 )
             except asyncio.CancelledError:
-                logger.exception("FormulaEngine task cancelled: %s", self._name)
+                _logger.exception("FormulaEngine task cancelled: %s", self._name)
                 break
             else:
                 await sender.send(msg)
 
-    async def _stop(self) -> None:
-        """Stop a running formula engine."""
-        if self._task is None:
-            return
-        await cancel_and_await(self._task)
-
     def new_receiver(
         self, name: Optional[str] = None, max_size: int = 50
-    ) -> FormulaReceiver3Phase:
+    ) -> Receiver[Sample3Phase]:
         """Create a new receiver that streams the output of the formula engine.
 
         Args:
             name: An optional name for the receiver.
             max_size: The size of the receiver's buffer.
 
         Returns:
@@ -385,437 +491,258 @@
         for metric in metrics:
             fetcher = self._metric_fetchers.setdefault(
                 metric[0], MetricFetcher(*metric)
             )
             fetchers.append(fetcher)
         self._steps.append(Averager(fetchers))
 
-    def build(self) -> FormulaEngine:
-        """Finalize and build the formula engine.
-
-        Returns:
-            A `FormulaEngine` instance.
-        """
-        while self._build_stack:
-            self._steps.append(self._build_stack.pop())
-
-        return FormulaEngine(self._name, self._steps, self._metric_fetchers)
-
-
-_GenericSample = TypeVar("_GenericSample", Sample, Sample3Phase)
-_GenericEngine = TypeVar("_GenericEngine", FormulaEngine, FormulaEngine3Phase)
-_GenericFormulaChannel = TypeVar(
-    "_GenericFormulaChannel", "FormulaChannel", "FormulaChannel3Phase"
-)
-_GenericFormulaReceiver = TypeVar(
-    "_GenericFormulaReceiver", "FormulaReceiver", "FormulaReceiver3Phase"
-)
-_GenericHOFormulaBuilder = TypeVar(
-    "_GenericHOFormulaBuilder",
-    "HigherOrderFormulaBuilder",
-    "HigherOrderFormulaBuilder3Phase",
-)
-
-
-class _BaseFormulaChannel(
-    Generic[_GenericSample, _GenericEngine],
-    Broadcast[_GenericSample],
-    ABC,
-):
-    """A broadcast channel implementation for use with formulas."""
-
-    ReceiverType: Type[FormulaReceiver | FormulaReceiver3Phase]
-
-    def __init__(
-        self, name: str, engine: _GenericEngine, resend_latest: bool = False
-    ) -> None:
-        """Create a `FormulaChannel` instance.
-
-        Args:
-            name: A name for the channel.
-            engine: A FormulaEngine instance that produces values for this channel.
-            resend_latest: Whether to resend latest channel values to newly created
-                receivers, like in `Broadcast` channels.
-        """
-        self._engine: _GenericEngine = engine
-        super().__init__(name, resend_latest)
-
-    @property
-    def engine(self) -> _GenericEngine:
-        """Return the formula engine attached to the channel.
-
-        Returns:
-            A FormulaEngine instance.
-        """
-        return self._engine
-
-    def new_receiver(
-        self, name: Optional[str] = None, maxsize: int = 50
-    ) -> _GenericFormulaReceiver:
-        """Create a new FormulaReceiver for the channel.
-
-        This implementation is similar to `Broadcast.new_receiver()`, except that it
-        creates and returns a `FormulaReceiver`.  The way the default name for the
-        receiver is constructed, is also slightly tweaked.
-
-        Args:
-            name: An optional name for the receiver.
-            maxsize: size of the receiver's buffer.
-
-        Returns:
-            A `FormulaReceiver` instance attached to the `FormulaChannel`.
-        """
-        uuid = uuid4()
-        if name is None:
-            name = self.name
-        recv = self.ReceiverType(uuid, name, maxsize, self)
-        self.receivers[uuid] = weakref.ReferenceType(recv)
-        if self._resend_latest and self._latest is not None:
-            recv.enqueue(self._latest)
-        return recv
-
-
-class _BaseFormulaReceiver(
-    Generic[_GenericSample, _GenericEngine],
-    BroadcastReceiver[_GenericSample],
-    ABC,
-):
-    """A receiver to receive calculated `Sample`s from a Formula channel.
-
-    They function as regular channel receivers, but can be composed to form higher order
-    formulas.
-    """
-
-    BuilderType: Type[HigherOrderFormulaBuilder | HigherOrderFormulaBuilder3Phase]
-
-    def __init__(
-        self,
-        uuid: UUID,
-        name: str,
-        maxsize: int,
-        chan: _GenericFormulaChannel,
-    ) -> None:
-        """Create a `FormulaReceiver` instance.
-
-        Args:
-            uuid: uuid to uniquely identify the receiver.  Forwarded to
-                BroadcastReceiver's `__init__` function.
-            name: Name for the receiver.
-            maxsize: Buffer size for the receiver.
-            chan: The `FormulaChannel` instance that this receiver is attached to.
-        """
-        self._engine = chan.engine
-        super().__init__(uuid, name, maxsize, chan)
-
     @property
     def name(self) -> str:
-        """Name of the receiver.
+        """Return the name of the formula being built.
 
         Returns:
-            Name of the receiver.
+            The name of the formula being built.
         """
         return self._name
 
-    @property
-    def engine(self) -> _GenericEngine:
-        """Return the formula engine attached to the receiver.
-
-        Returns:
-            Formula Engine attached to the receiver.
-        """
-        return self._engine
-
-    # The use of `Self` is necessary for mypy to deduce the type of `clone` method in
-    # the derived classes.  With `from __future__ import annotations`, both CPython and
-    # mypy accept this in python <= 3.10.
-    #
-    # Unfortunately pylint doesn't accept `Self` before python 3.11, even with `from
-    # __future__ import annotations`. So the pylint `undefined-variable` check is
-    # disabled to get `Self` to pass the checks.
-    def clone(self) -> Self:  # pylint: disable=undefined-variable
-        """Create a new receiver from the formula engine.
+    async def subscribe(self) -> None:
+        """Subscribe to metrics if needed.
 
-        Returns:
-            New `FormulaReceiver` streaming a copy of the formula engine output.
-        """
-        return self._engine.new_receiver()
-
-    def __add__(
-        self,
-        other: _BaseFormulaReceiver | _GenericHOFormulaBuilder,
-    ) -> _GenericHOFormulaBuilder:
-        """Return a formula builder that adds (data in) `other` to `self`.
-
-        Args:
-            other: A formula receiver, or a formula builder instance corresponding to a
-                sub-expression.
-
-        Returns:
-            A formula builder that can take further expressions, or can be built
-                into a formula engine.
+        This is a no-op for the `FormulaBuilder` class, but is used by the
+        `ResampledFormulaBuilder` class.
         """
-        return self.BuilderType(self) + other
 
-    def __sub__(
-        self,
-        other: _BaseFormulaReceiver | _GenericHOFormulaBuilder,
-    ) -> _GenericHOFormulaBuilder:
-        """Return a formula builder that subtracts (data in) `other` from `self`.
-
-        Args:
-            other: A formula receiver, or a formula builder instance corresponding to a
-                sub-expression.
-
-        Returns:
-            A formula builder that can take further expressions, or can be built
-                into a formula engine.
-        """
-        return self.BuilderType(self) - other
-
-    def __mul__(
-        self, other: _BaseFormulaReceiver | _GenericHOFormulaBuilder
-    ) -> _GenericHOFormulaBuilder:
-        """Return a formula builder that multiplies (data in) `self` with `other`.
-
-        Args:
-            other: A formula receiver, or a formula builder instance corresponding to a
-                sub-expression.
+    def finalize(self) -> tuple[list[FormulaStep], dict[str, MetricFetcher]]:
+        """Finalize and return the steps and fetchers for the formula.
 
         Returns:
-            A formula builder that can take further expressions, or can be built
-                into a formula engine.
+            A tuple of the steps and fetchers for the formula.
         """
-        return self.BuilderType(self) * other
+        while self._build_stack:
+            self._steps.append(self._build_stack.pop())
 
-    def __truediv__(
-        self, other: _BaseFormulaReceiver | _GenericHOFormulaBuilder
-    ) -> _GenericHOFormulaBuilder:
-        """Return a formula builder that divides (data in) `self` by `other`.
+        return self._steps, self._metric_fetchers
 
-        Args:
-            other: A formula receiver, or a formula builder instance corresponding to a
-                sub-expression.
+    def build(self) -> FormulaEngine:
+        """Create a formula engine with the steps and fetchers that have been pushed.
 
         Returns:
-            A formula builder that can take further expressions, or can be built
-                into a formula engine.
+            A `FormulaEngine` instance.
         """
-        return self.BuilderType(self) / other
+        self.finalize()
+        return FormulaEngine(self)
 
 
-class _BaseHOFormulaBuilder(
-    ABC, Generic[_GenericFormulaReceiver, _GenericSample, _GenericEngine]
-):
+class _BaseHOFormulaBuilder(ABC):
     """Provides a way to build formulas from the outputs of other formulas."""
 
-    def __init__(self, recv: _GenericFormulaReceiver) -> None:
+    def __init__(self, engine: FormulaEngine | FormulaEngine3Phase) -> None:
         """Create a `GenericHigherOrderFormulaBuilder` instance.
 
         Args:
-            recv: A first input stream to create a builder with, so that python
+            engine: A first input stream to create a builder with, so that python
                 operators `+, -, *, /` can be used directly on newly created instances.
         """
-        self._steps: deque[tuple[TokenType, _GenericFormulaReceiver | str]] = deque()
-        self._steps.append((TokenType.COMPONENT_METRIC, recv.clone()))
-        recv._deactivate()  # pylint: disable=protected-access
-        self._engine = None
+        self._steps: deque[
+            tuple[TokenType, FormulaEngine | FormulaEngine3Phase | str]
+        ] = deque()
+        self._steps.append((TokenType.COMPONENT_METRIC, engine))
 
+    @overload
     def _push(
-        self,
-        oper: str,
-        other: _GenericFormulaReceiver | _GenericHOFormulaBuilder,
-    ) -> _GenericHOFormulaBuilder:
+        self, oper: str, other: _CompositionType1Phase
+    ) -> HigherOrderFormulaBuilder:
+        ...
+
+    @overload
+    def _push(
+        self, oper: str, other: _CompositionType3Phase
+    ) -> HigherOrderFormulaBuilder3Phase:
+        ...
+
+    def _push(
+        self, oper: str, other: _CompositionType
+    ) -> HigherOrderFormulaBuilder | HigherOrderFormulaBuilder3Phase:
         self._steps.appendleft((TokenType.OPER, "("))
         self._steps.append((TokenType.OPER, ")"))
         self._steps.append((TokenType.OPER, oper))
 
         # pylint: disable=protected-access
-        if isinstance(other, _BaseFormulaReceiver):
-            self._steps.append((TokenType.COMPONENT_METRIC, other.clone()))
-            other._deactivate()
+        if isinstance(other, (FormulaEngine, FormulaEngine3Phase)):
+            self._steps.append((TokenType.COMPONENT_METRIC, other))
         elif isinstance(other, _BaseHOFormulaBuilder):
             self._steps.append((TokenType.OPER, "("))
             self._steps.extend(other._steps)
             self._steps.append((TokenType.OPER, ")"))
         # pylint: enable=protected-access
         else:
             raise RuntimeError(f"Can't build a formula from: {other}")
-
+        assert isinstance(
+            self, (HigherOrderFormulaBuilder, HigherOrderFormulaBuilder3Phase)
+        )
         return self
 
+    @overload
+    def __add__(self, other: _CompositionType1Phase) -> HigherOrderFormulaBuilder:
+        ...
+
+    @overload
+    def __add__(self, other: _CompositionType3Phase) -> HigherOrderFormulaBuilder3Phase:
+        ...
+
     def __add__(
-        self, other: _GenericFormulaReceiver | _GenericHOFormulaBuilder
-    ) -> _GenericHOFormulaBuilder:
+        self, other: _CompositionType
+    ) -> HigherOrderFormulaBuilder | HigherOrderFormulaBuilder3Phase:
         """Return a formula builder that adds (data in) `other` to `self`.
 
         Args:
             other: A formula receiver, or a formula builder instance corresponding to a
                 sub-expression.
 
         Returns:
             A formula builder that can take further expressions, or can be built
                 into a formula engine.
         """
         return self._push("+", other)
 
+    @overload
+    def __sub__(self, other: _CompositionType1Phase) -> HigherOrderFormulaBuilder:
+        ...
+
+    @overload
+    def __sub__(self, other: _CompositionType3Phase) -> HigherOrderFormulaBuilder3Phase:
+        ...
+
     def __sub__(
-        self, other: _GenericFormulaReceiver | _GenericHOFormulaBuilder
-    ) -> _GenericHOFormulaBuilder:
+        self,
+        other: _CompositionType,
+    ) -> HigherOrderFormulaBuilder | HigherOrderFormulaBuilder3Phase:
         """Return a formula builder that subtracts (data in) `other` from `self`.
 
         Args:
             other: A formula receiver, or a formula builder instance corresponding to a
                 sub-expression.
 
         Returns:
             A formula builder that can take further expressions, or can be built
                 into a formula engine.
         """
         return self._push("-", other)
 
+    @overload
+    def __mul__(self, other: _CompositionType1Phase) -> HigherOrderFormulaBuilder:
+        ...
+
+    @overload
+    def __mul__(self, other: _CompositionType3Phase) -> HigherOrderFormulaBuilder3Phase:
+        ...
+
     def __mul__(
-        self, other: _GenericFormulaReceiver | _GenericHOFormulaBuilder
-    ) -> _GenericHOFormulaBuilder:
+        self,
+        other: _CompositionType,
+    ) -> HigherOrderFormulaBuilder | HigherOrderFormulaBuilder3Phase:
         """Return a formula builder that multiplies (data in) `self` with `other`.
 
         Args:
             other: A formula receiver, or a formula builder instance corresponding to a
                 sub-expression.
 
         Returns:
             A formula builder that can take further expressions, or can be built
                 into a formula engine.
         """
         return self._push("*", other)
 
+    @overload
+    def __truediv__(self, other: _CompositionType1Phase) -> HigherOrderFormulaBuilder:
+        ...
+
+    @overload
+    def __truediv__(
+        self, other: _CompositionType3Phase
+    ) -> HigherOrderFormulaBuilder3Phase:
+        ...
+
     def __truediv__(
-        self, other: _GenericFormulaReceiver | _GenericHOFormulaBuilder
-    ) -> _GenericHOFormulaBuilder:
+        self,
+        other: _CompositionType,
+    ) -> HigherOrderFormulaBuilder | HigherOrderFormulaBuilder3Phase:
         """Return a formula builder that divides (data in) `self` by `other`.
 
         Args:
             other: A formula receiver, or a formula builder instance corresponding to a
                 sub-expression.
 
         Returns:
             A formula builder that can take further expressions, or can be built
                 into a formula engine.
         """
         return self._push("/", other)
 
-    def new_receiver(
-        self, name: Optional[str] = None, max_size: int = 50
-    ) -> _GenericFormulaReceiver:
-        """Get a new receiver from the corresponding engine.
-
-        Args:
-            name: optional name for the receiver.
-            max_size: size of the receiver's buffer.
-
-        Returns:
-            A FormulaReceiver that streams formula output `Sample`s.
-
-        Raises:
-            RuntimeError: If `build` hasn't been called yet.
-        """
-        if self._engine is None:
-            raise RuntimeError(
-                "Please call `build()` first, before calls to `new_receiver()`"
-            )
-        return self._engine.new_receiver(name, max_size)
 
-
-class HigherOrderFormulaBuilder(
-    _BaseHOFormulaBuilder["FormulaReceiver", Sample, FormulaEngine]
-):
+class HigherOrderFormulaBuilder(_BaseHOFormulaBuilder):
     """A specialization of the _BaseHOFormulaBuilder for `FormulaReceiver`."""
 
     def build(self, name: str, nones_are_zeros: bool = False) -> FormulaEngine:
         """Build a `FormulaEngine` instance from the builder.
 
         Args:
             name: A name for the newly generated formula.
             nones_are_zeros: whether `None` values in any of the input streams should be
                 treated as zeros.
 
         Returns:
             A `FormulaEngine` instance.
         """
         builder = FormulaBuilder(name)
-        for step in self._steps:
-            if step[0] == TokenType.COMPONENT_METRIC:
-                assert isinstance(step[1], FormulaReceiver)
-                builder.push_metric(step[1].name, step[1], nones_are_zeros)
-            elif step[0] == TokenType.OPER:
-                assert isinstance(step[1], str)
-                builder.push_oper(step[1])
-        self._engine = builder.build()
-
-        return self._engine
+        for typ, value in self._steps:
+            if typ == TokenType.COMPONENT_METRIC:
+                assert isinstance(value, FormulaEngine)
+                builder.push_metric(
+                    value._name,  # pylint: disable=protected-access
+                    value.new_receiver(),
+                    nones_are_zeros,
+                )
+            elif typ == TokenType.OPER:
+                assert isinstance(value, str)
+                builder.push_oper(value)
+        return builder.build()
 
 
-class HigherOrderFormulaBuilder3Phase(
-    _BaseHOFormulaBuilder["FormulaReceiver3Phase", Sample3Phase, FormulaEngine3Phase]
-):
+class HigherOrderFormulaBuilder3Phase(_BaseHOFormulaBuilder):
     """A specialization of the _BaseHOFormulaBuilder for `FormulaReceiver3Phase`."""
 
     def build(self, name: str, nones_are_zeros: bool = False) -> FormulaEngine3Phase:
         """Build a `FormulaEngine3Phase` instance from the builder.
 
         Args:
             name: A name for the newly generated formula.
             nones_are_zeros: whether `None` values in any of the input streams should be
                 treated as zeros.
 
         Returns:
             A `FormulaEngine3Phase` instance.
         """
         builders = [FormulaBuilder(name), FormulaBuilder(name), FormulaBuilder(name)]
-        for step in self._steps:
-            if step[0] == TokenType.COMPONENT_METRIC:
-                assert isinstance(step[1], FormulaReceiver3Phase)
+        for typ, value in self._steps:
+            if typ == TokenType.COMPONENT_METRIC:
+                assert isinstance(value, FormulaEngine3Phase)
                 for phase in range(3):
                     builders[phase].push_metric(
-                        f"{step[1].name}-{phase+1}",
-                        step[1]  # pylint: disable=protected-access
-                        .engine._streams[phase]
-                        .clone(),
+                        f"{value._name}-{phase+1}",  # pylint: disable=protected-access
+                        value._streams[  # pylint: disable=protected-access
+                            phase
+                        ].new_receiver(),
                         nones_are_zeros,
                     )
-                step[1]._deactivate()  # pylint: disable=protected-access
-            elif step[0] == TokenType.OPER:
-                assert isinstance(step[1], str)
+            elif typ == TokenType.OPER:
+                assert isinstance(value, str)
                 for phase in range(3):
-                    builders[phase].push_oper(step[1])
-        self._engine = FormulaEngine3Phase(
+                    builders[phase].push_oper(value)
+        return FormulaEngine3Phase(
             name,
             (
-                builders[0].build().new_receiver(),
-                builders[1].build().new_receiver(),
-                builders[2].build().new_receiver(),
+                builders[0].build(),
+                builders[1].build(),
+                builders[2].build(),
             ),
         )
-        return self._engine
-
-
-class FormulaReceiver(_BaseFormulaReceiver[Sample, FormulaEngine]):
-    """A specialization of the _BaseFormulaChannel for `Sample` objects."""
-
-    BuilderType = HigherOrderFormulaBuilder
-
-
-class FormulaReceiver3Phase(_BaseFormulaReceiver[Sample3Phase, FormulaEngine3Phase]):
-    """A specialization of the _BaseFormulaChannel for `Sample3Phase` objects."""
-
-    BuilderType = HigherOrderFormulaBuilder3Phase
-
-
-class FormulaChannel(_BaseFormulaChannel[Sample, FormulaEngine]):
-    """A specialization of the _BaseFormulaChannel for `Sample` objects."""
-
-    ReceiverType = FormulaReceiver
-
-
-class FormulaChannel3Phase(_BaseFormulaChannel[Sample3Phase, FormulaEngine3Phase]):
-    """A specialization of the _BaseFormulaChannel for `Sample3Phase` objects."""
-
-    ReceiverType = FormulaReceiver3Phase
```

### Comparing `frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_engine_pool.py` & `frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_engine_pool.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,20 +15,15 @@
     FormulaGenerator,
     FormulaGeneratorConfig,
 )
 from ._resampled_formula_builder import ResampledFormulaBuilder
 
 if TYPE_CHECKING:
     # Break circular import by enclosing these type hints in a `TYPE_CHECKING` block.
-    from .._formula_engine import (
-        FormulaReceiver,
-        FormulaReceiver3Phase,
-        _GenericEngine,
-        _GenericFormulaReceiver,
-    )
+    from .._formula_engine import FormulaEngine, FormulaEngine3Phase
 
 
 class FormulaEnginePool:
     """Creates and owns formula engines from string formulas, or formula generators.
 
     If an engine already exists with a given name, it is reused instead.
     """
@@ -47,71 +42,71 @@
                 actor.
             resampler_subscription_sender: A sender for sending metric requests to the
                 resampling actor.
         """
         self._namespace = namespace
         self._channel_registry = channel_registry
         self._resampler_subscription_sender = resampler_subscription_sender
-        self._engines: dict[str, "FormulaReceiver|FormulaReceiver3Phase"] = {}
+        self._engines: dict[str, "FormulaEngine|FormulaEngine3Phase"] = {}
 
-    async def from_string(
+    def from_string(
         self,
         formula: str,
         component_metric_id: ComponentMetricId,
         nones_are_zeros: bool = False,
-    ) -> "FormulaReceiver":
+    ) -> FormulaEngine:
         """Get a receiver for a manual formula.
 
         Args:
             formula: formula to execute.
             component_metric_id: The metric ID to use when fetching receivers from the
                 resampling actor.
             nones_are_zeros: Whether to treat None values from the stream as 0s.  If
                 False, the returned value will be a None.
 
         Returns:
             A FormulaReceiver that streams values with the formulas applied.
         """
         channel_key = formula + component_metric_id.value
         if channel_key in self._engines:
-            return self._engines[channel_key].new_receiver()
+            return self._engines[channel_key]  # type: ignore
 
         builder = ResampledFormulaBuilder(
             self._namespace,
             formula,
             self._channel_registry,
             self._resampler_subscription_sender,
             component_metric_id,
         )
-        formula_engine = await builder.from_string(formula, nones_are_zeros)
+        formula_engine = builder.from_string(formula, nones_are_zeros)
         self._engines[channel_key] = formula_engine
 
-        return formula_engine.new_receiver()
+        return formula_engine
 
-    async def from_generator(
+    def from_generator(
         self,
         channel_key: str,
-        generator: "Type[FormulaGenerator[_GenericEngine]]",
+        generator: "Type[FormulaGenerator]",
         config: FormulaGeneratorConfig = FormulaGeneratorConfig(),
-    ) -> "_GenericFormulaReceiver":
+    ) -> FormulaEngine | FormulaEngine3Phase:
         """Get a receiver for a formula from a generator.
 
         Args:
             channel_key: A string to uniquely identify the formula.
             generator: A formula generator.
             config: config to initialize the formula generator with.
 
         Returns:
             A FormulaReceiver or a FormulaReceiver3Phase instance based on what the
                 FormulaGenerator returns.
         """
         if channel_key in self._engines:
-            return self._engines[channel_key].new_receiver()
+            return self._engines[channel_key]
 
-        engine = await generator(
+        engine = generator(
             self._namespace,
             self._channel_registry,
             self._resampler_subscription_sender,
             config,
         ).generate()
         self._engines[channel_key] = engine
-        return engine.new_receiver()
+        return engine
```

### Comparing `frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/__init__.py` & `frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/__init__.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_battery_power_formula.py` & `frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_battery_power_formula.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 # License: MIT
 # Copyright © 2022 Frequenz Energy-as-a-Service GmbH
 
 """Formula generator from component graph for Grid Power."""
 
 import logging
 
-from .....sdk import microgrid
-from ....microgrid.component import ComponentCategory, ComponentMetricId, InverterType
+from ....microgrid import connection_manager
+from ....microgrid.component import ComponentMetricId
 from ..._formula_engine import FormulaEngine
-from ._formula_generator import NON_EXISTING_COMPONENT_ID, FormulaGenerator
+from ._formula_generator import (
+    NON_EXISTING_COMPONENT_ID,
+    ComponentNotFound,
+    FormulaGenerator,
+)
 
-logger = logging.getLogger(__name__)
+_logger = logging.getLogger(__name__)
 
 
 class BatteryPowerFormula(FormulaGenerator):
     """Creates a formula engine from the component graph for calculating grid power."""
 
-    async def generate(
+    def generate(
         self,
     ) -> FormulaEngine:
         """Make a formula for the cumulative AC battery power of a microgrid.
 
         The calculation is performed by adding the Active Powers of all the inverters
         that are attached to batteries.
 
@@ -33,35 +37,39 @@
         Raises:
             ComponentNotFound: if there are no batteries in the component graph, or if
                 they don't have an inverter as a predecessor.
             FormulaGenerationError: If a battery has a non-inverter predecessor
                 in the component graph.
         """
         builder = self._get_builder("battery-power", ComponentMetricId.ACTIVE_POWER)
-        component_graph = microgrid.get().component_graph
-        battery_inverters = list(
-            comp
-            for comp in component_graph.components()
-            if comp.category == ComponentCategory.INVERTER
-            and comp.type == InverterType.BATTERY
-        )
-
-        if not battery_inverters:
-            logger.warning(
-                "Unable to find any battery inverters in the component graph. "
+        component_ids = self._config.component_ids
+        if not component_ids:
+            _logger.warning(
+                "No Battery component IDs specified. "
                 "Subscribing to the resampling actor with a non-existing "
                 "component id, so that `0` values are sent from the formula."
             )
-            # If there are no battery inverters, we have to send 0 values as the same
-            # frequency as the other streams.  So we subscribe with a non-existing
+            # If there are no Batteries, we have to send 0 values as the same
+            # frequency as the other streams. So we subscribe with a non-existing
             # component id, just to get a `None` message at the resampling interval.
-            await builder.push_component_metric(
+            builder.push_component_metric(
                 NON_EXISTING_COMPONENT_ID, nones_are_zeros=True
             )
             return builder.build()
 
+        component_graph = connection_manager.get().component_graph
+
+        battery_inverters = list(
+            next(iter(component_graph.predecessors(bat_id))) for bat_id in component_ids
+        )
+
+        if len(component_ids) != len(battery_inverters):
+            raise ComponentNotFound(
+                "Can't find inverters for all batteries from the component graph."
+            )
+
         for idx, comp in enumerate(battery_inverters):
             if idx > 0:
                 builder.push_oper("+")
-            await builder.push_component_metric(comp.component_id, nones_are_zeros=True)
+            builder.push_component_metric(comp.component_id, nones_are_zeros=True)
 
         return builder.build()
```

### Comparing `frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_ev_charger_current_formula.py` & `frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_ev_charger_current_formula.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,81 +2,82 @@
 # Copyright © 2022 Frequenz Energy-as-a-Service GmbH
 
 """Formula generator from component graph for 3-phase Grid Current."""
 
 from __future__ import annotations
 
 import logging
+from collections import abc
 
 from ....microgrid.component import ComponentMetricId
 from .._formula_engine import FormulaEngine, FormulaEngine3Phase
 from ._formula_generator import NON_EXISTING_COMPONENT_ID, FormulaGenerator
 
-logger = logging.getLogger(__name__)
+_logger = logging.getLogger(__name__)
 
 
 class EVChargerCurrentFormula(FormulaGenerator):
     """Create a formula engine from the component graph for calculating grid current."""
 
-    async def generate(self) -> FormulaEngine3Phase:
+    def generate(self) -> FormulaEngine3Phase:
         """Generate a formula for calculating total EV current for given component ids.
 
         Returns:
             A formula engine that calculates total 3-phase EV Charger current values.
         """
         component_ids = self._config.component_ids
 
         if not component_ids:
-            logger.warning(
+            _logger.warning(
                 "No EV Charger component IDs specified. "
                 "Subscribing to the resampling actor with a non-existing "
                 "component id, so that `0` values are sent from the formula."
             )
             # If there are no EV Chargers, we have to send 0 values as the same
             # frequency as the other streams.  So we subscribe with a non-existing
             # component id, just to get a `None` message at the resampling interval.
             builder = self._get_builder("ev-current", ComponentMetricId.ACTIVE_POWER)
-            await builder.push_component_metric(
+            builder.push_component_metric(
                 NON_EXISTING_COMPONENT_ID, nones_are_zeros=True
             )
             engine = builder.build()
             return FormulaEngine3Phase(
                 "ev-current",
-                (engine.new_receiver(), engine.new_receiver(), engine.new_receiver()),
+                (engine, engine, engine),
             )
 
         return FormulaEngine3Phase(
             "ev-current",
             (
                 (
-                    await self._gen_phase_formula(
+                    self._gen_phase_formula(
                         component_ids, ComponentMetricId.CURRENT_PHASE_1
                     )
-                ).new_receiver(),
+                ),
                 (
-                    await self._gen_phase_formula(
+                    self._gen_phase_formula(
                         component_ids, ComponentMetricId.CURRENT_PHASE_2
                     )
-                ).new_receiver(),
+                ),
                 (
-                    await self._gen_phase_formula(
+                    self._gen_phase_formula(
                         component_ids, ComponentMetricId.CURRENT_PHASE_3
                     )
-                ).new_receiver(),
+                ),
             ),
         )
 
-    async def _gen_phase_formula(
+    def _gen_phase_formula(
         self,
-        component_ids: set[int],
+        component_ids: abc.Set[int],
         metric_id: ComponentMetricId,
     ) -> FormulaEngine:
         builder = self._get_builder("ev-current", metric_id)
 
         # generate a formula that just adds values from all EV Chargers.
         for idx, component_id in enumerate(component_ids):
             if idx > 0:
                 builder.push_oper("+")
 
-            await builder.push_component_metric(component_id, nones_are_zeros=True)
+            builder.push_component_metric(component_id, nones_are_zeros=True)
 
         return builder.build()
```

### Comparing `frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_ev_charger_power_formula.py` & `frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_ev_charger_power_formula.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,43 +5,43 @@
 
 import logging
 
 from ....microgrid.component import ComponentMetricId
 from .._formula_engine import FormulaEngine
 from ._formula_generator import NON_EXISTING_COMPONENT_ID, FormulaGenerator
 
-logger = logging.getLogger(__name__)
+_logger = logging.getLogger(__name__)
 
 
 class EVChargerPowerFormula(FormulaGenerator):
     """Create a formula engine from the component graph for calculating grid power."""
 
-    async def generate(self) -> FormulaEngine:
+    def generate(self) -> FormulaEngine:
         """Generate a formula for calculating total EV power for given component ids.
 
         Returns:
             A formula engine that calculates total EV Charger power values.
         """
         builder = self._get_builder("ev-power", ComponentMetricId.ACTIVE_POWER)
 
         component_ids = self._config.component_ids
         if not component_ids:
-            logger.warning(
+            _logger.warning(
                 "No EV Charger component IDs specified. "
                 "Subscribing to the resampling actor with a non-existing "
                 "component id, so that `0` values are sent from the formula."
             )
             # If there are no EV Chargers, we have to send 0 values as the same
             # frequency as the other streams. So we subscribe with a non-existing
             # component id, just to get a `None` message at the resampling interval.
-            await builder.push_component_metric(
+            builder.push_component_metric(
                 NON_EXISTING_COMPONENT_ID, nones_are_zeros=True
             )
             return builder.build()
 
         for idx, component_id in enumerate(component_ids):
             if idx > 0:
                 builder.push_oper("+")
 
-            await builder.push_component_metric(component_id, nones_are_zeros=True)
+            builder.push_component_metric(component_id, nones_are_zeros=True)
 
         return builder.build()
```

### Comparing `frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_formula_generator.py` & `frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_formula_generator.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 
 """Base class for formula generators that use the component graphs."""
 
 from __future__ import annotations
 
 import sys
 from abc import ABC, abstractmethod
+from collections import abc
 from dataclasses import dataclass
-from typing import Generic
 
 from frequenz.channels import Sender
 
 from ....actor import ChannelRegistry, ComponentMetricRequest
 from ....microgrid.component import ComponentMetricId
-from .._formula_engine import _GenericEngine
+from .._formula_engine import FormulaEngine, FormulaEngine3Phase
 from .._resampled_formula_builder import ResampledFormulaBuilder
 
 
 class FormulaGenerationError(Exception):
     """An error encountered during formula generation from the component graph."""
 
 
@@ -29,18 +29,18 @@
 NON_EXISTING_COMPONENT_ID = sys.maxsize
 
 
 @dataclass(frozen=True)
 class FormulaGeneratorConfig:
     """Config for formula generators."""
 
-    component_ids: set[int] | None = None
+    component_ids: abc.Set[int] | None = None
 
 
-class FormulaGenerator(ABC, Generic[_GenericEngine]):
+class FormulaGenerator(ABC):
     """A class for generating formulas from the component graph."""
 
     def __init__(
         self,
         namespace: str,
         channel_registry: ChannelRegistry,
         resampler_subscription_sender: Sender[ComponentMetricRequest],
@@ -70,9 +70,9 @@
             self._channel_registry,
             self._resampler_subscription_sender,
             component_metric_id,
         )
         return builder
 
     @abstractmethod
-    async def generate(self) -> _GenericEngine:
+    def generate(self) -> FormulaEngine | FormulaEngine3Phase:
         """Generate a formula engine, based on the component graph."""
```

### Comparing `frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_grid_current_formula.py` & `frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_grid_current_formula.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # License: MIT
 # Copyright © 2022 Frequenz Energy-as-a-Service GmbH
 
 """Formula generator from component graph for 3-phase Grid Current."""
 
 from typing import Set
 
-from .....sdk import microgrid
+from ....microgrid import connection_manager
 from ....microgrid.component import Component, ComponentCategory, ComponentMetricId
 from .._formula_engine import FormulaEngine, FormulaEngine3Phase
 from ._formula_generator import ComponentNotFound, FormulaGenerator
 
 
 class GridCurrentFormula(FormulaGenerator):
     """Create a formula engine from the component graph for calculating grid current."""
 
-    async def generate(self) -> FormulaEngine3Phase:
+    def generate(self) -> FormulaEngine3Phase:
         """Generate a formula for calculating grid current from the component graph.
 
         Returns:
             A formula engine that will calculate 3-phase grid current values.
 
         Raises:
             ComponentNotFound: when the component graph doesn't have a `GRID` component.
         """
-        component_graph = microgrid.get().component_graph
+        component_graph = connection_manager.get().component_graph
         grid_component = next(
             (
                 comp
                 for comp in component_graph.components()
                 if comp.category == ComponentCategory.GRID
             ),
             None,
@@ -39,33 +39,27 @@
             )
 
         grid_successors = component_graph.successors(grid_component.component_id)
 
         return FormulaEngine3Phase(
             "grid-current",
             (
-                (
-                    await self._gen_phase_formula(
-                        grid_successors, ComponentMetricId.CURRENT_PHASE_1
-                    )
-                ).new_receiver(),
-                (
-                    await self._gen_phase_formula(
-                        grid_successors, ComponentMetricId.CURRENT_PHASE_2
-                    )
-                ).new_receiver(),
-                (
-                    await self._gen_phase_formula(
-                        grid_successors, ComponentMetricId.CURRENT_PHASE_3
-                    )
-                ).new_receiver(),
+                self._gen_phase_formula(
+                    grid_successors, ComponentMetricId.CURRENT_PHASE_1
+                ),
+                self._gen_phase_formula(
+                    grid_successors, ComponentMetricId.CURRENT_PHASE_2
+                ),
+                self._gen_phase_formula(
+                    grid_successors, ComponentMetricId.CURRENT_PHASE_3
+                ),
             ),
         )
 
-    async def _gen_phase_formula(
+    def _gen_phase_formula(
         self,
         grid_successors: Set[Component],
         metric_id: ComponentMetricId,
     ) -> FormulaEngine:
         builder = self._get_builder("grid-current", metric_id)
 
         # generate a formula that just adds values from all components that are
@@ -86,12 +80,12 @@
             ):
                 nones_are_zeros = True
             elif comp.category == ComponentCategory.METER:
                 nones_are_zeros = False
             else:
                 continue
 
-            await builder.push_component_metric(
+            builder.push_component_metric(
                 comp.component_id, nones_are_zeros=nones_are_zeros
             )
 
         return builder.build()
```

### Comparing `frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_grid_power_formula.py` & `frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_grid_power_formula.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # License: MIT
 # Copyright © 2022 Frequenz Energy-as-a-Service GmbH
 
 """Formula generator from component graph for Grid Power."""
 
-from .....sdk import microgrid
+from ....microgrid import connection_manager
 from ....microgrid.component import ComponentCategory, ComponentMetricId
 from .._formula_engine import FormulaEngine
 from ._formula_generator import ComponentNotFound, FormulaGenerator
 
 
 class GridPowerFormula(FormulaGenerator):
     """Creates a formula engine from the component graph for calculating grid power."""
 
-    async def generate(
+    def generate(
         self,
     ) -> FormulaEngine:
         """Generate a formula for calculating grid power from the component graph.
 
         Returns:
             A formula engine that will calculate grid power values.
 
         Raises:
             ComponentNotFound: when the component graph doesn't have a `GRID` component.
         """
         builder = self._get_builder("grid-power", ComponentMetricId.ACTIVE_POWER)
-        component_graph = microgrid.get().component_graph
+        component_graph = connection_manager.get().component_graph
         grid_component = next(
             (
                 comp
                 for comp in component_graph.components()
                 if comp.category == ComponentCategory.GRID
             ),
             None,
@@ -59,12 +59,12 @@
             ):
                 nones_are_zeros = True
             elif comp.category == ComponentCategory.METER:
                 nones_are_zeros = False
             else:
                 continue
 
-            await builder.push_component_metric(
+            builder.push_component_metric(
                 comp.component_id, nones_are_zeros=nones_are_zeros
             )
 
         return builder.build()
```

### Comparing `frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_pv_power_formula.py` & `frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_pv_power_formula.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,58 +1,58 @@
 # License: MIT
 # Copyright © 2022 Frequenz Energy-as-a-Service GmbH
 
 """Formula generator for PV Power, from the component graph."""
 
 import logging
 
-from .....sdk import microgrid
+from ....microgrid import connection_manager
 from ....microgrid.component import ComponentCategory, ComponentMetricId, InverterType
 from .._formula_engine import FormulaEngine
 from ._formula_generator import NON_EXISTING_COMPONENT_ID, FormulaGenerator
 
-logger = logging.getLogger(__name__)
+_logger = logging.getLogger(__name__)
 
 
 class PVPowerFormula(FormulaGenerator):
     """Creates a formula engine for calculating the PV power production."""
 
-    async def generate(self) -> FormulaEngine:
+    def generate(self) -> FormulaEngine:
         """Make a formula for the PV power production of a microgrid.
 
         Returns:
             A formula engine that will calculate PV power production values.
 
         Raises:
             ComponentNotFound: if there are no PV inverters in the component graph.
         """
         builder = self._get_builder("pv-power", ComponentMetricId.ACTIVE_POWER)
 
-        component_graph = microgrid.get().component_graph
+        component_graph = connection_manager.get().component_graph
         pv_inverters = list(
             comp
             for comp in component_graph.components()
             if comp.category == ComponentCategory.INVERTER
             and comp.type == InverterType.SOLAR
         )
 
         if not pv_inverters:
-            logger.warning(
+            _logger.warning(
                 "Unable to find any PV inverters in the component graph. "
                 "Subscribing to the resampling actor with a non-existing "
                 "component id, so that `0` values are sent from the formula."
             )
             # If there are no PV inverters, we have to send 0 values as the same
             # frequency as the other streams.  So we subscribe with a non-existing
             # component id, just to get a `None` message at the resampling interval.
-            await builder.push_component_metric(
+            builder.push_component_metric(
                 NON_EXISTING_COMPONENT_ID, nones_are_zeros=True
             )
             return builder.build()
 
         for idx, comp in enumerate(pv_inverters):
             if idx > 0:
                 builder.push_oper("+")
 
-            await builder.push_component_metric(comp.component_id, nones_are_zeros=True)
+            builder.push_component_metric(comp.component_id, nones_are_zeros=True)
 
         return builder.build()
```

### Comparing `frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_steps.py` & `frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_formula_steps.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/_formula_engine/_resampled_formula_builder.py` & `frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_resampled_formula_builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # License: MIT
 # Copyright © 2022 Frequenz Energy-as-a-Service GmbH
 
 """A builder for creating formula engines that operate on resampled component metrics."""
 
 
+from __future__ import annotations
+
 from frequenz.channels import Receiver, Sender
 
 from ...actor import ChannelRegistry, ComponentMetricRequest
 from ...microgrid.component import ComponentMetricId
 from .. import Sample
 from ._formula_engine import FormulaBuilder, FormulaEngine
 from ._tokenizer import Tokenizer, TokenType
@@ -36,46 +38,52 @@
                 resampling actor.
             metric_id: A metric ID to fetch for all components in this formula.
         """
         self._channel_registry = channel_registry
         self._resampler_subscription_sender = resampler_subscription_sender
         self._namespace = namespace
         self._metric_id = metric_id
+        self._resampler_requests: list[ComponentMetricRequest] = []
         super().__init__(formula_name)
 
-    async def _get_resampled_receiver(
+    def _get_resampled_receiver(
         self, component_id: int, metric_id: ComponentMetricId
     ) -> Receiver[Sample]:
         """Get a receiver with the resampled data for the given component id.
 
         Args:
             component_id: The component id for which to get a resampled data receiver.
             metric_id: A metric ID to fetch for all components in this formula.
 
         Returns:
             A receiver to stream resampled data for the given component id.
         """
         request = ComponentMetricRequest(self._namespace, component_id, metric_id, None)
-        await self._resampler_subscription_sender.send(request)
+        self._resampler_requests.append(request)
         return self._channel_registry.new_receiver(request.get_channel_name())
 
-    async def push_component_metric(
+    async def subscribe(self) -> None:
+        """Subscribe to all resampled component metric streams."""
+        for request in self._resampler_requests:
+            await self._resampler_subscription_sender.send(request)
+
+    def push_component_metric(
         self, component_id: int, *, nones_are_zeros: bool
     ) -> None:
         """Push a resampled component metric stream to the formula engine.
 
         Args:
             component_id: The component id for which to push a metric fetcher.
             nones_are_zeros: Whether to treat None values from the stream as 0s.  If
                 False, the returned value will be a None.
         """
-        receiver = await self._get_resampled_receiver(component_id, self._metric_id)
+        receiver = self._get_resampled_receiver(component_id, self._metric_id)
         self.push_metric(f"#{component_id}", receiver, nones_are_zeros)
 
-    async def from_string(
+    def from_string(
         self,
         formula: str,
         nones_are_zeros: bool,
     ) -> FormulaEngine:
         """Construct a `FormulaEngine` from the given formula string.
 
         Formulas can have Component IDs that are preceeded by a pound symbol("#"), and
@@ -95,15 +103,15 @@
         Raises:
             ValueError: when there is an unknown token type.
         """
         tokenizer = Tokenizer(formula)
 
         for token in tokenizer:
             if token.type == TokenType.COMPONENT_METRIC:
-                await self.push_component_metric(
+                self.push_component_metric(
                     int(token.value), nones_are_zeros=nones_are_zeros
                 )
             elif token.type == TokenType.OPER:
                 self.push_oper(token.value)
             else:
                 raise ValueError(f"Unknown token type: {token}")
```

### Comparing `frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/_formula_engine/_tokenizer.py` & `frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_formula_engine/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/_resampling.py` & `frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_resampling.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,18 +11,16 @@
 import math
 from bisect import bisect
 from collections import deque
 from dataclasses import dataclass
 from datetime import datetime, timedelta, timezone
 from typing import AsyncIterator, Callable, Coroutine, Optional, Sequence
 
-from frequenz.channels.util import Timer
-
 from .._internal.asyncio import cancel_and_await
-from . import Sample
+from ._base_types import UNIX_EPOCH, Sample
 
 _logger = logging.getLogger(__name__)
 
 
 DEFAULT_BUFFER_LEN_INIT = 16
 """Default initial buffer length.
 
@@ -74,18 +72,18 @@
 ResamplingFunction = Callable[
     [Sequence[Sample], "ResamplerConfig", "SourceProperties"], float
 ]
 """Resampling function type.
 
 A resampling function produces a new sample based on a list of pre-existing
 samples. It can do "upsampling" when there data rate of the `input_samples`
-period is smaller than the `resampling_period_s`, or "downsampling" if it is
+period is smaller than the `resampling_period`, or "downsampling" if it is
 bigger.
 
-In general a resampling window is the same as the `resampling_period_s`, and
+In general a resampling window is the same as the `resampling_period`, and
 this function might receive input samples from multiple windows in the past to
 enable extrapolation, but no samples from the future (so the timestamp of the
 new sample that is going to be produced will always be bigger than the biggest
 timestamp in the input data).
 
 Args:
     input_samples (Sequence[Sample]): The sequence of pre-existing samples.
@@ -121,41 +119,41 @@
     return sum(values) / len(values)
 
 
 @dataclass(frozen=True)
 class ResamplerConfig:
     """Resampler configuration."""
 
-    resampling_period_s: float
-    """The resampling period in seconds.
+    resampling_period: timedelta
+    """The resampling period.
 
     This is the time it passes between resampled data should be calculated.
 
-    It must be a positive number.
+    It must be a positive time span.
     """
 
     max_data_age_in_periods: float = 3.0
     """The maximum age a sample can have to be considered *relevant* for resampling.
 
-    Expressed in number of periods, where period is the `resampling_period_s`
+    Expressed in number of periods, where period is the `resampling_period`
     if we are downsampling (resampling period bigger than the input period) or
     the input sampling period if we are upsampling (input period bigger than
     the resampling period).
 
     It must be bigger than 1.0.
 
     Example:
-        If `resampling_period_s` is 3, the input sampling period is
+        If `resampling_period` is 3 seconds, the input sampling period is
         1 and `max_data_age_in_periods` is 2, then data older than 3*2
-        = 6 secods will be discarded when creating a new sample and never
+        = 6 seconds will be discarded when creating a new sample and never
         passed to the resampling function.
 
-        If `resampling_period_s` is 3, the input sampling period is
+        If `resampling_period` is 3 seconds, the input sampling period is
         5 and `max_data_age_in_periods` is 2, then data older than 5*2
-        = 10 secods will be discarded when creating a new sample and never
+        = 10 seconds will be discarded when creating a new sample and never
         passed to the resampling function.
     """
 
     resampling_function: ResamplingFunction = average
     """The resampling function.
 
     This function will be applied to the sequence of relevant samples at
@@ -173,15 +171,15 @@
     It must be at least 1 and at most `max_buffer_len`.
     """
 
     warn_buffer_len: int = DEFAULT_BUFFER_LEN_WARN
     """The minimum length of the resampling buffer that will emit a warning.
 
     If a buffer grows bigger than this value, it will emit a warning in the
-    logs, so buffers don't grow too big inadvertly.
+    logs, so buffers don't grow too big inadvertently.
 
     It must be at least 1 and at most `max_buffer_len`.
     """
 
     max_buffer_len: int = DEFAULT_BUFFER_LEN_MAX
     """The maximum length of the resampling buffer.
 
@@ -189,23 +187,34 @@
     needed to keep all the requested past sampling periods. An error will be
     emitted in the logs if the buffer length needs to be truncated to this
     value.
 
     It must be at bigger than `warn_buffer_len`.
     """
 
+    align_to: datetime | None = UNIX_EPOCH
+    """The time to align the resampling period to.
+
+    The resampling period will be aligned to this time, so the first resampled
+    sample will be at the first multiple of `resampling_period` starting from
+    `align_to`. It must be an aware datetime and can be in the future too.
+
+    If `align_to` is `None`, the resampling period will be aligned to the
+    time the resampler is created.
+    """
+
     def __post_init__(self) -> None:
         """Check that config values are valid.
 
         Raises:
             ValueError: If any value is out of range.
         """
-        if self.resampling_period_s < 0.0:
+        if self.resampling_period.total_seconds() < 0.0:
             raise ValueError(
-                f"resampling_period_s ({self.resampling_period_s}) must be positive"
+                f"resampling_period ({self.resampling_period}) must be positive"
             )
         if self.max_data_age_in_periods < 1.0:
             raise ValueError(
                 f"max_data_age_in_periods ({self.max_data_age_in_periods}) should be at least 1.0"
             )
         if self.warn_buffer_len < 1:
             raise ValueError(
@@ -229,29 +238,32 @@
             )
         if self.initial_buffer_len > self.warn_buffer_len:
             _logger.warning(
                 "initial_buffer_len (%s) is bigger than warn_buffer_len (%s)",
                 self.initial_buffer_len,
                 self.warn_buffer_len,
             )
+        if self.align_to is not None and self.align_to.tzinfo is None:
+            raise ValueError(
+                f"align_to ({self.align_to}) should be a timezone aware datetime"
+            )
 
 
 class SourceStoppedError(RuntimeError):
     """A timeseries stopped producing samples."""
 
     def __init__(self, source: Source) -> None:
         """Create an instance.
 
         Args:
-            source: The source of the timeseries that stopped producting
-                samples.
+            source: The source of the timeseries that stopped producing samples.
         """
         super().__init__(f"Timeseries stopped producing samples, source: {source}")
         self.source = source
-        """The source of the timeseries that stopped producting samples."""
+        """The source of the timeseries that stopped producing samples."""
 
     def __repr__(self) -> str:
         """Return the representation of the instance.
 
         Returns:
             The representation of the instance.
         """
@@ -310,19 +322,19 @@
 
     `None` means it didn't started yet.
     """
 
     received_samples: int = 0
     """Total samples received by this source so far."""
 
-    sampling_period_s: Optional[float] = None
-    """The sampling period of this source (in seconds).
+    sampling_period: Optional[timedelta] = None
+    """The sampling period of this source.
 
-    This is we receive (on average) one sample for this source every
-    `sampling_period_s` seconds.
+    This means we receive (on average) one sample for this source every
+    `sampling_period` time.
 
     `None` means it is unknown.
     """
 
 
 class Resampler:
     """A timeseries resampler.
@@ -347,27 +359,25 @@
         """
         self._config = config
         """The configuration for this resampler."""
 
         self._resamplers: dict[Source, _StreamingHelper] = {}
         """A mapping between sources and the streaming helper handling that source."""
 
-        self._timer: Timer = Timer(config.resampling_period_s)
-        """The timer to trigger the next resampling."""
-
-        self._window_end: datetime = datetime.now(timezone.utc) + timedelta(
-            seconds=self._config.resampling_period_s
-        )
+        self._window_end: datetime = self._calculate_window_end()
         """The time in which the current window ends.
 
         This is used to make sure every resampling window is generated at
         precise times. We can't rely on the timer timestamp because timers will
         never fire at the exact requested time, so if we don't use a precise
         time for the end of the window, the resampling windows we produce will
         have different sizes.
+
+        The window end will also be aligned to the `config.align_to` time, so
+        the window end is deterministic.
         """
 
     @property
     def config(self) -> ResamplerConfig:
         """Get the resampler configuration.
 
         Returns:
@@ -425,38 +435,14 @@
         """
         try:
             del self._resamplers[source]
         except KeyError:
             return False
         return True
 
-    async def _wait_for_next_resampling_period(self) -> None:
-        """Wait for next resampling period.
-
-        If resampling period already started, then return without sleeping.
-        That would allow us to catch up with resampling.
-        Print warning if function woke up to late.
-        """
-        now = datetime.now(tz=timezone.utc)
-        if self._window_end > now:
-            sleep_for = self._window_end - now
-            await asyncio.sleep(sleep_for.total_seconds())
-
-        timer_error_s = (now - self._window_end).total_seconds()
-        if timer_error_s > (self._config.resampling_period_s / 10.0):
-            _logger.warning(
-                "The resampling task woke up too late. Resampling should have started "
-                "at %s, but it started at %s (%s seconds difference; resampling "
-                "period is %s seconds)",
-                self._window_end,
-                now,
-                timer_error_s,
-                self._config.resampling_period_s,
-            )
-
     async def resample(self, *, one_shot: bool = False) -> None:
         """Start resampling all known timeseries.
 
         This method will run forever unless there is an error while receiving
         from a source or sending to a sink (or `one_shot` is used).
 
         Args:
@@ -475,36 +461,86 @@
             await self._wait_for_next_resampling_period()
 
             results = await asyncio.gather(
                 *[r.resample(self._window_end) for r in self._resamplers.values()],
                 return_exceptions=True,
             )
 
-            self._window_end = self._window_end + timedelta(
-                seconds=self._config.resampling_period_s
-            )
+            self._window_end = self._window_end + self._config.resampling_period
             exceptions = {
                 source: results[i]
                 for i, source in enumerate(self._resamplers)
                 # CancelledError inherits from BaseException, but we don't want
                 # to catch *all* BaseExceptions here.
                 if isinstance(results[i], (Exception, asyncio.CancelledError))
             }
             if exceptions:
                 raise ResamplingError(exceptions)
             if one_shot:
                 break
 
+    async def _wait_for_next_resampling_period(self) -> None:
+        """Wait for next resampling period.
+
+        If resampling period already started, then return without sleeping.
+        That would allow us to catch up with resampling.
+        Print warning if function woke up to late.
+        """
+        now = datetime.now(tz=timezone.utc)
+        if self._window_end > now:
+            sleep_for = self._window_end - now
+            await asyncio.sleep(sleep_for.total_seconds())
+
+        timer_error = now - self._window_end
+        # We use a tolerance of 10% of the resampling period
+        tolerance = timedelta(
+            seconds=self._config.resampling_period.total_seconds() / 10.0
+        )
+        if timer_error > tolerance:
+            _logger.warning(
+                "The resampling task woke up too late. Resampling should have "
+                "started at %s, but it started at %s (tolerance: %s, "
+                "difference: %s; resampling period: %s)",
+                self._window_end,
+                now,
+                tolerance,
+                timer_error,
+                self._config.resampling_period,
+            )
+
+    def _calculate_window_end(self) -> datetime:
+        """Calculate the end of the current resampling window.
+
+        The calculated resampling window end is a multiple of
+        `self._config.resampling_period` starting at `self._config.align_to`.
+
+        if `self._config.align_to` is `None`, the current time is used.
+
+        Returns:
+            The end of the current resampling window aligned to
+                `self._config.align_to`.
+        """
+        now = datetime.now(timezone.utc)
+        period = self._config.resampling_period
+        align_to = self._config.align_to
+
+        if align_to is None:
+            return now + period
+
+        elapsed = (now - align_to) % period
+
+        return now + period - elapsed
+
 
 class _ResamplingHelper:
     """Keeps track of *relevant* samples to pass them to the resampling function.
 
     Samples are stored in an internal ring buffer. All collected samples that
-    are newer than `max(resampling_period_s, input_period_s)
-    * max_data_age_in_periods` seconds are considered *relevant* and are passed
+    are newer than `max(resampling_period, input_period)
+    * max_data_age_in_periods` are considered *relevant* and are passed
     to the provided `resampling_function` when calling the `resample()` method.
     All older samples are discarded.
     """
 
     def __init__(self, name: str, config: ResamplerConfig) -> None:
         """Initialize an instance.
 
@@ -551,67 +587,69 @@
         ), "We need a maxlen of at least 1 to update the sample period"
 
         config = self._config
         props = self._source_properties
 
         # We only update it if we didn't before and we have enough data
         if (
-            props.sampling_period_s is not None
+            props.sampling_period is not None
             or props.sampling_start is None
             or props.received_samples
-            < config.resampling_period_s * config.max_data_age_in_periods
+            < config.resampling_period.total_seconds() * config.max_data_age_in_periods
             or len(self._buffer) < self._buffer.maxlen
             # There might be a race between the first sample being received and
             # this function being called
             or now <= props.sampling_start
         ):
             return False
 
         samples_time_delta = now - props.sampling_start
-        props.sampling_period_s = (
-            samples_time_delta.total_seconds()
-        ) / props.received_samples
+        props.sampling_period = timedelta(
+            seconds=samples_time_delta.total_seconds() / props.received_samples
+        )
 
         _logger.debug(
             "New input sampling period calculated for %r: %ss",
             self._name,
-            props.sampling_period_s,
+            props.sampling_period,
         )
         return True
 
     def _update_buffer_len(self) -> bool:
         """Update the length of the buffer based on the source properties.
 
         Returns:
             Whether the buffer length was changed (was really updated).
         """
-        input_sampling_period_s = self._source_properties.sampling_period_s
-
         # To make type checking happy
-        assert input_sampling_period_s is not None
         assert self._buffer.maxlen is not None
+        assert self._source_properties.sampling_period is not None
+
+        input_sampling_period = self._source_properties.sampling_period
 
         config = self._config
 
-        # If we are upsampling, one sample could be enough for back-filling, but
-        # we store max_data_age_in_periods for input periods, so resampling
-        # functions can do more complex inter/extrapolation if they need to.
-        if input_sampling_period_s > config.resampling_period_s:
-            new_buffer_len = input_sampling_period_s * config.max_data_age_in_periods
-        # If we are upsampling, we want a buffer that can hold
-        # max_data_age_in_periods * resampling_period_s seconds of data, and we
-        # one sample every input_sampling_period_s.
-        else:
-            new_buffer_len = (
-                config.resampling_period_s
-                / input_sampling_period_s
+        new_buffer_len = math.ceil(
+            # If we are upsampling, one sample could be enough for
+            # back-filling, but we store max_data_age_in_periods for input
+            # periods, so resampling functions can do more complex
+            # inter/extrapolation if they need to.
+            (input_sampling_period.total_seconds() * config.max_data_age_in_periods)
+            if input_sampling_period > config.resampling_period
+            # If we are downsampling, we want a buffer that can hold
+            # max_data_age_in_periods * resampling_period of data, and we one
+            # sample every input_sampling_period.
+            else (
+                config.resampling_period.total_seconds()
+                / input_sampling_period.total_seconds()
                 * config.max_data_age_in_periods
             )
+        )
 
-        new_buffer_len = max(1, math.ceil(new_buffer_len))
+        new_buffer_len = max(1, new_buffer_len)
         if new_buffer_len > config.max_buffer_len:
             _logger.error(
                 "The new buffer length (%s) for timeseries %s is too big, using %s instead",
                 new_buffer_len,
                 self._name,
                 config.max_buffer_len,
             )
@@ -654,29 +692,30 @@
 
         conf = self._config
         props = self._source_properties
 
         # To see which samples are relevant we need to consider if we are down
         # or upsampling.
         period = (
-            max(conf.resampling_period_s, props.sampling_period_s)
-            if props.sampling_period_s is not None
-            else conf.resampling_period_s
-        )
-        minimum_relevant_timestamp = timestamp - timedelta(
-            seconds=period * conf.max_data_age_in_periods
+            max(
+                conf.resampling_period,
+                props.sampling_period,
+            )
+            if props.sampling_period is not None
+            else conf.resampling_period
         )
+        minimum_relevant_timestamp = timestamp - period * conf.max_data_age_in_periods
 
         # We need to pass a dummy Sample to bisect because it only support
         # specifying a key extraction function in Python 3.10, so we need to
         # compare samples at the moment.
         min_index = bisect(self._buffer, Sample(minimum_relevant_timestamp, None))
         max_index = bisect(self._buffer, Sample(timestamp, None))
         # Using itertools for slicing doesn't look very efficient, but
-        # experiements with a custom (ring) buffer that can slice showed that
+        # experiments with a custom (ring) buffer that can slice showed that
         # it is not that bad. See:
         # https://github.com/frequenz-floss/frequenz-sdk-python/pull/130
         # So if we need more performance beyond this point, we probably need to
         # resort to some C (or similar) implementation.
         relevant_samples = list(itertools.islice(self._buffer, min_index, max_index))
         value = (
             conf.resampling_function(relevant_samples, conf, props)
```

### Comparing `frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/_ringbuffer.py` & `frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/_ringbuffer/buffer.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 """Ringbuffer implementation with focus on time & memory efficiency."""
 
 from __future__ import annotations
 
 from collections.abc import Iterable
 from copy import deepcopy
 from dataclasses import dataclass
-from datetime import datetime, timedelta
+from datetime import datetime, timedelta, timezone
 from typing import Generic, List, SupportsFloat, SupportsIndex, TypeVar, overload
 
 import numpy as np
 import numpy.typing as npt
 
-from . import Sample
+from .._base_types import UNIX_EPOCH, Sample
 
 FloatArray = TypeVar("FloatArray", List[float], npt.NDArray[np.float64])
 
 
 @dataclass
 class Gap:
     """A gap defines the range for which we haven't received values yet."""
@@ -42,44 +42,49 @@
 
         return False
 
 
 class OrderedRingBuffer(Generic[FloatArray]):
     """Time aware ringbuffer that keeps its entries sorted by time."""
 
+    _DATETIME_MIN = datetime.min.replace(tzinfo=timezone.utc)
+    _DATETIME_MAX = datetime.max.replace(tzinfo=timezone.utc)
+
     def __init__(
         self,
         buffer: FloatArray,
         sampling_period: timedelta,
-        time_index_alignment: datetime = datetime(1, 1, 1),
+        align_to: datetime = UNIX_EPOCH,
     ) -> None:
         """Initialize the time aware ringbuffer.
 
         Args:
             buffer: Instance of a buffer container to use internally.
             sampling_period: Timedelta of the desired sampling period.
-            time_index_alignment: Arbitrary point in time used to align
+            align_to: Arbitrary point in time used to align
                 timestamped data with the index position in the buffer.
                 Used to make the data stored in the buffer align with the
                 beginning and end of the buffer borders.
 
-                For example, if the `time_index_alignment` is set to
+                For example, if the `align_to` is set to
                 "0001-01-01 12:00:00", and the `sampling_period` is set to
                 1 hour and the length of the buffer is 24, then the data
                 stored in the buffer could correspond to the time range from
                 "2022-01-01 12:00:00" to "2022-01-02 12:00:00" (date chosen
                 arbitrarily here).
         """
+        assert len(buffer) > 0, "The buffer capacity must be higher than zero"
+
         self._buffer: FloatArray = buffer
         self._sampling_period: timedelta = sampling_period
-        self._time_index_alignment: datetime = time_index_alignment
+        self._time_index_alignment: datetime = align_to
 
         self._gaps: list[Gap] = []
-        self._datetime_newest: datetime = datetime.min
-        self._datetime_oldest: datetime = datetime.max
+        self._datetime_newest: datetime = self._DATETIME_MIN
+        self._datetime_oldest: datetime = self._DATETIME_MAX
         self._time_range: timedelta = (len(self._buffer) - 1) * sampling_period
 
     @property
     def sampling_period(self) -> timedelta:
         """Return the sampling period of the ring buffer.
 
         Returns:
@@ -124,15 +129,18 @@
         Raises:
             IndexError: When the timestamp to be added is too old.
         """
         # adjust timestamp to be exactly on the sample period time point
         timestamp = self._normalize_timestamp(sample.timestamp)
 
         # Don't add outdated entries
-        if timestamp < self._datetime_oldest and self._datetime_oldest != datetime.max:
+        if (
+            timestamp < self._datetime_oldest
+            and self._datetime_oldest != self._DATETIME_MAX
+        ):
             raise IndexError(
                 f"Timestamp {timestamp} too old (cut-off is at {self._datetime_oldest})."
             )
 
         # Update timestamps
         prev_newest = self._datetime_newest
         self._datetime_newest = max(self._datetime_newest, timestamp)
@@ -188,15 +196,15 @@
 
         Will return a copy in the following cases:
         * The requested time period is crossing the start/end of the buffer.
         * The requested time period contains missing entries.
         * The force_copy parameter was set to True (default False).
 
         The first case can be avoided by using the appropriate
-        time_index_alignment value in the constructor so that the data lines up
+        `align_to` value in the constructor so that the data lines up
         with the start/end of the buffer.
 
         This means, if the caller needs to modify the data to account for
         missing entries, they can safely do so.
 
         Args:
             start: start time of the window.
@@ -479,16 +487,17 @@
 
     def __len__(self) -> int:
         """Return the amount of items that this container currently holds.
 
         Returns:
             The length.
         """
-        if self._datetime_newest == datetime.min:
+        if self._datetime_newest == self._DATETIME_MIN:
             return 0
 
         start_index = self.datetime_to_index(self._datetime_oldest)
         end_index = self.datetime_to_index(self._datetime_newest)
 
         if end_index < start_index:
-            return len(self._buffer) - start_index + end_index
-        return start_index - end_index
+            return len(self._buffer) - start_index + end_index + 1
+
+        return end_index + 1 - start_index
```

### Comparing `frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/battery_pool/_component_metric_fetcher.py` & `frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/battery_pool/_component_metric_fetcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 from ..._internal._constants import MAX_BATTERY_DATA_AGE_SEC
 from ..._internal.asyncio import AsyncConstructible
 from ...actor._data_sourcing.microgrid_api_source import (
     _BatteryDataMethods,
     _InverterDataMethods,
 )
-from ...microgrid import get as get_microgrid
+from ...microgrid import connection_manager
 from ...microgrid.component import (
     BatteryData,
     ComponentCategory,
     ComponentData,
     ComponentMetricId,
     InverterData,
 )
@@ -205,15 +205,15 @@
 
         Size of the receiver buffer should should be 1 to make sure we receive only
         the latest component data.
 
         Returns:
             Receiver for this component metrics.
         """
-        api = get_microgrid().api_client
+        api = connection_manager.get().api_client
         return await api.battery_data(self._component_id, maxsize=1)
 
     def _component_category(self) -> ComponentCategory:
         return ComponentCategory.BATTERY
 
 
 class LatestInverterMetricsFetcher(LatestMetricsFetcher[InverterData]):
@@ -256,12 +256,12 @@
 
         Size of the receiver buffer should should be 1 to make sure we receive only
         the latest component data.
 
         Returns:
             Receiver for this component metrics.
         """
-        api = get_microgrid().api_client
+        api = connection_manager.get().api_client
         return await api.inverter_data(self._component_id, maxsize=1)
 
     def _component_category(self) -> ComponentCategory:
         return ComponentCategory.INVERTER
```

### Comparing `frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/battery_pool/_component_metrics.py` & `frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/battery_pool/_component_metrics.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/battery_pool/_methods.py` & `frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/battery_pool/_methods.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/battery_pool/_metric_calculator.py` & `frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/battery_pool/_metric_calculator.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import logging
 from abc import ABC, abstractmethod
 from collections.abc import Mapping, Set
 from datetime import datetime, timezone
 from typing import Generic, Iterable, TypeVar
 
-from ... import microgrid
+from ...microgrid import connection_manager
 from ...microgrid.component import ComponentCategory, ComponentMetricId, InverterType
 from ._component_metrics import ComponentMetricsData
 from ._result_types import Bound, CapacityMetrics, PowerMetrics, SoCMetrics
 
 _logger = logging.getLogger(__name__)
 _MIN_TIMESTAMP = datetime.min.replace(tzinfo=timezone.utc)
 
@@ -24,15 +24,15 @@
 
     Args:
         batteries: Set of batteries
 
     Returns:
         Mapping between battery and adjacent inverter.
     """
-    graph = microgrid.get().component_graph
+    graph = connection_manager.get().component_graph
     bat_inv_map: dict[int, int] = {}
     for battery_id in batteries:
         try:
             predecessors = graph.predecessors(battery_id)
         except KeyError as err:
             # If battery_id is not in the component graph, then print error and ignore
             # this id. Wrong component id might be bug in config file. We won't stop
```

### Comparing `frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/battery_pool/_result_types.py` & `frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/battery_pool/_result_types.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/battery_pool/battery_pool.py` & `frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/battery_pool/battery_pool.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,46 +2,59 @@
 # Copyright © 2023 Frequenz Energy-as-a-Service GmbH
 
 """User interface for requesting aggregated battery-inverter data."""
 
 from __future__ import annotations
 
 import asyncio
+import uuid
 from collections.abc import Set
 from datetime import timedelta
 from typing import Any
 
-from frequenz.channels import Receiver
+from frequenz.channels import Receiver, Sender
 
-from ... import microgrid
 from ..._internal._constants import RECEIVER_MAX_SIZE
 from ..._internal.asyncio import cancel_and_await
+from ...actor import ChannelRegistry, ComponentMetricRequest
 from ...actor.power_distributing._battery_pool_status import BatteryStatus
+from ...microgrid import connection_manager
 from ...microgrid.component import ComponentCategory
+from .._formula_engine import FormulaEngine, FormulaEnginePool
+from .._formula_engine._formula_generators import (
+    BatteryPowerFormula,
+    FormulaGeneratorConfig,
+)
 from ._methods import AggregateMethod, SendOnUpdate
 from ._metric_calculator import CapacityCalculator, PowerBoundsCalculator, SoCCalculator
 from ._result_types import CapacityMetrics, PowerMetrics, SoCMetrics
 
 
 class BatteryPool:
     """Calculate high level metrics for a pool of the batteries.
 
     BatterPool accepts subset of the battery ids and provides methods methods for
     fetching high level metrics for this subset.
     """
 
-    def __init__(
+    def __init__(  # pylint: disable=too-many-arguments
         self,
+        channel_registry: ChannelRegistry,
+        resampler_subscription_sender: Sender[ComponentMetricRequest],
         batteries_status_receiver: Receiver[BatteryStatus],
         min_update_interval: timedelta,
         batteries_id: Set[int] | None = None,
     ) -> None:
         """Create the class instance.
 
         Args:
+            channel_registry: A channel registry instance shared with the resampling
+                actor.
+            resampler_subscription_sender: A sender for sending metric requests to the
+                resampling actor.
             batteries_status_receiver: Receiver to receive status of the batteries.
                 Receivers should has maxsize = 1 to fetch only the latest status.
                 Battery status channel should has resend_latest = True.
                 It should send information when any battery changed status.
                 Battery status should include status of the inverter adjacent to this
                 battery.
             min_update_interval: Some metrics in BatteryPool are send only when they
@@ -60,30 +73,58 @@
         if batteries_id:
             self._batteries: Set[int] = batteries_id
         else:
             self._batteries = self._get_all_batteries()
 
         self._working_batteries: set[int] = set()
 
-        self._update_battery_status_task = asyncio.create_task(
-            self._update_battery_status(batteries_status_receiver)
-        )
+        if self._batteries:
+            self._update_battery_status_task = asyncio.create_task(
+                self._update_battery_status(batteries_status_receiver)
+            )
 
         self._min_update_interval = min_update_interval
         self._active_methods: dict[str, AggregateMethod[Any]] = {}
 
+        self._namespace: str = f"battery-pool-{self._batteries}-{uuid.uuid4()}"
+        self._formula_pool: FormulaEnginePool = FormulaEnginePool(
+            self._namespace,
+            channel_registry,
+            resampler_subscription_sender,
+        )
+
     @property
     def battery_ids(self) -> Set[int]:
         """Return ids of the batteries in the pool.
 
         Returns:
             Ids of the batteries in the pool
         """
         return self._batteries
 
+    @property
+    def power(self) -> FormulaEngine:
+        """Fetch the total power of the batteries in the pool.
+
+        If a formula engine to calculate this metric is not already running, it will be
+        started.
+
+        A receiver from the formula engine can be obtained by calling the `new_receiver`
+        method.
+
+        Returns:
+            A FormulaEngine that will calculate and stream the total power of all
+                batteries in the pool.
+        """
+        return self._formula_pool.from_generator(
+            "battery_pool_power",
+            BatteryPowerFormula,
+            FormulaGeneratorConfig(component_ids=self._batteries),
+        )  # type: ignore[return-value]
+
     async def soc(
         self, maxsize: int | None = RECEIVER_MAX_SIZE
     ) -> Receiver[SoCMetrics | None]:
         """Get receiver to receive new soc metrics when they change.
 
         Soc formulas are described in the receiver return type.
         None will be send if there is no component to calculate metric.
@@ -170,15 +211,15 @@
 
     def _get_all_batteries(self) -> Set[int]:
         """Get all batteries from the microgrid.
 
         Returns:
             All batteries in the microgrid.
         """
-        graph = microgrid.get().component_graph
+        graph = connection_manager.get().component_graph
         return {
             battery.component_id
             for battery in graph.components(
                 component_category={ComponentCategory.BATTERY}
             )
         }
```

### Comparing `frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/ev_charger_pool/_state_tracker.py` & `frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/ev_charger_pool/_state_tracker.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,20 +2,18 @@
 # Copyright © 2023 Frequenz Energy-as-a-Service GmbH
 
 """State tracking for EV Charger pools."""
 
 from __future__ import annotations
 
 import asyncio
-from collections.abc import Iterator
-from dataclasses import dataclass
 from enum import Enum
 from typing import Optional
 
-from frequenz.channels import Broadcast, Receiver
+from frequenz.channels import Receiver
 from frequenz.channels.util import Merge
 
 from frequenz.sdk import microgrid
 from frequenz.sdk._internal.asyncio import cancel_and_await
 
 from ...microgrid.component import (
     EVChargerCableState,
@@ -24,14 +22,16 @@
 )
 
 
 class EVChargerState(Enum):
     """State of individual ev charger."""
 
     UNSPECIFIED = "UNSPECIFIED"
+    MISSING = "MISSING"
+
     IDLE = "IDLE"
     EV_PLUGGED = "EV_PLUGGED"
     EV_LOCKED = "EV_LOCKED"
     ERROR = "ERROR"
 
     @classmethod
     def from_ev_charger_data(cls, data: EVChargerData) -> EVChargerState:
@@ -39,140 +39,89 @@
 
         Args:
             data: ev charger data coming from microgrid.
 
         Returns:
             An `EVChargerState` instance.
         """
+        if data.component_state == EVChargerComponentState.UNSPECIFIED:
+            return EVChargerState.UNSPECIFIED
         if data.component_state in (
             EVChargerComponentState.AUTHORIZATION_REJECTED,
             EVChargerComponentState.ERROR,
         ):
             return EVChargerState.ERROR
+
+        if data.cable_state == EVChargerCableState.UNSPECIFIED:
+            return EVChargerState.UNSPECIFIED
         if data.cable_state == EVChargerCableState.EV_LOCKED:
             return EVChargerState.EV_LOCKED
         if data.cable_state == EVChargerCableState.EV_PLUGGED:
             return EVChargerState.EV_PLUGGED
         return EVChargerState.IDLE
 
-
-@dataclass(frozen=True)
-class EVChargerPoolStates:
-    """States of all EV Chargers in the pool."""
-
-    _states: dict[int, EVChargerState]
-    _changed_component: Optional[int] = None
-
-    def __iter__(self) -> Iterator[tuple[int, EVChargerState]]:
-        """Iterate over states of all EV Chargers.
+    def is_ev_connected(self) -> bool:
+        """Check whether an EV is connected to the charger.
 
         Returns:
-            An iterator over all EV Charger states.
+            Whether an EV is connected to the charger.
         """
-        return iter(self._states.items())
-
-    def latest_change(self) -> Optional[tuple[int, EVChargerState]]:
-        """Return the most recent EV Charger state change.
-
-        The first `EVChargerPoolStates` instance created by a `StateTracker` will just
-        be a representation of the states of all EV Chargers.  At that point, the most
-        recent change in state of an ev charger will be unknown, so this function will
-        return `None`.
-
-        Returns:
-            None, when the most recent change is unknown.  Otherwise, a tuple with
-                the component ID of an EV Charger that just had a state change, and its
-                new state.
-        """
-        if self._changed_component is None:
-            return None
-        return (
-            self._changed_component,
-            self._states.setdefault(
-                self._changed_component, EVChargerState.UNSPECIFIED
-            ),
-        )
+        return self in (EVChargerState.EV_PLUGGED, EVChargerState.EV_LOCKED)
 
 
 class StateTracker:
     """A class for keeping track of the states of all EV Chargers in a pool."""
 
     def __init__(self, component_ids: set[int]) -> None:
         """Create a `_StateTracker` instance.
 
         Args:
             component_ids: EV Charger component ids to track the states of.
         """
         self._component_ids = component_ids
-        self._channel = Broadcast[EVChargerPoolStates](
-            "EVCharger States", resend_latest=True
-        )
-        self._task: Optional[asyncio.Task[None]] = None
+        self._task: asyncio.Task[None] = asyncio.create_task(self._run())
         self._merged_stream: Optional[Merge[EVChargerData]] = None
-        self._states: dict[int, EVChargerState] = {}
 
-    def _get(self) -> EVChargerPoolStates:
-        """Get a representation of the current states of all EV Chargers.
+        # Initialize all components to the `MISSING` state.  This will change as data
+        # starts arriving from the individual components.
+        self._states: dict[int, EVChargerState] = {
+            component_id: EVChargerState.MISSING for component_id in component_ids
+        }
+
+    def get(self, component_id: int) -> EVChargerState:
+        """Return the current state of the EV Charger with the given component ID.
+
+        Args:
+            component_id: id of the EV Charger whose state is being fetched.
 
         Returns:
-            An `EVChargerPoolStates` instance.
+            An `EVChargerState` value corresponding to the given component id.
         """
-        return EVChargerPoolStates(self._states)
+        return self._states[component_id]
 
     def _update(
         self,
         data: EVChargerData,
-    ) -> Optional[EVChargerPoolStates]:
+    ) -> None:
         """Update the state of an EV Charger, from a new data point.
 
         Args:
             data: component data from the microgrid, for an EV Charger in the pool.
-
-        Returns:
-            A new `EVChargerPoolStates` instance representing all the EV Chargers in
-                the pool, in case there has been a state change for any of the EV
-                Chargers, or `None` otherwise.
         """
         evc_id = data.component_id
         new_state = EVChargerState.from_ev_charger_data(data)
-        if evc_id not in self._states or self._states[evc_id] != new_state:
-            self._states[evc_id] = new_state
-            return EVChargerPoolStates(self._states, evc_id)
-        return None
+        self._states[evc_id] = new_state
 
     async def _run(self) -> None:
-        api_client = microgrid.get().api_client
+        api_client = microgrid.connection_manager.get().api_client
         streams: list[Receiver[EVChargerData]] = await asyncio.gather(
             *[api_client.ev_charger_data(cid) for cid in self._component_ids]
         )
-
-        latest_messages: list[EVChargerData] = await asyncio.gather(
-            *[stream.receive() for stream in streams]
-        )
-        self._states = {
-            msg.component_id: EVChargerState.from_ev_charger_data(msg)
-            for msg in latest_messages
-        }
         self._merged_stream = Merge(*streams)
-        sender = self._channel.new_sender()
-        await sender.send(self._get())
         async for data in self._merged_stream:
-            if updated_states := self._update(data):
-                await sender.send(updated_states)
-
-    def new_receiver(self) -> Receiver[EVChargerPoolStates]:
-        """Return a receiver that streams ev charger states.
-
-        Returns:
-            A receiver that streams the states of all EV Chargers in the pool, every
-                time the states of any of them change.
-        """
-        if self._task is None or self._task.done():
-            self._task = asyncio.create_task(self._run())
-        return self._channel.new_receiver()
+            self._update(data)
 
     async def stop(self) -> None:
         """Stop the status tracker."""
-        if self._task:
-            await cancel_and_await(self._task)
+        await cancel_and_await(self._task)
         if self._merged_stream:
             await self._merged_stream.stop()
```

### Comparing `frequenz-sdk-0.19.0/src/frequenz/sdk/timeseries/logical_meter/_logical_meter.py` & `frequenz-sdk-0.20.0/src/frequenz/sdk/timeseries/logical_meter/_logical_meter.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,23 +9,22 @@
 import uuid
 
 from frequenz.channels import Sender
 
 from ...actor import ChannelRegistry, ComponentMetricRequest
 from ...microgrid import ComponentGraph
 from ...microgrid.component import ComponentMetricId
-from .._formula_engine import FormulaEnginePool, FormulaReceiver, FormulaReceiver3Phase
+from .._formula_engine import FormulaEngine, FormulaEngine3Phase, FormulaEnginePool
 from .._formula_engine._formula_generators import (
-    BatteryPowerFormula,
     GridCurrentFormula,
     GridPowerFormula,
     PVPowerFormula,
 )
 
-logger = logging.getLogger(__name__)
+_logger = logging.getLogger(__name__)
 
 
 class LogicalMeter:
     """A logical meter for calculating high level metrics in a microgrid.
 
     LogicalMeter provides methods for fetching power values from different points in the
     microgrid.  These methods return `FormulaReceiver` objects, which can be used like
@@ -108,20 +107,20 @@
         self._component_graph = component_graph
         self._formula_pool = FormulaEnginePool(
             self._namespace,
             self._channel_registry,
             self._resampler_subscription_sender,
         )
 
-    async def start_formula(
+    def start_formula(
         self,
         formula: str,
         component_metric_id: ComponentMetricId,
         nones_are_zeros: bool = False,
-    ) -> FormulaReceiver:
+    ) -> FormulaEngine:
         """Start execution of the given formula.
 
         Formulas can have Component IDs that are preceeded by a pound symbol("#"), and
         these operators: +, -, *, /, (, ).
 
         For example, the input string: "#20 + #5" is a formula for adding metrics from
         two components with ids 20 and 5.
@@ -130,68 +129,66 @@
             formula: formula to execute.
             component_metric_id: The metric ID to use when fetching receivers from the
                 resampling actor.
             nones_are_zeros: Whether to treat None values from the stream as 0s.  If
                 False, the returned value will be a None.
 
         Returns:
-            A FormulaReceiver that streams values with the formulas applied.
+            A FormulaEngine that applies the formula and streams values.
         """
-        return await self._formula_pool.from_string(
+        return self._formula_pool.from_string(
             formula, component_metric_id, nones_are_zeros
         )
 
-    async def grid_power(self) -> FormulaReceiver:
+    @property
+    def grid_power(self) -> FormulaEngine:
         """Fetch the grid power for the microgrid.
 
         If a formula engine to calculate grid power is not already running, it will be
-        started.  Else, it will return a new receiver to the already existing data
-        stream.
+        started.
 
-        Returns:
-            A *new* receiver that will stream grid_power values.
+        A receiver from the formula engine can be created using the `new_receiver`
+        method.
 
+        Returns:
+            A FormulaEngine that will calculate and stream grid power.
         """
-        return await self._formula_pool.from_generator("grid_power", GridPowerFormula)
+        return self._formula_pool.from_generator(
+            "grid_power",
+            GridPowerFormula,
+        )  # type: ignore[return-value]
 
-    async def grid_current(self) -> FormulaReceiver3Phase:
+    @property
+    def grid_current(self) -> FormulaEngine3Phase:
         """Fetch the grid power for the microgrid.
 
         If a formula engine to calculate grid current is not already running, it will be
-        started.  Else, it will return a new receiver to the already existing data
-        stream.
-
-        Returns:
-            A *new* receiver that will stream grid_current values.
-
-        """
-        return await self._formula_pool.from_generator(
-            "grid_current", GridCurrentFormula
-        )
-
-    async def battery_power(self) -> FormulaReceiver:
-        """Fetch the cumulative battery power in the microgrid.
+        started.
 
-        If a formula engine to calculate cumulative battery power is not already
-        running, it will be started.  Else, it will return a new receiver to the already
-        existing data stream.
+        A receiver from the formula engine can be created using the `new_receiver`
+        method.
 
         Returns:
-            A *new* receiver that will stream battery_power values.
-
+            A FormulaEngine that will calculate and stream grid current.
         """
-        return await self._formula_pool.from_generator(
-            "battery_power", BatteryPowerFormula
-        )
+        return self._formula_pool.from_generator(
+            "grid_current",
+            GridCurrentFormula,
+        )  # type: ignore[return-value]
 
-    async def pv_power(self) -> FormulaReceiver:
+    @property
+    def pv_power(self) -> FormulaEngine:
         """Fetch the PV power production in the microgrid.
 
         If a formula engine to calculate PV power production is not already running, it
-        will be started.  Else, it will return a new receiver to the already existing
-        data stream.
+        will be started.
 
-        Returns:
-            A *new* receiver that will stream PV power production values.
+        A receiver from the formula engine can be created using the `new_receiver`
+        method.
 
+        Returns:
+            A FormulaEngine that will calculate and stream PV power production.
         """
-        return await self._formula_pool.from_generator("pv_power", PVPowerFormula)
+        return self._formula_pool.from_generator(
+            "pv_power",
+            PVPowerFormula,
+        )  # type: ignore[return-value]
```

### Comparing `frequenz-sdk-0.19.0/src/frequenz_sdk.egg-info/PKG-INFO` & `frequenz-sdk-0.20.0/src/frequenz_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequenz-sdk
-Version: 0.19.0
+Version: 0.20.0
 Summary: Frequenz Python SDK
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-sdk-python/releases
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-sdk-python
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-sdk-python/issues
 Project-URL: Support, https://github.com/frequenz-floss/frequenz-sdk-python/discussions/categories/support
```

### Comparing `frequenz-sdk-0.19.0/src/frequenz_sdk.egg-info/SOURCES.txt` & `frequenz-sdk-0.20.0/src/frequenz_sdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -35,32 +35,31 @@
 src/frequenz/sdk/actor/power_distributing/_battery_status.py
 src/frequenz/sdk/actor/power_distributing/power_distributing.py
 src/frequenz/sdk/actor/power_distributing/request.py
 src/frequenz/sdk/actor/power_distributing/result.py
 src/frequenz/sdk/config/__init__.py
 src/frequenz/sdk/config/_config.py
 src/frequenz/sdk/microgrid/__init__.py
+src/frequenz/sdk/microgrid/_data_pipeline.py
 src/frequenz/sdk/microgrid/_graph.py
-src/frequenz/sdk/microgrid/_microgrid.py
+src/frequenz/sdk/microgrid/connection_manager.py
 src/frequenz/sdk/microgrid/client/__init__.py
 src/frequenz/sdk/microgrid/client/_client.py
 src/frequenz/sdk/microgrid/client/_connection.py
 src/frequenz/sdk/microgrid/client/_retry.py
 src/frequenz/sdk/microgrid/component/__init__.py
 src/frequenz/sdk/microgrid/component/_component.py
 src/frequenz/sdk/microgrid/component/_component_data.py
 src/frequenz/sdk/microgrid/component/_component_states.py
 src/frequenz/sdk/power/__init__.py
 src/frequenz/sdk/power/_distribution_algorithm.py
 src/frequenz/sdk/timeseries/__init__.py
 src/frequenz/sdk/timeseries/_base_types.py
 src/frequenz/sdk/timeseries/_moving_window.py
 src/frequenz/sdk/timeseries/_resampling.py
-src/frequenz/sdk/timeseries/_ringbuffer.py
-src/frequenz/sdk/timeseries/_serializable_ringbuffer.py
 src/frequenz/sdk/timeseries/_formula_engine/__init__.py
 src/frequenz/sdk/timeseries/_formula_engine/_exceptions.py
 src/frequenz/sdk/timeseries/_formula_engine/_formula_engine.py
 src/frequenz/sdk/timeseries/_formula_engine/_formula_engine_pool.py
 src/frequenz/sdk/timeseries/_formula_engine/_formula_steps.py
 src/frequenz/sdk/timeseries/_formula_engine/_resampled_formula_builder.py
 src/frequenz/sdk/timeseries/_formula_engine/_tokenizer.py
@@ -68,23 +67,27 @@
 src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_battery_power_formula.py
 src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_ev_charger_current_formula.py
 src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_ev_charger_power_formula.py
 src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_formula_generator.py
 src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_grid_current_formula.py
 src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_grid_power_formula.py
 src/frequenz/sdk/timeseries/_formula_engine/_formula_generators/_pv_power_formula.py
+src/frequenz/sdk/timeseries/_ringbuffer/__init__.py
+src/frequenz/sdk/timeseries/_ringbuffer/buffer.py
+src/frequenz/sdk/timeseries/_ringbuffer/serialization.py
 src/frequenz/sdk/timeseries/battery_pool/__init__.py
 src/frequenz/sdk/timeseries/battery_pool/_component_metric_fetcher.py
 src/frequenz/sdk/timeseries/battery_pool/_component_metrics.py
 src/frequenz/sdk/timeseries/battery_pool/_methods.py
 src/frequenz/sdk/timeseries/battery_pool/_metric_calculator.py
 src/frequenz/sdk/timeseries/battery_pool/_result_types.py
 src/frequenz/sdk/timeseries/battery_pool/battery_pool.py
 src/frequenz/sdk/timeseries/ev_charger_pool/__init__.py
 src/frequenz/sdk/timeseries/ev_charger_pool/_ev_charger_pool.py
+src/frequenz/sdk/timeseries/ev_charger_pool/_set_current_bounds.py
 src/frequenz/sdk/timeseries/ev_charger_pool/_state_tracker.py
 src/frequenz/sdk/timeseries/logical_meter/__init__.py
 src/frequenz/sdk/timeseries/logical_meter/_logical_meter.py
 src/frequenz_sdk.egg-info/PKG-INFO
 src/frequenz_sdk.egg-info/SOURCES.txt
 src/frequenz_sdk.egg-info/dependency_links.txt
 src/frequenz_sdk.egg-info/requires.txt
```

