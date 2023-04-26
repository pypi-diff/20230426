# Comparing `tmp/droughty-0.9.7.tar.gz` & `tmp/droughty-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "droughty-0.9.7.tar", max compression
+gzip compressed data, was "droughty-0.9.8.tar", max compression
```

## Comparing `droughty-0.9.7.tar` & `droughty-0.9.8.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0     1283 2023-02-13 12:40:42.477103 droughty-0.9.7/README.md
--rw-r--r--   0        0        0    13158 2023-02-13 12:40:42.495288 droughty-0.9.7/droughty/.ipynb_checkpoints/Untitled-Copy1-checkpoint.ipynb
--rw-r--r--   0        0        0       72 2023-02-13 12:40:42.495352 droughty-0.9.7/droughty/.ipynb_checkpoints/Untitled-checkpoint.ipynb
--rw-r--r--   0        0        0       72 2023-02-13 12:40:42.495414 droughty-0.9.7/droughty/.ipynb_checkpoints/Untitled1-checkpoint.ipynb
--rw-r--r--   0        0        0        7 2023-02-13 12:40:42.495467 droughty-0.9.7/droughty/.python-version
--rw-r--r--   0        0        0      133 2023-02-13 12:40:42.495538 droughty-0.9.7/droughty/__init__.py
--rw-r--r--   0        0        0       70 2023-02-13 12:40:42.498067 droughty-0.9.7/droughty/cube_parser/__main__.py
--rw-r--r--   0        0        0     3348 2023-02-13 12:40:42.498220 droughty-0.9.7/droughty/cube_parser/__pycache__/cube.cpython-38.pyc
--rw-r--r--   0        0        0     2214 2023-02-13 12:40:42.498303 droughty-0.9.7/droughty/cube_parser/__pycache__/keys.cpython-38.pyc
--rw-r--r--   0        0        0     6884 2023-02-13 12:40:42.498395 droughty-0.9.7/droughty/cube_parser/__pycache__/lexer.cpython-38.pyc
--rw-r--r--   0        0        0    15599 2023-02-13 12:40:42.498522 droughty-0.9.7/droughty/cube_parser/__pycache__/parser.cpython-38.pyc
--rw-r--r--   0        0        0    16129 2023-02-13 12:40:42.498650 droughty-0.9.7/droughty/cube_parser/__pycache__/simple.cpython-38.pyc
--rw-r--r--   0        0        0     5924 2023-02-13 12:40:42.498739 droughty-0.9.7/droughty/cube_parser/__pycache__/tokens.cpython-38.pyc
--rw-r--r--   0        0        0    17452 2023-02-13 12:40:42.498862 droughty-0.9.7/droughty/cube_parser/__pycache__/tree.cpython-38.pyc
--rw-r--r--   0        0        0      649 2023-02-13 12:40:42.498934 droughty-0.9.7/droughty/cube_parser/__pycache__/utils.cpython-38.pyc
--rw-r--r--   0        0        0     5334 2023-02-13 12:40:42.499016 droughty-0.9.7/droughty/cube_parser/__pycache__/visitors.cpython-38.pyc
--rw-r--r--   0        0        0     3184 2023-02-13 12:40:42.499095 droughty-0.9.7/droughty/cube_parser/cube.py
--rw-r--r--   0        0        0     3186 2023-02-13 12:40:42.499174 droughty-0.9.7/droughty/cube_parser/keys.py
--rw-r--r--   0        0        0     7144 2023-02-13 12:40:42.499260 droughty-0.9.7/droughty/cube_parser/lexer.py
--rw-r--r--   0        0        0    20443 2023-02-13 12:40:42.499381 droughty-0.9.7/droughty/cube_parser/parser.py
--rw-r--r--   0        0        0        0 2023-02-13 12:40:42.499422 droughty-0.9.7/droughty/cube_parser/py.typed
--rw-r--r--   0        0        0    19239 2023-02-13 12:40:42.499564 droughty-0.9.7/droughty/cube_parser/simple.py
--rw-r--r--   0        0        0     3690 2023-02-13 12:40:42.499660 droughty-0.9.7/droughty/cube_parser/tokens.py
--rw-r--r--   0        0        0    12933 2023-02-13 12:40:42.499772 droughty-0.9.7/droughty/cube_parser/tree.py
--rw-r--r--   0        0        0      521 2023-02-13 12:40:42.499845 droughty-0.9.7/droughty/cube_parser/utils.py
--rw-r--r--   0        0        0     3548 2023-02-13 12:40:42.499938 droughty-0.9.7/droughty/cube_parser/visitors.py
--rw-r--r--   0        0        0     7433 2023-02-13 12:40:42.500118 droughty-0.9.7/droughty/droughty_core/__pycache__/config.cpython-38.pyc
--rw-r--r--   0        0        0     1559 2023-02-13 12:40:42.500206 droughty-0.9.7/droughty/droughty_core/__pycache__/config_cli.cpython-38.pyc
--rw-r--r--   0        0        0    15822 2023-02-17 10:58:30.257720 droughty-0.9.7/droughty/droughty_core/__pycache__/warehouse_target.cpython-39.pyc
--rw-r--r--   0        0        0    15915 2023-02-15 13:23:58.574341 droughty-0.9.7/droughty/droughty_core/config.py
--rw-r--r--   0        0        0     3374 2023-02-13 12:40:51.347702 droughty-0.9.7/droughty/droughty_core/config_cli.py
--rw-r--r--   0        0        0    12530 2023-02-14 12:13:23.871899 droughty-0.9.7/droughty/droughty_core/droughty_data_prep.py
--rw-r--r--   0        0        0      705 2023-02-13 12:40:42.500514 droughty-0.9.7/droughty/droughty_core/droughty_init.py
--rw-r--r--   0        0        0    17978 2023-02-17 13:45:30.200794 droughty-0.9.7/droughty/droughty_core/warehouse_target.py
--rw-r--r--   0        0        0     2610 2023-02-13 12:40:42.500784 droughty-0.9.7/droughty/droughty_cube/cube_base_dict.py
--rw-r--r--   0        0        0      865 2023-02-13 12:40:42.500865 droughty-0.9.7/droughty/droughty_cube/cube_cli.py
--rw-r--r--   0        0        0     2384 2023-02-13 12:40:42.500922 droughty-0.9.7/droughty/droughty_cube/cube_explore_dict.py
--rw-r--r--   0        0        0     4246 2023-02-13 12:40:42.501093 droughty-0.9.7/droughty/droughty_cube/cube_explore_module.py
--rw-r--r--   0        0        0     2820 2023-02-13 12:40:42.501181 droughty-0.9.7/droughty/droughty_cube/cube_measure_module.py
--rw-r--r--   0        0        0     3164 2023-02-13 12:40:42.501254 droughty-0.9.7/droughty/droughty_cube/cube_module.py
--rw-r--r--   0        0        0     1665 2023-02-13 12:40:42.501385 droughty-0.9.7/droughty/droughty_dbml/dbml_base_dict.py
--rw-r--r--   0        0        0      253 2023-02-13 12:40:42.501455 droughty-0.9.7/droughty/droughty_dbml/dbml_cli.py
--rw-r--r--   0        0        0     3050 2023-02-13 12:40:42.501544 droughty-0.9.7/droughty/droughty_dbml/dbml_module.py
--rw-r--r--   0        0        0    13855 2023-02-13 12:40:42.501730 droughty-0.9.7/droughty/droughty_dbt/.ipynb_checkpoints/Untitled-checkpoint.ipynb
--rw-r--r--   0        0        0     1728 2023-02-13 12:40:42.501802 droughty-0.9.7/droughty/droughty_dbt/dbt_test_base_dict.py
--rw-r--r--   0        0        0      257 2023-02-13 12:40:42.501865 droughty-0.9.7/droughty/droughty_dbt/dbt_test_cli.py
--rw-r--r--   0        0        0      781 2023-02-13 12:40:42.501932 droughty-0.9.7/droughty/droughty_dbt/dbt_test_field_base.py
--rw-r--r--   0        0        0     5435 2023-02-13 12:40:42.502056 droughty-0.9.7/droughty/droughty_dbt/dbt_test_module.py
--rw-r--r--   0        0        0      439 2023-02-13 12:40:42.502165 droughty-0.9.7/droughty/droughty_docs/docs_cli.py
--rw-r--r--   0        0        0     2721 2023-02-13 12:40:42.502250 droughty-0.9.7/droughty/droughty_docs/openai_descriptions.py
--rw-r--r--   0        0        0      133 2023-02-17 13:43:43.236142 droughty-0.9.7/droughty/droughty_jinjasql/jinjasql/__init__.py
--rw-r--r--   0        0        0     7582 2023-02-17 13:43:43.236849 droughty-0.9.7/droughty/droughty_jinjasql/jinjasql/core.py
--rw-r--r--   0        0        0     2240 2023-02-17 10:58:30.256290 droughty-0.9.7/droughty/droughty_lookml/__pycache__/lookml_base_dict.cpython-39.pyc
--rw-r--r--   0        0        0     1854 2023-02-17 10:30:20.078328 droughty-0.9.7/droughty/droughty_lookml/__pycache__/lookml_cli.cpython-39.pyc
--rw-r--r--   0        0        0     3025 2023-02-17 10:30:20.079420 droughty-0.9.7/droughty/droughty_lookml/__pycache__/lookml_module.cpython-39.pyc
--rw-r--r--   0        0        0     2568 2023-02-13 12:40:42.502360 droughty-0.9.7/droughty/droughty_lookml/lookml_base_dict.py
--rw-r--r--   0        0        0     1670 2023-02-13 12:40:42.502437 droughty-0.9.7/droughty/droughty_lookml/lookml_cli.py
--rw-r--r--   0        0        0     2302 2023-02-13 12:40:42.502497 droughty-0.9.7/droughty/droughty_lookml/lookml_explore_dict.py
--rw-r--r--   0        0        0     3646 2023-02-13 12:40:42.502573 droughty-0.9.7/droughty/droughty_lookml/lookml_explore_module.py
--rw-r--r--   0        0        0     2933 2023-02-13 12:40:42.502649 droughty-0.9.7/droughty/droughty_lookml/lookml_measure_module.py
--rw-r--r--   0        0        0     5070 2023-02-13 12:40:42.502723 droughty-0.9.7/droughty/droughty_lookml/lookml_module.py
--rw-r--r--   0        0        0    25632 2023-02-13 12:40:42.502799 droughty-0.9.7/droughty/droughty_lookml/lookml_pop_module.py
--rw-r--r--   0        0        0    25179 2023-02-13 12:40:42.502906 droughty-0.9.7/droughty/droughty_lookml/lookml_pop_module_snowflake.py
--rw-r--r--   0        0        0     1442 2023-02-14 12:13:56.790408 droughty-0.9.7/droughty/droughty_resolve/resolve_base_dict.py
--rw-r--r--   0        0        0      292 2023-02-13 12:40:51.348128 droughty-0.9.7/droughty/droughty_resolve/resolve_cli.py
--rw-r--r--   0        0        0     2134 2023-02-15 13:23:47.670789 droughty-0.9.7/droughty/droughty_resolve/resolve_module.py
--rw-r--r--   0        0        0     1911 2023-02-13 12:40:51.348323 droughty-0.9.7/droughty/main.py
--rw-r--r--   0        0        0      903 2023-02-17 13:45:51.083073 droughty-0.9.7/pyproject.toml
--rw-r--r--   0        0        0     2885 1970-01-01 00:00:00.000000 droughty-0.9.7/setup.py
--rw-r--r--   0        0        0     2657 1970-01-01 00:00:00.000000 droughty-0.9.7/PKG-INFO
+-rw-r--r--   0        0        0     1283 2023-02-13 12:40:42.477103 droughty-0.9.8/README.md
+-rw-r--r--   0        0        0    13158 2023-02-13 12:40:42.495288 droughty-0.9.8/droughty/.ipynb_checkpoints/Untitled-Copy1-checkpoint.ipynb
+-rw-r--r--   0        0        0       72 2023-02-13 12:40:42.495352 droughty-0.9.8/droughty/.ipynb_checkpoints/Untitled-checkpoint.ipynb
+-rw-r--r--   0        0        0       72 2023-02-13 12:40:42.495414 droughty-0.9.8/droughty/.ipynb_checkpoints/Untitled1-checkpoint.ipynb
+-rw-r--r--   0        0        0        7 2023-02-13 12:40:42.495467 droughty-0.9.8/droughty/.python-version
+-rw-r--r--   0        0        0      133 2023-02-13 12:40:42.495538 droughty-0.9.8/droughty/__init__.py
+-rw-r--r--   0        0        0       70 2023-02-13 12:40:42.498067 droughty-0.9.8/droughty/cube_parser/__main__.py
+-rw-r--r--   0        0        0     3348 2023-02-13 12:40:42.498220 droughty-0.9.8/droughty/cube_parser/__pycache__/cube.cpython-38.pyc
+-rw-r--r--   0        0        0     2214 2023-02-13 12:40:42.498303 droughty-0.9.8/droughty/cube_parser/__pycache__/keys.cpython-38.pyc
+-rw-r--r--   0        0        0     6884 2023-02-13 12:40:42.498395 droughty-0.9.8/droughty/cube_parser/__pycache__/lexer.cpython-38.pyc
+-rw-r--r--   0        0        0    15599 2023-02-13 12:40:42.498522 droughty-0.9.8/droughty/cube_parser/__pycache__/parser.cpython-38.pyc
+-rw-r--r--   0        0        0    16129 2023-02-13 12:40:42.498650 droughty-0.9.8/droughty/cube_parser/__pycache__/simple.cpython-38.pyc
+-rw-r--r--   0        0        0     5924 2023-02-13 12:40:42.498739 droughty-0.9.8/droughty/cube_parser/__pycache__/tokens.cpython-38.pyc
+-rw-r--r--   0        0        0    17452 2023-02-13 12:40:42.498862 droughty-0.9.8/droughty/cube_parser/__pycache__/tree.cpython-38.pyc
+-rw-r--r--   0        0        0      649 2023-02-13 12:40:42.498934 droughty-0.9.8/droughty/cube_parser/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0        0        0     5334 2023-02-13 12:40:42.499016 droughty-0.9.8/droughty/cube_parser/__pycache__/visitors.cpython-38.pyc
+-rw-r--r--   0        0        0     3184 2023-02-13 12:40:42.499095 droughty-0.9.8/droughty/cube_parser/cube.py
+-rw-r--r--   0        0        0     3186 2023-02-13 12:40:42.499174 droughty-0.9.8/droughty/cube_parser/keys.py
+-rw-r--r--   0        0        0     7144 2023-02-13 12:40:42.499260 droughty-0.9.8/droughty/cube_parser/lexer.py
+-rw-r--r--   0        0        0    20443 2023-02-13 12:40:42.499381 droughty-0.9.8/droughty/cube_parser/parser.py
+-rw-r--r--   0        0        0        0 2023-02-13 12:40:42.499422 droughty-0.9.8/droughty/cube_parser/py.typed
+-rw-r--r--   0        0        0    19239 2023-02-13 12:40:42.499564 droughty-0.9.8/droughty/cube_parser/simple.py
+-rw-r--r--   0        0        0     3690 2023-02-13 12:40:42.499660 droughty-0.9.8/droughty/cube_parser/tokens.py
+-rw-r--r--   0        0        0    12933 2023-02-13 12:40:42.499772 droughty-0.9.8/droughty/cube_parser/tree.py
+-rw-r--r--   0        0        0      521 2023-02-13 12:40:42.499845 droughty-0.9.8/droughty/cube_parser/utils.py
+-rw-r--r--   0        0        0     3548 2023-02-13 12:40:42.499938 droughty-0.9.8/droughty/cube_parser/visitors.py
+-rw-r--r--   0        0        0     7433 2023-02-13 12:40:42.500118 droughty-0.9.8/droughty/droughty_core/__pycache__/config.cpython-38.pyc
+-rw-r--r--   0        0        0     1559 2023-02-13 12:40:42.500206 droughty-0.9.8/droughty/droughty_core/__pycache__/config_cli.cpython-38.pyc
+-rw-r--r--   0        0        0    15822 2023-02-17 10:58:30.257720 droughty-0.9.8/droughty/droughty_core/__pycache__/warehouse_target.cpython-39.pyc
+-rw-r--r--   0        0        0    15915 2023-02-15 13:23:58.574341 droughty-0.9.8/droughty/droughty_core/config.py
+-rw-r--r--   0        0        0     3374 2023-02-13 12:40:51.347702 droughty-0.9.8/droughty/droughty_core/config_cli.py
+-rw-r--r--   0        0        0    12530 2023-02-14 12:13:23.871899 droughty-0.9.8/droughty/droughty_core/droughty_data_prep.py
+-rw-r--r--   0        0        0      705 2023-02-13 12:40:42.500514 droughty-0.9.8/droughty/droughty_core/droughty_init.py
+-rw-r--r--   0        0        0    17979 2023-02-17 14:32:20.049047 droughty-0.9.8/droughty/droughty_core/warehouse_target.py
+-rw-r--r--   0        0        0     2610 2023-02-13 12:40:42.500784 droughty-0.9.8/droughty/droughty_cube/cube_base_dict.py
+-rw-r--r--   0        0        0      865 2023-02-13 12:40:42.500865 droughty-0.9.8/droughty/droughty_cube/cube_cli.py
+-rw-r--r--   0        0        0     2384 2023-02-13 12:40:42.500922 droughty-0.9.8/droughty/droughty_cube/cube_explore_dict.py
+-rw-r--r--   0        0        0     4246 2023-02-13 12:40:42.501093 droughty-0.9.8/droughty/droughty_cube/cube_explore_module.py
+-rw-r--r--   0        0        0     2820 2023-02-13 12:40:42.501181 droughty-0.9.8/droughty/droughty_cube/cube_measure_module.py
+-rw-r--r--   0        0        0     3164 2023-02-13 12:40:42.501254 droughty-0.9.8/droughty/droughty_cube/cube_module.py
+-rw-r--r--   0        0        0     1665 2023-02-13 12:40:42.501385 droughty-0.9.8/droughty/droughty_dbml/dbml_base_dict.py
+-rw-r--r--   0        0        0      253 2023-02-13 12:40:42.501455 droughty-0.9.8/droughty/droughty_dbml/dbml_cli.py
+-rw-r--r--   0        0        0     3050 2023-02-13 12:40:42.501544 droughty-0.9.8/droughty/droughty_dbml/dbml_module.py
+-rw-r--r--   0        0        0    13855 2023-02-13 12:40:42.501730 droughty-0.9.8/droughty/droughty_dbt/.ipynb_checkpoints/Untitled-checkpoint.ipynb
+-rw-r--r--   0        0        0     1728 2023-02-13 12:40:42.501802 droughty-0.9.8/droughty/droughty_dbt/dbt_test_base_dict.py
+-rw-r--r--   0        0        0      257 2023-02-13 12:40:42.501865 droughty-0.9.8/droughty/droughty_dbt/dbt_test_cli.py
+-rw-r--r--   0        0        0      781 2023-02-13 12:40:42.501932 droughty-0.9.8/droughty/droughty_dbt/dbt_test_field_base.py
+-rw-r--r--   0        0        0     5435 2023-02-13 12:40:42.502056 droughty-0.9.8/droughty/droughty_dbt/dbt_test_module.py
+-rw-r--r--   0        0        0      439 2023-02-13 12:40:42.502165 droughty-0.9.8/droughty/droughty_docs/docs_cli.py
+-rw-r--r--   0        0        0     2721 2023-02-13 12:40:42.502250 droughty-0.9.8/droughty/droughty_docs/openai_descriptions.py
+-rw-r--r--   0        0        0      133 2023-02-17 14:32:48.712534 droughty-0.9.8/droughty/droughty_jinjasql/jinjasql/__init__
+-rw-r--r--   0        0        0     7582 2023-02-17 13:43:43.236849 droughty-0.9.8/droughty/droughty_jinjasql/jinjasql/core.py
+-rw-r--r--   0        0        0     2240 2023-02-17 10:58:30.256290 droughty-0.9.8/droughty/droughty_lookml/__pycache__/lookml_base_dict.cpython-39.pyc
+-rw-r--r--   0        0        0     1854 2023-02-17 10:30:20.078328 droughty-0.9.8/droughty/droughty_lookml/__pycache__/lookml_cli.cpython-39.pyc
+-rw-r--r--   0        0        0     3025 2023-02-17 10:30:20.079420 droughty-0.9.8/droughty/droughty_lookml/__pycache__/lookml_module.cpython-39.pyc
+-rw-r--r--   0        0        0     2568 2023-02-13 12:40:42.502360 droughty-0.9.8/droughty/droughty_lookml/lookml_base_dict.py
+-rw-r--r--   0        0        0     1670 2023-02-13 12:40:42.502437 droughty-0.9.8/droughty/droughty_lookml/lookml_cli.py
+-rw-r--r--   0        0        0     2302 2023-02-13 12:40:42.502497 droughty-0.9.8/droughty/droughty_lookml/lookml_explore_dict.py
+-rw-r--r--   0        0        0     3646 2023-02-13 12:40:42.502573 droughty-0.9.8/droughty/droughty_lookml/lookml_explore_module.py
+-rw-r--r--   0        0        0     2933 2023-02-13 12:40:42.502649 droughty-0.9.8/droughty/droughty_lookml/lookml_measure_module.py
+-rw-r--r--   0        0        0     5070 2023-02-13 12:40:42.502723 droughty-0.9.8/droughty/droughty_lookml/lookml_module.py
+-rw-r--r--   0        0        0    25632 2023-02-13 12:40:42.502799 droughty-0.9.8/droughty/droughty_lookml/lookml_pop_module.py
+-rw-r--r--   0        0        0    25179 2023-02-13 12:40:42.502906 droughty-0.9.8/droughty/droughty_lookml/lookml_pop_module_snowflake.py
+-rw-r--r--   0        0        0     1442 2023-02-14 12:13:56.790408 droughty-0.9.8/droughty/droughty_resolve/resolve_base_dict.py
+-rw-r--r--   0        0        0      292 2023-02-13 12:40:51.348128 droughty-0.9.8/droughty/droughty_resolve/resolve_cli.py
+-rw-r--r--   0        0        0     2134 2023-02-15 13:23:47.670789 droughty-0.9.8/droughty/droughty_resolve/resolve_module.py
+-rw-r--r--   0        0        0     1911 2023-02-13 12:40:51.348323 droughty-0.9.8/droughty/main.py
+-rw-r--r--   0        0        0      908 2023-02-17 14:33:54.976388 droughty-0.9.8/pyproject.toml
+-rw-r--r--   0        0        0     2888 1970-01-01 00:00:00.000000 droughty-0.9.8/setup.py
+-rw-r--r--   0        0        0     2660 1970-01-01 00:00:00.000000 droughty-0.9.8/PKG-INFO
```

### Comparing `droughty-0.9.7/README.md` & `droughty-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/.ipynb_checkpoints/Untitled-Copy1-checkpoint.ipynb` & `droughty-0.9.8/droughty/.ipynb_checkpoints/Untitled-Copy1-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/cube_parser/__pycache__/cube.cpython-38.pyc` & `droughty-0.9.8/droughty/cube_parser/__pycache__/cube.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/cube_parser/__pycache__/keys.cpython-38.pyc` & `droughty-0.9.8/droughty/cube_parser/__pycache__/keys.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/cube_parser/__pycache__/lexer.cpython-38.pyc` & `droughty-0.9.8/droughty/cube_parser/__pycache__/lexer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/cube_parser/__pycache__/parser.cpython-38.pyc` & `droughty-0.9.8/droughty/cube_parser/__pycache__/parser.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/cube_parser/__pycache__/simple.cpython-38.pyc` & `droughty-0.9.8/droughty/cube_parser/__pycache__/simple.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/cube_parser/__pycache__/tokens.cpython-38.pyc` & `droughty-0.9.8/droughty/cube_parser/__pycache__/tokens.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/cube_parser/__pycache__/tree.cpython-38.pyc` & `droughty-0.9.8/droughty/cube_parser/__pycache__/tree.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/cube_parser/__pycache__/utils.cpython-38.pyc` & `droughty-0.9.8/droughty/cube_parser/__pycache__/utils.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/cube_parser/__pycache__/visitors.cpython-38.pyc` & `droughty-0.9.8/droughty/cube_parser/__pycache__/visitors.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/cube_parser/cube.py` & `droughty-0.9.8/droughty/cube_parser/cube.py`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/cube_parser/keys.py` & `droughty-0.9.8/droughty/cube_parser/keys.py`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/cube_parser/lexer.py` & `droughty-0.9.8/droughty/cube_parser/lexer.py`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/cube_parser/parser.py` & `droughty-0.9.8/droughty/cube_parser/parser.py`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/cube_parser/simple.py` & `droughty-0.9.8/droughty/cube_parser/simple.py`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/cube_parser/tokens.py` & `droughty-0.9.8/droughty/cube_parser/tokens.py`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/cube_parser/tree.py` & `droughty-0.9.8/droughty/cube_parser/tree.py`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/cube_parser/utils.py` & `droughty-0.9.8/droughty/cube_parser/utils.py`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/cube_parser/visitors.py` & `droughty-0.9.8/droughty/cube_parser/visitors.py`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/droughty_core/__pycache__/config.cpython-38.pyc` & `droughty-0.9.8/droughty/droughty_core/__pycache__/config.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/droughty_core/__pycache__/config_cli.cpython-38.pyc` & `droughty-0.9.8/droughty/droughty_core/__pycache__/config_cli.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/droughty_core/__pycache__/warehouse_target.cpython-39.pyc` & `droughty-0.9.8/droughty/droughty_core/__pycache__/warehouse_target.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/droughty_core/config.py` & `droughty-0.9.8/droughty/droughty_core/config.py`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/droughty_core/config_cli.py` & `droughty-0.9.8/droughty/droughty_core/config_cli.py`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/droughty_core/droughty_data_prep.py` & `droughty-0.9.8/droughty/droughty_core/droughty_data_prep.py`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/droughty_core/droughty_init.py` & `droughty-0.9.8/droughty/droughty_core/droughty_init.py`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/droughty_core/warehouse_target.py` & `droughty-0.9.8/droughty/droughty_core/warehouse_target.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import yaml
 
 from google.oauth2 import service_account
 import os
 import yaml
 import git
 
-from droughty.droughty_jinjasql.jinjasql.core import JinjaSql
+from droughty.droughty_jinjasql.jinjasql.core import JinjaSql 
 
 from six import string_types
 from copy import deepcopy
 
 from droughty.droughty_core.config import ProjectVariables,ExploresVariables
 
 # resolution warehouse schema
```

### Comparing `droughty-0.9.7/droughty/droughty_cube/cube_base_dict.py` & `droughty-0.9.8/droughty/droughty_cube/cube_base_dict.py`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/droughty_cube/cube_cli.py` & `droughty-0.9.8/droughty/droughty_cube/cube_cli.py`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/droughty_cube/cube_explore_dict.py` & `droughty-0.9.8/droughty/droughty_cube/cube_explore_dict.py`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/droughty_cube/cube_explore_module.py` & `droughty-0.9.8/droughty/droughty_cube/cube_explore_module.py`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/droughty_cube/cube_measure_module.py` & `droughty-0.9.8/droughty/droughty_cube/cube_measure_module.py`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/droughty_cube/cube_module.py` & `droughty-0.9.8/droughty/droughty_cube/cube_module.py`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/droughty_dbml/dbml_base_dict.py` & `droughty-0.9.8/droughty/droughty_dbml/dbml_base_dict.py`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/droughty_dbml/dbml_module.py` & `droughty-0.9.8/droughty/droughty_dbml/dbml_module.py`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/droughty_dbt/.ipynb_checkpoints/Untitled-checkpoint.ipynb` & `droughty-0.9.8/droughty/droughty_dbt/.ipynb_checkpoints/Untitled-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/droughty_dbt/dbt_test_base_dict.py` & `droughty-0.9.8/droughty/droughty_dbt/dbt_test_base_dict.py`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/droughty_dbt/dbt_test_field_base.py` & `droughty-0.9.8/droughty/droughty_dbt/dbt_test_field_base.py`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/droughty_dbt/dbt_test_module.py` & `droughty-0.9.8/droughty/droughty_dbt/dbt_test_module.py`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/droughty_docs/openai_descriptions.py` & `droughty-0.9.8/droughty/droughty_docs/openai_descriptions.py`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/droughty_jinjasql/jinjasql/core.py` & `droughty-0.9.8/droughty/droughty_jinjasql/jinjasql/core.py`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/droughty_lookml/__pycache__/lookml_base_dict.cpython-39.pyc` & `droughty-0.9.8/droughty/droughty_lookml/__pycache__/lookml_base_dict.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/droughty_lookml/__pycache__/lookml_cli.cpython-39.pyc` & `droughty-0.9.8/droughty/droughty_lookml/__pycache__/lookml_cli.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/droughty_lookml/__pycache__/lookml_module.cpython-39.pyc` & `droughty-0.9.8/droughty/droughty_lookml/__pycache__/lookml_module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/droughty_lookml/lookml_base_dict.py` & `droughty-0.9.8/droughty/droughty_lookml/lookml_base_dict.py`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/droughty_lookml/lookml_cli.py` & `droughty-0.9.8/droughty/droughty_lookml/lookml_cli.py`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/droughty_lookml/lookml_explore_dict.py` & `droughty-0.9.8/droughty/droughty_lookml/lookml_explore_dict.py`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/droughty_lookml/lookml_explore_module.py` & `droughty-0.9.8/droughty/droughty_lookml/lookml_explore_module.py`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/droughty_lookml/lookml_measure_module.py` & `droughty-0.9.8/droughty/droughty_lookml/lookml_measure_module.py`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/droughty_lookml/lookml_module.py` & `droughty-0.9.8/droughty/droughty_lookml/lookml_module.py`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/droughty_lookml/lookml_pop_module.py` & `droughty-0.9.8/droughty/droughty_lookml/lookml_pop_module.py`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/droughty_lookml/lookml_pop_module_snowflake.py` & `droughty-0.9.8/droughty/droughty_lookml/lookml_pop_module_snowflake.py`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/droughty_resolve/resolve_base_dict.py` & `droughty-0.9.8/droughty/droughty_resolve/resolve_base_dict.py`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/droughty_resolve/resolve_module.py` & `droughty-0.9.8/droughty/droughty_resolve/resolve_module.py`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/droughty/main.py` & `droughty-0.9.8/droughty/main.py`

 * *Files identical despite different names*

### Comparing `droughty-0.9.7/pyproject.toml` & `droughty-0.9.8/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [tool.poetry]
 name = "droughty"
-version = "0.9.7"
+version = "0.9.8"
 description = "droughty is an analytics engineering toolkit, helping keep your workflow dry."
 authors = ["Lewis <lewischarlesbaker@gmail.com>"]
 license = "MIT"
 repository = 'https://github.com/lewischarlesbaker/droughty'
 readme = 'README.md'
 
 [tool.poetry.dependencies]
@@ -15,15 +15,15 @@
 lkml = "1.3.1"
 Markdown = "3.4.1"
 numpy = "1.24.2"
 openai = "0.26.5"
 pandas = "1.5.3"
 pandas_dedupe = "1.5.0"
 pandas_gbq = "0.19.1"
-protobuf = "4.22.0"
+protobuf = ">=3.13.0,<4"
 PyYAML = "6.0"
 six = "1.16.0"
 ruamel-yaml = "0.17.21"
 snowflake-connector-python = "^3.0.0"
 sqlalchemy = ">=1.4.0,<2.0.0"
 snowflake-sqlalchemy = "^1.4.6"
 pyarrow = "10.0.1"
```

### Comparing `droughty-0.9.7/setup.py` & `droughty-0.9.8/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,28 +26,28 @@
  'jinja2>=3.1.2,<4.0.0',
  'lkml==1.3.1',
  'numpy==1.24.2',
  'openai==0.26.5',
  'pandas==1.5.3',
  'pandas_dedupe==1.5.0',
  'pandas_gbq==0.19.1',
- 'protobuf==4.22.0',
+ 'protobuf>=3.13.0,<4',
  'pyarrow==10.0.1',
  'ruamel-yaml==0.17.21',
  'six==1.16.0',
  'snowflake-connector-python>=3.0.0,<4.0.0',
  'snowflake-sqlalchemy>=1.4.6,<2.0.0',
  'sqlalchemy>=1.4.0,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['droughty = droughty.main:start']}
 
 setup_kwargs = {
     'name': 'droughty',
-    'version': '0.9.7',
+    'version': '0.9.8',
     'description': 'droughty is an analytics engineering toolkit, helping keep your workflow dry.',
     'long_description': '\\#\\#\\#\\# droughty. \\#\\# adjective, drought·i·er, drought·i·est. \\#\\#\ndry.\n\nDroughty helps keep your workflow *ah hem* dry\n\n------------------------------------------------------------------------\n\n**What is droughty?**\n\ndroughty is an analytics engineering toolkit. It takes warehouse\nmetadata and outputs semantic files.\n\nCurrent tools and supported platforms are:\n\n-   lookml - generates a lkml with views, explores and measures from a\n    warehouse schema\n-   dbt - generates a base schema from specified warehouse schemas.\n    Includes standard testing routines\n-   dbml - generates an ERD based on the warehouse layer of your\n    warehouse. Includes pk, fk relationships\n-   cube - generates a cube schema including dimensions, integrations\n    and meassures\n\nThe purpose of this project is to automate the repetitive, dull elements\nof analytics engineering in the modern data stack. It turns out this\nalso leads to cleaner projects, less human error and increases the\nlikelihood of the basics getting done\\...\n\n**Documentation**\n\nInstallation, configuration and usage documentation can be found on\n[ReadTheDocs](https://droughty.readthedocs.io/en/latest/)\n\n**Installation**\n\ndroughty is available through [pip](https://pypi.org/project/droughty):\n\n    pip install droughty\n',
     'author': 'Lewis',
     'author_email': 'lewischarlesbaker@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/lewischarlesbaker/droughty',
```

### Comparing `droughty-0.9.7/PKG-INFO` & `droughty-0.9.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: droughty
-Version: 0.9.7
+Version: 0.9.8
 Summary: droughty is an analytics engineering toolkit, helping keep your workflow dry.
 Home-page: https://github.com/lewischarlesbaker/droughty
 License: MIT
 Author: Lewis
 Author-email: lewischarlesbaker@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -20,15 +20,15 @@
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: lkml (==1.3.1)
 Requires-Dist: numpy (==1.24.2)
 Requires-Dist: openai (==0.26.5)
 Requires-Dist: pandas (==1.5.3)
 Requires-Dist: pandas_dedupe (==1.5.0)
 Requires-Dist: pandas_gbq (==0.19.1)
-Requires-Dist: protobuf (==4.22.0)
+Requires-Dist: protobuf (>=3.13.0,<4)
 Requires-Dist: pyarrow (==10.0.1)
 Requires-Dist: ruamel-yaml (==0.17.21)
 Requires-Dist: six (==1.16.0)
 Requires-Dist: snowflake-connector-python (>=3.0.0,<4.0.0)
 Requires-Dist: snowflake-sqlalchemy (>=1.4.6,<2.0.0)
 Requires-Dist: sqlalchemy (>=1.4.0,<2.0.0)
 Project-URL: Repository, https://github.com/lewischarlesbaker/droughty
```

